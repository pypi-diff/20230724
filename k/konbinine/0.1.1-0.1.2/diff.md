# Comparing `tmp/konbinine-0.1.1.tar.gz` & `tmp/konbinine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konbinine-0.1.1.tar", last modified: Mon Jul 24 08:56:46 2023, max compression
+gzip compressed data, was "konbinine-0.1.2.tar", last modified: Mon Jul 24 09:07:07 2023, max compression
```

## Comparing `konbinine-0.1.1.tar` & `konbinine-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 08:56:46.360035 konbinine-0.1.1/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.1/LICENSE
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 08:56:46.360035 konbinine-0.1.1/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1408 2023-07-24 08:53:23.000000 konbinine-0.1.1/README.md
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 08:56:46.360035 konbinine-0.1.1/konbinine/
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 08:56:46.360035 konbinine-0.1.1/konbinine/konbinine.egg-info/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 08:56:46.000000 konbinine-0.1.1/konbinine/konbinine.egg-info/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      255 2023-07-24 08:56:46.000000 konbinine-0.1.1/konbinine/konbinine.egg-info/SOURCES.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 08:56:46.000000 konbinine-0.1.1/konbinine/konbinine.egg-info/dependency_links.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-24 08:56:46.000000 konbinine-0.1.1/konbinine/konbinine.egg-info/requires.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 08:56:46.000000 konbinine-0.1.1/konbinine/konbinine.egg-info/top_level.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1333 2023-07-24 08:53:23.000000 konbinine-0.1.1/pyproject.toml
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 08:56:46.360035 konbinine-0.1.1/setup.cfg
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1636 2023-07-24 08:54:59.000000 konbinine-0.1.1/setup.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:07:07.670057 konbinine-0.1.2/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.2/LICENSE
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 09:07:07.670057 konbinine-0.1.2/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1408 2023-07-24 08:53:23.000000 konbinine-0.1.2/README.md
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:07:07.670057 konbinine-0.1.2/konbinine/
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:07:07.670057 konbinine-0.1.2/konbinine/konbinine.egg-info/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      255 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/SOURCES.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/dependency_links.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/requires.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/top_level.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1333 2023-07-24 08:53:23.000000 konbinine-0.1.2/pyproject.toml
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:07:07.670057 konbinine-0.1.2/setup.cfg
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1636 2023-07-24 08:54:59.000000 konbinine-0.1.2/setup.py
```

### Comparing `konbinine-0.1.1/LICENSE` & `konbinine-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.1/PKG-INFO` & `konbinine-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.1
+Version: 0.1.2
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
```

### Comparing `konbinine-0.1.1/README.md` & `konbinine-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.1/konbinine/konbinine.egg-info/PKG-INFO` & `konbinine-0.1.2/konbinine/konbinine.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.1
+Version: 0.1.2
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
```

### Comparing `konbinine-0.1.1/pyproject.toml` & `konbinine-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.1/setup.py` & `konbinine-0.1.2/setup.py`

 * *Files identical despite different names*

