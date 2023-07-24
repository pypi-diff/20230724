# Comparing `tmp/Flask-SQL-Pro-4.1.tar.gz` & `tmp/Flask-SQL-Pro-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SQL-Pro-4.1.tar", last modified: Sun Jul 23 23:57:17 2023, max compression
+gzip compressed data, was "Flask-SQL-Pro-4.2.tar", last modified: Sun Jul 23 23:58:25 2023, max compression
```

## Comparing `Flask-SQL-Pro-4.1.tar` & `Flask-SQL-Pro-4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:57:17.274178 Flask-SQL-Pro-4.1/
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:57:17.273475 Flask-SQL-Pro-4.1/Flask_SQL_Pro.egg-info/
--rw-r--r--   0 kela       (501) staff       (20)     8905 2023-07-23 23:57:17.000000 Flask-SQL-Pro-4.1/Flask_SQL_Pro.egg-info/PKG-INFO
--rw-r--r--   0 kela       (501) staff       (20)      277 2023-07-23 23:57:17.000000 Flask-SQL-Pro-4.1/Flask_SQL_Pro.egg-info/SOURCES.txt
--rw-r--r--   0 kela       (501) staff       (20)        1 2023-07-23 23:57:17.000000 Flask-SQL-Pro-4.1/Flask_SQL_Pro.egg-info/dependency_links.txt
--rw-r--r--   0 kela       (501) staff       (20)       30 2023-07-23 23:57:17.000000 Flask-SQL-Pro-4.1/Flask_SQL_Pro.egg-info/requires.txt
--rw-r--r--   0 kela       (501) staff       (20)       14 2023-07-23 23:57:17.000000 Flask-SQL-Pro-4.1/Flask_SQL_Pro.egg-info/top_level.txt
--rw-r--r--   0 kela       (501) staff       (20)     8905 2023-07-23 23:57:17.274031 Flask-SQL-Pro-4.1/PKG-INFO
--rw-r--r--   0 kela       (501) staff       (20)     8388 2023-07-23 23:57:05.000000 Flask-SQL-Pro-4.1/README.rst
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:57:17.273847 Flask-SQL-Pro-4.1/flask_sql_pro/
--rw-r--r--   0 kela       (501) staff       (20)     1843 2023-07-23 16:05:44.000000 Flask-SQL-Pro-4.1/flask_sql_pro/__init__.py
--rw-r--r--   0 kela       (501) staff       (20)     9293 2023-07-23 23:53:43.000000 Flask-SQL-Pro-4.1/flask_sql_pro/db.py
--rw-r--r--   0 kela       (501) staff       (20)     6020 2023-07-23 16:21:52.000000 Flask-SQL-Pro-4.1/flask_sql_pro/sql_loader.py
--rw-r--r--   0 kela       (501) staff       (20)       38 2023-07-23 23:57:17.274224 Flask-SQL-Pro-4.1/setup.cfg
--rw-r--r--   0 kela       (501) staff       (20)      816 2023-07-23 23:57:09.000000 Flask-SQL-Pro-4.1/setup.py
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:58:25.497035 Flask-SQL-Pro-4.2/
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:58:25.496260 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/
+-rw-r--r--   0 kela       (501) staff       (20)     8934 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/PKG-INFO
+-rw-r--r--   0 kela       (501) staff       (20)      277 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/SOURCES.txt
+-rw-r--r--   0 kela       (501) staff       (20)        1 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/dependency_links.txt
+-rw-r--r--   0 kela       (501) staff       (20)       30 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/requires.txt
+-rw-r--r--   0 kela       (501) staff       (20)       14 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/top_level.txt
+-rw-r--r--   0 kela       (501) staff       (20)     8934 2023-07-23 23:58:25.496762 Flask-SQL-Pro-4.2/PKG-INFO
+-rw-r--r--   0 kela       (501) staff       (20)     8388 2023-07-23 23:57:05.000000 Flask-SQL-Pro-4.2/README.rst
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:58:25.496591 Flask-SQL-Pro-4.2/flask_sql_pro/
+-rw-r--r--   0 kela       (501) staff       (20)     1843 2023-07-23 16:05:44.000000 Flask-SQL-Pro-4.2/flask_sql_pro/__init__.py
+-rw-r--r--   0 kela       (501) staff       (20)     9293 2023-07-23 23:53:43.000000 Flask-SQL-Pro-4.2/flask_sql_pro/db.py
+-rw-r--r--   0 kela       (501) staff       (20)     6020 2023-07-23 16:21:52.000000 Flask-SQL-Pro-4.2/flask_sql_pro/sql_loader.py
+-rw-r--r--   0 kela       (501) staff       (20)       38 2023-07-23 23:58:25.497098 Flask-SQL-Pro-4.2/setup.cfg
+-rw-r--r--   0 kela       (501) staff       (20)      845 2023-07-23 23:58:13.000000 Flask-SQL-Pro-4.2/setup.py
```

### Comparing `Flask-SQL-Pro-4.1/Flask_SQL_Pro.egg-info/PKG-INFO` & `Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Flask-SQL-Pro
-Version: 4.1
-Summary: 基于Flask-SQLAlchemy, 抽离SQL语句, 使用Jinja2语法实现动态SQL, 支持上下文事务, 支持分页
+Version: 4.2
+Summary: Based on Flask-SQLAlchemy, extract SQL statements, use Jinja2 syntax to achieve dynamic SQL, support contextual transactions, support paging
 Author: miaokela
 Author-email: 2972799448@qq.com
 Maintainer: miaokela
 Maintainer-email: 2972799448@qq.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Flask-SQL-Pro-4.1/PKG-INFO` & `Flask-SQL-Pro-4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Flask-SQL-Pro
-Version: 4.1
-Summary: 基于Flask-SQLAlchemy, 抽离SQL语句, 使用Jinja2语法实现动态SQL, 支持上下文事务, 支持分页
+Version: 4.2
+Summary: Based on Flask-SQLAlchemy, extract SQL statements, use Jinja2 syntax to achieve dynamic SQL, support contextual transactions, support paging
 Author: miaokela
 Author-email: 2972799448@qq.com
 Maintainer: miaokela
 Maintainer-email: 2972799448@qq.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Flask-SQL-Pro-4.1/README.rst` & `Flask-SQL-Pro-4.2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQL-Pro-4.1/flask_sql_pro/__init__.py` & `Flask-SQL-Pro-4.2/flask_sql_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-SQL-Pro-4.1/flask_sql_pro/db.py` & `Flask-SQL-Pro-4.2/flask_sql_pro/db.py`

 * *Files identical despite different names*

### Comparing `Flask-SQL-Pro-4.1/flask_sql_pro/sql_loader.py` & `Flask-SQL-Pro-4.2/flask_sql_pro/sql_loader.py`

 * *Files identical despite different names*

