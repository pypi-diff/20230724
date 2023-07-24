# Comparing `tmp/syscolouringpkgV2-1.0.0.tar.gz` & `tmp/syscolouringpkgV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscolouringpkgV2-1.0.0.tar", last modified: Mon Jul 24 00:42:13 2023, max compression
+gzip compressed data, was "syscolouringpkgV2-1.1.0.tar", last modified: Mon Jul 24 00:44:18 2023, max compression
```

## Comparing `syscolouringpkgV2-1.0.0.tar` & `syscolouringpkgV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:42:13.648573 syscolouringpkgV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-24 00:42:13.648573 syscolouringpkgV2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 00:42:13.648573 syscolouringpkgV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-07-24 00:42:13.000000 syscolouringpkgV2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:42:13.648573 syscolouringpkgV2-1.0.0/syscolouringpkgV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 00:42:13.000000 syscolouringpkgV2-1.0.0/syscolouringpkgV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:42:13.648573 syscolouringpkgV2-1.0.0/syscolouringpkgV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-24 00:42:13.000000 syscolouringpkgV2-1.0.0/syscolouringpkgV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-24 00:42:13.000000 syscolouringpkgV2-1.0.0/syscolouringpkgV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:42:13.000000 syscolouringpkgV2-1.0.0/syscolouringpkgV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 00:42:13.000000 syscolouringpkgV2-1.0.0/syscolouringpkgV2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:44:18.636479 syscolouringpkgV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-24 00:44:18.636479 syscolouringpkgV2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 00:44:18.636479 syscolouringpkgV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-07-24 00:44:18.000000 syscolouringpkgV2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:44:18.636479 syscolouringpkgV2-1.1.0/syscolouringpkgV2/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-24 00:44:18.000000 syscolouringpkgV2-1.1.0/syscolouringpkgV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 00:44:18.636479 syscolouringpkgV2-1.1.0/syscolouringpkgV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-24 00:44:18.000000 syscolouringpkgV2-1.1.0/syscolouringpkgV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-24 00:44:18.000000 syscolouringpkgV2-1.1.0/syscolouringpkgV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 00:44:18.000000 syscolouringpkgV2-1.1.0/syscolouringpkgV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 00:44:18.000000 syscolouringpkgV2-1.1.0/syscolouringpkgV2.egg-info/top_level.txt
```

### Comparing `syscolouringpkgV2-1.0.0/setup.py` & `syscolouringpkgV2-1.1.0/setup.py`

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
     name="syscolouringpkgV2",
     version=VERSION,
```

