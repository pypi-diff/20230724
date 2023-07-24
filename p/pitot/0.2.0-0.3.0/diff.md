# Comparing `tmp/pitot-0.2.0.tar.gz` & `tmp/pitot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitot-0.2.0.tar", max compression
+gzip compressed data, was "pitot-0.3.0.tar", max compression
```

## Comparing `pitot-0.2.0.tar` & `pitot-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0     1080 2022-09-06 22:05:35.357318 pitot-0.2.0/license.txt
--rw-r--r--   0        0        0     2031 2022-09-06 22:05:35.357318 pitot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3448 2022-09-06 22:05:35.357318 pitot-0.2.0/readme.md
--rw-r--r--   0        0        0      403 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/__init__.py
--rw-r--r--   0        0        0     3277 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/aero.py
--rw-r--r--   0        0        0     1305 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/aero.pyi
--rw-r--r--   0        0        0     2791 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/geodesy.py
--rw-r--r--   0        0        0     1453 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/geodesy.pyi
--rw-r--r--   0        0        0     3236 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/isa.py
--rw-r--r--   0        0        0     1044 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/isa.pyi
--rw-r--r--   0        0        0        0 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/py.typed
--rw-r--r--   0        0        0      429 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/types.py
--rw-r--r--   0        0        0     1784 2022-09-06 22:05:35.357318 pitot-0.2.0/src/pitot/wrapper.py
--rw-r--r--   0        0        0     4389 2022-09-06 22:05:50.995591 pitot-0.2.0/setup.py
--rw-r--r--   0        0        0     4564 2022-09-06 22:05:50.996045 pitot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-24 13:23:13.766199 pitot-0.3.0/license.txt
+-rw-r--r--   0        0        0     2453 2023-07-24 13:23:13.770199 pitot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1998 2023-07-24 13:23:13.770199 pitot-0.3.0/readme.md
+-rw-r--r--   0        0        0      410 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/__init__.py
+-rw-r--r--   0        0        0     3537 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/aero.py
+-rw-r--r--   0        0        0      885 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/airac.py
+-rw-r--r--   0        0        0     3610 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/geodesy.py
+-rw-r--r--   0        0        0     2604 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/geodesy.pyi
+-rw-r--r--   0        0        0     4314 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/isa.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/py.typed
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 pitot-0.3.0/PKG-INFO
```

### Comparing `pitot-0.2.0/license.txt` & `pitot-0.3.0/license.txt`

 * *Files identical despite different names*

### Comparing `pitot-0.2.0/pyproject.toml` & `pitot-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pitot"
-version = "0.2.0"
+version = "0.3.0"
 description = "Toolbox for aeronautic units and conversions"
 authors = ["Xavier Olive <git@xoolive.org>", "Junzi Sun <junzisun@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Information Technology",
@@ -23,29 +23,29 @@
 include = [
   "license.txt",
   "py.typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-numpy = "^1.23.0"
-pandas = "^1.4.3"
-Pint = "^0.19.2"
-Pint-Pandas = "^0.2"
-typing-extensions = "^4.3.0"
-pyproj = "^3.3.1"
-
-[tool.poetry.dev-dependencies]
-mypy = "^0.961"
-isort = "^5.10.1"
-black = "^22.6.0"
-flake8 = "^4.0.1"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-pre-commit = "^2.20.0"
+numpy = ">=1.23.0"
+pandas = ">=1.4.3"
+typing-extensions = ">=4.3.0"
+pyproj = ">=3.3.1"
+impunity = ">=1.0.2"
+# impunity = { path = "../impunity", develop = true }
+
+[tool.poetry.group.dev.dependencies]
+mypy = ">=0.991"
+isort = ">=5.10.1"
+black = ">=22.12.0"
+pytest = ">=7.1.2"
+pytest-cov = ">=4.0.0"
+pre-commit = ">=2.20.0"
+ruff = "^0.0.253"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 80
@@ -58,18 +58,32 @@
   | \.mypy_cache
   | \.ipynb_checkpoints
   | build
   | dist
 )/
 '''
 
-[tool.isort]
-line_length = 80
-profile = "black"
-skip = ["*.pyi"]
+[tool.ruff]
+select = [
+  "E", "W",  # pycodestyle
+  "F",  # pyflakes
+  "I",  # isort
+  "NPY",  # numpy
+  # "PD",  # pandas
+  "DTZ", # flake8-datetimez
+  "RUF"
+]
+line-length = 80
+target-version = "py38"
+
+[tool.ruff.isort]
+known-first-party = ["numpy", "pandas", "pyproj", "shapely"]
+
+# [tool.isort]
+# skip = ["*.pyi"]
 
 [tool.mypy]
 python_version = 3.8
 platform = "posix"
 
 color_output = true
 pretty = true
@@ -81,12 +95,13 @@
 ignore_missing_imports = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.pytest.ini_options]
-addopts = "--log-level=DEBUG --color=yes"
+addopts = "--log-level=INFO --color=yes --doctest-modules --doctest-report ndiff"
 filterwarnings = [
   "ignore:.*unit of the quantity is strip.*:"
 ]
-testpaths = ["tests"]
+testpaths = ["tests", "src"]
+doctest_optionflags = ["NORMALIZE_WHITESPACE", "ELLIPSIS", "NUMBER"]
```

