# Comparing `tmp/swordartonline-2.2.8.tar.gz` & `tmp/swordartonline-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swordartonline-2.2.8.tar", last modified: Mon Jul 24 11:28:05 2023, max compression
+gzip compressed data, was "swordartonline-2.2.9.tar", last modified: Mon Jul 24 11:32:08 2023, max compression
```

## Comparing `swordartonline-2.2.8.tar` & `swordartonline-2.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 ucat      (1000) ucat      (1000)        0 2023-07-24 11:28:05.634588 swordartonline-2.2.8/
--rw-r--r--   0 ucat      (1000) ucat      (1000)      380 2023-07-24 11:28:05.634588 swordartonline-2.2.8/PKG-INFO
--rw-r--r--   0 ucat      (1000) ucat      (1000)       34 2023-07-24 11:21:39.000000 swordartonline-2.2.8/README.md
--rw-r--r--   0 ucat      (1000) ucat      (1000)       38 2023-07-24 11:28:05.634588 swordartonline-2.2.8/setup.cfg
--rw-r--r--   0 ucat      (1000) ucat      (1000)      665 2023-07-24 11:24:58.000000 swordartonline-2.2.8/setup.py
-drwxr-xr-x   0 ucat      (1000) ucat      (1000)        0 2023-07-24 11:28:05.633588 swordartonline-2.2.8/src/
-drwxr-xr-x   0 ucat      (1000) ucat      (1000)        0 2023-07-24 11:28:05.634588 swordartonline-2.2.8/src/swordartonline.egg-info/
--rw-r--r--   0 ucat      (1000) ucat      (1000)      380 2023-07-24 11:28:05.000000 swordartonline-2.2.8/src/swordartonline.egg-info/PKG-INFO
--rw-r--r--   0 ucat      (1000) ucat      (1000)      186 2023-07-24 11:28:05.000000 swordartonline-2.2.8/src/swordartonline.egg-info/SOURCES.txt
--rw-r--r--   0 ucat      (1000) ucat      (1000)        1 2023-07-24 11:28:05.000000 swordartonline-2.2.8/src/swordartonline.egg-info/dependency_links.txt
--rw-r--r--   0 ucat      (1000) ucat      (1000)        1 2023-07-24 11:28:05.000000 swordartonline-2.2.8/src/swordartonline.egg-info/top_level.txt
+drwxr-xr-x   0 ucat      (1000) ucat      (1000)        0 2023-07-24 11:32:08.462566 swordartonline-2.2.9/
+-rw-r--r--   0 ucat      (1000) ucat      (1000)      380 2023-07-24 11:32:08.461566 swordartonline-2.2.9/PKG-INFO
+-rw-r--r--   0 ucat      (1000) ucat      (1000)       34 2023-07-24 11:21:39.000000 swordartonline-2.2.9/README.md
+-rw-r--r--   0 ucat      (1000) ucat      (1000)       38 2023-07-24 11:32:08.462566 swordartonline-2.2.9/setup.cfg
+-rw-r--r--   0 ucat      (1000) ucat      (1000)      665 2023-07-24 11:31:56.000000 swordartonline-2.2.9/setup.py
+drwxr-xr-x   0 ucat      (1000) ucat      (1000)        0 2023-07-24 11:32:08.457566 swordartonline-2.2.9/src/
+drwxr-xr-x   0 ucat      (1000) ucat      (1000)        0 2023-07-24 11:32:08.461566 swordartonline-2.2.9/src/swordartonline.egg-info/
+-rw-r--r--   0 ucat      (1000) ucat      (1000)      380 2023-07-24 11:32:08.000000 swordartonline-2.2.9/src/swordartonline.egg-info/PKG-INFO
+-rw-r--r--   0 ucat      (1000) ucat      (1000)      186 2023-07-24 11:32:08.000000 swordartonline-2.2.9/src/swordartonline.egg-info/SOURCES.txt
+-rw-r--r--   0 ucat      (1000) ucat      (1000)        1 2023-07-24 11:32:08.000000 swordartonline-2.2.9/src/swordartonline.egg-info/dependency_links.txt
+-rw-r--r--   0 ucat      (1000) ucat      (1000)        1 2023-07-24 11:32:08.000000 swordartonline-2.2.9/src/swordartonline.egg-info/top_level.txt
```

### Comparing `swordartonline-2.2.8/setup.py` & `swordartonline-2.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="swordartonline",
-    version="2.2.8",
+    version="2.2.9",
     author="Orange Alice",
     author_email="author@example.com",
     description="Sample package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

