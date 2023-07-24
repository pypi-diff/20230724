# Comparing `tmp/invoke-plugin-for-sphinx-1.0.0.tar.gz` & `tmp/invoke-plugin-for-sphinx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoke-plugin-for-sphinx-1.0.0.tar", last modified: Thu Mar 23 12:44:27 2023, max compression
+gzip compressed data, was "invoke-plugin-for-sphinx-1.1.0.tar", last modified: Mon Jul 24 08:19:09 2023, max compression
```

## Comparing `invoke-plugin-for-sphinx-1.0.0.tar` & `invoke-plugin-for-sphinx-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:44:27.015168 invoke-plugin-for-sphinx-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-23 12:43:59.000000 invoke-plugin-for-sphinx-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-23 12:44:27.015168 invoke-plugin-for-sphinx-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-23 12:43:59.000000 invoke-plugin-for-sphinx-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:44:27.011167 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-23 12:43:59.000000 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-23 12:43:59.000000 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:43:59.000000 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:44:27.015168 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-23 12:44:27.000000 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-23 12:44:27.000000 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 12:44:27.000000 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-23 12:44:27.000000 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-23 12:44:27.000000 invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-23 12:43:59.000000 invoke-plugin-for-sphinx-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 12:44:27.015168 invoke-plugin-for-sphinx-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:44:27.015168 invoke-plugin-for-sphinx-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-23 12:43:59.000000 invoke-plugin-for-sphinx-1.0.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:09.615178 invoke-plugin-for-sphinx-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 08:18:40.000000 invoke-plugin-for-sphinx-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-24 08:19:09.611178 invoke-plugin-for-sphinx-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-24 08:18:40.000000 invoke-plugin-for-sphinx-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:09.611178 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 08:18:40.000000 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 08:18:40.000000 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:18:40.000000 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:09.611178 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-24 08:19:09.000000 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 08:19:09.000000 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:19:09.000000 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 08:19:09.000000 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 08:19:09.000000 invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-24 08:18:40.000000 invoke-plugin-for-sphinx-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:19:09.615178 invoke-plugin-for-sphinx-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:19:09.611178 invoke-plugin-for-sphinx-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-24 08:18:40.000000 invoke-plugin-for-sphinx-1.1.0/tests/test_plugin.py
```

### Comparing `invoke-plugin-for-sphinx-1.0.0/LICENSE` & `invoke-plugin-for-sphinx-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invoke-plugin-for-sphinx-1.0.0/README.md` & `invoke-plugin-for-sphinx-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[![REUSE status](https://api.reuse.software/badge/github.com/SAP/invoke-plugin-for-sphinx)](https://api.reuse.software/info/github.com/SAP/invoke-plugin-for-sphinx)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![PyPI version](https://badge.fury.io/py/invoke-plugin-for-sphinx.svg)](https://badge.fury.io/py/invoke-plugin-for-sphinx)
+
 # Invoke Plugin for Sphinx
 This is a plugin which allows the documentation of invoke tasks with sphinx `autodoc`.
 An invoke task looks like a normal function but the `@task` decorator creates a `Task` object behind the scenes.
 Documenting these with `autodoc` can lead to errors or unexpected results.
 
 ## Installation
 `pip install invoke-plugin-for-sphinx`, that's it.
```

### Comparing `invoke-plugin-for-sphinx-1.0.0/invoke_plugin_for_sphinx/_plugin.py` & `invoke-plugin-for-sphinx-1.1.0/invoke_plugin_for_sphinx/_plugin.py`

 * *Files identical despite different names*

### Comparing `invoke-plugin-for-sphinx-1.0.0/pyproject.toml` & `invoke-plugin-for-sphinx-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invoke-plugin-for-sphinx"
-version = "1.0.0"
+version = "1.1.0"
 description = "Sphinx plugin which can render invoke tasks with autodoc"
 authors = [{ name = "Kai Mueller", email = "kai.mueller01@sap.com"}]
 readme = "README.md"
 keywords = ["sphinx", "invoke", "plugin", "inv", "documentation"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Typing :: Typed"
 ]
 requires-python = ">=3.7,<4"
 dependencies = [
-    "sphinx>=4,<7",
+    "sphinx>=4,<8",
     "invoke>=1,<3",
     "importlib_metadata>3; python_version<'3.8'",
 ]
 
 [project.license]
 text = "Apache-2.0"
```

### Comparing `invoke-plugin-for-sphinx-1.0.0/tests/test_plugin.py` & `invoke-plugin-for-sphinx-1.1.0/tests/test_plugin.py`

 * *Files identical despite different names*

