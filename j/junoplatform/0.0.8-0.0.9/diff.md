# Comparing `tmp/junoplatform-0.0.8.tar.gz` & `tmp/junoplatform-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junoplatform-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "junoplatform-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `junoplatform-0.0.8.tar` & `junoplatform-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       31 2023-07-12 03:20:16.720150 junoplatform-0.0.8/.gitignore
--rw-r--r--   0        0        0      507 2023-07-19 05:36:13.410996 junoplatform-0.0.8/README.md
--rw-r--r--   0        0        0      886 2023-07-24 08:15:05.146347 junoplatform-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 08:03:40.679259 junoplatform-0.0.8/src/junoplatform/__init__.py
--rw-r--r--   0        0        0     2180 2023-07-24 07:19:22.526970 junoplatform-0.0.8/src/junoplatform/io/__init__.py
--rw-r--r--   0        0        0     6770 2023-07-24 07:24:03.365887 junoplatform-0.0.8/src/junoplatform/io/_driver.py
--rw-r--r--   0        0        0     2712 2023-07-24 07:31:48.238244 junoplatform-0.0.8/src/junoplatform/io/utils.py
--rw-r--r--   0        0        0        0 2023-07-14 02:04:06.922936 junoplatform-0.0.8/src/junoplatform/meta/__init__.py
--rw-r--r--   0        0        0     2490 2023-07-24 06:40:22.971935 junoplatform-0.0.8/src/junoplatform/meta/decorators.py
--rw-r--r--   0        0        0     1015 2023-07-24 07:20:51.249308 junoplatform-0.0.8/src/junoplatform/templates/main.py
--rw-r--r--   0        0        0        0 2023-07-10 08:39:47.775803 junoplatform-0.0.8/src/junoplatform/tools/__init__.py
--rw-r--r--   0        0        0     6831 2023-07-24 08:02:10.605013 junoplatform-0.0.8/src/junoplatform/tools/cmd.py
--rw-r--r--   0        0        0      163 2023-07-13 05:56:20.979580 junoplatform-0.0.8/tests/fputs.egg-info/PKG-INFO
--rw-r--r--   0        0        0      138 2023-07-13 05:56:20.999580 junoplatform-0.0.8/tests/fputs.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-07-13 05:56:20.979580 junoplatform-0.0.8/tests/fputs.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        6 2023-07-13 05:56:20.979580 junoplatform-0.0.8/tests/fputs.egg-info/top_level.txt
--rw-r--r--   0        0        0       76 2023-07-17 08:32:09.175206 junoplatform-0.0.8/tests/input.json
--rw-r--r--   0        0        0      363 2023-07-13 05:55:54.568005 junoplatform-0.0.8/tests/setup.py
--rw-r--r--   0        0        0      202 2023-07-24 07:10:54.672586 junoplatform-0.0.8/tests/test.py
--rw-r--r--   0        0        0      782 2023-07-17 09:02:02.959111 junoplatform-0.0.8/tests/test_module.c
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 junoplatform-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       31 2023-07-12 03:20:16.720150 junoplatform-0.0.9/.gitignore
+-rw-r--r--   0        0        0      507 2023-07-19 05:36:13.410996 junoplatform-0.0.9/README.md
+-rw-r--r--   0        0        0      907 2023-07-24 08:17:45.176108 junoplatform-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 08:03:40.679259 junoplatform-0.0.9/src/junoplatform/__init__.py
+-rw-r--r--   0        0        0     2180 2023-07-24 07:19:22.526970 junoplatform-0.0.9/src/junoplatform/io/__init__.py
+-rw-r--r--   0        0        0     6770 2023-07-24 07:24:03.365887 junoplatform-0.0.9/src/junoplatform/io/_driver.py
+-rw-r--r--   0        0        0     2712 2023-07-24 07:31:48.238244 junoplatform-0.0.9/src/junoplatform/io/utils.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:04:06.922936 junoplatform-0.0.9/src/junoplatform/meta/__init__.py
+-rw-r--r--   0        0        0     2490 2023-07-24 06:40:22.971935 junoplatform-0.0.9/src/junoplatform/meta/decorators.py
+-rw-r--r--   0        0        0     1015 2023-07-24 07:20:51.249308 junoplatform-0.0.9/src/junoplatform/templates/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:39:47.775803 junoplatform-0.0.9/src/junoplatform/tools/__init__.py
+-rw-r--r--   0        0        0     6831 2023-07-24 08:02:10.605013 junoplatform-0.0.9/src/junoplatform/tools/cmd.py
+-rw-r--r--   0        0        0      163 2023-07-13 05:56:20.979580 junoplatform-0.0.9/tests/fputs.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      138 2023-07-13 05:56:20.999580 junoplatform-0.0.9/tests/fputs.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-07-13 05:56:20.979580 junoplatform-0.0.9/tests/fputs.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        6 2023-07-13 05:56:20.979580 junoplatform-0.0.9/tests/fputs.egg-info/top_level.txt
+-rw-r--r--   0        0        0       76 2023-07-17 08:32:09.175206 junoplatform-0.0.9/tests/input.json
+-rw-r--r--   0        0        0      363 2023-07-13 05:55:54.568005 junoplatform-0.0.9/tests/setup.py
+-rw-r--r--   0        0        0      202 2023-07-24 07:10:54.672586 junoplatform-0.0.9/tests/test.py
+-rw-r--r--   0        0        0      782 2023-07-17 09:02:02.959111 junoplatform-0.0.9/tests/test_module.c
+-rw-r--r--   0        0        0     1369 1970-01-01 00:00:00.000000 junoplatform-0.0.9/PKG-INFO
```

### Comparing `junoplatform-0.0.8/pyproject.toml` & `junoplatform-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project.scripts]
 junocli = "junoplatform.tools.cmd:main"
 
 [project]
 name = "junoplatform"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Bruce.Lu", email="lzbgt@icloud.com" },
 ]
 description = "juno AI platform lib"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -30,12 +30,13 @@
     "pymongo",
     "questdb",
     "postgres",
     "cryptography",
     "bcrypt",
     "redis",
     "pylint",
+    "elasticsearch",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lzbgt/sampleproject"
 "Bug Tracker" = "https://github.com/lzbgt/sampleproject/issues"
```

### Comparing `junoplatform-0.0.8/src/junoplatform/io/__init__.py` & `junoplatform-0.0.9/src/junoplatform/io/__init__.py`

 * *Files identical despite different names*

### Comparing `junoplatform-0.0.8/src/junoplatform/io/_driver.py` & `junoplatform-0.0.9/src/junoplatform/io/_driver.py`

 * *Files identical despite different names*

### Comparing `junoplatform-0.0.8/src/junoplatform/io/utils.py` & `junoplatform-0.0.9/src/junoplatform/io/utils.py`

 * *Files identical despite different names*

### Comparing `junoplatform-0.0.8/src/junoplatform/meta/decorators.py` & `junoplatform-0.0.9/src/junoplatform/meta/decorators.py`

 * *Files identical despite different names*

### Comparing `junoplatform-0.0.8/src/junoplatform/templates/main.py` & `junoplatform-0.0.9/src/junoplatform/templates/main.py`

 * *Files identical despite different names*

### Comparing `junoplatform-0.0.8/src/junoplatform/tools/cmd.py` & `junoplatform-0.0.9/src/junoplatform/tools/cmd.py`

 * *Files identical despite different names*

### Comparing `junoplatform-0.0.8/tests/test_module.c` & `junoplatform-0.0.9/tests/test_module.c`

 * *Files identical despite different names*

### Comparing `junoplatform-0.0.8/PKG-INFO` & `junoplatform-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junoplatform
-Version: 0.0.8
+Version: 0.0.9
 Summary: juno AI platform lib
 Author-email: "Bruce.Lu" <lzbgt@icloud.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Dist: pymongo
 Requires-Dist: questdb
 Requires-Dist: postgres
 Requires-Dist: cryptography
 Requires-Dist: bcrypt
 Requires-Dist: redis
 Requires-Dist: pylint
+Requires-Dist: elasticsearch
 Project-URL: Bug Tracker, https://github.com/lzbgt/sampleproject/issues
 Project-URL: Homepage, https://github.com/lzbgt/sampleproject
 
 # Juno Platform
 
 ## Description
```

