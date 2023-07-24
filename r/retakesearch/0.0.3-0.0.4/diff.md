# Comparing `tmp/retakesearch-0.0.3.tar.gz` & `tmp/retakesearch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.0.3.tar", max compression
+gzip compressed data, was "retakesearch-0.0.4.tar", max compression
```

## Comparing `retakesearch-0.0.3.tar` & `retakesearch-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-24 21:07:51.988951 retakesearch-0.0.3/README.md
--rw-r--r--   0        0        0      412 2023-07-24 21:08:15.341048 retakesearch-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-24 21:07:51.988951 retakesearch-0.0.3/retakesearch/__init__.py
--rw-r--r--   0        0        0     2471 2023-07-24 21:07:51.988951 retakesearch-0.0.3/retakesearch/client.py
--rw-r--r--   0        0        0       67 2023-07-24 21:07:51.988951 retakesearch-0.0.3/retakesearch/search.py
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 retakesearch-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 21:10:19.379558 retakesearch-0.0.4/README.md
+-rw-r--r--   0        0        0      412 2023-07-24 21:10:37.423494 retakesearch-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-24 21:10:19.379558 retakesearch-0.0.4/retakesearch/__init__.py
+-rw-r--r--   0        0        0     2471 2023-07-24 21:10:19.379558 retakesearch-0.0.4/retakesearch/client.py
+-rw-r--r--   0        0        0       67 2023-07-24 21:10:19.379558 retakesearch-0.0.4/retakesearch/search.py
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 retakesearch-0.0.4/PKG-INFO
```

### Comparing `retakesearch-0.0.3/retakesearch/client.py` & `retakesearch-0.0.4/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.0.3/PKG-INFO` & `retakesearch-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Open Source Search Infrastructure for Developers
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

