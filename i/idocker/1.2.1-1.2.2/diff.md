# Comparing `tmp/idocker-1.2.1.tar.gz` & `tmp/idocker-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idocker-1.2.1.tar", last modified: Mon Jul 24 02:23:17 2023, max compression
+gzip compressed data, was "idocker-1.2.2.tar", last modified: Mon Jul 24 03:06:20 2023, max compression
```

## Comparing `idocker-1.2.1.tar` & `idocker-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 02:23:17.115595 idocker-1.2.1/
--rw-rw-r--   0 pon       (1001) pon       (1001)     1082 2023-07-21 07:30:42.000000 idocker-1.2.1/LICENSE
--rw-rw-r--   0 pon       (1001) pon       (1001)     4879 2023-07-24 02:23:17.115595 idocker-1.2.1/PKG-INFO
--rw-rw-r--   0 pon       (1001) pon       (1001)     4018 2023-07-21 07:39:04.000000 idocker-1.2.1/README.md
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 02:23:17.111595 idocker-1.2.1/idocker/
--rw-rw-r--   0 pon       (1001) pon       (1001)      101 2023-07-24 02:20:33.000000 idocker-1.2.1/idocker/__init__.py
-drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 02:23:17.115595 idocker-1.2.1/idocker.egg-info/
--rw-rw-r--   0 pon       (1001) pon       (1001)     4879 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/PKG-INFO
--rw-rw-r--   0 pon       (1001) pon       (1001)      244 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/SOURCES.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)        1 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/dependency_links.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       49 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/entry_points.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       18 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/requires.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)        8 2023-07-24 02:23:16.000000 idocker-1.2.1/idocker.egg-info/top_level.txt
--rw-rw-r--   0 pon       (1001) pon       (1001)       38 2023-07-24 02:23:17.119595 idocker-1.2.1/setup.cfg
--rw-rw-r--   0 pon       (1001) pon       (1001)     1290 2023-07-07 01:40:26.000000 idocker-1.2.1/setup.py
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 03:06:20.116954 idocker-1.2.2/
+-rw-rw-r--   0 pon       (1001) pon       (1001)     1082 2023-07-21 07:30:42.000000 idocker-1.2.2/LICENSE
+-rw-rw-r--   0 pon       (1001) pon       (1001)     4879 2023-07-24 03:06:20.116954 idocker-1.2.2/PKG-INFO
+-rw-rw-r--   0 pon       (1001) pon       (1001)     4018 2023-07-21 07:39:04.000000 idocker-1.2.2/README.md
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 03:06:20.116954 idocker-1.2.2/idocker/
+-rw-rw-r--   0 pon       (1001) pon       (1001)      101 2023-07-24 03:05:13.000000 idocker-1.2.2/idocker/__init__.py
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 03:06:20.116954 idocker-1.2.2/idocker/cli/
+-rw-rw-r--   0 pon       (1001) pon       (1001)        0 2023-01-31 02:12:48.000000 idocker-1.2.2/idocker/cli/__init__.py
+-rw-rw-r--   0 pon       (1001) pon       (1001)     4127 2023-07-24 02:21:57.000000 idocker-1.2.2/idocker/cli/main.py
+drwxrwxr-x   0 pon       (1001) pon       (1001)        0 2023-07-24 03:06:20.116954 idocker-1.2.2/idocker.egg-info/
+-rw-rw-r--   0 pon       (1001) pon       (1001)     4879 2023-07-24 03:06:20.000000 idocker-1.2.2/idocker.egg-info/PKG-INFO
+-rw-rw-r--   0 pon       (1001) pon       (1001)      288 2023-07-24 03:06:20.000000 idocker-1.2.2/idocker.egg-info/SOURCES.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)        1 2023-07-24 03:06:20.000000 idocker-1.2.2/idocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       49 2023-07-24 03:06:20.000000 idocker-1.2.2/idocker.egg-info/entry_points.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       18 2023-07-24 03:06:20.000000 idocker-1.2.2/idocker.egg-info/requires.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)        8 2023-07-24 03:06:20.000000 idocker-1.2.2/idocker.egg-info/top_level.txt
+-rw-rw-r--   0 pon       (1001) pon       (1001)       38 2023-07-24 03:06:20.120955 idocker-1.2.2/setup.cfg
+-rw-rw-r--   0 pon       (1001) pon       (1001)     1331 2023-07-24 03:04:33.000000 idocker-1.2.2/setup.py
```

### Comparing `idocker-1.2.1/LICENSE` & `idocker-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idocker-1.2.1/PKG-INFO` & `idocker-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idocker
-Version: 1.2.1
+Version: 1.2.2
 Summary: docker cli with python
 Home-page: https://github.com/ponponon/idocker
 Author: ponponon
 Author-email: 1729303158@qq.com
 Maintainer: ponponon
 Maintainer-email: 1729303158@qq.com
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: idocker Version: 1.2.1 Summary: docker cli with
+Metadata-Version: 2.1 Name: idocker Version: 1.2.2 Summary: docker cli with
 python Home-page: https://github.com/ponponon/idocker Author: ponponon Author-
 email: 1729303158@qq.com Maintainer: ponponon Maintainer-email:
 1729303158@qq.com License: MIT License Platform: all Classifier: Programming
 Language :: Python Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idocker-1.2.1/README.md` & `idocker-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `idocker-1.2.1/idocker.egg-info/PKG-INFO` & `idocker-1.2.2/idocker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idocker
-Version: 1.2.1
+Version: 1.2.2
 Summary: docker cli with python
 Home-page: https://github.com/ponponon/idocker
 Author: ponponon
 Author-email: 1729303158@qq.com
 Maintainer: ponponon
 Maintainer-email: 1729303158@qq.com
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: idocker Version: 1.2.1 Summary: docker cli with
+Metadata-Version: 2.1 Name: idocker Version: 1.2.2 Summary: docker cli with
 python Home-page: https://github.com/ponponon/idocker Author: ponponon Author-
 email: 1729303158@qq.com Maintainer: ponponon Maintainer-email:
 1729303158@qq.com License: MIT License Platform: all Classifier: Programming
 Language :: Python Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idocker-1.2.1/setup.py` & `idocker-1.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import setuptools
+from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 from idocker import VERSION
 
 setuptools.setup(
@@ -14,15 +15,15 @@
     maintainer_email='1729303158@qq.com',
     license='MIT License',
     platforms=["all"],
     description="docker cli with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ponponon/idocker",
-    packages=['idocker'],
+    packages=find_packages(),
     entry_points={
         'console_scripts': [
             'idocker=idocker.cli.main:cli',
         ]
     },
     install_requires=[
         'docker',
```

