# Comparing `tmp/connectors_to_databases-1.1.0.tar.gz` & `tmp/connectors_to_databases-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectors_to_databases-1.1.0.tar", last modified: Tue Jul 18 05:07:35 2023, max compression
+gzip compressed data, was "connectors_to_databases-1.1.1.tar", last modified: Mon Jul 24 02:08:45 2023, max compression
```

## Comparing `connectors_to_databases-1.1.0.tar` & `connectors_to_databases-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-18 05:07:35.498667 connectors_to_databases-1.1.0/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.1.0/LICENSE.MD
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-18 05:07:35.498545 connectors_to_databases-1.1.0/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1280 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.0/README.md
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-18 05:07:35.497838 connectors_to_databases-1.1.0/connectors_to_databases/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.0/connectors_to_databases/BaseOperator.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1161 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.0/connectors_to_databases/ClickHouse.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     7957 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.0/connectors_to_databases/PostgreSQL.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.1.0/connectors_to_databases/TypeHinting.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      346 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.0/connectors_to_databases/__init__.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      132 2023-07-17 09:59:52.000000 connectors_to_databases-1.1.0/connectors_to_databases/class_use.py
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-18 05:07:35.498387 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/SOURCES.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/dependency_links.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      140 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/requires.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/top_level.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.0/pyproject.toml
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-18 05:07:35.498701 connectors_to_databases-1.1.0/setup.cfg
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1760 2023-07-18 05:06:59.000000 connectors_to_databases-1.1.0/setup.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 02:08:45.676911 connectors_to_databases-1.1.1/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.1.1/LICENSE.MD
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-24 02:08:45.676700 connectors_to_databases-1.1.1/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1280 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.1/README.md
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 02:08:45.675367 connectors_to_databases-1.1.1/connectors_to_databases/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.1/connectors_to_databases/BaseOperator.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1161 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.1/connectors_to_databases/ClickHouse.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     7957 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.1/connectors_to_databases/PostgreSQL.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.1.1/connectors_to_databases/TypeHinting.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      346 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.1/connectors_to_databases/__init__.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      132 2023-07-17 09:59:52.000000 connectors_to_databases-1.1.1/connectors_to_databases/class_use.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-24 02:08:45.676454 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/SOURCES.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/dependency_links.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      124 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/requires.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-24 02:08:45.000000 connectors_to_databases-1.1.1/connectors_to_databases.egg-info/top_level.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.1/pyproject.toml
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-24 02:08:45.676965 connectors_to_databases-1.1.1/setup.cfg
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1762 2023-07-24 02:08:12.000000 connectors_to_databases-1.1.1/setup.py
```

### Comparing `connectors_to_databases-1.1.0/LICENSE.MD` & `connectors_to_databases-1.1.1/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.0/PKG-INFO` & `connectors_to_databases-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectors_to_databases
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python module for connect with PostgreSQL and ClickHouse 
 Home-page: https://github.com/k0rsakov/connectors_to_databases
 Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 Author: k0rsakov
 Author-email: korsakov.iyu@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
```

### Comparing `connectors_to_databases-1.1.0/README.md` & `connectors_to_databases-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.0/connectors_to_databases/BaseOperator.py` & `connectors_to_databases-1.1.1/connectors_to_databases/BaseOperator.py`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.0/connectors_to_databases/ClickHouse.py` & `connectors_to_databases-1.1.1/connectors_to_databases/ClickHouse.py`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.0/connectors_to_databases/PostgreSQL.py` & `connectors_to_databases-1.1.1/connectors_to_databases/PostgreSQL.py`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.0/connectors_to_databases.egg-info/PKG-INFO` & `connectors_to_databases-1.1.1/connectors_to_databases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectors-to-databases
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python module for connect with PostgreSQL and ClickHouse 
 Home-page: https://github.com/k0rsakov/connectors_to_databases
 Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 Author: k0rsakov
 Author-email: korsakov.iyu@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
```

### Comparing `connectors_to_databases-1.1.0/pyproject.toml` & `connectors_to_databases-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.1.0/setup.py` & `connectors_to_databases-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '1.1.0'
+version = '1.1.1'
 
 with open('README.md', encoding='utf-8-sig') as f:
     long_description = f.read()
 
 setup(
     name='connectors_to_databases',
     version=version,
@@ -26,16 +26,16 @@
     license='Apache License, Version 2.0, see LICENSE file',
     
     # TODO: deprecated psycopg2, clickhouse-sqlalchemy
     packages=['connectors_to_databases'],
     install_requires=[
         'SQLAlchemy==1.4.44',
         'pandas==1.5.1',
-        'psycopg2-binary==2.9.6',
-        'psycopg2==2.9.5',
+        'psycopg2-binary==2.9.5',
+        # 'psycopg2==2.9.5',
         'clickhouse-sqlalchemy==0.2.3',
         'clickhouse_driver==0.2.5',
         'ruff==0.0.278',
     ],
 
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
```

