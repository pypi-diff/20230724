# Comparing `tmp/resoto-plugin-cleanup-aws-vpcs-3.6.2.tar.gz` & `tmp/resoto-plugin-cleanup-aws-vpcs-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.6.2.tar", last modified: Fri Jul 21 22:10:19 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.6.3.tar", last modified: Mon Jul 24 12:13:06 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.2.tar` & `resoto-plugin-cleanup-aws-vpcs-3.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:19.516438 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:07:50.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:06.483780 resoto-plugin-cleanup-aws-vpcs-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:09:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-24 12:13:06.483780 resoto-plugin-cleanup-aws-vpcs-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 12:09:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-24 12:09:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:06.479780 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-24 12:09:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-24 12:09:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:06.483780 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-24 12:13:06.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-24 12:13:06.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:13:06.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-24 12:13:06.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:10:40.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 12:13:06.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 12:13:06.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:13:06.483780 resoto-plugin-cleanup-aws-vpcs-3.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:13:06.483780 resoto-plugin-cleanup-aws-vpcs-3.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-24 12:09:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.3/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.2/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.6.2
+Version: 3.6.3
 Summary: AWS VPC Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.2/README.md` & `resoto-plugin-cleanup-aws-vpcs-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.2/pyproject.toml` & `resoto-plugin-cleanup-aws-vpcs-3.6.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-aws-vpcs"
 description = "AWS VPC Cleaner Plugin"
-version = "3.6.2"
+version = "3.6.3"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,16 +23,16 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.2",
-    "resoto-plugin-aws==3.6.2"
+    "resotolib==3.6.3",
+    "resoto-plugin-aws==3.6.3"
 ]
 
 [project.entry-points."resoto.plugins"]
 cleanup_aws_vpcs = "resoto_plugin_cleanup_aws_vpcs:CleanupAWSVPCsPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/__init__.py` & `resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/config.py` & `resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.6.2
+Version: 3.6.3
 Summary: AWS VPC Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-vpcs-3.6.3/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

