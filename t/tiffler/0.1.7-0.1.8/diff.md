# Comparing `tmp/tiffler-0.1.7.tar.gz` & `tmp/tiffler-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiffler-0.1.7.tar", last modified: Sun Oct  2 04:53:39 2022, max compression
+gzip compressed data, was "tiffler-0.1.8.tar", last modified: Mon Jul 24 05:00:51 2023, max compression
```

## Comparing `tiffler-0.1.7.tar` & `tiffler-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-10-02 04:53:39.124376 tiffler-0.1.7/
--rw-r--r--   0 datnh      (501) staff       (20)     1263 2022-10-02 04:53:39.124170 tiffler-0.1.7/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)      896 2022-10-02 04:48:43.000000 tiffler-0.1.7/README.md
--rw-r--r--   0 datnh      (501) staff       (20)       38 2022-10-02 04:53:39.124463 tiffler-0.1.7/setup.cfg
--rw-r--r--   0 datnh      (501) staff       (20)     1250 2022-10-02 04:52:38.000000 tiffler-0.1.7/setup.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-10-02 04:53:39.123116 tiffler-0.1.7/tiffler/
--rw-r--r--   0 datnh      (501) staff       (20)       23 2022-10-02 04:48:43.000000 tiffler-0.1.7/tiffler/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     2884 2022-10-02 04:52:17.000000 tiffler-0.1.7/tiffler/tiffler.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-10-02 04:53:39.123967 tiffler-0.1.7/tiffler.egg-info/
--rw-r--r--   0 datnh      (501) staff       (20)     1263 2022-10-02 04:53:39.000000 tiffler-0.1.7/tiffler.egg-info/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)      181 2022-10-02 04:53:39.000000 tiffler-0.1.7/tiffler.egg-info/SOURCES.txt
--rw-r--r--   0 datnh      (501) staff       (20)        1 2022-10-02 04:53:39.000000 tiffler-0.1.7/tiffler.egg-info/dependency_links.txt
--rw-r--r--   0 datnh      (501) staff       (20)        8 2022-10-02 04:53:39.000000 tiffler-0.1.7/tiffler.egg-info/top_level.txt
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:00:51.179825 tiffler-0.1.8/
+-rw-r--r--   0 datnh      (501) staff       (20)     1319 2023-07-24 05:00:51.179705 tiffler-0.1.8/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)      896 2022-10-02 04:48:43.000000 tiffler-0.1.8/README.md
+-rw-r--r--   0 datnh      (501) staff       (20)       38 2023-07-24 05:00:51.179923 tiffler-0.1.8/setup.cfg
+-rw-r--r--   0 datnh      (501) staff       (20)     1250 2023-07-24 05:00:39.000000 tiffler-0.1.8/setup.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:00:51.178631 tiffler-0.1.8/tiffler/
+-rw-r--r--   0 datnh      (501) staff       (20)       23 2022-10-02 04:48:43.000000 tiffler-0.1.8/tiffler/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2893 2023-07-24 05:00:32.000000 tiffler-0.1.8/tiffler/tiffler.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:00:51.179420 tiffler-0.1.8/tiffler.egg-info/
+-rw-r--r--   0 datnh      (501) staff       (20)     1319 2023-07-24 05:00:51.000000 tiffler-0.1.8/tiffler.egg-info/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)      181 2023-07-24 05:00:51.000000 tiffler-0.1.8/tiffler.egg-info/SOURCES.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        1 2023-07-24 05:00:51.000000 tiffler-0.1.8/tiffler.egg-info/dependency_links.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        8 2023-07-24 05:00:51.000000 tiffler-0.1.8/tiffler.egg-info/top_level.txt
```

### Comparing `tiffler-0.1.7/PKG-INFO` & `tiffler-0.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: tiffler
-Version: 0.1.7
+Version: 0.1.8
 Summary: This Niffler finds shiny variables in text
+Home-page: UNKNOWN
 Author: nghoangdat
 Author-email: dat.nh.216@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Tiffler
@@ -49,7 +52,9 @@
 for match in tiffler.search(template, bill, case_sensitive=False):
     print(match)
 
 # {'item': 'Pewter cauldron', 'price': 15, 'unit': 'galeons'}
 # {'item': 'Brass cauldron', 'price': 21, 'unit': 'galeons'}
 # {'item': 'Copper cauldron', 'price': 25, 'unit': 'galeons'}
 ```
+
+
```

### Comparing `tiffler-0.1.7/README.md` & `tiffler-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tiffler-0.1.7/setup.py` & `tiffler-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 extras_require = {}
 for path in glob("requirements.*.txt"):
     match = re.search("(?<=\.).+(?=\.)", path)
     if match:
         mode = match.group(0)
         extras_require[mode] = read_requirements(path)
 
-__VERSION__ = "0.1.7"
+__VERSION__ = "0.1.8"
 __DESCRIPTION__ = "This Niffler finds shiny variables in text"
 
 
 setuptools.setup(
     name="tiffler",
     packages=setuptools.find_packages(),
     version=__VERSION__,
```

### Comparing `tiffler-0.1.7/tiffler/tiffler.py` & `tiffler-0.1.8/tiffler/tiffler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from collections import OrderedDict
 from functools import lru_cache
 from typing import *
 
 SUPPORTED_TYPES = {
     "float": "[-+]?\d*\.\d+|\d+",
-    "int": "[-+]?\d+",
+    "int": "[-+]?\d*\.\d+|\d+",
     "bool": "true|True|false|False|0|1",
     "str": ".+",
 }
 
 __all__ = ["Tiffler", "compile", "scan", "search"]
```

### Comparing `tiffler-0.1.7/tiffler.egg-info/PKG-INFO` & `tiffler-0.1.8/tiffler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: tiffler
-Version: 0.1.7
+Version: 0.1.8
 Summary: This Niffler finds shiny variables in text
+Home-page: UNKNOWN
 Author: nghoangdat
 Author-email: dat.nh.216@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Tiffler
@@ -49,7 +52,9 @@
 for match in tiffler.search(template, bill, case_sensitive=False):
     print(match)
 
 # {'item': 'Pewter cauldron', 'price': 15, 'unit': 'galeons'}
 # {'item': 'Brass cauldron', 'price': 21, 'unit': 'galeons'}
 # {'item': 'Copper cauldron', 'price': 25, 'unit': 'galeons'}
 ```
+
+
```

