# Comparing `tmp/pyfontstools-1.0.0.tar.gz` & `tmp/pyfontstools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfontstools-1.0.0.tar", last modified: Mon Jul 24 18:14:29 2023, max compression
+gzip compressed data, was "pyfontstools-1.1.0.tar", last modified: Mon Jul 24 18:16:34 2023, max compression
```

## Comparing `pyfontstools-1.0.0.tar` & `pyfontstools-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:14:29.347275 pyfontstools-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-24 18:14:29.347275 pyfontstools-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:14:29.343275 pyfontstools-1.0.0/pyfontstools/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 18:14:28.000000 pyfontstools-1.0.0/pyfontstools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:14:29.347275 pyfontstools-1.0.0/pyfontstools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-24 18:14:29.000000 pyfontstools-1.0.0/pyfontstools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-24 18:14:29.000000 pyfontstools-1.0.0/pyfontstools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 18:14:29.000000 pyfontstools-1.0.0/pyfontstools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 18:14:29.000000 pyfontstools-1.0.0/pyfontstools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 18:14:29.347275 pyfontstools-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-24 18:14:28.000000 pyfontstools-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:16:34.318800 pyfontstools-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-24 18:16:34.318800 pyfontstools-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:16:34.314800 pyfontstools-1.1.0/pyfontstools/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-24 18:16:33.000000 pyfontstools-1.1.0/pyfontstools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 18:16:34.318800 pyfontstools-1.1.0/pyfontstools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-24 18:16:34.000000 pyfontstools-1.1.0/pyfontstools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-24 18:16:34.000000 pyfontstools-1.1.0/pyfontstools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 18:16:34.000000 pyfontstools-1.1.0/pyfontstools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 18:16:34.000000 pyfontstools-1.1.0/pyfontstools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 18:16:34.318800 pyfontstools-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-24 18:16:33.000000 pyfontstools-1.1.0/setup.py
```

### Comparing `pyfontstools-1.0.0/setup.py` & `pyfontstools-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pyfontstools",
     version=VERSION,
```

