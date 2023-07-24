# Comparing `tmp/resoto-plugin-cleanup-volumes-3.6.3.tar.gz` & `tmp/resoto-plugin-cleanup-volumes-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-volumes-3.6.3.tar", last modified: Mon Jul 24 12:10:33 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-volumes-3.6.4.tar", last modified: Mon Jul 24 18:30:01 2023, max compression
```

## Comparing `resoto-plugin-cleanup-volumes-3.6.3.tar` & `resoto-plugin-cleanup-volumes-3.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:33.187298 resoto-plugin-cleanup-volumes-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:06:05.000000 resoto-plugin-cleanup-volumes-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-24 12:10:33.187298 resoto-plugin-cleanup-volumes-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 12:06:05.000000 resoto-plugin-cleanup-volumes-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 12:06:05.000000 resoto-plugin-cleanup-volumes-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:33.183298 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-24 12:06:05.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 12:06:05.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:33.187298 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-24 12:10:33.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 12:10:33.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:10:33.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 12:10:33.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:07:54.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 12:10:33.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 12:10:33.000000 resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:10:33.187298 resoto-plugin-cleanup-volumes-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:33.187298 resoto-plugin-cleanup-volumes-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 12:06:05.000000 resoto-plugin-cleanup-volumes-3.6.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:01.788707 resoto-plugin-cleanup-volumes-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:26:02.000000 resoto-plugin-cleanup-volumes-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-24 18:30:01.788707 resoto-plugin-cleanup-volumes-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 18:26:02.000000 resoto-plugin-cleanup-volumes-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 18:26:02.000000 resoto-plugin-cleanup-volumes-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:01.788707 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-24 18:26:02.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 18:26:02.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:01.788707 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-24 18:30:01.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 18:30:01.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:30:01.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 18:30:01.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:27:35.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:30:01.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 18:30:01.000000 resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:30:01.788707 resoto-plugin-cleanup-volumes-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:01.788707 resoto-plugin-cleanup-volumes-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 18:26:02.000000 resoto-plugin-cleanup-volumes-3.6.4/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-volumes-3.6.3/PKG-INFO` & `resoto-plugin-cleanup-volumes-3.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-volumes
-Version: 3.6.3
+Version: 3.6.4
 Summary: Volume Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-volumes-3.6.3/README.md` & `resoto-plugin-cleanup-volumes-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.6.3/pyproject.toml` & `resoto-plugin-cleanup-volumes-3.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-volumes"
 description = "Volume Cleaner Plugin"
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
 cleanup_volumes = "resoto_plugin_cleanup_volumes:CleanupVolumesPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes/__init__.py` & `resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes/config.py` & `resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO` & `resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-volumes
-Version: 3.6.3
+Version: 3.6.4
 Summary: Volume Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_volumes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-volumes-3.6.3/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-volumes-3.6.4/resoto_plugin_cleanup_volumes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

