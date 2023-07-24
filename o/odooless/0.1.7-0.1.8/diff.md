# Comparing `tmp/odooless-0.1.7.tar.gz` & `tmp/odooless-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odooless-0.1.7.tar", last modified: Sat Jul 22 17:48:54 2023, max compression
+gzip compressed data, was "odooless-0.1.8.tar", last modified: Mon Jul 24 00:41:46 2023, max compression
```

## Comparing `odooless-0.1.7.tar` & `odooless-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:48:54.239889 odooless-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 17:48:54.239889 odooless-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-22 17:48:42.000000 odooless-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:48:54.239889 odooless-0.1.7/odooless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:48:42.000000 odooless-0.1.7/odooless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-22 17:48:42.000000 odooless-0.1.7/odooless/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    35379 2023-07-22 17:48:42.000000 odooless-0.1.7/odooless/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:48:54.239889 odooless-0.1.7/odooless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 17:48:54.000000 odooless-0.1.7/odooless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-22 17:48:54.000000 odooless-0.1.7/odooless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 17:48:54.000000 odooless-0.1.7/odooless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 17:48:54.000000 odooless-0.1.7/odooless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 17:48:54.000000 odooless-0.1.7/odooless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 17:48:54.239889 odooless-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-22 17:48:42.000000 odooless-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:41:46.762802 odooless-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 00:41:46.762802 odooless-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-24 00:41:31.000000 odooless-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:41:46.758803 odooless-0.1.8/odooless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:41:31.000000 odooless-0.1.8/odooless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-24 00:41:31.000000 odooless-0.1.8/odooless/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35388 2023-07-24 00:41:31.000000 odooless-0.1.8/odooless/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:41:46.762802 odooless-0.1.8/odooless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:41:46.762802 odooless-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 00:41:31.000000 odooless-0.1.8/setup.py
```

### Comparing `odooless-0.1.7/PKG-INFO` & `odooless-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.7
+Version: 0.1.8
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.7/README.md` & `odooless-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `odooless-0.1.7/odooless/models.py` & `odooless-0.1.8/odooless/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 import uuid
 import json
 
-from clients import resource, client
+from odooless.clients import resource, client
 
 defaultFields = ['id', 'createdAt', 'updatedAt', 'deleted']
 
 
 def create_table(
         TableName=None,  # required
         Fields=None,
```

### Comparing `odooless-0.1.7/odooless.egg-info/PKG-INFO` & `odooless-0.1.8/odooless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.7
+Version: 0.1.8
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.7/setup.py` & `odooless-0.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='odooless',
-    version='0.1.7',
+    version='0.1.8',
     description='A DynamoDB ORM inspired by Odoo',
     long_description='A DynamoDB ORM inspired by Odoo',
     author='Sam Hasan',
     author_email='sam@barameg.co',
     url='https://github.com/Barameg/odooless.git',
     packages=find_packages(),
     classifiers=[
```

