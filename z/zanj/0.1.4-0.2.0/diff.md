# Comparing `tmp/zanj-0.1.4.tar.gz` & `tmp/zanj-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanj-0.1.4.tar", max compression
+gzip compressed data, was "zanj-0.2.0.tar", max compression
```

## Comparing `zanj-0.1.4.tar` & `zanj-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.1.4/LICENSE
--rw-r--r--   0        0        0     1094 2023-06-14 19:12:43.894602 zanj-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    10945 2023-06-14 19:11:26.380447 zanj-0.1.4/README.md
--rw-r--r--   0        0        0      146 2023-06-14 19:12:11.197526 zanj-0.1.4/zanj/__init__.py
--rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.1.4/zanj/externals.py
--rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.1.4/zanj/loading.py
--rw-r--r--   0        0        0        0 2023-06-13 22:16:55.290434 zanj-0.1.4/zanj/py.typed
--rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.1.4/zanj/readme.md
--rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.1.4/zanj/serializing.py
--rw-r--r--   0        0        0     9778 2023-06-14 03:53:30.489964 zanj-0.1.4/zanj/torchutil.py
--rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.1.4/zanj/zanj.py
--rw-r--r--   0        0        0    11918 1970-01-01 00:00:00.000000 zanj-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 zanj-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1177 2023-07-24 06:50:37.656207 zanj-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10945 2023-06-14 19:11:26.380447 zanj-0.2.0/README.md
+-rw-r--r--   0        0        0      146 2023-07-24 06:50:41.147372 zanj-0.2.0/zanj/__init__.py
+-rw-r--r--   0        0        0     1468 2023-05-28 05:22:18.527493 zanj-0.2.0/zanj/externals.py
+-rw-r--r--   0        0        0    15618 2023-05-28 05:22:18.537492 zanj-0.2.0/zanj/loading.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:16:55.290434 zanj-0.2.0/zanj/py.typed
+-rw-r--r--   0        0        0     4143 2023-05-28 05:13:20.057826 zanj-0.2.0/zanj/readme.md
+-rw-r--r--   0        0        0     8121 2023-05-28 05:22:18.541492 zanj-0.2.0/zanj/serializing.py
+-rw-r--r--   0        0        0     9778 2023-06-14 03:53:30.489964 zanj-0.2.0/zanj/torchutil.py
+-rw-r--r--   0        0        0     8468 2023-05-28 05:22:18.555490 zanj-0.2.0/zanj/zanj.py
+-rw-r--r--   0        0        0    11702 1970-01-01 00:00:00.000000 zanj-0.2.0/PKG-INFO
```

### Comparing `zanj-0.1.4/LICENSE` & `zanj-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zanj-0.1.4/README.md` & `zanj-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zanj-0.1.4/zanj/externals.py` & `zanj-0.2.0/zanj/externals.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.4/zanj/loading.py` & `zanj-0.2.0/zanj/loading.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.4/zanj/readme.md` & `zanj-0.2.0/zanj/readme.md`

 * *Files identical despite different names*

### Comparing `zanj-0.1.4/zanj/serializing.py` & `zanj-0.2.0/zanj/serializing.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.4/zanj/torchutil.py` & `zanj-0.2.0/zanj/torchutil.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.4/zanj/zanj.py` & `zanj-0.2.0/zanj/zanj.py`

 * *Files identical despite different names*

### Comparing `zanj-0.1.4/PKG-INFO` & `zanj-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: zanj
-Version: 0.1.4
+Version: 0.2.0
 Summary: save and load complex objects to disk without pickling
 Home-page: https://github.com/mivanit/ZANJ
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jaxtyping (>=0.2.12,<0.3.0)
-Requires-Dist: muutils (>=0.4.1,<0.5.0)
-Requires-Dist: numpy (>=1.22.4,<2.0.0)
+Requires-Dist: muutils[array] (>=0.5.1,<0.6.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: torch (>=1.13.1,<2.0.0)
 Project-URL: Repository, https://github.com/mivanit/ZANJ
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/zanj)](https://pypi.org/project/zanj/)
 [![Checks](https://github.com/mivanit/zanj/actions/workflows/checks.yml/badge.svg)](https://github.com/mivanit/zanj/actions/workflows/checks.yml)
 [![Coverage](docs/coverage/coverage.svg)](docs/coverage/coverage.txt)
 ![code size, bytes](https://img.shields.io/github/languages/code-size/mivanit/zanj)
```

