# Comparing `tmp/betterreplitdb-0.0.2.tar.gz` & `tmp/betterreplitdb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterreplitdb-0.0.2.tar", max compression
+gzip compressed data, was "betterreplitdb-0.0.3.tar", max compression
```

## Comparing `betterreplitdb-0.0.2.tar` & `betterreplitdb-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      728 2023-07-24 20:06:47.300281 betterreplitdb-0.0.2/LICENSE
--rw-r--r--   0        0        0     2750 2023-07-24 20:06:47.300281 betterreplitdb-0.0.2/README.md
--rw-r--r--   0        0        0      361 2023-07-24 20:11:32.635538 betterreplitdb-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    28525 2023-07-24 20:06:47.300281 betterreplitdb-0.0.2/src/betterreplitdb.py
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 betterreplitdb-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      728 2023-07-24 20:06:47.300281 betterreplitdb-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2750 2023-07-24 20:06:47.300281 betterreplitdb-0.0.3/README.md
+-rw-r--r--   0        0        0      361 2023-07-24 20:35:22.398378 betterreplitdb-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    28525 2023-07-24 20:06:47.300281 betterreplitdb-0.0.3/src/betterreplitdb.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 betterreplitdb-0.0.3/PKG-INFO
```

### Comparing `betterreplitdb-0.0.2/LICENSE` & `betterreplitdb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `betterreplitdb-0.0.2/README.md` & `betterreplitdb-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `betterreplitdb-0.0.2/src/betterreplitdb.py` & `betterreplitdb-0.0.3/src/betterreplitdb.py`

 * *Files identical despite different names*

### Comparing `betterreplitdb-0.0.2/PKG-INFO` & `betterreplitdb-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterreplitdb
-Version: 0.0.2
+Version: 0.0.3
 Summary: Replit DB with a memcache
 License: ISC
 Author: Dev380
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

