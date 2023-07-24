# Comparing `tmp/resoto-plugin-github-3.6.2.tar.gz` & `tmp/resoto-plugin-github-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-github-3.6.2.tar", last modified: Fri Jul 21 22:11:04 2023, max compression
+gzip compressed data, was "resoto-plugin-github-3.6.3.tar", last modified: Mon Jul 24 12:15:14 2023, max compression
```

## Comparing `resoto-plugin-github-3.6.2.tar` & `resoto-plugin-github-3.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:04.436567 resoto-plugin-github-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:06:17.000000 resoto-plugin-github-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-21 22:11:04.436567 resoto-plugin-github-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 22:06:17.000000 resoto-plugin-github-3.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-21 22:06:17.000000 resoto-plugin-github-3.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:04.436567 resoto-plugin-github-3.6.2/resoto_plugin_github/
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-21 22:06:17.000000 resoto-plugin-github-3.6.2/resoto_plugin_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-21 22:06:17.000000 resoto-plugin-github-3.6.2/resoto_plugin_github/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-07-21 22:06:17.000000 resoto-plugin-github-3.6.2/resoto_plugin_github/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:04.436567 resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-21 22:11:04.000000 resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-21 22:11:04.000000 resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:11:04.000000 resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 22:11:04.000000 resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:08:12.000000 resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 22:11:04.000000 resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 22:11:04.000000 resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:11:04.436567 resoto-plugin-github-3.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:04.436567 resoto-plugin-github-3.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-21 22:06:17.000000 resoto-plugin-github-3.6.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:15:14.381017 resoto-plugin-github-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:11:35.000000 resoto-plugin-github-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 12:15:14.381017 resoto-plugin-github-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 12:11:35.000000 resoto-plugin-github-3.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-24 12:11:35.000000 resoto-plugin-github-3.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:15:14.377017 resoto-plugin-github-3.6.3/resoto_plugin_github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-24 12:11:35.000000 resoto-plugin-github-3.6.3/resoto_plugin_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-24 12:11:35.000000 resoto-plugin-github-3.6.3/resoto_plugin_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-07-24 12:11:35.000000 resoto-plugin-github-3.6.3/resoto_plugin_github/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:15:14.377017 resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 12:15:14.000000 resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-24 12:15:14.000000 resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:15:14.000000 resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 12:15:14.000000 resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:13:03.000000 resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 12:15:14.000000 resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 12:15:14.000000 resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 12:15:14.381017 resoto-plugin-github-3.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:15:14.381017 resoto-plugin-github-3.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 12:11:35.000000 resoto-plugin-github-3.6.3/test/test_config.py
```

### Comparing `resoto-plugin-github-3.6.2/PKG-INFO` & `resoto-plugin-github-3.6.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.6.2
+Version: 3.6.3
 Summary: Resoto Github Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/github
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-github-3.6.2/pyproject.toml` & `resoto-plugin-github-3.6.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-github"
 description = "Resoto Github Collector Plugin"
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
     "PyGithub",
 ]
 
 [project.entry-points."resoto.plugins"]
 github = "resoto_plugin_github:GithubCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-github-3.6.2/resoto_plugin_github/__init__.py` & `resoto-plugin-github-3.6.3/resoto_plugin_github/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.6.2/resoto_plugin_github/config.py` & `resoto-plugin-github-3.6.3/resoto_plugin_github/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.6.2/resoto_plugin_github/resources.py` & `resoto-plugin-github-3.6.3/resoto_plugin_github/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.6.2/resoto_plugin_github.egg-info/PKG-INFO` & `resoto-plugin-github-3.6.3/resoto_plugin_github.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.6.2
+Version: 3.6.3
 Summary: Resoto Github Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/github
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

