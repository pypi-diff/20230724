# Comparing `tmp/python_frank_energie-5.0.0.tar.gz` & `tmp/python_frank_energie-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_frank_energie-5.0.0.tar", max compression
+gzip compressed data, was "python_frank_energie-5.0.1.tar", max compression
```

## Comparing `python_frank_energie-5.0.0.tar` & `python_frank_energie-5.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11346 2023-06-12 21:41:16.326471 python_frank_energie-5.0.0/LICENSE
--rw-r--r--   0        0        0     1442 2023-06-12 21:41:16.326471 python_frank_energie-5.0.0/README.md
--rw-r--r--   0        0        0     2352 2023-06-12 21:41:45.992268 python_frank_energie-5.0.0/pyproject.toml
--rw-r--r--   0        0        0      175 2023-06-12 21:41:16.330471 python_frank_energie-5.0.0/python_frank_energie/__init__.py
--rw-r--r--   0        0        0      378 2023-06-12 21:41:16.330471 python_frank_energie-5.0.0/python_frank_energie/exceptions.py
--rw-r--r--   0        0        0     9007 2023-06-12 21:41:16.330471 python_frank_energie-5.0.0/python_frank_energie/frank_energie.py
--rw-r--r--   0        0        0    11198 2023-06-12 21:41:16.330471 python_frank_energie-5.0.0/python_frank_energie/models.py
--rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 python_frank_energie-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-24 19:15:53.318544 python_frank_energie-5.0.1/LICENSE
+-rw-r--r--   0        0        0     1442 2023-07-24 19:15:53.318544 python_frank_energie-5.0.1/README.md
+-rw-r--r--   0        0        0     2352 2023-07-24 19:16:21.779750 python_frank_energie-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-24 19:15:53.318544 python_frank_energie-5.0.1/python_frank_energie/__init__.py
+-rw-r--r--   0        0        0      378 2023-07-24 19:15:53.318544 python_frank_energie-5.0.1/python_frank_energie/exceptions.py
+-rw-r--r--   0        0        0     9007 2023-07-24 19:15:53.318544 python_frank_energie-5.0.1/python_frank_energie/frank_energie.py
+-rw-r--r--   0        0        0    11198 2023-07-24 19:15:53.318544 python_frank_energie-5.0.1/python_frank_energie/models.py
+-rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 python_frank_energie-5.0.1/PKG-INFO
```

### Comparing `python_frank_energie-5.0.0/LICENSE` & `python_frank_energie-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_frank_energie-5.0.0/README.md` & `python_frank_energie-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python_frank_energie-5.0.0/pyproject.toml` & `python_frank_energie-5.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-frank-energie"
-version = "5.0.0"
+version = "5.0.1"
 description = "Asynchronous Python client for the Frank Energie"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-frank-energie"
 repository = "https://github.com/dcsbl/python-frank-energie"
@@ -19,38 +19,38 @@
 python = "^3.10"
 aiohttp = ">=3.8.0"
 python-dateutil = ">=2.8.0"
 
 [tool.poetry.dev-dependencies]
 aresponses = "^2.1.6"
 black = "^22.12"
-blacken-docs = "^1.13.0"
+blacken-docs = "^1.15.0"
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.5.0"
 isort = "^5.11.4"
 pre-commit = "^3.3.2"
 pre-commit-hooks = "^4.4.0"
 pylint = "^2.17.4"
-pytest = "^7.2.1"
+pytest = "^7.4.0"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.1.0"
 yamllint = "^1.29.0"
-pyupgrade = "^3.6.0"
+pyupgrade = "^3.9.0"
 flake8-simplify = "^0.20.0"
 vulture = "^2.7"
 flake8-bandit = "^3.0.0"
 flake8-bugbear = "^23.3.12"
 flake8-builtins = "^2.1.0"
-flake8-comprehensions = "^3.10.0"
+flake8-comprehensions = "^3.14.0"
 flake8-eradicate = "^1.2.1"
 flake8-markdown = "^0.3.0"
 freezegun = "^1.2.2"
 darglint = "^1.8.1"
 safety = "^2.3.5"
-codespell = "^2.2.2"
+codespell = "^2.2.5"
 bandit = "^1.7.3"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/dcsbl/python-frank-energie/issues"
 Changelog = "https://github.com/dcsbl/python-frank-energie/releases"
 
 [tool.black]
```

### Comparing `python_frank_energie-5.0.0/python_frank_energie/frank_energie.py` & `python_frank_energie-5.0.1/python_frank_energie/frank_energie.py`

 * *Files identical despite different names*

### Comparing `python_frank_energie-5.0.0/python_frank_energie/models.py` & `python_frank_energie-5.0.1/python_frank_energie/models.py`

 * *Files identical despite different names*

### Comparing `python_frank_energie-5.0.0/PKG-INFO` & `python_frank_energie-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-frank-energie
-Version: 5.0.0
+Version: 5.0.1
 Summary: Asynchronous Python client for the Frank Energie
 Home-page: https://github.com/dcsbl/python-frank-energie
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

