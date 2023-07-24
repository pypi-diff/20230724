# Comparing `tmp/autogluon-0.8.3b20230723.tar.gz` & `tmp/autogluon-0.8.3b20230724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.3b20230723.tar", last modified: Sun Jul 23 09:04:11 2023, max compression
+gzip compressed data, was "autogluon-0.8.3b20230724.tar", last modified: Mon Jul 24 09:04:35 2023, max compression
```

## Comparing `autogluon-0.8.3b20230723.tar` & `autogluon-0.8.3b20230724.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:04:11.932470 autogluon-0.8.3b20230723/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-23 09:04:11.932470 autogluon-0.8.3b20230723/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 09:04:11.932470 autogluon-0.8.3b20230723/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-23 09:03:30.000000 autogluon-0.8.3b20230723/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:04:11.928470 autogluon-0.8.3b20230723/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:04:11.928470 autogluon-0.8.3b20230723/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:04:11.932470 autogluon-0.8.3b20230723/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 09:03:30.000000 autogluon-0.8.3b20230723/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 09:04:11.932470 autogluon-0.8.3b20230723/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-23 09:04:11.000000 autogluon-0.8.3b20230723/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-23 09:04:11.000000 autogluon-0.8.3b20230723/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 09:04:11.000000 autogluon-0.8.3b20230723/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-23 09:04:11.000000 autogluon-0.8.3b20230723/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-23 09:04:11.000000 autogluon-0.8.3b20230723/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-23 09:04:11.000000 autogluon-0.8.3b20230723/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 09:04:11.000000 autogluon-0.8.3b20230723/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:04:35.261164 autogluon-0.8.3b20230724/
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-24 09:04:35.261164 autogluon-0.8.3b20230724/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:04:35.261164 autogluon-0.8.3b20230724/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-24 09:03:56.000000 autogluon-0.8.3b20230724/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:04:35.261164 autogluon-0.8.3b20230724/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:04:35.261164 autogluon-0.8.3b20230724/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:04:35.261164 autogluon-0.8.3b20230724/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:03:56.000000 autogluon-0.8.3b20230724/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:04:35.261164 autogluon-0.8.3b20230724/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-24 09:04:35.000000 autogluon-0.8.3b20230724/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-24 09:04:35.000000 autogluon-0.8.3b20230724/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:04:35.000000 autogluon-0.8.3b20230724/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 09:04:35.000000 autogluon-0.8.3b20230724/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 09:04:35.000000 autogluon-0.8.3b20230724/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 09:04:35.000000 autogluon-0.8.3b20230724/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:04:35.000000 autogluon-0.8.3b20230724/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.3b20230723/PKG-INFO` & `autogluon-0.8.3b20230724/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.3b20230723
+Version: 0.8.3b20230724
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.8.3b20230723/setup.py` & `autogluon-0.8.3b20230724/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.3b20230723/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.3b20230724/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.3b20230723
+Version: 0.8.3b20230724
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

