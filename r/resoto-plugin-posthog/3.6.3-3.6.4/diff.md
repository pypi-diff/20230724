# Comparing `tmp/resoto-plugin-posthog-3.6.3.tar.gz` & `tmp/resoto-plugin-posthog-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-posthog-3.6.3.tar", last modified: Mon Jul 24 12:13:29 2023, max compression
+gzip compressed data, was "resoto-plugin-posthog-3.6.4.tar", last modified: Mon Jul 24 18:32:24 2023, max compression
```

## Comparing `resoto-plugin-posthog-3.6.3.tar` & `resoto-plugin-posthog-3.6.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:29.102378 resoto-plugin-posthog-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:09:08.000000 resoto-plugin-posthog-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-24 12:13:29.102378 resoto-plugin-posthog-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-24 12:09:08.000000 resoto-plugin-posthog-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-24 12:09:08.000000 resoto-plugin-posthog-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:29.102378 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-24 12:09:08.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 12:09:08.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-24 12:09:08.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-24 12:09:08.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:29.102378 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-24 12:13:29.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-24 12:13:29.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:13:29.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 12:13:29.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:10:52.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 12:13:29.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 12:13:29.000000 resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:13:29.106378 resoto-plugin-posthog-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:29.102378 resoto-plugin-posthog-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 12:09:08.000000 resoto-plugin-posthog-3.6.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:24.328945 resoto-plugin-posthog-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:27:35.000000 resoto-plugin-posthog-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-24 18:32:24.328945 resoto-plugin-posthog-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-24 18:27:35.000000 resoto-plugin-posthog-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-24 18:27:35.000000 resoto-plugin-posthog-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:24.324946 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-24 18:27:35.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 18:27:35.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-24 18:27:35.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-24 18:27:35.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:24.328945 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-24 18:32:24.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-24 18:32:24.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:32:24.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 18:32:24.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:29:30.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 18:32:24.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:32:24.000000 resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:32:24.328945 resoto-plugin-posthog-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:24.328945 resoto-plugin-posthog-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 18:27:35.000000 resoto-plugin-posthog-3.6.4/test/test_config.py
```

### Comparing `resoto-plugin-posthog-3.6.3/PKG-INFO` & `resoto-plugin-posthog-3.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto Posthog Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/posthog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.6.3/README.md` & `resoto-plugin-posthog-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.6.3/pyproject.toml` & `resoto-plugin-posthog-3.6.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-posthog"
 description = "Resoto Posthog Collector Plugin"
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
     "requests",
 ]
 
 [project.entry-points."resoto.plugins"]
 posthog = "resoto_plugin_posthog:PosthogCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-posthog-3.6.3/resoto_plugin_posthog/__init__.py` & `resoto-plugin-posthog-3.6.4/resoto_plugin_posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.6.3/resoto_plugin_posthog/posthog.py` & `resoto-plugin-posthog-3.6.4/resoto_plugin_posthog/posthog.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.6.3/resoto_plugin_posthog/resources.py` & `resoto-plugin-posthog-3.6.4/resoto_plugin_posthog/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/PKG-INFO` & `resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto Posthog Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/posthog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.6.3/resoto_plugin_posthog.egg-info/SOURCES.txt` & `resoto-plugin-posthog-3.6.4/resoto_plugin_posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

