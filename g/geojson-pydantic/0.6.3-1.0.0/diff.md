# Comparing `tmp/geojson_pydantic-0.6.3.tar.gz` & `tmp/geojson_pydantic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson_pydantic-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geojson_pydantic-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geojson_pydantic-0.6.3.tar` & `geojson_pydantic-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      220 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/.bumpversion.cfg
--rw-r--r--   0        0        0     1173 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/.gitignore
--rw-r--r--   0        0        0      797 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/LICENSE
--rw-r--r--   0        0        0     7913 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/README.md
--rw-r--r--   0        0        0      448 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/__init__.py
--rw-r--r--   0        0        0     1906 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/features.py
--rw-r--r--   0        0        0      705 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/geo_interface.py
--rw-r--r--   0        0        0    10976 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/geometries.py
--rw-r--r--   0        0        0        0 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/py.typed
--rw-r--r--   0        0        0     1696 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/types.py
--rw-r--r--   0        0        0     2271 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     8922 1970-01-01 00:00:00.000000 geojson_pydantic-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      220 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1173 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/.gitignore
+-rw-r--r--   0        0        0      797 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2892 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/README.md
+-rw-r--r--   0        0        0      448 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/geojson_pydantic/__init__.py
+-rw-r--r--   0        0        0     2612 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/geojson_pydantic/base.py
+-rw-r--r--   0        0        0     1564 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/geojson_pydantic/features.py
+-rw-r--r--   0        0        0    10662 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/geojson_pydantic/geometries.py
+-rw-r--r--   0        0        0        0 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/geojson_pydantic/py.typed
+-rw-r--r--   0        0        0      647 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/geojson_pydantic/types.py
+-rw-r--r--   0        0        0     2254 2023-07-24 09:04:56.209304 geojson_pydantic-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 geojson_pydantic-1.0.0/PKG-INFO
```

### Comparing `geojson_pydantic-0.6.3/.gitignore` & `geojson_pydantic-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-0.6.3/.pre-commit-config.yaml` & `geojson_pydantic-1.0.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
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
         # No reason to run if only tests have changed. They intentionally break typing.
         exclude: tests/.*
         additional_dependencies:
-        - pydantic~=1.0
+        - pydantic~=2.0
```

### Comparing `geojson_pydantic-0.6.3/LICENSE` & `geojson_pydantic-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-0.6.3/geojson_pydantic/features.py` & `geojson_pydantic-1.0.0/geojson_pydantic/features.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 """pydantic models for GeoJSON Feature objects."""
 
 from typing import Any, Dict, Generic, Iterator, List, Literal, Optional, TypeVar, Union
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
-from pydantic.generics import GenericModel
+from pydantic import BaseModel, Field, StrictInt, StrictStr, field_validator
 
-from geojson_pydantic.geo_interface import GeoInterfaceMixin
-from geojson_pydantic.geometries import Geometry, GeometryCollection
-from geojson_pydantic.types import BBox, validate_bbox
+from geojson_pydantic.base import _GeoJsonBase
+from geojson_pydantic.geometries import Geometry
 
 Props = TypeVar("Props", bound=Union[Dict[str, Any], BaseModel])
-Geom = TypeVar("Geom", bound=Union[Geometry, GeometryCollection])
+Geom = TypeVar("Geom", bound=Geometry)
 
 
-class Feature(GenericModel, Generic[Geom, Props], GeoInterfaceMixin):
+class Feature(_GeoJsonBase, Generic[Geom, Props]):
     """Feature Model"""
 
     type: Literal["Feature"]
     geometry: Union[Geom, None] = Field(...)
     properties: Union[Props, None] = Field(...)
     id: Optional[Union[StrictInt, StrictStr]] = None
-    bbox: Optional[BBox] = None
 
-    _validate_bbox = validator("bbox", allow_reuse=True)(validate_bbox)
+    __geojson_exclude_if_none__ = {"bbox", "id"}
 
-    @validator("geometry", pre=True, always=True)
+    @field_validator("geometry", mode="before")
     def set_geometry(cls, geometry: Any) -> Any:
         """set geometry from geo interface or input"""
         if hasattr(geometry, "__geo_interface__"):
             return geometry.__geo_interface__
 
         return geometry
 
 
-class FeatureCollection(GenericModel, Generic[Geom, Props], GeoInterfaceMixin):
+Feat = TypeVar("Feat", bound=Feature)
+
+
+class FeatureCollection(_GeoJsonBase, Generic[Feat]):
     """FeatureCollection Model"""
 
     type: Literal["FeatureCollection"]
-    features: List[Feature[Geom, Props]]
-    bbox: Optional[BBox] = None
+    features: List[Feat]
 
-    def __iter__(self) -> Iterator[Feature]:  # type: ignore [override]
+    def __iter__(self) -> Iterator[Feat]:  # type: ignore [override]
         """iterate over features"""
         return iter(self.features)
 
     def __len__(self) -> int:
         """return features length"""
         return len(self.features)
 
-    def __getitem__(self, index: int) -> Feature:
+    def __getitem__(self, index: int) -> Feat:
         """get feature at a given index"""
         return self.features[index]
-
-    _validate_bbox = validator("bbox", allow_reuse=True)(validate_bbox)
```

### Comparing `geojson_pydantic-0.6.3/geojson_pydantic/geometries.py` & `geojson_pydantic-1.0.0/geojson_pydantic/geometries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """pydantic models for GeoJSON Geometry objects."""
 from __future__ import annotations
 
 import abc
 import warnings
-from typing import Any, Iterator, List, Literal, Optional, Union
+from typing import Any, Iterator, List, Literal, Union
 
-from pydantic import BaseModel, Field, ValidationError, validator
-from pydantic.error_wrappers import ErrorWrapper
+from pydantic import Field, field_validator
 from typing_extensions import Annotated
 
-from geojson_pydantic.geo_interface import GeoInterfaceMixin
+from geojson_pydantic.base import _GeoJsonBase
 from geojson_pydantic.types import (
-    BBox,
     LinearRing,
     LineStringCoords,
     MultiLineStringCoords,
     MultiPointCoords,
     MultiPolygonCoords,
     PolygonCoords,
     Position,
-    validate_bbox,
 )
 
 
 def _position_wkt_coordinates(coordinates: Position, force_z: bool = False) -> str:
     """Converts a Position to WKT Coordinates."""
     wkt_coordinates = " ".join(str(number) for number in coordinates)
     if force_z and len(coordinates) < 3:
@@ -64,25 +61,24 @@
         _position_has_z(position) for positions in lines for position in positions
     )
 
 
 def _polygons_wkt_coordinates(
     coordinates: List[PolygonCoords], force_z: bool = False
 ) -> str:
-    return ",".join(
+    return ", ".join(
         f"({_lines_wtk_coordinates(polygon, force_z)})" for polygon in coordinates
     )
 
 
-class _GeometryBase(BaseModel, abc.ABC, GeoInterfaceMixin):
+class _GeometryBase(_GeoJsonBase, abc.ABC):
     """Base class for geometry models"""
 
     type: str
     coordinates: Any
-    bbox: Optional[BBox] = None
 
     @abc.abstractmethod
     def __wkt_coordinates__(self, coordinates: Any, force_z: bool) -> str:
         """return WKT coordinates."""
         ...
 
     @property
@@ -104,16 +100,14 @@
             wkt += f"({self.__wkt_coordinates__(self.coordinates, force_z=has_z)})"
         else:
             # Otherwise it will be "EMPTY"
             wkt += " EMPTY"
 
         return wkt
 
-    _validate_bbox = validator("bbox", allow_reuse=True)(validate_bbox)
-
 
 class Point(_GeometryBase):
     """Point Model"""
 
     type: Literal["Point"]
     coordinates: Position
 
@@ -131,15 +125,18 @@
     """MultiPoint Model"""
 
     type: Literal["MultiPoint"]
     coordinates: MultiPointCoords
 
     def __wkt_coordinates__(self, coordinates: Any, force_z: bool) -> str:
         """return WKT coordinates."""
-        return _position_list_wkt_coordinates(coordinates, force_z)
+        return ", ".join(
+            f"({_position_wkt_coordinates(position, force_z)})"
+            for position in coordinates
+        )
 
     @property
     def has_z(self) -> bool:
         """Checks if any coordinate has a Z value."""
         return _position_list_has_z(self.coordinates)
 
 
@@ -181,15 +178,15 @@
     type: Literal["Polygon"]
     coordinates: PolygonCoords
 
     def __wkt_coordinates__(self, coordinates: Any, force_z: bool) -> str:
         """return WKT coordinates."""
         return _lines_wtk_coordinates(coordinates, force_z)
 
-    @validator("coordinates")
+    @field_validator("coordinates")
     def check_closure(cls, coordinates: List) -> List:
         """Validate that Polygon is closed (first and last coordinate are the same)."""
         if any(ring[-1] != ring[0] for ring in coordinates):
             raise ValueError("All linear rings have the same start and end coordinates")
 
         return coordinates
 
@@ -234,45 +231,38 @@
         return _polygons_wkt_coordinates(coordinates, force_z)
 
     @property
     def has_z(self) -> bool:
         """Checks if any coordinates have a Z value."""
         return any(_lines_has_z(polygon) for polygon in self.coordinates)
 
-    @validator("coordinates")
+    @field_validator("coordinates")
     def check_closure(cls, coordinates: List) -> List:
         """Validate that Polygon is closed (first and last coordinate are the same)."""
         if any(ring[-1] != ring[0] for polygon in coordinates for ring in polygon):
             raise ValueError("All linear rings have the same start and end coordinates")
 
         return coordinates
 
 
-Geometry = Annotated[
-    Union[Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon],
-    Field(discriminator="type"),
-]
-
-
-class GeometryCollection(BaseModel, GeoInterfaceMixin):
+class GeometryCollection(_GeoJsonBase):
     """GeometryCollection Model"""
 
     type: Literal["GeometryCollection"]
-    geometries: List[Union[Geometry, GeometryCollection]]
-    bbox: Optional[BBox] = None
+    geometries: List[Geometry]
 
-    def __iter__(self) -> Iterator[Union[Geometry, GeometryCollection]]:  # type: ignore [override]
+    def __iter__(self) -> Iterator[Geometry]:  # type: ignore [override]
         """iterate over geometries"""
         return iter(self.geometries)
 
     def __len__(self) -> int:
         """return geometries length"""
         return len(self.geometries)
 
-    def __getitem__(self, index: int) -> Union[Geometry, GeometryCollection]:
+    def __getitem__(self, index: int) -> Geometry:
         """get geometry at a given index"""
         return self.geometries[index]
 
     @property
     def wkt(self) -> str:
         """Return the Well Known Text representation."""
         # Each geometry will check its own coordinates for Z and include "Z" in the wkt
@@ -286,55 +276,74 @@
             if self.geometries
             else "EMPTY"
         )
         # If any of them contain `Z` add Z to the output wkt
         z = " Z " if "Z" in geometries else " "
         return f"{self.type.upper()}{z}{geometries}"
 
-    _validate_bbox = validator("bbox", allow_reuse=True)(validate_bbox)
-
-    @validator("geometries")
+    @field_validator("geometries")
     def check_geometries(cls, geometries: List) -> List:
         """Add warnings for conditions the spec does not explicitly forbid."""
         if len(geometries) == 1:
             warnings.warn(
                 "GeometryCollection should not be used for single geometries."
             )
+
         if any(geom.type == "GeometryCollection" for geom in geometries):
             warnings.warn(
                 "GeometryCollection should not be used for nested GeometryCollections."
             )
+
         if len({geom.type for geom in geometries}) == 1:
             warnings.warn(
                 "GeometryCollection should not be used for homogeneous collections."
             )
+
         return geometries
 
 
+Geometry = Annotated[
+    Union[
+        Point,
+        MultiPoint,
+        LineString,
+        MultiLineString,
+        Polygon,
+        MultiPolygon,
+        GeometryCollection,
+    ],
+    Field(discriminator="type"),
+]
+
+GeometryCollection.model_rebuild()
+
+
 def parse_geometry_obj(obj: Any) -> Geometry:
     """
     `obj` is an object that is supposed to represent a GeoJSON geometry. This method returns the
     reads the `"type"` field and returns the correct pydantic Geometry model.
     """
     if "type" not in obj:
-        raise ValidationError(
-            errors=[
-                ErrorWrapper(ValueError("Missing 'type' field in geometry"), loc="type")
-            ],
-            model=_GeometryBase,
-        )
+        raise ValueError("Missing 'type' field in geometry")
+
     if obj["type"] == "Point":
-        return Point.parse_obj(obj)
+        return Point.model_validate(obj)
+
     elif obj["type"] == "MultiPoint":
-        return MultiPoint.parse_obj(obj)
+        return MultiPoint.model_validate(obj)
+
     elif obj["type"] == "LineString":
-        return LineString.parse_obj(obj)
+        return LineString.model_validate(obj)
+
     elif obj["type"] == "MultiLineString":
-        return MultiLineString.parse_obj(obj)
+        return MultiLineString.model_validate(obj)
+
     elif obj["type"] == "Polygon":
-        return Polygon.parse_obj(obj)
+        return Polygon.model_validate(obj)
+
     elif obj["type"] == "MultiPolygon":
-        return MultiPolygon.parse_obj(obj)
-    raise ValidationError(
-        errors=[ErrorWrapper(ValueError("Unknown type"), loc="type")],
-        model=_GeometryBase,
-    )
+        return MultiPolygon.model_validate(obj)
+
+    elif obj["type"] == "GeometryCollection":
+        return GeometryCollection.model_validate(obj)
+
+    raise ValueError(f"Unknown type: {obj['type']}")
```

### Comparing `geojson_pydantic-0.6.3/pyproject.toml` & `geojson_pydantic-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,24 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
-dependencies = ["pydantic~=1.0"]
+dependencies = ["pydantic~=2.0"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "shapely"]
 dev = ["pre-commit"]
+docs = [
+    "mkdocs",
+    "mkdocs-material",
+    "pygments",
+]
 
 [project.urls]
 Source = "https://github.com/developmentseed/geojson-pydantic"
 
 [build-system]
 requires = ["flit>=3.2,<4"]
 build-backend = "flit_core.buildapi"
@@ -84,10 +89,8 @@
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
 ]
 
 [tool.ruff.per-file-ignores]
-"tests/test_geometries.py" = ["D1"]
-"tests/test_features.py" = ["D1"]
-"tests/test_package.py" = ["D1"]
+"tests/*.py" = ["D1"]
```

