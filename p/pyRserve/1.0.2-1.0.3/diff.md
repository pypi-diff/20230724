# Comparing `tmp/pyRserve-1.0.2.tar.gz` & `tmp/pyRserve-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRserve-1.0.2.tar", last modified: Mon Jul  3 09:38:49 2023, max compression
+gzip compressed data, was "pyRserve-1.0.3.tar", last modified: Mon Jul 24 20:02:24 2023, max compression
```

## Comparing `pyRserve-1.0.2.tar` & `pyRserve-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-03 09:38:49.582800 pyRserve-1.0.2/
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)     1169 2023-03-28 19:22:37.000000 pyRserve-1.0.2/LICENSE
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)     5492 2023-07-03 09:38:49.582800 pyRserve-1.0.2/PKG-INFO
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)     4088 2023-07-01 11:52:38.000000 pyRserve-1.0.2/README.rst
-drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-03 09:38:49.582800 pyRserve-1.0.2/pyRserve/
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)      563 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/__init__.py
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)     2288 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/misc.py
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)    16449 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rconn.py
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)      485 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rexceptions.py
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)    25642 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rparser.py
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)    17306 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rserializer.py
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)    14652 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rtypes.py
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)    11791 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/taggedContainers.py
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)        6 2023-07-01 14:31:55.000000 pyRserve-1.0.2/pyRserve/version.txt
-drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-03 09:38:49.582800 pyRserve-1.0.2/pyRserve.egg-info/
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)     5492 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/PKG-INFO
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)      389 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/SOURCES.txt
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)        1 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/dependency_links.txt
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)       70 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/requires.txt
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)        9 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/top_level.txt
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)      187 2023-07-03 09:38:49.582800 pyRserve-1.0.2/setup.cfg
--rw-r--r--   0 heinkel   (1000) heinkel   (1000)     2108 2023-07-01 14:29:24.000000 pyRserve-1.0.2/setup.py
+drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-24 20:02:24.261001 pyRserve-1.0.3/
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     1169 2023-03-28 19:22:37.000000 pyRserve-1.0.3/LICENSE
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     5492 2023-07-24 20:02:24.261001 pyRserve-1.0.3/PKG-INFO
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     4088 2023-07-01 11:52:38.000000 pyRserve-1.0.3/README.rst
+drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-24 20:02:24.261001 pyRserve-1.0.3/pyRserve/
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)      563 2023-03-28 19:22:37.000000 pyRserve-1.0.3/pyRserve/__init__.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     2288 2023-03-28 19:22:37.000000 pyRserve-1.0.3/pyRserve/misc.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    16449 2023-03-28 19:22:37.000000 pyRserve-1.0.3/pyRserve/rconn.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)      485 2023-03-28 19:22:37.000000 pyRserve-1.0.3/pyRserve/rexceptions.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    25642 2023-03-28 19:22:37.000000 pyRserve-1.0.3/pyRserve/rparser.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    17306 2023-03-28 19:22:37.000000 pyRserve-1.0.3/pyRserve/rserializer.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    14652 2023-03-28 19:22:37.000000 pyRserve-1.0.3/pyRserve/rtypes.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    11791 2023-03-28 19:22:37.000000 pyRserve-1.0.3/pyRserve/taggedContainers.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)        6 2023-07-24 19:58:11.000000 pyRserve-1.0.3/pyRserve/version.txt
+drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-24 20:02:24.261001 pyRserve-1.0.3/pyRserve.egg-info/
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     5492 2023-07-24 20:02:24.000000 pyRserve-1.0.3/pyRserve.egg-info/PKG-INFO
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)      427 2023-07-24 20:02:24.000000 pyRserve-1.0.3/pyRserve.egg-info/SOURCES.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)        1 2023-07-24 20:02:24.000000 pyRserve-1.0.3/pyRserve.egg-info/dependency_links.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)       70 2023-07-24 20:02:24.000000 pyRserve-1.0.3/pyRserve.egg-info/requires.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)        9 2023-07-24 20:02:24.000000 pyRserve-1.0.3/pyRserve.egg-info/top_level.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)        6 2023-03-28 19:22:37.000000 pyRserve-1.0.3/requirements.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)       53 2023-03-28 19:22:37.000000 pyRserve-1.0.3/requirements_dev.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)      187 2023-07-24 20:02:24.261001 pyRserve-1.0.3/setup.cfg
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     2224 2023-07-24 19:57:01.000000 pyRserve-1.0.3/setup.py
```

### Comparing `pyRserve-1.0.2/LICENSE` & `pyRserve-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/PKG-INFO` & `pyRserve-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRserve
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python client to remotely access the R statistic package via network
 Home-page: https://github.com/ralhei/pyRserve
 Author: Ralph Heinkel
 Author-email: rh@ralph-heinkel.com
 License: MIT license
 Project-URL: Documentation, https://pyrserve.readthedocs.io/
 Project-URL: Changelog, https://pyrserve.readthedocs.io/en/latest/changelog.html
```

### Comparing `pyRserve-1.0.2/README.rst` & `pyRserve-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/pyRserve/__init__.py` & `pyRserve-1.0.3/pyRserve/__init__.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/pyRserve/misc.py` & `pyRserve-1.0.3/pyRserve/misc.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/pyRserve/rconn.py` & `pyRserve-1.0.3/pyRserve/rconn.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/pyRserve/rparser.py` & `pyRserve-1.0.3/pyRserve/rparser.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/pyRserve/rserializer.py` & `pyRserve-1.0.3/pyRserve/rserializer.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/pyRserve/rtypes.py` & `pyRserve-1.0.3/pyRserve/rtypes.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/pyRserve/taggedContainers.py` & `pyRserve-1.0.3/pyRserve/taggedContainers.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.2/pyRserve.egg-info/PKG-INFO` & `pyRserve-1.0.3/pyRserve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRserve
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python client to remotely access the R statistic package via network
 Home-page: https://github.com/ralhei/pyRserve
 Author: Ralph Heinkel
 Author-email: rh@ralph-heinkel.com
 License: MIT license
 Project-URL: Documentation, https://pyrserve.readthedocs.io/
 Project-URL: Changelog, https://pyrserve.readthedocs.io/en/latest/changelog.html
```

### Comparing `pyRserve-1.0.2/setup.py` & `pyRserve-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup
-from pyRserve import __version__
 
 PACKAGE_NAME = "pyRserve"
 
+__version__ = open(os.path.join('pyRserve', 'version.txt')).readline().strip()
 requirements = open('requirements.txt').read().splitlines()
 requirements_testing = open('requirements_dev.txt').read().splitlines()
 
 # Get long_description from intro.txt:
 here = os.path.dirname(os.path.abspath(__file__))
 with open('README.rst') as fp:
     long_description = fp.read()
@@ -30,14 +30,15 @@
     },
     keywords='R Rserve',
     packages=['pyRserve'],
     include_package_data=True,
     package_data={
         'pyRserve': ['version.txt'],
     },
+    data_files=[('.', ['requirements.txt', 'requirements_dev.txt'])],
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4',
     install_requires=requirements,
     extras_require={
         'testing': requirements_testing
     },
     license='MIT license',
     platforms=['unix', 'linux', 'cygwin', 'win32'],
```

