# Comparing `tmp/Jedutils-0.1.6.tar.gz` & `tmp/Jedutils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jedutils-0.1.6.tar", last modified: Mon Jul 17 15:10:48 2023, max compression
+gzip compressed data, was "Jedutils-0.1.7.tar", last modified: Mon Jul 24 01:07:35 2023, max compression
```

## Comparing `Jedutils-0.1.6.tar` & `Jedutils-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:10:48.143226 Jedutils-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:10:48.139227 Jedutils-0.1.6/Jedutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-17 15:10:48.000000 Jedutils-0.1.6/Jedutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-17 15:10:48.000000 Jedutils-0.1.6/Jedutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:10:48.000000 Jedutils-0.1.6/Jedutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 15:10:48.000000 Jedutils-0.1.6/Jedutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 15:10:48.000000 Jedutils-0.1.6/Jedutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 15:10:46.000000 Jedutils-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 15:10:46.000000 Jedutils-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-17 15:10:48.143226 Jedutils-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-17 15:10:46.000000 Jedutils-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:10:48.139227 Jedutils-0.1.6/jedutils/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:10:48.139227 Jedutils-0.1.6/jedutils/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/asyncio/_async_redis_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/asyncio/_run_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:10:48.143226 Jedutils-0.1.6/jedutils/asyncio/network/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/asyncio/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/asyncio/network/_dl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:10:48.143226 Jedutils-0.1.6/jedutils/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/strings/_chunked_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-17 15:10:46.000000 Jedutils-0.1.6/jedutils/strings/_random_string.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:10:48.143226 Jedutils-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-17 15:10:46.000000 Jedutils-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:07:35.656093 Jedutils-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:07:35.652093 Jedutils-0.1.7/Jedutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 01:07:35.000000 Jedutils-0.1.7/Jedutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 01:07:35.000000 Jedutils-0.1.7/Jedutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 01:07:35.000000 Jedutils-0.1.7/Jedutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 01:07:35.000000 Jedutils-0.1.7/Jedutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 01:07:35.000000 Jedutils-0.1.7/Jedutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 01:07:34.000000 Jedutils-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 01:07:34.000000 Jedutils-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 01:07:35.656093 Jedutils-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 01:07:34.000000 Jedutils-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:07:35.652093 Jedutils-0.1.7/jedutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:07:35.652093 Jedutils-0.1.7/jedutils/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/asyncio/_async_redis_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/asyncio/_run_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:07:35.652093 Jedutils-0.1.7/jedutils/asyncio/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/asyncio/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/asyncio/network/_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:07:35.652093 Jedutils-0.1.7/jedutils/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/databases/_in_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:07:35.656093 Jedutils-0.1.7/jedutils/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/strings/_chunked_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-24 01:07:34.000000 Jedutils-0.1.7/jedutils/strings/_random_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 01:07:35.656093 Jedutils-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-24 01:07:34.000000 Jedutils-0.1.7/setup.py
```

### Comparing `Jedutils-0.1.6/Jedutils.egg-info/PKG-INFO` & `Jedutils-0.1.7/Jedutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
```

### Comparing `Jedutils-0.1.6/LICENSE` & `Jedutils-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.6/PKG-INFO` & `Jedutils-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
```

### Comparing `Jedutils-0.1.6/README.md` & `Jedutils-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.6/jedutils/asyncio/_async_redis_pipe.py` & `Jedutils-0.1.7/jedutils/asyncio/_async_redis_pipe.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.6/jedutils/asyncio/network/_dl.py` & `Jedutils-0.1.7/jedutils/asyncio/network/_dl.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.6/jedutils/strings/_chunked_text.py` & `Jedutils-0.1.7/jedutils/strings/_chunked_text.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.6/jedutils/strings/_random_string.py` & `Jedutils-0.1.7/jedutils/strings/_random_string.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.6/setup.py` & `Jedutils-0.1.7/setup.py`

 * *Files identical despite different names*

