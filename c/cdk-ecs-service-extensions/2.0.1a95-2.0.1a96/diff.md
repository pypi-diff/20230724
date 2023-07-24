# Comparing `tmp/cdk-ecs-service-extensions-2.0.1a95.tar.gz` & `tmp/cdk-ecs-service-extensions-2.0.1a96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-ecs-service-extensions-2.0.1a95.tar", last modified: Sun Jul 23 00:31:17 2023, max compression
+gzip compressed data, was "cdk-ecs-service-extensions-2.0.1a96.tar", last modified: Mon Jul 24 00:30:01 2023, max compression
```

## Comparing `cdk-ecs-service-extensions-2.0.1a95.tar` & `cdk-ecs-service-extensions-2.0.1a96.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 00:31:17.081502 cdk-ecs-service-extensions-2.0.1a95/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-23 00:31:17.081502 cdk-ecs-service-extensions-2.0.1a95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24273 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 00:31:17.081502 cdk-ecs-service-extensions-2.0.1a95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 00:31:17.077502 cdk-ecs-service-extensions-2.0.1a95/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 00:31:17.077502 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)   295093 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 00:31:17.077502 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   172611 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.95.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 00:30:58.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 00:31:17.077502 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-23 00:31:17.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-23 00:31:17.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 00:31:17.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-23 00:31:17.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-23 00:31:17.000000 cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:30:01.468455 cdk-ecs-service-extensions-2.0.1a96/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-24 00:30:01.468455 cdk-ecs-service-extensions-2.0.1a96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24273 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:30:01.468455 cdk-ecs-service-extensions-2.0.1a96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:30:01.468455 cdk-ecs-service-extensions-2.0.1a96/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:30:01.468455 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)   295093 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:30:01.468455 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172617 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.96.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:29:47.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:30:01.468455 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-24 00:30:01.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-24 00:30:01.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:30:01.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 00:30:01.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 00:30:01.000000 cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions.egg-info/top_level.txt
```

### Comparing `cdk-ecs-service-extensions-2.0.1a95/LICENSE` & `cdk-ecs-service-extensions-2.0.1a96/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-ecs-service-extensions-2.0.1a95/PKG-INFO` & `cdk-ecs-service-extensions-2.0.1a96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-ecs-service-extensions
-Version: 2.0.1a95
+Version: 2.0.1a96
 Summary: The CDK Construct Library that helps you build ECS services using simple extensions
 Home-page: https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-ecs-service-extensions-2.0.1a95/README.md` & `cdk-ecs-service-extensions-2.0.1a96/README.md`

 * *Files identical despite different names*

### Comparing `cdk-ecs-service-extensions-2.0.1a95/setup.py` & `cdk-ecs-service-extensions-2.0.1a96/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-ecs-service-extensions",
-    "version": "2.0.1.a95",
+    "version": "2.0.1.a96",
     "description": "The CDK Construct Library that helps you build ECS services using simple extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-ecs-service-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_ecs_service_extensions",
         "cdk_ecs_service_extensions._jsii"
     ],
     "package_data": {
         "cdk_ecs_service_extensions._jsii": [
-            "ecs-service-extensions@2.0.1-alpha.95.jsii.tgz"
+            "ecs-service-extensions@2.0.1-alpha.96.jsii.tgz"
         ],
         "cdk_ecs_service_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions/__init__.py` & `cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions.egg-info/PKG-INFO` & `cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-ecs-service-extensions
-Version: 2.0.1a95
+Version: 2.0.1a96
 Summary: The CDK Construct Library that helps you build ECS services using simple extensions
 Home-page: https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-ecs-service-extensions-2.0.1a95/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt` & `cdk-ecs-service-extensions-2.0.1a96/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_ecs_service_extensions/py.typed
 src/cdk_ecs_service_extensions.egg-info/PKG-INFO
 src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
 src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
 src/cdk_ecs_service_extensions.egg-info/requires.txt
 src/cdk_ecs_service_extensions.egg-info/top_level.txt
 src/cdk_ecs_service_extensions/_jsii/__init__.py
-src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.95.jsii.tgz
+src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.96.jsii.tgz
```

