# Comparing `tmp/konbinine-0.1.2.tar.gz` & `tmp/konbinine-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konbinine-0.1.2.tar", last modified: Mon Jul 24 09:07:07 2023, max compression
+gzip compressed data, was "konbinine-0.1.3.tar", last modified: Mon Jul 24 09:52:07 2023, max compression
```

## Comparing `konbinine-0.1.2.tar` & `konbinine-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:07:07.670057 konbinine-0.1.2/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.2/LICENSE
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 09:07:07.670057 konbinine-0.1.2/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1408 2023-07-24 08:53:23.000000 konbinine-0.1.2/README.md
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:07:07.670057 konbinine-0.1.2/konbinine/
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:07:07.670057 konbinine-0.1.2/konbinine/konbinine.egg-info/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      255 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/SOURCES.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/dependency_links.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/requires.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:07:07.000000 konbinine-0.1.2/konbinine/konbinine.egg-info/top_level.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1333 2023-07-24 08:53:23.000000 konbinine-0.1.2/pyproject.toml
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:07:07.670057 konbinine-0.1.2/setup.cfg
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1636 2023-07-24 08:54:59.000000 konbinine-0.1.2/setup.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:52:07.519967 konbinine-0.1.3/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.3/LICENSE
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 09:52:07.519967 konbinine-0.1.3/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1408 2023-07-24 08:53:23.000000 konbinine-0.1.3/README.md
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:52:07.509967 konbinine-0.1.3/konbinine/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)    27357 2023-07-24 09:26:46.000000 konbinine-0.1.3/konbinine/__init__.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      873 2023-06-29 09:15:35.000000 konbinine-0.1.3/konbinine/enums.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      392 2023-07-03 01:33:22.000000 konbinine-0.1.3/konbinine/exceptions.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      145 2023-07-03 01:33:22.000000 konbinine-0.1.3/konbinine/logs.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     7084 2023-07-24 08:53:23.000000 konbinine-0.1.3/konbinine/models.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      487 2023-06-29 09:15:35.000000 konbinine-0.1.3/konbinine/utils.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 09:52:07.519967 konbinine-0.1.3/konbinine.egg-info/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     3730 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      382 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/SOURCES.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/dependency_links.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/requires.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       10 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/top_level.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.3/konbinine.egg-info/zip-safe
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1325 2023-07-24 09:52:01.000000 konbinine-0.1.3/pyproject.toml
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-07 02:46:56.000000 konbinine-0.1.3/requirements.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1058 2023-07-24 09:52:07.519967 konbinine-0.1.3/setup.cfg
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:47:46.000000 konbinine-0.1.3/setup.py
```

### Comparing `konbinine-0.1.2/LICENSE` & `konbinine-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.2/PKG-INFO` & `konbinine-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.2
+Version: 0.1.3
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
```

### Comparing `konbinine-0.1.2/README.md` & `konbinine-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.2/konbinine/konbinine.egg-info/PKG-INFO` & `konbinine-0.1.3/konbinine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.2
+Version: 0.1.3
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
```

### Comparing `konbinine-0.1.2/pyproject.toml` & `konbinine-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
 [project.urls]
 "Homepage" = "https://github.com/hueyyeng/konbini"
 "Bug Reports" = "https://github.com/hueyyeng/konbini/issues"
 "Source" = "https://github.com/hueyyeng/konbini"
 
 [build-system]
-requires = ["setuptools >= 61.0.0"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools.packages.find]
-where = ["konbinine"]
+#[tool.setuptools.packages.find]
+#where = ["konbinine"]
 
 [tool.setuptools.dynamic]
 version = {attr = "konbinine.__version__"}
 dependencies = {file = "requirements.txt"}
```

