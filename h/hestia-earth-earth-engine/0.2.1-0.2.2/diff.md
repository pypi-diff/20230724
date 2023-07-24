# Comparing `tmp/hestia-earth-earth-engine-0.2.1.tar.gz` & `tmp/hestia-earth-earth-engine-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-earth-engine-0.2.1.tar", last modified: Mon Apr 10 12:40:53 2023, max compression
+gzip compressed data, was "hestia-earth-earth-engine-0.2.2.tar", last modified: Mon Jul 24 14:29:36 2023, max compression
```

## Comparing `hestia-earth-earth-engine-0.2.1.tar` & `hestia-earth-earth-engine-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.482087 hestia-earth-earth-engine-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1851 2023-04-10 12:40:53.482087 hestia-earth-earth-engine-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.473087 hestia-earth-earth-engine-0.2.1/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.475087 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/
--rw-rw-rw-   0 root         (0) root         (0)     2515 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.476087 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2347 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.477087 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.477087 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5917 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gee_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/log.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.479087 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1851 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-10 12:40:53.000000 hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 12:40:53.482087 hestia-earth-earth-engine-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.471087 hestia-earth-earth-engine-0.2.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.480087 hestia-earth-earth-engine-0.2.1/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.480087 hestia-earth-earth-engine-0.2.1/tests/integration/boundary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/boundary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2051 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/boundary/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.481087 hestia-earth-earth-engine-0.2.1/tests/integration/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/coordinates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/coordinates/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:40:53.482087 hestia-earth-earth-engine-0.2.1/tests/integration/gadm/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/gadm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2086 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/gadm/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-10 12:40:29.000000 hestia-earth-earth-engine-0.2.1/tests/integration/test_gee_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.313655 hestia-earth-earth-engine-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-07-24 14:29:36.312654 hestia-earth-earth-engine-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.308654 hestia-earth-earth-engine-0.2.2/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.309654 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.309654 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/boundary/
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/boundary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/boundary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.309654 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/coordinates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/coordinates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.310654 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/gadm/
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/gadm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/gadm/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6198 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/gee_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.311654 hestia-earth-earth-engine-0.2.2/hestia_earth_earth_engine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-07-24 14:29:36.000000 hestia-earth-earth-engine-0.2.2/hestia_earth_earth_engine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-07-24 14:29:36.000000 hestia-earth-earth-engine-0.2.2/hestia_earth_earth_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:29:36.000000 hestia-earth-earth-engine-0.2.2/hestia_earth_earth_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-24 14:29:36.000000 hestia-earth-earth-engine-0.2.2/hestia_earth_earth_engine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 14:29:36.000000 hestia-earth-earth-engine-0.2.2/hestia_earth_earth_engine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 14:29:36.313655 hestia-earth-earth-engine-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.306654 hestia-earth-earth-engine-0.2.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.311654 hestia-earth-earth-engine-0.2.2/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.311654 hestia-earth-earth-engine-0.2.2/tests/integration/boundary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/tests/integration/boundary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/tests/integration/boundary/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.312654 hestia-earth-earth-engine-0.2.2/tests/integration/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/tests/integration/coordinates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/tests/integration/coordinates/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:29:36.312654 hestia-earth-earth-engine-0.2.2/tests/integration/gadm/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/tests/integration/gadm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/tests/integration/gadm/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-24 14:29:18.000000 hestia-earth-earth-engine-0.2.2/tests/integration/test_gee_utils.py
```

### Comparing `hestia-earth-earth-engine-0.2.1/LICENSE` & `hestia-earth-earth-engine-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/PKG-INFO` & `hestia-earth-earth-engine-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-earth-engine
-Version: 0.2.1
+Version: 0.2.2
 Summary: Hestia's earth engine.
 Home-page: https://gitlab.com/hestia-earth/hestia-earth-engine
 Author: Hestia Team
 Author-email: guillaume@hestia.earth
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-earth-engine-0.2.1/README.md` & `hestia-earth-earth-engine-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/__init__.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,22 @@
 
 __path__ = extend_path(__path__, __name__)
 
 EE_ACCOUNT_ID = os.getenv('EARTH_ENGINE_ACCOUNT_ID')
 EE_KEY_FILE = os.getenv('EARTH_ENGINE_KEY_FILE', 'ee-credentials.json')
 
 
-def init_gee():
+def init_gee(high_volume: bool = False):
     now = current_time_ms()
     logger.debug(f"initializing ee using {EE_KEY_FILE}...")
-    ee.Initialize(ee.ServiceAccountCredentials(EE_ACCOUNT_ID, EE_KEY_FILE))
+    opt_url = 'https://earthengine-highvolume.googleapis.com' if high_volume else 'https://earthengine.googleapis.com'
+    ee.Initialize(
+        credentials=ee.ServiceAccountCredentials(EE_ACCOUNT_ID, EE_KEY_FILE),
+        opt_url=opt_url
+    )
     logger.debug(f"done initializing ee in {current_time_ms() - now} ms")
 
 
 class RunType(Enum):
     BOUNDARY = 'boundary'
     COORDINATES = 'coordinates'
     GADM = 'gadm'
```

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/__init__.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/boundary/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/boundary/utils.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/boundary/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/__init__.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/coordinates/utils.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/coordinates/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ee
 
 from hestia_earth.earth_engine.utils import get_param, get_required_param, get_fields_from_params
 from hestia_earth.earth_engine.gee_utils import (
-    clean_collection, data_from_raster, data_from_raster_by_period, defaut_scale
+    get_point, clean_collection, data_from_raster, data_from_raster_by_period, defaut_scale
 )
 
 
 def _data_from_vector(point: ee.Geometry, collection: str, params: dict):
     fields = get_fields_from_params(params)
     collection = ee.FeatureCollection(collection).filterBounds(point)
     return clean_collection(collection, fields)
@@ -38,9 +38,9 @@
     'vector': _data_from_vector,
     'raster': _data_from_raster,
     'raster_by_period': _data_from_point_by_period
 }
 
 
 def load(collection: str, ee_type: str, coordinates, params: dict):
-    geometry = ee.Geometry.Point(coordinates) if isinstance(coordinates, list) else coordinates
+    geometry = get_point(coordinates) if isinstance(coordinates, list) else coordinates
     return DATA_BY_TYPE[ee_type](geometry, collection, params)
```

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/__init__.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/gadm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import ee
-
 from hestia_earth.earth_engine.utils import get_required_param
-from hestia_earth.earth_engine.gee_utils import load_region, area_km2
+from hestia_earth.earth_engine.gee_utils import load_region, area_km2, get_point
 from hestia_earth.earth_engine.coordinates import _load_single as load_coordinates
 from .utils import load
 
 
 def _load_single(geometry, data: dict):
     collection = get_required_param(data, 'collection')
     ee_type = get_required_param(data, 'ee_type')
@@ -42,15 +40,25 @@
 
 
 def get_distance_to_coordinates(gadm_id: str, latitude: float, longitude: float):
     """
     Returns the distance between the coordinates and the GADM region, in meters.
     """
     region = load_region(gadm_id)
-    coordinates = ee.Geometry.Point(longitude, latitude)
+    coordinates = get_point(longitude=longitude, latitude=latitude)
     return region.geometry().distance(coordinates).getInfo()
 
 
+def get_id_by_coordinates(level: int, latitude: float, longitude: float):
+    """
+    Returns the GADM ID of the closest region to the coordinates by level (0 to 5).
+    """
+    collection = load_region(level=level)
+    coordinates = get_point(longitude=longitude, latitude=latitude)
+    region = collection.filterBounds(coordinates).first()
+    return region.get(f"GID_{level}").getInfo()
+
+
 def run(data: dict):
     region = _get_region(data)
     use_centroid = str(data.get('centroid', 'false')).lower() == 'true'
     return _load_centroid(region.geometry().centroid(), data) if use_centroid else _load_region(region, data)
```

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gadm/utils.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/gadm/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/gee_utils.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/gee_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,23 @@
 
 def _date_year(date: str): return int(date.split('-')[0])
 
 
 def _id_to_level(id: str): return id.count('.')
 
 
-def load_region(gadm_id: str):
-    level = _id_to_level(gadm_id)
-    id = gadm_id.replace('GADM-', '')
-    return ee.FeatureCollection(f"{GADM_COLLECTION_PREFIX}{level}").filterMetadata(f"GID_{level}", 'equals', id)
+def load_region(gadm_id: str = '', level: int = None):
+    collection = ee.FeatureCollection(f"{GADM_COLLECTION_PREFIX}{level or _id_to_level(gadm_id)}")
+    return collection.filterMetadata(
+        f"GID_{_id_to_level(gadm_id)}", 'equals', gadm_id.replace('GADM-', '')
+    ) if gadm_id else collection
+
+
+def get_point(coordinates: list = None, longitude: float = None, latitude: float = None):
+    return ee.Geometry.Point(coordinates) if coordinates else ee.Geometry.Point(longitude, latitude)
 
 
 def defaut_scale(image: ee.Image, band_name: str = None, default: int = 1):
     try:
         band_name = band_name or image.bandNames().getInfo()[0]
     except Exception:
         ''
```

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/log.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth/earth_engine/utils.py` & `hestia-earth-earth-engine-0.2.2/hestia_earth/earth_engine/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/PKG-INFO` & `hestia-earth-earth-engine-0.2.2/hestia_earth_earth_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-earth-engine
-Version: 0.2.1
+Version: 0.2.2
 Summary: Hestia's earth engine.
 Home-page: https://gitlab.com/hestia-earth/hestia-earth-engine
 Author: Hestia Team
 Author-email: guillaume@hestia.earth
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-earth-engine-0.2.1/hestia_earth_earth_engine.egg-info/SOURCES.txt` & `hestia-earth-earth-engine-0.2.2/hestia_earth_earth_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/setup.py` & `hestia-earth-earth-engine-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/tests/integration/boundary/test_utils.py` & `hestia-earth-earth-engine-0.2.2/tests/integration/boundary/test_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/tests/integration/coordinates/test_utils.py` & `hestia-earth-earth-engine-0.2.2/tests/integration/coordinates/test_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.2.1/tests/integration/gadm/test_utils.py` & `hestia-earth-earth-engine-0.2.2/tests/integration/gadm/test_utils.py`

 * *Files identical despite different names*

