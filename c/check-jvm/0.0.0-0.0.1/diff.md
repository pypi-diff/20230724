# Comparing `tmp/check_jvm-0.0.0.tar.gz` & `tmp/check_jvm-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_jvm-0.0.0.tar", max compression
+gzip compressed data, was "check_jvm-0.0.1.tar", max compression
```

## Comparing `check_jvm-0.0.0.tar` & `check_jvm-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1098 2023-07-24 02:57:15.199928 check_jvm-0.0.0/LICENSE
--rw-r--r--   0        0        0      314 2023-07-24 02:57:55.200190 check_jvm-0.0.0/README.md
--rw-r--r--   0        0        0     1872 2023-07-24 09:00:37.236000 check_jvm-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      259 2023-07-24 03:14:01.063254 check_jvm-0.0.0/src/check_jvm/__init__.py
--rw-r--r--   0        0        0       49 2023-07-24 17:24:17.454058 check_jvm-0.0.0/src/check_jvm/__main__.py
--rw-r--r--   0        0        0     6070 2023-07-24 10:38:35.966231 check_jvm-0.0.0/src/check_jvm/app.py
--rw-r--r--   0        0        0     3479 2023-07-24 10:21:55.008914 check_jvm-0.0.0/src/check_jvm/java_version.py
--rw-r--r--   0        0        0      192 2023-07-24 03:11:59.386980 check_jvm-0.0.0/src/check_jvm/logger.py
--rw-r--r--   0        0        0        0 2023-07-24 03:12:30.381374 check_jvm-0.0.0/src/check_jvm/py.typed
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 check_jvm-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-07-24 02:57:15.199928 check_jvm-0.0.1/LICENSE
+-rw-r--r--   0        0        0      314 2023-07-24 02:57:55.200190 check_jvm-0.0.1/README.md
+-rw-r--r--   0        0        0     1872 2023-07-24 17:30:07.843324 check_jvm-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-07-24 03:14:01.063254 check_jvm-0.0.1/src/check_jvm/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-24 17:24:17.454058 check_jvm-0.0.1/src/check_jvm/__main__.py
+-rw-r--r--   0        0        0     6070 2023-07-24 10:38:35.966231 check_jvm-0.0.1/src/check_jvm/app.py
+-rw-r--r--   0        0        0     3479 2023-07-24 10:21:55.008914 check_jvm-0.0.1/src/check_jvm/java_version.py
+-rw-r--r--   0        0        0      192 2023-07-24 03:11:59.386980 check_jvm-0.0.1/src/check_jvm/logger.py
+-rw-r--r--   0        0        0        0 2023-07-24 03:12:30.381374 check_jvm-0.0.1/src/check_jvm/py.typed
+-rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 check_jvm-0.0.1/PKG-INFO
```

### Comparing `check_jvm-0.0.0/LICENSE` & `check_jvm-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `check_jvm-0.0.0/pyproject.toml` & `check_jvm-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "check-jvm"
-version = "0.0.0"
+version = "0.0.1"
 description = ""
 authors = ["Dániel Hagyárossy <daniel@hagyarossy.hu>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://"
 # documentation = "https://"
 keywords = ["oracle jvm", "jvm checker"]
```

### Comparing `check_jvm-0.0.0/src/check_jvm/app.py` & `check_jvm-0.0.1/src/check_jvm/app.py`

 * *Files identical despite different names*

### Comparing `check_jvm-0.0.0/src/check_jvm/java_version.py` & `check_jvm-0.0.1/src/check_jvm/java_version.py`

 * *Files identical despite different names*

### Comparing `check_jvm-0.0.0/PKG-INFO` & `check_jvm-0.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-jvm
-Version: 0.0.0
+Version: 0.0.1
 Summary: 
 License: MIT
 Keywords: oracle jvm,jvm checker
 Author: Dániel Hagyárossy
 Author-email: daniel@hagyarossy.hu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

