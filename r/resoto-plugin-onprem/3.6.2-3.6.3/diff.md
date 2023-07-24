# Comparing `tmp/resoto-plugin-onprem-3.6.2.tar.gz` & `tmp/resoto-plugin-onprem-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onprem-3.6.2.tar", last modified: Fri Jul 21 22:10:40 2023, max compression
+gzip compressed data, was "resoto-plugin-onprem-3.6.3.tar", last modified: Mon Jul 24 12:18:25 2023, max compression
```

## Comparing `resoto-plugin-onprem-3.6.2.tar` & `resoto-plugin-onprem-3.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:40.236432 resoto-plugin-onprem-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:06:14.000000 resoto-plugin-onprem-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-21 22:10:40.236432 resoto-plugin-onprem-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 22:06:14.000000 resoto-plugin-onprem-3.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-21 22:06:14.000000 resoto-plugin-onprem-3.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:40.236432 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-21 22:06:14.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-21 22:06:14.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-21 22:06:14.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-21 22:06:14.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:40.236432 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-21 22:10:40.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-21 22:10:40.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:10:40.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 22:10:40.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:08:01.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 22:10:40.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 22:10:40.000000 resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:10:40.236432 resoto-plugin-onprem-3.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:40.236432 resoto-plugin-onprem-3.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-21 22:06:14.000000 resoto-plugin-onprem-3.6.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:18:25.128377 resoto-plugin-onprem-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:14:52.000000 resoto-plugin-onprem-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-24 12:18:25.128377 resoto-plugin-onprem-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 12:14:52.000000 resoto-plugin-onprem-3.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-24 12:14:52.000000 resoto-plugin-onprem-3.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:18:25.128377 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-24 12:14:52.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-24 12:14:52.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 12:14:52.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-24 12:14:52.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:18:25.128377 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-24 12:18:25.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 12:18:25.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:18:25.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 12:18:25.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:16:15.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 12:18:25.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 12:18:25.000000 resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:18:25.128377 resoto-plugin-onprem-3.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:18:25.128377 resoto-plugin-onprem-3.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-24 12:14:52.000000 resoto-plugin-onprem-3.6.3/test/test_config.py
```

### Comparing `resoto-plugin-onprem-3.6.2/PKG-INFO` & `resoto-plugin-onprem-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onprem
-Version: 3.6.2
+Version: 3.6.3
 Summary: Resoto On-Premises Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onprem-3.6.2/pyproject.toml` & `resoto-plugin-onprem-3.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-onprem"
 description = "Resoto On-Premises Collector Plugin"
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
     "paramiko",
 ]
 
 [project.entry-points."resoto.plugins"]
 onprem = "resoto_plugin_onprem:OnpremCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/__init__.py` & `resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/config.py` & `resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/resources.py` & `resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.6.2/resoto_plugin_onprem/ssh.py` & `resoto-plugin-onprem-3.6.3/resoto_plugin_onprem/ssh.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.6.2/resoto_plugin_onprem.egg-info/PKG-INFO` & `resoto-plugin-onprem-3.6.3/resoto_plugin_onprem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onprem
-Version: 3.6.2
+Version: 3.6.3
 Summary: Resoto On-Premises Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onprem-3.6.2/test/test_config.py` & `resoto-plugin-onprem-3.6.3/test/test_config.py`

 * *Files identical despite different names*

