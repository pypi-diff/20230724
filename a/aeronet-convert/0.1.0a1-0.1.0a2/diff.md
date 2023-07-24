# Comparing `tmp/aeronet_convert-0.1.0a1.tar.gz` & `tmp/aeronet_convert-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_convert-0.1.0a1.tar", last modified: Mon Jul 24 09:42:52 2023, max compression
+gzip compressed data, was "aeronet_convert-0.1.0a2.tar", last modified: Mon Jul 24 12:57:23 2023, max compression
```

## Comparing `aeronet_convert-0.1.0a1.tar` & `aeronet_convert-0.1.0a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:52.333874 aeronet_convert-0.1.0a1/
--rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-24 09:42:52.333579 aeronet_convert-0.1.0a1/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     2053 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a1/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:52.331347 aeronet_convert-0.1.0a1/aeronet_convert/
--rw-r--r--   0 trekin     (501) staff       (20)       67 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a1/aeronet_convert/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a1/aeronet_convert/__version__.py
--rw-r--r--   0 trekin     (501) staff       (20)     1250 2023-07-21 06:21:28.000000 aeronet_convert-0.1.0a1/aeronet_convert/rasterize.py
--rw-r--r--   0 trekin     (501) staff       (20)     5428 2023-07-21 06:21:18.000000 aeronet_convert-0.1.0a1/aeronet_convert/vectorize.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:52.333115 aeronet_convert-0.1.0a1/aeronet_convert.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-24 09:42:52.000000 aeronet_convert-0.1.0a1/aeronet_convert.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      330 2023-07-24 09:42:52.000000 aeronet_convert-0.1.0a1/aeronet_convert.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 09:42:52.000000 aeronet_convert-0.1.0a1/aeronet_convert.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       71 2023-07-24 09:42:52.000000 aeronet_convert-0.1.0a1/aeronet_convert.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       16 2023-07-24 09:42:52.000000 aeronet_convert-0.1.0a1/aeronet_convert.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 09:42:52.333988 aeronet_convert-0.1.0a1/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     4373 2023-07-24 09:02:15.000000 aeronet_convert-0.1.0a1/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:57:23.661167 aeronet_convert-0.1.0a2/
+-rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-24 12:57:23.660806 aeronet_convert-0.1.0a2/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     2053 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a2/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:57:23.658535 aeronet_convert-0.1.0a2/aeronet_convert/
+-rw-r--r--   0 trekin     (501) staff       (20)       67 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a2/aeronet_convert/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 12:56:22.000000 aeronet_convert-0.1.0a2/aeronet_convert/__version__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1250 2023-07-21 06:21:28.000000 aeronet_convert-0.1.0a2/aeronet_convert/rasterize.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5428 2023-07-21 06:21:18.000000 aeronet_convert-0.1.0a2/aeronet_convert/vectorize.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:57:23.660307 aeronet_convert-0.1.0a2/aeronet_convert.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-24 12:57:23.000000 aeronet_convert-0.1.0a2/aeronet_convert.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      330 2023-07-24 12:57:23.000000 aeronet_convert-0.1.0a2/aeronet_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 12:57:23.000000 aeronet_convert-0.1.0a2/aeronet_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       71 2023-07-24 12:57:23.000000 aeronet_convert-0.1.0a2/aeronet_convert.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       16 2023-07-24 12:57:23.000000 aeronet_convert-0.1.0a2/aeronet_convert.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 12:57:23.661277 aeronet_convert-0.1.0a2/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     4373 2023-07-24 09:02:15.000000 aeronet_convert-0.1.0a2/setup.py
```

### Comparing `aeronet_convert-0.1.0a1/PKG-INFO` & `aeronet_convert-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_convert
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_convert-0.1.0a1/README.rst` & `aeronet_convert-0.1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a1/aeronet_convert/rasterize.py` & `aeronet_convert-0.1.0a2/aeronet_convert/rasterize.py`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a1/aeronet_convert/vectorize.py` & `aeronet_convert-0.1.0a2/aeronet_convert/vectorize.py`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a1/aeronet_convert.egg-info/PKG-INFO` & `aeronet_convert-0.1.0a2/aeronet_convert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-convert
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_convert-0.1.0a1/setup.py` & `aeronet_convert-0.1.0a2/setup.py`

 * *Files identical despite different names*

