# Comparing `tmp/pytch-fetch-1.0.0.tar.gz` & `tmp/pytch-fetch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytch-fetch-1.0.0.tar", last modified: Mon Jul 24 15:27:19 2023, max compression
+gzip compressed data, was "pytch-fetch-1.0.1.tar", last modified: Mon Jul 24 15:35:19 2023, max compression
```

## Comparing `pytch-fetch-1.0.0.tar` & `pytch-fetch-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:27:19.870798 pytch-fetch-1.0.0/
--rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.0.0/LICENSE
--rw-r--r--   0 krit      (1000) krit      (1001)     4099 2023-07-24 15:27:19.869798 pytch-fetch-1.0.0/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)     1658 2023-07-24 15:21:55.000000 pytch-fetch-1.0.0/README.md
--rw-r--r--   0 krit      (1000) krit      (1001)     1298 2023-07-24 15:21:23.000000 pytch-fetch-1.0.0/pyproject.toml
--rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-24 15:27:19.870798 pytch-fetch-1.0.0/setup.cfg
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:27:19.868798 pytch-fetch-1.0.0/src/
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:27:19.868798 pytch-fetch-1.0.0/src/pytch/
--rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.0.0/src/pytch/__init__.py
--rwxr-xr-x   0 krit      (1000) krit      (1001)     2241 2023-07-24 15:22:39.000000 pytch-fetch-1.0.0/src/pytch/__main__.py
--rw-r--r--   0 krit      (1000) krit      (1001)       22 2023-07-24 14:28:41.000000 pytch-fetch-1.0.0/src/pytch/__version__.py
--rw-r--r--   0 krit      (1000) krit      (1001)    19845 2023-07-24 13:46:09.000000 pytch-fetch-1.0.0/src/pytch/art.py
--rw-r--r--   0 krit      (1000) krit      (1001)     4590 2023-07-24 15:17:37.000000 pytch-fetch-1.0.0/src/pytch/funcs.py
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:27:19.868798 pytch-fetch-1.0.0/src/pytch_fetch.egg-info/
--rw-r--r--   0 krit      (1000) krit      (1001)     4099 2023-07-24 15:27:19.000000 pytch-fetch-1.0.0/src/pytch_fetch.egg-info/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)      335 2023-07-24 15:27:19.000000 pytch-fetch-1.0.0/src/pytch_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-24 15:27:19.000000 pytch-fetch-1.0.0/src/pytch_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-24 15:27:19.000000 pytch-fetch-1.0.0/src/pytch_fetch.egg-info/entry_points.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-24 15:27:19.000000 pytch-fetch-1.0.0/src/pytch_fetch.egg-info/top_level.txt
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:35:19.776999 pytch-fetch-1.0.1/
+-rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.0.1/LICENSE
+-rw-r--r--   0 krit      (1000) krit      (1001)     4099 2023-07-24 15:35:19.776999 pytch-fetch-1.0.1/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)     1658 2023-07-24 15:21:55.000000 pytch-fetch-1.0.1/README.md
+-rw-r--r--   0 krit      (1000) krit      (1001)     1298 2023-07-24 15:34:52.000000 pytch-fetch-1.0.1/pyproject.toml
+-rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-24 15:35:19.776999 pytch-fetch-1.0.1/setup.cfg
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:35:19.773999 pytch-fetch-1.0.1/src/
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:35:19.774999 pytch-fetch-1.0.1/src/pytch/
+-rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.0.1/src/pytch/__init__.py
+-rwxr-xr-x   0 krit      (1000) krit      (1001)     2207 2023-07-24 15:34:37.000000 pytch-fetch-1.0.1/src/pytch/__main__.py
+-rw-r--r--   0 krit      (1000) krit      (1001)    19845 2023-07-24 13:46:09.000000 pytch-fetch-1.0.1/src/pytch/art.py
+-rw-r--r--   0 krit      (1000) krit      (1001)     4596 2023-07-24 15:34:15.000000 pytch-fetch-1.0.1/src/pytch/funcs.py
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:35:19.776999 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/
+-rw-r--r--   0 krit      (1000) krit      (1001)     4099 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/entry_points.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/top_level.txt
```

### Comparing `pytch-fetch-1.0.0/LICENSE` & `pytch-fetch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.0.0/PKG-INFO` & `pytch-fetch-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
```

### Comparing `pytch-fetch-1.0.0/README.md` & `pytch-fetch-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.0.0/pyproject.toml` & `pytch-fetch-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytch-fetch"
-version = "1.0.0"
+version = "1.0.1"
 description="Pytch Yields Technical Characteristics Hastily"
 readme = "README.md"
 authors = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 maintainers = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 1 - Planning",
```

### Comparing `pytch-fetch-1.0.0/src/pytch/__main__.py` & `pytch-fetch-1.0.1/src/pytch/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
-from __version__ import __version__
 from os import getlogin
 from argparse import ArgumentParser
-from funcs import (
+from pytch.funcs import (
     get_name,
     get_uptime,
     get_shell,
     get_packages,
     get_memory,
     get_kernel,
     art,
@@ -26,15 +25,15 @@
         "-l",
         "--logo",
         metavar="DISTRO",
         dest="logo",
         help="use an alternate distribution's logo",
     )
 
-    parser.add_argument("-v", "--version", action="version", version=__version__)
+    parser.add_argument("-v", "--version", action="version", version="1.0.1")
 
     args = parser.parse_args()
 
     attrs = [
         {"name": "user", "value": getlogin(), "icon": "", "color": "red"},
         {"name": "os", "value": get_name(), "icon": "", "color": "yellow"},
         {"name": "kernel", "value": get_kernel(), "icon": "", "color": "green"},
```

### Comparing `pytch-fetch-1.0.0/src/pytch/art.py` & `pytch-fetch-1.0.1/src/pytch/art.py`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.0.0/src/pytch/funcs.py` & `pytch-fetch-1.0.1/src/pytch/funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import walk, environ
 from os.path import isfile
 from platform import release
 from subprocess import check_output, DEVNULL, CalledProcessError
 from re import search, findall, sub, split
-from art import art_dict
+from pytch.art import art_dict
 
 
 def color(text, color):
     colors = {
         "black": 90,
         "red": 31,
         "green": 32,
```

### Comparing `pytch-fetch-1.0.0/src/pytch_fetch.egg-info/PKG-INFO` & `pytch-fetch-1.0.1/src/pytch_fetch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
```

