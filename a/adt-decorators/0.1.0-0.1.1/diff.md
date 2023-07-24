# Comparing `tmp/adt-decorators-0.1.0.tar.gz` & `tmp/adt-decorators-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adt-decorators-0.1.0.tar", last modified: Mon Jul 24 10:54:51 2023, max compression
+gzip compressed data, was "adt-decorators-0.1.1.tar", last modified: Mon Jul 24 11:02:22 2023, max compression
```

## Comparing `adt-decorators-0.1.0.tar` & `adt-decorators-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 10:54:51.823544 adt-decorators-0.1.0/
--rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.1.0/LICENSE
--rw-r--r--   0 m0rphism  (1000) users      (100)     3938 2023-07-24 10:54:51.823544 adt-decorators-0.1.0/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)     3514 2023-07-24 10:37:54.000000 adt-decorators-0.1.0/README.md
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 10:54:51.823544 adt-decorators-0.1.0/adt/
--rw-r--r--   0 m0rphism  (1000) users      (100)     4591 2023-07-24 10:31:01.000000 adt-decorators-0.1.0/adt/__init__.py
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 10:54:51.823544 adt-decorators-0.1.0/adt_decorators.egg-info/
--rw-r--r--   0 m0rphism  (1000) users      (100)     3938 2023-07-24 10:54:51.000000 adt-decorators-0.1.0/adt_decorators.egg-info/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)      194 2023-07-24 10:54:51.000000 adt-decorators-0.1.0/adt_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 10:54:51.000000 adt-decorators-0.1.0/adt_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 10:54:51.000000 adt-decorators-0.1.0/adt_decorators.egg-info/top_level.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 10:54:51.823544 adt-decorators-0.1.0/setup.cfg
--rw-r--r--   0 m0rphism  (1000) users      (100)      633 2023-07-24 10:31:00.000000 adt-decorators-0.1.0/setup.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 11:02:22.058579 adt-decorators-0.1.1/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.1.1/LICENSE
+-rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.1.1/MANIFEST.in
+-rw-r--r--   0 m0rphism  (1000) users      (100)     3938 2023-07-24 11:02:22.058579 adt-decorators-0.1.1/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)     3514 2023-07-24 10:37:54.000000 adt-decorators-0.1.1/README.md
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 11:02:22.057579 adt-decorators-0.1.1/adt/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     4591 2023-07-24 11:01:15.000000 adt-decorators-0.1.1/adt/__init__.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 11:02:22.057579 adt-decorators-0.1.1/adt_decorators.egg-info/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     3938 2023-07-24 11:02:22.000000 adt-decorators-0.1.1/adt_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 11:02:22.000000 adt-decorators-0.1.1/adt_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 11:02:22.000000 adt-decorators-0.1.1/adt_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 11:02:22.000000 adt-decorators-0.1.1/adt_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 11:02:22.057579 adt-decorators-0.1.1/docs/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     3514 2023-07-24 10:37:54.000000 adt-decorators-0.1.1/docs/overview.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.1.1/docs/reference.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.1.1/mkdocs.yml
+-rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 11:02:22.058579 adt-decorators-0.1.1/setup.cfg
+-rw-r--r--   0 m0rphism  (1000) users      (100)      633 2023-07-24 11:01:08.000000 adt-decorators-0.1.1/setup.py
```

### Comparing `adt-decorators-0.1.0/LICENSE` & `adt-decorators-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.1.0/PKG-INFO` & `adt-decorators-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.1.0
+Version: 0.1.1
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `adt-decorators-0.1.0/README.md` & `adt-decorators-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.1.0/adt/__init__.py` & `adt-decorators-0.1.1/adt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Provides class decorators for Algebraic Data Types (ADTs)
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = 'Hannes Saffrich'
 
 from dataclasses import dataclass
 import inspect
 
 def adt(Base):
     """Class-decorator for Algebraic Data Types (ADTs), which defines the constructors as static fields of the base type.
```

### Comparing `adt-decorators-0.1.0/adt_decorators.egg-info/PKG-INFO` & `adt-decorators-0.1.1/adt_decorators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.1.0
+Version: 0.1.1
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `adt-decorators-0.1.0/setup.py` & `adt-decorators-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('docs/overview.md', 'r') as f:
     desc = f.read()
 
 setup(
     name='adt-decorators',
-    version='0.1.0',    
+    version='0.1.1',    
     description='Algebraic Data Types via Class Decorators',
     long_description=desc,
     long_description_content_type='text/markdown',
     url='https://github.com/m0rphism/adt-decorators',
     author='Hannes Saffrich',
     author_email='saffrich@informatik.uni-freiburg.de',
     license='BSD 2-clause',
```

