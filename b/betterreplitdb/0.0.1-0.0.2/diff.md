# Comparing `tmp/betterreplitdb-0.0.1.tar.gz` & `tmp/betterreplitdb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterreplitdb-0.0.1.tar", max compression
+gzip compressed data, was "betterreplitdb-0.0.2.tar", max compression
```

## Comparing `betterreplitdb-0.0.1.tar` & `betterreplitdb-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      728 2023-02-26 12:35:10.384068 betterreplitdb-0.0.1/LICENSE
--rw-r--r--   0        0        0     2750 2023-02-26 19:31:54.380586 betterreplitdb-0.0.1/README.md
--rw-r--r--   0        0        0      359 2023-02-26 19:45:58.102989 betterreplitdb-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    28525 2023-02-26 17:37:57.037901 betterreplitdb-0.0.1/src/betterreplitdb.py
--rw-r--r--   0        0        0     3373 1970-01-01 00:00:00.000000 betterreplitdb-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      728 2023-07-24 20:06:47.300281 betterreplitdb-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2750 2023-07-24 20:06:47.300281 betterreplitdb-0.0.2/README.md
+-rw-r--r--   0        0        0      361 2023-07-24 20:11:32.635538 betterreplitdb-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    28525 2023-07-24 20:06:47.300281 betterreplitdb-0.0.2/src/betterreplitdb.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 betterreplitdb-0.0.2/PKG-INFO
```

### Comparing `betterreplitdb-0.0.1/LICENSE` & `betterreplitdb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `betterreplitdb-0.0.1/README.md` & `betterreplitdb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `betterreplitdb-0.0.1/src/betterreplitdb.py` & `betterreplitdb-0.0.2/src/betterreplitdb.py`

 * *Files identical despite different names*

### Comparing `betterreplitdb-0.0.1/PKG-INFO` & `betterreplitdb-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: betterreplitdb
-Version: 0.0.1
+Version: 0.0.2
 Summary: Replit DB with a memcache
 License: ISC
 Author: Dev380
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (==3.6.2)
+Requires-Dist: aiohttp (>=3.6.2,<4.0.0)
 Requires-Dist: black (>=23.1.0,<24.0.0)
-Requires-Dist: requests (==2.25.1)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Better Replit DB (Python)
 
 *Adds a memcache to the standard replit database*
```

