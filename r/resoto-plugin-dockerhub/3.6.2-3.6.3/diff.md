# Comparing `tmp/resoto-plugin-dockerhub-3.6.2.tar.gz` & `tmp/resoto-plugin-dockerhub-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-dockerhub-3.6.2.tar", last modified: Fri Jul 21 22:09:45 2023, max compression
+gzip compressed data, was "resoto-plugin-dockerhub-3.6.3.tar", last modified: Mon Jul 24 12:17:19 2023, max compression
```

## Comparing `resoto-plugin-dockerhub-3.6.2.tar` & `resoto-plugin-dockerhub-3.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:09:45.743232 resoto-plugin-dockerhub-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:06:09.000000 resoto-plugin-dockerhub-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-21 22:09:45.743232 resoto-plugin-dockerhub-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 22:06:09.000000 resoto-plugin-dockerhub-3.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-21 22:06:09.000000 resoto-plugin-dockerhub-3.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:09:45.743232 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-21 22:06:09.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-21 22:06:09.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-21 22:06:09.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:09:45.743232 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-21 22:09:45.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-21 22:09:45.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:09:45.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-21 22:09:45.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:07:35.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 22:09:45.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 22:09:45.000000 resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:09:45.743232 resoto-plugin-dockerhub-3.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:09:45.743232 resoto-plugin-dockerhub-3.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-21 22:06:09.000000 resoto-plugin-dockerhub-3.6.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:17:19.496887 resoto-plugin-dockerhub-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:13:44.000000 resoto-plugin-dockerhub-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-24 12:17:19.500887 resoto-plugin-dockerhub-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 12:13:44.000000 resoto-plugin-dockerhub-3.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-24 12:13:44.000000 resoto-plugin-dockerhub-3.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:17:19.496887 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 12:13:44.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 12:13:44.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-24 12:13:44.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:17:19.496887 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-24 12:17:19.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-24 12:17:19.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:17:19.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 12:17:19.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:15:10.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 12:17:19.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 12:17:19.000000 resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:17:19.500887 resoto-plugin-dockerhub-3.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:17:19.496887 resoto-plugin-dockerhub-3.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 12:13:44.000000 resoto-plugin-dockerhub-3.6.3/test/test_config.py
```

### Comparing `resoto-plugin-dockerhub-3.6.2/PKG-INFO` & `resoto-plugin-dockerhub-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.6.2
+Version: 3.6.3
 Summary: Resoto Docker Hub Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-dockerhub-3.6.2/README.md` & `resoto-plugin-dockerhub-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.6.2/pyproject.toml` & `resoto-plugin-dockerhub-3.6.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-dockerhub"
 description = "Resoto Docker Hub Collector Plugin"
-version = "3.6.2"
+version = "3.6.3"
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
-    "resotolib==3.6.2",
+    "resotolib==3.6.3",
     "requests",
 
 ]
 
 [project.entry-points."resoto.plugins"]
 dockerhub = "resoto_plugin_dockerhub:DockerHubCollectorPlugin"
```

### Comparing `resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub/__init__.py` & `resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub/resources.py` & `resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.6.2/resoto_plugin_dockerhub.egg-info/PKG-INFO` & `resoto-plugin-dockerhub-3.6.3/resoto_plugin_dockerhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.6.2
+Version: 3.6.3
 Summary: Resoto Docker Hub Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

