# Comparing `tmp/retakesearch-0.0.0.tar.gz` & `tmp/retakesearch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.0.0.tar", max compression
+gzip compressed data, was "retakesearch-0.0.2.tar", max compression
```

## Comparing `retakesearch-0.0.0.tar` & `retakesearch-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-23 15:55:12.716126 retakesearch-0.0.0/README.md
--rw-r--r--   0        0        0      412 2023-07-23 18:58:28.361654 retakesearch-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-23 18:48:24.114748 retakesearch-0.0.0/retakesearch/__init__.py
--rw-r--r--   0        0        0     2471 2023-07-23 18:48:24.151791 retakesearch-0.0.0/retakesearch/client.py
--rw-r--r--   0        0        0       67 2023-07-23 18:48:24.117198 retakesearch-0.0.0/retakesearch/search.py
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 retakesearch-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 20:52:48.647227 retakesearch-0.0.2/README.md
+-rw-r--r--   0        0        0      412 2023-07-24 20:53:06.147400 retakesearch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-24 20:52:48.647227 retakesearch-0.0.2/retakesearch/__init__.py
+-rw-r--r--   0        0        0     2471 2023-07-24 20:52:48.647227 retakesearch-0.0.2/retakesearch/client.py
+-rw-r--r--   0        0        0       67 2023-07-24 20:52:48.647227 retakesearch-0.0.2/retakesearch/search.py
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 retakesearch-0.0.2/PKG-INFO
```

### Comparing `retakesearch-0.0.0/retakesearch/client.py` & `retakesearch-0.0.2/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.0.0/PKG-INFO` & `retakesearch-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.0.0
+Version: 0.0.2
 Summary: Open Source Search Infrastructure for Developers
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

