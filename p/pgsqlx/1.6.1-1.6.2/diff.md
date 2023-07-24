# Comparing `tmp/pgsqlx-1.6.1.tar.gz` & `tmp/pgsqlx-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.6.1.tar", last modified: Mon Jul 24 07:19:30 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.6.2.tar", last modified: Mon Jul 24 07:28:28 2023, max compression
```

## Comparing `pgsqlx-1.6.1.tar` & `pgsqlx-1.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/
-drwxrwxrwx   0        0        0        0 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/pgsqlx/
--rw-rw-rw-   0        0        0     1426 2023-07-24 00:56:26.000000 pgsqlx-1.6.1/pgsqlx/db.py
--rw-rw-rw-   0        0        0      630 2023-07-24 00:18:48.000000 pgsqlx-1.6.1/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      534 2023-07-24 00:56:26.000000 pgsqlx-1.6.1/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     1889 2023-07-24 01:02:17.000000 pgsqlx-1.6.1/pgsqlx/orm.py
--rw-rw-rw-   0        0        0      115 2023-07-24 02:35:21.000000 pgsqlx-1.6.1/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0      103 2023-07-24 00:31:03.000000 pgsqlx-1.6.1/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0      125 2023-07-23 23:06:11.000000 pgsqlx-1.6.1/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4410 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      320 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4410 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     3897 2023-07-24 03:07:05.000000 pgsqlx-1.6.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-24 07:19:30.000000 pgsqlx-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1233 2023-07-24 07:19:22.000000 pgsqlx-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/
+drwxrwxrwx   0        0        0        0 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx/
+-rw-rw-rw-   0        0        0     1426 2023-07-24 00:56:26.000000 pgsqlx-1.6.2/pgsqlx/db.py
+-rw-rw-rw-   0        0        0      630 2023-07-24 00:18:48.000000 pgsqlx-1.6.2/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      534 2023-07-24 00:56:26.000000 pgsqlx-1.6.2/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     1889 2023-07-24 01:02:17.000000 pgsqlx-1.6.2/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0      115 2023-07-24 02:35:21.000000 pgsqlx-1.6.2/pgsqlx/snowflake.py
+-rw-rw-rw-   0        0        0      103 2023-07-24 00:31:03.000000 pgsqlx-1.6.2/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0      125 2023-07-23 23:06:11.000000 pgsqlx-1.6.2/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4639 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      320 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4639 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4122 2023-07-24 07:27:35.000000 pgsqlx-1.6.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1233 2023-07-24 07:28:25.000000 pgsqlx-1.6.2/setup.py
```

### Comparing `pgsqlx-1.6.1/pgsqlx/db.py` & `pgsqlx-1.6.2/pgsqlx/db.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.1/pgsqlx/dbx.py` & `pgsqlx-1.6.2/pgsqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.1/pgsqlx/log_support.py` & `pgsqlx-1.6.2/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.1/pgsqlx/orm.py` & `pgsqlx-1.6.2/pgsqlx/orm.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.1/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.6.2/pgsqlx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.1
+Version: 1.6.2
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -142,12 +142,16 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate MySQL database, you may need pgsqlx: https://pypi.org/project/pgsqlx
+You can generate model class with pgsqlx-generator: https://pypi.org/project/pgsqlx-generator
 
-If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you want to operate MySQL database, may be you need pgsqlx: https://pypi.org/project/mysqlx
+
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+
+If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `pgsqlx-1.6.1/PKG-INFO` & `pgsqlx-1.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.1
+Version: 1.6.2
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -142,12 +142,16 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate MySQL database, you may need pgsqlx: https://pypi.org/project/pgsqlx
+You can generate model class with pgsqlx-generator: https://pypi.org/project/pgsqlx-generator
 
-If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you want to operate MySQL database, may be you need pgsqlx: https://pypi.org/project/mysqlx
+
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+
+If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `pgsqlx-1.6.1/README.rst` & `pgsqlx-1.6.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -129,10 +129,14 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate MySQL database, you may need pgsqlx: https://pypi.org/project/pgsqlx
+You can generate model class with pgsqlx-generator: https://pypi.org/project/pgsqlx-generator
 
-If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you want to operate MySQL database, may be you need pgsqlx: https://pypi.org/project/mysqlx
+
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+
+If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `pgsqlx-1.6.1/setup.py` & `pgsqlx-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'psycopg2>=2.7.4',
         'sqlx-batis>=0.0.7',
     ],
-    version='1.6.1',
+    version='1.6.2',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

