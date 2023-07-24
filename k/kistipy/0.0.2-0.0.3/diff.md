# Comparing `tmp/kistipy-0.0.2.tar.gz` & `tmp/kistipy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kistipy-0.0.2.tar", last modified: Mon Jul 24 07:05:27 2023, max compression
+gzip compressed data, was "kistipy-0.0.3.tar", last modified: Mon Jul 24 07:18:49 2023, max compression
```

## Comparing `kistipy-0.0.2.tar` & `kistipy-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:05:27.614865 kistipy-0.0.2/
--rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:05:27.614631 kistipy-0.0.2/PKG-INFO
-drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:05:27.614314 kistipy-0.0.2/kistipy.egg-info/
--rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:05:27.000000 kistipy-0.0.2/kistipy.egg-info/PKG-INFO
--rw-r--r--   0 hmc123     (501) staff       (20)      132 2023-07-24 07:05:27.000000 kistipy-0.0.2/kistipy.egg-info/SOURCES.txt
--rw-r--r--   0 hmc123     (501) staff       (20)        1 2023-07-24 07:05:27.000000 kistipy-0.0.2/kistipy.egg-info/dependency_links.txt
--rw-r--r--   0 hmc123     (501) staff       (20)        1 2023-07-24 07:05:27.000000 kistipy-0.0.2/kistipy.egg-info/top_level.txt
--rw-r--r--   0 hmc123     (501) staff       (20)       38 2023-07-24 07:05:27.614948 kistipy-0.0.2/setup.cfg
--rw-r--r--   0 hmc123     (501) staff       (20)      576 2023-07-24 07:05:01.000000 kistipy-0.0.2/setup.py
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:18:49.056789 kistipy-0.0.3/
+-rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:18:49.056553 kistipy-0.0.3/PKG-INFO
+-rw-r--r--   0 hmc123     (501) staff       (20)     3014 2023-07-24 04:41:04.000000 kistipy-0.0.3/README.md
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:18:49.055231 kistipy-0.0.3/kistipy/
+-rw-r--r--   0 hmc123     (501) staff       (20)      210 2023-07-24 07:15:36.000000 kistipy-0.0.3/kistipy/__init__.py
+drwxr-xr-x   0 hmc123     (501) staff       (20)        0 2023-07-24 07:18:49.056210 kistipy-0.0.3/kistipy.egg-info/
+-rw-r--r--   0 hmc123     (501) staff       (20)     3381 2023-07-24 07:18:48.000000 kistipy-0.0.3/kistipy.egg-info/PKG-INFO
+-rw-r--r--   0 hmc123     (501) staff       (20)      162 2023-07-24 07:18:49.000000 kistipy-0.0.3/kistipy.egg-info/SOURCES.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)        1 2023-07-24 07:18:48.000000 kistipy-0.0.3/kistipy.egg-info/dependency_links.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)        8 2023-07-24 07:18:48.000000 kistipy-0.0.3/kistipy.egg-info/top_level.txt
+-rw-r--r--   0 hmc123     (501) staff       (20)       38 2023-07-24 07:18:49.056884 kistipy-0.0.3/setup.cfg
+-rw-r--r--   0 hmc123     (501) staff       (20)      568 2023-07-24 07:17:50.000000 kistipy-0.0.3/setup.py
```

### Comparing `kistipy-0.0.2/PKG-INFO` & `kistipy-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kistipy
-Version: 0.0.2
+Version: 0.0.3
 Summary: kistipy
 Home-page: https://github.com/prosopher/kistipy
 Author: prosopher
 Author-email: prosopher@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kistipy-0.0.2/kistipy.egg-info/PKG-INFO` & `kistipy-0.0.3/kistipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kistipy
-Version: 0.0.2
+Version: 0.0.3
 Summary: kistipy
 Home-page: https://github.com/prosopher/kistipy
 Author: prosopher
 Author-email: prosopher@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kistipy-0.0.2/setup.py` & `kistipy-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open("kistipy/README.md", "r") as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kistipy",
-    version="0.0.2",
+    version="0.0.3",
     author="prosopher",
     author_email="prosopher@gmail.com",
     description="kistipy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prosopher/kistipy",
     packages=setuptools.find_packages(),
```

