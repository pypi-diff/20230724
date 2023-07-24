# Comparing `tmp/databrowser-0.1.3.tar.gz` & `tmp/databrowser-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databrowser-0.1.3.tar", max compression
+gzip compressed data, was "databrowser-0.26.0.tar", max compression
```

## Comparing `databrowser-0.1.3.tar` & `databrowser-0.26.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-03-19 11:53:06.886355 databrowser-0.1.3/LICENSE
--rw-r--r--   0        0        0     1139 2023-04-10 15:34:17.335155 databrowser-0.1.3/README.md
--rw-r--r--   0        0        0     1199 2023-04-10 16:28:44.526146 databrowser-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 15:34:17.342376 databrowser-0.1.3/src/databrowser/__init__.py
--rw-r--r--   0        0        0      353 2023-04-10 15:34:17.346013 databrowser-0.1.3/src/databrowser/data_browser.css
--rw-r--r--   0        0        0     4256 2023-04-10 16:19:44.558279 databrowser-0.1.3/src/databrowser/data_browser.py
--rw-r--r--   0        0        0      118 2023-04-10 15:34:17.350519 databrowser-0.1.3/src/databrowser/widgets/__init__.py
--rw-r--r--   0        0        0     6522 2023-04-10 16:14:58.950117 databrowser-0.1.3/src/databrowser/widgets/_directory_filter_tree.py
--rw-r--r--   0        0        0     2161 1970-01-01 00:00:00.000000 databrowser-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-03-19 11:53:06.886355 databrowser-0.26.0/LICENSE
+-rw-r--r--   0        0        0     1139 2023-04-10 15:34:17.335155 databrowser-0.26.0/README.md
+-rw-r--r--   0        0        0     1203 2023-07-24 09:37:57.814335 databrowser-0.26.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 15:34:17.342376 databrowser-0.26.0/src/databrowser/__init__.py
+-rw-r--r--   0        0        0      353 2023-04-10 15:34:17.346013 databrowser-0.26.0/src/databrowser/data_browser.css
+-rw-r--r--   0        0        0     4256 2023-04-10 16:19:44.558279 databrowser-0.26.0/src/databrowser/data_browser.py
+-rw-r--r--   0        0        0      118 2023-04-10 15:34:17.350519 databrowser-0.26.0/src/databrowser/widgets/__init__.py
+-rw-r--r--   0        0        0     6522 2023-04-10 16:14:58.950117 databrowser-0.26.0/src/databrowser/widgets/_directory_filter_tree.py
+-rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 databrowser-0.26.0/PKG-INFO
```

### Comparing `databrowser-0.1.3/LICENSE` & `databrowser-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databrowser-0.1.3/README.md` & `databrowser-0.26.0/README.md`

 * *Files identical despite different names*

### Comparing `databrowser-0.1.3/pyproject.toml` & `databrowser-0.26.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "databrowser"
-version = "0.1.3"
+version = "0.26.0"
 description = "Quick tool to browse and view data files (json,csv,parquet,more) on local disk and s3"
 authors = ["Jacob Verhoeks <jacob.verhoeks@gmail.com>"]
 repository = "https://github.com/jverhoeks/databrowser"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 s3fs = {extras = ["boto3"], version = "^2023.3.0"}
 s3path = "^0.4.1"
-pandas = "^1.5.2"
-textual = ">=0.16,<0.20"
+pandas = ">=1.5.2,<3.0.0"
+textual = "0.29.0"
 pyarrow = ">=5.0.0"
 xlrd = "^2.0.1"
 beautifulsoup4 = "^4.12.2"
 lxml = "^4.9.2"
 html5lib = "^1.1"
 
 [tool.poetry.group.dev.dependencies]
@@ -54,8 +54,8 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.pytest.ini_options]
 log_cli = true
-log_cli_level = "INFO"
+log_cli_level = "INFO"
```

### Comparing `databrowser-0.1.3/src/databrowser/data_browser.py` & `databrowser-0.26.0/src/databrowser/data_browser.py`

 * *Files identical despite different names*

### Comparing `databrowser-0.1.3/src/databrowser/widgets/_directory_filter_tree.py` & `databrowser-0.26.0/src/databrowser/widgets/_directory_filter_tree.py`

 * *Files identical despite different names*

### Comparing `databrowser-0.1.3/PKG-INFO` & `databrowser-0.26.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: databrowser
-Version: 0.1.3
+Version: 0.26.0
 Summary: Quick tool to browse and view data files (json,csv,parquet,more) on local disk and s3
 Home-page: https://github.com/jverhoeks/databrowser
 License: MIT
 Author: Jacob Verhoeks
 Author-email: jacob.verhoeks@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pandas (>=1.5.2,<3.0.0)
 Requires-Dist: pyarrow (>=5.0.0)
 Requires-Dist: s3fs[boto3] (>=2023.3.0,<2024.0.0)
 Requires-Dist: s3path (>=0.4.1,<0.5.0)
-Requires-Dist: textual (>=0.16,<0.20)
+Requires-Dist: textual (==0.29.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/jverhoeks/databrowser
 Description-Content-Type: text/markdown
 
 # databrowser
 
 A easy file browser to view data files.
```

