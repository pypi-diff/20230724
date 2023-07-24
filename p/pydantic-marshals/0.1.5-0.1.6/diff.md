# Comparing `tmp/pydantic_marshals-0.1.5.tar.gz` & `tmp/pydantic_marshals-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_marshals-0.1.5.tar", max compression
+gzip compressed data, was "pydantic_marshals-0.1.6.tar", max compression
```

## Comparing `pydantic_marshals-0.1.5.tar` & `pydantic_marshals-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2023-07-24 15:23:44.444272 pydantic_marshals-0.1.5/pydantic_marshals/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 15:23:44.444272 pydantic_marshals-0.1.5/pydantic_marshals/fields/__init__.py
--rw-r--r--   0        0        0     2141 2023-07-24 16:21:12.685692 pydantic_marshals-0.1.5/pydantic_marshals/fields/base.py
--rw-r--r--   0        0        0     1564 2023-07-24 17:10:13.355398 pydantic_marshals-0.1.5/pydantic_marshals/fields/properties.py
--rw-r--r--   0        0        0        0 2023-07-24 17:37:20.443298 pydantic_marshals-0.1.5/pydantic_marshals/fields/py.typed
--rw-r--r--   0        0        0        0 2023-07-24 16:21:13.724902 pydantic_marshals-0.1.5/pydantic_marshals/fields/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-24 16:21:13.724902 pydantic_marshals-0.1.5/pydantic_marshals/fields/sqlalchemy/columns.py
--rw-r--r--   0        0        0        0 2023-07-24 17:37:25.616136 pydantic_marshals-0.1.5/pydantic_marshals/fields/sqlalchemy/py.typed
--rw-r--r--   0        0        0     1785 2023-07-24 17:10:11.383393 pydantic_marshals-0.1.5/pydantic_marshals/fields/sqlalchemy/relationships.py
--rw-r--r--   0        0        0        0 2023-07-24 15:23:44.444272 pydantic_marshals-0.1.5/pydantic_marshals/models/__init__.py
--rw-r--r--   0        0        0     4523 2023-07-24 15:24:52.674538 pydantic_marshals-0.1.5/pydantic_marshals/models/base.py
--rw-r--r--   0        0        0        0 2023-07-24 17:37:35.734218 pydantic_marshals-0.1.5/pydantic_marshals/models/py.typed
--rw-r--r--   0        0        0     2261 2023-07-24 17:10:13.723986 pydantic_marshals-0.1.5/pydantic_marshals/models/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-07-24 17:10:13.711932 pydantic_marshals-0.1.5/pydantic_marshals/mypy/__init__.py
--rw-r--r--   0        0        0      764 2023-07-24 17:31:24.845118 pydantic_marshals-0.1.5/pydantic_marshals/mypy/magic.pyi
--rw-r--r--   0        0        0     1672 2023-07-24 17:30:02.365323 pydantic_marshals-0.1.5/pydantic_marshals/mypy/plugin.py
--rw-r--r--   0        0        0        0 2023-07-24 17:37:43.378209 pydantic_marshals-0.1.5/pydantic_marshals/mypy/py.typed
--rw-r--r--   0        0        0        0 2023-07-24 17:37:50.209216 pydantic_marshals-0.1.5/pydantic_marshals/py.typed
--rw-r--r--   0        0        0      262 2023-07-24 17:10:13.343190 pydantic_marshals-0.1.5/pydantic_marshals/utils.py
--rw-r--r--   0        0        0     1436 2023-07-24 17:38:37.853884 pydantic_marshals-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      624 2023-07-23 20:50:24.552860 pydantic_marshals-0.1.5/README.md
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 pydantic_marshals-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 15:23:44.444272 pydantic_marshals-0.1.6/pydantic_marshals/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:23:44.444272 pydantic_marshals-0.1.6/pydantic_marshals/fields/__init__.py
+-rw-r--r--   0        0        0     2141 2023-07-24 16:21:12.685692 pydantic_marshals-0.1.6/pydantic_marshals/fields/base.py
+-rw-r--r--   0        0        0     1564 2023-07-24 17:10:13.355398 pydantic_marshals-0.1.6/pydantic_marshals/fields/properties.py
+-rw-r--r--   0        0        0        0 2023-07-24 17:37:20.443298 pydantic_marshals-0.1.6/pydantic_marshals/fields/py.typed
+-rw-r--r--   0        0        0        0 2023-07-24 16:21:13.724902 pydantic_marshals-0.1.6/pydantic_marshals/fields/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-24 16:21:13.724902 pydantic_marshals-0.1.6/pydantic_marshals/fields/sqlalchemy/columns.py
+-rw-r--r--   0        0        0        0 2023-07-24 17:37:25.616136 pydantic_marshals-0.1.6/pydantic_marshals/fields/sqlalchemy/py.typed
+-rw-r--r--   0        0        0     1785 2023-07-24 17:10:11.383393 pydantic_marshals-0.1.6/pydantic_marshals/fields/sqlalchemy/relationships.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:23:44.444272 pydantic_marshals-0.1.6/pydantic_marshals/models/__init__.py
+-rw-r--r--   0        0        0     4523 2023-07-24 15:24:52.674538 pydantic_marshals-0.1.6/pydantic_marshals/models/base.py
+-rw-r--r--   0        0        0        0 2023-07-24 17:37:35.734218 pydantic_marshals-0.1.6/pydantic_marshals/models/py.typed
+-rw-r--r--   0        0        0     2261 2023-07-24 17:10:13.723986 pydantic_marshals-0.1.6/pydantic_marshals/models/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-24 17:10:13.711932 pydantic_marshals-0.1.6/pydantic_marshals/mypy/__init__.py
+-rw-r--r--   0        0        0      764 2023-07-24 17:31:24.845118 pydantic_marshals-0.1.6/pydantic_marshals/mypy/magic.pyi
+-rw-r--r--   0        0        0     1672 2023-07-24 17:30:02.365323 pydantic_marshals-0.1.6/pydantic_marshals/mypy/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-24 17:37:43.378209 pydantic_marshals-0.1.6/pydantic_marshals/mypy/py.typed
+-rw-r--r--   0        0        0        0 2023-07-24 17:37:50.209216 pydantic_marshals-0.1.6/pydantic_marshals/py.typed
+-rw-r--r--   0        0        0      262 2023-07-24 17:10:13.343190 pydantic_marshals-0.1.6/pydantic_marshals/utils.py
+-rw-r--r--   0        0        0     1483 2023-07-24 17:41:52.811372 pydantic_marshals-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      624 2023-07-23 20:50:24.552860 pydantic_marshals-0.1.6/README.md
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 pydantic_marshals-0.1.6/PKG-INFO
```

### Comparing `pydantic_marshals-0.1.5/pydantic_marshals/fields/base.py` & `pydantic_marshals-0.1.6/pydantic_marshals/fields/base.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/pydantic_marshals/fields/properties.py` & `pydantic_marshals-0.1.6/pydantic_marshals/fields/properties.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/pydantic_marshals/fields/sqlalchemy/columns.py` & `pydantic_marshals-0.1.6/pydantic_marshals/fields/sqlalchemy/columns.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/pydantic_marshals/fields/sqlalchemy/relationships.py` & `pydantic_marshals-0.1.6/pydantic_marshals/fields/sqlalchemy/relationships.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/pydantic_marshals/models/base.py` & `pydantic_marshals-0.1.6/pydantic_marshals/models/base.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/pydantic_marshals/models/sqlalchemy.py` & `pydantic_marshals-0.1.6/pydantic_marshals/models/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/pydantic_marshals/mypy/magic.pyi` & `pydantic_marshals-0.1.6/pydantic_marshals/mypy/magic.pyi`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/pydantic_marshals/mypy/plugin.py` & `pydantic_marshals-0.1.6/pydantic_marshals/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/pyproject.toml` & `pydantic_marshals-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [tool.poetry]
 name = "pydantic-marshals"
-version = "0.1.5"
+version = "0.1.6"
 description = "Library for creating partial pydantic models (automatic converters) from different mappings"
 authors = ["niqzart <niqzart@gmail.com>"]
 readme = "README.md"
+exclude = [
+    "examples",
+    "tests",
+]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = ">=2.0,<3.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
```

### Comparing `pydantic_marshals-0.1.5/README.md` & `pydantic_marshals-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.1.5/PKG-INFO` & `pydantic_marshals-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-marshals
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for creating partial pydantic models (automatic converters) from different mappings
 Author: niqzart
 Author-email: niqzart@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=2.0,<3.0)
```

