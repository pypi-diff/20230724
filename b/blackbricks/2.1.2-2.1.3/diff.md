# Comparing `tmp/blackbricks-2.1.2.tar.gz` & `tmp/blackbricks-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackbricks-2.1.2.tar", max compression
+gzip compressed data, was "blackbricks-2.1.3.tar", max compression
```

## Comparing `blackbricks-2.1.2.tar` & `blackbricks-2.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2023-05-23 12:01:08.318061 blackbricks-2.1.2/LICENSE
--rw-r--r--   0        0        0    11881 2023-05-23 12:01:08.318061 blackbricks-2.1.2/README.md
--rw-r--r--   0        0        0       22 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/__init__.py
--rw-r--r--   0        0        0     4561 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/blackbricks.py
--rw-r--r--   0        0        0     6512 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/cli.py
--rw-r--r--   0        0        0     5430 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/databricks_sync.py
--rw-r--r--   0        0        0     4355 2023-05-23 12:01:08.318061 blackbricks-2.1.2/blackbricks/files.py
--rw-r--r--   0        0        0     1585 2023-05-23 12:01:08.318061 blackbricks-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    13114 1970-01-01 00:00:00.000000 blackbricks-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-24 13:20:13.401854 blackbricks-2.1.3/LICENSE
+-rw-r--r--   0        0        0    11881 2023-07-24 13:20:13.401854 blackbricks-2.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-07-24 13:20:13.401854 blackbricks-2.1.3/blackbricks/__init__.py
+-rw-r--r--   0        0        0     4561 2023-07-24 13:20:13.401854 blackbricks-2.1.3/blackbricks/blackbricks.py
+-rw-r--r--   0        0        0     6512 2023-07-24 13:20:13.401854 blackbricks-2.1.3/blackbricks/cli.py
+-rw-r--r--   0        0        0     5430 2023-07-24 13:20:13.401854 blackbricks-2.1.3/blackbricks/databricks_sync.py
+-rw-r--r--   0        0        0     4355 2023-07-24 13:20:13.401854 blackbricks-2.1.3/blackbricks/files.py
+-rw-r--r--   0        0        0     1585 2023-07-24 13:20:13.405854 blackbricks-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0    13114 1970-01-01 00:00:00.000000 blackbricks-2.1.3/PKG-INFO
```

### Comparing `blackbricks-2.1.2/LICENSE` & `blackbricks-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.2/README.md` & `blackbricks-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.2/blackbricks/blackbricks.py` & `blackbricks-2.1.3/blackbricks/blackbricks.py`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.2/blackbricks/cli.py` & `blackbricks-2.1.3/blackbricks/cli.py`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.2/blackbricks/databricks_sync.py` & `blackbricks-2.1.3/blackbricks/databricks_sync.py`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.2/blackbricks/files.py` & `blackbricks-2.1.3/blackbricks/files.py`

 * *Files identical despite different names*

### Comparing `blackbricks-2.1.2/pyproject.toml` & `blackbricks-2.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackbricks"
-version = "2.1.2"
+version = "2.1.3"
 description = "Black for Databricks notebooks"
 authors = ["Bendik Samseth <bendik.samseth@inspera.no>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/inspera/blackbricks"
 keywords = [
     "automation",
@@ -47,15 +47,15 @@
 flake8 = "^3.9.2"
 commitizen = "^2.32.2"
 mypy = "^0.971"
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.1.2"
+version = "2.1.3"
 tag_format = "$version"
 version_files = ["blackbricks/__init__.py:version", "pyproject.toml:version"]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
```

### Comparing `blackbricks-2.1.2/PKG-INFO` & `blackbricks-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackbricks
-Version: 2.1.2
+Version: 2.1.3
 Summary: Black for Databricks notebooks
 Home-page: https://github.com/inspera/blackbricks
 License: MIT
 Keywords: automation,formatter,black,sql,yapf,autopep8,pyfmt,gofmt,rustfmt
 Author: Bendik Samseth
 Author-email: bendik.samseth@inspera.no
 Requires-Python: >=3.8,<4.0
```

