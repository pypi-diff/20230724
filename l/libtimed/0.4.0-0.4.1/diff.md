# Comparing `tmp/libtimed-0.4.0.tar.gz` & `tmp/libtimed-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtimed-0.4.0.tar", max compression
+gzip compressed data, was "libtimed-0.4.1.tar", max compression
```

## Comparing `libtimed-0.4.0.tar` & `libtimed-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34454 2023-07-22 15:47:31.766713 libtimed-0.4.0/LICENSE
--rw-r--r--   0        0        0      750 2023-07-22 15:47:31.766713 libtimed-0.4.0/README.md
--rw-r--r--   0        0        0     1307 2023-07-22 15:47:32.518713 libtimed-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1376 2023-07-22 15:47:31.770712 libtimed-0.4.0/src/libtimed/__init__.py
--rw-r--r--   0        0        0     9535 2023-07-22 15:47:31.770712 libtimed-0.4.0/src/libtimed/models.py
--rw-r--r--   0        0        0     4555 2023-07-22 15:47:31.770712 libtimed-0.4.0/src/libtimed/oidc.py
--rw-r--r--   0        0        0     6134 2023-07-22 15:47:31.770712 libtimed-0.4.0/src/libtimed/transforms.py
--rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-24 07:04:48.375942 libtimed-0.4.1/LICENSE
+-rw-r--r--   0        0        0      750 2023-07-24 07:04:48.375942 libtimed-0.4.1/README.md
+-rw-r--r--   0        0        0     1307 2023-07-24 07:04:49.379943 libtimed-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1376 2023-07-24 07:04:48.375942 libtimed-0.4.1/src/libtimed/__init__.py
+-rw-r--r--   0        0        0     9536 2023-07-24 07:04:48.375942 libtimed-0.4.1/src/libtimed/models.py
+-rw-r--r--   0        0        0     4555 2023-07-24 07:04:48.375942 libtimed-0.4.1/src/libtimed/oidc.py
+-rw-r--r--   0        0        0     6134 2023-07-24 07:04:48.375942 libtimed-0.4.1/src/libtimed/transforms.py
+-rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.4.1/PKG-INFO
```

### Comparing `libtimed-0.4.0/LICENSE` & `libtimed-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.0/README.md` & `libtimed-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.0/pyproject.toml` & `libtimed-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libtimed"
-version = "0.4.0"
+version = "0.4.1"
 description = "Library to intreact with timed webapp."
 authors = [
   "Arthur Deierlein <arthur.deierlein@adfinis.com>",
   "Gian Klug <gian.klug@adfinis.com>",
 ]
 readme = "README.md"
 packages = [{ include = "libtimed", from = "src" }]
```

### Comparing `libtimed-0.4.0/src/libtimed/__init__.py` & `libtimed-0.4.1/src/libtimed/__init__.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.0/src/libtimed/models.py` & `libtimed-0.4.1/src/libtimed/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional, Union
 
 from inflection import underscore
 from requests import Response
 
 from libtimed import transforms
 
-ARCHIVED = ("archived", None, transforms.Type(bool, pipe=int))
+ARCHIVED = ("archived", False, transforms.Type(bool, pipe=int))
 DATE = ("date", date.today(), transforms.Date)
 FROM_DATE = ("from_date", None, transforms.Date)
 TO_DATE = ("to_date", None, transforms.Date)
 DURATION = ("duration", timedelta(minutes=15), transforms.Duration)
 COMMENT = ("comment", "", transforms.Type(str, False))
 REVIEW = ("review", False, transforms.Type(bool, False))
 NOT_BILLABLE = ("not-billable", False, transforms.Type(bool, False))
```

### Comparing `libtimed-0.4.0/src/libtimed/oidc.py` & `libtimed-0.4.1/src/libtimed/oidc.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.0/src/libtimed/transforms.py` & `libtimed-0.4.1/src/libtimed/transforms.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.0/PKG-INFO` & `libtimed-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libtimed
-Version: 0.4.0
+Version: 0.4.1
 Summary: Library to intreact with timed webapp.
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

