# Comparing `tmp/rsplan-1.0.1.tar.gz` & `tmp/rsplan-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsplan-1.0.1.tar", last modified: Sun Jul 23 20:14:42 2023, max compression
+gzip compressed data, was "rsplan-1.0.2.tar", last modified: Mon Jul 24 00:07:22 2023, max compression
```

## Comparing `rsplan-1.0.1.tar` & `rsplan-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-23 20:14:42.366807 rsplan-1.0.1/
--rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.1/LICENSE
--rw-rw-r--   0 built     (1000) built     (1000)     5412 2023-07-23 20:14:42.366807 rsplan-1.0.1/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)     3755 2023-07-21 21:43:28.000000 rsplan-1.0.1/README.md
--rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-23 20:14:12.000000 rsplan-1.0.1/pyproject.toml
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-23 20:14:42.366807 rsplan-1.0.1/rsplan/
--rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-19 03:21:47.000000 rsplan-1.0.1/rsplan/__init__.py
--rw-rw-r--   0 built     (1000) built     (1000)    28383 2023-07-23 20:09:00.000000 rsplan-1.0.1/rsplan/curves.py
--rw-rw-r--   0 built     (1000) built     (1000)     2614 2023-07-23 20:09:06.000000 rsplan-1.0.1/rsplan/demo.py
--rw-rw-r--   0 built     (1000) built     (1000)     3082 2023-07-19 19:07:31.000000 rsplan-1.0.1/rsplan/helpers.py
--rw-rw-r--   0 built     (1000) built     (1000)     6527 2023-07-23 20:08:41.000000 rsplan-1.0.1/rsplan/planner.py
--rw-rw-r--   0 built     (1000) built     (1000)    11977 2023-07-21 17:30:35.000000 rsplan-1.0.1/rsplan/primitives.py
--rw-rw-r--   0 built     (1000) built     (1000)     5109 2023-07-23 20:08:55.000000 rsplan-1.0.1/rsplan/unit_tests.py
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-23 20:14:42.366807 rsplan-1.0.1/rsplan.egg-info/
--rw-rw-r--   0 built     (1000) built     (1000)     5412 2023-07-23 20:14:42.000000 rsplan-1.0.1/rsplan.egg-info/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)      319 2023-07-23 20:14:42.000000 rsplan-1.0.1/rsplan.egg-info/SOURCES.txt
--rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-23 20:14:42.000000 rsplan-1.0.1/rsplan.egg-info/dependency_links.txt
--rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-23 20:14:42.000000 rsplan-1.0.1/rsplan.egg-info/requires.txt
--rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-23 20:14:42.000000 rsplan-1.0.1/rsplan.egg-info/top_level.txt
--rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-23 20:14:42.366807 rsplan-1.0.1/setup.cfg
--rw-rw-r--   0 built     (1000) built     (1000)      643 2023-07-23 20:14:21.000000 rsplan-1.0.1/setup.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-24 00:07:22.968987 rsplan-1.0.2/
+-rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.2/LICENSE
+-rw-rw-r--   0 built     (1000) built     (1000)     5412 2023-07-24 00:07:22.968987 rsplan-1.0.2/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)     3755 2023-07-21 21:43:28.000000 rsplan-1.0.2/README.md
+-rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-24 00:07:13.000000 rsplan-1.0.2/pyproject.toml
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-24 00:07:22.968987 rsplan-1.0.2/rsplan/
+-rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-19 03:21:47.000000 rsplan-1.0.2/rsplan/__init__.py
+-rw-rw-r--   0 built     (1000) built     (1000)    28383 2023-07-23 20:09:00.000000 rsplan-1.0.2/rsplan/curves.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2614 2023-07-23 20:09:06.000000 rsplan-1.0.2/rsplan/demo.py
+-rw-rw-r--   0 built     (1000) built     (1000)     3082 2023-07-19 19:07:31.000000 rsplan-1.0.2/rsplan/helpers.py
+-rw-rw-r--   0 built     (1000) built     (1000)     6527 2023-07-23 20:08:41.000000 rsplan-1.0.2/rsplan/planner.py
+-rw-rw-r--   0 built     (1000) built     (1000)    11989 2023-07-24 00:04:40.000000 rsplan-1.0.2/rsplan/primitives.py
+-rw-rw-r--   0 built     (1000) built     (1000)     5109 2023-07-23 20:08:55.000000 rsplan-1.0.2/rsplan/unit_tests.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-24 00:07:22.968987 rsplan-1.0.2/rsplan.egg-info/
+-rw-rw-r--   0 built     (1000) built     (1000)     5412 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)      319 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/SOURCES.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/dependency_links.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/requires.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-24 00:07:22.000000 rsplan-1.0.2/rsplan.egg-info/top_level.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-24 00:07:22.968987 rsplan-1.0.2/setup.cfg
+-rw-rw-r--   0 built     (1000) built     (1000)      643 2023-07-24 00:07:00.000000 rsplan-1.0.2/setup.py
```

### Comparing `rsplan-1.0.1/LICENSE` & `rsplan-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.1/PKG-INFO` & `rsplan-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.1
+Version: 1.0.2
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
```

### Comparing `rsplan-1.0.1/README.md` & `rsplan-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.1/pyproject.toml` & `rsplan-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsplan"
-version = "1.0.1"
+version = "1.0.2"
 description = "Reeds-Shepp algorithm implementation in Python"
 readme = "README.md"
 authors = [{ name = "Built Robotics", email = "tarakapoor9@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rsplan-1.0.1/rsplan/curves.py` & `rsplan-1.0.2/rsplan/curves.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.1/rsplan/demo.py` & `rsplan-1.0.2/rsplan/demo.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.1/rsplan/helpers.py` & `rsplan-1.0.2/rsplan/helpers.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.1/rsplan/planner.py` & `rsplan-1.0.2/rsplan/planner.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.1/rsplan/primitives.py` & `rsplan-1.0.2/rsplan/primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import dataclasses
 import functools
 from typing import Any, List, Literal, Optional, Tuple
 
 import numpy as np
 
-import helpers
+from rsplan import helpers
 
 
 @dataclasses.dataclass
 class Path:
     """Reeds-Shepp path represented as its start/end points, turn radius (in meters),
     and a list of Segments. Additionally contains a step size value (in meters) used to
     calculate the Waypoint representation of the path.
```

### Comparing `rsplan-1.0.1/rsplan/unit_tests.py` & `rsplan-1.0.2/rsplan/unit_tests.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.1/rsplan.egg-info/PKG-INFO` & `rsplan-1.0.2/rsplan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.1
+Version: 1.0.2
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
```

### Comparing `rsplan-1.0.1/setup.py` & `rsplan-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "rsplan",
-    version = "1.0.1",
+    version = "1.0.2",
     author = "Built Robotics",
     author_email = "tarakapoor9@gmail.com",
     description = ("Reeds-Shepp algorithm implementation in Python."),
     license = "MIT",
     keywords = "reeds-shepp path planning",
     url = "https://github.com/builtrobotics/rs",
     packages=['rsplan'],
```

