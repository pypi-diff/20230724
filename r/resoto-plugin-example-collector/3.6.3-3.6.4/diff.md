# Comparing `tmp/resoto-plugin-example-collector-3.6.3.tar.gz` & `tmp/resoto-plugin-example-collector-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-example-collector-3.6.3.tar", last modified: Mon Jul 24 12:19:21 2023, max compression
+gzip compressed data, was "resoto-plugin-example-collector-3.6.4.tar", last modified: Mon Jul 24 18:33:00 2023, max compression
```

## Comparing `resoto-plugin-example-collector-3.6.3.tar` & `resoto-plugin-example-collector-3.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:19:21.575225 resoto-plugin-example-collector-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:15:30.000000 resoto-plugin-example-collector-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-24 12:19:21.575225 resoto-plugin-example-collector-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 12:15:30.000000 resoto-plugin-example-collector-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-24 12:15:30.000000 resoto-plugin-example-collector-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:19:21.571225 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector/
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-24 12:15:30.000000 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:19:21.575225 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-24 12:19:21.000000 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-24 12:19:21.000000 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:19:21.000000 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 12:19:21.000000 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:17:01.000000 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 12:19:21.000000 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 12:19:21.000000 resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:19:21.575225 resoto-plugin-example-collector-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:19:21.575225 resoto-plugin-example-collector-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-24 12:15:30.000000 resoto-plugin-example-collector-3.6.3/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 12:15:30.000000 resoto-plugin-example-collector-3.6.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:00.777639 resoto-plugin-example-collector-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:29:24.000000 resoto-plugin-example-collector-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-24 18:33:00.777639 resoto-plugin-example-collector-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:29:24.000000 resoto-plugin-example-collector-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-24 18:29:24.000000 resoto-plugin-example-collector-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:00.773639 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-24 18:29:24.000000 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:00.777639 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-24 18:33:00.000000 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-24 18:33:00.000000 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:33:00.000000 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 18:33:00.000000 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:30:48.000000 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:33:00.000000 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 18:33:00.000000 resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:33:00.777639 resoto-plugin-example-collector-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:00.777639 resoto-plugin-example-collector-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-24 18:29:24.000000 resoto-plugin-example-collector-3.6.4/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 18:29:24.000000 resoto-plugin-example-collector-3.6.4/test/test_config.py
```

### Comparing `resoto-plugin-example-collector-3.6.3/PKG-INFO` & `resoto-plugin-example-collector-3.6.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-example-collector
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto Example Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/example_collector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-example-collector-3.6.3/pyproject.toml` & `resoto-plugin-example-collector-3.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-example-collector"
 description = "Resoto Example Collector Plugin"
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
 ]
 
 [project.entry-points."resoto.plugins"]
 example_collector = "resoto_plugin_example_collector:ExampleCollectorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector/__init__.py` & `resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/PKG-INFO` & `resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-example-collector
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto Example Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/example_collector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-example-collector-3.6.3/resoto_plugin_example_collector.egg-info/SOURCES.txt` & `resoto-plugin-example-collector-3.6.4/resoto_plugin_example_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

