# Comparing `tmp/resoto-plugin-gcp-3.6.3.tar.gz` & `tmp/resoto-plugin-gcp-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.6.3.tar", last modified: Mon Jul 24 12:13:13 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.6.4.tar", last modified: Mon Jul 24 18:39:44 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.6.3.tar` & `resoto-plugin-gcp-3.6.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:13.854852 resoto-plugin-gcp-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-24 12:13:13.854852 resoto-plugin-gcp-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:13.842852 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/gcp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:13.850852 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   284565 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:13.846852 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-24 12:13:13.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-24 12:13:13.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:13:13.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 12:13:13.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:08:25.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-24 12:13:13.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 12:13:13.000000 resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-24 12:13:13.854852 resoto-plugin-gcp-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:13.854852 resoto-plugin-gcp-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/test_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-24 12:06:56.000000 resoto-plugin-gcp-3.6.3/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:39:44.771720 resoto-plugin-gcp-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-24 18:39:44.771720 resoto-plugin-gcp-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:39:44.767720 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/gcp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:39:44.771720 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   284565 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:39:44.771720 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-24 18:39:44.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-24 18:39:44.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:39:44.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 18:39:44.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:34:46.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-24 18:39:44.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:39:44.000000 resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-24 18:39:44.771720 resoto-plugin-gcp-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:39:44.771720 resoto-plugin-gcp-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-24 18:33:19.000000 resoto-plugin-gcp-3.6.4/test/test_storage.py
```

### Comparing `resoto-plugin-gcp-3.6.3/PKG-INFO` & `resoto-plugin-gcp-3.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.6.3/pyproject.toml` & `resoto-plugin-gcp-3.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-gcp"
 description = "Resoto GCP Collector Plugin"
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
     "google-api-python-client",
     "oauth2client",
     "retrying",
     "tenacity",
 ]
 
 [project.entry-points."resoto.plugins"]
```

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/collector.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/resources/storage.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/resources/storage.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.6.3
+Version: 3.6.4
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.6.3/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.6.4/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/conftest.py` & `resoto-plugin-gcp-3.6.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/random_client.py` & `resoto-plugin-gcp-3.6.4/test/random_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/test_base.py` & `resoto-plugin-gcp-3.6.4/test/test_base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/test_billing.py` & `resoto-plugin-gcp-3.6.4/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/test_collector.py` & `resoto-plugin-gcp-3.6.4/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/test_compute.py` & `resoto-plugin-gcp-3.6.4/test/test_compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/test_config.py` & `resoto-plugin-gcp-3.6.4/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/test_container.py` & `resoto-plugin-gcp-3.6.4/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.3/test/test_sqladmin.py` & `resoto-plugin-gcp-3.6.4/test/test_sqladmin.py`

 * *Files identical despite different names*

