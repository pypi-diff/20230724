# Comparing `tmp/resoto-plugin-cleanup-aws-alarms-3.6.3.tar.gz` & `tmp/resoto-plugin-cleanup-aws-alarms-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-alarms-3.6.3.tar", last modified: Mon Jul 24 12:10:36 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-alarms-3.6.4.tar", last modified: Mon Jul 24 18:30:32 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-alarms-3.6.3.tar` & `resoto-plugin-cleanup-aws-alarms-3.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:36.343462 resoto-plugin-cleanup-aws-alarms-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:06:38.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 12:10:36.343462 resoto-plugin-cleanup-aws-alarms-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-24 12:06:38.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-24 12:06:38.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:36.343462 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-24 12:06:38.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 12:06:38.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:36.343462 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 12:10:36.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 12:10:36.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:10:36.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 12:10:36.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:08:16.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 12:10:36.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 12:10:36.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:10:36.343462 resoto-plugin-cleanup-aws-alarms-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:36.343462 resoto-plugin-cleanup-aws-alarms-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-24 12:06:38.000000 resoto-plugin-cleanup-aws-alarms-3.6.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:32.567328 resoto-plugin-cleanup-aws-alarms-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:25:53.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 18:30:32.567328 resoto-plugin-cleanup-aws-alarms-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-24 18:25:53.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-24 18:25:53.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:32.567328 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-24 18:25:53.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 18:25:53.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:32.567328 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 18:30:32.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 18:30:32.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:30:32.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 18:30:32.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:27:48.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:30:32.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 18:30:32.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 18:30:32.567328 resoto-plugin-cleanup-aws-alarms-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:32.567328 resoto-plugin-cleanup-aws-alarms-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-24 18:25:53.000000 resoto-plugin-cleanup-aws-alarms-3.6.4/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.6.3/PKG-INFO` & `resoto-plugin-cleanup-aws-alarms-3.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-alarms
-Version: 3.6.3
+Version: 3.6.4
 Summary: AWS Cloudwatch Alarms Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.6.3/README.md` & `resoto-plugin-cleanup-aws-alarms-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.6.3/pyproject.toml` & `resoto-plugin-cleanup-aws-alarms-3.6.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-cleanup-aws-alarms"
-version = "3.6.3"
+version = "3.6.4"
 authors = [{name="Some Engineering Inc."}]
 description = "AWS Cloudwatch Alarms Cleaner Plugin"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -22,15 +22,15 @@
     "Environment :: Console",
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
-dependencies = [ "resotolib==3.6.3" ]
+dependencies = [ "resotolib==3.6.4" ]
 
 [project.entry-points."resoto.plugins"]
 cleanup_aws_alarms = "resoto_plugin_cleanup_aws_alarms:CleanupAWSAlarmsPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
 Source = "https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms"
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms/__init__.py` & `resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms/config.py` & `resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-alarms
-Version: 3.6.3
+Version: 3.6.4
 Summary: AWS Cloudwatch Alarms Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_alarms
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-alarms-3.6.3/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-alarms-3.6.4/resoto_plugin_cleanup_aws_alarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

