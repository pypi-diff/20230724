# Comparing `tmp/python_homewizard_energy-2.0.1.tar.gz` & `tmp/python_homewizard_energy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_homewizard_energy-2.0.1.tar", max compression
+gzip compressed data, was "python_homewizard_energy-2.0.2.tar", max compression
```

## Comparing `python_homewizard_energy-2.0.1.tar` & `python_homewizard_energy-2.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11346 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/LICENSE
--rw-r--r--   0        0        0      936 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/README.md
--rw-r--r--   0        0        0      468 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/__init__.py
--rw-r--r--   0        0        0      244 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/const.py
--rw-r--r--   0        0        0      765 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/errors.py
--rw-r--r--   0        0        0     8438 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/homewizard_energy.py
--rw-r--r--   0        0        0    11246 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/models.py
--rw-r--r--   0        0        0        0 2023-04-08 19:06:56.815922 python_homewizard_energy-2.0.1/homewizard_energy/py.typed
--rw-r--r--   0        0        0     2383 2023-04-08 19:08:08.635884 python_homewizard_energy-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.1/setup.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-24 19:17:26.771143 python_homewizard_energy-2.0.2/LICENSE
+-rw-r--r--   0        0        0      936 2023-07-24 19:17:26.771143 python_homewizard_energy-2.0.2/README.md
+-rw-r--r--   0        0        0      468 2023-07-24 19:17:26.771143 python_homewizard_energy-2.0.2/homewizard_energy/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-24 19:17:26.771143 python_homewizard_energy-2.0.2/homewizard_energy/const.py
+-rw-r--r--   0        0        0      765 2023-07-24 19:17:26.771143 python_homewizard_energy-2.0.2/homewizard_energy/errors.py
+-rw-r--r--   0        0        0     8438 2023-07-24 19:17:26.775143 python_homewizard_energy-2.0.2/homewizard_energy/homewizard_energy.py
+-rw-r--r--   0        0        0    11246 2023-07-24 19:17:26.775143 python_homewizard_energy-2.0.2/homewizard_energy/models.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:17:26.775143 python_homewizard_energy-2.0.2/homewizard_energy/py.typed
+-rw-r--r--   0        0        0     2382 2023-07-24 19:17:58.463423 python_homewizard_energy-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 python_homewizard_energy-2.0.2/PKG-INFO
```

### Comparing `python_homewizard_energy-2.0.1/LICENSE` & `python_homewizard_energy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.1/README.md` & `python_homewizard_energy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.1/homewizard_energy/errors.py` & `python_homewizard_energy-2.0.2/homewizard_energy/errors.py`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.1/homewizard_energy/homewizard_energy.py` & `python_homewizard_energy-2.0.2/homewizard_energy/homewizard_energy.py`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.1/homewizard_energy/models.py` & `python_homewizard_energy-2.0.2/homewizard_energy/models.py`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-2.0.1/pyproject.toml` & `python_homewizard_energy-2.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-homewizard-energy"
-version = "2.0.1"
+version = "2.0.2"
 description = "Asynchronous Python client for the HomeWizard Energy"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-homewizard-energy"
 repository = "https://github.com/dcsbl/python-homewizard-energy"
@@ -21,28 +21,28 @@
 awesomeversion = ">=22.9.0"
 
 [tool.poetry.dev-dependencies]
 aresponses = "^2.1.6"
 black = "^22.12"
 blacken-docs = "^1.13.0"
 flake8 = "^4.0.1"
-flake8-docstrings = "^1.5.0"
-isort = "^5.11.4"
-pre-commit = "^3.0.0"
+flake8-docstrings = "^1.7.0"
+isort = "^5.12.0"
+pre-commit = "^3.3.3"
 pre-commit-hooks = "^4.4.0"
-pylint = "^2.15.10"
+pylint = "^2.17.3"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
 yamllint = "^1.29.0"
 pyupgrade = "^3.3.1"
 flake8-simplify = "^0.19.3"
 vulture = "^2.7"
 flake8-bandit = "^3.0.0"
-flake8-bugbear = "^23.1.17"
+flake8-bugbear = "^23.3.12"
 flake8-builtins = "^2.1.0"
 flake8-comprehensions = "^3.10.0"
 flake8-eradicate = "^1.2.1"
 flake8-markdown = "^0.3.0"
 darglint = "^1.8.1"
 safety = "^2.3.5"
 codespell = "^2.2.2"
```

### Comparing `python_homewizard_energy-2.0.1/PKG-INFO` & `python_homewizard_energy-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-homewizard-energy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Asynchronous Python client for the HomeWizard Energy
 Home-page: https://github.com/dcsbl/python-homewizard-energy
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

