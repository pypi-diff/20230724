# Comparing `tmp/crepex_pyutil-0.5.0.tar.gz` & `tmp/crepex_pyutil-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepex_pyutil-0.5.0.tar", max compression
+gzip compressed data, was "crepex_pyutil-0.6.0.tar", max compression
```

## Comparing `crepex_pyutil-0.5.0.tar` & `crepex_pyutil-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      791 2023-04-12 09:41:55.227358 crepex_pyutil-0.5.0/README.md
--rw-r--r--   0        0        0      413 2023-07-03 16:26:54.652483 crepex_pyutil-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 06:42:39.752853 crepex_pyutil-0.5.0/src/crepex_pyutil/__init__.py
--rw-r--r--   0        0        0      212 2023-07-03 16:26:40.532032 crepex_pyutil-0.5.0/src/crepex_pyutil/collections.py
--rwxr-xr-x   0        0        0     3246 2023-07-01 09:13:24.096916 crepex_pyutil-0.5.0/src/crepex_pyutil/dates.py
--rw-r--r--   0        0        0      712 2023-07-01 09:08:24.771723 crepex_pyutil-0.5.0/src/crepex_pyutil/exceptions.py
--rw-r--r--   0        0        0       81 2023-05-15 08:44:18.527777 crepex_pyutil-0.5.0/src/crepex_pyutil/requests/__init__.py
--rw-r--r--   0        0        0     2107 2023-04-12 06:02:06.720570 crepex_pyutil-0.5.0/src/crepex_pyutil/requests/helper.py
--rw-r--r--   0        0        0     2197 2023-05-15 08:45:17.992026 crepex_pyutil-0.5.0/src/crepex_pyutil/requests/slack.py
--rwxr-xr-x   0        0        0     1726 2023-04-27 01:58:48.842662 crepex_pyutil-0.5.0/src/crepex_pyutil/string.py
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 crepex_pyutil-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      791 2023-04-12 09:41:55.227358 crepex_pyutil-0.6.0/README.md
+-rw-r--r--   0        0        0      413 2023-07-24 13:43:27.950147 crepex_pyutil-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 06:42:39.752853 crepex_pyutil-0.6.0/src/crepex_pyutil/__init__.py
+-rw-r--r--   0        0        0      937 2023-07-24 13:43:18.766419 crepex_pyutil-0.6.0/src/crepex_pyutil/collections.py
+-rwxr-xr-x   0        0        0     3246 2023-07-01 09:13:24.096916 crepex_pyutil-0.6.0/src/crepex_pyutil/dates.py
+-rw-r--r--   0        0        0      712 2023-07-01 09:08:24.771723 crepex_pyutil-0.6.0/src/crepex_pyutil/exceptions.py
+-rw-r--r--   0        0        0       81 2023-05-15 08:44:18.527777 crepex_pyutil-0.6.0/src/crepex_pyutil/requests/__init__.py
+-rw-r--r--   0        0        0     2107 2023-04-12 06:02:06.720570 crepex_pyutil-0.6.0/src/crepex_pyutil/requests/helper.py
+-rw-r--r--   0        0        0     2197 2023-05-15 08:45:17.992026 crepex_pyutil-0.6.0/src/crepex_pyutil/requests/slack.py
+-rwxr-xr-x   0        0        0     1726 2023-04-27 01:58:48.842662 crepex_pyutil-0.6.0/src/crepex_pyutil/string.py
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 crepex_pyutil-0.6.0/PKG-INFO
```

### Comparing `crepex_pyutil-0.5.0/README.md` & `crepex_pyutil-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.5.0/src/crepex_pyutil/dates.py` & `crepex_pyutil-0.6.0/src/crepex_pyutil/dates.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.5.0/src/crepex_pyutil/exceptions.py` & `crepex_pyutil-0.6.0/src/crepex_pyutil/exceptions.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.5.0/src/crepex_pyutil/requests/helper.py` & `crepex_pyutil-0.6.0/src/crepex_pyutil/requests/helper.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.5.0/src/crepex_pyutil/requests/slack.py` & `crepex_pyutil-0.6.0/src/crepex_pyutil/requests/slack.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.5.0/src/crepex_pyutil/string.py` & `crepex_pyutil-0.6.0/src/crepex_pyutil/string.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.5.0/PKG-INFO` & `crepex_pyutil-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepex-pyutil
-Version: 0.5.0
+Version: 0.6.0
 Summary: CrepeX python utilities
 Author: Hyunwoo Shim
 Author-email: hyunwoo.shim@crepe-x.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

