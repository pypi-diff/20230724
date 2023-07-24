# Comparing `tmp/aeronet-0.1.0a3.tar.gz` & `tmp/aeronet-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet-0.1.0a3.tar", last modified: Mon Jul 24 12:57:24 2023, max compression
+gzip compressed data, was "aeronet-0.1.0a4.tar", last modified: Mon Jul 24 13:13:25 2023, max compression
```

## Comparing `aeronet-0.1.0a3.tar` & `aeronet-0.1.0a4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:57:24.057213 aeronet-0.1.0a3/
--rw-r--r--   0 trekin     (501) staff       (20)     1077 2023-04-01 13:22:48.000000 aeronet-0.1.0a3/LICENSE
--rw-r--r--   0 trekin     (501) staff       (20)       18 2023-07-24 09:31:48.000000 aeronet-0.1.0a3/MANIFEST.in
--rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-24 12:57:24.056799 aeronet-0.1.0a3/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     4586 2023-07-24 09:42:18.000000 aeronet-0.1.0a3/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:57:24.051382 aeronet-0.1.0a3/aeronet/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a3/aeronet/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 12:57:19.000000 aeronet-0.1.0a3/aeronet/__version__.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:57:24.055323 aeronet-0.1.0a3/aeronet/converters/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a3/aeronet/converters/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)      225 2023-07-21 05:30:39.000000 aeronet-0.1.0a3/aeronet/converters/split.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:57:24.056292 aeronet-0.1.0a3/aeronet/dataset/
--rw-r--r--   0 trekin     (501) staff       (20)      972 2023-07-21 14:58:33.000000 aeronet-0.1.0a3/aeronet/dataset/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)      230 2023-07-21 14:31:48.000000 aeronet-0.1.0a3/aeronet/dataset/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:57:24.054230 aeronet-0.1.0a3/aeronet.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-24 12:57:24.000000 aeronet-0.1.0a3/aeronet.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      348 2023-07-24 12:57:24.000000 aeronet-0.1.0a3/aeronet.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 12:57:24.000000 aeronet-0.1.0a3/aeronet.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)      190 2023-07-24 12:57:24.000000 aeronet-0.1.0a3/aeronet.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       43 2023-07-24 12:57:24.000000 aeronet-0.1.0a3/aeronet.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 12:57:24.057331 aeronet-0.1.0a3/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     4135 2023-07-24 08:53:55.000000 aeronet-0.1.0a3/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:25.845748 aeronet-0.1.0a4/
+-rw-r--r--   0 trekin     (501) staff       (20)     1077 2023-04-01 13:22:48.000000 aeronet-0.1.0a4/LICENSE
+-rw-r--r--   0 trekin     (501) staff       (20)       18 2023-07-24 09:31:48.000000 aeronet-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-24 13:13:25.844727 aeronet-0.1.0a4/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     4586 2023-07-24 09:42:18.000000 aeronet-0.1.0a4/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:25.841372 aeronet-0.1.0a4/aeronet/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a4/aeronet/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 13:12:38.000000 aeronet-0.1.0a4/aeronet/__version__.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:25.843585 aeronet-0.1.0a4/aeronet/converters/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a4/aeronet/converters/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)      225 2023-07-21 05:30:39.000000 aeronet-0.1.0a4/aeronet/converters/split.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:25.844262 aeronet-0.1.0a4/aeronet/dataset/
+-rw-r--r--   0 trekin     (501) staff       (20)      972 2023-07-21 14:58:33.000000 aeronet-0.1.0a4/aeronet/dataset/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)      230 2023-07-21 14:31:48.000000 aeronet-0.1.0a4/aeronet/dataset/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:25.843078 aeronet-0.1.0a4/aeronet.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-24 13:13:25.000000 aeronet-0.1.0a4/aeronet.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      348 2023-07-24 13:13:25.000000 aeronet-0.1.0a4/aeronet.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 13:13:25.000000 aeronet-0.1.0a4/aeronet.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)      190 2023-07-24 13:13:25.000000 aeronet-0.1.0a4/aeronet.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       43 2023-07-24 13:13:25.000000 aeronet-0.1.0a4/aeronet.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 13:13:25.846192 aeronet-0.1.0a4/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     4135 2023-07-24 08:53:55.000000 aeronet-0.1.0a4/setup.py
```

### Comparing `aeronet-0.1.0a3/LICENSE` & `aeronet-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a3/PKG-INFO` & `aeronet-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Deep learning with remote sensing data.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet-0.1.0a3/README.rst` & `aeronet-0.1.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a3/aeronet/dataset/__init__.py` & `aeronet-0.1.0a4/aeronet/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a3/aeronet.egg-info/PKG-INFO` & `aeronet-0.1.0a4/aeronet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Deep learning with remote sensing data.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet-0.1.0a3/setup.py` & `aeronet-0.1.0a4/setup.py`

 * *Files identical despite different names*

