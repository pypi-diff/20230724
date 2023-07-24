# Comparing `tmp/plyfile-1.0.tar.gz` & `tmp/plyfile-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyfile-1.0.tar", last modified: Mon Jul 10 06:45:14 2023, max compression
+gzip compressed data, was "plyfile-1.0.1.tar", last modified: Mon Jul 24 02:43:06 2023, max compression
```

## Comparing `plyfile-1.0.tar` & `plyfile-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35147 2023-07-02 02:49:51.243322 plyfile-1.0/COPYING
--rw-r--r--   0        0        0     1144 2023-07-02 02:49:51.243322 plyfile-1.0/README.md
--rw-r--r--   0        0        0    42554 2023-07-02 02:49:51.243322 plyfile-1.0/plyfile.py
--rw-r--r--   0        0        0     1538 2023-07-10 06:41:40.695934 plyfile-1.0/pyproject.toml
--rw-r--r--   0        0        0     2029 1970-01-01 00:00:00.000000 plyfile-1.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-02 02:49:51.243322 plyfile-1.0.1/COPYING
+-rw-r--r--   0        0        0     1144 2023-07-02 02:49:51.243322 plyfile-1.0.1/README.md
+-rw-r--r--   0        0        0    42554 2023-07-02 02:49:51.243322 plyfile-1.0.1/plyfile.py
+-rw-r--r--   0        0        0     1553 2023-07-24 02:38:17.796527 plyfile-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 plyfile-1.0.1/PKG-INFO
```

### Comparing `plyfile-1.0/COPYING` & `plyfile-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `plyfile-1.0/README.md` & `plyfile-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `plyfile-1.0/plyfile.py` & `plyfile-1.0.1/plyfile.py`

 * *Files identical despite different names*

### Comparing `plyfile-1.0/pyproject.toml` & `plyfile-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 test-matrix = "tox -v --skip-missing-interpreters=true"
 test-all = "tox -v --skip-missing-interpreters=false"
 doc = "sphinx-build doc doc/build -b html"
 lint = "flake8 plyfile.py test/test_plyfile.py"
 
 [project]
 name = "plyfile"
-version = "1.0"
+version = "1.0.1"
 description = "PLY file reader/writer"
 authors = [
     { name = "Darsh Ranjan", email = "dranjan@berkeley.edu" },
 ]
 dependencies = [
     "numpy>=1.17",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "ply",
     "numpy",
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `plyfile-1.0/PKG-INFO` & `plyfile-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: plyfile
-Version: 1.0
+Version: 1.0.1
 Summary: PLY file reader/writer
 Keywords: ply,numpy
 Author-email: Darsh Ranjan <dranjan@berkeley.edu>
 Requires-Python: >=3.8
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

