# Comparing `tmp/geomancy-0.6.1b0.tar.gz` & `tmp/geomancy-0.6.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-0.6.1b0.tar", last modified: Sun Jul 23 20:59:48 2023, max compression
+gzip compressed data, was "geomancy-0.6.2b0.tar", last modified: Sun Jul 23 22:09:53 2023, max compression
```

## Comparing `geomancy-0.6.1b0.tar` & `geomancy-0.6.2b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.619172 geomancy-0.6.1b0/
--rw-r--r--   0 jlorieau   (501) staff       (20)      256 2023-07-20 19:04:04.000000 geomancy-0.6.1b0/.editorconfig
--rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-20 09:53:51.000000 geomancy-0.6.1b0/.gitignore
--rw-r--r--   0 jlorieau   (501) staff       (20)    35142 2023-07-19 19:00:29.000000 geomancy-0.6.1b0/LICENSE.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     6229 2023-07-23 20:59:48.618455 geomancy-0.6.1b0/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     5883 2023-07-23 20:38:21.000000 geomancy-0.6.1b0/README.md
--rw-r--r--   0 jlorieau   (501) staff       (20)      587 2023-07-20 19:50:56.000000 geomancy-0.6.1b0/Taskfile.yml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.600286 geomancy-0.6.1b0/examples/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1273 2023-07-23 19:48:55.000000 geomancy-0.6.1b0/examples/geomancy.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.6.1b0/examples/pyproject.toml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.601660 geomancy-0.6.1b0/geomancy/
--rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.6.1b0/geomancy/__description__.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      477 2023-07-23 20:58:09.000000 geomancy-0.6.1b0/geomancy/__init__.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.609605 geomancy-0.6.1b0/geomancy/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)      257 2023-07-23 18:46:46.000000 geomancy-0.6.1b0/geomancy/checks/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    11237 2023-07-23 18:44:11.000000 geomancy-0.6.1b0/geomancy/checks/base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-23 16:57:03.000000 geomancy-0.6.1b0/geomancy/checks/env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2812 2023-07-23 19:41:18.000000 geomancy-0.6.1b0/geomancy/checks/exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.6.1b0/geomancy/checks/path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      184 2023-07-23 20:24:18.000000 geomancy-0.6.1b0/geomancy/checks/python.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     3542 2023-07-23 19:33:47.000000 geomancy-0.6.1b0/geomancy/checks/utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.610817 geomancy-0.6.1b0/geomancy/cli/
--rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.6.1b0/geomancy/cli/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.6.1b0/geomancy/cli/term.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.612210 geomancy-0.6.1b0/geomancy/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.6.1b0/geomancy/config/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9726 2023-07-22 15:36:57.000000 geomancy-0.6.1b0/geomancy/config/config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     5046 2023-07-23 20:54:10.000000 geomancy-0.6.1b0/geomancy/main.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.605488 geomancy-0.6.1b0/geomancy.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6229 2023-07-23 20:59:48.000000 geomancy-0.6.1b0/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)      858 2023-07-23 20:59:48.000000 geomancy-0.6.1b0/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-23 20:59:48.000000 geomancy-0.6.1b0/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-23 20:59:48.000000 geomancy-0.6.1b0/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       45 2023-07-23 20:59:48.000000 geomancy-0.6.1b0/geomancy.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-23 20:59:48.000000 geomancy-0.6.1b0/geomancy.egg-info/top_level.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      702 2023-07-23 20:59:37.000000 geomancy-0.6.1b0/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-23 20:59:48.619388 geomancy-0.6.1b0/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.612847 geomancy-0.6.1b0/tests/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.615893 geomancy-0.6.1b0/tests/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)     2968 2023-07-22 17:33:51.000000 geomancy-0.6.1b0/tests/checks/test_base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.6.1b0/tests/checks/test_env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1171 2023-07-23 19:38:14.000000 geomancy-0.6.1b0/tests/checks/test_exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.6.1b0/tests/checks/test_path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.6.1b0/tests/checks/test_utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 20:59:48.617106 geomancy-0.6.1b0/tests/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.6.1b0/tests/config/config1.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.6.1b0/tests/config/test_config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1647 2023-07-22 16:20:11.000000 geomancy-0.6.1b0/tests/test_main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.851487 geomancy-0.6.2b0/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      256 2023-07-20 19:04:04.000000 geomancy-0.6.2b0/.editorconfig
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-20 09:53:51.000000 geomancy-0.6.2b0/.gitignore
+-rw-r--r--   0 jlorieau   (501) staff       (20)    35142 2023-07-19 19:00:29.000000 geomancy-0.6.2b0/LICENSE.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6613 2023-07-23 22:09:53.850958 geomancy-0.6.2b0/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6216 2023-07-23 22:08:52.000000 geomancy-0.6.2b0/README.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)      587 2023-07-20 19:50:56.000000 geomancy-0.6.2b0/Taskfile.yml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.826649 geomancy-0.6.2b0/examples/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1273 2023-07-23 19:48:55.000000 geomancy-0.6.2b0/examples/geomancy.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.6.2b0/examples/pyproject.toml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.828225 geomancy-0.6.2b0/geomancy/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.6.2b0/geomancy/__description__.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      477 2023-07-23 22:09:21.000000 geomancy-0.6.2b0/geomancy/__init__.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.836951 geomancy-0.6.2b0/geomancy/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      257 2023-07-23 18:46:46.000000 geomancy-0.6.2b0/geomancy/checks/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    11237 2023-07-23 18:44:11.000000 geomancy-0.6.2b0/geomancy/checks/base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-23 16:57:03.000000 geomancy-0.6.2b0/geomancy/checks/env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2812 2023-07-23 19:41:18.000000 geomancy-0.6.2b0/geomancy/checks/exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.6.2b0/geomancy/checks/path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      184 2023-07-23 20:24:18.000000 geomancy-0.6.2b0/geomancy/checks/python.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     3542 2023-07-23 19:33:47.000000 geomancy-0.6.2b0/geomancy/checks/utils.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.838674 geomancy-0.6.2b0/geomancy/cli/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.6.2b0/geomancy/cli/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.6.2b0/geomancy/cli/term.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.840056 geomancy-0.6.2b0/geomancy/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.6.2b0/geomancy/config/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9726 2023-07-22 15:36:57.000000 geomancy-0.6.2b0/geomancy/config/config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5046 2023-07-23 20:54:10.000000 geomancy-0.6.2b0/geomancy/main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.831724 geomancy-0.6.2b0/geomancy.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6613 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)      858 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       45 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-23 22:09:53.000000 geomancy-0.6.2b0/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      748 2023-07-23 22:03:01.000000 geomancy-0.6.2b0/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-23 22:09:53.851612 geomancy-0.6.2b0/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.840808 geomancy-0.6.2b0/tests/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.847025 geomancy-0.6.2b0/tests/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2968 2023-07-22 17:33:51.000000 geomancy-0.6.2b0/tests/checks/test_base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.6.2b0/tests/checks/test_env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1171 2023-07-23 19:38:14.000000 geomancy-0.6.2b0/tests/checks/test_exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.6.2b0/tests/checks/test_path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.6.2b0/tests/checks/test_utils.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-23 22:09:53.849583 geomancy-0.6.2b0/tests/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.6.2b0/tests/config/config1.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.6.2b0/tests/config/test_config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1647 2023-07-22 16:20:11.000000 geomancy-0.6.2b0/tests/test_main.py
```

### Comparing `geomancy-0.6.1b0/.gitignore` & `geomancy-0.6.2b0/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/LICENSE.md` & `geomancy-0.6.2b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/PKG-INFO` & `geomancy-0.6.2b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.6.1b0
+Version: 0.6.2b0
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # geomancy
 
+[![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
+[![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
+[![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
 Currently, ``geomancy`` can check that:
 - [environment variables](#checkenv) are properly set
 - [file and directory paths](#checkpath) exist
 - [executables](#checkexec) are available and, optionally, of the correct version
@@ -46,15 +51,15 @@
 1. Create a file containing checks. Either
 
    - ``.geomancy.toml`` in the project root. See the ``examples`` directory for
      examples.
 
    or
 
-   - ``pyproject.toml`` with check in the ``[tool.geomancy]`` section.
+   - ``pyproject.toml`` with checks and config in the ``[tool.geomancy]`` section.
 
 2. Run the geo
 
    ```shell
    $ geo
    ```
 
@@ -147,15 +152,15 @@
 
 #### checkPath
 
 Check the existence and type of a path.
 
 | name      | description                                                                                                                                    |
 |:----------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
-| checkPath | Path to check, which may include environment varaibles wrapped in curly braces for substitution. <br>__aliases__: ``checkPath``, ``CheckPath`` |
+| checkPath | Path to check, which may include environment variables wrapped in curly braces for substitution. <br>__aliases__: ``checkPath``, ``CheckPath`` |
 | desc      | _(Optional)_ The description for the check                                                                                                     |
 | type      | _(Optional)_ Additionally check whether the path corresponds to a valid ``'file'`` or ``'dir'``.                                               |
 
 ##### Examples
 
 ```toml
 [checks.Environment.Pyproject]
```

### Comparing `geomancy-0.6.1b0/README.md` & `geomancy-0.6.2b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # geomancy
 
+[![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
+[![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
+[![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
 Currently, ``geomancy`` can check that:
 - [environment variables](#checkenv) are properly set
 - [file and directory paths](#checkpath) exist
 - [executables](#checkexec) are available and, optionally, of the correct version
@@ -34,15 +38,15 @@
 1. Create a file containing checks. Either
 
    - ``.geomancy.toml`` in the project root. See the ``examples`` directory for
      examples.
 
    or
 
-   - ``pyproject.toml`` with check in the ``[tool.geomancy]`` section.
+   - ``pyproject.toml`` with checks and config in the ``[tool.geomancy]`` section.
 
 2. Run the geo
 
    ```shell
    $ geo
    ```
 
@@ -135,15 +139,15 @@
 
 #### checkPath
 
 Check the existence and type of a path.
 
 | name      | description                                                                                                                                    |
 |:----------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
-| checkPath | Path to check, which may include environment varaibles wrapped in curly braces for substitution. <br>__aliases__: ``checkPath``, ``CheckPath`` |
+| checkPath | Path to check, which may include environment variables wrapped in curly braces for substitution. <br>__aliases__: ``checkPath``, ``CheckPath`` |
 | desc      | _(Optional)_ The description for the check                                                                                                     |
 | type      | _(Optional)_ Additionally check whether the path corresponds to a valid ``'file'`` or ``'dir'``.                                               |
 
 ##### Examples
 
 ```toml
 [checks.Environment.Pyproject]
```

### Comparing `geomancy-0.6.1b0/Taskfile.yml` & `geomancy-0.6.2b0/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/examples/geomancy.toml` & `geomancy-0.6.2b0/examples/geomancy.toml`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/examples/pyproject.toml` & `geomancy-0.6.2b0/examples/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy/checks/base.py` & `geomancy-0.6.2b0/geomancy/checks/base.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy/checks/env.py` & `geomancy-0.6.2b0/geomancy/checks/env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy/checks/exec.py` & `geomancy-0.6.2b0/geomancy/checks/exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy/checks/path.py` & `geomancy-0.6.2b0/geomancy/checks/path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy/checks/utils.py` & `geomancy-0.6.2b0/geomancy/checks/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy/cli/term.py` & `geomancy-0.6.2b0/geomancy/cli/term.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy/config/config.py` & `geomancy-0.6.2b0/geomancy/config/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy/main.py` & `geomancy-0.6.2b0/geomancy/main.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/geomancy.egg-info/PKG-INFO` & `geomancy-0.6.2b0/geomancy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.6.1b0
+Version: 0.6.2b0
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # geomancy
 
+[![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
+[![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
+[![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
 Currently, ``geomancy`` can check that:
 - [environment variables](#checkenv) are properly set
 - [file and directory paths](#checkpath) exist
 - [executables](#checkexec) are available and, optionally, of the correct version
@@ -46,15 +51,15 @@
 1. Create a file containing checks. Either
 
    - ``.geomancy.toml`` in the project root. See the ``examples`` directory for
      examples.
 
    or
 
-   - ``pyproject.toml`` with check in the ``[tool.geomancy]`` section.
+   - ``pyproject.toml`` with checks and config in the ``[tool.geomancy]`` section.
 
 2. Run the geo
 
    ```shell
    $ geo
    ```
 
@@ -147,15 +152,15 @@
 
 #### checkPath
 
 Check the existence and type of a path.
 
 | name      | description                                                                                                                                    |
 |:----------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
-| checkPath | Path to check, which may include environment varaibles wrapped in curly braces for substitution. <br>__aliases__: ``checkPath``, ``CheckPath`` |
+| checkPath | Path to check, which may include environment variables wrapped in curly braces for substitution. <br>__aliases__: ``checkPath``, ``CheckPath`` |
 | desc      | _(Optional)_ The description for the check                                                                                                     |
 | type      | _(Optional)_ Additionally check whether the path corresponds to a valid ``'file'`` or ``'dir'``.                                               |
 
 ##### Examples
 
 ```toml
 [checks.Environment.Pyproject]
```

### Comparing `geomancy-0.6.1b0/geomancy.egg-info/SOURCES.txt` & `geomancy-0.6.2b0/geomancy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/pyproject.toml` & `geomancy-0.6.2b0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 authors = [
     {name = "Justin Lorieau"},
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta"
     ]
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.4",
```

### Comparing `geomancy-0.6.1b0/tests/checks/test_base.py` & `geomancy-0.6.2b0/tests/checks/test_base.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/tests/checks/test_env.py` & `geomancy-0.6.2b0/tests/checks/test_env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/tests/checks/test_exec.py` & `geomancy-0.6.2b0/tests/checks/test_exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/tests/checks/test_path.py` & `geomancy-0.6.2b0/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/tests/checks/test_utils.py` & `geomancy-0.6.2b0/tests/checks/test_utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/tests/config/test_config.py` & `geomancy-0.6.2b0/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.1b0/tests/test_main.py` & `geomancy-0.6.2b0/tests/test_main.py`

 * *Files identical despite different names*

