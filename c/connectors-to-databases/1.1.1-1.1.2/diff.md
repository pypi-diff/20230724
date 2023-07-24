# Comparing `tmp/connectors_to_databases-1.1.1.tar.gz` & `tmp/connectors_to_databases-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectors_to_databases-1.1.1.tar", last modified: Mon Jul 24 02:08:45 2023, max compression
+gzip compressed data, was "connectors_to_databases-1.1.2.tar", last modified: Mon Jul 24 14:04:17 2023, max compression
```

## Comparing `connectors_to_databases-1.1.1.tar` & `connectors_to_databases-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 02:08:45.676911 connectors_to_databases-1.1.1/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.1.1/LICENSE.MD
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-24 02:08:45.676700 connectors_to_databases-1.1.1/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1280 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.1/README.md
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 02:08:45.675367 connectors_to_databases-1.1.1/connectors_to_databases/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.1/connectors_to_databases/BaseOperator.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1161 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.1/connectors_to_databases/ClickHouse.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     7957 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.1/connectors_to_databases/PostgreSQL.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.1.1/connectors_to_databases/TypeHinting.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      346 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.1/connectors_to_databases/__init__.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      132 2023-07-17 09:59:52.000000 connectors_to_databases-1.1.1/connectors_to_databases/class_use.py
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 02:08:45.676454 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/SOURCES.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/dependency_links.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      124 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/requires.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/top_level.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.1/pyproject.toml
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-24 02:08:45.676965 connectors_to_databases-1.1.1/setup.cfg
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1762 2023-07-24 02:08:12.000000 connectors_to_databases-1.1.1/setup.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 14:04:17.673750 connectors_to_databases-1.1.2/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.1.2/LICENSE.MD
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-24 14:04:17.673497 connectors_to_databases-1.1.2/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1280 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.2/README.md
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 14:04:17.671578 connectors_to_databases-1.1.2/connectors_to_databases/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.2/connectors_to_databases/BaseOperator.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1225 2023-07-24 13:58:53.000000 connectors_to_databases-1.1.2/connectors_to_databases/ClickHouse.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     7958 2023-07-24 13:55:54.000000 connectors_to_databases-1.1.2/connectors_to_databases/PostgreSQL.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.1.2/connectors_to_databases/TypeHinting.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      346 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.2/connectors_to_databases/__init__.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      512 2023-07-24 13:58:53.000000 connectors_to_databases-1.1.2/connectors_to_databases/class_use.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 14:04:17.673123 connectors_to_databases-1.1.2/connectors_to_databases.egg-info/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-24 14:04:17.000000 connectors_to_databases-1.1.2/connectors_to_databases.egg-info/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-24 14:04:17.000000 connectors_to_databases-1.1.2/connectors_to_databases.egg-info/SOURCES.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-24 14:04:17.000000 connectors_to_databases-1.1.2/connectors_to_databases.egg-info/dependency_links.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      124 2023-07-24 14:04:17.000000 connectors_to_databases-1.1.2/connectors_to_databases.egg-info/requires.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-24 14:04:17.000000 connectors_to_databases-1.1.2/connectors_to_databases.egg-info/top_level.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.2/pyproject.toml
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-24 14:04:17.673822 connectors_to_databases-1.1.2/setup.cfg
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1762 2023-07-24 14:03:50.000000 connectors_to_databases-1.1.2/setup.py
```

### Comparing `connectors_to_databases-1.1.1/LICENSE.MD` & `connectors_to_databases-1.1.2/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.1/PKG-INFO` & `connectors_to_databases-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectors_to_databases
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python module for connect with PostgreSQL and ClickHouse 
 Home-page: https://github.com/k0rsakov/connectors_to_databases
 Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 Author: k0rsakov
 Author-email: korsakov.iyu@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
```

### Comparing `connectors_to_databases-1.1.1/README.md` & `connectors_to_databases-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.1/connectors_to_databases/BaseOperator.py` & `connectors_to_databases-1.1.2/connectors_to_databases/BaseOperator.py`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.1/connectors_to_databases/ClickHouse.py` & `connectors_to_databases-1.1.2/connectors_to_databases/ClickHouse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from urllib.parse import quote
 
 from sqlalchemy import create_engine, engine
 
-from .BaseOperator import BaseOperator
+# from .BaseOperator import BaseOperator
+from connectors_to_databases.BaseOperator import BaseOperator
 
 # TODO: Change sqlalchemy to clickhouse-driver
 
 class ClickHouse(BaseOperator):
     """
     Connector to PostgreSQL database
     """
```

### Comparing `connectors_to_databases-1.1.1/connectors_to_databases/PostgreSQL.py` & `connectors_to_databases-1.1.2/connectors_to_databases/PostgreSQL.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # from .BaseOperator import BaseOperator
 from connectors_to_databases.BaseOperator import BaseOperator
 from urllib.parse import quote
-from typing import Union, Iterable
+from typing import Iterable
 
 from sqlalchemy import create_engine, engine
 
 
 class PostgreSQL(BaseOperator):
     """
     Connector to PostgreSQL database
@@ -88,15 +88,15 @@
     def generate_on_conflict_sql_query(
             cls,
             source_table_schema_name: str = 'public',
             source_table_name: str = None, # noqa: RUF013
             target_table_schema_name: str = 'public',
             target_table_name: str = None, # noqa: RUF013
             list_columns: Iterable[str] = None, # noqa: RUF013
-            pk: Union[str, list] = 'id',
+            pk: str | list[str, ...] = 'id',
             replace: bool = False,
     ) -> str:
         """
         **Function: generate_on_conflict_sql_query**
 
         This class method generates an SQL query for performing data insertion with conflict handling using a
         specified primary key.
@@ -105,15 +105,15 @@
         - `source_table_schema_name` (str, optional): The schema name of the source table. Defaults to `'public'`.
         - `source_table_name` (str): The name of the source table from which data will be inserted.
         - `target_table_schema_name` (str, optional): The schema name of the target table where data will be inserted.
             Defaults to `'public'`.
         - `target_table_name` (str): The name of the target table where data will be inserted.
         - `list_columns` (Iterable[str], optional): An iterable object containing the names of columns to be inserted.
             If not specified, all columns from the source table will be inserted.
-        - `pk` (Union[str, list]): The primary key for checking insertion conflicts. It can be a string representing
+        - `pk` (str | list[str, ...]): The primary key for checking insertion conflicts. It can be a string representing
             a single column name or a list of column names.
         - `replace` (bool): A flag indicating whether to replace existing data in case of conflicts. Defaults to
             `False`, which means conflicts will be ignored and nothing will be done.
 
         **Return:**
         - `str`: The generated SQL query for data insertion with conflict handling.
```

### Comparing `connectors_to_databases-1.1.1/connectors_to_databases.egg-info/PKG-INFO` & `connectors_to_databases-1.1.2/connectors_to_databases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectors-to-databases
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python module for connect with PostgreSQL and ClickHouse 
 Home-page: https://github.com/k0rsakov/connectors_to_databases
 Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 Author: k0rsakov
 Author-email: korsakov.iyu@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
```

### Comparing `connectors_to_databases-1.1.1/pyproject.toml` & `connectors_to_databases-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.1/setup.py` & `connectors_to_databases-1.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '1.1.1'
+version = '1.1.2'
 
 with open('README.md', encoding='utf-8-sig') as f:
     long_description = f.read()
 
 setup(
     name='connectors_to_databases',
     version=version,
```

