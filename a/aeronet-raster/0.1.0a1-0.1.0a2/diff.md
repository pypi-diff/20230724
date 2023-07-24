# Comparing `tmp/aeronet_raster-0.1.0a1.tar.gz` & `tmp/aeronet_raster-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_raster-0.1.0a1.tar", last modified: Mon Jul 24 09:42:51 2023, max compression
+gzip compressed data, was "aeronet_raster-0.1.0a2.tar", last modified: Mon Jul 24 12:47:02 2023, max compression
```

## Comparing `aeronet_raster-0.1.0a1.tar` & `aeronet_raster-0.1.0a2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.107635 aeronet_raster-0.1.0a1/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 09:42:51.107202 aeronet_raster-0.1.0a1/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.099171 aeronet_raster-0.1.0a1/aeronet_raster/
--rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 09:38:11.000000 aeronet_raster-0.1.0a1/aeronet_raster/__version__.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.102441 aeronet_raster-0.1.0a1/aeronet_raster/band/
--rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/band/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/band/band.py
--rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/band/bandsample.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.103523 aeronet_raster-0.1.0a1/aeronet_raster/bandcollection/
--rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/bandcollection/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     7413 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/bandcollection/bandcollection.py
--rw-r--r--   0 trekin     (501) staff       (20)     5936 2023-07-21 14:48:40.000000 aeronet_raster-0.1.0a1/aeronet_raster/bandcollection/bandcollectionsample.py
--rw-r--r--   0 trekin     (501) staff       (20)    10666 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/collectionprocessor.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.104328 aeronet_raster-0.1.0a1/aeronet_raster/geoobject/
--rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/geoobject/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/geoobject/geoobject.py
--rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/merge.py
--rw-r--r--   0 trekin     (501) staff       (20)     5705 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/split.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.106223 aeronet_raster-0.1.0a1/aeronet_raster/utils/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/utils/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/utils/coords.py
--rw-r--r--   0 trekin     (501) staff       (20)     1783 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a1/aeronet_raster/utils/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.101338 aeronet_raster-0.1.0a1/aeronet_raster.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 09:42:51.000000 aeronet_raster-0.1.0a1/aeronet_raster.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-24 09:42:51.000000 aeronet_raster-0.1.0a1/aeronet_raster.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 09:42:51.000000 aeronet_raster-0.1.0a1/aeronet_raster.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-24 09:42:51.000000 aeronet_raster-0.1.0a1/aeronet_raster.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-24 09:42:51.000000 aeronet_raster-0.1.0a1/aeronet_raster.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 09:42:51.107807 aeronet_raster-0.1.0a1/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a1/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.698657 aeronet_raster-0.1.0a2/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 12:47:02.698133 aeronet_raster-0.1.0a2/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.687009 aeronet_raster-0.1.0a2/aeronet_raster/
+-rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 12:46:25.000000 aeronet_raster-0.1.0a2/aeronet_raster/__version__.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.692253 aeronet_raster-0.1.0a2/aeronet_raster/band/
+-rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/band/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/band/band.py
+-rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/band/bandsample.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.694244 aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/
+-rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     7413 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/bandcollection.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5936 2023-07-21 14:48:40.000000 aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/bandcollectionsample.py
+-rw-r--r--   0 trekin     (501) staff       (20)    10666 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/collectionprocessor.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.695586 aeronet_raster-0.1.0a2/aeronet_raster/geoobject/
+-rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/geoobject/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/geoobject/geoobject.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/merge.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5705 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/split.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.697329 aeronet_raster-0.1.0a2/aeronet_raster/utils/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/utils/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/utils/coords.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1790 2023-07-24 12:45:43.000000 aeronet_raster-0.1.0a2/aeronet_raster/utils/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.690261 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 12:47:02.698848 aeronet_raster-0.1.0a2/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a2/setup.py
```

### Comparing `aeronet_raster-0.1.0a1/PKG-INFO` & `aeronet_raster-0.1.0a2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_raster
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a1/README.rst` & `aeronet_raster-0.1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/band/band.py` & `aeronet_raster-0.1.0a2/aeronet_raster/band/band.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/band/bandsample.py` & `aeronet_raster-0.1.0a2/aeronet_raster/band/bandsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/bandcollection/bandcollection.py` & `aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/bandcollection.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/bandcollection/bandcollectionsample.py` & `aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/bandcollectionsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/collectionprocessor.py` & `aeronet_raster-0.1.0a2/aeronet_raster/collectionprocessor.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/geoobject/geoobject.py` & `aeronet_raster-0.1.0a2/aeronet_raster/geoobject/geoobject.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/merge.py` & `aeronet_raster-0.1.0a2/aeronet_raster/merge.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/split.py` & `aeronet_raster-0.1.0a2/aeronet_raster/split.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/utils/coords.py` & `aeronet_raster-0.1.0a2/aeronet_raster/utils/coords.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster/utils/utils.py` & `aeronet_raster-0.1.0a2/aeronet_raster/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import re
 import glob
 from warnings import warn
-from typing import Final
+from typing import Final, Tuple
 import string
 import random
 import numpy as np
 
 TMP_DIR: Final[str] = '/tmp/raster'
 
 
-def parse_directory(directory: str, names: tuple[str],
-                    extensions: tuple[str] = ('tif', 'tiff', 'TIF', 'TIFF')) -> list[str]:
+def parse_directory(directory: str, names: Tuple[str],
+                    extensions: Tuple[str] = ('tif', 'tiff', 'TIF', 'TIFF')) -> list[str]:
     """
     Extract necessary filenames
     Args:
         directory: str
         names: tuple of str, band or file names, e.g. ['RED', '101']
         extensions: tuple of str, allowable file extensions
```

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster.egg-info/PKG-INFO` & `aeronet_raster-0.1.0a2/aeronet_raster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-raster
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a1/aeronet_raster.egg-info/SOURCES.txt` & `aeronet_raster-0.1.0a2/aeronet_raster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a1/setup.py` & `aeronet_raster-0.1.0a2/setup.py`

 * *Files identical despite different names*

