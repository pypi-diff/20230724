# Comparing `tmp/mpc_obscodes-2023.7.20.tar.gz` & `tmp/mpc_obscodes-2023.7.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.7.20.tar", last modified: Thu Jul 20 02:28:10 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.7.24.tar", last modified: Mon Jul 24 02:29:45 2023, max compression
```

## Comparing `mpc_obscodes-2023.7.20.tar` & `mpc_obscodes-2023.7.24.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:28:10.865886 mpc_obscodes-2023.7.20/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-20 02:28:10.865886 mpc_obscodes-2023.7.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:28:10.865886 mpc_obscodes-2023.7.20/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   246593 2023-07-20 02:27:59.000000 mpc_obscodes-2023.7.20/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 02:27:59.000000 mpc_obscodes-2023.7.20/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:28:10.865886 mpc_obscodes-2023.7.20/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-20 02:27:53.000000 mpc_obscodes-2023.7.20/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:28:10.865886 mpc_obscodes-2023.7.20/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-20 02:28:10.000000 mpc_obscodes-2023.7.20/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-20 02:28:10.000000 mpc_obscodes-2023.7.20/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 02:28:10.000000 mpc_obscodes-2023.7.20/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 02:28:10.000000 mpc_obscodes-2023.7.20/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 02:28:10.000000 mpc_obscodes-2023.7.20/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 02:27:59.000000 mpc_obscodes-2023.7.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 02:28:10.865886 mpc_obscodes-2023.7.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:45.699179 mpc_obscodes-2023.7.24/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-24 02:29:45.699179 mpc_obscodes-2023.7.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:45.695179 mpc_obscodes-2023.7.24/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246592 2023-07-24 02:29:34.000000 mpc_obscodes-2023.7.24/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 02:29:34.000000 mpc_obscodes-2023.7.24/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:45.699179 mpc_obscodes-2023.7.24/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 02:29:30.000000 mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:29:45.695179 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 02:29:45.000000 mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-24 02:29:34.000000 mpc_obscodes-2023.7.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:29:45.699179 mpc_obscodes-2023.7.24/setup.cfg
```

### Comparing `mpc_obscodes-2023.7.20/PKG-INFO` & `mpc_obscodes-2023.7.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2023.7.20
+Version: 2023.7.24
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.7.20/README.md` & `mpc_obscodes-2023.7.24/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.20/mpc_obscodes/compare.py` & `mpc_obscodes-2023.7.24/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.20/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.7.24/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.20/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.7.24/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999488124488124%*

 * *Differences: {"'Y05'": "{'cos': 0.94132, 'sin': -0.337075}"}*

```diff
@@ -13924,16 +13924,16 @@
         "Name": "SONEAR 2 Observatory, Belo Horizonte",
         "cos": 0.94089,
         "sin": -0.337985
     },
     "Y05": {
         "Longitude": 316.31,
         "Name": "SONEAR Wykrota-CEAMIG, Serra da Piedade",
-        "cos": 0.941254,
-        "sin": -0.337051
+        "cos": 0.94132,
+        "sin": -0.337075
     },
     "Y16": {
         "Longitude": 318.68794,
         "Name": "ROCG, Campos dos Goytacazes",
         "cos": 0.929268,
         "sin": -0.36817
     },
```

### Comparing `mpc_obscodes-2023.7.20/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.20/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.20/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2023.7.24/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.7.20/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2023.7.24/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc-obscodes
-Version: 2023.7.20
+Version: 2023.7.24
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.7.20/pyproject.toml` & `mpc_obscodes-2023.7.24/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.07.20"
+version = "2023.07.24"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

