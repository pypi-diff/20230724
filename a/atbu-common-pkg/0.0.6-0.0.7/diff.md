# Comparing `tmp/atbu-common-pkg-0.0.6.tar.gz` & `tmp/atbu-common-pkg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atbu-common-pkg-0.0.6.tar", last modified: Tue May 16 05:31:43 2023, max compression
+gzip compressed data, was "atbu-common-pkg-0.0.7.tar", last modified: Mon Jul 24 12:08:37 2023, max compression
```

## Comparing `atbu-common-pkg-0.0.6.tar` & `atbu-common-pkg-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.812369 atbu-common-pkg-0.0.6/
--rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2419 2023-05-16 05:31:43.811370 atbu-common-pkg-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2022-06-09 04:50:33.000000 atbu-common-pkg-0.0.6/README.md
--rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 05:31:43.812369 atbu-common-pkg-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1782 2023-05-16 05:29:05.000000 atbu-common-pkg-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.762422 atbu-common-pkg-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.762422 atbu-common-pkg-0.0.6/src/atbu/
-drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.786374 atbu-common-pkg-0.0.6/src/atbu/common/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.6/src/atbu/common/__init__.py
--rw-rw-rw-   0        0        0     6142 2022-06-08 21:42:34.000000 atbu-common-pkg-0.0.6/src/atbu/common/aes_cbc.py
--rw-rw-rw-   0        0        0     8076 2022-06-09 03:13:12.000000 atbu-common-pkg-0.0.6/src/atbu/common/exception.py
--rw-rw-rw-   0        0        0     2503 2022-06-09 03:47:47.000000 atbu-common-pkg-0.0.6/src/atbu/common/hasher.py
--rw-rw-rw-   0        0        0     4223 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.6/src/atbu/common/multi_json_enc_dec.py
--rw-rw-rw-   0        0        0     3946 2022-07-26 01:57:07.000000 atbu-common-pkg-0.0.6/src/atbu/common/profile.py
--rw-rw-rw-   0        0        0     2745 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.6/src/atbu/common/simple_report.py
--rw-rw-rw-   0        0        0     1330 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.6/src/atbu/common/singleton.py
--rw-rw-rw-   0        0        0     8660 2022-10-12 15:50:13.000000 atbu-common-pkg-0.0.6/src/atbu/common/util_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.808381 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/
--rw-rw-rw-   0        0        0     2419 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.809372 atbu-common-pkg-0.0.6/tests/
--rw-rw-rw-   0        0        0     3282 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.6/tests/test_enc_dec.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.260083 atbu-common-pkg-0.0.7/
+-rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2419 2023-07-24 12:08:37.259094 atbu-common-pkg-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1718 2022-06-09 04:50:33.000000 atbu-common-pkg-0.0.7/README.md
+-rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 12:08:37.260083 atbu-common-pkg-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1782 2023-07-24 12:01:38.000000 atbu-common-pkg-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.197087 atbu-common-pkg-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.196092 atbu-common-pkg-0.0.7/src/atbu/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.225083 atbu-common-pkg-0.0.7/src/atbu/common/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.7/src/atbu/common/__init__.py
+-rw-rw-rw-   0        0        0     6142 2022-06-08 21:42:34.000000 atbu-common-pkg-0.0.7/src/atbu/common/aes_cbc.py
+-rw-rw-rw-   0        0        0     8076 2022-06-09 03:13:12.000000 atbu-common-pkg-0.0.7/src/atbu/common/exception.py
+-rw-rw-rw-   0        0        0     2503 2022-06-09 03:47:47.000000 atbu-common-pkg-0.0.7/src/atbu/common/hasher.py
+-rw-rw-rw-   0        0        0     4223 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.7/src/atbu/common/multi_json_enc_dec.py
+-rw-rw-rw-   0        0        0     3946 2022-07-26 01:57:07.000000 atbu-common-pkg-0.0.7/src/atbu/common/profile.py
+-rw-rw-rw-   0        0        0     2745 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.7/src/atbu/common/simple_report.py
+-rw-rw-rw-   0        0        0     1330 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.7/src/atbu/common/singleton.py
+-rw-rw-rw-   0        0        0    10618 2023-07-24 11:21:50.000000 atbu-common-pkg-0.0.7/src/atbu/common/util_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.255088 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/
+-rw-rw-rw-   0        0        0     2419 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-24 12:08:37.000000 atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 12:08:37.257082 atbu-common-pkg-0.0.7/tests/
+-rw-rw-rw-   0        0        0     3282 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.7/tests/test_enc_dec.py
```

### Comparing `atbu-common-pkg-0.0.6/LICENSE` & `atbu-common-pkg-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/PKG-INFO` & `atbu-common-pkg-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-common-pkg
-Version: 0.0.6
+Version: 0.0.7
 Summary: ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline.
 Home-page: https://github.com/AshleyT3/atbu-common
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu-common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atbu-common-pkg-0.0.6/README.md` & `atbu-common-pkg-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/setup.py` & `atbu-common-pkg-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="atbu-common-pkg",
-    version="0.0.6",
+    version="0.0.7",
     author="Ashley R. Thomas",
     author_email="ashley.r.thomas.701@gmail.com",
     description= (
         "ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `atbu-common-pkg-0.0.6/src/atbu/common/aes_cbc.py` & `atbu-common-pkg-0.0.7/src/atbu/common/aes_cbc.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/src/atbu/common/exception.py` & `atbu-common-pkg-0.0.7/src/atbu/common/exception.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/src/atbu/common/hasher.py` & `atbu-common-pkg-0.0.7/src/atbu/common/hasher.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/src/atbu/common/multi_json_enc_dec.py` & `atbu-common-pkg-0.0.7/src/atbu/common/multi_json_enc_dec.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/src/atbu/common/profile.py` & `atbu-common-pkg-0.0.7/src/atbu/common/profile.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/src/atbu/common/simple_report.py` & `atbu-common-pkg-0.0.7/src/atbu/common/simple_report.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/src/atbu/common/singleton.py` & `atbu-common-pkg-0.0.7/src/atbu/common/singleton.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/src/atbu/common/util_helpers.py` & `atbu-common-pkg-0.0.7/src/atbu/common/util_helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import fnmatch
 from io import SEEK_END, SEEK_SET
 import io
 import os
 from pathlib import Path
 import platform
 import random
+import re
 from shutil import copy2
 from typing import Iterator, Union
 from datetime import datetime, timezone
 
 from .exception import InvalidFunctionArgument
 
 
@@ -116,14 +117,74 @@
             deep_union_dicts(dest_v, src_v)
         else:
             # Overwrite existing d1 value.
             dest[src_k] = src_v
     return dest
 
 
+def get_path_sep_list():
+    return [os.path.sep] if os.path.altsep is None else [os.path.sep, os.path.altsep]
+
+
+def get_path_sep_re():
+    if os.path.altsep is None:
+        path_sep_re_group_pattern = rf"({re.escape(os.path.sep)})"
+    else:
+        path_sep_re_group_pattern = rf"({re.escape(os.path.sep)}|{re.escape(os.path.altsep)})"
+    return re.compile(path_sep_re_group_pattern)
+
+
+_PATH_SEP_RE = get_path_sep_re()
+
+
+def strip_leading_sep(path: str) -> str:
+    if path and path[0] in [os.sep, os.altsep]:
+        path = path[1:]
+    return path
+
+
+def rel_path(top_level_dir: str, path: str):
+    common_path = os.path.commonpath([os.path.normcase(top_level_dir), os.path.normcase(path)])
+    if common_path != os.path.normcase(top_level_dir):
+        raise ValueError(
+            f"The path must be a subdirectory of top_level_dir: "
+            f"top_level_dir={top_level_dir} path={path}"
+        )
+    rpath = path[len(top_level_dir) :]
+    return strip_leading_sep(rpath)
+
+
+def strip_common_path(path1: str, path2: str) -> tuple[str, str]:
+    common_path = os.path.normcase(os.path.commonpath([path1, path2]))
+    if not common_path:
+        raise ValueError("Paths have no common path.")
+    path1 = strip_leading_sep(path1[len(common_path):])
+    path2 = strip_leading_sep(path2[len(common_path):])
+    return path1, path2
+
+
+def get_subdir_distance(path1: str, path2: str) -> int:
+    if len(path1)==0 and len(path2)==0:
+        return 0
+    try:
+        path1, path2 = strip_common_path(path1, path2)
+    except ValueError:
+        if path1 and path2:
+            return -1
+    if len(path1) >= len(path2):
+        subdir_part = path1[len(path2):]
+    else:
+        subdir_part = path2[len(path1):]
+    subdir_part = strip_leading_sep(subdir_part)
+    if not subdir_part:
+        return 0
+    num_seps = len(_PATH_SEP_RE.findall(subdir_part))
+    return num_seps + 1
+
+
 def convert_to_pathlib_path(p):
     if p is None:
         return None
     if not isinstance(p, Path):
         p = Path(p)
     return p
```

### Comparing `atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/PKG-INFO` & `atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-common-pkg
-Version: 0.0.6
+Version: 0.0.7
 Summary: ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline.
 Home-page: https://github.com/AshleyT3/atbu-common
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu-common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/SOURCES.txt` & `atbu-common-pkg-0.0.7/src/atbu_common_pkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.6/tests/test_enc_dec.py` & `atbu-common-pkg-0.0.7/tests/test_enc_dec.py`

 * *Files identical despite different names*

