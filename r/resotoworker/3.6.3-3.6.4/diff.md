# Comparing `tmp/resotoworker-3.6.3.tar.gz` & `tmp/resotoworker-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.6.3.tar", last modified: Mon Jul 24 12:11:12 2023, max compression
+gzip compressed data, was "resotoworker-3.6.4.tar", last modified: Mon Jul 24 18:33:58 2023, max compression
```

## Comparing `resotoworker-3.6.3.tar` & `resotoworker-3.6.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:11:12.463284 resotoworker-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:06:31.000000 resotoworker-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-24 12:11:12.463284 resotoworker-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-24 12:06:31.000000 resotoworker-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 12:06:31.000000 resotoworker-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:11:12.459284 resotoworker-3.6.3/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-24 12:06:31.000000 resotoworker-3.6.3/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:11:12.463284 resotoworker-3.6.3/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-24 12:11:12.000000 resotoworker-3.6.3/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 12:11:12.000000 resotoworker-3.6.3/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:11:12.000000 resotoworker-3.6.3/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 12:11:12.000000 resotoworker-3.6.3/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:07:55.000000 resotoworker-3.6.3/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 12:11:12.000000 resotoworker-3.6.3/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:11:12.000000 resotoworker-3.6.3/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:11:12.467284 resotoworker-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:11:12.463284 resotoworker-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:31.000000 resotoworker-3.6.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 12:06:31.000000 resotoworker-3.6.3/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 12:06:31.000000 resotoworker-3.6.3/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-24 12:06:31.000000 resotoworker-3.6.3/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-24 12:06:31.000000 resotoworker-3.6.3/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-24 12:06:31.000000 resotoworker-3.6.3/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:58.866428 resotoworker-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:29:01.000000 resotoworker-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-24 18:33:58.866428 resotoworker-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-24 18:29:01.000000 resotoworker-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 18:29:01.000000 resotoworker-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:58.866428 resotoworker-3.6.4/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-24 18:29:01.000000 resotoworker-3.6.4/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:58.866428 resotoworker-3.6.4/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-24 18:33:58.000000 resotoworker-3.6.4/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 18:33:58.000000 resotoworker-3.6.4/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:33:58.000000 resotoworker-3.6.4/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 18:33:58.000000 resotoworker-3.6.4/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:30:31.000000 resotoworker-3.6.4/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 18:33:58.000000 resotoworker-3.6.4/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:33:58.000000 resotoworker-3.6.4/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:33:58.866428 resotoworker-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:58.866428 resotoworker-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:29:01.000000 resotoworker-3.6.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 18:29:01.000000 resotoworker-3.6.4/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 18:29:01.000000 resotoworker-3.6.4/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-24 18:29:01.000000 resotoworker-3.6.4/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-24 18:29:01.000000 resotoworker-3.6.4/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-24 18:29:01.000000 resotoworker-3.6.4/test/test_utils.py
```

### Comparing `resotoworker-3.6.3/PKG-INFO` & `resotoworker-3.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.6.3
+Version: 3.6.4
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.6.3/README.md` & `resotoworker-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/pyproject.toml` & `resotoworker-3.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "resotoworker"
-version = "3.6.3"
+version = "3.6.4"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.3",
+    "resotolib==3.6.4",
     "tenacity",
     "CherryPy",
 ]
 
 [project.scripts]
 resotoworker = "resotoworker.__main__:main"
```

### Comparing `resotoworker-3.6.3/resotoworker/__main__.py` & `resotoworker-3.6.4/resotoworker/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/resotoworker/cleanup.py` & `resotoworker-3.6.4/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/resotoworker/collect.py` & `resotoworker-3.6.4/resotoworker/collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/resotoworker/config.py` & `resotoworker-3.6.4/resotoworker/config.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/resotoworker/pluginloader.py` & `resotoworker-3.6.4/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/resotoworker/resotocore.py` & `resotoworker-3.6.4/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/resotoworker/tag.py` & `resotoworker-3.6.4/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/resotoworker/utils.py` & `resotoworker-3.6.4/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.6.4/resotoworker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.6.3
+Version: 3.6.4
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.6.3/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.6.4/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/test/test_args.py` & `resotoworker-3.6.4/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/test/test_collect.py` & `resotoworker-3.6.4/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/test/test_resotocore.py` & `resotoworker-3.6.4/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.3/test/test_utils.py` & `resotoworker-3.6.4/test/test_utils.py`

 * *Files identical despite different names*

