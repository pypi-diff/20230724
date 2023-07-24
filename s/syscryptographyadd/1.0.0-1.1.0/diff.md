# Comparing `tmp/syscryptographyadd-1.0.0.tar.gz` & `tmp/syscryptographyadd-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscryptographyadd-1.0.0.tar", last modified: Mon Jul 24 19:16:07 2023, max compression
+gzip compressed data, was "syscryptographyadd-1.1.0.tar", last modified: Mon Jul 24 19:18:12 2023, max compression
```

## Comparing `syscryptographyadd-1.0.0.tar` & `syscryptographyadd-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:16:07.787827 syscryptographyadd-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-24 19:16:07.787827 syscryptographyadd-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 19:16:07.787827 syscryptographyadd-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-24 19:16:07.000000 syscryptographyadd-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:16:07.787827 syscryptographyadd-1.0.0/syscryptographyadd/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 19:16:07.000000 syscryptographyadd-1.0.0/syscryptographyadd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:16:07.787827 syscryptographyadd-1.0.0/syscryptographyadd.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-24 19:16:07.000000 syscryptographyadd-1.0.0/syscryptographyadd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-24 19:16:07.000000 syscryptographyadd-1.0.0/syscryptographyadd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 19:16:07.000000 syscryptographyadd-1.0.0/syscryptographyadd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 19:16:07.000000 syscryptographyadd-1.0.0/syscryptographyadd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:18:12.551382 syscryptographyadd-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-24 19:18:12.551382 syscryptographyadd-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 19:18:12.551382 syscryptographyadd-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-24 19:18:12.000000 syscryptographyadd-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:18:12.551382 syscryptographyadd-1.1.0/syscryptographyadd/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-24 19:18:12.000000 syscryptographyadd-1.1.0/syscryptographyadd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:18:12.551382 syscryptographyadd-1.1.0/syscryptographyadd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-24 19:18:12.000000 syscryptographyadd-1.1.0/syscryptographyadd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-24 19:18:12.000000 syscryptographyadd-1.1.0/syscryptographyadd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 19:18:12.000000 syscryptographyadd-1.1.0/syscryptographyadd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 19:18:12.000000 syscryptographyadd-1.1.0/syscryptographyadd.egg-info/top_level.txt
```

### Comparing `syscryptographyadd-1.0.0/setup.py` & `syscryptographyadd-1.1.0/setup.py`

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
     name="syscryptographyadd",
     version=VERSION,
```

