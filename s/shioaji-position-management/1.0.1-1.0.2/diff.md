# Comparing `tmp/shioaji_position_management-1.0.1.tar.gz` & `tmp/shioaji_position_management-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioaji_position_management-1.0.1.tar", last modified: Mon Jul 24 05:53:53 2023, max compression
+gzip compressed data, was "shioaji_position_management-1.0.2.tar", last modified: Mon Jul 24 05:55:37 2023, max compression
```

## Comparing `shioaji_position_management-1.0.1.tar` & `shioaji_position_management-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:53:53.028354 shioaji_position_management-1.0.1/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     1067 2023-07-24 05:41:32.000000 shioaji_position_management-1.0.1/LICENSE
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2618 2023-07-24 05:53:53.028354 shioaji_position_management-1.0.1/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2010 2023-07-24 05:53:20.000000 shioaji_position_management-1.0.1/README.md
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-07-24 05:41:50.000000 shioaji_position_management-1.0.1/pyproject.toml
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      771 2023-07-24 05:53:53.028354 shioaji_position_management-1.0.1/setup.cfg
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:53:53.028354 shioaji_position_management-1.0.1/src/
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:53:53.028354 shioaji_position_management-1.0.1/src/shioaji_position_management/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       95 2023-07-24 05:41:49.000000 shioaji_position_management-1.0.1/src/shioaji_position_management/__init__.py
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3084 2023-07-24 05:52:37.000000 shioaji_position_management-1.0.1/src/shioaji_position_management/shioaji_position_management.py
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:53:53.028354 shioaji_position_management-1.0.1/src/shioaji_position_management.egg-info/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2618 2023-07-24 05:53:53.000000 shioaji_position_management-1.0.1/src/shioaji_position_management.egg-info/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      423 2023-07-24 05:53:53.000000 shioaji_position_management-1.0.1/src/shioaji_position_management.egg-info/SOURCES.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-24 05:53:53.000000 shioaji_position_management-1.0.1/src/shioaji_position_management.egg-info/dependency_links.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-07-24 05:53:53.000000 shioaji_position_management-1.0.1/src/shioaji_position_management.egg-info/requires.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       28 2023-07-24 05:53:53.000000 shioaji_position_management-1.0.1/src/shioaji_position_management.egg-info/top_level.txt
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:55:37.121884 shioaji_position_management-1.0.2/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     1067 2023-07-24 05:41:32.000000 shioaji_position_management-1.0.2/LICENSE
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2627 2023-07-24 05:55:37.121884 shioaji_position_management-1.0.2/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2019 2023-07-24 05:55:28.000000 shioaji_position_management-1.0.2/README.md
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-07-24 05:41:50.000000 shioaji_position_management-1.0.2/pyproject.toml
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      771 2023-07-24 05:55:37.121884 shioaji_position_management-1.0.2/setup.cfg
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:55:37.117884 shioaji_position_management-1.0.2/src/
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:55:37.121884 shioaji_position_management-1.0.2/src/shioaji_position_management/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       95 2023-07-24 05:41:49.000000 shioaji_position_management-1.0.2/src/shioaji_position_management/__init__.py
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3096 2023-07-24 05:55:07.000000 shioaji_position_management-1.0.2/src/shioaji_position_management/shioaji_position_management.py
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:55:37.121884 shioaji_position_management-1.0.2/src/shioaji_position_management.egg-info/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2627 2023-07-24 05:55:37.000000 shioaji_position_management-1.0.2/src/shioaji_position_management.egg-info/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      423 2023-07-24 05:55:37.000000 shioaji_position_management-1.0.2/src/shioaji_position_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-24 05:55:37.000000 shioaji_position_management-1.0.2/src/shioaji_position_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-07-24 05:55:37.000000 shioaji_position_management-1.0.2/src/shioaji_position_management.egg-info/requires.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       28 2023-07-24 05:55:37.000000 shioaji_position_management-1.0.2/src/shioaji_position_management.egg-info/top_level.txt
```

### Comparing `shioaji_position_management-1.0.1/LICENSE` & `shioaji_position_management-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shioaji_position_management-1.0.1/PKG-INFO` & `shioaji_position_management-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioaji_position_management
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Extensions help you trading with Sinopac shioaji
 Home-page: https://github.com/NickLin910221/shioaji_position_management
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Position_Management/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +58,16 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
-- v1.0.1 (2023/7/24) Release & fix some bugs
+- v1.0.2 (2023/7/24) Release & fix some bugs
+- v1.0.1
 - v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/shioaji_position_management/issues) for a list of proposed features (and known issues).
 
 ## Authors
```

### Comparing `shioaji_position_management-1.0.1/README.md` & `shioaji_position_management-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
-- v1.0.1 (2023/7/24) Release & fix some bugs
+- v1.0.2 (2023/7/24) Release & fix some bugs
+- v1.0.1
 - v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/shioaji_position_management/issues) for a list of proposed features (and known issues).
 
 ## Authors
```

### Comparing `shioaji_position_management-1.0.1/setup.cfg` & `shioaji_position_management-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shioaji_position_management
-version = 1.0.1
+version = 1.0.2
 author = NickLin910221
 author_email = nicklin910221@gmail.com
 description = An Extensions help you trading with Sinopac shioaji
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = shioaji
 url = https://github.com/NickLin910221/shioaji_position_management
```

### Comparing `shioaji_position_management-1.0.1/src/shioaji_position_management/shioaji_position_management.py` & `shioaji_position_management-1.0.2/src/shioaji_position_management/shioaji_position_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import loguru
+from loguru import logger
 
 class shioaji_position_management:
     __slots__ = ["api", "stock", "future", "option", "ordering", "acc", "logger"]
 
     def __init__(self, api, acc):
         self.api = api
         assert len(api.list_accounts()) > 0
```

### Comparing `shioaji_position_management-1.0.1/src/shioaji_position_management.egg-info/PKG-INFO` & `shioaji_position_management-1.0.2/src/shioaji_position_management.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioaji-position-management
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Extensions help you trading with Sinopac shioaji
 Home-page: https://github.com/NickLin910221/shioaji_position_management
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Position_Management/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +58,16 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
-- v1.0.1 (2023/7/24) Release & fix some bugs
+- v1.0.2 (2023/7/24) Release & fix some bugs
+- v1.0.1
 - v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/shioaji_position_management/issues) for a list of proposed features (and known issues).
 
 ## Authors
```

