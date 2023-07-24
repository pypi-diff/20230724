# Comparing `tmp/pygeoops-0.2.0a1.tar.gz` & `tmp/pygeoops-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoops-0.2.0a1.tar", last modified: Sat Jul 22 22:03:44 2023, max compression
+gzip compressed data, was "pygeoops-0.2.0a2.tar", last modified: Mon Jul 24 17:33:39 2023, max compression
```

## Comparing `pygeoops-0.2.0a1.tar` & `pygeoops-0.2.0a2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:03:44.766509 pygeoops-0.2.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-22 22:03:44.766509 pygeoops-0.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:03:44.762508 pygeoops-0.2.0a1/pygeoops/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/_view_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pygeoops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:03:44.762508 pygeoops-0.2.0a1/pygeoops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-22 22:03:44.000000 pygeoops-0.2.0a1/pygeoops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-22 22:03:44.000000 pygeoops-0.2.0a1/pygeoops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 22:03:44.000000 pygeoops-0.2.0a1/pygeoops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-22 22:03:44.000000 pygeoops-0.2.0a1/pygeoops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 22:03:44.000000 pygeoops-0.2.0a1/pygeoops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-22 22:03:44.766509 pygeoops-0.2.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 22:03:44.766509 pygeoops-0.2.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-22 22:03:29.000000 pygeoops-0.2.0a1/tests/test_view_angles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:33:39.501299 pygeoops-0.2.0a2/pygeoops/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_view_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/pygeoops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_view_angles.py
```

### Comparing `pygeoops-0.2.0a1/LICENSE.txt` & `pygeoops-0.2.0a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a1/PKG-INFO` & `pygeoops-0.2.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pygeoops-0.2.0a1/README.md` & `pygeoops-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a1/pygeoops/_centerline.py` & `pygeoops-0.2.0a2/pygeoops/_centerline.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import logging
 import math
 from typing import Optional, Union
-import numpy as np
 
+from geopandas import GeoSeries
+import numpy as np
+from numpy.typing import NDArray
 import shapely
 from shapely.geometry.base import BaseGeometry
 
-
 logger = logging.getLogger(__name__)
 
 
 def centerline(
-    geometry: Union[BaseGeometry, np.ndarray, list, None],
+    geometry,
     densify_distance: float = -1,
     min_branch_length: float = -1,
     simplifytolerance: float = -0.25,
-) -> Union[BaseGeometry, np.ndarray, list, None]:
+) -> Union[BaseGeometry, NDArray[BaseGeometry], GeoSeries, None]:
     """
     Calculates an approximated centerline for a polygon.
 
     Negative values for the algorithm parameters will result in an automatic
     optimisation based on the average geometry width for each input geometry.
 
     Alternative name: medial axis.
 
     Example output:
 
     |centerline_L_shape|
 
     Args:
-        geometry (geometry or array_like): a geometry or ndarray of geometries
+        geometry (geometry, GeoSeries or arraylike): a geometry, GeoSeries or arraylike.
         densify_distance (float, optional): densify input geometry
             so each segment has maximum this length. A reasonable value is the typical
             minimal width of the input geometries. If a larger value is used centerlines
             might have holes on narrow places in the input geometry. The smaller the
             value choosen, the longer the processing will take. Defaults to -1.
 
               - value = 0: no densification
@@ -49,33 +50,38 @@
             centerline (using Douglas-Peucker algoritm). Defaults to -0.25.
 
               - value = 0: no simplify
               - value > 0: simplify with this value as tolerance
               - value < 0: simplifytolerance = average width of geometry * abs(value)
 
     Returns:
-        geometry or array_like: the centerline for each of the input geometries.
+        geometry, GeoSeries or array_like: the centerline for each of the input
+            geometries.
 
     .. |centerline_L_shape| image:: ../_static/images/centerline_fancy_Lshape.png
         :alt: Centerline of a fancy L shaped polygon
     """
     if geometry is None:
         return None
 
     # If input is arraylike, treat every geometry in loop
     if hasattr(geometry, "__len__"):
-        result = [
-            _centerline(
-                geom=geom,
-                densify_distance=densify_distance,
-                min_branch_length=min_branch_length,
-                simplifytolerance=simplifytolerance,
-            )
-            for geom in geometry
-        ]
+        result = np.array(
+            [
+                _centerline(
+                    geom=geom,
+                    densify_distance=densify_distance,
+                    min_branch_length=min_branch_length,
+                    simplifytolerance=simplifytolerance,
+                )
+                for geom in geometry
+            ]
+        )
+        if isinstance(geometry, GeoSeries):
+            result = GeoSeries(result, index=geometry.index, crs=geometry.crs)
         return result
     else:
         return _centerline(
             geom=geometry,
             densify_distance=densify_distance,
             min_branch_length=min_branch_length,
             simplifytolerance=simplifytolerance,
```

### Comparing `pygeoops-0.2.0a1/pygeoops/_general.py` & `pygeoops-0.2.0a2/pygeoops/_general.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-from typing import List, Optional, Union
+from typing import Optional, Union
 
+from geopandas import GeoSeries
+import numpy as np
+from numpy.typing import NDArray
 import pyproj
 import shapely
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 
 from pygeoops._types import GeometryType, PrimitiveType
 
 
 def collect(
-    geometries: Union[BaseGeometry, List[BaseGeometry], None],
+    geometries,
 ) -> Optional[BaseGeometry]:
     """
-    Collects a list of geometries to one geometry.
+    Collects a list of geometries to one (multi)geometry.
 
     Elements in the list that are None or empty geometries are dropped.
 
     Examples:
       * if the list contains only Polygon's, returns a MultiPolygon.
       * if the list contains different types (and Multipolygon != Polygon!), returns a
         GeometryCollection.
 
     Args:
-        geometries (List[BaseGeometry]): arraylike list of geometries to collect to one
-            geometry.
+        geometry (geometry, GeoSeries or arraylike): geometry or arraylike.
 
     Raises:
         ValueError: raises an exception if one of the input geometries is of an
             unknown type.
 
     Returns:
-        BaseGeometry: the result
+        BaseGeometry: the result.
     """
     # If geometry_list is None or no list, just return itself
     if geometries is None:
         return None
     if not hasattr(geometries, "__len__"):
         return geometries
 
@@ -80,38 +82,59 @@
     elif result_collection_type == GeometryType.GEOMETRYCOLLECTION:
         return shapely.GeometryCollection(geometries)
     else:
         raise ValueError(f"Unsupported geometry type: {result_collection_type}")
 
 
 def collection_extract(
-    geometry: Optional[BaseGeometry], primitivetype: PrimitiveType
-) -> Optional[BaseGeometry]:
+    geometry, primitivetype: PrimitiveType
+) -> Union[BaseGeometry, NDArray[BaseGeometry], None]:
     """
-    Extracts the geometries from the input geom that comply with the
+    Extracts the parts from the input geometry/geometries that comply with the
     primitive_type specified and returns them as (Multi)geometry.
 
     Args:
-        geometry (BaseGeometry): geometry to extract the polygons
-            from.
-        primitivetype (GeometryPrimitiveTypes): the primitive type to extract
-            from the input geom.
+        geometry (geometry, GeoSeries or arraylike): geometry or arraylike.
+        primitivetype (GeometryPrimitiveTypes): the primitive type to extract from the
+            input geometry.
 
     Raises:
-        Exception: if in_geom is an unsupported geometry type or the primitive
+        ValueError: if in_geom is an unsupported geometry type or the primitive
             type is invalid.
 
     Returns:
-        BaseGeometry: List of primitive geometries, only
-            containing the primitive type specified.
+        Union[BaseGeometry, NDArray[BaseGeometry], None]: geometry or array of
+            geometries containing only parts of the primitive type specified.
     """
     # Extract the polygons from the multipolygon, but store them as multipolygons anyway
     if geometry is None:
         return None
-    elif isinstance(geometry, (shapely.MultiPoint, shapely.Point)):
+
+    # If input is not arraylike, apply once, otherwise apply to all elements
+    if not hasattr(geometry, "__len__"):
+        return _collection_extract(geometry=geometry, primitivetype=primitivetype)
+    else:
+        result = np.array(
+            [
+                _collection_extract(geometry=geom, primitivetype=primitivetype)
+                for geom in geometry
+            ]
+        )
+        if isinstance(geometry, GeoSeries):
+            result = GeoSeries(result, index=geometry.index, crs=geometry.crs)
+        return result
+
+
+def _collection_extract(
+    geometry: Optional[BaseGeometry], primitivetype: PrimitiveType
+) -> Optional[BaseGeometry]:
+    if geometry is None:
+        return None
+
+    if isinstance(geometry, (shapely.MultiPoint, shapely.Point)):
         if primitivetype == PrimitiveType.POINT:
             return geometry
     elif isinstance(geometry, (shapely.LineString, shapely.MultiLineString)):
         if primitivetype == PrimitiveType.LINESTRING:
             return geometry
     elif isinstance(geometry, (shapely.MultiPolygon, shapely.Polygon)):
         if primitivetype == PrimitiveType.POLYGON:
@@ -122,36 +145,33 @@
             for geometry in shapely.GeometryCollection(geometry).geoms
         ]
         if len(returngeoms) > 0:
             return collect(returngeoms)
     else:
         raise ValueError(f"Invalid/unsupported geometry(type): {geometry}")
 
-    # Nothing found yet, so return None
-    return None
-
 
-def explode(geometry: Optional[BaseGeometry]) -> Optional[List[BaseGeometry]]:
+def explode(geometry: Optional[BaseGeometry]) -> Optional[NDArray[BaseGeometry]]:
     """
     Dump all (multi)geometries in the input to one list of single geometries.
 
     Args:
         geometry (BaseGeometry, optional): geometry to explode.
 
     Returns:
-        Optional[List[BaseGeometry]]: a list of simple geometries or None if the input
+        Optional[NDArray[BaseGeometry]]: array of simple geometries or None if the input
             was None.
 
     """
     if geometry is None:
         return None
     elif isinstance(geometry, BaseMultipartGeometry):
-        return list(geometry.geoms)
+        return np.array(geometry.geoms)
     else:
-        return [geometry]
+        return np.array([geometry])
 
 
 """
 def force_geometrytype(
         geometry: BaseGeometry,
         dest_geometrytype: GeometryType) -> BaseGeometry:
     # Cast to destination geometrytype
```

### Comparing `pygeoops-0.2.0a1/pygeoops/_grid.py` & `pygeoops-0.2.0a2/pygeoops/_grid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,69 @@
 # -*- coding: utf-8 -*-
 """
 Module containing utilities to create/manipulate grids.
 """
 
 import logging
 import math
-from typing import Optional, Tuple, Union
+from typing import Optional, Tuple
+import numpy as np
 
-import geopandas as gpd
-import pyproj
+from numpy.typing import NDArray
+from geopandas import GeoDataFrame
 import shapely
 import shapely.ops
-
-#####################################################################
-# First define/init some general variables/constants
-#####################################################################
+from shapely import Polygon
 
 # Get a logger...
 logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-#####################################################################
-# Grid tile helpers
-#####################################################################
 
 
 def create_grid(
     total_bounds: Tuple[float, float, float, float],
     nb_columns: int,
     nb_rows: int,
-    crs: Union[pyproj.CRS, int, str, None],
-) -> gpd.GeoDataFrame:
+) -> NDArray[Polygon]:
     """
     Creates a grid with tiles of the width and height specified.
 
     Args:
         total_bounds (Tuple[float, float, float, float]): bounds of the grid to be
             created.
         nb_columns (int): number of columns the grid should have.
         nb_rows (int): number of rows the grid should have.
-        crs (Union[pyproj.CRS, int, str, None]): the projection to create the grid in.
 
     Returns:
-        gpd.GeoDataFrame: geodataframe with the grid.
+        NDArray[Polygon]: ndarray with tiles.
     """
     xmin, ymin, xmax, ymax = total_bounds
     width = (xmax - xmin) / nb_columns
     height = (ymax - ymin) / nb_rows
 
-    return create_grid3(total_bounds=total_bounds, width=width, height=height, crs=crs)
+    return create_grid3(total_bounds=total_bounds, width=width, height=height)
 
 
 def create_grid3(
     total_bounds: Tuple[float, float, float, float],
     width: float,
     height: float,
-    crs: Union[pyproj.CRS, int, str, None],
-) -> gpd.GeoDataFrame:
+) -> NDArray[Polygon]:
     """
     Creates a grid with tiles of the width and height specified.
 
     Args:
         total_bounds (Tuple[float, float, float, float]): bounds of the grid to be
             created.
         width (float): width of the tiles.
         height (float): height of the tiles.
-        crs (Union[pyproj.CRS, int, str, None]): the projection to create the grid in.
         number_decimals (int, optional): the number of decimals the coordinates of the
             grid will have. Defaults to None, so no rounding.
 
     Returns:
-        gpd.GeoDataFrame: geodataframe with the grid.
+        NDArray[Polygon]: ndarray with tiles.
     """
 
     xmin, ymin, xmax, ymax = total_bounds
     rows = int(math.ceil((ymax - ymin) / height))
     cols = int(math.ceil((xmax - xmin) / width))
 
     polygons = []
@@ -100,36 +89,34 @@
             )
             cell_top += height
             cell_bottom += height
 
         cell_left += width
         cell_right += width
 
-    return gpd.GeoDataFrame(geometry=polygons, crs=crs)
+    return np.array(polygons)
 
 
 def create_grid2(
     total_bounds: Tuple[float, float, float, float],
     nb_squarish_tiles: int,
-    crs: Union[pyproj.CRS, int, str, None],
     nb_squarish_tiles_max: Optional[int] = None,
-) -> gpd.GeoDataFrame:
+) -> NDArray[Polygon]:
     """
     Creates a grid and tries to approximate the number of cells asked as good as
     possible with grid cells that as close to square as possible.
 
     Args:
         total_bounds (Tuple[float, float, float, float]): bounds of the grid to be
             created.
         nb_squarish_cells (int): about the number of cells wanted.
-        crs (pyproj.CRS, int, str, optional): the projection to create the grid in.
         nb_squarish_tiles_max (int, optional): the maximum number of cells.
 
     Returns:
-        gpd.GeoDataFrame: geodataframe with the grid.
+        NDArray[Polygon]: ndarray with tiles.
     """
     # Check input
     if nb_squarish_tiles <= 0:
         raise ValueError("nb_squarish_tiles should be > 0")
     if nb_squarish_tiles_max is not None:
         if not nb_squarish_tiles_max > 0:
             raise ValueError("nb_squarish_tiles_max should be > 0")
@@ -160,32 +147,31 @@
                 # Cell width is larger than cell height
                 nb_columns -= 1
             else:
                 nb_rows -= 1
 
     # Now we know everything to create the grid
     return create_grid(
-        total_bounds=total_bounds, nb_columns=nb_columns, nb_rows=nb_rows, crs=crs
+        total_bounds=total_bounds, nb_columns=nb_columns, nb_rows=nb_rows
     )
 
 
-def split_tiles(
-    input_tiles: gpd.GeoDataFrame, nb_tiles_wanted: int
-) -> gpd.GeoDataFrame:
+def split_tiles(input_tiles: GeoDataFrame, nb_tiles_wanted: int) -> GeoDataFrame:
     """
     Split the tiles in the input tiles so the number of tiles approaches
-    nb_tiles_wanted specified as close as possible.
+    nb_tiles_wanted specified as close as possible. For tiles that are split, any values
+    in additional attribute columns in the GeoDataFrame will be retainedin the result.
 
     Args:
-        input_tiles (gpd.GeoDataFrame): the input tiles to split.
+        input_tiles (GeoDataFrame): the input tiles to split.
         nb_tiles_wanted (int): the number of tiles wanted in the result.
 
     Returns:
-        gpd.GeoDataFrame: tiles that are the result of splitting input_tiles and
-        approaching nb_tiles_wanted as close as possible.
+        GeoDataFrame: tiles that are the result of splitting input tiles and approaching
+            nb_tiles_wanted as close as possible.
     """
     nb_tiles = len(input_tiles)
     if nb_tiles >= nb_tiles_wanted:
         return input_tiles
 
     nb_tiles_ratio_target = nb_tiles_wanted / nb_tiles
 
@@ -249,9 +235,9 @@
                 )
             curr_tiles_being_split = tmp_tiles_after_split
 
         # Copy the tile parts to the result and retain possible other columns
         for tile_split_part in curr_tiles_being_split:
             result_tiles.append(tile._replace(geometry=tile_split_part))
 
-    # We should be ready...
-    return gpd.GeoDataFrame(data=result_tiles, crs=input_tiles.crs)
+    # We should be ready
+    return GeoDataFrame(data=result_tiles, crs=input_tiles.crs)
```

### Comparing `pygeoops-0.2.0a1/pygeoops/_simplify.py` & `pygeoops-0.2.0a2/pygeoops/_simplify.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,86 +2,110 @@
 """
 Module containing utilities to simplify geometries.
 """
 
 import logging
 from typing import Optional, Union
 
+from geopandas import GeoSeries
 import numpy as np
+from numpy.typing import NDArray
 import shapely
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 import shapely.coords
 
 try:
     import simplification.cutil as simplification
 
     HAS_SIMPLIFICATION = True
 except ImportError:
     HAS_SIMPLIFICATION = False
 
 import pygeoops._general as general
 from pygeoops._general import PrimitiveType
 from pygeoops import _simplify_lang as simplify_lang
+from pygeoops import _simplify_topo as simplify_topo
 
 logger = logging.getLogger(__name__)
 
 
 def simplify(
-    geometry: Union[BaseGeometry, np.ndarray, list, None],
+    geometry,
     tolerance: float,
     algorithm: str = "rdp",
     lookahead: int = 8,
     preserve_topology: bool = True,
+    preserve_common_boundaries=False,
     keep_points_on: Optional[BaseGeometry] = None,
-) -> Union[BaseGeometry, np.ndarray, list, None]:
+) -> Union[BaseGeometry, NDArray[BaseGeometry], GeoSeries, None]:
     """
-    Simplify the geometry.
+    Simplify the geometry/geometries.
 
     Args:
-        geometry (geometry or array_like): a geometry or ndarray of geometries
+        geometry (geometry or array_like): a geometry or ndarray of geometries.
         tolerance (float): mandatory for the following algorithms:
             * "rdp": distance to use as tolerance
             * "lang": distance to use as tolerance
             * "vw": area to use as tolerance
         algorithm (str, optional): algorithm to use. Defaults to "rdp".
             * "rdp": Ramer Douglas Peuker
             * "lang": Lang
             * "vw": Visvalingal Whyatt
         lookahead (int, optional): the number of points to consider for removing
             in a moving window. Used for LANG algorithm. Defaults to 8.
         preserve_topology (bool, optional): True to (try to) return valid
             geometries as result. Defaults to True.
+        preserve_common_bounderies (bool, optional): True to (try to) maintain common
+            boundaries between all geometries in the input geometry list.
+            Defaults to False.
         keep_points_on (BaseGeometry], optional): point of the geometry to
             that intersect with these geometries are not removed. Defaults to None.
 
     Raises:
         Exception: [description]
-        Exception: [description]
-        Exception: [description]
 
     Returns:
-        BaseGeometry: The simplified version of the geometry.
+        Union[BaseGeometry, NDArray[BaseGeometry], GeoSeries, None]: the
+            simplified version of the input geometry/geometries.
     """
     if geometry is None:
         return None
 
-    # Check if input is arraylike
-    if hasattr(geometry, "__len__"):
-        # Treat every geometry
-        result = [
-            _simplify(
-                geometry=geom,
-                tolerance=tolerance,
-                algorithm=algorithm,
-                lookahead=lookahead,
-                preserve_topology=preserve_topology,
-                keep_points_on=keep_points_on,
+    # If common boundaries need to be preserved, use topologic implementation
+    if preserve_common_boundaries:
+        if not preserve_topology:
+            raise ValueError(
+                "The combination of preserve_common_boundaries=True and "
+                "preserve_topology=False is not supported."
             )
-            for geom in geometry
-        ]
+        return simplify_topo.simplify_topo(
+            geometry=geometry,
+            tolerance=tolerance,
+            algorithm=algorithm,
+            lookahead=lookahead,
+            keep_points_on=keep_points_on,
+        )
+
+    # If input is arraylike, apply to all elements
+    if hasattr(geometry, "__len__"):
+        result = np.array(
+            [
+                _simplify(
+                    geometry=geom,
+                    tolerance=tolerance,
+                    algorithm=algorithm,
+                    lookahead=lookahead,
+                    preserve_topology=preserve_topology,
+                    keep_points_on=keep_points_on,
+                )
+                for geom in geometry
+            ]
+        )
+        if isinstance(geometry, GeoSeries):
+            result = GeoSeries(result, index=geometry.index, crs=geometry.crs)
         return result
     else:
         return _simplify(
             geometry=geometry,
             tolerance=tolerance,
             algorithm=algorithm,
             lookahead=lookahead,
```

### Comparing `pygeoops-0.2.0a1/pygeoops/_simplify_lang.py` & `pygeoops-0.2.0a2/pygeoops/_simplify_lang.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a1/pygeoops/_types.py` & `pygeoops-0.2.0a2/pygeoops/_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a1/pygeoops/_view_angles.py` & `pygeoops-0.2.0a2/pygeoops/_view_angles.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
     Remark: the start angle can be larger than the end angle. E.g. if the visible geom
     is located in the south east of the viewpoint till the north east.
 
     |view_angles|
 
     Args:
-        viewpoint (Geometry or arraylike): the point that is being viewed from.
-        visible_geom (Geometry or arraylike): the visible geometry to calculate the view
-            angles to. Only singlepart geometries are supported.
+        viewpoint (Geometry, GeoSeries or arraylike): the point being viewed from.
+        visible_geom (Geometry, GeoSeries or arraylike): the visible geometry to
+            calculate the view angles to. Only singlepart geometries are supported.
 
     Returns:
         Tuple or array of floats with for each viewpoint/visible_geom combination the
         start angle and end angle in degrees. Values are between 0 and 360, or np.nan
         for None or empty geometries.
 
     .. |view_angles| image:: ../_static/images/view_angles.png
```

### Comparing `pygeoops-0.2.0a1/pygeoops.egg-info/PKG-INFO` & `pygeoops-0.2.0a2/pygeoops.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pygeoops-0.2.0a1/pygeoops.egg-info/SOURCES.txt` & `pygeoops-0.2.0a2/pygeoops.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 setup.py
 pygeoops/__init__.py
 pygeoops/_centerline.py
 pygeoops/_general.py
 pygeoops/_grid.py
 pygeoops/_simplify.py
 pygeoops/_simplify_lang.py
+pygeoops/_simplify_topo.py
 pygeoops/_types.py
 pygeoops/_view_angles.py
 pygeoops/version.txt
 pygeoops.egg-info/PKG-INFO
 pygeoops.egg-info/SOURCES.txt
 pygeoops.egg-info/dependency_links.txt
 pygeoops.egg-info/requires.txt
 pygeoops.egg-info/top_level.txt
 tests/test_centerline.py
 tests/test_general.py
-tests/test_geopandas.py
 tests/test_grid.py
 tests/test_helper.py
 tests/test_simplify.py
 tests/test_simplify_lang.py
+tests/test_simplify_topo.py
 tests/test_types.py
 tests/test_view_angles.py
```

### Comparing `pygeoops-0.2.0a1/pyproject.toml` & `pygeoops-0.2.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoops"
-version = "0.2.0a1"
+version = "0.2.0a2"
 authors = [
   { name="Pieter Roggemans", email="pieter.roggemans@gmail.com" },
 ]
 description = "Library with some less common or extended spatial functions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "shapely>1",
     "geopandas",
+    "shapely>1",
+    "topojson",
 ]
 keywords = ["GIS", "cartography", "pandas", "shapely", "geopandas"]
 
 [project.urls]
 "Homepage" = "https://github.com/pygeoops/pygeoops"
 "Bug Tracker" = "https://github.com/pygeoops/pygeoops/issues"
```

### Comparing `pygeoops-0.2.0a1/tests/test_general.py` & `pygeoops-0.2.0a2/tests/test_general.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Tests for functionalities in vector_util, regarding geometry operations.
 """
 
+import geopandas as gpd
+import numpy as np
 import pytest
 import shapely
 
 import pygeoops
 from pygeoops import PrimitiveType
 
 
@@ -49,19 +51,25 @@
     assert pygeoops.collect([geometrycoll, line]) == shapely.GeometryCollection(
         [geometrycoll, line]
     )
     assert pygeoops.collect([poly, multipoly]) == shapely.GeometryCollection(
         [poly, multipoly]
     )
 
+    # Test arraylike input
+    # --------------------
+    assert pygeoops.collect(gpd.GeoSeries([point, line, poly])) == geometrycoll
+    assert pygeoops.collect(np.array([point, line, poly])) == geometrycoll
+
 
 def test_collection_extract():
     # Test None input
     # ---------------
     assert pygeoops.collection_extract(None, PrimitiveType.POINT) is None
+    assert pygeoops.collection_extract([None], PrimitiveType.POINT) == [None]
 
     # Test dealing with points
     # ------------------------
     point = shapely.Point((0, 0))
     multipoint = shapely.MultiPoint([point, point])
     assert pygeoops.collection_extract(point, PrimitiveType.POINT) == point
     assert pygeoops.collection_extract(multipoint, PrimitiveType.POINT) == multipoint
@@ -76,44 +84,84 @@
     assert pygeoops.collection_extract(geometrycoll, PrimitiveType.POINT) == point
     assert pygeoops.collection_extract(geometrycoll, PrimitiveType.LINESTRING) == line
     assert pygeoops.collection_extract(
         geometrycoll, PrimitiveType.POLYGON
     ) == shapely.GeometryCollection([poly, multipoly])
 
 
+@pytest.mark.parametrize("input_type", ["geoseries", "ndarray", "list"])
+def test_collection_extract_geometries(input_type):
+    """
+    Test collection_extract with several geometries as input.
+    """
+    # Prepare test data
+    point = shapely.Point((0, 0))
+    multipoint = shapely.MultiPoint([point, point])
+    line = shapely.LineString([(0, 0), (0, 1)])
+    poly = shapely.Polygon([(0, 0), (0, 1), (0, 0)])
+    multipoly = shapely.MultiPolygon([poly, poly])
+    geometrycoll = shapely.GeometryCollection([point, line, poly, multipoly])
+    input = [point, multipoint, line, poly, multipoly, geometrycoll]
+    start_idx = 0
+    if input_type == "geoseries":
+        # For geoseries, also check if the indexers are retained!
+        start_idx = 5
+        input = gpd.GeoSeries(
+            input, index=[index + start_idx for index in range(len(input))]
+        )
+    elif input_type == "ndarray":
+        input = np.array(input)
+
+    # Run test
+    result = pygeoops.collection_extract(input, primitivetype=PrimitiveType.POINT)
+
+    # Check result
+    assert result is not None
+    if input_type == "geoseries":
+        assert isinstance(result, gpd.GeoSeries)
+    else:
+        assert isinstance(result, np.ndarray)
+    assert result[start_idx] == point
+    assert result[start_idx + 1] == multipoint
+    assert result[start_idx + 2] is None
+    assert result[start_idx + 3] is None
+    assert result[start_idx + 4] is None
+    assert result[start_idx + 5] == point
+
+
 def test_explode():
     # Test dealing with None/empty input
     # ----------------------------------
     assert pygeoops.explode(None) is None
 
     # Test dealing with points
     # ------------------------
     point = shapely.Point((0, 0))
     multipoint = shapely.MultiPoint([point, point])
-    assert pygeoops.explode(point) == [point]
-    assert pygeoops.explode(multipoint) == [point, point]
+    assert pygeoops.explode(point).tolist() == [point]
+    assert pygeoops.explode(multipoint).tolist() == [point, point]
 
     # Test dealing with linestrings
     # -----------------------------
     line = shapely.LineString([(0, 0), (0, 1)])
     multiline = shapely.MultiLineString([line, line])
-    assert pygeoops.explode(line) == [line]
-    assert pygeoops.explode(multiline) == [line, line]
+    assert pygeoops.explode(line).tolist() == [line]
+    assert pygeoops.explode(multiline).tolist() == [line, line]
 
     # Test dealing with Polygons
     # --------------------------
     poly = shapely.Polygon([(0, 0), (0, 1), (0, 0)])
     multipoly = shapely.MultiPolygon([poly, poly])
-    assert pygeoops.explode(poly) == [poly]
-    assert pygeoops.explode(multipoly) == [poly, poly]
+    assert pygeoops.explode(poly).tolist() == [poly]
+    assert pygeoops.explode(multipoly).tolist() == [poly, poly]
 
     # Test geometrycollection
     # -----------------------
     geometrycoll = shapely.GeometryCollection([point, line, poly])
-    assert pygeoops.explode(geometrycoll) == [point, line, poly]
+    assert pygeoops.explode(geometrycoll).tolist() == [point, line, poly]
 
 
 def test_remove_inner_rings():
     # Test with None input
     assert pygeoops.remove_inner_rings(None, min_area_to_keep=1, crs=None) is None
 
     # Apply to single Polygon, with area tolerance smaller than holes
```

### Comparing `pygeoops-0.2.0a1/tests/test_grid.py` & `pygeoops-0.2.0a2/tests/test_grid.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 # -*- coding: utf-8 -*-
 """
 Tests for functionalities in _grid.py.
 """
 
+import geopandas as gpd
+import numpy as np
 import pytest
 
 import pygeoops
 
 
 def test_create_grid():
-    grid_gdf = pygeoops.create_grid(
-        total_bounds=(40000.0, 160000.0, 45000.0, 210000.0),
-        nb_columns=2,
-        nb_rows=2,
-        crs="epsg:31370",
+    grid = pygeoops.create_grid(
+        total_bounds=(40000.0, 160000.0, 45000.0, 210000.0), nb_columns=2, nb_rows=2
     )
-    assert len(grid_gdf) == 4
+    assert grid is not None
+    assert isinstance(grid, np.ndarray)
+    assert len(grid) == 4
 
 
 def test_create_grid2():
     # Test for small number of cells
     for i in range(1, 10):
-        grid_gdf = pygeoops.create_grid2(
-            total_bounds=(40000.0, 160000.0, 45000.0, 210000.0),
-            nb_squarish_tiles=i,
-            crs="epsg:31370",
+        grid = pygeoops.create_grid2(
+            total_bounds=(40000.0, 160000.0, 45000.0, 210000.0), nb_squarish_tiles=i
         )
-        assert len(grid_gdf) == i
+        assert grid is not None
+        assert isinstance(grid, np.ndarray)
+        assert len(grid) == i
 
     # Test for larger number of cells
-    grid_gdf = pygeoops.create_grid2(
-        total_bounds=(40000.0, 160000.0, 45000.0, 210000.0),
-        nb_squarish_tiles=100,
-        crs="epsg:31370",
+    grid = pygeoops.create_grid2(
+        total_bounds=(40000.0, 160000.0, 45000.0, 210000.0), nb_squarish_tiles=100
     )
-    assert len(grid_gdf) == 96
+    assert grid is not None
+    assert isinstance(grid, np.ndarray)
+    assert len(grid) == 96
 
     # Test for larger number of cells + nb_squarish_tiles_max
     # Remark: without nb_squarish_tiles_max, nb_squarish_tiles=150 results in 156 tiles
-    grid_gdf = pygeoops.create_grid2(
+    grid = pygeoops.create_grid2(
         total_bounds=(40000.0, 160000.0, 45000.0, 210000.0),
         nb_squarish_tiles=150,
         nb_squarish_tiles_max=150,
-        crs="epsg:31370",
     )
-    assert len(grid_gdf) == 148
+    assert grid is not None
+    assert isinstance(grid, np.ndarray)
+    assert len(grid) == 148
 
 
 @pytest.mark.parametrize(
     "exp_error, nb_squarish_tiles, nb_squarish_tiles_max",
     [
         ("nb_squarish_tiles_max should be > 0", 1, 0),
         ("nb_squarish_tiles_max should be >= nb_squarich_tiles", 4, 3),
@@ -60,27 +62,27 @@
 ):
     # Test for invalid number of nb_squarish_tiles_max
     with pytest.raises(ValueError, match=exp_error):
         _ = pygeoops.create_grid2(
             total_bounds=(40000.0, 160000.0, 45000.0, 210000.0),
             nb_squarish_tiles=nb_squarish_tiles,
             nb_squarish_tiles_max=nb_squarish_tiles_max,
-            crs="epsg:31370",
         )
 
 
 def test_create_grid3():
     bounds = (40000.0, 160000.0, 45000.0, 210000.0)
-    grid_gdf = pygeoops.create_grid3(
+    grid = pygeoops.create_grid3(
         total_bounds=bounds,
         width=(bounds[2] - bounds[0]) / 2,
         height=(bounds[3] - bounds[1]) / 2,
-        crs="epsg:31370",
     )
-    assert len(grid_gdf) == 4
+    assert grid is not None
+    assert isinstance(grid, np.ndarray)
+    assert len(grid) == 4
 
 
 @pytest.mark.parametrize(
     "bounds, nb_input_tiles, nb_tiles_wanted, exp_tiles",
     [
         ((40, 40, 45, 46), 4, 8, 8),
         ((40, 40, 45, 46), 4, 12, 12),
@@ -89,19 +91,31 @@
         ((40, 40, 45, 45), 4, 2, 4),
     ],
 )
 def test_split_tiles(bounds, nb_input_tiles, nb_tiles_wanted, exp_tiles):
     # Prepare test data
     nb_input_tiles = 4
     input_tiles = pygeoops.create_grid2(
-        total_bounds=bounds,
-        nb_squarish_tiles=nb_input_tiles,
-        crs="epsg:31370",
+        total_bounds=bounds, nb_squarish_tiles=nb_input_tiles
     )
     assert len(input_tiles) == nb_input_tiles
+    names = {"name": ["foo", "bar", "spam", "ni"]}
 
     # Test split_tiles
-    result = pygeoops.split_tiles(input_tiles, nb_tiles_wanted)
+    input_tiles_gdf = gpd.GeoDataFrame(
+        data=names, geometry=input_tiles, crs="epsg:31370"
+    )
+    result_gdf = pygeoops.split_tiles(input_tiles_gdf, nb_tiles_wanted)
 
-    assert len(result) == exp_tiles
+    # Check result
+    assert result_gdf is not None
+    assert isinstance(result_gdf, gpd.GeoDataFrame)
+    assert len(result_gdf) == exp_tiles
+    # Attribute column data should be retained when a tile is split
+    assert "name" in result_gdf.columns
+    assert (
+        len(result_gdf[result_gdf.name == "spam"])
+        / len(input_tiles_gdf[input_tiles_gdf.name == "spam"])
+        == exp_tiles / nb_input_tiles
+    )
     # Total area of tiles should stay the same after split
-    assert input_tiles.geometry.area.sum() == result.geometry.area.sum()
+    assert input_tiles_gdf.geometry.area.sum() == result_gdf.geometry.area.sum()
```

### Comparing `pygeoops-0.2.0a1/tests/test_helper.py` & `pygeoops-0.2.0a2/tests/test_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     figure = mpl_figure.Figure()
     figure.subplots(1, 1)
     if title is not None:
         figure.suptitle(title)
 
     colors = mcolors.TABLEAU_COLORS
     for geom_idx, geom in enumerate(geoms):
-        if geom.is_empty:
+        if geom is None or geom.is_empty:
             continue
 
         color = colors[list(colors.keys())[geom_idx % len(colors)]]
         if isinstance(geom, (shapely.MultiPolygon, shapely.Polygon)):
             shapely.plotting.plot_polygon(geom, ax=figure.axes[0], color=color)
         elif isinstance(geom, (shapely.LineString, shapely.MultiLineString)):
             shapely.plotting.plot_line(geom, ax=figure.axes[0], color=color)
```

### Comparing `pygeoops-0.2.0a1/tests/test_simplify.py` & `pygeoops-0.2.0a2/tests/test_simplify.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 Tests on simplify.
 """
 
+import geopandas as gpd
+import numpy as np
 import pytest
 import shapely
 
 import pygeoops
 import test_helper
 
 
-def test_simplify_arr():
-    """Test simplify of an array of linestrings."""
-    linestrings = [shapely.LineString([(0, 0), (10, 10), (20, 20)])] * 2
-    simplified_lines = pygeoops.simplify(
-        geometry=linestrings, algorithm="lang", tolerance=1
-    )
-    assert simplified_lines is not None
-    assert len(simplified_lines) == 2
-    for test_idx, simplified_line in enumerate(simplified_lines):
-        assert isinstance(simplified_line, shapely.LineString)
-        assert len(simplified_line.coords) < len(linestrings[test_idx].coords)
-        assert len(simplified_line.coords) == 2
-
-
 def test_simplify_basic_lang():
     """
     Some basic tests of simplify. The lang algorithm is used because it is no optional
     dependency.
     """
     # Test LineString, lookahead -1, via geometry
     linestring = shapely.LineString([(0, 0), (10, 10), (20, 20)])
@@ -133,14 +121,68 @@
         [point, multipoint, linestring, multilinestring, poly, multipoly]
     )
     geom_simplified = pygeoops.simplify(geometry=geom, algorithm="lang", tolerance=1)
     assert isinstance(geom_simplified, shapely.GeometryCollection)
     assert len(geom_simplified.geoms) == 6
 
 
+@pytest.mark.parametrize("input_type", ["geoseries", "ndarray", "list"])
+def test_simplify_input_geometries(input_type):
+    """Test simplify of an array of linestrings."""
+    # Prepare test data
+    input = [shapely.LineString([(0, 0), (10, 10), (20, 20)])] * 2
+    start_idx = 0
+    if input_type == "geoseries":
+        # For geoseries, also check if the indexers are retained!
+        start_idx = 5
+        input = gpd.GeoSeries(
+            input, index=[index + start_idx for index in range(len(input))]
+        )
+    elif input_type == "ndarray":
+        input = np.array(input)
+
+    # Run test
+    result = pygeoops.simplify(geometry=input, algorithm="lang", tolerance=1)
+
+    # Check result
+    assert result is not None
+    if input_type == "geoseries":
+        assert isinstance(result, gpd.GeoSeries)
+    else:
+        assert isinstance(result, np.ndarray)
+    assert len(result) == 2
+    for test_idx, simplified_line in enumerate(result):
+        assert isinstance(simplified_line, shapely.LineString)
+        assert len(simplified_line.coords) < len(input[start_idx + test_idx].coords)
+        assert len(simplified_line.coords) == 2
+
+
+@pytest.mark.parametrize("preserve_common_boundaries", [True, False])
+def test_simplify_input_geoseries(preserve_common_boundaries: bool):
+    """Test simplify of a geoseries of linestrings."""
+    line1 = shapely.LineString([(0, 0), (10, 10), (20, 20)])
+    line2 = shapely.LineString([(0, 0), (10, 0), (20, 0)])
+    lines_gs = gpd.GeoSeries([line1, line2, line2])
+    lines_gs = lines_gs.drop(index=1)
+    simplified_lines_gs = pygeoops.simplify(
+        geometry=lines_gs,
+        algorithm="lang",
+        tolerance=1,
+        preserve_common_boundaries=preserve_common_boundaries,
+    )
+    assert simplified_lines_gs is not None
+    assert isinstance(simplified_lines_gs, gpd.GeoSeries)
+    assert len(simplified_lines_gs) == len(lines_gs)
+    assert simplified_lines_gs.index.to_list() == lines_gs.index.to_list()
+    for test_idx, simplified_line in simplified_lines_gs.items():
+        assert isinstance(simplified_line, shapely.LineString)
+        assert len(simplified_line.coords) < len(lines_gs.geometry[test_idx].coords)
+        assert len(simplified_line.coords) == 2
+
+
 def test_simplify_invalid_geometry():
     # Test Polygon simplification, with invalid exterior ring
     poly = shapely.Polygon(
         shell=[(0, 0), (0, 10), (5, 10), (3, 12), (3, 9), (10, 10), (10, 0), (0, 0)],
         holes=[[(2, 2), (2, 8), (8, 8), (8, 2), (2, 2)]],
     )
     geom_simplified = pygeoops.simplify(geometry=poly, algorithm="lang", tolerance=1)
@@ -214,14 +256,26 @@
     with pytest.raises(ValueError, match="Unsupported algorythm specified: invalid!"):
         pygeoops.simplify(
             geometry=shapely.LineString([(0, 0), (10, 10), (20, 20)]),
             tolerance=1,
             algorithm="invalid!",
         )
 
+    expected_error = (
+        "The combination of preserve_common_boundaries=True and "
+        "preserve_topology=False is not supported."
+    )
+    with pytest.raises(ValueError, match=expected_error):
+        pygeoops.simplify(
+            geometry=shapely.LineString([(0, 0), (10, 10), (20, 20)]),
+            tolerance=1,
+            preserve_topology=False,
+            preserve_common_boundaries=True,
+        )
+
 
 @pytest.mark.parametrize("algorithm, tolerance", [("lang", 2), ("rdp", 2), ("vw", 15)])
 def test_simplify_keep_points_on(tmp_path, algorithm, tolerance):
     # Skip test if simplification is not available
     _ = pytest.importorskip("simplification")
 
     # Prepare test data
@@ -269,26 +323,26 @@
 
 def test_simplify_preservetopology_lang():
     # Test Polygon lookahead -1
     poly = shapely.Polygon(
         shell=[(0, 0), (0, 10), (1, 10), (10, 10), (10, 0), (0, 0)],
         holes=[[(2, 2), (2, 8), (8, 8), (8, 2), (2, 2)]],
     )
-    # If preserve_topology True, the original polygon is returned...
+    # If preserve_topology True, the original polygon is returned
     geom_simplified = pygeoops.simplify(
         geometry=poly,
         algorithm="lang",
         tolerance=10,
         preserve_topology=True,
         lookahead=-1,
     )
     assert isinstance(geom_simplified, shapely.Polygon)
     assert poly.equals(geom_simplified) is True
 
-    # If preserve_topology True, the original polygon is returned...
+    # If preserve_topology False, the polygon becomes None
     geom_simplified = pygeoops.simplify(
         geometry=poly,
         algorithm="lang",
         tolerance=10,
         preserve_topology=False,
         lookahead=-1,
     )
```

### Comparing `pygeoops-0.2.0a1/tests/test_simplify_lang.py` & `pygeoops-0.2.0a2/tests/test_simplify_lang.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a1/tests/test_types.py` & `pygeoops-0.2.0a2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a1/tests/test_view_angles.py` & `pygeoops-0.2.0a2/tests/test_view_angles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Tuple
 
+from geopandas import GeoSeries
 import numpy as np
 import pytest
 import shapely
 import shapely.affinity
 from shapely import from_wkt
 
 import pygeoops
@@ -111,37 +112,45 @@
     with pytest.raises(
         ValueError,
         match="viewpoint and visible_geom are arrays, so they must be the same length",
     ):
         pygeoops.view_angles([shapely.Point(), shapely.Point()], [shapely.Polygon()])
 
 
-def test_view_angles_arraylike():
+@pytest.mark.parametrize("input_type", ["geoseries", "ndarray", "list"])
+def test_view_angles_geometries(input_type):
     """
-    Test view_angles with arraylike input(s).
+    Test view_angles with input(s) > 1 geometry.
     """
     viewpoint, visible_geoms, expected_angles = get_testdata()
+    if input_type == "geoseries":
+        visible_geoms = GeoSeries(visible_geoms)
+    elif input_type == "ndarray":
+        visible_geoms = np.array(visible_geoms)
 
     # Run test with viewpoint a Point and visible_geoms an array
     # ----------------------------------------------------------
     angles_arr = pygeoops.view_angles(viewpoint, visible_geoms)
 
     # Compare expected results
+    assert isinstance(angles_arr, np.ndarray)
     assert np.array_equal(angles_arr, np.array(expected_angles), equal_nan=True)
 
     # Run test with viewpoint + visible_goms as an array
     # --------------------------------------------------
     viewpoint_arr = np.array([viewpoint for i in range(len(visible_geoms))])
     angles_arr = pygeoops.view_angles(viewpoint_arr, visible_geoms)
 
     # Compare expected results
+    assert isinstance(angles_arr, np.ndarray)
     assert np.array_equal(angles_arr, np.array(expected_angles), equal_nan=True)
 
     # Run test with viewpoint an array and visible_geoms a single geometry
     # --------------------------------------------------------------------
     viewpoint_arr = np.array([viewpoint for i in range(len(visible_geoms))])
     visible_geom = visible_geoms[3]
     angles_arr = pygeoops.view_angles(viewpoint_arr, visible_geom)
 
     # Compare expected results
+    assert isinstance(angles_arr, np.ndarray)
     exp_angles_arr = np.full((len(viewpoint_arr), 2), expected_angles[3])
     assert np.array_equal(angles_arr, exp_angles_arr, equal_nan=True)
```

