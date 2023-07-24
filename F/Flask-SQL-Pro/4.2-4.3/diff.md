# Comparing `tmp/Flask-SQL-Pro-4.2.tar.gz` & `tmp/Flask-SQL-Pro-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SQL-Pro-4.2.tar", last modified: Sun Jul 23 23:58:25 2023, max compression
+gzip compressed data, was "Flask-SQL-Pro-4.3.tar", last modified: Mon Jul 24 00:09:15 2023, max compression
```

## Comparing `Flask-SQL-Pro-4.2.tar` & `Flask-SQL-Pro-4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:58:25.497035 Flask-SQL-Pro-4.2/
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:58:25.496260 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/
--rw-r--r--   0 kela       (501) staff       (20)     8934 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/PKG-INFO
--rw-r--r--   0 kela       (501) staff       (20)      277 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/SOURCES.txt
--rw-r--r--   0 kela       (501) staff       (20)        1 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/dependency_links.txt
--rw-r--r--   0 kela       (501) staff       (20)       30 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/requires.txt
--rw-r--r--   0 kela       (501) staff       (20)       14 2023-07-23 23:58:25.000000 Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/top_level.txt
--rw-r--r--   0 kela       (501) staff       (20)     8934 2023-07-23 23:58:25.496762 Flask-SQL-Pro-4.2/PKG-INFO
--rw-r--r--   0 kela       (501) staff       (20)     8388 2023-07-23 23:57:05.000000 Flask-SQL-Pro-4.2/README.rst
-drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-23 23:58:25.496591 Flask-SQL-Pro-4.2/flask_sql_pro/
--rw-r--r--   0 kela       (501) staff       (20)     1843 2023-07-23 16:05:44.000000 Flask-SQL-Pro-4.2/flask_sql_pro/__init__.py
--rw-r--r--   0 kela       (501) staff       (20)     9293 2023-07-23 23:53:43.000000 Flask-SQL-Pro-4.2/flask_sql_pro/db.py
--rw-r--r--   0 kela       (501) staff       (20)     6020 2023-07-23 16:21:52.000000 Flask-SQL-Pro-4.2/flask_sql_pro/sql_loader.py
--rw-r--r--   0 kela       (501) staff       (20)       38 2023-07-23 23:58:25.497098 Flask-SQL-Pro-4.2/setup.cfg
--rw-r--r--   0 kela       (501) staff       (20)      845 2023-07-23 23:58:13.000000 Flask-SQL-Pro-4.2/setup.py
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-24 00:09:15.761106 Flask-SQL-Pro-4.3/
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-24 00:09:15.759876 Flask-SQL-Pro-4.3/Flask_SQL_Pro.egg-info/
+-rw-r--r--   0 kela       (501) staff       (20)     8934 2023-07-24 00:09:15.000000 Flask-SQL-Pro-4.3/Flask_SQL_Pro.egg-info/PKG-INFO
+-rw-r--r--   0 kela       (501) staff       (20)      277 2023-07-24 00:09:15.000000 Flask-SQL-Pro-4.3/Flask_SQL_Pro.egg-info/SOURCES.txt
+-rw-r--r--   0 kela       (501) staff       (20)        1 2023-07-24 00:09:15.000000 Flask-SQL-Pro-4.3/Flask_SQL_Pro.egg-info/dependency_links.txt
+-rw-r--r--   0 kela       (501) staff       (20)       30 2023-07-24 00:09:15.000000 Flask-SQL-Pro-4.3/Flask_SQL_Pro.egg-info/requires.txt
+-rw-r--r--   0 kela       (501) staff       (20)       14 2023-07-24 00:09:15.000000 Flask-SQL-Pro-4.3/Flask_SQL_Pro.egg-info/top_level.txt
+-rw-r--r--   0 kela       (501) staff       (20)     8934 2023-07-24 00:09:15.760922 Flask-SQL-Pro-4.3/PKG-INFO
+-rw-r--r--   0 kela       (501) staff       (20)     8388 2023-07-24 00:06:08.000000 Flask-SQL-Pro-4.3/README.rst
+drwxr-xr-x   0 kela       (501) staff       (20)        0 2023-07-24 00:09:15.760650 Flask-SQL-Pro-4.3/flask_sql_pro/
+-rw-r--r--   0 kela       (501) staff       (20)     1843 2023-07-24 00:06:08.000000 Flask-SQL-Pro-4.3/flask_sql_pro/__init__.py
+-rw-r--r--   0 kela       (501) staff       (20)     9174 2023-07-24 00:09:06.000000 Flask-SQL-Pro-4.3/flask_sql_pro/db.py
+-rw-r--r--   0 kela       (501) staff       (20)     6020 2023-07-24 00:06:08.000000 Flask-SQL-Pro-4.3/flask_sql_pro/sql_loader.py
+-rw-r--r--   0 kela       (501) staff       (20)       38 2023-07-24 00:09:15.761155 Flask-SQL-Pro-4.3/setup.cfg
+-rw-r--r--   0 kela       (501) staff       (20)      845 2023-07-24 00:08:14.000000 Flask-SQL-Pro-4.3/setup.py
```

### Comparing `Flask-SQL-Pro-4.2/Flask_SQL_Pro.egg-info/PKG-INFO` & `Flask-SQL-Pro-4.3/Flask_SQL_Pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SQL-Pro
-Version: 4.2
+Version: 4.3
 Summary: Based on Flask-SQLAlchemy, extract SQL statements, use Jinja2 syntax to achieve dynamic SQL, support contextual transactions, support paging
 Author: miaokela
 Author-email: 2972799448@qq.com
 Maintainer: miaokela
 Maintainer-email: 2972799448@qq.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Flask-SQL-Pro-4.2/PKG-INFO` & `Flask-SQL-Pro-4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SQL-Pro
-Version: 4.2
+Version: 4.3
 Summary: Based on Flask-SQLAlchemy, extract SQL statements, use Jinja2 syntax to achieve dynamic SQL, support contextual transactions, support paging
 Author: miaokela
 Author-email: 2972799448@qq.com
 Maintainer: miaokela
 Maintainer-email: 2972799448@qq.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Flask-SQL-Pro-4.2/README.rst` & `Flask-SQL-Pro-4.3/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-SQL-Pro-4.2/flask_sql_pro/__init__.py` & `Flask-SQL-Pro-4.3/flask_sql_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-SQL-Pro-4.2/flask_sql_pro/db.py` & `Flask-SQL-Pro-4.3/flask_sql_pro/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,15 @@
         where_str = where_str[0:-5]
         sql += where_str
 
         return sql
 
     @classmethod
     def filter_sql_injection(cls, input_string):
-        sql_injection_keywords = ['DROP', 'SELECT', 'DELETE', 'UPDATE', 'INSERT', 'EXEC', '--', '/*', '*/', 'xp_', 'sp_']
-
-        for keyword in sql_injection_keywords:
+        for keyword in cls.sql_injection_keywords:
             if keyword in input_string.upper():
                 raise ValueError('Keywords that may be at risk for SQL injection:' + keyword)
         return input_string 
 
     @classmethod
     def fullfilled_data(cls, data, where):
         """
```

### Comparing `Flask-SQL-Pro-4.2/flask_sql_pro/sql_loader.py` & `Flask-SQL-Pro-4.3/flask_sql_pro/sql_loader.py`

 * *Files identical despite different names*

### Comparing `Flask-SQL-Pro-4.2/setup.py` & `Flask-SQL-Pro-4.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Flask-SQL-Pro',
-    version='4.2',
+    version='4.3',
     description='Based on Flask-SQLAlchemy, extract SQL statements, use Jinja2 syntax to achieve dynamic SQL, support contextual transactions, support paging',
     long_description=open('README.rst').read(),
     author='miaokela',
     author_email='2972799448@qq.com',
     maintainer='miaokela',
     maintainer_email='2972799448@qq.com',
     packages=find_packages(),
```

