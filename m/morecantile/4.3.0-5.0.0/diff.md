# Comparing `tmp/morecantile-4.3.0.tar.gz` & `tmp/morecantile-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morecantile-4.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "morecantile-5.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `morecantile-4.3.0.tar` & `morecantile-5.0.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0      215 2023-07-11 20:41:39.883545 morecantile-4.3.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1817 2023-07-11 20:41:39.883545 morecantile-4.3.0/.gitignore
--rw-r--r--   0        0        0      822 2023-07-11 20:41:39.883545 morecantile-4.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-07-11 20:41:39.883545 morecantile-4.3.0/LICENSE
--rw-r--r--   0        0        0     5305 2023-07-11 20:41:39.883545 morecantile-4.3.0/README.md
--rw-r--r--   0        0        0      436 2023-07-11 20:41:39.883545 morecantile-4.3.0/morecantile/__init__.py
--rw-r--r--   0        0        0     1015 2023-07-11 20:41:39.883545 morecantile-4.3.0/morecantile/commons.py
--rw-r--r--   0        0        0     7267 2023-07-11 20:41:39.883545 morecantile-4.3.0/morecantile/data/CanadianNAD83_LCC.json
--rw-r--r--   0        0        0     4679 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/EuropeanETRS89_LAEAQuad.json
--rw-r--r--   0        0        0     5176 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/LINZAntarticaMapTilegrid.json
--rw-r--r--   0        0        0     8457 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/NZTM2000Quad.json
--rw-r--r--   0        0        0      242 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/README.md
--rw-r--r--   0        0        0     7374 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/UPSAntarcticWGS84Quad.json
--rw-r--r--   0        0        0     7365 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/UPSArcticWGS84Quad.json
--rw-r--r--   0        0        0     7367 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/UTM31WGS84Quad.json
--rw-r--r--   0        0        0     6932 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/WGS1984Quad.json
--rw-r--r--   0        0        0     7843 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/WebMercatorQuad.json
--rw-r--r--   0        0        0     7072 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/WorldCRS84Quad.json
--rw-r--r--   0        0        0     7001 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/data/WorldMercatorWGS84Quad.json
--rw-r--r--   0        0        0     1748 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/defaults.py
--rw-r--r--   0        0        0      907 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/errors.py
--rw-r--r--   0        0        0    42119 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/models.py
--rw-r--r--   0        0        0        0 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/py.typed
--rw-r--r--   0        0        0       23 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/scripts/__init__.py
--rw-r--r--   0        0        0    16657 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/scripts/cli.py
--rw-r--r--   0        0        0     3364 2023-07-11 20:41:39.887544 morecantile-4.3.0/morecantile/utils.py
--rw-r--r--   0        0        0     2300 2023-07-11 20:41:39.887544 morecantile-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     6737 1970-01-01 00:00:00.000000 morecantile-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0      215 2023-07-24 14:10:23.602322 morecantile-5.0.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1817 2023-07-24 14:10:23.602322 morecantile-5.0.0/.gitignore
+-rw-r--r--   0        0        0      705 2023-07-24 14:10:23.602322 morecantile-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-07-24 14:10:23.602322 morecantile-5.0.0/LICENSE
+-rw-r--r--   0        0        0     5484 2023-07-24 14:10:23.602322 morecantile-5.0.0/README.md
+-rw-r--r--   0        0        0      436 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/__init__.py
+-rw-r--r--   0        0        0     1015 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/commons.py
+-rw-r--r--   0        0        0    36115 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/data/CDB1GlobalGrid.json
+-rw-r--r--   0        0        0     7267 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/data/CanadianNAD83_LCC.json
+-rw-r--r--   0        0        0     4679 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/data/EuropeanETRS89_LAEAQuad.json
+-rw-r--r--   0        0        0    74685 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/data/GNOSISGlobalGrid.json
+-rw-r--r--   0        0        0     5176 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/data/LINZAntarticaMapTilegrid.json
+-rw-r--r--   0        0        0     8457 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/data/NZTM2000Quad.json
+-rw-r--r--   0        0        0      242 2023-07-24 14:10:23.602322 morecantile-5.0.0/morecantile/data/README.md
+-rw-r--r--   0        0        0     7374 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/data/UPSAntarcticWGS84Quad.json
+-rw-r--r--   0        0        0     7365 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/data/UPSArcticWGS84Quad.json
+-rw-r--r--   0        0        0     7367 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/data/UTM31WGS84Quad.json
+-rw-r--r--   0        0        0     6932 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/data/WGS1984Quad.json
+-rw-r--r--   0        0        0     7843 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/data/WebMercatorQuad.json
+-rw-r--r--   0        0        0     7072 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/data/WorldCRS84Quad.json
+-rw-r--r--   0        0        0     7001 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/data/WorldMercatorWGS84Quad.json
+-rw-r--r--   0        0        0     1804 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/defaults.py
+-rw-r--r--   0        0        0      907 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/errors.py
+-rw-r--r--   0        0        0    46277 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/models.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/py.typed
+-rw-r--r--   0        0        0       23 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/scripts/__init__.py
+-rw-r--r--   0        0        0    16657 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/scripts/cli.py
+-rw-r--r--   0        0        0     3364 2023-07-24 14:10:23.606322 morecantile-5.0.0/morecantile/utils.py
+-rw-r--r--   0        0        0     2334 2023-07-24 14:10:23.606322 morecantile-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 morecantile-5.0.0/PKG-INFO
```

### Comparing `morecantile-4.3.0/.gitignore` & `morecantile-5.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/.pre-commit-config.yaml` & `morecantile-5.0.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -19,16 +19,14 @@
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: v0.0.238
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.4.1
     hooks:
       - id: mypy
         language_version: python
-        # No reason to run if only tests have changed. They intentionally break typing.
-        exclude: tests/.*
         additional_dependencies:
         - types-attrs
-        - types-cachetools
+        - pydantic~=2.0
```

### Comparing `morecantile-4.3.0/LICENSE` & `morecantile-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/README.md` & `morecantile-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,17 @@
 
 Morecantile is like [mercantile](https://github.com/mapbox/mercantile) (the best tool to work with Web Mercator tile indexes), but with support for other TileMatrixSet grids.
 
 **Morecantile** follows the **OGC Two Dimensional Tile Matrix Set** specification **2.0** found in [https://docs.ogc.org/is/17-083r4/17-083r4.html](https://docs.ogc.org/is/17-083r4/17-083r4.html)
 
 | Morecantile Version | OGC Specification Version | Link
 | ------------------- | ------------------------- |---------
-| 4.0                 | 2.0                       | https://docs.ogc.org/is/17-083r4/17-083r4.html
-| 3.0 and earlier     | 1.0                       | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html
+| >=4.0               | 2.0                       | https://docs.ogc.org/is/17-083r4/17-083r4.html
+| =<3.0               | 1.0                       | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html
 
-**Note**: Variable matrix width tile set are not supported.
 
 ## Install
 
 ```bash
 $ python -m pip install -U pip
 $ python -m pip install morecantile
 
@@ -88,28 +87,32 @@
 )
 ```
 
 More info can be found at https://developmentseed.org/morecantile/usage/
 
 ### Defaults Grids
 
-`morecantile` provides a set of default TMS grids:
+`morecantile` provides a set of default TileMatrixSets:
 
+- **CDB1GlobalGrid** \*: CDB 1 Global Grid - EPGS:4326 (WGS84)
 - **CanadianNAD83_LCC**: Lambert conformal conic NAD83 for Canada - EPSG:3978
 - **EuropeanETRS89_LAEAQuad**: ETRS89-extended / LAEA Europe - EPGS:3035
+- **GNOSISGlobalGrid** \*: GNOSIS Global Grid - EPGS:4326 (WGS84)
 - **LINZAntarticaMapTilegrid**: LINZ Antarctic Map Tile Grid (Ross Sea Region) - EPSG:5482
 - **NZTM2000Quad**: LINZ NZTM2000 Map Tile Grid - EPSG:2193
 - **UPSAntarcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for Antarctic - EPSG:5042
 - **UPSArcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for Arctic - EPSG:5041
 - **UTM31WGS84Quad**: Example of UTM grid - EPSG:32631
 - **WebMercatorQuad**: Spherical Mercator - EPGS:3857 (default grid for Web Mercator based maps)
 - **WGS1984Quad**: EPSG:4326 for the World - EPGS:4326 (WGS84)
 - **WorldCRS84Quad**: CRS84 for the World
 - **WorldMercatorWGS84Quad**: Elliptical Mercator projection - EPGS:3395
 
+\* TileMatrixSets with variable Matrix Width (see https://docs.ogc.org/is/17-083r4/17-083r4.html#toc15)
+
 ref: https://schemas.opengis.net/tms/2.0/json/examples/tilematrixset/
 
 ## Implementations
 
 - [rio-tiler](https://github.com/cogeotiff/rio-tiler): Create tile from raster using Morecantile TMS.
 - [titiler](https://github.com/developmentseed/titiler): A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
 - [tipg](https://github.com/developmentseed/tipg): OGC Features and Tiles API.
```

#### html2text {}

```diff
@@ -7,46 +7,49 @@
 Code**: https://github.com/developmentseed/morecantile --- Morecantile is like
 [mercantile](https://github.com/mapbox/mercantile) (the best tool to work with
 Web Mercator tile indexes), but with support for other TileMatrixSet grids.
 **Morecantile** follows the **OGC Two Dimensional Tile Matrix Set**
 specification **2.0** found in [https://docs.ogc.org/is/17-083r4/17-083r4.html]
 (https://docs.ogc.org/is/17-083r4/17-083r4.html) | Morecantile Version | OGC
 Specification Version | Link | ------------------- | ------------------------
-- |--------- | 4.0 | 2.0 | https://docs.ogc.org/is/17-083r4/17-083r4.html | 3.0
-and earlier | 1.0 | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html
-**Note**: Variable matrix width tile set are not supported. ## Install ```bash
-$ python -m pip install -U pip $ python -m pip install morecantile # Or install
-from source: $ python -m pip install -U pip $ python -m pip install git+https:/
-/github.com/developmentseed/morecantile.git ``` ## Usage ```python import
-morecantile tms = morecantile.tms.get("WebMercatorQuad") # Get TMS bounding box
-print(tms.xy_bbox) >>> BoundingBox( left=-20037508.342789244, bottom=-
-20037508.34278919, right=20037508.34278919, top=20037508.342789244, ) # Get the
-bounds for tile Z=4, X=10, Y=10 in the TMS's CRS (e.g epsg:3857) print
-(tms.xy_bounds(morecantile.Tile(10, 10, 4))) >>> BoundingBox
-( left=5009377.085697308, bottom=-7514065.628545959, right=7514065.628545959,
-top=-5009377.085697308, ) # Get the bounds for tile Z=4, X=10, Y=10 in
-Geographic CRS (e.g epsg:4326) print(tms.bounds(morecantile.Tile(10, 10, 4)))
->>> BoundingBox( left=44.999999999999964, bottom=-55.776573018667634,
-right=67.4999999999999, top=-40.97989806962009, ) ``` More info can be found at
-https://developmentseed.org/morecantile/usage/ ### Defaults Grids `morecantile`
-provides a set of default TMS grids: - **CanadianNAD83_LCC**: Lambert conformal
-conic NAD83 for Canada - EPSG:3978 - **EuropeanETRS89_LAEAQuad**: ETRS89-
-extended / LAEA Europe - EPGS:3035 - **LINZAntarticaMapTilegrid**: LINZ
-Antarctic Map Tile Grid (Ross Sea Region) - EPSG:5482 - **NZTM2000Quad**: LINZ
-NZTM2000 Map Tile Grid - EPSG:2193 - **UPSAntarcticWGS84Quad**: Universal Polar
-Stereographic WGS 84 Quad for Antarctic - EPSG:5042 - **UPSArcticWGS84Quad**:
-Universal Polar Stereographic WGS 84 Quad for Arctic - EPSG:5041 -
-**UTM31WGS84Quad**: Example of UTM grid - EPSG:32631 - **WebMercatorQuad**:
-Spherical Mercator - EPGS:3857 (default grid for Web Mercator based maps) -
-**WGS1984Quad**: EPSG:4326 for the World - EPGS:4326 (WGS84) -
-**WorldCRS84Quad**: CRS84 for the World - **WorldMercatorWGS84Quad**:
-Elliptical Mercator projection - EPGS:3395 ref: https://schemas.opengis.net/
-tms/2.0/json/examples/tilematrixset/ ## Implementations - [rio-tiler](https://
-github.com/cogeotiff/rio-tiler): Create tile from raster using Morecantile TMS.
-- [titiler](https://github.com/developmentseed/titiler): A modern dynamic tile
+- |--------- | >=4.0 | 2.0 | https://docs.ogc.org/is/17-083r4/17-083r4.html |
+=<3.0 | 1.0 | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html ##
+Install ```bash $ python -m pip install -U pip $ python -m pip install
+morecantile # Or install from source: $ python -m pip install -U pip $ python -
+m pip install git+https://github.com/developmentseed/morecantile.git ``` ##
+Usage ```python import morecantile tms = morecantile.tms.get("WebMercatorQuad")
+# Get TMS bounding box print(tms.xy_bbox) >>> BoundingBox( left=-
+20037508.342789244, bottom=-20037508.34278919, right=20037508.34278919,
+top=20037508.342789244, ) # Get the bounds for tile Z=4, X=10, Y=10 in the
+TMS's CRS (e.g epsg:3857) print(tms.xy_bounds(morecantile.Tile(10, 10, 4))) >>>
+BoundingBox( left=5009377.085697308, bottom=-7514065.628545959,
+right=7514065.628545959, top=-5009377.085697308, ) # Get the bounds for tile
+Z=4, X=10, Y=10 in Geographic CRS (e.g epsg:4326) print(tms.bounds
+(morecantile.Tile(10, 10, 4))) >>> BoundingBox( left=44.999999999999964,
+bottom=-55.776573018667634, right=67.4999999999999, top=-40.97989806962009, )
+``` More info can be found at https://developmentseed.org/morecantile/usage/
+### Defaults Grids `morecantile` provides a set of default TileMatrixSets: -
+**CDB1GlobalGrid** \*: CDB 1 Global Grid - EPGS:4326 (WGS84) -
+**CanadianNAD83_LCC**: Lambert conformal conic NAD83 for Canada - EPSG:3978 -
+**EuropeanETRS89_LAEAQuad**: ETRS89-extended / LAEA Europe - EPGS:3035 -
+**GNOSISGlobalGrid** \*: GNOSIS Global Grid - EPGS:4326 (WGS84) -
+**LINZAntarticaMapTilegrid**: LINZ Antarctic Map Tile Grid (Ross Sea Region) -
+EPSG:5482 - **NZTM2000Quad**: LINZ NZTM2000 Map Tile Grid - EPSG:2193 -
+**UPSAntarcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for
+Antarctic - EPSG:5042 - **UPSArcticWGS84Quad**: Universal Polar Stereographic
+WGS 84 Quad for Arctic - EPSG:5041 - **UTM31WGS84Quad**: Example of UTM grid -
+EPSG:32631 - **WebMercatorQuad**: Spherical Mercator - EPGS:3857 (default grid
+for Web Mercator based maps) - **WGS1984Quad**: EPSG:4326 for the World - EPGS:
+4326 (WGS84) - **WorldCRS84Quad**: CRS84 for the World -
+**WorldMercatorWGS84Quad**: Elliptical Mercator projection - EPGS:3395 \*
+TileMatrixSets with variable Matrix Width (see https://docs.ogc.org/is/17-
+083r4/17-083r4.html#toc15) ref: https://schemas.opengis.net/tms/2.0/json/
+examples/tilematrixset/ ## Implementations - [rio-tiler](https://github.com/
+cogeotiff/rio-tiler): Create tile from raster using Morecantile TMS. -
+[titiler](https://github.com/developmentseed/titiler): A modern dynamic tile
 server built on top of FastAPI and Rasterio/GDAL. - [tipg](https://github.com/
 developmentseed/tipg): OGC Features and Tiles API. - [planetcantile](https://
 github.com/AndrewAnnex/planetcantile): Tile matrix sets for other planets. -
 [supermorecado](https://github.com/developmentseed/supermorecado): Extend the
 functionality of morecantile with additional commands. ## Changes See
 [CHANGES.md](https://github.com/developmentseed/morecantile/blob/main/
 CHANGES.md). ## Contribution & Development See [CONTRIBUTING.md](https://
```

### Comparing `morecantile-4.3.0/morecantile/commons.py` & `morecantile-5.0.0/morecantile/commons.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/CanadianNAD83_LCC.json` & `morecantile-5.0.0/morecantile/data/CanadianNAD83_LCC.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/EuropeanETRS89_LAEAQuad.json` & `morecantile-5.0.0/morecantile/data/EuropeanETRS89_LAEAQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/LINZAntarticaMapTilegrid.json` & `morecantile-5.0.0/morecantile/data/LINZAntarticaMapTilegrid.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/NZTM2000Quad.json` & `morecantile-5.0.0/morecantile/data/NZTM2000Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/UPSAntarcticWGS84Quad.json` & `morecantile-5.0.0/morecantile/data/UPSAntarcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/UPSArcticWGS84Quad.json` & `morecantile-5.0.0/morecantile/data/UPSArcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/UTM31WGS84Quad.json` & `morecantile-5.0.0/morecantile/data/UTM31WGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/WGS1984Quad.json` & `morecantile-5.0.0/morecantile/data/WGS1984Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/WebMercatorQuad.json` & `morecantile-5.0.0/morecantile/data/WebMercatorQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/WorldCRS84Quad.json` & `morecantile-5.0.0/morecantile/data/WorldCRS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/data/WorldMercatorWGS84Quad.json` & `morecantile-5.0.0/morecantile/data/WorldMercatorWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/defaults.py` & `morecantile-5.0.0/morecantile/defaults.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,16 +33,17 @@
         if identifier not in self.tms:
             raise InvalidIdentifier(f"Invalid identifier: {identifier}")
 
         tms = self.tms[identifier]
 
         # We lazyload the TMS document only when called
         if isinstance(tms, pathlib.Path):
-            tms = TileMatrixSet.parse_file(tms)
-            self.tms[identifier] = tms
+            with tms.open() as f:
+                tms = TileMatrixSet.model_validate_json(f.read())
+                self.tms[identifier] = tms
 
         return tms
 
     def list(self) -> List[str]:
         """List registered TMS."""
         return list(self.tms.keys())
```

### Comparing `morecantile-4.3.0/morecantile/errors.py` & `morecantile-5.0.0/morecantile/errors.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/models.py` & `morecantile-5.0.0/morecantile/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 """Pydantic modules for OGC TileMatrixSets (https://www.ogc.org/standards/tms)"""
 
 import math
+import sys
 import warnings
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    Iterator,
-    List,
-    Literal,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
+from functools import cached_property
+from typing import Any, Dict, Iterator, List, Literal, Optional, Sequence, Tuple, Union
 
-from cachetools import LRUCache, cached
-from cachetools.keys import hashkey
 from pydantic import (
     AnyHttpUrl,
     AnyUrl,
     BaseModel,
     Field,
     PrivateAttr,
-    conlist,
-    validator,
+    RootModel,
+    field_validator,
+    model_validator,
 )
 from pyproj import CRS, Transformer
 from pyproj.exceptions import CRSError, ProjError
 
 from morecantile.commons import BoundingBox, Coords, Tile
 from morecantile.errors import (
     DeprecationError,
@@ -42,77 +32,79 @@
     bbox_to_feature,
     check_quadkey_support,
     meters_per_unit,
     point_in_bbox,
     to_rasterio_crs,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Annotated  # pylint: disable=no-name-in-module
+else:
+    from typing_extensions import Annotated
+
 NumType = Union[float, int]
 BoundsType = Tuple[NumType, NumType]
 LL_EPSILON = 1e-11
 WGS84_CRS = CRS.from_epsg(4326)
-
-
-if TYPE_CHECKING:
-    axesInfo = List[str]
-else:
-    axesInfo = conlist(str, min_items=2, max_items=2)
+axesInfo = Annotated[List[str], Field(min_length=2, max_length=2)]
 
 
 class CRSUri(BaseModel):
     """Coordinate Reference System (CRS) from URI."""
 
-    uri: AnyUrl = Field(
-        ...,
-        description="Reference to one coordinate reference system (CRS) as URI",
-        examples=[
-            "http://www.opengis.net/def/crs/EPSG/0/3978",
-            "urn:ogc:def:crs:EPSG::2193",
-        ],
-    )
+    uri: Annotated[
+        AnyUrl,
+        Field(
+            description="Reference to one coordinate reference system (CRS) as URI",
+            examples=[
+                "http://www.opengis.net/def/crs/EPSG/0/3978",
+                "urn:ogc:def:crs:EPSG::2193",
+            ],
+        ),
+    ]
 
 
 class CRSWKT(BaseModel):
     """Coordinate Reference System (CRS) from WKT."""
 
-    wkt: str = Field(
-        ...,
-        description="Reference to one coordinate reference system (CRS) as WKT string",
-        examples=[
-            'GEOGCS["GCS_WGS_1984",DATUM["D_WGS_1984",SPHEROID["WGS_1984",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["Degree",0.017453292519943295]]',
-        ],
-    )
+    wkt: Annotated[
+        str,
+        Field(
+            description="Reference to one coordinate reference system (CRS) as WKT string",
+            examples=[
+                'GEOGCS["GCS_WGS_1984",DATUM["D_WGS_1984",SPHEROID["WGS_1984",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["Degree",0.017453292519943295]]',
+            ],
+        ),
+    ]
 
 
 # NOT SUPPORTED
 # class CRSRef(BaseModel):
 #     """CRS from referenceSystem."""
 #
 #     referenceSystem: Dict[str, Any] = Field(
 #         ...,
 #         description="A reference system data structure as defined in the MD_ReferenceSystem of the ISO 19115",
 #     )
 
 
-class CRSType(BaseModel):
+class CRSType(RootModel[Union[str, Union[CRSUri, CRSWKT]]]):
     """CRS model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/common-geodata/crs.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
-    __root__: Union[str, Union[CRSUri, CRSWKT]] = Field(..., title="CRS")
     _pyproj_crs: CRS = PrivateAttr()
 
-    def __init__(self, **data):
-        """Custom Init to validate CRS string and create Pyproj CRS object."""
-        super().__init__(**data)
-
-        self._pyproj_crs = CRS.from_user_input(data.get("__root__"))
+    def model_post_init(self, __context: Any) -> None:
+        """Post Init: Set private attr."""
+        super().model_post_init(__context)
+        self._pyproj_crs = CRS.from_user_input(self.root)
 
     @property
     def srs(self) -> str:
         """return the string form of the user input used to create the CRS."""
         return self._pyproj_crs.srs
 
     def to_epsg(self, *args: Any, **kwargs: Any) -> Optional[int]:
@@ -157,173 +149,251 @@
 
 
 def ordered_axis_inverted(ordered_axes: List[str]) -> bool:
     """Check if ordered axes have inverted AXIS (lat,lon) instead of (lon,lat)."""
     return ordered_axes[0].upper() in ["Y", "LAT", "N"]
 
 
-class TMSBoundingBox(BaseModel):
+class TMSBoundingBox(BaseModel, arbitrary_types_allowed=True):
     """Bounding box
 
     ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/2DBoundingBox.json
 
     """
 
-    lowerLeft: BoundsType = Field(
-        description="A 2D Point in the CRS indicated elsewhere"
-    )
-    upperRight: BoundsType = Field(
-        description="A 2D Point in the CRS indicated elsewhere"
-    )
-    crs: Optional[CRSType]
-    orderedAxes: Optional[axesInfo]
-
-    class Config:
-        """Configure TMSBoundingBox."""
-
-        arbitrary_types_allowed = True
-
+    lowerLeft: Annotated[
+        BoundsType,
+        Field(description="A 2D Point in the CRS indicated elsewhere"),
+    ]
+    upperRight: Annotated[
+        BoundsType,
+        Field(description="A 2D Point in the CRS indicated elsewhere"),
+    ]
+    crs: Annotated[
+        Optional[CRSType],
+        Field(description="Coordinate Reference System (CRS)"),
+    ] = None
+    orderedAxes: Annotated[
+        Optional[axesInfo],
+        Field(description="Ordered list of names of the dimensions defined in the CRS"),
+    ] = None
 
-# class variableMatrixWidth(BaseModel):
-#     """Variable Matrix Width Definition
 
+class variableMatrixWidth(BaseModel):
+    """Variable Matrix Width Definition
 
-#     ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/variableMatrixWidth.json
-#     """
+    ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/variableMatrixWidth.json
+    """
 
-#     coalesce: int = Field(..., ge=2, multiple_of=1, description="Number of tiles in width that coalesce in a single tile for these rows")
-#     minTileRow: int = Field(..., ge=0, multiple_of=1, description="First tile row where the coalescence factor applies for this tilematrix")
-#     maxTileRow: int = Field(..., ge=0, multiple_of=1, description="Last tile row where the coalescence factor applies for this tilematrix")
+    coalesce: Annotated[
+        int,
+        Field(
+            ge=2,
+            multiple_of=1,
+            description="Number of tiles in width that coalesce in a single tile for these rows",
+        ),
+    ]
+    minTileRow: Annotated[
+        int,
+        Field(
+            ge=0,
+            multiple_of=1,
+            description="First tile row where the coalescence factor applies for this tilematrix",
+        ),
+    ]
+    maxTileRow: Annotated[
+        int,
+        Field(
+            ge=0,
+            multiple_of=1,
+            description="Last tile row where the coalescence factor applies for this tilematrix",
+        ),
+    ]
 
 
-class TileMatrix(BaseModel):
+class TileMatrix(BaseModel, extra="forbid"):
     """Tile Matrix Definition
 
     A tile matrix, usually corresponding to a particular zoom level of a TileMatrixSet.
 
     ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/tileMatrix.json
     """
 
-    title: Optional[str] = Field(
-        description="Title of this tile matrix, normally used for display to a human"
-    )
-    description: Optional[str] = Field(
-        description="Brief narrative description of this tile matrix set, normally available for display to a human"
-    )
-    keywords: Optional[List[str]] = Field(
-        description="Unordered list of one or more commonly used or formalized word(s) or phrase(s) used to describe this dataset"
-    )
-    id: str = Field(
-        ...,
-        regex=r"^[0-9]+$",
-        description="Identifier selecting one of the scales defined in the TileMatrixSet and representing the scaleDenominator the tile. Implementation of 'identifier'",
-    )
-    scaleDenominator: float = Field(
-        ..., description="Scale denominator of this tile matrix"
-    )
-    cellSize: float = Field(..., description="Cell size of this tile matrix")
-    cornerOfOrigin: Optional[Literal["topLeft", "bottomLeft"]] = Field(
-        description="The corner of the tile matrix (_topLeft_ or _bottomLeft_) used as the origin for numbering tile rows and columns. This corner is also a corner of the (0, 0) tile."
-    )
-    pointOfOrigin: BoundsType = Field(
-        ...,
-        description="Precise position in CRS coordinates of the corner of origin (e.g. the top-left corner) for this tile matrix. This position is also a corner of the (0, 0) tile. In previous version, this was 'topLeftCorner' and 'cornerOfOrigin' did not exist.",
-    )
-    tileWidth: int = Field(
-        ...,
-        ge=1,
-        multiple_of=1,
-        description="Width of each tile of this tile matrix in pixels",
-    )
-    tileHeight: int = Field(
-        ...,
-        ge=1,
-        multiple_of=1,
-        description="Height of each tile of this tile matrix in pixels",
-    )
-    matrixWidth: int = Field(
-        ...,
-        ge=1,
-        multiple_of=1,
-        description="Width of the matrix (number of tiles in width)",
-    )
-    matrixHeight: int = Field(
-        ...,
-        ge=1,
-        multiple_of=1,
-        description="Height of the matrix (number of tiles in height)",
-    )
-    # variableMatrixWidths: Optional[List[variableMatrixWidth]] = Field(description="Describes the rows that has variable matrix width")
+    title: Annotated[
+        Optional[str],
+        Field(
+            description="Title of this tile matrix, normally used for display to a human"
+        ),
+    ] = None
+    description: Annotated[
+        Optional[str],
+        Field(
+            description="Brief narrative description of this tile matrix set, normally available for display to a human",
+        ),
+    ] = None
+    keywords: Annotated[
+        Optional[List[str]],
+        Field(
+            description="Unordered list of one or more commonly used or formalized word(s) or phrase(s) used to describe this dataset",
+        ),
+    ] = None
+    id: Annotated[
+        str,
+        Field(
+            pattern=r"^\-?[0-9]+$",
+            description="Identifier selecting one of the scales defined in the TileMatrixSet and representing the scaleDenominator the tile. Implementation of 'identifier'",
+        ),
+    ]
+    scaleDenominator: Annotated[
+        float,
+        Field(description="Scale denominator of this tile matrix"),
+    ]
+    cellSize: Annotated[
+        float,
+        Field(description="Cell size of this tile matrix"),
+    ]
+    cornerOfOrigin: Annotated[
+        Optional[Literal["topLeft", "bottomLeft"]],
+        Field(
+            description="The corner of the tile matrix (_topLeft_ or _bottomLeft_) used as the origin for numbering tile rows and columns. This corner is also a corner of the (0, 0) tile.",
+        ),
+    ] = None
+    pointOfOrigin: Annotated[
+        BoundsType,
+        Field(
+            description="Precise position in CRS coordinates of the corner of origin (e.g. the top-left corner) for this tile matrix. This position is also a corner of the (0, 0) tile. In previous version, this was 'topLeftCorner' and 'cornerOfOrigin' did not exist.",
+        ),
+    ] = None
+    tileWidth: Annotated[
+        int,
+        Field(
+            ge=1,
+            multiple_of=1,
+            description="Width of each tile of this tile matrix in pixels",
+        ),
+    ]
+    tileHeight: Annotated[
+        int,
+        Field(
+            ge=1,
+            multiple_of=1,
+            description="Height of each tile of this tile matrix in pixels",
+        ),
+    ]
+    matrixWidth: Annotated[
+        int,
+        Field(
+            ge=1,
+            multiple_of=1,
+            description="Width of the matrix (number of tiles in width)",
+        ),
+    ]
+    matrixHeight: Annotated[
+        int,
+        Field(
+            ge=1,
+            multiple_of=1,
+            description="Height of the matrix (number of tiles in height)",
+        ),
+    ]
+    variableMatrixWidths: Annotated[
+        Optional[List[variableMatrixWidth]],
+        Field(description="Describes the rows that has variable matrix width"),
+    ] = None
+
+    def get_coalesce_factor(self, row: int) -> int:
+        """Get Coalesce value for TileMatrix."""
+        if not self.variableMatrixWidths:
+            raise ValueError("TileMatrix has not variableMatrixWidths")
+
+        if row < 0:
+            raise ValueError(f"Cannot find coalesce factor for Negative Row ({row})")
+
+        if row > self.matrixHeight - 1:
+            raise ValueError(
+                f"Row {row} is greater than the TileMatrix height ({self.matrixHeight})"
+            )
 
-    class Config:
-        """Forbid additional items like variableMatrixWidths."""
+        for matrix_width in self.variableMatrixWidths:
+            if matrix_width.maxTileRow >= row >= matrix_width.minTileRow:
+                return matrix_width.coalesce
 
-        extra = "forbid"
+        return 1
 
 
-class TileMatrixSet(BaseModel):
+class TileMatrixSet(BaseModel, arbitrary_types_allowed=True):
     """Tile Matrix Set Definition
 
     A definition of a tile matrix set following the Tile Matrix Set standard.
     For tileset metadata, such a description (in `tileMatrixSet` property) is only required for offline use,
     as an alternative to a link with a `http://www.opengis.net/def/rel/ogc/1.0/tiling-scheme` relation type.
 
     ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/tileMatrixSet.json
 
     """
 
-    title: Optional[str] = Field(
-        description="Title of this tile matrix set, normally used for display to a human"
-    )
+    title: Annotated[
+        Optional[str],
+        Field(
+            description="Title of this tile matrix set, normally used for display to a human",
+        ),
+    ] = None
     description: Optional[str] = Field(
-        description="Brief narrative description of this tile matrix set, normally available for display to a human"
-    )
-    keywords: Optional[List[str]] = Field(
-        description="Unordered list of one or more commonly used or formalized word(s) or phrase(s) used to describe this tile matrix set"
-    )
-    id: Optional[str] = Field(
-        regex=r"^[\w\d_\-]+$",
-        description="Tile matrix set identifier. Implementation of 'identifier'",
-    )
-    uri: Optional[str] = Field(
-        description="Reference to an official source for this tileMatrixSet"
-    )
-    orderedAxes: Optional[axesInfo]
-    crs: CRSType = Field(..., description="Coordinate Reference System (CRS)")
-    wellKnownScaleSet: Optional[AnyHttpUrl] = Field(
-        description="Reference to a well-known scale set"
-    )
-    boundingBox: Optional[TMSBoundingBox] = Field(
-        description="Minimum bounding rectangle surrounding the tile matrix set, in the supported CRS"
-    )
-    tileMatrices: List[TileMatrix] = Field(
-        ..., description="Describes scale levels and its tile matrices"
+        None,
+        description="Brief narrative description of this tile matrix set, normally available for display to a human",
     )
+    keywords: Annotated[
+        Optional[List[str]],
+        Field(
+            description="Unordered list of one or more commonly used or formalized word(s) or phrase(s) used to describe this tile matrix set",
+        ),
+    ] = None
+    id: Annotated[
+        Optional[str],
+        Field(
+            pattern=r"^[\w\d_\-]+$",
+            description="Tile matrix set identifier. Implementation of 'identifier'",
+        ),
+    ] = None
+    uri: Annotated[
+        Optional[str],
+        Field(description="Reference to an official source for this tileMatrixSet"),
+    ] = None
+    orderedAxes: Annotated[
+        Optional[axesInfo],
+        Field(description="Ordered list of names of the dimensions defined in the CRS"),
+    ] = None
+    crs: Annotated[
+        CRSType,
+        Field(description="Coordinate Reference System (CRS)"),
+    ]
+    wellKnownScaleSet: Annotated[
+        Optional[AnyHttpUrl],
+        Field(description="Reference to a well-known scale set"),
+    ] = None
+    boundingBox: Annotated[
+        Optional[TMSBoundingBox],
+        Field(
+            description="Minimum bounding rectangle surrounding the tile matrix set, in the supported CRS",
+        ),
+    ] = None
+    tileMatrices: Annotated[
+        List[TileMatrix],
+        Field(description="Describes scale levels and its tile matrices"),
+    ]
 
     # Private attributes
-    _is_quadtree: bool = PrivateAttr()
     _geographic_crs: CRS = PrivateAttr(default=WGS84_CRS)
     _to_geographic: Transformer = PrivateAttr()
     _from_geographic: Transformer = PrivateAttr()
 
-    class Config:
-        """Configure TileMatrixSet."""
-
-        arbitrary_types_allowed = True
-
     def __init__(self, **data):
-        """Create PyProj transforms and check if TileMatrixSet supports quadkeys."""
-        if {"supportedCRS", "topLeftCorner"}.intersection(data):
-            raise DeprecationError(
-                "Tile Matrix Set must be version 2.0. Use morecantile <4.0 for TMS 1.0 support"
-            )
-
+        """Set private attributes."""
         super().__init__(**data)
 
-        self._is_quadtree = check_quadkey_support(self.tileMatrices)
         self._geographic_crs = data.get("_geographic_crs", WGS84_CRS)
 
         try:
             self._to_geographic = Transformer.from_crs(
                 self.crs._pyproj_crs, self._geographic_crs, always_xy=True
             )
             self._from_geographic = Transformer.from_crs(
@@ -334,54 +404,80 @@
                 "Could not create coordinate Transformer from input CRS to the given geographic CRS"
                 "some methods might not be available.",
                 UserWarning,
             )
             self._to_geographic = None
             self._from_geographic = None
 
-    @validator("tileMatrices")
+    @model_validator(mode="before")
+    def check_for_old_specification(cls, data):
+        """Check for TMS V1.0 keywords."""
+        if {"supportedCRS", "topLeftCorner"}.intersection(data):
+            raise DeprecationError(
+                "Tile Matrix Set must be version 2.0. Use morecantile <4.0 for TMS 1.0 support"
+            )
+        return data
+
+    @field_validator("tileMatrices")
     def sort_tile_matrices(cls, v):
         """Sort matrices by identifier"""
         return sorted(v, key=lambda m: int(m.id))
 
+    @cached_property
+    def is_quadtree(self) -> bool:
+        """Check for quadtree support."""
+        return check_quadkey_support(self.tileMatrices)
+
+    @cached_property
+    def is_variable(self) -> bool:
+        """Check if TMS has variable width matrix."""
+        return any(
+            [
+                True if matrix.variableMatrixWidths is not None else False
+                for matrix in self.tileMatrices
+            ]
+        )
+
     def __iter__(self):
         """Iterate over matrices"""
         for matrix in self.tileMatrices:
             yield matrix
 
     def __repr__(self):
         """Simplify default pydantic model repr."""
-        return f"<TileMatrixSet title='{self.title}' id='{self.id}' crs='{self.crs.__root__}>"
+        return (
+            f"<TileMatrixSet title='{self.title}' id='{self.id}' crs='{self.crs.root}>"
+        )
 
-    @property
-    def geographic_crs(self) -> CRSType:
+    @cached_property
+    def geographic_crs(self) -> CRS:
         """Return the TMS's geographic CRS."""
         return self._geographic_crs
 
-    @property
+    @cached_property
     def rasterio_crs(self):
         """Return rasterio CRS."""
         return to_rasterio_crs(self.crs._pyproj_crs)
 
-    @property
+    @cached_property
     def rasterio_geographic_crs(self):
         """Return the geographic CRS as a rasterio CRS."""
         return to_rasterio_crs(self._geographic_crs)
 
     @property
     def minzoom(self) -> int:
         """TileMatrixSet minimum TileMatrix identifier"""
         return int(self.tileMatrices[0].id)
 
     @property
     def maxzoom(self) -> int:
         """TileMatrixSet maximum TileMatrix identifier"""
         return int(self.tileMatrices[-1].id)
 
-    @property
+    @cached_property
     def _invert_axis(self) -> bool:
         """Check if CRS has inverted AXIS (lat,lon) instead of (lon,lat)."""
         return (
             ordered_axis_inverted(self.orderedAxes)
             if self.orderedAxes
             else crs_axis_inverted(self.crs._pyproj_crs)
         )
@@ -560,14 +656,22 @@
 
     def matrix(self, zoom: int) -> TileMatrix:
         """Return the TileMatrix for a specific zoom."""
         for m in self.tileMatrices:
             if m.id == str(zoom):
                 return m
 
+        #######################################################################
+        # If user wants a deeper matrix we calculate it
+        #######################################################################
+        if self.is_variable:
+            raise InvalidZoomError(
+                f"TileMatrix not found for level: {zoom} - Unable to construct tileMatrix for TMS with variable width"
+            )
+
         matrix_scale = list(
             {
                 round(
                     self.tileMatrices[idx].scaleDenominator
                     / self.tileMatrices[idx - 1].scaleDenominator,
                     2,
                 )
@@ -580,28 +684,27 @@
             )
 
         warnings.warn(
             f"TileMatrix not found for level: {zoom} - Creating values from TMS Scale.",
             UserWarning,
         )
 
+        # TODO: what if we want to construct a matrix for a level up ?
         tile_matrix = self.tileMatrices[-1]
         factor = 1 / matrix_scale[0]
         while not str(zoom) == tile_matrix.id:
             tile_matrix = TileMatrix(
-                **{
-                    "id": str(int(tile_matrix.id) + 1),
-                    "scaleDenominator": tile_matrix.scaleDenominator / factor,
-                    "cellSize": tile_matrix.cellSize / factor,
-                    "pointOfOrigin": tile_matrix.pointOfOrigin,
-                    "tileWidth": tile_matrix.tileWidth,
-                    "tileHeight": tile_matrix.tileHeight,
-                    "matrixWidth": int(tile_matrix.matrixWidth * factor),
-                    "matrixHeight": int(tile_matrix.matrixHeight * factor),
-                }
+                id=str(int(tile_matrix.id) + 1),
+                scaleDenominator=tile_matrix.scaleDenominator / factor,
+                cellSize=tile_matrix.cellSize / factor,
+                pointOfOrigin=tile_matrix.pointOfOrigin,
+                tileWidth=tile_matrix.tileWidth,
+                tileHeight=tile_matrix.tileHeight,
+                matrixWidth=int(tile_matrix.matrixWidth * factor),
+                matrixHeight=int(tile_matrix.matrixHeight * factor),
             )
 
         return tile_matrix
 
     def _resolution(self, matrix: TileMatrix) -> float:
         """
         Tile resolution for a TileMatrix.
@@ -609,14 +712,24 @@
         From note g in http://docs.opengeospatial.org/is/17-083r2/17-083r2.html#table_2:
           The pixel size of the tile can be obtained from the scaleDenominator
           by multiplying the later by 0.28 10-3 / metersPerUnit.
 
         """
         return matrix.scaleDenominator * 0.28e-3 / meters_per_unit(self.crs._pyproj_crs)
 
+    def _matrix_origin(self, matrix: TileMatrix) -> Coords:
+        """Return the Origin coordinates of the matrix."""
+        origin_x = (
+            matrix.pointOfOrigin[1] if self._invert_axis else matrix.pointOfOrigin[0]
+        )
+        origin_y = (
+            matrix.pointOfOrigin[0] if self._invert_axis else matrix.pointOfOrigin[1]
+        )
+        return Coords(origin_x, origin_y)
+
     def zoom_for_res(
         self,
         res: float,
         max_z: Optional[int] = None,
         zoom_level_strategy: str = "auto",
         min_z: Optional[int] = None,
     ) -> int:
@@ -650,21 +763,24 @@
             matrix_res = self._resolution(self.matrix(zoom_level))
             if res > matrix_res or abs(res - matrix_res) / matrix_res <= 1e-8:
                 break
 
         if zoom_level > 0 and abs(res - matrix_res) / matrix_res > 1e-8:
             if zoom_level_strategy.lower() == "lower":
                 zoom_level = max(zoom_level - 1, min_z)
+
             elif zoom_level_strategy.lower() == "upper":
                 zoom_level = min(zoom_level, max_z)
+
             elif zoom_level_strategy.lower() == "auto":
                 if (self._resolution(self.matrix(max(zoom_level - 1, min_z))) / res) < (
                     res / matrix_res
                 ):
                     zoom_level = max(zoom_level - 1, min_z)
+
             else:
                 raise ValueError(
                     f"Invalid strategy: {zoom_level_strategy}. Should be one of lower|upper|auto"
                 )
 
         return zoom_level
 
@@ -733,45 +849,39 @@
         Returns
         -------
         Tile
 
         """
         matrix = self.matrix(zoom)
         res = self._resolution(matrix)
-
-        origin_x = (
-            matrix.pointOfOrigin[1] if self._invert_axis else matrix.pointOfOrigin[0]
-        )
-        origin_y = (
-            matrix.pointOfOrigin[0] if self._invert_axis else matrix.pointOfOrigin[1]
-        )
+        origin_x, origin_y = self._matrix_origin(matrix)
 
         xtile = (
             math.floor((xcoord - origin_x) / float(res * matrix.tileWidth))
             if not math.isinf(xcoord)
             else 0
         )
         ytile = (
             math.floor((origin_y - ycoord) / float(res * matrix.tileHeight))
             if not math.isinf(ycoord)
             else 0
         )
 
-        # # avoid out-of-range tiles
+        # avoid out-of-range tiles
         if xtile < 0:
             xtile = 0
 
         if ytile < 0:
             ytile = 0
 
-        if xtile > matrix.matrixWidth:
-            xtile = matrix.matrixWidth
+        if xtile >= matrix.matrixWidth:
+            xtile = matrix.matrixWidth - 1
 
-        if ytile > matrix.matrixHeight:
-            ytile = matrix.matrixHeight
+        if ytile >= matrix.matrixHeight:
+            ytile = matrix.matrixHeight - 1
 
         return Tile(x=xtile, y=ytile, z=zoom)
 
     def tile(self, lng: float, lat: float, zoom: int, truncate=False) -> Tile:
         """
         Get the tile for a given geographic longitude and latitude pair.
 
@@ -805,25 +915,52 @@
         Coords: The upper left coordinates of the input tile.
 
         """
         t = _parse_tile_arg(*tile)
 
         matrix = self.matrix(t.z)
         res = self._resolution(matrix)
+        origin_x, origin_y = self._matrix_origin(matrix)
 
-        origin_x = (
-            matrix.pointOfOrigin[1] if self._invert_axis else matrix.pointOfOrigin[0]
-        )
-        origin_y = (
-            matrix.pointOfOrigin[0] if self._invert_axis else matrix.pointOfOrigin[1]
+        cf = 1
+        if matrix.variableMatrixWidths is not None:
+            cf = matrix.get_coalesce_factor(t.y)
+
+        return Coords(
+            origin_x + math.floor(t.x / cf) * res * cf * matrix.tileWidth,
+            origin_y - t.y * res * matrix.tileHeight,
         )
 
-        xcoord = origin_x + t.x * res * matrix.tileWidth
-        ycoord = origin_y - t.y * res * matrix.tileHeight
-        return Coords(xcoord, ycoord)
+    def _lr(self, *tile: Tile) -> Coords:
+        """
+        Return the lower right coordinate of the tile in TMS coordinate reference system.
+
+        Attributes
+        ----------
+        tile: (x, y, z) tile coordinates or a Tile object we want the lower right coordinates of.
+
+        Returns
+        -------
+        Coords: The lower right coordinates of the input tile.
+
+        """
+        t = _parse_tile_arg(*tile)
+
+        matrix = self.matrix(t.z)
+        res = self._resolution(matrix)
+        origin_x, origin_y = self._matrix_origin(matrix)
+
+        cf = 1
+        if matrix.variableMatrixWidths is not None:
+            cf = matrix.get_coalesce_factor(t.y)
+
+        return Coords(
+            origin_x + (math.floor(t.x / cf) + 1) * res * cf * matrix.tileWidth,
+            origin_y - (t.y + 1) * res * matrix.tileHeight,
+        )
 
     def xy_bounds(self, *tile: Tile) -> BoundingBox:
         """
         Return the bounding box of the tile in TMS coordinate reference system.
 
         Attributes
         ----------
@@ -833,15 +970,15 @@
         -------
         BoundingBox: The bounding box of the input tile.
 
         """
         t = _parse_tile_arg(*tile)
 
         left, top = self._ul(t)
-        right, bottom = self._ul(Tile(t.x + 1, t.y + 1, t.z))
+        right, bottom = self._lr(t)
         return BoundingBox(left, bottom, right, top)
 
     def ul(self, *tile: Tile) -> Coords:
         """
         Return the upper left coordinates of the tile in geographic coordinate reference system.
 
         Attributes
@@ -854,14 +991,32 @@
 
         """
         t = _parse_tile_arg(*tile)
 
         x, y = self._ul(t)
         return Coords(*self.lnglat(x, y))
 
+    def lr(self, *tile: Tile) -> Coords:
+        """
+        Return the lower right coordinates of the tile in geographic coordinate reference system.
+
+        Attributes
+        ----------
+        tile (tuple or Tile): (x, y, z) tile coordinates or a Tile object we want the lower right geographic coordinates of.
+
+        Returns
+        -------
+        Coords: The lower right geographic coordinates of the input tile.
+
+        """
+        t = _parse_tile_arg(*tile)
+
+        x, y = self._lr(t)
+        return Coords(*self.lnglat(x, y))
+
     def bounds(self, *tile: Tile) -> BoundingBox:
         """
         Return the bounding box of the tile in geographic coordinate reference system.
 
         Attributes
         ----------
         tile (tuple or Tile): A tuple of (x, y, z) tile coordinates or a Tile object we want the bounding box of.
@@ -870,38 +1025,30 @@
         -------
         BoundingBox: The bounding box of the input tile.
 
         """
         t = _parse_tile_arg(*tile)
 
         left, top = self.ul(t)
-        right, bottom = self.ul(Tile(t.x + 1, t.y + 1, t.z))
+        right, bottom = self.lr(t)
         return BoundingBox(left, bottom, right, top)
 
     @property
     def xy_bbox(self):
         """Return TMS bounding box in TileMatrixSet's CRS."""
         zoom = self.minzoom
         matrix = self.matrix(zoom)
 
         left, top = self._ul(Tile(0, 0, zoom))
-        right, bottom = self._ul(Tile(matrix.matrixWidth, matrix.matrixHeight, zoom))
-
+        right, bottom = self._lr(
+            Tile(matrix.matrixWidth - 1, matrix.matrixHeight - 1, zoom)
+        )
         return BoundingBox(left, bottom, right, top)
 
-    @property
-    @cached(  # type: ignore
-        LRUCache(maxsize=512),
-        key=lambda self: hashkey(
-            self.crs.__root__,
-            self.tileMatrices[0].pointOfOrigin,
-            self.tileMatrices[0].matrixWidth,
-            self.tileMatrices[0].matrixHeight,
-        ),
-    )
+    @cached_property
     def bbox(self):
         """Return TMS bounding box in geographic coordinate reference system."""
         left, bottom, right, top = self.xy_bbox
         return BoundingBox(
             *self._to_geographic.transform_bounds(
                 left,
                 bottom,
@@ -1054,15 +1201,15 @@
             "type": "Feature",
             "bbox": bbox,
             "id": xyz,
             "geometry": geom,
             "properties": {
                 "title": f"XYZ tile {xyz}",
                 "grid_name": self.id,
-                "grid_crs": self.crs.__root__,
+                "grid_crs": self.crs.root,
             },
         }
 
         if projected:
             warnings.warn(
                 "CRS is no longer part of the GeoJSON specification."
                 "Other projection than EPSG:4326 might not be supported.",
@@ -1094,15 +1241,15 @@
             May be be either an instance of Tile or 3 ints, X, Y, Z.
 
         Returns
         -------
         str
 
         """
-        if not self._is_quadtree:
+        if not self.is_quadtree:
             raise NoQuadkeySupport(
                 "This Tile Matrix Set doesn't support 2 x 2 quadkeys."
             )
 
         t = _parse_tile_arg(*tile)
 
         qk = []
@@ -1126,15 +1273,15 @@
             A quadkey string.
 
         Returns
         -------
         Tile
 
         """
-        if not self._is_quadtree:
+        if not self.is_quadtree:
             raise NoQuadkeySupport(
                 "This Tile Matrix Set doesn't support 2 x 2 quadkeys."
             )
 
         if len(qk) == 0:
             return Tile(0, 0, 0)
 
@@ -1247,14 +1394,15 @@
             return []
 
         if zoom is not None and t.z <= zoom:
             raise InvalidZoomError("zoom must be less than that of the input tile")
 
         target_zoom = t.z - 1 if zoom is None else zoom
 
+        # buffer value to apply on bbox
         res = self._resolution(self.matrix(t.z)) / 10.0
 
         bbox = self.xy_bounds(t)
         ul_tile = self._tile(bbox.left + res, bbox.top - res, target_zoom)
         lr_tile = self._tile(bbox.right - res, bbox.bottom + res, target_zoom)
 
         tiles = []
@@ -1285,17 +1433,18 @@
         t = _parse_tile_arg(*tile)
 
         if zoom is not None and t.z > zoom:
             raise InvalidZoomError("zoom must be greater than that of the input tile")
 
         target_zoom = t.z + 1 if zoom is None else zoom
 
-        bbox = self.xy_bounds(t)
+        # buffer value to apply on bbox
         res = self._resolution(self.matrix(t.z)) / 10.0
 
+        bbox = self.xy_bounds(t)
         ul_tile = self._tile(bbox.left + res, bbox.top - res, target_zoom)
         lr_tile = self._tile(bbox.right - res, bbox.bottom + res, target_zoom)
 
         tiles = []
         for i in range(ul_tile.x, lr_tile.x + 1):
             for j in range(ul_tile.y, lr_tile.y + 1):
                 tiles.append(Tile(i, j, target_zoom))
```

### Comparing `morecantile-4.3.0/morecantile/scripts/cli.py` & `morecantile-5.0.0/morecantile/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/morecantile/utils.py` & `morecantile-5.0.0/morecantile/utils.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.3.0/pyproject.toml` & `morecantile-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "attrs",
     "pyproj~=3.1",
-    "pydantic~=1.0",
-    "cachetools",
+    "pydantic~=2.0",
 ]
 
 [project.optional-dependencies]
 rasterio = [
     "rasterio>=1.2.1",
 ]
 test = [
@@ -98,7 +97,10 @@
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
 ]
+
+[tool.ruff.per-file-ignores]
+"tests/*.py" = ["D1"]
```

### Comparing `morecantile-4.3.0/PKG-INFO` & `morecantile-5.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morecantile
-Version: 4.3.0
+Version: 5.0.0
 Summary: Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
 Keywords: GIS,TMS,TileMatrixSet,Map Tile
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -12,16 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: attrs
 Requires-Dist: pyproj~=3.1
-Requires-Dist: pydantic~=1.0
-Requires-Dist: cachetools
+Requires-Dist: pydantic~=2.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: pygments ; extra == "docs"
 Requires-Dist: rasterio>=1.2.1 ; extra == "rasterio"
 Requires-Dist: mercantile ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
@@ -69,18 +68,17 @@
 
 Morecantile is like [mercantile](https://github.com/mapbox/mercantile) (the best tool to work with Web Mercator tile indexes), but with support for other TileMatrixSet grids.
 
 **Morecantile** follows the **OGC Two Dimensional Tile Matrix Set** specification **2.0** found in [https://docs.ogc.org/is/17-083r4/17-083r4.html](https://docs.ogc.org/is/17-083r4/17-083r4.html)
 
 | Morecantile Version | OGC Specification Version | Link
 | ------------------- | ------------------------- |---------
-| 4.0                 | 2.0                       | https://docs.ogc.org/is/17-083r4/17-083r4.html
-| 3.0 and earlier     | 1.0                       | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html
+| >=4.0               | 2.0                       | https://docs.ogc.org/is/17-083r4/17-083r4.html
+| =<3.0               | 1.0                       | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html
 
-**Note**: Variable matrix width tile set are not supported.
 
 ## Install
 
 ```bash
 $ python -m pip install -U pip
 $ python -m pip install morecantile
 
@@ -124,28 +122,32 @@
 )
 ```
 
 More info can be found at https://developmentseed.org/morecantile/usage/
 
 ### Defaults Grids
 
-`morecantile` provides a set of default TMS grids:
+`morecantile` provides a set of default TileMatrixSets:
 
+- **CDB1GlobalGrid** \*: CDB 1 Global Grid - EPGS:4326 (WGS84)
 - **CanadianNAD83_LCC**: Lambert conformal conic NAD83 for Canada - EPSG:3978
 - **EuropeanETRS89_LAEAQuad**: ETRS89-extended / LAEA Europe - EPGS:3035
+- **GNOSISGlobalGrid** \*: GNOSIS Global Grid - EPGS:4326 (WGS84)
 - **LINZAntarticaMapTilegrid**: LINZ Antarctic Map Tile Grid (Ross Sea Region) - EPSG:5482
 - **NZTM2000Quad**: LINZ NZTM2000 Map Tile Grid - EPSG:2193
 - **UPSAntarcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for Antarctic - EPSG:5042
 - **UPSArcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for Arctic - EPSG:5041
 - **UTM31WGS84Quad**: Example of UTM grid - EPSG:32631
 - **WebMercatorQuad**: Spherical Mercator - EPGS:3857 (default grid for Web Mercator based maps)
 - **WGS1984Quad**: EPSG:4326 for the World - EPGS:4326 (WGS84)
 - **WorldCRS84Quad**: CRS84 for the World
 - **WorldMercatorWGS84Quad**: Elliptical Mercator projection - EPGS:3395
 
+\* TileMatrixSets with variable Matrix Width (see https://docs.ogc.org/is/17-083r4/17-083r4.html#toc15)
+
 ref: https://schemas.opengis.net/tms/2.0/json/examples/tilematrixset/
 
 ## Implementations
 
 - [rio-tiler](https://github.com/cogeotiff/rio-tiler): Create tile from raster using Morecantile TMS.
 - [titiler](https://github.com/developmentseed/titiler): A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
 - [tipg](https://github.com/developmentseed/tipg): OGC Features and Tiles API.
```

#### html2text {}

```diff
@@ -1,71 +1,73 @@
-Metadata-Version: 2.1 Name: morecantile Version: 4.3.0 Summary: Construct and
+Metadata-Version: 2.1 Name: morecantile Version: 5.0.0 Summary: Construct and
 use map tile grids (a.k.a TileMatrixSet / TMS). Keywords:
 GIS,TMS,TileMatrixSet,Map Tile Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: GIS Requires-Dist: attrs Requires-Dist:
-pyproj~=3.1 Requires-Dist: pydantic~=1.0 Requires-Dist: cachetools Requires-
-Dist: pre-commit ; extra == "dev" Requires-Dist: mkdocs ; extra == "docs"
-Requires-Dist: mkdocs-material ; extra == "docs" Requires-Dist: pygments ;
-extra == "docs" Requires-Dist: rasterio>=1.2.1 ; extra == "rasterio" Requires-
-Dist: mercantile ; extra == "test" Requires-Dist: pytest ; extra == "test"
-Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: rasterio>=1.2.1 ;
-extra == "test" Project-URL: Documentation, https://developmentseed.org/
-morecantile/ Project-URL: Source, https://github.com/developmentseed/
-morecantile Provides-Extra: dev Provides-Extra: docs Provides-Extra: rasterio
-Provides-Extra: test # Morecantile
+pyproj~=3.1 Requires-Dist: pydantic~=2.0 Requires-Dist: pre-commit ; extra ==
+"dev" Requires-Dist: mkdocs ; extra == "docs" Requires-Dist: mkdocs-material ;
+extra == "docs" Requires-Dist: pygments ; extra == "docs" Requires-Dist:
+rasterio>=1.2.1 ; extra == "rasterio" Requires-Dist: mercantile ; extra ==
+"test" Requires-Dist: pytest ; extra == "test" Requires-Dist: pytest-cov ;
+extra == "test" Requires-Dist: rasterio>=1.2.1 ; extra == "test" Project-URL:
+Documentation, https://developmentseed.org/morecantile/ Project-URL: Source,
+https://github.com/developmentseed/morecantile Provides-Extra: dev Provides-
+Extra: docs Provides-Extra: rasterio Provides-Extra: test # Morecantile
 [https://github.com/developmentseed/morecantile/assets/10407788/a1523c6d-e255-
                             4dc6-a201-20029715858a]
          Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
            [Test] [Coverage] [Package_version] [Downloads] [License]
 --- **Documentation**: https://developmentseed.org/morecantile/ **Source
 Code**: https://github.com/developmentseed/morecantile --- Morecantile is like
 [mercantile](https://github.com/mapbox/mercantile) (the best tool to work with
 Web Mercator tile indexes), but with support for other TileMatrixSet grids.
 **Morecantile** follows the **OGC Two Dimensional Tile Matrix Set**
 specification **2.0** found in [https://docs.ogc.org/is/17-083r4/17-083r4.html]
 (https://docs.ogc.org/is/17-083r4/17-083r4.html) | Morecantile Version | OGC
 Specification Version | Link | ------------------- | ------------------------
-- |--------- | 4.0 | 2.0 | https://docs.ogc.org/is/17-083r4/17-083r4.html | 3.0
-and earlier | 1.0 | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html
-**Note**: Variable matrix width tile set are not supported. ## Install ```bash
-$ python -m pip install -U pip $ python -m pip install morecantile # Or install
-from source: $ python -m pip install -U pip $ python -m pip install git+https:/
-/github.com/developmentseed/morecantile.git ``` ## Usage ```python import
-morecantile tms = morecantile.tms.get("WebMercatorQuad") # Get TMS bounding box
-print(tms.xy_bbox) >>> BoundingBox( left=-20037508.342789244, bottom=-
-20037508.34278919, right=20037508.34278919, top=20037508.342789244, ) # Get the
-bounds for tile Z=4, X=10, Y=10 in the TMS's CRS (e.g epsg:3857) print
-(tms.xy_bounds(morecantile.Tile(10, 10, 4))) >>> BoundingBox
-( left=5009377.085697308, bottom=-7514065.628545959, right=7514065.628545959,
-top=-5009377.085697308, ) # Get the bounds for tile Z=4, X=10, Y=10 in
-Geographic CRS (e.g epsg:4326) print(tms.bounds(morecantile.Tile(10, 10, 4)))
->>> BoundingBox( left=44.999999999999964, bottom=-55.776573018667634,
-right=67.4999999999999, top=-40.97989806962009, ) ``` More info can be found at
-https://developmentseed.org/morecantile/usage/ ### Defaults Grids `morecantile`
-provides a set of default TMS grids: - **CanadianNAD83_LCC**: Lambert conformal
-conic NAD83 for Canada - EPSG:3978 - **EuropeanETRS89_LAEAQuad**: ETRS89-
-extended / LAEA Europe - EPGS:3035 - **LINZAntarticaMapTilegrid**: LINZ
-Antarctic Map Tile Grid (Ross Sea Region) - EPSG:5482 - **NZTM2000Quad**: LINZ
-NZTM2000 Map Tile Grid - EPSG:2193 - **UPSAntarcticWGS84Quad**: Universal Polar
-Stereographic WGS 84 Quad for Antarctic - EPSG:5042 - **UPSArcticWGS84Quad**:
-Universal Polar Stereographic WGS 84 Quad for Arctic - EPSG:5041 -
-**UTM31WGS84Quad**: Example of UTM grid - EPSG:32631 - **WebMercatorQuad**:
-Spherical Mercator - EPGS:3857 (default grid for Web Mercator based maps) -
-**WGS1984Quad**: EPSG:4326 for the World - EPGS:4326 (WGS84) -
-**WorldCRS84Quad**: CRS84 for the World - **WorldMercatorWGS84Quad**:
-Elliptical Mercator projection - EPGS:3395 ref: https://schemas.opengis.net/
-tms/2.0/json/examples/tilematrixset/ ## Implementations - [rio-tiler](https://
-github.com/cogeotiff/rio-tiler): Create tile from raster using Morecantile TMS.
-- [titiler](https://github.com/developmentseed/titiler): A modern dynamic tile
+- |--------- | >=4.0 | 2.0 | https://docs.ogc.org/is/17-083r4/17-083r4.html |
+=<3.0 | 1.0 | http://docs.opengeospatial.org/is/17-083r2/17-083r2.html ##
+Install ```bash $ python -m pip install -U pip $ python -m pip install
+morecantile # Or install from source: $ python -m pip install -U pip $ python -
+m pip install git+https://github.com/developmentseed/morecantile.git ``` ##
+Usage ```python import morecantile tms = morecantile.tms.get("WebMercatorQuad")
+# Get TMS bounding box print(tms.xy_bbox) >>> BoundingBox( left=-
+20037508.342789244, bottom=-20037508.34278919, right=20037508.34278919,
+top=20037508.342789244, ) # Get the bounds for tile Z=4, X=10, Y=10 in the
+TMS's CRS (e.g epsg:3857) print(tms.xy_bounds(morecantile.Tile(10, 10, 4))) >>>
+BoundingBox( left=5009377.085697308, bottom=-7514065.628545959,
+right=7514065.628545959, top=-5009377.085697308, ) # Get the bounds for tile
+Z=4, X=10, Y=10 in Geographic CRS (e.g epsg:4326) print(tms.bounds
+(morecantile.Tile(10, 10, 4))) >>> BoundingBox( left=44.999999999999964,
+bottom=-55.776573018667634, right=67.4999999999999, top=-40.97989806962009, )
+``` More info can be found at https://developmentseed.org/morecantile/usage/
+### Defaults Grids `morecantile` provides a set of default TileMatrixSets: -
+**CDB1GlobalGrid** \*: CDB 1 Global Grid - EPGS:4326 (WGS84) -
+**CanadianNAD83_LCC**: Lambert conformal conic NAD83 for Canada - EPSG:3978 -
+**EuropeanETRS89_LAEAQuad**: ETRS89-extended / LAEA Europe - EPGS:3035 -
+**GNOSISGlobalGrid** \*: GNOSIS Global Grid - EPGS:4326 (WGS84) -
+**LINZAntarticaMapTilegrid**: LINZ Antarctic Map Tile Grid (Ross Sea Region) -
+EPSG:5482 - **NZTM2000Quad**: LINZ NZTM2000 Map Tile Grid - EPSG:2193 -
+**UPSAntarcticWGS84Quad**: Universal Polar Stereographic WGS 84 Quad for
+Antarctic - EPSG:5042 - **UPSArcticWGS84Quad**: Universal Polar Stereographic
+WGS 84 Quad for Arctic - EPSG:5041 - **UTM31WGS84Quad**: Example of UTM grid -
+EPSG:32631 - **WebMercatorQuad**: Spherical Mercator - EPGS:3857 (default grid
+for Web Mercator based maps) - **WGS1984Quad**: EPSG:4326 for the World - EPGS:
+4326 (WGS84) - **WorldCRS84Quad**: CRS84 for the World -
+**WorldMercatorWGS84Quad**: Elliptical Mercator projection - EPGS:3395 \*
+TileMatrixSets with variable Matrix Width (see https://docs.ogc.org/is/17-
+083r4/17-083r4.html#toc15) ref: https://schemas.opengis.net/tms/2.0/json/
+examples/tilematrixset/ ## Implementations - [rio-tiler](https://github.com/
+cogeotiff/rio-tiler): Create tile from raster using Morecantile TMS. -
+[titiler](https://github.com/developmentseed/titiler): A modern dynamic tile
 server built on top of FastAPI and Rasterio/GDAL. - [tipg](https://github.com/
 developmentseed/tipg): OGC Features and Tiles API. - [planetcantile](https://
 github.com/AndrewAnnex/planetcantile): Tile matrix sets for other planets. -
 [supermorecado](https://github.com/developmentseed/supermorecado): Extend the
 functionality of morecantile with additional commands. ## Changes See
 [CHANGES.md](https://github.com/developmentseed/morecantile/blob/main/
 CHANGES.md). ## Contribution & Development See [CONTRIBUTING.md](https://
```

