# Comparing `tmp/aeronet_convert-0.1.0a3.tar.gz` & `tmp/aeronet_convert-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_convert-0.1.0a3.tar", last modified: Mon Jul 24 13:13:25 2023, max compression
+gzip compressed data, was "aeronet_convert-0.1.0a4.tar", last modified: Mon Jul 24 13:30:40 2023, max compression
```

## Comparing `aeronet_convert-0.1.0a3.tar` & `aeronet_convert-0.1.0a4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:25.491258 aeronet_convert-0.1.0a3/
--rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-24 13:13:25.490908 aeronet_convert-0.1.0a3/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     2053 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a3/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:25.488647 aeronet_convert-0.1.0a3/aeronet_convert/
--rw-r--r--   0 trekin     (501) staff       (20)       67 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a3/aeronet_convert/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 13:12:37.000000 aeronet_convert-0.1.0a3/aeronet_convert/__version__.py
--rw-r--r--   0 trekin     (501) staff       (20)     1250 2023-07-21 06:21:28.000000 aeronet_convert-0.1.0a3/aeronet_convert/rasterize.py
--rw-r--r--   0 trekin     (501) staff       (20)     5428 2023-07-21 06:21:18.000000 aeronet_convert-0.1.0a3/aeronet_convert/vectorize.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:25.490439 aeronet_convert-0.1.0a3/aeronet_convert.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-24 13:13:25.000000 aeronet_convert-0.1.0a3/aeronet_convert.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      330 2023-07-24 13:13:25.000000 aeronet_convert-0.1.0a3/aeronet_convert.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 13:13:25.000000 aeronet_convert-0.1.0a3/aeronet_convert.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       71 2023-07-24 13:13:25.000000 aeronet_convert-0.1.0a3/aeronet_convert.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       16 2023-07-24 13:13:25.000000 aeronet_convert-0.1.0a3/aeronet_convert.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 13:13:25.491356 aeronet_convert-0.1.0a3/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     4373 2023-07-24 09:02:15.000000 aeronet_convert-0.1.0a3/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:40.774163 aeronet_convert-0.1.0a4/
+-rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-24 13:30:40.773807 aeronet_convert-0.1.0a4/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     2053 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a4/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:40.771411 aeronet_convert-0.1.0a4/aeronet_convert/
+-rw-r--r--   0 trekin     (501) staff       (20)       67 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a4/aeronet_convert/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 13:30:18.000000 aeronet_convert-0.1.0a4/aeronet_convert/__version__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1250 2023-07-21 06:21:28.000000 aeronet_convert-0.1.0a4/aeronet_convert/rasterize.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5428 2023-07-21 06:21:18.000000 aeronet_convert-0.1.0a4/aeronet_convert/vectorize.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:40.773280 aeronet_convert-0.1.0a4/aeronet_convert.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-24 13:30:40.000000 aeronet_convert-0.1.0a4/aeronet_convert.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      330 2023-07-24 13:30:40.000000 aeronet_convert-0.1.0a4/aeronet_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 13:30:40.000000 aeronet_convert-0.1.0a4/aeronet_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       71 2023-07-24 13:30:40.000000 aeronet_convert-0.1.0a4/aeronet_convert.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       16 2023-07-24 13:30:40.000000 aeronet_convert-0.1.0a4/aeronet_convert.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 13:30:40.774273 aeronet_convert-0.1.0a4/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     4373 2023-07-24 09:02:15.000000 aeronet_convert-0.1.0a4/setup.py
```

### Comparing `aeronet_convert-0.1.0a3/PKG-INFO` & `aeronet_convert-0.1.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_convert
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_convert-0.1.0a3/README.rst` & `aeronet_convert-0.1.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a3/aeronet_convert/rasterize.py` & `aeronet_convert-0.1.0a4/aeronet_convert/rasterize.py`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a3/aeronet_convert/vectorize.py` & `aeronet_convert-0.1.0a4/aeronet_convert/vectorize.py`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a3/aeronet_convert.egg-info/PKG-INFO` & `aeronet_convert-0.1.0a4/aeronet_convert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-convert
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_convert-0.1.0a3/setup.py` & `aeronet_convert-0.1.0a4/setup.py`

 * *Files identical despite different names*

