# Comparing `tmp/pydid-0.3.9a0.tar.gz` & `tmp/pydid-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydid-0.3.9a0.tar", max compression
+gzip compressed data, was "pydid-0.4.0a0.tar", max compression
```

## Comparing `pydid-0.3.9a0.tar` & `pydid-0.4.0a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-07-08 15:51:00.765497 pydid-0.3.9a0/LICENSE
--rw-r--r--   0        0        0      848 2023-07-08 15:51:00.765497 pydid-0.3.9a0/README.md
--rw-r--r--   0        0        0     1680 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/__init__.py
--rw-r--r--   0        0        0      318 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/common.py
--rw-r--r--   0        0        0     2294 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/did.py
--rw-r--r--   0        0        0     2773 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/did_url.py
--rw-r--r--   0        0        0      560 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/__init__.py
--rw-r--r--   0        0        0     8263 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/builder.py
--rw-r--r--   0        0        0     1322 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/corrections.py
--rw-r--r--   0        0        0     8287 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/doc.py
--rw-r--r--   0        0        0     1807 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/doc/generic.py
--rw-r--r--   0        0        0     4647 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/resource.py
--rw-r--r--   0        0        0     1463 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/service.py
--rw-r--r--   0        0        0     1002 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/validation.py
--rw-r--r--   0        0        0     8458 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pydid/verification_method.py
--rw-r--r--   0        0        0     1106 2023-07-08 15:51:00.765497 pydid-0.3.9a0/pyproject.toml
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 pydid-0.3.9a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 17:20:12.110167 pydid-0.4.0a0/LICENSE
+-rw-r--r--   0        0        0      848 2023-07-24 17:20:12.110167 pydid-0.4.0a0/README.md
+-rw-r--r--   0        0        0     1680 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/__init__.py
+-rw-r--r--   0        0        0      318 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/common.py
+-rw-r--r--   0        0        0     2294 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/did.py
+-rw-r--r--   0        0        0     2773 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/did_url.py
+-rw-r--r--   0        0        0      560 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/doc/__init__.py
+-rw-r--r--   0        0        0     8263 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/doc/builder.py
+-rw-r--r--   0        0        0     1322 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/doc/corrections.py
+-rw-r--r--   0        0        0     8287 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/doc/doc.py
+-rw-r--r--   0        0        0     1807 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/doc/generic.py
+-rw-r--r--   0        0        0     4647 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/resource.py
+-rw-r--r--   0        0        0     1463 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/service.py
+-rw-r--r--   0        0        0     1002 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/validation.py
+-rw-r--r--   0        0        0     8458 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pydid/verification_method.py
+-rw-r--r--   0        0        0     1100 2023-07-24 17:20:12.118167 pydid-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 pydid-0.4.0a0/PKG-INFO
```

### Comparing `pydid-0.3.9a0/LICENSE` & `pydid-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/README.md` & `pydid-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/__init__.py` & `pydid-0.4.0a0/pydid/__init__.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/did.py` & `pydid-0.4.0a0/pydid/did.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/did_url.py` & `pydid-0.4.0a0/pydid/did_url.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/doc/__init__.py` & `pydid-0.4.0a0/pydid/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/doc/builder.py` & `pydid-0.4.0a0/pydid/doc/builder.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/doc/corrections.py` & `pydid-0.4.0a0/pydid/doc/corrections.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/doc/doc.py` & `pydid-0.4.0a0/pydid/doc/doc.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/doc/generic.py` & `pydid-0.4.0a0/pydid/doc/generic.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/resource.py` & `pydid-0.4.0a0/pydid/resource.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/service.py` & `pydid-0.4.0a0/pydid/service.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/validation.py` & `pydid-0.4.0a0/pydid/validation.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pydid/verification_method.py` & `pydid-0.4.0a0/pydid/verification_method.py`

 * *Files identical despite different names*

### Comparing `pydid-0.3.9a0/pyproject.toml` & `pydid-0.4.0a0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydid"
-version = "0.3.9a0"
+version = "0.4.0a0"
 description = "Python library for validating, constructing, and representing DIDs and DID Documents"
 authors = ["Daniel Bluhm <dbluhm@pm.me>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/Indicio-tech/pydid"
 repository = "https://github.com/Indicio-tech/pydid"
 keywords = [
@@ -12,29 +12,29 @@
 ]
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = "^3.6.9"
-pydantic = "^1.8.1"
-typing-extensions = ">=4.0.0,<4.1.0"
+python = "^3.9.0"
+pydantic = "^1.10.0"
+typing-extensions = "^4.7.0"
 inflection = "^0.5.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.2"
-black = "^22.3.0"
-poetry = "^1.1.5"
-pre-commit = "^2.11.1"
-flake8 = "^5.0.4"
+pytest = "^7.4.0"
+black = "^23.7.0"
+poetry = "^1.5.0"
+pre-commit = "^3.3.0"
+flake8 = "^6.0.0"
 pytest-coverage = "^0.0"
-aiohttp = "^3.7.4"
-pytest-asyncio = "^0.14.0"
-coverage = {extras = ["toml"], version = "^5.5"}
+aiohttp = "^3.8.0"
+pytest-asyncio = "^0.21.0"
+coverage = {extras = ["toml"], version = "^7.2.0"}
 
 [tool.pytest.ini_options]
 addopts = "-p no:warnings --cov pydid"
 markers = "int: integration tests"
 
 [tool.coverage.report]
 exclude_lines = [
```

### Comparing `pydid-0.3.9a0/PKG-INFO` & `pydid-0.4.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: pydid
-Version: 0.3.9a0
+Version: 0.4.0a0
 Summary: Python library for validating, constructing, and representing DIDs and DID Documents
 Home-page: https://github.com/Indicio-tech/pydid
 License: Apache 2.0
 Keywords: decentralized,identity,ssi
 Author: Daniel Bluhm
 Author-email: dbluhm@pm.me
-Requires-Python: >=3.6.9,<4.0.0
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
-Requires-Dist: pydantic (>=1.8.1,<2.0.0)
-Requires-Dist: typing-extensions (>=4.0.0,<4.1.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: typing-extensions (>=4.7.0,<5.0.0)
 Project-URL: Repository, https://github.com/Indicio-tech/pydid
 Description-Content-Type: text/markdown
 
 # PyDID
 
 [![pypi release](https://img.shields.io/pypi/v/pydid)](https://pypi.org/project/pydid/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
```

