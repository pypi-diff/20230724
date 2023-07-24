# Comparing `tmp/sqlx-exec-1.1.4.tar.gz` & `tmp/sqlx-exec-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.1.4.tar", last modified: Sun Jul 23 10:23:16 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.1.5.tar", last modified: Mon Jul 24 01:44:11 2023, max compression
```

## Comparing `sqlx-exec-1.1.4.tar` & `sqlx-exec-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     2701 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2159 2023-07-22 02:28:05.000000 sqlx-exec-1.1.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1254 2023-07-23 10:22:11.000000 sqlx-exec-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/sqlexec/
--rw-rw-rw-   0        0        0      529 2023-07-23 08:55:03.000000 sqlx-exec-1.1.4/sqlexec/constant.py
--rw-rw-rw-   0        0        0     3512 2023-07-23 08:10:22.000000 sqlx-exec-1.1.4/sqlexec/engin.py
--rw-rw-rw-   0        0        0    11599 2023-07-23 10:19:08.000000 sqlx-exec-1.1.4/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1030 2023-07-21 22:35:47.000000 sqlx-exec-1.1.4/sqlexec/log_support.py
--rw-rw-rw-   0        0        0      772 2023-07-23 10:18:39.000000 sqlx-exec-1.1.4/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     2229 2023-07-22 21:58:27.000000 sqlx-exec-1.1.4/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4275 2023-07-23 09:51:27.000000 sqlx-exec-1.1.4/sqlexec/support.py
--rw-rw-rw-   0        0        0      361 2023-07-22 17:31:16.000000 sqlx-exec-1.1.4/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-22 22:12:16.000000 sqlx-exec-1.1.4/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2701 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/sqlx_exec.egg-info/requires.txt
--rw-rw-rw-   0        0        0      380 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-23 10:23:16.000000 sqlx-exec-1.1.4/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2701 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2159 2023-07-22 02:28:05.000000 sqlx-exec-1.1.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-23 13:20:12.000000 sqlx-exec-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlexec/
+-rw-rw-rw-   0        0        0      529 2023-07-23 08:55:03.000000 sqlx-exec-1.1.5/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     4272 2023-07-23 23:54:10.000000 sqlx-exec-1.1.5/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    11712 2023-07-23 22:50:17.000000 sqlx-exec-1.1.5/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1030 2023-07-21 22:35:47.000000 sqlx-exec-1.1.5/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0      629 2023-07-23 22:45:17.000000 sqlx-exec-1.1.5/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1556 2023-07-23 13:53:53.000000 sqlx-exec-1.1.5/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4275 2023-07-23 09:51:27.000000 sqlx-exec-1.1.5/sqlexec/support.py
+-rw-rw-rw-   0        0        0      389 2023-07-23 13:53:53.000000 sqlx-exec-1.1.5/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2701 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.1.4/LICENSE` & `sqlx-exec-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.4/PKG-INFO` & `sqlx-exec-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.1.4
+Version: 1.1.5
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.1.4/README.rst` & `sqlx-exec-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.4/setup.py` & `sqlx-exec-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=[
-        'DBUtils>=3.0.0',
-    ],
-    version='1.1.4',
+    version='1.1.5',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.1.4/sqlexec/constant.py` & `sqlx-exec-1.1.5/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.4/sqlexec/engin.py` & `sqlx-exec-1.1.5/sqlexec/engin.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,29 +2,58 @@
 from enum import Enum
 from typing import Sequence
 from .support import DBError
 from functools import lru_cache
 from .log_support import logger
 from .constant import CACHE_SIZE, MYSQL_COLUMN_SQL, POSTGRES_COLUMN_SQL
 
-
-def create_sql_engin(engin, show_sql):
-    if engin == Engin.MySQL:
-        return MySqlEngin(show_sql)
-    elif engin == Engin.PostgreSQL:
-        return PostgresEngin(show_sql)
-    raise
+_ENGIN = None
+_DB_ENGIN = None
 
 
 class Engin(Enum):
-    MySQL = 'MySQL'
-    PostgreSQL = 'PostgreSQL'
+    MYSQL = 'MySQL'
+    POSTGRESQL = 'PostgreSQL'
+    OTHER = 'other'
+
+    @staticmethod
+    def current_engin():
+        global _ENGIN
+        return _ENGIN
+
+
+class DBEngin:
+    before_execute = None
+    before_execute = None
+    before_execute = None
+    before_execute = None
+    before_execute = None
+
+    @classmethod
+    def init_db_engin(cls, engin, show_sql):
+        global _ENGIN
+        global _DB_ENGIN
+        _ENGIN = engin
+        if engin == Engin.MYSQL:
+            _DB_ENGIN = MySqlEngin(show_sql)
+        elif engin == Engin.POSTGRESQL:
+            _DB_ENGIN = PostgresEngin(show_sql)
+        elif engin == Engin.OTHER:
+            _DB_ENGIN = BaseEngin(show_sql)
+        else:
+            raise DBError("Unknown engin type: {}".format(engin))
+
+        cls.before_execute = _DB_ENGIN.before_execute
+        cls.page_sql_args = _DB_ENGIN.page_sql_args
+        cls.create_insert_sql = _DB_ENGIN.create_insert_sql
+        cls.get_select_key = _DB_ENGIN.get_select_key
+        cls.get_column_sql = _DB_ENGIN.get_column_sql
 
 
-class SqlEngin:
+class BaseEngin:
     def __init__(self, show_sql):
         self.show_sql = show_sql
 
     def before_execute(self, function: str, sql: str, *args):
         if self.show_sql:
             logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
         if '%' in sql and 'like' in sql.lower():
@@ -33,16 +62,28 @@
 
     @staticmethod
     @lru_cache(maxsize=CACHE_SIZE)
     def create_insert_sql(table: str, cols: Sequence[str]):
         columns, placeholders = zip(*[('{}'.format(col), '?') for col in cols])
         return 'INSERT INTO {}({}) VALUES({})'.format(table, ', '.join(columns), ','.join(placeholders))
 
+    @staticmethod
+    def page_sql_args(require_limit, sql: str, start, page_size, *args):
+        pass
+
+    @staticmethod
+    def get_select_key(*args, **kwargs):
+        pass
+
+    @staticmethod
+    def get_column_sql():
+        pass
+
 
-class MySqlEngin(SqlEngin):
+class MySqlEngin(BaseEngin):
 
     def __init__(self, show_sql):
         super().__init__(show_sql)
 
     @staticmethod
     def page_sql_args(require_limit, sql: str, start, page_size, *args):
         if require_limit(sql):
@@ -55,55 +96,47 @@
         return "SELECT LAST_INSERT_ID()"
 
     @staticmethod
     def get_column_sql():
         return MYSQL_COLUMN_SQL
 
 
-
-
-class PostgresEngin(SqlEngin):
+class PostgresEngin(BaseEngin):
 
     def __init__(self, show_sql):
         super().__init__(show_sql)
 
-    def before_execute(self, function: str, sql: str, *args):
-        if self.show_sql:
-            logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
-        if '%' in sql and 'like' in sql.lower():
-            sql = sql.replace('%', '%%').replace('%%%%', '%%')
-        return sql.replace('?', '%s')
 
     @staticmethod
     def page_sql_args(require_limit, sql: str, start, page_size, *args):
         if require_limit(sql):
             sql = '{} LIMIT ? OFFSET ?'.format(sql)
         args = [*args, page_size, start]
         return sql, args
 
     @staticmethod
-    def get_select_key(pk_seq: str = None, table: str = None, sql: str = None, *args, **kwargs):
-        if not pk_seq:
+    def get_select_key(key_seq: str = None, table: str = None, sql: str = None):
+        if not key_seq:
             if table:
-                pk_seq = PostgresEngin._build_pk_seq(table)
+                key_seq = PostgresEngin._build_key_seq(table)
             else:
                 if sql:
-                    pk_seq = PostgresEngin._get_pk_seq_from_sql(sql)
+                    key_seq = PostgresEngin._get_key_seq_from_sql(sql)
                 else:
-                    raise DBError("Get PostgreSQL select key fail, all of 'pk_seq', 'table', 'sql' are None")
-        return f"SELECT currval('{pk_seq}')"
+                    raise DBError("Get PostgreSQL select key fail, all of 'key_seq', 'table', 'sql' are None")
+        return f"SELECT currval('{key_seq}')"
 
     @staticmethod
     def get_column_sql():
         return POSTGRES_COLUMN_SQL
 
     @staticmethod
-    def _build_pk_seq(table: str):
+    def _build_key_seq(table: str):
         return f'{table}_id_seq'
 
     @staticmethod
     @lru_cache(maxsize=CACHE_SIZE)
-    def _get_pk_seq_from_sql(sql: str):
+    def _get_key_seq_from_sql(sql: str):
         table = re.search('(?<=into )\w+', sql, re.I)
-        pk_seq = PostgresEngin._build_pk_seq(table.group())
-        logger.warning("'pk_seq' is None, will use default '{}' from sql.".format(pk_seq))
-        return pk_seq
+        key_seq = PostgresEngin._build_key_seq(table.group())
+        logger.warning("'key_seq' is None, will use default '{}' from sql.".format(key_seq))
+        return key_seq
```

### Comparing `sqlx-exec-1.1.4/sqlexec/exec.py` & `sqlx-exec-1.1.5/sqlexec/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import functools
 import importlib
-from .engin import Engin
+from .engin import Engin, DBEngin
 from . import sql_support
 from .constant import MAPPER_PATH, DRIVER
 from .log_support import logger, insert_log, save_log, get_log, page_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
 
 
-def init_db(connect=None, user='root', password='', database='test', host='127.0.0.1', port=3306, engin=Engin.MySQL, pool_size=2, show_sql=False, **kwargs):
-    sql_support.set_config(engin, show_sql)
+def init_db(connect=None, user='root', password='', database='test', host='127.0.0.1', port=3306, engin=Engin.MYSQL, pool_size=0, show_sql=False, **kwargs):
+    DBEngin.init_db_engin(engin, show_sql)
     _del_kwarg(MAPPER_PATH, kwargs)
     driver = kwargs.pop(DRIVER) if DRIVER in kwargs else None
     if 'debug' in kwargs:
         if kwargs.pop('debug'):
             from logging import DEBUG
             logger.setLevel(DEBUG)
 
@@ -30,31 +30,35 @@
         kwargs['port'] = port
 
         _import_init(engin, pool_size, driver, **kwargs)
 
 
 def _import_init(engin, pool_size, driver, **kwargs):
     prepared = False
-    if engin == Engin.MySQL:
+    if engin == Engin.MYSQL:
         if not driver:
             driver = 'pymysql'
             logger.warning("Not set MySQL driver, will use default driver: 'pymysql'.")
         creator = _import(driver)
         if 'mysql.connector' == driver:
             prepared = True
             if pool_size > 0:
                 kwargs['pool_size'] = pool_size
                 pool_size = 0
 
-    elif engin == Engin.PostgreSQL:
+    elif engin == Engin.POSTGRESQL:
         if not driver:
             driver = 'psycopg2'
             logger.warning("Not set PostgreSQL driver, will use default driver: 'psycopg2'.")
         creator = _import(driver)
         _del_kwarg('use_unicode', kwargs)
+    elif engin == Engin.OTHER:
+        if driver:
+            creator = _import(driver)
+        _del_kwarg('use_unicode', kwargs)
     else:
         raise DBError('Engin is invalid: %s', engin)
 
     if pool_size >= 1 and driver != 'mysql.connector':
         from .pooling import pooled_connect
         connect = pooled_connect(creator, pool_size, **kwargs)
         _init_db(connect, engin, pool_size, driver, prepared)
@@ -62,28 +66,27 @@
         _init_db(lambda: creator.connect(**kwargs), engin, pool_size, driver, prepared)
 
 
 def _import(driver):
     try:
         return importlib.import_module(driver)
     except ModuleNotFoundError:
-        raise DBError(f"Import db driver '{driver}' failed, please sure it was intalled or change other driver.")
+        raise DBError(f"Import db driver '{driver}' failed, please sure it was installed or change other driver.")
 
 
 def _del_kwarg(key, kwargs):
     if key in kwargs:
         del kwargs[key]
 
 
 def _init_db(connect, engin, pool_size, driver, prepared=False):
     global _DB_CTX
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
-
         _DB_CTX = DBCtx(connect=connect, pool_size=pool_size, prepared=prepared)
     logger.info("Init db engine <%s> of %s with driver: '%s', pool size is %d." % (hex(id(_DB_CTX)), engin.value, driver, pool_size))
 
 
 def connection():
     """
     Return _ConnectionCtx object that can be used by 'with' statement:
@@ -145,15 +148,15 @@
 def execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = sql_support.before_execute('execute', sql.strip(), *args)
+    sql = DBEngin.before_execute('execute', sql.strip(), *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
     finally:
@@ -194,15 +197,15 @@
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
     logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s" % ('save_sql', select_key, sql, args))
-    sql = sql_support.before_execute('save_sql', sql, *args)
+    sql = DBEngin.before_execute('save_sql', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute(select_key)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
@@ -232,15 +235,15 @@
     :param args: All number must have same size.
     :return: Effect rowcount
     """
     global _DB_CTX
     cursor = None
     if isinstance(args[0], dict):
         sql, args = sql_support.batch_named_sql_args(sql, *args)
-    sql = sql_support.before_execute('batch_execute', sql.strip(), *args)
+    sql = DBEngin.before_execute('batch_execute', sql.strip(), *args)
     args = sql_support.get_batch_args(*args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.executemany(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
@@ -270,15 +273,15 @@
 def select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = sql_support.before_execute('select', sql.strip(), *args)
+    sql = DBEngin.before_execute('select', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchall()
     finally:
         if cursor:
             cursor.close()
@@ -288,15 +291,15 @@
 def select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = sql_support.before_execute('select_one', sql.strip(), *args)
+    sql = DBEngin.before_execute('select_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
@@ -312,15 +315,15 @@
 def query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = sql_support.before_execute('query', sql.strip(), *args)
+    sql = DBEngin.before_execute('query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         results = cursor.fetchall()
         if results and cursor.description:
             names = [x[0] for x in cursor.description]
             return [Dict(names, x) for x in results]
@@ -335,15 +338,15 @@
 def query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = sql_support.before_execute('query_one', sql.strip(), *args)
+    sql = DBEngin.before_execute('query_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         result = cursor.fetchone()
         if result and cursor.description:
             names = [x[0] for x in cursor.description]
             return Dict(names, result)
```

### Comparing `sqlx-exec-1.1.4/sqlexec/log_support.py` & `sqlx-exec-1.1.5/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.4/sqlexec/sql_support.py` & `sqlx-exec-1.1.5/sqlexec/sql_support.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 import re
 from typing import Sequence
 from functools import lru_cache
-from .engin import create_sql_engin
+from .engin import DBEngin
 from .constant import CACHE_SIZE, NAMED_REGEX
 
-_ENGIN = None
-_SQL_ENGIN = None
-before_execute = None
-
-
-def get_select_key(*args, **kwargs):
-    global _SQL_ENGIN
-    return _SQL_ENGIN.get_select_key(*args, **kwargs)
-
-
-def get_column_sql():
-    global _SQL_ENGIN
-    return _SQL_ENGIN.get_column_sql()
-
 
 def insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
-    sql = _SQL_ENGIN.create_insert_sql(table, cols)
+    sql = DBEngin.create_insert_sql(table, cols)
     return sql, args
 
 
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
 def batch_insert_sql_args(table: str, *args):
     args = get_batch_args(*args)
     args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
     cols, args = zip(*args)  # (cols), (args)
-    sql = _SQL_ENGIN.create_insert_sql(table, cols[0])
+    sql = DBEngin.create_insert_sql(table, cols[0])
     return sql, args
 
 
 def batch_named_sql_args(sql: str, *args):
     args = get_batch_args(*args)
     args = [get_named_args(sql, **arg) for arg in args]
     sql = get_named_sql(sql)
@@ -50,39 +36,19 @@
 
 
 def get_named_args(sql: str, **kwargs):
     return [kwargs[r[1:]] for r in re.findall(NAMED_REGEX, sql)]
 
 
 def page_sql_args(sql: str, page_num=1, page_size=10, *args):
-    global _SQL_ENGIN
     start = (page_num - 1) * page_size
-    return _SQL_ENGIN.page_sql_args(require_limit, sql, start, page_size, *args)
+    return DBEngin.page_sql_args(require_limit, sql, start, page_size, *args)
 
 
 def require_limit(sql: str):
     lower_sql = sql.lower()
     if 'limit' not in lower_sql:
         return True
     idx = lower_sql.rindex('limit')
     if idx > 0 and ')' in lower_sql[idx:]:
         return True
     return False
-
-
-def set_config(engin, show_sql):
-    global _ENGIN
-    global _SQL_ENGIN
-    global before_execute
-    _ENGIN = engin
-    _SQL_ENGIN = create_sql_engin(engin, show_sql)
-    before_execute = _SQL_ENGIN.before_execute
-
-
-def get_engin():
-    global _ENGIN
-    return _ENGIN
-
-
-# def get_sql_engin():
-#     global _SQL_ENGIN
-#     return _SQL_ENGIN
```

### Comparing `sqlx-exec-1.1.4/sqlexec/support.py` & `sqlx-exec-1.1.5/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.4/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.1.5/sqlx_exec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.1.4
+Version: 1.1.5
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

