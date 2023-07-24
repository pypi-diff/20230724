# Comparing `tmp/biggo_pms_api_python-1.1.0.tar.gz` & `tmp/biggo_pms_api_python-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biggo_pms_api_python-1.1.0.tar", last modified: Mon Jul 24 06:42:13 2023, max compression
+gzip compressed data, was "biggo_pms_api_python-1.1.1.tar", last modified: Mon Jul 24 06:45:17 2023, max compression
```

## Comparing `biggo_pms_api_python-1.1.0.tar` & `biggo_pms_api_python-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 06:42:13.266747 biggo_pms_api_python-1.1.0/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1069 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.1.0/LICENSE
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1842 2023-07-24 06:42:13.266747 biggo_pms_api_python-1.1.0/PKG-INFO
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1548 2023-07-24 06:38:56.000000 biggo_pms_api_python-1.1.0/README.md
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 06:42:13.266747 biggo_pms_api_python-1.1.0/biggo_pms_api_python/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)       30 2023-07-24 06:05:08.000000 biggo_pms_api_python-1.1.0/biggo_pms_api_python/__init__.py
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      451 2023-07-24 01:44:32.000000 biggo_pms_api_python-1.1.0/biggo_pms_api_python/error.py
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     8273 2023-07-24 05:56:33.000000 biggo_pms_api_python-1.1.0/biggo_pms_api_python/index.py
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 06:42:13.266747 biggo_pms_api_python-1.1.0/biggo_pms_api_python.egg-info/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1842 2023-07-24 06:42:13.000000 biggo_pms_api_python-1.1.0/biggo_pms_api_python.egg-info/PKG-INFO
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 06:42:13.000000 biggo_pms_api_python-1.1.0/biggo_pms_api_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 06:42:13.000000 biggo_pms_api_python-1.1.0/biggo_pms_api_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)       21 2023-07-24 06:42:13.000000 biggo_pms_api_python-1.1.0/biggo_pms_api_python.egg-info/top_level.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)       38 2023-07-24 06:42:13.266747 biggo_pms_api_python-1.1.0/setup.cfg
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      502 2023-07-24 06:41:13.000000 biggo_pms_api_python-1.1.0/setup.py
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 06:45:17.558422 biggo_pms_api_python-1.1.1/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1069 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.1.1/LICENSE
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1833 2023-07-24 06:45:17.558422 biggo_pms_api_python-1.1.1/PKG-INFO
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1539 2023-07-24 06:44:38.000000 biggo_pms_api_python-1.1.1/README.md
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 06:45:17.558422 biggo_pms_api_python-1.1.1/biggo_pms_api_python/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       30 2023-07-24 06:05:08.000000 biggo_pms_api_python-1.1.1/biggo_pms_api_python/__init__.py
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      451 2023-07-24 01:44:32.000000 biggo_pms_api_python-1.1.1/biggo_pms_api_python/error.py
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     8273 2023-07-24 05:56:33.000000 biggo_pms_api_python-1.1.1/biggo_pms_api_python/index.py
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 06:45:17.558422 biggo_pms_api_python-1.1.1/biggo_pms_api_python.egg-info/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1833 2023-07-24 06:45:17.000000 biggo_pms_api_python-1.1.1/biggo_pms_api_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 06:45:17.000000 biggo_pms_api_python-1.1.1/biggo_pms_api_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 06:45:17.000000 biggo_pms_api_python-1.1.1/biggo_pms_api_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       21 2023-07-24 06:45:17.000000 biggo_pms_api_python-1.1.1/biggo_pms_api_python.egg-info/top_level.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       38 2023-07-24 06:45:17.558422 biggo_pms_api_python-1.1.1/setup.cfg
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      502 2023-07-24 06:45:10.000000 biggo_pms_api_python-1.1.1/setup.py
```

### Comparing `biggo_pms_api_python-1.1.0/LICENSE` & `biggo_pms_api_python-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biggo_pms_api_python-1.1.0/PKG-INFO` & `biggo_pms_api_python-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-Metadata-Version: 2.1
-Name: biggo_pms_api_python
-Version: 1.1.0
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: MIT
-Platform: UNKNOWN
-Requires: requests
-Requires: base64
-Requires: time
-Requires: json
-Requires: os
-Requires: datetime
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# BigGo API PMS Python Client
 
-# BigGo API PMS Javascript Client
 
-
-BigGo API PMS Javascript Client is a API written in Javascript. 
+BigGo API PMS Python Client is a API written in Python. 
 
 short future:
 
 - [Getting Started](#getting-started)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Initializing](#initializing)
@@ -31,15 +15,15 @@
 ## Getting Started
 
 ### Installation
 
 Using pip
 
 ```shell
-pip install biggo_pms_api_python
+pip install -U biggo_pms_api_python
 ```
 
 ### Usage
 
 Using:
 
 ```python
@@ -74,9 +58,7 @@
 ```
 
 if you need more information, you can refer to this [document](./biggo_pms_api_python/README.md).
 
 ## License
 
 [MIT](./LICENSE)
-
-
```

### Comparing `biggo_pms_api_python-1.1.0/biggo_pms_api_python/index.py` & `biggo_pms_api_python-1.1.1/biggo_pms_api_python/index.py`

 * *Files identical despite different names*

### Comparing `biggo_pms_api_python-1.1.0/biggo_pms_api_python.egg-info/PKG-INFO` & `biggo_pms_api_python-1.1.1/biggo_pms_api_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: biggo-pms-api-python
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Requires: requests
 Requires: base64
 Requires: time
 Requires: json
 Requires: os
 Requires: datetime
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# BigGo API PMS Javascript Client
+# BigGo API PMS Python Client
 
 
-BigGo API PMS Javascript Client is a API written in Javascript. 
+BigGo API PMS Python Client is a API written in Python. 
 
 short future:
 
 - [Getting Started](#getting-started)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Initializing](#initializing)
@@ -31,15 +31,15 @@
 ## Getting Started
 
 ### Installation
 
 Using pip
 
 ```shell
-pip install biggo_pms_api_python
+pip install -U biggo_pms_api_python
 ```
 
 ### Usage
 
 Using:
 
 ```python
```

