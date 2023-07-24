# Comparing `tmp/lets_debug_helper-1.5.8.tar.gz` & `tmp/lets_debug_helper-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lets_debug_helper-1.5.8.tar", max compression
+gzip compressed data, was "lets_debug_helper-1.5.9.tar", max compression
```

## Comparing `lets_debug_helper-1.5.8.tar` & `lets_debug_helper-1.5.9.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1070 2020-12-30 17:36:35.000000 lets_debug_helper-1.5.8/LICENSE
--rw-r--r--   0        0        0      602 2022-11-09 23:11:52.000026 lets_debug_helper-1.5.8/README.md
--rw-r--r--   0        0        0        0 2022-05-21 18:48:28.935073 lets_debug_helper-1.5.8/letsdebughelper/__init__.py
--rw-r--r--   0        0        0      833 2022-11-09 21:26:35.530699 lets_debug_helper-1.5.8/letsdebughelper/helpers.py
--rwxr-xr-x   0        0        0     3691 2022-11-09 23:01:49.551755 lets_debug_helper-1.5.8/letsdebughelper/letsdebug.py
--rw-r--r--   0        0        0        0 2022-05-21 18:48:28.936018 lets_debug_helper-1.5.8/letsdebughelper/tests/__init__.py
--rw-r--r--   0        0        0     1161 2022-11-09 21:30:15.848526 lets_debug_helper-1.5.8/letsdebughelper/tests/test_helpers.py
--rw-r--r--   0        0        0     9710 2022-11-09 23:08:21.750119 lets_debug_helper-1.5.8/letsdebughelper/tests/test_letsdebug.py
--rw-r--r--   0        0        0      900 2023-06-07 15:21:33.669409 lets_debug_helper-1.5.8/pyproject.toml
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 lets_debug_helper-1.5.8/setup.py
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 lets_debug_helper-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-12-30 17:36:35.000000 lets_debug_helper-1.5.9/LICENSE
+-rw-r--r--   0        0        0      602 2022-11-09 23:11:52.000026 lets_debug_helper-1.5.9/README.md
+-rw-r--r--   0        0        0        0 2022-05-21 18:48:28.935073 lets_debug_helper-1.5.9/letsdebughelper/__init__.py
+-rw-r--r--   0        0        0      833 2022-11-09 21:26:35.530699 lets_debug_helper-1.5.9/letsdebughelper/helpers.py
+-rwxr-xr-x   0        0        0     3691 2022-11-09 23:01:49.551755 lets_debug_helper-1.5.9/letsdebughelper/letsdebug.py
+-rw-r--r--   0        0        0        0 2022-05-21 18:48:28.936018 lets_debug_helper-1.5.9/letsdebughelper/tests/__init__.py
+-rw-r--r--   0        0        0     1161 2022-11-09 21:30:15.848526 lets_debug_helper-1.5.9/letsdebughelper/tests/test_helpers.py
+-rw-r--r--   0        0        0     9710 2022-11-09 23:08:21.750119 lets_debug_helper-1.5.9/letsdebughelper/tests/test_letsdebug.py
+-rw-r--r--   0        0        0      900 2023-07-24 15:59:09.507599 lets_debug_helper-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 lets_debug_helper-1.5.9/PKG-INFO
```

### Comparing `lets_debug_helper-1.5.8/LICENSE` & `lets_debug_helper-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.8/README.md` & `lets_debug_helper-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.8/letsdebughelper/helpers.py` & `lets_debug_helper-1.5.9/letsdebughelper/helpers.py`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.8/letsdebughelper/letsdebug.py` & `lets_debug_helper-1.5.9/letsdebughelper/letsdebug.py`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.8/letsdebughelper/tests/test_helpers.py` & `lets_debug_helper-1.5.9/letsdebughelper/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.8/letsdebughelper/tests/test_letsdebug.py` & `lets_debug_helper-1.5.9/letsdebughelper/tests/test_letsdebug.py`

 * *Files identical despite different names*

### Comparing `lets_debug_helper-1.5.8/pyproject.toml` & `lets_debug_helper-1.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lets-debug-helper"
-version = "1.5.8"
+version = "1.5.9"
 description = "This is a cli tool that interacts with the Let's Debug API"
 authors = ["Jeffrey Crane <jediknight11206@gmail.com>"]
 license = "License :: OSI Approved :: MIT License"
 include = ["README.md"]
 packages = [
     { include = "letsdebughelper" },
 ]
```

### Comparing `lets_debug_helper-1.5.8/PKG-INFO` & `lets_debug_helper-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lets-debug-helper
-Version: 1.5.8
+Version: 1.5.9
 Summary: This is a cli tool that interacts with the Let's Debug API
 License: License :: OSI Approved :: MIT License
 Author: Jeffrey Crane
 Author-email: jediknight11206@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

