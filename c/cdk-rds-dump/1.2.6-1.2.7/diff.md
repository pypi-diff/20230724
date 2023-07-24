# Comparing `tmp/cdk-rds-dump-1.2.6.tar.gz` & `tmp/cdk-rds-dump-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-1.2.6.tar", last modified: Thu Jul 20 09:26:03 2023, max compression
+gzip compressed data, was "cdk-rds-dump-1.2.7.tar", last modified: Mon Jul 24 14:03:41 2023, max compression
```

## Comparing `cdk-rds-dump-1.2.6.tar` & `cdk-rds-dump-1.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.609114 cdk-rds-dump-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-20 09:26:03.609114 cdk-rds-dump-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 09:26:03.609114 cdk-rds-dump-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.605114 cdk-rds-dump-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.605114 cdk-rds-dump-1.2.6/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.605114 cdk-rds-dump-1.2.6/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2575769 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:25:49.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:26:03.605114 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 09:26:03.000000 cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:41.314585 cdk-rds-dump-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-24 14:03:41.314585 cdk-rds-dump-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:03:41.314585 cdk-rds-dump-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:41.310585 cdk-rds-dump-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:41.310585 cdk-rds-dump-1.2.7/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:41.314585 cdk-rds-dump-1.2.7/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2569950 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:03:26.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:41.314585 cdk-rds-dump-1.2.7/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-24 14:03:41.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-24 14:03:41.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:03:41.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 14:03:41.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 14:03:41.000000 cdk-rds-dump-1.2.7/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-1.2.6/LICENSE` & `cdk-rds-dump-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.6/PKG-INFO` & `cdk-rds-dump-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.2.6
+Version: 1.2.7
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-rds-dump-1.2.6/README.md` & `cdk-rds-dump-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.6/setup.py` & `cdk-rds-dump-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "1.2.6",
+    "version": "1.2.7",
     "description": "CDK Construct Library by Typescript for RDS Dump",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-rds-dump.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_rds_dump",
         "cdk_rds_dump._jsii"
     ],
     "package_data": {
         "cdk_rds_dump._jsii": [
-            "cdk-rds-dump@1.2.6.jsii.tgz"
+            "cdk-rds-dump@1.2.7.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-rds-dump-1.2.6/src/cdk_rds_dump/__init__.py` & `cdk-rds-dump-1.2.7/src/cdk_rds_dump/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.6/src/cdk_rds_dump.egg-info/PKG-INFO` & `cdk-rds-dump-1.2.7/src/cdk_rds_dump.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.2.6
+Version: 1.2.7
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

