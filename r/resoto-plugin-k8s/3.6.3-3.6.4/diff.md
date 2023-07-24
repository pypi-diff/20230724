# Comparing `tmp/resoto-plugin-k8s-3.6.3.tar.gz` & `tmp/resoto-plugin-k8s-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-k8s-3.6.3.tar", last modified: Mon Jul 24 12:17:25 2023, max compression
+gzip compressed data, was "resoto-plugin-k8s-3.6.4.tar", last modified: Mon Jul 24 18:34:11 2023, max compression
```

## Comparing `resoto-plugin-k8s-3.6.3.tar` & `resoto-plugin-k8s-3.6.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:17:25.833932 resoto-plugin-k8s-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 12:17:25.833932 resoto-plugin-k8s-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:17:25.829932 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:17:25.833932 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/deferred_edges/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/deferred_edges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/deferred_edges/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/deferred_edges/digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/deferred_edges/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-07-24 12:12:09.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:17:25.833932 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 12:17:25.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-24 12:17:25.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:17:25.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 12:17:25.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:13:44.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 12:17:25.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:17:25.000000 resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 12:17:25.833932 resoto-plugin-k8s-3.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:11.264295 resoto-plugin-k8s-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 18:34:11.264295 resoto-plugin-k8s-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:11.264295 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:11.264295 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/deferred_edges/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/deferred_edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/deferred_edges/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/deferred_edges/digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/deferred_edges/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-07-24 18:29:13.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:34:11.264295 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 18:34:11.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-24 18:34:11.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:34:11.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 18:34:11.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:30:39.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 18:34:11.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:34:11.000000 resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 18:34:11.264295 resoto-plugin-k8s-3.6.4/setup.cfg
```

### Comparing `resoto-plugin-k8s-3.6.3/PKG-INFO` & `resoto-plugin-k8s-3.6.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.6.3/pyproject.toml` & `resoto-plugin-k8s-3.6.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-k8s"
 description = "Resoto Kubernetes Collector Plugin"
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
     "kubernetes",
 ]
 
 [project.entry-points."resoto.plugins"]
 k8s_collector = "resoto_plugin_k8s:KubernetesCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/__init__.py` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/base.py` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/collector.py` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/deferred_edges/__init__.py` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/deferred_edges/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/deferred_edges/aws.py` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/deferred_edges/aws.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/deferred_edges/digitalocean.py` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/deferred_edges/digitalocean.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s/resources.py` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/PKG-INFO` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.6.3/resoto_plugin_k8s.egg-info/SOURCES.txt` & `resoto-plugin-k8s-3.6.4/resoto_plugin_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

