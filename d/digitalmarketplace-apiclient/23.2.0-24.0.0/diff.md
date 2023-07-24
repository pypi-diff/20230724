# Comparing `tmp/digitalmarketplace-apiclient-23.2.0.tar.gz` & `tmp/digitalmarketplace-apiclient-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalmarketplace-apiclient-23.2.0.tar", last modified: Thu Sep  8 13:15:39 2022, max compression
+gzip compressed data, was "digitalmarketplace-apiclient-24.0.0.tar", last modified: Mon Jul 24 15:22:03 2023, max compression
```

## Comparing `digitalmarketplace-apiclient-23.2.0.tar` & `digitalmarketplace-apiclient-24.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 13:15:39.509674 digitalmarketplace-apiclient-23.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-08 13:15:39.509674 digitalmarketplace-apiclient-23.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 13:15:39.509674 digitalmarketplace-apiclient-23.2.0/digitalmarketplace_apiclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-08 13:15:39.000000 digitalmarketplace-apiclient-23.2.0/digitalmarketplace_apiclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-08 13:15:39.000000 digitalmarketplace-apiclient-23.2.0/digitalmarketplace_apiclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 13:15:39.000000 digitalmarketplace-apiclient-23.2.0/digitalmarketplace_apiclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-08 13:15:39.000000 digitalmarketplace-apiclient-23.2.0/digitalmarketplace_apiclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-08 13:15:39.000000 digitalmarketplace-apiclient-23.2.0/digitalmarketplace_apiclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 13:15:39.509674 digitalmarketplace-apiclient-23.2.0/dmapiclient/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/dmapiclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/dmapiclient/antivirus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/dmapiclient/audit.py
--rw-r--r--   0 runner    (1001) docker     (121)    13174 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/dmapiclient/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    44397 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/dmapiclient/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/dmapiclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/dmapiclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/dmapiclient/search.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-08 13:15:39.509674 digitalmarketplace-apiclient-23.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-09-08 13:15:28.000000 digitalmarketplace-apiclient-23.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:22:03.224259 digitalmarketplace-apiclient-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 15:22:03.224259 digitalmarketplace-apiclient-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:22:03.220259 digitalmarketplace-apiclient-24.0.0/digitalmarketplace_apiclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 15:22:03.000000 digitalmarketplace-apiclient-24.0.0/digitalmarketplace_apiclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-24 15:22:03.000000 digitalmarketplace-apiclient-24.0.0/digitalmarketplace_apiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:22:03.000000 digitalmarketplace-apiclient-24.0.0/digitalmarketplace_apiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 15:22:03.000000 digitalmarketplace-apiclient-24.0.0/digitalmarketplace_apiclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 15:22:03.000000 digitalmarketplace-apiclient-24.0.0/digitalmarketplace_apiclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:22:03.224259 digitalmarketplace-apiclient-24.0.0/dmapiclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/dmapiclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/dmapiclient/antivirus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/dmapiclient/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/dmapiclient/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44397 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/dmapiclient/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/dmapiclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/dmapiclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/dmapiclient/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-24 15:22:03.224259 digitalmarketplace-apiclient-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-24 15:21:48.000000 digitalmarketplace-apiclient-24.0.0/setup.py
```

### Comparing `digitalmarketplace-apiclient-23.2.0/LICENCE` & `digitalmarketplace-apiclient-24.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-apiclient-23.2.0/README.md` & `digitalmarketplace-apiclient-24.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Digital Marketplace API client
 =========================
 
-![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
+![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 
 ## What's in here?
 
 API clients for Digital Marketplace [Data API](https://github.com/Crown-Commercial-Service/digitalmarketplace-api) and
 [Search API](https://github.com/Crown-Commercial-Service/digitalmarketplace-search-api).
 
 Originally was part of [Digital Marketplace Utils](https://github.com/Crown-Commercial-Service/digitalmarketplace-utils).
```

### Comparing `digitalmarketplace-apiclient-23.2.0/dmapiclient/antivirus.py` & `digitalmarketplace-apiclient-24.0.0/dmapiclient/antivirus.py`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-apiclient-23.2.0/dmapiclient/audit.py` & `digitalmarketplace-apiclient-24.0.0/dmapiclient/audit.py`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-apiclient-23.2.0/dmapiclient/base.py` & `digitalmarketplace-apiclient-24.0.0/dmapiclient/base.py`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-apiclient-23.2.0/dmapiclient/data.py` & `digitalmarketplace-apiclient-24.0.0/dmapiclient/data.py`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-apiclient-23.2.0/dmapiclient/errors.py` & `digitalmarketplace-apiclient-24.0.0/dmapiclient/errors.py`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-apiclient-23.2.0/dmapiclient/search.py` & `digitalmarketplace-apiclient-24.0.0/dmapiclient/search.py`

 * *Files identical despite different names*

### Comparing `digitalmarketplace-apiclient-23.2.0/setup.py` & `digitalmarketplace-apiclient-24.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     long_description=__doc__,
     packages=find_packages(),
     package_data={'dmapiclient': ['py.typed']},
     include_package_data=True,
     install_requires=[
         'requests<3,>=2.18.4',
     ],
-    python_requires="~=3.8",
+    python_requires="~=3.9",
 )
```

