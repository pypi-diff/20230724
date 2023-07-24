# Comparing `tmp/resoto-plugin-onelogin-3.6.3.tar.gz` & `tmp/resoto-plugin-onelogin-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onelogin-3.6.3.tar", last modified: Mon Jul 24 12:11:37 2023, max compression
+gzip compressed data, was "resoto-plugin-onelogin-3.6.4.tar", last modified: Mon Jul 24 18:28:13 2023, max compression
```

## Comparing `resoto-plugin-onelogin-3.6.3.tar` & `resoto-plugin-onelogin-3.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:11:37.256740 resoto-plugin-onelogin-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:08:00.000000 resoto-plugin-onelogin-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-24 12:11:37.256740 resoto-plugin-onelogin-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-24 12:08:00.000000 resoto-plugin-onelogin-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-24 12:08:00.000000 resoto-plugin-onelogin-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:11:37.252740 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-24 12:08:00.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-24 12:08:00.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:11:37.256740 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-24 12:11:37.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-24 12:11:37.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:11:37.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 12:11:37.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:09:25.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 12:11:37.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 12:11:37.000000 resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:11:37.256740 resoto-plugin-onelogin-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:11:37.256740 resoto-plugin-onelogin-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-24 12:08:00.000000 resoto-plugin-onelogin-3.6.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:13.904286 resoto-plugin-onelogin-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:23:42.000000 resoto-plugin-onelogin-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-24 18:28:13.904286 resoto-plugin-onelogin-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-24 18:23:42.000000 resoto-plugin-onelogin-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-24 18:23:42.000000 resoto-plugin-onelogin-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:13.904286 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-24 18:23:42.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-24 18:23:42.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:13.904286 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-24 18:28:13.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-24 18:28:13.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:28:13.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 18:28:13.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:25:30.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 18:28:13.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:28:13.000000 resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:28:13.908286 resoto-plugin-onelogin-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:28:13.904286 resoto-plugin-onelogin-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-24 18:23:42.000000 resoto-plugin-onelogin-3.6.4/test/test_config.py
```

### Comparing `resoto-plugin-onelogin-3.6.3/PKG-INFO` & `resoto-plugin-onelogin-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onelogin
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto OneLogin Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onelogin-3.6.3/pyproject.toml` & `resoto-plugin-onelogin-3.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-onelogin"
 description = "Resoto OneLogin Plugin"
-version = "3.6.3"
+version = "3.6.4"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.3",
+    "resotolib==3.6.4",
     "onelogin==2.0.4",
 ]
 
 [project.entry-points."resoto.plugins"]
 onelogin = "resoto_plugin_onelogin:OneLoginPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin/__init__.py` & `resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onelogin-3.6.3/resoto_plugin_onelogin.egg-info/PKG-INFO` & `resoto-plugin-onelogin-3.6.4/resoto_plugin_onelogin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onelogin
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto OneLogin Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

