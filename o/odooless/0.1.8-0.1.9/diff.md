# Comparing `tmp/odooless-0.1.8.tar.gz` & `tmp/odooless-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odooless-0.1.8.tar", last modified: Mon Jul 24 00:41:46 2023, max compression
+gzip compressed data, was "odooless-0.1.9.tar", last modified: Mon Jul 24 00:46:20 2023, max compression
```

## Comparing `odooless-0.1.8.tar` & `odooless-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:41:46.762802 odooless-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 00:41:46.762802 odooless-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-24 00:41:31.000000 odooless-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:41:46.758803 odooless-0.1.8/odooless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:41:31.000000 odooless-0.1.8/odooless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-24 00:41:31.000000 odooless-0.1.8/odooless/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    35388 2023-07-24 00:41:31.000000 odooless-0.1.8/odooless/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:41:46.762802 odooless-0.1.8/odooless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 00:41:46.000000 odooless-0.1.8/odooless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:41:46.762802 odooless-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 00:41:31.000000 odooless-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:46:20.262842 odooless-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 00:46:20.262842 odooless-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-24 00:46:07.000000 odooless-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:46:20.258842 odooless-0.1.9/odooless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:46:07.000000 odooless-0.1.9/odooless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-24 00:46:07.000000 odooless-0.1.9/odooless/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35388 2023-07-24 00:46:07.000000 odooless-0.1.9/odooless/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:46:20.258842 odooless-0.1.9/odooless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 00:46:20.000000 odooless-0.1.9/odooless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 00:46:20.000000 odooless-0.1.9/odooless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:46:20.000000 odooless-0.1.9/odooless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 00:46:20.000000 odooless-0.1.9/odooless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 00:46:20.000000 odooless-0.1.9/odooless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:46:20.262842 odooless-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 00:46:07.000000 odooless-0.1.9/setup.py
```

### Comparing `odooless-0.1.8/PKG-INFO` & `odooless-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.8
+Version: 0.1.9
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.8/README.md` & `odooless-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `odooless-0.1.8/odooless/models.py` & `odooless-0.1.9/odooless/models.py`

 * *Files identical despite different names*

### Comparing `odooless-0.1.8/odooless.egg-info/PKG-INFO` & `odooless-0.1.9/odooless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.8
+Version: 0.1.9
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.8/setup.py` & `odooless-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='odooless',
-    version='0.1.8',
+    version='0.1.9',
     description='A DynamoDB ORM inspired by Odoo',
     long_description='A DynamoDB ORM inspired by Odoo',
     author='Sam Hasan',
     author_email='sam@barameg.co',
     url='https://github.com/Barameg/odooless.git',
     packages=find_packages(),
     classifiers=[
```

