# Comparing `tmp/pg_alchemy_kit-0.1.2.tar.gz` & `tmp/pg_alchemy_kit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_alchemy_kit-0.1.2.tar", max compression
+gzip compressed data, was "pg_alchemy_kit-0.1.4.tar", max compression
```

## Comparing `pg_alchemy_kit-0.1.2.tar` & `pg_alchemy_kit-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685538 pg_alchemy_kit-0.1.2/README.md
--rw-r--r--   0        0        0     2380 2023-07-23 04:59:06.899758 pg_alchemy_kit-0.1.2/pg_alchemy_kit/PG.py
--rw-r--r--   0        0        0     5575 2023-07-23 04:50:57.872766 pg_alchemy_kit-0.1.2/pg_alchemy_kit/PGUtils.py
--rw-r--r--   0        0        0      138 2023-07-23 04:57:39.246037 pg_alchemy_kit-0.1.2/pg_alchemy_kit/__init__.py
--rw-r--r--   0        0        0      438 2023-07-23 05:06:05.824682 pg_alchemy_kit-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685000 pg_alchemy_kit-0.1.4/README.md
+-rw-r--r--   0        0        0     2315 2023-07-24 18:38:24.966281 pg_alchemy_kit-0.1.4/pg_alchemy_kit/PG.py
+-rw-r--r--   0        0        0     6073 2023-07-24 18:39:48.162003 pg_alchemy_kit-0.1.4/pg_alchemy_kit/PGUtils.py
+-rw-r--r--   0        0        0      138 2023-07-23 04:57:39.246000 pg_alchemy_kit-0.1.4/pg_alchemy_kit/__init__.py
+-rw-r--r--   0        0        0      496 2023-07-24 18:45:21.557415 pg_alchemy_kit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5850 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.1.4/PKG-INFO
```

### Comparing `pg_alchemy_kit-0.1.2/README.md` & `pg_alchemy_kit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.1.2/pg_alchemy_kit/PG.py` & `pg_alchemy_kit-0.1.4/pg_alchemy_kit/PG.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from sqlalchemy.orm import sessionmaker, scoped_session
 from sqlalchemy.orm import DeclarativeMeta
 import sqlalchemy
 import logging
 from contextlib import contextmanager
 from typing import List, Iterator
 
+
 class PG:
     def initialize(cls, url: str = None, logger: logging.Logger = None, **kwargs):
         url = url or get_engine_url()
         cls.engine: Engine = get_engine(url, **kwargs)
         cls.SessionLocal = sessionmaker(
             autocommit=False, autoflush=False, bind=cls.engine
         )
@@ -21,15 +22,14 @@
         cls.logger = logger
 
         if cls.logger is None:
             logger = logging.getLogger(__name__)
             logger.setLevel(logging.INFO)
             logger.addHandler(logging.StreamHandler())
             cls.logger = logger
-            # cls.logger = logging.getLogger("uvicorn.error")
 
         cls.utils = PGUtils(cls.logger)
 
         cls.logger.info("Initialized PG")
 
     def create_tables(
         cls, Bases: List[DeclarativeMeta], schemas: List[str] = ["public"]
@@ -47,15 +47,14 @@
             try:
                 if schema not in cls.inspector.get_schema_names():
                     cls.engine.execute(sqlalchemy.schema.CreateSchema(schema))
                 Base.metadata.create_all(cls.engine)
             except Exception as e:
                 cls.logger.info(f"Error in create_tables: {e}")
 
-    
     @contextmanager
     def get_session_ctx(cls) -> Iterator[Session]:
         with cls.SessionLocal() as session:
             try:
                 yield session
             finally:
                 session.close()
@@ -69,8 +68,9 @@
 
     def get_session_scoped(cls) -> scoped_session:
         return scoped_session(cls.SessionLocal)
 
     def close(cls):
         cls.engine.dispose()
 
+
 db = PG()
```

### Comparing `pg_alchemy_kit-0.1.2/pg_alchemy_kit/PGUtils.py` & `pg_alchemy_kit-0.1.4/pg_alchemy_kit/PGUtils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-
-
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.orm.session import Session
 from sqlalchemy import create_engine, text
 from sqlalchemy.engine.base import Engine
 import logging
 from typing import Any, List, Union
 import uuid
 import os
 
+
 class PGUtils:
     def __init__(cls, logger: logging.Logger):
         cls.session = None
         cls.logger = logger
 
     def initialize(cls, session: Session):
         cls.session = session
 
     @staticmethod
     def wrap_to_json(stmt: str) -> text:
         stmt = stmt.replace(";", "")
         return text(f"SELECT json_agg(t) FROM ({stmt}) t")
 
-    def select(cls, session: Session, sql: str, params: dict = {}) -> Union[List[dict], None]:
+    def select(
+        cls, session: Session, sql: str, params: dict = {}
+    ) -> Union[List[dict], None]:
         try:
             stmt: text = cls.wrap_to_json(sql)
             results = session.execute(stmt, params=params).fetchone()[0]
             if results is None:
                 return []
 
             return results
@@ -121,17 +122,15 @@
         session: Session,
         model: Any,
         records: List[dict],
     ):
         for record in records:
             cls.insert_orm(session, model, record)
 
-    def delete_orm(
-        cls, session: Session, model: Any, records: List[uuid.UUID]
-    ) -> bool:
+    def delete_orm(cls, session: Session, model: Any, records: List[uuid.UUID]) -> bool:
         try:
             session.query(model).filter(model.uuid.in_(records)).delete(
                 synchronize_session=False
             )
             session.commit()
             cls.logger.info(f"Deleted {len(records)} records")
             return True
@@ -155,21 +154,34 @@
         except Exception as e:
             cls.logger.info(f"Error in get_uuid: {e}")
             return None
 
 
 def get_engine(url: str, **kwargs) -> Engine:
     try:
-        return create_engine(url, **kwargs)
+        pool_size = kwargs.get("pool_size", 5)
+        max_overflow = kwargs.get("max_overflow", 0)
+        pool_pre_ping = kwargs.get("pool_pre_ping", True)
+        return create_engine(
+            url,
+            pool_size=pool_size,
+            max_overflow=max_overflow,
+            pool_pre_ping=pool_pre_ping,
+            **kwargs,
+        )
     except DBAPIError as e:
         raise e
 
 
+def get_engine_url(
+    connection_type: str = "postgresql", settings: Any = None, **kwargs
+) -> str:
+    if settings is not None:
+        return f"{connection_type}://{settings.pg_username}:{settings.pg_password}@{settings.pg_host}:{settings.pg_port}/{settings.pg_db}"
 
-def get_engine_url(connection_type: str = "postgresql", **kwargs) -> str:
     username = kwargs.get("pg_username", os.environ.get("PG_USERNAME"))
     password = kwargs.get("pg_password", os.environ.get("PG_PASSWORD"))
     host = kwargs.get("pg_host", os.environ.get("PG_HOST"))
     port = kwargs.get("pg_port", os.environ.get("PG_PORT"))
     db = kwargs.get("pg_db", os.environ.get("PG_DB"))
-    
-    return f"{connection_type}://{username}:{password}@{host}:{port}/{db}"
+
+    return f"{connection_type}://{username}:{password}@{host}:{port}/{db}"
```

### Comparing `pg_alchemy_kit-0.1.2/PKG-INFO` & `pg_alchemy_kit-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pg-alchemy-kit
-Version: 0.1.2
+Version: 0.1.4
 Summary: A simple wrapper around sqlalchemy to make it easier to use with postgresql
+Home-page: https://github.com/jsaied99/pg-alchemy-kit
 Author: jsaied99
 Author-email: jsaied99@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
+Project-URL: Repository, https://github.com/jsaied99/pg-alchemy-kit
 Description-Content-Type: text/markdown
 
 # Documentation for `PG` Library
 
 ## Introduction
 The `PG` library offers a suite of utilities to manage and interact with PostgreSQL databases using SQLAlchemy. It provides functionality such as initializing the database engine, creating tables, and managing sessions.
```

