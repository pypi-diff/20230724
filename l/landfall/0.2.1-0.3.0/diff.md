# Comparing `tmp/landfall-0.2.1.tar.gz` & `tmp/landfall-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landfall-0.2.1.tar", last modified: Mon Jul 24 15:03:08 2023, max compression
+gzip compressed data, was "landfall-0.3.0.tar", last modified: Mon Jul 24 18:56:20 2023, max compression
```

## Comparing `landfall-0.2.1.tar` & `landfall-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 15:03:08.553761 landfall-0.2.1/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.2.1/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-24 15:03:08.553911 landfall-0.2.1/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1348 2023-07-21 17:24:03.000000 landfall-0.2.1/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.2.1/pyproject.toml
--rw-r--r--   0 odosmatthews   (501) staff       (20)      871 2023-07-24 15:03:08.555961 landfall-0.2.1/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-02-28 17:08:57.000000 landfall-0.2.1/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 15:03:08.527670 landfall-0.2.1/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 15:03:08.542930 landfall-0.2.1/src/landfall/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      121 2023-07-24 15:01:36.000000 landfall-0.2.1/src/landfall/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.2.1/src/landfall/color.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.2.1/src/landfall/colorsys.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.2.1/src/landfall/distinctipy.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2550 2023-07-21 17:37:15.000000 landfall-0.2.1/src/landfall/points.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 15:03:08.553401 landfall-0.2.1/src/landfall.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      388 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.2.1/src/landfall.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      156 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 18:56:20.780232 landfall-0.3.0/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.0/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-24 18:56:20.780382 landfall-0.3.0/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1348 2023-07-21 17:24:03.000000 landfall-0.3.0/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.0/pyproject.toml
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      871 2023-07-24 18:56:20.781624 landfall-0.3.0/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-02-28 17:08:57.000000 landfall-0.3.0/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 18:56:20.767212 landfall-0.3.0/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 18:56:20.775134 landfall-0.3.0/src/landfall/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      179 2023-07-24 18:55:40.000000 landfall-0.3.0/src/landfall/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.3.0/src/landfall/color.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.0/src/landfall/colorsys.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.0/src/landfall/combos.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.3.0/src/landfall/distinctipy.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     3057 2023-07-24 18:54:52.000000 landfall-0.3.0/src/landfall/points.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2213 2023-07-24 18:49:22.000000 landfall-0.3.0/src/landfall/polygons.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 18:56:20.779926 landfall-0.3.0/src/landfall.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-24 18:56:20.000000 landfall-0.3.0/src/landfall.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      436 2023-07-24 18:56:20.000000 landfall-0.3.0/src/landfall.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-24 18:56:20.000000 landfall-0.3.0/src/landfall.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.0/src/landfall.egg-info/not-zip-safe
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      156 2023-07-24 18:56:20.000000 landfall-0.3.0/src/landfall.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-24 18:56:20.000000 landfall-0.3.0/src/landfall.egg-info/top_level.txt
```

### Comparing `landfall-0.2.1/LICENSE` & `landfall-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `landfall-0.2.1/PKG-INFO` & `landfall-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.2.1
+Version: 0.3.0
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `landfall-0.2.1/README.md` & `landfall-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `landfall-0.2.1/setup.cfg` & `landfall-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = landfall
-version = 0.2.1
+version = 0.3.0
 description = Easy to use functions to plot geospatial data on maps using staticmaps.
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `landfall-0.2.1/src/landfall/color.py` & `landfall-0.3.0/src/landfall/color.py`

 * *Files identical despite different names*

### Comparing `landfall-0.2.1/src/landfall/colorsys.py` & `landfall-0.3.0/src/landfall/colorsys.py`

 * *Files identical despite different names*

### Comparing `landfall-0.2.1/src/landfall/points.py` & `landfall-0.3.0/src/landfall/points.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Functions for plotting points.
 """
-
 from pprint import pprint
 from typing import Mapping, Optional, Sequence, Union
 from itertools import repeat
 
 import staticmaps
 from PIL.Image import Image
 
@@ -39,17 +38,15 @@
 
     if ids is not None and id_colors is not None:
         colors = process_id_colors(ids, id_colors)
         color_mapping = {color.int_rgb(): ids for color, ids in zip(colors, ids)}
         pprint(color_mapping)
 
     for lat, lon, clr in zip(latitudes, longitudes, colors):
-        point = staticmaps.create_latlng(lat, lon)
-        marker = staticmaps.Marker(point, color=clr, size=point_size)
-        context.add_object(marker)
+        add_point(context, lat, lon, clr, point_size)
 
     _, _zoom = context.determine_center_zoom(*window_size)
     if _zoom is not None:
         context.set_zoom(_zoom + zoom)
 
     if set_zoom is not None:
         context.set_zoom(set_zoom)
@@ -86,8 +83,31 @@
         ids=ids_values,
         id_colors=id_colors,
         tile_provider=tile_provider,
         point_size=point_size,
         window_size=window_size,
         zoom=zoom,
         color=color,
-        set_zoom=set_zoom)
+        set_zoom=set_zoom)
+
+
+def add_point(
+    context: staticmaps.Context,
+    lat: float,
+    lon: float,
+    color: staticmaps.Color,
+    point_size: int
+) -> None:
+    point = staticmaps.create_latlng(lat, lon)
+    marker = staticmaps.Marker(point, color=color, size=point_size)
+    context.add_object(marker)
+
+
+def add_points(
+        context: staticmaps.Context,
+        latitudes: Sequence[float],
+        longitudes: Sequence[float],
+        colors: Sequence[staticmaps.Color],
+        point_size: int
+) -> None:
+    for lat, lon, clr in zip(latitudes, longitudes, colors):
+        add_point(context, lat, lon, clr, point_size)
```

### Comparing `landfall-0.2.1/src/landfall.egg-info/PKG-INFO` & `landfall-0.3.0/src/landfall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.2.1
+Version: 0.3.0
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

