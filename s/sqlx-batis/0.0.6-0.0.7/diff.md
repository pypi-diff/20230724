# Comparing `tmp/sqlx-batis-0.0.6.tar.gz` & `tmp/sqlx-batis-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.0.6.tar", last modified: Sun Jul 23 14:10:43 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.0.7.tar", last modified: Mon Jul 24 01:45:01 2023, max compression
```

## Comparing `sqlx-batis-0.0.6.tar` & `sqlx-batis-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/
--rw-rw-rw-   0        0        0     3427 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2023-07-23 14:10:39.000000 sqlx-batis-0.0.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-23 14:10:39.000000 sqlx-batis-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/sqlbatis/
--rw-rw-rw-   0        0        0      387 2023-07-23 13:58:19.000000 sqlx-batis-0.0.6/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8258 2023-07-23 13:56:11.000000 sqlx-batis-0.0.6/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6472 2023-07-23 13:59:13.000000 sqlx-batis-0.0.6/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0      800 2023-07-23 14:05:59.000000 sqlx-batis-0.0.6/sqlbatis/exec_support.py
--rw-rw-rw-   0        0        0     3875 2023-07-22 21:17:32.000000 sqlx-batis-0.0.6/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38549 2023-07-23 14:00:47.000000 sqlx-batis-0.0.6/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2399 2023-07-22 21:14:39.000000 sqlx-batis-0.0.6/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7056 2023-07-22 18:30:15.000000 sqlx-batis-0.0.6/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     4120 2023-07-22 18:31:21.000000 sqlx-batis-0.0.6/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1421 2023-07-23 14:00:47.000000 sqlx-batis-0.0.6/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      287 2023-07-23 13:34:34.000000 sqlx-batis-0.0.6/sqlbatis/support.py
--rw-rw-rw-   0        0        0      154 2023-07-23 13:54:14.000000 sqlx-batis-0.0.6/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-22 02:18:23.000000 sqlx-batis-0.0.6/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3427 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      471 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-23 14:10:43.000000 sqlx-batis-0.0.6/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/
+-rw-rw-rw-   0        0        0     3427 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2023-07-23 14:10:39.000000 sqlx-batis-0.0.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-23 23:35:52.000000 sqlx-batis-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlbatis/
+-rw-rw-rw-   0        0        0      394 2023-07-23 23:51:01.000000 sqlx-batis-0.0.7/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8455 2023-07-23 23:23:36.000000 sqlx-batis-0.0.7/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6538 2023-07-23 23:33:37.000000 sqlx-batis-0.0.7/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0      806 2023-07-23 23:51:27.000000 sqlx-batis-0.0.7/sqlbatis/exec_support.py
+-rw-rw-rw-   0        0        0     3875 2023-07-22 21:17:32.000000 sqlx-batis-0.0.7/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38662 2023-07-23 23:51:00.000000 sqlx-batis-0.0.7/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-07-23 22:35:05.000000 sqlx-batis-0.0.7/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.0.7/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     4126 2023-07-23 23:51:27.000000 sqlx-batis-0.0.7/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1421 2023-07-23 14:00:47.000000 sqlx-batis-0.0.7/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      354 2023-07-23 22:35:05.000000 sqlx-batis-0.0.7/sqlbatis/support.py
+-rw-rw-rw-   0        0        0      154 2023-07-23 13:54:14.000000 sqlx-batis-0.0.7/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3427 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      471 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.0.6/PKG-INFO` & `sqlx-batis-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.6
+Version: 0.0.7
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.0.6/README.rst` & `sqlx-batis-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.6/setup.py` & `sqlx-batis-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'sqlx-exec>=1.1.5',
     ],
-    version='0.0.6',
+    version='0.0.7',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.0.6/sqlbatis/db.py` & `sqlx-batis-0.0.7/sqlbatis/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import sqlexec
 from . import sql_support, Engin
 from .constant import MAPPER_PATH
 from .log_support import sql_log, page_log, do_sql_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec import(insert, save, save_sql, batch_insert, batch_execute)
+from sqlexec import init_db as supper_init_db, insert, save, batch_insert, batch_execute, execute as supper_execute, get as supper_get, \
+    query as supper_query, query_one as supper_query_one, query_page as supper_query_page, select as supper_select, select_one as supper_select_one, \
+    select_page as supper_select_page
 
 
-def init_db(connect=None, user='root', password='', database='test', host='127.0.0.1', port=3306, engin=Engin.MySQL, pool_size=0, show_sql=False, **kwargs):
+def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, engin=Engin.MYSQL, pool_size=0, show_sql=False, **kwargs):
     if MAPPER_PATH in kwargs:
         from .sql_holder import load_mapper
         load_mapper(kwargs.pop(MAPPER_PATH))
-    sqlexec.init_db(connect=connect, user=user, password=password, database=database, host=host, port=port, engin=engin, pool_size=pool_size,
-                    show_sql=show_sql, **kwargs)
+    supper_init_db(user=user, password=password, database=database, host=host, port=port, engin=engin, pool_size=pool_size, show_sql=show_sql,
+                   **kwargs)
 
 
 # ----------------------------------------------------------Update function------------------------------------------------------------------
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
@@ -113,72 +114,71 @@
 
 # ----------------------------------------------------------Do function------------------------------------------------------------------
 def do_execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into user(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
-    return sqlexec.execute(sql, *args)
+    return supper_execute(sql, *args)
 
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_get', sql, *args)
     sql, args = sql_support.limit_one_sql_args(sql, *args)
-    return sqlexec.get(sql, *args)
+    return supper_get(sql, *args)
 
 
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    return sqlexec.query(sql, *args)
+    return supper_query(sql, *args)
 
 
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_query_one', sql, *args)
     sql, args = sql_support.limit_one_sql_args(sql, *args)
-    return sqlexec.query_one(sql, *args)
+    return supper_query_one(sql, *args)
 
 
 def do_select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    return sqlexec.select(sql, *args)
+    return supper_select(sql, *args)
 
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_select_one', sql, *args)
     sql, args = sql_support.limit_one_sql_args(sql, *args)
-    return sqlexec.select_one(sql, *args)
+    return supper_select_one(sql, *args)
 
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    return sqlexec.query_page(sql, page_num, page_size, *args)
+    return supper_query_page(sql, page_num, page_size, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    return sqlexec.select_page(sql, page_num, page_size, *args)
-
+    return supper_select_page(sql, page_num, page_size, *args)
```

### Comparing `sqlx-batis-0.0.6/sqlbatis/dbx.py` & `sqlx-batis-0.0.7/sqlbatis/dbx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import sqlexec
 from .exec_support import do_save
-from . import db, Engin, sql_holder as holder
 from .sql_support import get_batch_args
+from . import Engin, sql_holder as holder
 from .log_support import logger, sql_id_log, page_sql_id_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec import(insert, batch_insert)
+from .db import(init_db as supper_init_db, do_execute, insert, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, \
+                do_query_page, do_select, do_select_one, do_select_page)
 
 
-def init_db(connect=None, user='root', password='', database='test', host='127.0.0.1', port=3306, mapper_path='mapper', engin=Engin.MySQL,
-        pool_size=0, show_sql=False, **kwargs):
+def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, mapper_path='mapper', engin=Engin.MYSQL, pool_size=0,
+        show_sql=False, **kwargs):
     holder.load_mapper(mapper_path)
-    sqlexec.init_db(connect=connect, user=user, password=password, database=database, host=host, port=port, engin=engin, pool_size=pool_size,
-                    show_sql=show_sql, **kwargs)
+    supper_init_db(user=user, password=password, database=database, host=host, port=port, engin=engin, pool_size=pool_size, show_sql=show_sql, **kwargs)
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
@@ -29,106 +28,106 @@
     """
     Execute SQL.
     sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('dbx.execute', sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return sqlexec.execute(sql, *args)
+    return do_execute(sql, *args)
 
 
 def batch_execute(sql_id: str, *args):
     """
     Batch execute
     sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
          INSERT INTO person(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
     logger.debug("Exec func 'mysqlx.dbx.%s' \n\t sql_id: '%s' \n\t args: %s" % ('batch_execute', sql_id, args))
     assert len(args) > 0, 'args must not be empty.'
     args = get_batch_args(*args)
     sql, _ = holder.do_get_sql(holder.get_sql_model(sql_id), True, None, *args)
-    return sqlexec.batch_execute(sql, *args)
+    return db_batch_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('get', sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return db.do_get(sql, *args)
+    return do_get(sql, *args)
 
 
 def query(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('query', sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return sqlexec.query(sql, *args)
+    return do_query(sql, *args)
 
 
 def query_one(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(dict). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('query_one', sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return db.do_query_one(sql, *args)
+    return do_query_one(sql, *args)
 
 
 def select(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('select', sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return sqlexec.select(sql, *args)
+    return do_select(sql, *args)
 
 
 def select_one(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('select_one', sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return db.do_select_one(sql, *args)
+    return do_select_one(sql, *args)
 
 
 def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     page_sql_id_log('query_page', sql_id, page_num, page_size, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return sqlexec.query_page(sql, page_num, page_size, *args)
+    return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     page_sql_id_log('select_page', sql_id, page_num, page_size, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return sqlexec.select_page(sql, page_num, page_size, *args)
+    return do_select_page(sql, page_num, page_size, *args)
```

### Comparing `sqlx-batis-0.0.6/sqlbatis/log_support.py` & `sqlx-batis-0.0.7/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.6/sqlbatis/orm.py` & `sqlx-batis-0.0.7/sqlbatis/orm.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
 from .sql_support import simple_sql
 from .support import DBError, NotFoundError
 from typing import Sequence, Union, List, Tuple
 from . import db, log_support, transaction, DBEngin
-from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, PK, PK_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, CACHE_SIZE
+from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, KEY_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY, CACHE_SIZE
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
 
-class PkStrategy(Enum):
+class KeyStrategy(Enum):
     """
     SNOWFLAKE: 由Snowflake算法生成主键
     DB_AUTO_INCREMENT: 由数据库的AUTO_INCREMENT自动生成主键
 
     在Windows上，使用Snowflake可能会报下列错误，这是因为Snowflake生成的id是15位的数字，而Windows上C语言的long类型是32位的
     OverflowError: Python int too large to convert to C long
 
@@ -32,20 +32,20 @@
 
 
 class Model:
     """
     Create a class extends Model:
 
     class Person(Model):
-        __pk__ = 'id'
+        __key__ = 'id'
         __table__ = 'person'
         __update_by__ = 'update_by'
         __update_time__ = 'update_time'
         __del_flag__ = 'del_flag'
-        __pk_seq__ = 'person_id_seq'
+        __key_seq__ = 'person_id_seq'
 
         def __init__(self, id: int = None, name: str = None, age: int = None, update_by: int = None, update_time: datetime = None, del_flag: int = None):
             self.id = id
 
             self.update_by = update_by
             self.update_time = update_time
             self.del_flag = del_flag
@@ -59,16 +59,16 @@
         id = person.inst_save()
     """
 
     def __str__(self):
         return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
 
     def __getattr__(self, name):
-        if PK == name:
-            return self._get_pk()
+        if KEY == name:
+            return self._get_key()
         elif TABLE == name:
             return self._get_table()
         elif UPDATE_BY == name:
             return self._get_update_by_field()
         elif UPDATE_TIME == name:
             return self._get_update_time_field()
         else:
@@ -88,160 +88,160 @@
         """
         person = Person(name='张三', age=55)
         id = person.save()
         :return: Primary key
         """
         log_support.orm_inst_log('inst_save', self.__class__.__name__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        pk = self._get_pk()
+        key = self._get_key()
         _id = self.save(**kv)
-        if pk not in kv:
-            self.__dict__.update({pk: _id})
+        if key not in kv:
+            self.__dict__.update({key: _id})
         return _id
 
     def update(self, ignored_none=True):
         """
         person = Person(id=1, name='李四', age=66)
         rowcount = person.update()
         :return: Effect rowcount
         """
         log_support.orm_inst_log('update', self.__class__.__name__)
-        pk, table = self._get_pk_and_table()
+        key, table = self._get_key_and_table()
         if ignored_none:
             kv = {k: v for k, v in self.__dict__.items() if v is not None}
         else:
             kv = {k: v for k, v in self.__dict__.items()}
-        _id = kv[pk]
+        _id = kv[key]
         assert _id is not None, 'Primary key must not be None.'
-        update_kv = {k: v for k, v in kv.items() if k != pk}
+        update_kv = {k: v for k, v in kv.items() if k != key}
         if update_kv:
             return self.update_by_id(_id, **update_kv)
         else:
             log_support.logger.warning("Exec func 'sqlx-batis.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
             return 0
 
     def load(self, *fields):
         """
         Return new object from database and update itself.
         :param fields: Default select all fields if not set. like: ('id', 'name', 'age')
         person = Person(id=1)
         person2 = person.load()
         """
         log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
-        pk = self._get_pk()
+        key = self._get_key()
         kv = self.__dict__
-        _id = kv.get(pk)
+        _id = kv.get(key)
         assert _id is not None, 'Primary key must not be None.'
         if not fields:
             fields, _ = zip(*kv.items())
         result = self.query_by_id(_id, *fields)
         if result:
             self.__dict__.update(result)
             return self
         else:
-            raise NotFoundError("Load not found from db, Class: '%s', %s=%d." % (self.__class__.__name__, pk, _id))
+            raise NotFoundError("Load not found from db, Class: '%s', %s=%d." % (self.__class__.__name__, key, _id))
 
     def logical_delete(self):
         """
         Logic delete only update the del flag
         person = Person(id=1)
         rowcount = person.logical_delete()
         """
         log_support.orm_inst_log('logical_delete', self.__class__.__name__)
-        pk = self._get_pk()
+        key = self._get_key()
         kv = self.__dict__
-        _id = kv.get(pk)
+        _id = kv.get(key)
         assert _id is not None, 'Primary key must not be None.'
         update_by = kv.get(self._get_update_by_field())
         return self.logical_delete_by_id(_id, update_by)
 
     def un_logical_delete(self):
         """
         Logic un delete only update the del flag
         person = Person(id=1)
         rowcount = person.un_logical_delete()
         """
         log_support.orm_inst_log('un_logical_delete', self.__class__.__name__)
-        pk = self._get_pk()
+        key = self._get_key()
         kv = self.__dict__
-        _id = kv.get(pk)
+        _id = kv.get(key)
         assert _id is not None, 'Primary key must not be None.'
         update_by = kv.get(self._get_update_by_field())
         return self.un_logical_delete_by_id(_id, update_by)
 
     def delete(self):
         """
         Physical delete
         person = Person(id=1)
         rowcount = person.delete()
         """
         log_support.orm_inst_log('delete', self.__class__.__name__)
-        pk = self._get_pk()
-        _id = self.__dict__.get(pk)
+        key = self._get_key()
+        _id = self.__dict__.get(key)
         assert _id is not None, 'Primary key must not be None.'
         return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
     def insert(cls, **kwargs):
         """
         rowcount = Person.insert(name='张三', age=20)
         return: Effect rowcount
         """
         log_support.orm_insert_log('insert', cls.__name__, **kwargs)
-        pk, table = cls._get_pk_and_table()
-        pk_strategy = cls._get_pk_strategy()
-        if pk_strategy == PkStrategy.SNOWFLAKE and pk not in kwargs:
-            kwargs[pk] = get_id()
+        key, table = cls._get_key_and_table()
+        key_strategy = cls._get_key_strategy()
+        if key_strategy == KeyStrategy.SNOWFLAKE and key not in kwargs:
+            kwargs[key] = get_id()
         return sqlexec.insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = Person.save(name='张三', age=20)
         :return: Primary key
         """
         log_support.orm_insert_log('save', cls.__name__, **kwargs)
-        pk, table = cls._get_pk_and_table()
-        pk_strategy = cls._get_pk_strategy()
-        if pk_strategy == PkStrategy.SNOWFLAKE:
-            if pk in kwargs:
-                _id = kwargs[pk]
+        key, table = cls._get_key_and_table()
+        key_strategy = cls._get_key_strategy()
+        if key_strategy == KeyStrategy.SNOWFLAKE:
+            if key in kwargs:
+                _id = kwargs[key]
             else:
                 _id = get_id()
-                kwargs[pk] = _id
+                kwargs[key] = _id
             sqlexec.insert(table, **kwargs)
         else:
-            pk_seq = cls._get_pk_seq()
-            _id = sqlexec.save(DBEngin.get_select_key(pk_seq=pk_seq, table=table), table, **kwargs)
+            key_seq = cls._get_key_seq()
+            _id = sqlexec.save(DBEngin.get_select_key(key_seq=key_seq, table=table), table, **kwargs)
         return _id
 
     @classmethod
     def create(cls, **kwargs):
         """
         person = Person.create(name='张三', age=20)
         :return: Instance object
         """
         log_support.orm_insert_log('create', cls.__name__, **kwargs)
-        pk = cls._get_pk()
+        key = cls._get_key()
         _id = cls.save(**kwargs)
-        if pk not in kwargs:
-            kwargs[pk] = _id
+        if key not in kwargs:
+            kwargs[key] = _id
         return cls.to_obj(**kwargs)
 
     @classmethod
     def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = Person.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
-        pk = cls._get_pk()
-        where = '%s=?' % pk
+        key = cls._get_key()
+        where = '%s=?' % key
         cols, args = zip(*kwargs.items())
         sql, update_time_arg = cls._update_sql(where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
         return sqlexec.execute(sql, *args, _id)
 
     @classmethod
@@ -302,16 +302,16 @@
     def delete_by_id(cls, _id: Union[int, str]):
         """
         Physical delete
         rowcount = Person.delete_by_id(id=1)
         return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
-        pk, table = cls._get_pk_and_table()
-        sql = 'DELETE FROM %s WHERE %s=?' % (table, pk)
+        key, table = cls._get_key_and_table()
+        sql = 'DELETE FROM %s WHERE %s=?' % (table, key)
         return sqlexec.execute(sql, _id)
 
     @classmethod
     def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
         Batch physical delete, they will be executed in batches if there are too many
         rowcount = Person.delete_by_ids(id=[1,2])
@@ -334,34 +334,34 @@
     def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
         """
         Batch physical delete, please use delete_by_ids if there are too many
         rowcount = Person.do_delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
         ids_size = len(ids)
-        pk, table = cls._get_pk_and_table()
-        sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
+        key, table = cls._get_key_and_table()
+        sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, key, ','.join(['?' for _ in range(ids_size)]))
         return sqlexec.execute(sql, *ids)
 
     @classmethod
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
         assert len(args) > 0, 'args must not be empty.'
-        pk, table = cls._get_pk_and_table()
-        pk_strategy = cls._get_pk_strategy()
-        if pk_strategy == PkStrategy.SNOWFLAKE:
+        key, table = cls._get_key_and_table()
+        key_strategy = cls._get_key_strategy()
+        if key_strategy == KeyStrategy.SNOWFLAKE:
             for arg in args:
-                if pk not in arg:
-                    arg[pk] = get_id()
+                if key not in arg:
+                    arg[key] = get_id()
 
         return sqlexec.batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
@@ -457,27 +457,27 @@
         return [cls.to_obj(**d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
 
     @classmethod
     def find_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one class object or None if no result.
         person = Person.find_by_id(1, 'id', 'name', 'age')
-        :param _id: pk
+        :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('find_by_id', cls.__name__, _id, *fields)
         result = cls.query_by_id(_id, *fields)
         return cls.to_obj(**result) if result else None
 
     @classmethod
     def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(class object) or empty list if no result.
         persons = Person.find_by_ids([1,2], 'id', 'name', 'age')
-        :param ids: List of pk
+        :param ids: List of key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_ids_log('find_by_ids', cls.__name__, ids, *fields)
         return [cls.to_obj(**d) for d in cls.query_by_ids(ids, *fields)]
 
     @classmethod
     def query(cls, *fields, **kwargs):
@@ -548,37 +548,37 @@
         return sqlexec.query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         person = Person.query_by_id(1, 'id', 'name', 'age')
-        :param _id: pk
+        :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
-        pk, table = cls._get_pk_and_table()
-        where = 'WHERE {}=?'.format(pk)
+        key, table = cls._get_key_and_table()
+        where = 'WHERE {}=?'.format(key)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return sqlexec.query_one(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         persons = Person.query_by_ids([1,2], 'id', 'name', 'age')
-        :param ids: List of pk
+        :param ids: List of key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk, table = cls._get_pk_and_table()
-        where = 'WHERE {} in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
+        key, table = cls._get_key_and_table()
+        where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return sqlexec.query(sql, *ids, ids_size)
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
@@ -647,54 +647,54 @@
         return sqlexec.select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         row = Person.select_by_id(1, 'id', 'name', 'age')
-        :param _id: pk
+        :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
-        pk, table = cls._get_pk_and_table()
-        where = 'WHERE {}=?'.format(pk)
+        key, table = cls._get_key_and_table()
+        where = 'WHERE {}=?'.format(key)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return sqlexec.select_one(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
-        :param ids: List of pk
+        :param ids: List of key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk, table = cls._get_pk_and_table()
-        where = 'WHERE {} in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
+        key, table = cls._get_key_and_table()
+        where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return sqlexec.select(sql, *ids, ids_size)
 
     @classmethod
     def to_obj(cls, **kwargs):
         model = cls.__new__(cls)
         model.__dict__.update(**kwargs)
         return model
 
     # ------------------------------------------------Private class method------------------------------------------------------------------
     @classmethod
     def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
-        pk, table = cls._get_pk_and_table()
+        key, table = cls._get_key_and_table()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
-        where = '%s=?' % pk
+        where = '%s=?' % key
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
                 return sqlexec.execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
             return sqlexec.execute(sql, del_status.value, update_by, _id, LIMIT_1)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
@@ -716,60 +716,60 @@
             split_ids = _split_ids(ids, batch_size)
             with transaction():
                 results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
             return sum(results)
 
     @classmethod
     def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
-        pk = cls._get_pk()
+        key = cls._get_key()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
-        where = '%s in (%s)' % (pk, ','.join(['?' for _ in range(len(ids))]))
+        where = '%s in (%s)' % (key, ','.join(['?' for _ in range(len(ids))]))
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
                 return sqlexec.execute(sql, del_status.value, update_by, update_time_arg, *ids)
             return sqlexec.execute(sql, del_status.value, update_by, *ids)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
                 return sqlexec.execute(sql, del_status.value, update_time_arg, *ids)
             return sqlexec.execute(sql, del_status.value, *ids)
 
     @classmethod
-    def _get_pk(cls):
-        if hasattr(cls, PK):
-            return cls.__pk__
-        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
-        return DEFAULT_PK_FIELD
+    def _get_key(cls):
+        if hasattr(cls, KEY):
+            return cls.__key__
+        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, KEY))
+        return DEFAULT_KEY_FIELD
 
     @classmethod
-    def _get_pk_seq(cls):
-        if hasattr(cls, PK_SEQ):
-            return cls.__pk_seq__
-        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, PK_SEQ))
-        pk, table = cls._get_pk_and_table()
-        return "{}_{}_seq".format(table, pk)
+    def _get_key_seq(cls):
+        if hasattr(cls, KEY_SEQ):
+            return cls.__key_seq__
+        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, KEY_SEQ))
+        key, table = cls._get_key_and_table()
+        return "{}_{}_seq".format(table, key)
 
     @classmethod
     def _get_table(cls):
         if hasattr(cls, TABLE):
             return cls.__table__
         log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
         return _get_table_name(cls.__name__)
 
     @classmethod
-    def _get_pk_and_table(cls):
-        return cls._get_pk(), cls._get_table()
+    def _get_key_and_table(cls):
+        return cls._get_key(), cls._get_table()
 
     @classmethod
-    def _get_pk_strategy(cls):
-        if hasattr(cls, PK_STRATEGY):
-            return cls.__pk_strategy__
+    def _get_key_strategy(cls):
+        if hasattr(cls, KEY_STRATEGY):
+            return cls.__key_strategy__
         return None
 
     @classmethod
     def _get_update_by_field(cls):
         if hasattr(cls, UPDATE_BY):
             return cls.__update_by__
         return None
```

### Comparing `sqlx-batis-0.0.6/sqlbatis/snowflake.py` & `sqlx-batis-0.0.7/sqlbatis/snowflake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from sqlexec.support import DB_LOCK
+from .support import DB_LOCK
 
 _SNOWFLAKE = None
 _WORKER_BITS = 10
 _SEQUENCE_BITS = 12
 _EPOCH = 1688140800000
 # _SEQUENCE_MASK = 4095
```

### Comparing `sqlx-batis-0.0.6/sqlbatis/sql_holder.py` & `sqlx-batis-0.0.7/sqlbatis/sql_holder.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     import xml.etree.ElementTree as ET
 
 _SQL_CONTAINER = dict()
 _valid_sql_actions = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.SELECT.value)
 
 
 class SqlModel:
-    def __init__(self, sql: str, action: str, namespace: str, dynamic=False, includes: List[str] = None, pk_seq: str = None, select_key: str=None):
+    def __init__(self, sql: str, action: str, namespace: str, dynamic=False, includes: List[str] = None, key_seq: str = None, select_key: str=None):
         self.sql = sql
         self.action = action
         self.namespace = namespace
         self.dynamic = dynamic
         self.includes = includes
-        self.pk_seq = pk_seq
+        self.key_seq = key_seq
         self.select_key = select_key
         self.mapping = True if dynamic else ':' in sql
         self.placeholder = False if self.mapping else '?' in sql
 
 
 def get_sql(sql_id: str, *args, **kwargs):
     sql_model = get_sql_model(sql_id)
@@ -147,26 +147,26 @@
     _id = child.attrib.get('id')
     assert _id, "Mapper 'id' must be set in mapper file: %s." % file
     sql_id = build_sql_id(namespace, _id)
     assert sql_id not in _SQL_CONTAINER, "Sql id '%s' repeat." % sql_id
     include = child.attrib.get('include')
     sql = child.text.strip()
     action = child.tag
-    pk_seq = child.attrib.get('pkSeq')
+    key_seq = child.attrib.get('keySeq')
     select_key = child.attrib.get('selectKey')
     if include:
         includes = include.split(",")
         for include in set(includes):
             assert include != _id, "Include must not be it self, id: '%s' = include: '%s' " % (_id, include)
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=action, namespace=namespace, includes=includes, pk_seq=pk_seq, select_key=select_key)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=action, namespace=namespace, includes=includes, key_seq=key_seq, select_key=select_key)
     elif is_dynamic_sql(sql):
         _valid_sql(sql_id, sql, child.tag)
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=action, namespace=namespace, dynamic=True, pk_seq=pk_seq, select_key=select_key)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=action, namespace=namespace, dynamic=True, key_seq=key_seq, select_key=select_key)
     else:
         _valid_sql(sql_id, sql, child.tag)
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=action, namespace=namespace, pk_seq=pk_seq, select_key=select_key)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=action, namespace=namespace, key_seq=key_seq, select_key=select_key)
 
     return _id, includes
 
 
 def _valid_sql(sql_id, sql, tag):
     assert tag in _valid_sql_actions and tag in sql.lower(), "Sql id: '{}' has not '{}' key word in {} sql.".format(sql_id, tag, tag)
```

### Comparing `sqlx-batis-0.0.6/sqlbatis/sql_mapper.py` & `sqlx-batis-0.0.7/sqlbatis/sql_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,53 +6,53 @@
 from .exec_support import do_save, do_save0
 from .sql_support import simple_sql, get_named_sql_args
 from .sql_holder import get_sql_model, do_get_sql, build_sql_id
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
-def mapper(namespace: str = None, sql_id: str = None, batch=False, return_pk=False):
+def mapper(namespace: str = None, sql_id: str = None, batch=False, return_key=False):
     def _decorator(func):
         @functools.wraps(func)
         def _wrapper(*args, **kwargs):
             param_names = func.__code__.co_varnames
             full_sql_id, func_name = _before(func, namespace, sql_id, *args, **kwargs)
             sql_model = get_sql_model(full_sql_id)
             exec_func = _get_exec_func(func, sql_model.action, batch)
-            if return_pk:
+            if return_key:
                 return do_save(sql_model, batch, param_names, *args, **kwargs)
             if batch:
                 if kwargs:
                     logger.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
                     args = list(kwargs.values())[0]
                 use_sql, _ = do_get_sql(sql_model, batch, param_names, *args)
             else:
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
             return exec_func(use_sql, *args)
 
         return _wrapper
     return _decorator
 
 
-def sql(value: str, batch=False, return_pk=False, select_key=None, pk_seq=None):
+def sql(value: str, batch=False, return_key=False, select_key=None, key_seq=None):
     def _decorator(func):
         @functools.wraps(func)
         def _wrapper(*args, **kwargs):
             use_sql = value
             low_sql = value.lower()
             if any([action in low_sql for action in _UPDATE_ACTIONS]):
                 if batch:
                     if kwargs:
                         args = list(kwargs.values())[0]
                     return sqlexec.batch_execute(use_sql, *args)
-                if return_pk:
+                if return_key:
                     assert SqlAction.INSERT.value in low_sql, 'Only insert sql can return primary key.'
                     if kwargs:
                         use_sql, args = get_named_sql_args(use_sql, **kwargs)
-                    return do_save0(select_key, pk_seq, use_sql, *args)
+                    return do_save0(select_key, key_seq, use_sql, *args)
 
                 if kwargs:
                     use_sql, args = get_named_sql_args(use_sql, **kwargs)
                 return sqlexec.execute(use_sql, *args)
             elif SqlAction.SELECT.value in low_sql:
                 select_func = _get_select_func(func)
                 use_sql, args = simple_sql(use_sql, *args, **kwargs)
```

### Comparing `sqlx-batis-0.0.6/sqlbatis/sql_support.py` & `sqlx-batis-0.0.7/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.6/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.0.7/sqlx_batis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.6
+Version: 0.0.7
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

