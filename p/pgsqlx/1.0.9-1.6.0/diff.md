# Comparing `tmp/pgsqlx-1.0.9.tar.gz` & `tmp/pgsqlx-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.0.9.tar", last modified: Fri Jul 21 10:08:16 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.6.0.tar", last modified: Mon Jul 24 01:53:49 2023, max compression
```

## Comparing `pgsqlx-1.0.9.tar` & `pgsqlx-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/
-drwxrwxrwx   0        0        0        0 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx/
--rw-rw-rw-   0        0        0      552 2023-07-19 13:24:36.000000 pgsqlx-1.0.9/pgsqlx/constant.py
--rw-rw-rw-   0        0        0    17295 2023-07-21 06:06:21.000000 pgsqlx-1.0.9/pgsqlx/db.py
--rw-rw-rw-   0        0        0     7496 2023-07-19 13:34:57.000000 pgsqlx-1.0.9/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.9/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0    38425 2023-07-19 13:46:35.000000 pgsqlx-1.0.9/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-07-19 06:32:34.000000 pgsqlx-1.0.9/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0     6412 2023-07-19 13:34:08.000000 pgsqlx-1.0.9/pgsqlx/sql_holder.py
--rw-rw-rw-   0        0        0     5138 2023-07-19 13:36:00.000000 pgsqlx-1.0.9/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     3752 2023-07-21 08:20:35.000000 pgsqlx-1.0.9/pgsqlx/sql_support.py
--rw-rw-rw-   0        0        0     4737 2023-07-19 14:00:04.000000 pgsqlx-1.0.9/pgsqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.9/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4413 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      400 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4413 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3900 2023-07-21 10:07:42.000000 pgsqlx-1.0.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 10:08:16.000000 pgsqlx-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-07-21 10:07:42.000000 pgsqlx-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/pgsqlx/
+-rw-rw-rw-   0        0        0     1426 2023-07-24 00:56:26.000000 pgsqlx-1.6.0/pgsqlx/db.py
+-rw-rw-rw-   0        0        0      630 2023-07-24 00:18:48.000000 pgsqlx-1.6.0/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      534 2023-07-24 00:56:26.000000 pgsqlx-1.6.0/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     1889 2023-07-24 01:02:17.000000 pgsqlx-1.6.0/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0       57 2023-07-24 00:49:57.000000 pgsqlx-1.6.0/pgsqlx/snowflake.py
+-rw-rw-rw-   0        0        0      103 2023-07-24 00:31:03.000000 pgsqlx-1.6.0/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0      125 2023-07-23 23:06:11.000000 pgsqlx-1.6.0/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4413 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      320 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4413 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3900 2023-07-21 10:07:42.000000 pgsqlx-1.6.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-24 01:53:49.000000 pgsqlx-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1233 2023-07-24 01:53:19.000000 pgsqlx-1.6.0/setup.py
```

### Comparing `pgsqlx-1.0.9/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.6.0/pgsqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.9
+Version: 1.6.0
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.0.9/PKG-INFO` & `pgsqlx-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.9
+Version: 1.6.0
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.0.9/README.rst` & `pgsqlx-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.9/setup.py` & `pgsqlx-1.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     packages=['pgsqlx'],
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'psycopg2>=2.7.4',
+        'sqlx-batis>=0.0.7',
     ],
-    version='1.0.9',
+    version='1.6.0',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

