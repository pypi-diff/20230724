# Comparing `tmp/aeronet_raster-0.1.0a2.tar.gz` & `tmp/aeronet_raster-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_raster-0.1.0a2.tar", last modified: Mon Jul 24 12:47:02 2023, max compression
+gzip compressed data, was "aeronet_raster-0.1.0a3.tar", last modified: Mon Jul 24 13:13:24 2023, max compression
```

## Comparing `aeronet_raster-0.1.0a2.tar` & `aeronet_raster-0.1.0a3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.698657 aeronet_raster-0.1.0a2/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 12:47:02.698133 aeronet_raster-0.1.0a2/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.687009 aeronet_raster-0.1.0a2/aeronet_raster/
--rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 12:46:25.000000 aeronet_raster-0.1.0a2/aeronet_raster/__version__.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.692253 aeronet_raster-0.1.0a2/aeronet_raster/band/
--rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/band/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/band/band.py
--rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/band/bandsample.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.694244 aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/
--rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     7413 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/bandcollection.py
--rw-r--r--   0 trekin     (501) staff       (20)     5936 2023-07-21 14:48:40.000000 aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/bandcollectionsample.py
--rw-r--r--   0 trekin     (501) staff       (20)    10666 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/collectionprocessor.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.695586 aeronet_raster-0.1.0a2/aeronet_raster/geoobject/
--rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/geoobject/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/geoobject/geoobject.py
--rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/merge.py
--rw-r--r--   0 trekin     (501) staff       (20)     5705 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/split.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.697329 aeronet_raster-0.1.0a2/aeronet_raster/utils/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/utils/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a2/aeronet_raster/utils/coords.py
--rw-r--r--   0 trekin     (501) staff       (20)     1790 2023-07-24 12:45:43.000000 aeronet_raster-0.1.0a2/aeronet_raster/utils/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 12:47:02.690261 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-24 12:47:02.000000 aeronet_raster-0.1.0a2/aeronet_raster.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 12:47:02.698848 aeronet_raster-0.1.0a2/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a2/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:24.549836 aeronet_raster-0.1.0a3/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 13:13:24.548196 aeronet_raster-0.1.0a3/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:24.535620 aeronet_raster-0.1.0a3/aeronet_raster/
+-rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 13:12:38.000000 aeronet_raster-0.1.0a3/aeronet_raster/__version__.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:24.541167 aeronet_raster-0.1.0a3/aeronet_raster/band/
+-rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/band/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/band/band.py
+-rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/band/bandsample.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:24.543307 aeronet_raster-0.1.0a3/aeronet_raster/bandcollection/
+-rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/bandcollection/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     7413 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/bandcollection/bandcollection.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5936 2023-07-21 14:48:40.000000 aeronet_raster-0.1.0a3/aeronet_raster/bandcollection/bandcollectionsample.py
+-rw-r--r--   0 trekin     (501) staff       (20)    10679 2023-07-24 13:11:22.000000 aeronet_raster-0.1.0a3/aeronet_raster/collectionprocessor.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:24.544670 aeronet_raster-0.1.0a3/aeronet_raster/geoobject/
+-rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/geoobject/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/geoobject/geoobject.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/merge.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5729 2023-07-24 13:07:04.000000 aeronet_raster-0.1.0a3/aeronet_raster/split.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:24.546533 aeronet_raster-0.1.0a3/aeronet_raster/utils/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/utils/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a3/aeronet_raster/utils/coords.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1790 2023-07-24 13:11:22.000000 aeronet_raster-0.1.0a3/aeronet_raster/utils/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:13:24.539034 aeronet_raster-0.1.0a3/aeronet_raster.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 13:13:24.000000 aeronet_raster-0.1.0a3/aeronet_raster.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-24 13:13:24.000000 aeronet_raster-0.1.0a3/aeronet_raster.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 13:13:24.000000 aeronet_raster-0.1.0a3/aeronet_raster.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-24 13:13:24.000000 aeronet_raster-0.1.0a3/aeronet_raster.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-24 13:13:24.000000 aeronet_raster-0.1.0a3/aeronet_raster.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 13:13:24.550073 aeronet_raster-0.1.0a3/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a3/setup.py
```

### Comparing `aeronet_raster-0.1.0a2/PKG-INFO` & `aeronet_raster-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_raster
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a2/README.rst` & `aeronet_raster-0.1.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/band/band.py` & `aeronet_raster-0.1.0a3/aeronet_raster/band/band.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/band/bandsample.py` & `aeronet_raster-0.1.0a3/aeronet_raster/band/bandsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/bandcollection.py` & `aeronet_raster-0.1.0a3/aeronet_raster/bandcollection/bandcollection.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/bandcollection/bandcollectionsample.py` & `aeronet_raster-0.1.0a3/aeronet_raster/bandcollection/bandcollectionsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/collectionprocessor.py` & `aeronet_raster-0.1.0a3/aeronet_raster/collectionprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import numpy as np
 import rasterio
 from multiprocessing.pool import ThreadPool
 from threading import Lock
 from tqdm import tqdm
 from .band.band import Band
 from .bandcollection.bandcollection import BandCollection
-from typing import Union, Optional, Callable
+from typing import Union, Optional, Callable, List, Tuple
 
 
 class SequentialSampler:
 
     def __init__(self,
                  band_collection: BandCollection,
-                 channels: list[str],
+                 channels: List[str],
                  sample_size: Union[int, tuple, list],
                  bound: int = 0):
         """ Iterate over BandCollection sequentially with specified shape (+ bounds)
         Args:
             band_collection: BandCollection instance
             channels: list of str, required channels with required order
             sample_size: (height, width), size of `pure` sample in pixels (bounds not included)
@@ -40,15 +40,15 @@
     def __getitem__(self, i: int) -> tuple:
         block = self.blocks[i]
         sample = (self.band_collection
                   .ordered(*self.channels)
                   .sample(block['y'], block['x'], block['height'], block['width']))
         return sample, block
 
-    def _compute_blocks(self) -> list[dict]:
+    def _compute_blocks(self) -> List[dict]:
 
         h, w = self.sample_size
         blocks = []
         height = h + 2 * self.bound
         width = w + 2 * self.bound
 
         for y in range(- self.bound, self.band_collection.height, h):
@@ -147,15 +147,15 @@
             width = width - bounds[1][1] - bounds[1][0]
             height = height - bounds[0][1] - bounds[0][0]
         self.dst.write(raster, 1, window=((y, y + height), (x, x + width)))
 
 
 class SampleCollectionWindowWriter:
 
-    def __init__(self, directory: str, channels: list[str], shape: tuple[int],
+    def __init__(self, directory: str, channels: List[str], shape: Tuple[int],
                  transform, crs, nodata: int, dtype: str = 'uint8'):
         """ Create empty `Band` (rasterio open file) and write blocks sequentially
         Args:
             directory: directory path of created BandCollection
             channels: channel names of created BandCollection
             shape: (height, width), size of band in pixels
             transform: rasterio Affine object
@@ -211,16 +211,16 @@
     def close(self) -> BandCollection:
         bands = [w.close() for w in self.writers]
         return BandCollection(bands)
 
 
 class CollectionProcessor:
 
-    def __init__(self, input_channels: list[str], output_labels: list[str], processing_fn: Callable,
-                 sample_size: tuple[int] = (1024, 1024), bound: int = 256,
+    def __init__(self, input_channels: List[str], output_labels: List[str], processing_fn: Callable,
+                 sample_size: Tuple[int] = (1024, 1024), bound: int = 256,
                  n_workers: int = 1, verbose: bool = True, **kwargs):
         """
         Args:
             input_channels: list of str, names of bands/channels
             output_labels: list of str, names of output classes
             processing_fn: callable, function that take as an input `SampleCollection`
                 and return raster with shape (output_labels, H, W)
```

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/geoobject/geoobject.py` & `aeronet_raster-0.1.0a3/aeronet_raster/geoobject/geoobject.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/merge.py` & `aeronet_raster-0.1.0a3/aeronet_raster/merge.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/split.py` & `aeronet_raster-0.1.0a3/aeronet_raster/split.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
+import rasterio
 import numpy as np
 from tqdm import tqdm
-import rasterio
+from typing import List
 from rasterio.windows import Window
 from rasterio.enums import MaskFlags, ColorInterp
 from .bandcollection.bandcollection import BandCollection
 
 
-def _check_channels_num(src, channels: list[str],
+def _check_channels_num(src, channels: List[str],
                         dst_channels: int, allow_singleband: bool) -> bool:
     src_channels = src.count
     singleband = allow_singleband and \
                  (src_channels == 1 or (src_channels == 2 and src.colorinterp[1] == ColorInterp.alpha))
     # we can handle real singleband images and with alpha channel
 
     if src_channels < dst_channels:
@@ -74,15 +75,15 @@
             yield (Window(col_off=x, row_off=y,
                           width=min(window_width, dataset_width-x),
                           height=min(window_height, dataset_height-y)))
 
 
 def split(src_fp: str,
           dst_fp: str,
-          channels: list[str],
+          channels: List[str],
           exist_ok: bool = True,
           allow_singleband: bool = True,
           window_size: int = 10000):
     """Split multi-band tiff to separate bands
     This is necessary to prepare the source multi-band data for use with the BandCollection
     Args:
         src_fp: file path to multi-band tiff
```

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/utils/coords.py` & `aeronet_raster-0.1.0a3/aeronet_raster/utils/coords.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster/utils/utils.py` & `aeronet_raster-0.1.0a3/aeronet_raster/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import random
 import numpy as np
 
 TMP_DIR: Final[str] = '/tmp/raster'
 
 
 def parse_directory(directory: str, names: Tuple[str],
-                    extensions: Tuple[str] = ('tif', 'tiff', 'TIF', 'TIFF')) -> list[str]:
+                    extensions: Tuple[str] = ('tif', 'tiff', 'TIF', 'TIFF')) -> List[str]:
     """
     Extract necessary filenames
     Args:
         directory: str
         names: tuple of str, band or file names, e.g. ['RED', '101']
         extensions: tuple of str, allowable file extensions
```

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster.egg-info/PKG-INFO` & `aeronet_raster-0.1.0a3/aeronet_raster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-raster
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a2/aeronet_raster.egg-info/SOURCES.txt` & `aeronet_raster-0.1.0a3/aeronet_raster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a2/setup.py` & `aeronet_raster-0.1.0a3/setup.py`

 * *Files identical despite different names*

