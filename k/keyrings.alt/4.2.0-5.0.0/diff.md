# Comparing `tmp/keyrings.alt-4.2.0.tar.gz` & `tmp/keyrings.alt-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrings.alt-4.2.0.tar", last modified: Mon Sep  5 01:39:28 2022, max compression
+gzip compressed data, was "keyrings.alt-5.0.0.tar", last modified: Mon Jul 24 00:13:06 2023, max compression
```

## Comparing `keyrings.alt-4.2.0.tar` & `keyrings.alt-5.0.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 01:39:28.433189 keyrings.alt-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 01:39:28.417189 keyrings.alt-4.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 01:39:28.417189 keyrings.alt-4.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-09-05 01:39:28.433189 keyrings.alt-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 01:39:28.421189 keyrings.alt-4.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 01:39:28.421189 keyrings.alt-4.2.0/keyrings/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 01:39:28.425189 keyrings.alt-4.2.0/keyrings/alt/
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/Gnome.py
--rw-r--r--   0 runner    (1001) docker     (121)    12421 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/Google.py
--rw-r--r--   0 runner    (1001) docker     (121)     4701 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/Windows.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/_win_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/escape.py
--rw-r--r--   0 runner    (1001) docker     (121)     7705 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/file_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/keyczar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/multi.py
--rw-r--r--   0 runner    (1001) docker     (121)     9030 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/keyrings/alt/pyfs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 01:39:28.421189 keyrings.alt-4.2.0/keyrings.alt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-09-05 01:39:28.000000 keyrings.alt-4.2.0/keyrings.alt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-09-05 01:39:28.000000 keyrings.alt-4.2.0/keyrings.alt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 01:39:28.000000 keyrings.alt-4.2.0/keyrings.alt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-09-05 01:39:28.000000 keyrings.alt-4.2.0/keyrings.alt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-05 01:39:28.000000 keyrings.alt-4.2.0/keyrings.alt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-05 01:39:28.000000 keyrings.alt-4.2.0/keyrings.alt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-09-05 01:39:28.433189 keyrings.alt-4.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 01:39:28.425189 keyrings.alt-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6375 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/test_Gnome.py
--rw-r--r--   0 runner    (1001) docker     (121)    15281 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/test_Google.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/test_Windows.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     7819 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/test_keyczar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3347 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tests/test_pyfs.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-09-05 01:38:48.000000 keyrings.alt-4.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.673857 keyrings.alt-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-24 00:13:06.673857 keyrings.alt-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/keyrings/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/keyrings/alt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/Gnome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/Google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/Windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/_win_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/file_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/keyczar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/keyrings.alt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-24 00:13:06.673857 keyrings.alt-5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.673857 keyrings.alt-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_Gnome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_Google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_Windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_keyczar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tox.ini
```

### Comparing `keyrings.alt-4.2.0/CHANGES.rst` & `keyrings.alt-5.0.0/NEWS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v5.0.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
+Deprecations and Removals
+-------------------------
+
+- Removed the pyfs backend, as it has eroded beyond repair. (#49)
+
+
 v4.2.0
 ======
 
 #46: EncryptedFileKeyring now supports both pycryptodome and
 pycryptodomex (preferring the latter).
 
 v4.1.2
```

### Comparing `keyrings.alt-4.2.0/LICENSE` & `keyrings.alt-5.0.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `keyrings.alt-4.2.0/PKG-INFO` & `keyrings.alt-5.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: keyrings.alt
-Version: 4.2.0
+Version: 5.0.0
 Summary: Alternate keyring implementations
 Home-page: https://github.com/jaraco/keyrings.alt
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/keyrings.alt.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/keyrings.alt
 
 .. image:: https://img.shields.io/pypi/pyversions/keyrings.alt.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/keyrings.alt
 
 .. image:: https://github.com/jaraco/keyrings.alt/workflows/tests/badge.svg
    :target: https://github.com/jaraco/keyrings.alt/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/keyrings.alt
    :target: https://tidelift.com/subscription/pkg/pypi-keyrings.alt?utm_source=pypi-keyrings.alt&utm_medium=readme
 
 Alternate keyring backend implementations for use with the
 `keyring package <https://pypi.python.org/pypi/keyring>`_.
@@ -57,14 +58,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-keyrings.alt?utm_source=pypi-keyrings.alt&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `keyrings.alt-4.2.0/README.rst` & `keyrings.alt-5.0.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .. image:: https://img.shields.io/pypi/v/keyrings.alt.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/keyrings.alt
 
 .. image:: https://img.shields.io/pypi/pyversions/keyrings.alt.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/keyrings.alt
 
 .. image:: https://github.com/jaraco/keyrings.alt/workflows/tests/badge.svg
    :target: https://github.com/jaraco/keyrings.alt/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/keyrings.alt
    :target: https://tidelift.com/subscription/pkg/pypi-keyrings.alt?utm_source=pypi-keyrings.alt&utm_medium=readme
 
 Alternate keyring backend implementations for use with the
 `keyring package <https://pypi.python.org/pypi/keyring>`_.
@@ -40,14 +41,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-keyrings.alt?utm_source=pypi-keyrings.alt&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `keyrings.alt-4.2.0/docs/conf.py` & `keyrings.alt-5.0.0/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
@@ -21,18 +24,25 @@
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
                 url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
 
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
+
 extensions += ['jaraco.tidelift']
+
+intersphinx_mapping.update(
+    keyring=('https://keyring.readthedocs.io/en/latest/', None),
+)
```

### Comparing `keyrings.alt-4.2.0/docs/index.rst` & `keyrings.alt-5.0.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Welcome to |project| documentation!
 ===================================
 
+.. sidebar-links::
+   :home:
+   :pypi:
+
 .. toctree::
    :maxdepth: 1
 
    history
 
 
 .. tidelift-referral-banner::
@@ -30,23 +34,24 @@
     :show-inheritance:
 
 .. automodule:: keyrings.alt.multi
     :members:
     :undoc-members:
     :show-inheritance:
 
-.. automodule:: keyrings.alt.pyfs
+.. automodule:: keyrings.alt.Windows
     :members:
     :undoc-members:
     :show-inheritance:
 
-.. automodule:: keyrings.alt.Windows
+.. automodule:: keyrings.alt.file_base
     :members:
     :undoc-members:
     :show-inheritance:
 
+
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `keyrings.alt-4.2.0/keyrings/alt/Gnome.py` & `keyrings.alt-5.0.0/keyrings/alt/Gnome.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/keyrings/alt/Google.py` & `keyrings.alt-5.0.0/keyrings/alt/Google.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,17 +325,18 @@
     def __init__(self):
         crypter = keyczar.EnvironCrypter()
         credential = EnvironCredential()
         source = os.environ.get('GOOGLE_KEYRING_SOURCE')
         super(KeyczarDocsKeyring, self).__init__(credential, source, crypter)
 
     def supported(self):
-        """Return if this keyring supports current environment:
+        """
+        Return if this keyring supports current environment:
         -1: not applicable
-         0: suitable
-         1: recommended
+        0: suitable
+        1: recommended
         """
         try:
             __import__('keyczar.keyczar')
             return super(KeyczarDocsKeyring, self).supported()
         except ImportError:
             return -1
```

### Comparing `keyrings.alt-4.2.0/keyrings/alt/Windows.py` & `keyrings.alt-5.0.0/keyrings/alt/Windows.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/keyrings/alt/_win_crypto.py` & `keyrings.alt-5.0.0/keyrings/alt/_win_crypto.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/keyrings/alt/escape.py` & `keyrings.alt-5.0.0/keyrings/alt/escape.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/keyrings/alt/file.py` & `keyrings.alt-5.0.0/keyrings/alt/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .escape import escape as escape_for_ini
 from keyrings.alt.file_base import Keyring, decodebytes, encodebytes
 
 
 class PlaintextKeyring(Keyring):
     """Simple File Keyring with no encryption"""
 
-    priority = 0.5
+    priority = 0.5  # type: ignore
     "Applicable for all platforms, but not recommended"
 
     filename = 'keyring_pass.cfg'
     scheme = 'no encyption'
     version = '1.0'
 
     def encrypt(self, password, assoc=None):
```

### Comparing `keyrings.alt-4.2.0/keyrings/alt/file_base.py` & `keyrings.alt-5.0.0/keyrings/alt/file_base.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/keyrings/alt/keyczar.py` & `keyrings.alt-5.0.0/keyrings/alt/keyczar.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/keyrings/alt/multi.py` & `keyrings.alt-5.0.0/keyrings/alt/multi.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/keyrings.alt.egg-info/PKG-INFO` & `keyrings.alt-5.0.0/keyrings.alt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: keyrings.alt
-Version: 4.2.0
+Version: 5.0.0
 Summary: Alternate keyring implementations
 Home-page: https://github.com/jaraco/keyrings.alt
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/keyrings.alt.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/keyrings.alt
 
 .. image:: https://img.shields.io/pypi/pyversions/keyrings.alt.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/keyrings.alt
 
 .. image:: https://github.com/jaraco/keyrings.alt/workflows/tests/badge.svg
    :target: https://github.com/jaraco/keyrings.alt/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/keyrings.alt
    :target: https://tidelift.com/subscription/pkg/pypi-keyrings.alt?utm_source=pypi-keyrings.alt&utm_medium=readme
 
 Alternate keyring backend implementations for use with the
 `keyring package <https://pypi.python.org/pypi/keyring>`_.
@@ -57,14 +58,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-keyrings.alt?utm_source=pypi-keyrings.alt&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `keyrings.alt-4.2.0/setup.cfg` & `keyrings.alt-5.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	jaraco.classes
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
+	pytest-ruff
 	
 	backports.unittest_mock
 	keyring >= 20
 	
-	fs>=0.5,<3
 	pycryptodomex
 	pycryptodome
 	
 	gdata; python_version=="2.7"
 	
 	python-keyczar; python_version=="2.7"
 docs = 
-	sphinx
-	jaraco.packaging >= 9
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
+	
 	jaraco.tidelift >= 1.4
 
 [options.entry_points]
 keyring.backends = 
 	file = keyrings.alt.file
 	Gnome = keyrings.alt.Gnome
 	Google = keyrings.alt.Google
 	keyczar = keyrings.alt.keyczar
 	multi = keyrings.alt.multi
-	pyfs = keyrings.alt.pyfs
 	Windows (alt) = keyrings.alt.Windows
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `keyrings.alt-4.2.0/tests/mocks.py` & `keyrings.alt-5.0.0/tests/mocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         account_type=None,
         service=None,
         auth_service_url=None,
         source=None,
         captcha_token=None,
         captcha_response=None,
     ):
-
         """Client side login to the service."""
         if hasattr(self, '_login_err'):
             raise self._login_err()
 
 
 class MockDocumentService(MockGDataService):
     """
```

### Comparing `keyrings.alt-4.2.0/tests/test_Gnome.py` & `keyrings.alt-5.0.0/tests/test_Gnome.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/tests/test_Google.py` & `keyrings.alt-5.0.0/tests/test_Google.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/tests/test_Windows.py` & `keyrings.alt-5.0.0/tests/test_Windows.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/tests/test_crypto.py` & `keyrings.alt-5.0.0/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/tests/test_file.py` & `keyrings.alt-5.0.0/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/tests/test_keyczar.py` & `keyrings.alt-5.0.0/tests/test_keyczar.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-4.2.0/tests/test_multi.py` & `keyrings.alt-5.0.0/tests/test_multi.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 
 class MultipartKeyringWrapperTestCase(unittest.TestCase):
 
     """Test the wrapper that breaks passwords into smaller chunks"""
 
     class MockKeyring(KeyringBackend):
-
-        priority = 1
+        priority = 1  # type: ignore
 
         def __init__(self):
             self.passwords = {}
 
         def get_password(self, service, username):
             return self.passwords.get(service + username)
```

