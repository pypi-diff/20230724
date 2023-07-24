# Comparing `tmp/chalk-harness-1.0.9.tar.gz` & `tmp/chalk-harness-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalk-harness-1.0.9.tar", last modified: Mon Jul 24 18:54:36 2023, max compression
+gzip compressed data, was "chalk-harness-1.1.0.tar", last modified: Mon Jul 24 19:02:00 2023, max compression
```

## Comparing `chalk-harness-1.0.9.tar` & `chalk-harness-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:54:36.202770 chalk-harness-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 18:54:36.202770 chalk-harness-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:54:36.202770 chalk-harness-1.0.9/chalk_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 18:54:36.000000 chalk-harness-1.0.9/chalk_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 18:54:36.000000 chalk-harness-1.0.9/chalk_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:54:36.000000 chalk-harness-1.0.9/chalk_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 18:54:36.000000 chalk-harness-1.0.9/chalk_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 18:54:36.000000 chalk-harness-1.0.9/chalk_harness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:54:36.202770 chalk-harness-1.0.9/chalkharness/
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/chalkharness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/chalkharness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:54:36.202770 chalk-harness-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:54:36.202770 chalk-harness-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/tests/SanityTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:54:24.000000 chalk-harness-1.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:02:00.135024 chalk-harness-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 19:02:00.135024 chalk-harness-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:02:00.135024 chalk-harness-1.1.0/chalk_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 19:02:00.000000 chalk-harness-1.1.0/chalk_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 19:02:00.000000 chalk-harness-1.1.0/chalk_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:02:00.000000 chalk-harness-1.1.0/chalk_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 19:02:00.000000 chalk-harness-1.1.0/chalk_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 19:02:00.000000 chalk-harness-1.1.0/chalk_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:02:00.135024 chalk-harness-1.1.0/chalkharness/
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/chalkharness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/chalkharness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:02:00.135024 chalk-harness-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:02:00.135024 chalk-harness-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/tests/SanityTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:01:48.000000 chalk-harness-1.1.0/tests/__init__.py
```

### Comparing `chalk-harness-1.0.9/PKG-INFO` & `chalk-harness-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.0.9/README.md` & `chalk-harness-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.0.9/chalk_harness.egg-info/PKG-INFO` & `chalk-harness-1.1.0/chalk_harness.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.0.9/chalkharness/__init__.py` & `chalk-harness-1.1.0/chalkharness/__init__.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.0.9/setup.py` & `chalk-harness-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.0.9/tests/SanityTestCase.py` & `chalk-harness-1.1.0/tests/SanityTestCase.py`

 * *Files identical despite different names*

