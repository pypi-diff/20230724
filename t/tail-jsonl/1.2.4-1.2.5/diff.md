# Comparing `tmp/tail_jsonl-1.2.4.tar.gz` & `tmp/tail_jsonl-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tail_jsonl-1.2.4.tar", max compression
+gzip compressed data, was "tail_jsonl-1.2.5.tar", max compression
```

## Comparing `tail_jsonl-1.2.4.tar` & `tail_jsonl-1.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-06-17 13:45:06.556013 tail_jsonl-1.2.4/LICENSE
--rw-r--r--   0        0        0     3288 2023-06-17 14:26:26.308819 tail_jsonl-1.2.4/docs/README.md
--rw-r--r--   0        0        0     1516 2023-06-17 14:26:21.598040 tail_jsonl-1.2.4/pyproject.toml
--rw-r--r--   0        0        0      233 2023-06-17 14:26:21.593339 tail_jsonl-1.2.4/tail_jsonl/__init__.py
--rw-r--r--   0        0        0        0 2023-01-31 09:03:15.236071 tail_jsonl-1.2.4/tail_jsonl/_private/__init__.py
--rw-r--r--   0        0        0     2755 2023-06-17 13:27:03.021123 tail_jsonl-1.2.4/tail_jsonl/_private/core.py
--rw-r--r--   0        0        0      698 2023-02-25 23:44:27.489284 tail_jsonl-1.2.4/tail_jsonl/config.py
--rw-r--r--   0        0        0     1406 2023-03-02 03:09:37.979638 tail_jsonl-1.2.4/tail_jsonl/scripts.py
--rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 tail_jsonl-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-17 13:45:06.556013 tail_jsonl-1.2.5/LICENSE
+-rw-r--r--   0        0        0     3288 2023-07-23 22:44:39.451708 tail_jsonl-1.2.5/docs/README.md
+-rw-r--r--   0        0        0     1537 2023-07-23 22:44:33.777205 tail_jsonl-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0      233 2023-07-23 22:44:33.770504 tail_jsonl-1.2.5/tail_jsonl/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-31 09:03:15.236071 tail_jsonl-1.2.5/tail_jsonl/_private/__init__.py
+-rw-r--r--   0        0        0     2755 2023-06-17 13:27:03.021123 tail_jsonl-1.2.5/tail_jsonl/_private/core.py
+-rw-r--r--   0        0        0      698 2023-02-25 23:44:27.489284 tail_jsonl-1.2.5/tail_jsonl/config.py
+-rw-r--r--   0        0        0     1406 2023-07-23 22:41:43.630084 tail_jsonl-1.2.5/tail_jsonl/scripts.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 tail_jsonl-1.2.5/PKG-INFO
```

### Comparing `tail_jsonl-1.2.4/LICENSE` & `tail_jsonl-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tail_jsonl-1.2.4/docs/README.md` & `tail_jsonl-1.2.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `tail_jsonl-1.2.4/pyproject.toml` & `tail_jsonl-1.2.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.4"
+version = "1.2.5"
 version_files = ["pyproject.toml:^version", "tail_jsonl/__init__.py:^__version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
@@ -22,24 +22,25 @@
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "tail_jsonl"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/tail-jsonl"
-version = "1.2.4"
+version = "1.2.5"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
-corallium = ">=0.2.2"
+corallium = ">=0.3.0"
 dotted-notation = ">=0.9.2"
+pydantic = ">=2.0.3"
 
 [tool.poetry.group.dev.dependencies]
-calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=1.2.4"}
-pytest-cache-assert = ">=3.0.7"
+calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=1.5.0"}
+pytest-cache-assert = ">=3.0.8"
 pytest-pretty = ">=1.0.1"
 tomli-w = ">=1.0.0"
 
 [tool.poetry.scripts]
 tail-jsonl = "tail_jsonl.scripts:start"
 
 [tool.poetry.urls]
```

### Comparing `tail_jsonl-1.2.4/tail_jsonl/_private/core.py` & `tail_jsonl-1.2.5/tail_jsonl/_private/core.py`

 * *Files identical despite different names*

### Comparing `tail_jsonl-1.2.4/tail_jsonl/config.py` & `tail_jsonl-1.2.5/tail_jsonl/config.py`

 * *Files identical despite different names*

### Comparing `tail_jsonl-1.2.4/tail_jsonl/scripts.py` & `tail_jsonl-1.2.5/tail_jsonl/scripts.py`

 * *Files identical despite different names*

### Comparing `tail_jsonl-1.2.4/PKG-INFO` & `tail_jsonl-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: tail-jsonl
-Version: 1.2.4
+Version: 1.2.5
 Summary: Pretty Print Tailed JSONL Logs
 Home-page: https://github.com/kyleking/tail-jsonl
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: corallium (>=0.2.2)
+Requires-Dist: corallium (>=0.3.0)
 Requires-Dist: dotted-notation (>=0.9.2)
+Requires-Dist: pydantic (>=2.0.3)
 Project-URL: Bug Tracker, https://github.com/kyleking/tail-jsonl/issues
 Project-URL: Changelog, https://github.com/kyleking/tail-jsonl/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://tail-jsonl.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/tail-jsonl
 Description-Content-Type: text/markdown
 
 # tail-jsonl
```

