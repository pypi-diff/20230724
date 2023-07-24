# Comparing `tmp/pynatrace-1.6.2.tar.gz` & `tmp/pynatrace-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynatrace-1.6.2.tar", max compression
+gzip compressed data, was "pynatrace-1.7.0.tar", max compression
```

## Comparing `pynatrace-1.6.2.tar` & `pynatrace-1.7.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1163 2022-05-24 15:19:33.389537 pynatrace-1.6.2/LICENSE
--rw-r--r--   0        0        0      358 2022-05-31 18:47:22.814394 pynatrace-1.6.2/README.md
--rw-r--r--   0        0        0      588 2022-05-31 18:54:28.704898 pynatrace-1.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-24 15:19:33.386537 pynatrace-1.6.2/src/pynatrace/__init__.py
--rw-r--r--   0        0        0     5679 2022-05-31 18:48:57.818730 pynatrace-1.6.2/src/pynatrace/cli.py
--rw-r--r--   0        0        0     1254 2022-05-31 18:54:47.130392 pynatrace-1.6.2/setup.py
--rw-r--r--   0        0        0     1013 2022-05-31 18:54:47.131239 pynatrace-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1163 2022-05-24 15:19:33.389537 pynatrace-1.7.0/LICENSE
+-rw-r--r--   0        0        0      358 2022-05-31 18:47:22.814394 pynatrace-1.7.0/README.md
+-rw-r--r--   0        0        0      668 2023-07-24 13:53:27.662218 pynatrace-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-05-24 15:19:33.386537 pynatrace-1.7.0/src/pynatrace/__init__.py
+-rw-r--r--   0        0        0     5679 2022-05-31 18:48:57.818730 pynatrace-1.7.0/src/pynatrace/cli.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pynatrace-1.7.0/PKG-INFO
```

### Comparing `pynatrace-1.6.2/LICENSE` & `pynatrace-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynatrace-1.6.2/pyproject.toml` & `pynatrace-1.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [tool.poetry]
 name = "pynatrace"
-version = "1.6.2"
+version = "1.7.0"
 description = "Python limited CLI for Dynatrace"
 authors = ["Michael MacKenna <mmackenna@unitedfiregroup.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.27.1"
 click = "^8.1.3"
-termcolor = "^1.1.0"
+termcolor = "^2.2.0"
 dt = "^1.1.48"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.13.9"
 ipython = "^8.3.0"
 black = "^22.3.0"
 jupyter = "^1.0.0"
 mdv = "^1.7.4"
 
 [tool.poetry.scripts]
 pynatrace = 'pynatrace.cli:main'
 
+[tool.poetry.group.dev.dependencies]
+mkdocs = "^1.4.3"
+mkdocs-click = "^0.8.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pynatrace-1.6.2/src/pynatrace/cli.py` & `pynatrace-1.7.0/src/pynatrace/cli.py`

 * *Files identical despite different names*

### Comparing `pynatrace-1.6.2/PKG-INFO` & `pynatrace-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pynatrace
-Version: 1.6.2
+Version: 1.7.0
 Summary: Python limited CLI for Dynatrace
 License: MIT
 Author: Michael MacKenna
 Author-email: mmackenna@unitedfiregroup.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dt (>=1.1.48,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: termcolor (>=1.1.0,<2.0.0)
+Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pynatrace
 
 Python CLI for Dynatrace
 =======
```

