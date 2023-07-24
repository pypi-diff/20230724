# Comparing `tmp/geomancy-0.6.2b0.tar.gz` & `tmp/geomancy-0.6.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-0.6.2b0.tar", last modified: Sun Jul 23 22:09:53 2023, max compression
+gzip compressed data, was "geomancy-0.6.3b0.tar", last modified: Mon Jul 24 15:16:26 2023, max compression
```

## Comparing `geomancy-0.6.2b0.tar` & `geomancy-0.6.3b0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.851487 geomancy-0.6.2b0/
--rw-r--r--   0 jlorieau   (501) staff       (20)      256 2023-07-20 19:04:04.000000 geomancy-0.6.2b0/.editorconfig
--rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-20 09:53:51.000000 geomancy-0.6.2b0/.gitignore
--rw-r--r--   0 jlorieau   (501) staff       (20)    35142 2023-07-19 19:00:29.000000 geomancy-0.6.2b0/LICENSE.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     6613 2023-07-23 22:09:53.850958 geomancy-0.6.2b0/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     6216 2023-07-23 22:08:52.000000 geomancy-0.6.2b0/README.md
--rw-r--r--   0 jlorieau   (501) staff       (20)      587 2023-07-20 19:50:56.000000 geomancy-0.6.2b0/Taskfile.yml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.826649 geomancy-0.6.2b0/examples/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1273 2023-07-23 19:48:55.000000 geomancy-0.6.2b0/examples/geomancy.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.6.2b0/examples/pyproject.toml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.828225 geomancy-0.6.2b0/geomancy/
--rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.6.2b0/geomancy/__description__.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      477 2023-07-23 22:09:21.000000 geomancy-0.6.2b0/geomancy/__init__.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.836951 geomancy-0.6.2b0/geomancy/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)      257 2023-07-23 18:46:46.000000 geomancy-0.6.2b0/geomancy/checks/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    11237 2023-07-23 18:44:11.000000 geomancy-0.6.2b0/geomancy/checks/base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-23 16:57:03.000000 geomancy-0.6.2b0/geomancy/checks/env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2812 2023-07-23 19:41:18.000000 geomancy-0.6.2b0/geomancy/checks/exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.6.2b0/geomancy/checks/path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      184 2023-07-23 20:24:18.000000 geomancy-0.6.2b0/geomancy/checks/python.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     3542 2023-07-23 19:33:47.000000 geomancy-0.6.2b0/geomancy/checks/utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.838674 geomancy-0.6.2b0/geomancy/cli/
--rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.6.2b0/geomancy/cli/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.6.2b0/geomancy/cli/term.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.840056 geomancy-0.6.2b0/geomancy/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.6.2b0/geomancy/config/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9726 2023-07-22 15:36:57.000000 geomancy-0.6.2b0/geomancy/config/config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     5046 2023-07-23 20:54:10.000000 geomancy-0.6.2b0/geomancy/main.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.831724 geomancy-0.6.2b0/geomancy.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6613 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)      858 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       45 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/top_level.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      748 2023-07-23 22:03:01.000000 geomancy-0.6.2b0/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-23 22:09:53.851612 geomancy-0.6.2b0/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.840808 geomancy-0.6.2b0/tests/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.847025 geomancy-0.6.2b0/tests/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)     2968 2023-07-22 17:33:51.000000 geomancy-0.6.2b0/tests/checks/test_base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.6.2b0/tests/checks/test_env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1171 2023-07-23 19:38:14.000000 geomancy-0.6.2b0/tests/checks/test_exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.6.2b0/tests/checks/test_path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.6.2b0/tests/checks/test_utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.849583 geomancy-0.6.2b0/tests/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.6.2b0/tests/config/config1.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.6.2b0/tests/config/test_config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1647 2023-07-22 16:20:11.000000 geomancy-0.6.2b0/tests/test_main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.720303 geomancy-0.6.3b0/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      256 2023-07-20 19:04:04.000000 geomancy-0.6.3b0/.editorconfig
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-20 09:53:51.000000 geomancy-0.6.3b0/.gitignore
+-rw-r--r--   0 jlorieau   (501) staff       (20)    35142 2023-07-19 19:00:29.000000 geomancy-0.6.3b0/LICENSE.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6721 2023-07-24 15:16:26.719597 geomancy-0.6.3b0/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6324 2023-07-24 15:11:27.000000 geomancy-0.6.3b0/README.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)      587 2023-07-20 19:50:56.000000 geomancy-0.6.3b0/Taskfile.yml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.695136 geomancy-0.6.3b0/assets/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1340 2023-07-24 14:40:21.000000 geomancy-0.6.3b0/assets/geomancy.svg
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1525 2023-07-24 14:52:00.000000 geomancy-0.6.3b0/assets/geomancy_logo.svg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.696334 geomancy-0.6.3b0/examples/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1273 2023-07-23 19:48:55.000000 geomancy-0.6.3b0/examples/geomancy.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.6.3b0/examples/pyproject.toml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.697878 geomancy-0.6.3b0/geomancy/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.6.3b0/geomancy/__description__.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      477 2023-07-24 15:12:23.000000 geomancy-0.6.3b0/geomancy/__init__.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.706363 geomancy-0.6.3b0/geomancy/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-24 12:18:52.000000 geomancy-0.6.3b0/geomancy/checks/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    13168 2023-07-24 01:16:25.000000 geomancy-0.6.3b0/geomancy/checks/base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-23 16:57:03.000000 geomancy-0.6.3b0/geomancy/checks/env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2206 2023-07-24 01:29:48.000000 geomancy-0.6.3b0/geomancy/checks/exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.6.3b0/geomancy/checks/path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4180 2023-07-24 01:10:18.000000 geomancy-0.6.3b0/geomancy/checks/utils.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.709133 geomancy-0.6.3b0/geomancy/cli/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.6.3b0/geomancy/cli/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.6.3b0/geomancy/cli/term.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.711183 geomancy-0.6.3b0/geomancy/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.6.3b0/geomancy/config/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9726 2023-07-22 15:36:57.000000 geomancy-0.6.3b0/geomancy/config/config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5046 2023-07-23 20:54:10.000000 geomancy-0.6.3b0/geomancy/main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.700497 geomancy-0.6.3b0/geomancy.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6721 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)      877 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       45 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      791 2023-07-24 15:16:01.000000 geomancy-0.6.3b0/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-24 15:16:26.720494 geomancy-0.6.3b0/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.712195 geomancy-0.6.3b0/tests/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.716483 geomancy-0.6.3b0/tests/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2968 2023-07-22 17:33:51.000000 geomancy-0.6.3b0/tests/checks/test_base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.6.3b0/tests/checks/test_env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1171 2023-07-23 19:38:14.000000 geomancy-0.6.3b0/tests/checks/test_exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.6.3b0/tests/checks/test_path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.6.3b0/tests/checks/test_utils.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.718207 geomancy-0.6.3b0/tests/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.6.3b0/tests/config/config1.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.6.3b0/tests/config/test_config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1647 2023-07-22 16:20:11.000000 geomancy-0.6.3b0/tests/test_main.py
```

### Comparing `geomancy-0.6.2b0/.gitignore` & `geomancy-0.6.3b0/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/LICENSE.md` & `geomancy-0.6.3b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/PKG-INFO` & `geomancy-0.6.3b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.6.2b0
+Version: 0.6.3b0
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
-# geomancy
+<img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/assets/geomancy_logo.svg" alt="geomancy" height="120" />
 
 [![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
-Currently, ``geomancy`` can check that:
+Currently, ``geomancy`` can check:
 - [environment variables](#checkenv) are properly set
 - [file and directory paths](#checkpath) exist
 - [executables](#checkexec) are available and, optionally, of the correct version
-- [check grouping](#check-groups) and conditional evaluation
-- supports setting values with environment variable substitution.
+- [groups of checks](#check-groups) with conditional evaluation
+- parameter values with substitution of environment variables.
   ex: ``checkPath: {HOME}/.geomancy.toml``
 
 The following is an example ``geomancy`` run with an example checks file.
 
 ```shell
 $ geo examples/geomancy.toml
 ========================= examples/geomancy.toml =========================
```

### Comparing `geomancy-0.6.2b0/README.md` & `geomancy-0.6.3b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# geomancy
+<img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/assets/geomancy_logo.svg" alt="geomancy" height="120" />
 
 [![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
-Currently, ``geomancy`` can check that:
+Currently, ``geomancy`` can check:
 - [environment variables](#checkenv) are properly set
 - [file and directory paths](#checkpath) exist
 - [executables](#checkexec) are available and, optionally, of the correct version
-- [check grouping](#check-groups) and conditional evaluation
-- supports setting values with environment variable substitution.
+- [groups of checks](#check-groups) with conditional evaluation
+- parameter values with substitution of environment variables.
   ex: ``checkPath: {HOME}/.geomancy.toml``
 
 The following is an example ``geomancy`` run with an example checks file.
 
 ```shell
 $ geo examples/geomancy.toml
 ========================= examples/geomancy.toml =========================
```

### Comparing `geomancy-0.6.2b0/Taskfile.yml` & `geomancy-0.6.3b0/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/examples/geomancy.toml` & `geomancy-0.6.3b0/examples/geomancy.toml`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/examples/pyproject.toml` & `geomancy-0.6.3b0/examples/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/geomancy/checks/base.py` & `geomancy-0.6.3b0/geomancy/checks/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 Abstract base class for checks
 """
 import typing as t
+from abc import ABC, abstractmethod
+from inspect import isabstract
 from collections import namedtuple
 from time import process_time
 
-from .utils import sub_env
+from .utils import sub_env, name_and_version, all_subclasses
 from ..config import Parameter
 from ..cli import Term
 
-__all__ = ("CheckBase", "CheckException", "CheckResult")
+__all__ = ("CheckBase", "CheckVersion", "CheckException", "CheckResult")
 
 
 class CheckException(Exception):
     """Exception raised when an error is encountered in the setup of a check."""
 
 
 # Storage class for the results of checks
 CheckResult = namedtuple("CheckResult", "passed msg status", defaults=("", ""))
 
 
-class CheckBase:
+class CheckBase(ABC):
     """Check base class and grouper"""
 
     # Unprocessed value for the check
     raw_value: str
 
     # Description of the check
     desc: str = ""
@@ -232,34 +234,38 @@
         sub checks."""
         flattened = [self]
         for sub_check in self.sub_checks:
             flattened += sub_check.flatten()
         return flattened
 
     @classmethod
-    def types_dict(cls) -> t.Dict[str, type]:
+    def types_dict(cls) -> t.Dict[str, t.Type]:
         """Return all the types and subtypes of Checks in a dict."""
         # Retrieve the base class (BaseCheck) and subclasses
-        cls_types = [cls] + cls.__subclasses__()
+        cls_types = [cls] + list(all_subclasses(cls))
 
         # Create a dict with the class name string (key) and the class type
         # (value)
         d = dict()
         for cls_type in cls_types:
+            # Skip abstract classes, which can't be instantiated
+            if isabstract(cls_type):
+                continue
+
             # Add the class name directly
             d[cls_type.__name__] = cls_type
 
             # Add class name aliases
             aliases = cls_type.aliases if cls_type.aliases is not None else ()
             for alias in aliases:
                 # Aliases should not create name collisions
                 assert alias not in d, f"Duplicate alias name '{alias}'"
 
                 d[alias] = cls_type
-
+        print(d)
         return d
 
     @classmethod
     def load(
         cls, d: dict, name: str, level: int = 1, max_level: t.Optional[int] = None
     ) -> t.Union["CheckBase", None]:
         """Load checks from a dict.
@@ -334,7 +340,58 @@
 
         # No sub-checks found; nothing else to do
         if len(found_checks) == 0:
             return None
 
         # Create a check grouping, first, by parsing the other arguments
         return CheckBase(name=name, sub_checks=found_checks, **other_d)
+
+
+class CheckVersion(CheckBase):
+    """An abstract Check for package and program versions"""
+
+    @property
+    def value(
+        self,
+    ) -> t.Tuple[
+        t.Union[str, None], t.Union[t.Callable, None], t.Union[t.Tuple[int], None]
+    ]:
+        """Get the package name, comparison operator and version tuple."""
+        value = CheckBase.value.fget(self)
+        name, op, version = name_and_version(value)
+        return name, op, version
+
+    @value.setter
+    def value(self, v):
+        CheckBase.value.fset(self, v)
+
+    @abstractmethod
+    def get_current_version(self) -> t.Union[None, t.Tuple[int]]:
+        """Get the current version, or None if it can't be found."""
+        return None
+
+    def check(self, level: int = 0) -> CheckResult:
+        """Check whether the current version is compatible with the version
+        specified in the value."""
+        name, op, version = self.value
+        current_version = self.get_current_version()
+        passed = False
+
+        if name is None:
+            status = "missing"
+        else:
+            if version is not None and current_version is None:
+                status = "present but current version unknown"
+            elif (
+                version is not None
+                and current_version is not None
+                and op is not None
+                and not op(current_version, version)
+            ):
+                status = f"version={'.'.join(map(str, current_version))}"
+            else:
+                status = "passed"
+                passed = True
+
+        return CheckResult(
+            passed=passed, msg=self.msg.format(check=self), status=status
+        )
```

### Comparing `geomancy-0.6.2b0/geomancy/checks/env.py` & `geomancy-0.6.3b0/geomancy/checks/env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/geomancy/checks/exec.py` & `geomancy-0.6.3b0/geomancy/checks/exec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,77 @@
 """
 Checks for executables
 """
 import typing as t
 from shutil import which
-import re
 import subprocess
 
-from .base import CheckBase, CheckResult
-from .utils import name_and_version, version_to_tuple
+from .base import CheckVersion
+from .utils import version_to_tuple
 from ..config import Parameter
 
 __all__ = ("CheckExec",)
 
 
-class CheckExec(CheckBase):
-    """Check for the presence and version of executables
-
-    Notes
-    """
+class CheckExec(CheckVersion):
+    """Check for the presence and version of executables"""
 
     # The message for checking environment variables
     msg = Parameter(
         "CHECKEXEC.MSG",
         default="Check executable '{check.raw_value}'...",
     )
 
     # Alternative names for the class
     aliases = ("checkExec",)
 
     @property
-    def value(self) -> t.Any:
-        """Get the value, with parsing of versions"""
-        value = CheckBase.value.fget(self)
-        return name_and_version(value)
+    def value(
+        self,
+    ) -> t.Tuple[
+        t.Union[str, None], t.Union[t.Callable, None], t.Union[t.Tuple[int], None]
+    ]:
+        """Get the package name, comparison operator and version tuple."""
+        cmd_name, op, version = CheckVersion.value.fget(self)
+
+        # Check to see if the cmd_name exists. Returns None if it doesn't
+        cmd_name = which(cmd_name) if cmd_name is not None else cmd_name
+
+        return cmd_name, op, version
 
     @value.setter
     def value(self, v):
-        CheckBase.value.fset(self, v)
+        CheckVersion.value.fset(self, v)
+
+    def get_current_version(self) -> t.Union[None, t.Tuple[int]]:
+        cmd_name, op, version = self.value
+
+        if cmd_name is None:  # command not found
+            return None
 
-    def check(self, level: int = 0) -> CheckResult:
-        """Check for the executable."""
-        # Setup variables and values
-        name, op, version = self.value
-        current_version = None
-        passed = False
-
-        # See if the executable can be found
-        cmd_path = which(name)
-
-        # See if a version string was specified and whether it can be determined
-        if cmd_path is not None and version is not None:
-            for args in (  # Different commands to try for versions
-                (cmd_path, "-V"),
-                (cmd_path, "--version"),
-            ):
+        for args in (  # Different commands to try for versions
+            (cmd_name, "-V"),
+            (cmd_name, "--version"),
+        ):
+            try:
                 proc = subprocess.run(args, capture_output=True)
-                if proc.returncode != 0:  # Wasn't a success
-                    continue
+            except FileNotFoundError:
+                # Couldn't find the executable
+                continue
+
+            if proc.returncode != 0:  # Wasn't a success
+                continue
+
+            # Try to parse the current version string
+            current_version = version_to_tuple(proc.stdout.decode("UTF-8"))
+            current_version = (
+                current_version
+                if current_version is not None
+                else version_to_tuple(proc.stderr.decode("UTF-8"))
+            )
+
+            if current_version is not None:
+                # Current version found! We're done
+                return current_version
 
-                # Try to parse the current version string
-                current_version = version_to_tuple(proc.stdout.decode("UTF-8"))
-                current_version = (
-                    current_version
-                    if current_version is not None
-                    else version_to_tuple(proc.stderr.decode("UTF-8"))
-                )
-
-                if current_version is not None:
-                    # Current version found! We're done
-                    break
-
-        # Evaluate whether the check passed
-        if cmd_path is None:
-            status = "missing"
-        else:
-            if version is not None and current_version is None:
-                status = "present but current version unknown"
-            elif (
-                version is not None
-                and current_version is not None
-                and op is not None
-                and not op(current_version, version)
-            ):
-                status = f"version={'.'.join(map(str, current_version))}"
-            else:
-                status = "passed"
-                passed = True
-
-        return CheckResult(
-            passed=passed, msg=self.msg.format(check=self), status=status
-        )
+        # Not found
+        return None
```

### Comparing `geomancy-0.6.2b0/geomancy/checks/path.py` & `geomancy-0.6.3b0/geomancy/checks/path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/geomancy/checks/utils.py` & `geomancy-0.6.3b0/geomancy/checks/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,40 @@
 """Utility functions"""
 import typing as t
 import os
 import operator
 import re
 
-__all__ = ("sub_env", "version_to_tuple", "name_and_version")
+__all__ = ("all_subclasses", "sub_env", "version_to_tuple", "name_and_version")
+
+
+def all_subclasses(cls) -> t.List[t.Type]:
+    """Retrieve all subclasses, sub-subclasses and so on for a class
+
+    Parameters
+    ----------
+    cls : Type
+        The class object to inspect for subclasses.
+
+    Returns
+    -------
+    subclasses : list
+        The list of all subclasses.
+
+    Examples
+    --------
+    >>> class A(object): pass
+    >>> class B(A): pass
+    >>> class C(B): pass
+    >>> all_subclasses(A)
+    [<class 'geomancy.checks.utils.B'>, <class 'geomancy.checks.utils.C'>]
+    """
+    return cls.__subclasses__() + [
+        g for s in cls.__subclasses__() for g in all_subclasses(s)
+    ]
 
 
 def sub_env(obj):
     """Substitutes environment variables of the form {VARIABLE_NAME} in
     strings.
     """
     if isinstance(obj, str):
```

### Comparing `geomancy-0.6.2b0/geomancy/cli/term.py` & `geomancy-0.6.3b0/geomancy/cli/term.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/geomancy/config/config.py` & `geomancy-0.6.3b0/geomancy/config/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/geomancy/main.py` & `geomancy-0.6.3b0/geomancy/main.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/geomancy.egg-info/PKG-INFO` & `geomancy-0.6.3b0/geomancy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.6.2b0
+Version: 0.6.3b0
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
-# geomancy
+<img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/assets/geomancy_logo.svg" alt="geomancy" height="120" />
 
 [![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
-Currently, ``geomancy`` can check that:
+Currently, ``geomancy`` can check:
 - [environment variables](#checkenv) are properly set
 - [file and directory paths](#checkpath) exist
 - [executables](#checkexec) are available and, optionally, of the correct version
-- [check grouping](#check-groups) and conditional evaluation
-- supports setting values with environment variable substitution.
+- [groups of checks](#check-groups) with conditional evaluation
+- parameter values with substitution of environment variables.
   ex: ``checkPath: {HOME}/.geomancy.toml``
 
 The following is an example ``geomancy`` run with an example checks file.
 
 ```shell
 $ geo examples/geomancy.toml
 ========================= examples/geomancy.toml =========================
```

### Comparing `geomancy-0.6.2b0/geomancy.egg-info/SOURCES.txt` & `geomancy-0.6.3b0/geomancy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 .editorconfig
 .gitignore
 LICENSE.md
 README.md
 Taskfile.yml
 pyproject.toml
+assets/geomancy.svg
+assets/geomancy_logo.svg
 examples/geomancy.toml
 examples/pyproject.toml
 geomancy/__description__.txt
 geomancy/__init__.py
 geomancy/main.py
 geomancy.egg-info/PKG-INFO
 geomancy.egg-info/SOURCES.txt
@@ -16,15 +18,14 @@
 geomancy.egg-info/requires.txt
 geomancy.egg-info/top_level.txt
 geomancy/checks/__init__.py
 geomancy/checks/base.py
 geomancy/checks/env.py
 geomancy/checks/exec.py
 geomancy/checks/path.py
-geomancy/checks/python.py
 geomancy/checks/utils.py
 geomancy/cli/__init__.py
 geomancy/cli/term.py
 geomancy/config/__init__.py
 geomancy/config/config.py
 tests/test_main.py
 tests/checks/test_base.py
```

### Comparing `geomancy-0.6.2b0/pyproject.toml` & `geomancy-0.6.3b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta"
     ]
 dynamic = ["version", "description"]
 
+[tool.setuptools]
+packages = ["geomancy"]
+
+[tool.setuptools.dynamic]
+version = {attr = "geomancy.__version__"}
+description = {file = "geomancy/__description__.txt"}
+
 [project.optional-dependencies]
 dev = [
     "pytest>=7.4",
     "twine>=4.0",
     "black[d]",
     "build"
     ]
 
-[tool.setuptools.dynamic]
-version = {attr = "geomancy.__version__"}
-description = {file = "geomancy/__description__.txt"}
-
 [project.scripts]
 geo = "geomancy.main:main_cli"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
```

### Comparing `geomancy-0.6.2b0/tests/checks/test_base.py` & `geomancy-0.6.3b0/tests/checks/test_base.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/tests/checks/test_env.py` & `geomancy-0.6.3b0/tests/checks/test_env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/tests/checks/test_exec.py` & `geomancy-0.6.3b0/tests/checks/test_exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/tests/checks/test_path.py` & `geomancy-0.6.3b0/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/tests/checks/test_utils.py` & `geomancy-0.6.3b0/tests/checks/test_utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/tests/config/test_config.py` & `geomancy-0.6.3b0/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.2b0/tests/test_main.py` & `geomancy-0.6.3b0/tests/test_main.py`

 * *Files identical despite different names*

