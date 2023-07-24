# Comparing `tmp/kistipy-0.0.5.tar.gz` & `tmp/kistipy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kistipy-0.0.5.tar", last modified: Mon Jul 24 07:32:31 2023, max compression
+gzip compressed data, was "kistipy-0.0.6.tar", last modified: Mon Jul 24 07:42:38 2023, max compression
```

## Comparing `kistipy-0.0.5.tar` & `kistipy-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:32:31.396538 kistipy-0.0.5/
--rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:32:31.396281 kistipy-0.0.5/PKG-INFO
--rw-r--r--   0 hmc123     (501) staff       (20)     3014 2023-07-24 04:41:04.000000 kistipy-0.0.5/README.md
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:32:31.392423 kistipy-0.0.5/kistipy/
--rw-r--r--   0 hmc123     (501) staff       (20)      187 2023-07-24 07:24:53.000000 kistipy-0.0.5/kistipy/__init__.py
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:32:31.394626 kistipy-0.0.5/kistipy/sdk/
--rw-r--r--   0 hmc123     (501) staff       (20)        0 2023-07-24 07:28:34.000000 kistipy-0.0.5/kistipy/sdk/__init__.py
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:32:31.395064 kistipy-0.0.5/kistipy/sdk/metadata/
--rw-r--r--   0 hmc123     (501) staff       (20)        0 2023-07-24 07:28:23.000000 kistipy-0.0.5/kistipy/sdk/metadata/__init__.py
--rw-r--r--   0 hmc123     (501) staff       (20)      416 2023-07-20 14:14:38.000000 kistipy-0.0.5/kistipy/sdk/metadata/store.py
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:32:31.395735 kistipy-0.0.5/kistipy/sdk/type/
--rw-r--r--   0 hmc123     (501) staff       (20)        0 2023-07-24 07:28:27.000000 kistipy-0.0.5/kistipy/sdk/type/__init__.py
--rw-r--r--   0 hmc123     (501) staff       (20)      871 2023-07-20 14:14:45.000000 kistipy-0.0.5/kistipy/sdk/type/common.py
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:32:31.394325 kistipy-0.0.5/kistipy.egg-info/
--rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:32:30.000000 kistipy-0.0.5/kistipy.egg-info/PKG-INFO
--rw-r--r--   0 hmc123     (501) staff       (20)      335 2023-07-24 07:32:31.000000 kistipy-0.0.5/kistipy.egg-info/SOURCES.txt
--rw-r--r--   0 hmc123     (501) staff       (20)        1 2023-07-24 07:32:31.000000 kistipy-0.0.5/kistipy.egg-info/dependency_links.txt
--rw-r--r--   0 hmc123     (501) staff       (20)       22 2023-07-24 07:32:31.000000 kistipy-0.0.5/kistipy.egg-info/requires.txt
--rw-r--r--   0 hmc123     (501) staff       (20)        8 2023-07-24 07:32:31.000000 kistipy-0.0.5/kistipy.egg-info/top_level.txt
--rw-r--r--   0 hmc123     (501) staff       (20)       38 2023-07-24 07:32:31.396639 kistipy-0.0.5/setup.cfg
--rw-r--r--   0 hmc123     (501) staff       (20)      623 2023-07-24 07:32:18.000000 kistipy-0.0.5/setup.py
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:42:38.925440 kistipy-0.0.6/
+-rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:42:38.925197 kistipy-0.0.6/PKG-INFO
+-rw-r--r--   0 hmc123     (501) staff       (20)     3014 2023-07-24 04:41:04.000000 kistipy-0.0.6/README.md
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:42:38.922659 kistipy-0.0.6/kistipy/
+-rw-r--r--   0 hmc123     (501) staff       (20)      187 2023-07-24 07:24:53.000000 kistipy-0.0.6/kistipy/__init__.py
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:42:38.924052 kistipy-0.0.6/kistipy/sdk/
+-rw-r--r--   0 hmc123     (501) staff       (20)        0 2023-07-24 07:28:34.000000 kistipy-0.0.6/kistipy/sdk/__init__.py
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:42:38.924404 kistipy-0.0.6/kistipy/sdk/metadata/
+-rw-r--r--   0 hmc123     (501) staff       (20)        0 2023-07-24 07:28:23.000000 kistipy-0.0.6/kistipy/sdk/metadata/__init__.py
+-rw-r--r--   0 hmc123     (501) staff       (20)      428 2023-07-24 07:40:11.000000 kistipy-0.0.6/kistipy/sdk/metadata/store.py
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:42:38.924839 kistipy-0.0.6/kistipy/sdk/type/
+-rw-r--r--   0 hmc123     (501) staff       (20)        0 2023-07-24 07:28:27.000000 kistipy-0.0.6/kistipy/sdk/type/__init__.py
+-rw-r--r--   0 hmc123     (501) staff       (20)      871 2023-07-20 14:14:45.000000 kistipy-0.0.6/kistipy/sdk/type/common.py
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:42:38.923805 kistipy-0.0.6/kistipy.egg-info/
+-rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:42:38.000000 kistipy-0.0.6/kistipy.egg-info/PKG-INFO
+-rw-r--r--   0 hmc123     (501) staff       (20)      335 2023-07-24 07:42:38.000000 kistipy-0.0.6/kistipy.egg-info/SOURCES.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)        1 2023-07-24 07:42:38.000000 kistipy-0.0.6/kistipy.egg-info/dependency_links.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)       22 2023-07-24 07:42:38.000000 kistipy-0.0.6/kistipy.egg-info/requires.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)        8 2023-07-24 07:42:38.000000 kistipy-0.0.6/kistipy.egg-info/top_level.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)       38 2023-07-24 07:42:38.925525 kistipy-0.0.6/setup.cfg
+-rw-r--r--   0 hmc123     (501) staff       (20)      623 2023-07-24 07:41:36.000000 kistipy-0.0.6/setup.py
```

### Comparing `kistipy-0.0.5/PKG-INFO` & `kistipy-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kistipy
-Version: 0.0.5
+Version: 0.0.6
 Summary: kistipy
 Home-page: https://github.com/prosopher/kistipy
 Author: prosopher
 Author-email: prosopher@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kistipy-0.0.5/README.md` & `kistipy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kistipy-0.0.5/kistipy/sdk/type/common.py` & `kistipy-0.0.6/kistipy/sdk/type/common.py`

 * *Files identical despite different names*

### Comparing `kistipy-0.0.5/kistipy.egg-info/PKG-INFO` & `kistipy-0.0.6/kistipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kistipy
-Version: 0.0.5
+Version: 0.0.6
 Summary: kistipy
 Home-page: https://github.com/prosopher/kistipy
 Author: prosopher
 Author-email: prosopher@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kistipy-0.0.5/setup.py` & `kistipy-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='kistipy',
-    version='0.0.5',
+    version='0.0.6',
     author='prosopher',
     author_email='prosopher@gmail.com',
     description='kistipy',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/prosopher/kistipy',
     install_requires=['datasets', 'numpy', 'pandas'],
```

