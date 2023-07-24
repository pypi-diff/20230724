# Comparing `tmp/pythoncoloringpackage-1.0.0.tar.gz` & `tmp/pythoncoloringpackage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoloringpackage-1.0.0.tar", last modified: Mon Jul 24 21:36:38 2023, max compression
+gzip compressed data, was "pythoncoloringpackage-1.1.0.tar", last modified: Mon Jul 24 21:38:42 2023, max compression
```

## Comparing `pythoncoloringpackage-1.0.0.tar` & `pythoncoloringpackage-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:36:38.030267 pythoncoloringpackage-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-24 21:36:38.026267 pythoncoloringpackage-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:36:38.026267 pythoncoloringpackage-1.0.0/pipcolortoolsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 pythoncoloringpackage-1.0.0/pipcolortoolsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:36:38.026267 pythoncoloringpackage-1.0.0/pythoncoloringpackage/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:36:37.000000 pythoncoloringpackage-1.0.0/pythoncoloringpackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:36:38.026267 pythoncoloringpackage-1.0.0/pythoncoloringpackage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-24 21:36:37.000000 pythoncoloringpackage-1.0.0/pythoncoloringpackage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2023-07-24 21:36:37.000000 pythoncoloringpackage-1.0.0/pythoncoloringpackage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:36:37.000000 pythoncoloringpackage-1.0.0/pythoncoloringpackage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 21:36:37.000000 pythoncoloringpackage-1.0.0/pythoncoloringpackage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 21:36:38.030267 pythoncoloringpackage-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      567 2023-07-24 21:36:37.000000 pythoncoloringpackage-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:42.395815 pythoncoloringpackage-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-24 21:38:42.391815 pythoncoloringpackage-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:42.391815 pythoncoloringpackage-1.1.0/pipcolortoolsV2/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 pythoncoloringpackage-1.1.0/pipcolortoolsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:42.391815 pythoncoloringpackage-1.1.0/pythoncoloringpackage/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-24 21:38:42.000000 pythoncoloringpackage-1.1.0/pythoncoloringpackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:38:42.391815 pythoncoloringpackage-1.1.0/pythoncoloringpackage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-24 21:38:42.000000 pythoncoloringpackage-1.1.0/pythoncoloringpackage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-24 21:38:42.000000 pythoncoloringpackage-1.1.0/pythoncoloringpackage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:38:42.000000 pythoncoloringpackage-1.1.0/pythoncoloringpackage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 21:38:42.000000 pythoncoloringpackage-1.1.0/pythoncoloringpackage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 21:38:42.395815 pythoncoloringpackage-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      567 2023-07-24 21:38:42.000000 pythoncoloringpackage-1.1.0/setup.py
```

### Comparing `pythoncoloringpackage-1.0.0/setup.py` & `pythoncoloringpackage-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncoloringpackage",
     version=VERSION,
```

