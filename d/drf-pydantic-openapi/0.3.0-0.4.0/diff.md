# Comparing `tmp/drf_pydantic_openapi-0.3.0.tar.gz` & `tmp/drf_pydantic_openapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pydantic_openapi-0.3.0.tar", max compression
+gzip compressed data, was "drf_pydantic_openapi-0.4.0.tar", max compression
```

## Comparing `drf_pydantic_openapi-0.3.0.tar` & `drf_pydantic_openapi-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.3.0/LICENSE
--rw-r--r--   0        0        0     2596 2023-05-09 09:59:45.223778 drf_pydantic_openapi-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/__init__.py
--rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/apps.py
--rw-r--r--   0        0        0     1456 2023-05-08 13:59:43.276920 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/errors.py
--rw-r--r--   0        0        0      489 2023-04-27 13:44:28.146816 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/exception_handler.py
--rw-r--r--   0        0        0     5780 2023-06-02 09:32:51.712376 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/generator.py
--rw-r--r--   0        0        0     2289 2023-06-02 08:27:03.420495 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/patches.py
--rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/path.py
--rw-r--r--   0        0        0     1517 2023-05-23 13:35:05.835776 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/ref_source.py
--rw-r--r--   0        0        0     4143 2023-05-26 14:34:32.395942 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/ref_utils.py
--rw-r--r--   0        0        0      885 2023-06-02 08:31:26.725739 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/settings.py
--rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
--rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
--rw-r--r--   0        0        0      256 2023-06-01 11:25:29.626778 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/urls.py
--rw-r--r--   0        0        0     3938 2023-06-02 09:26:21.617715 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/utils.py
--rw-r--r--   0        0        0     1720 2023-06-02 09:33:50.952500 drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/views.py
--rw-r--r--   0        0        0     1230 2023-06-02 09:34:18.528242 drf_pydantic_openapi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2596 2023-05-09 09:59:45.223778 drf_pydantic_openapi-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/apps.py
+-rw-r--r--   0        0        0     1456 2023-05-08 13:59:43.276920 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/errors.py
+-rw-r--r--   0        0        0      489 2023-04-27 13:44:28.146816 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/exception_handler.py
+-rw-r--r--   0        0        0     6091 2023-07-24 14:03:27.394681 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/generator.py
+-rw-r--r--   0        0        0     2289 2023-06-02 08:27:03.420495 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/patches.py
+-rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/path.py
+-rw-r--r--   0        0        0     1517 2023-05-23 13:35:05.835776 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/ref_source.py
+-rw-r--r--   0        0        0     4143 2023-05-26 14:34:32.395942 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/ref_utils.py
+-rw-r--r--   0        0        0     1112 2023-07-24 14:01:09.538626 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/settings.py
+-rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
+-rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
+-rw-r--r--   0        0        0      246 2023-07-24 13:38:54.240481 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/urls.py
+-rw-r--r--   0        0        0     4085 2023-07-24 13:43:20.072536 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/utils.py
+-rw-r--r--   0        0        0     2186 2023-07-24 14:04:40.140850 drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/views.py
+-rw-r--r--   0        0        0     1230 2023-07-24 14:05:12.043190 drf_pydantic_openapi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.4.0/PKG-INFO
```

### Comparing `drf_pydantic_openapi-0.3.0/LICENSE` & `drf_pydantic_openapi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.3.0/README.md` & `drf_pydantic_openapi-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/errors.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/errors.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/generator.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 
 from django.urls import get_resolver
 from openapi_schema_pydantic import (
     Info,
     MediaType,
     OpenAPI,
     Operation,
-    PathItem,
     RequestBody,
     Response,
 )
 from openapi_schema_pydantic.util import (
     PydanticSchema,
     construct_open_api_with_schema_class,
 )
 from pydantic import BaseModel
 from rest_framework.schemas.generators import BaseSchemaGenerator
 
 from .path import Path
 from .settings import config
-from .utils import Docstring, ParameterLocation, get_view_version, method_mapping
+from .utils import Docstring, ParameterLocation, PathItemEx, get_view_version, method_mapping
 
 
 class Document(BaseSchemaGenerator):
     def __init__(self, api_version: str, tag_path_regex: str | None, *args, **kwargs) -> None:
         self.api_version = api_version
         self.tag_path_regex = tag_path_regex
-        self.openapi = OpenAPI(info=Info(title="test", version="3.0.0"), paths={})
+        # TODO: change info
+        self.openapi = OpenAPI(openapi=config.openapi_version, info=Info(title="DPO API", version="0.0.4"), paths={})
         self.responses = {}
         super().__init__(*args, **kwargs)
 
     @property
     def _tag_path_regex(self):
         # Get path prefix regex
         return self.tag_path_regex if self.tag_path_regex else config.tag_path_regex
@@ -113,18 +113,22 @@
             responses=self.generate_responses(docstring, view_func),
             summary=docstring.short_description if docstring else "",
             description=docstring.long_description if docstring else "",
             parameters=parameters,
         )
 
     def generate_docs(self, paths: list[Path]):
-        docs = PathItem()
+        docs = PathItemEx()
         for path in paths:
             if operation := self.generate_operation(path):
-                setattr(docs, path.method.lower(), operation)
+                if not config.include_empty_endpoints:
+                    if operation.responses:
+                        setattr(docs, path.method.lower(), operation)
+                else:
+                    setattr(docs, path.method.lower(), operation)
         return docs
 
     def get_schema(self, request=None, public=False):
         self._initialise_endpoints()
         _, view_endpoints = self._get_paths_and_endpoints(request)
         paths = defaultdict(list)
         path_prefix = self.find_path_prefix(view_endpoints)
@@ -141,12 +145,13 @@
                     path_prefix=path_prefix,
                     method=method,
                     view=view,
                 )
             )
 
         for path in paths.keys():
-            docs = self.generate_docs(paths[path])
-            self.openapi.paths[path] = docs
+            if docs := self.generate_docs(paths[path]):
+                if not docs.is_empty():
+                    self.openapi.paths[path] = docs
 
         self.openapi = construct_open_api_with_schema_class(self.openapi)
         return self.openapi.json(by_alias=True, exclude_none=True)
```

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/patches.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/patches.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/path.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/path.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/ref_source.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/ref_source.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/ref_utils.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/ref_utils.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/settings.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 
 from .ref_source import RefSource
 
 
 class Config(BaseModel):
     ref_sources: dict[str, RefSource] = Field(default={}, alias="REF_SOURCES")
     tag_path_regex: str = Field(default=None, alias="TAG_PATH_REGEX")
+    openapi_version: str = Field(default="3.1.0", alias="OPENAPI_VERSION")
+    include_empty_endpoints: bool = Field(default=True, alias="INCLUDE_EMPTY_ENDPOINTS")
 
     def get_source(self, name: str) -> RefSource | None:
         """Find source by given source name"""
         if ref_source := self.ref_sources.get(name):
             try:
                 ref_source.init()
                 return ref_source
             except Exception as e:
                 logger.warning(f"Error while initializing the {name} source: {str(e)}")
 
 
 USER_SETTINGS = getattr(settings, "DRF_PYDANTIC_OPENAPI", {"REF_SOURCES": {}})
 
-config = Config(
-    **{"REF_SOURCES": {name: RefSource(name, value) for name, value in USER_SETTINGS["REF_SOURCES"].items()}}
-)
+# Override ref_sources to use the class
+USER_SETTINGS["REF_SOURCES"] = {name: RefSource(name, value) for name, value in USER_SETTINGS["REF_SOURCES"].items()}
+
+config = Config(**USER_SETTINGS)
```

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/utils.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import builtins
 import re
 from enum import Enum
 from inspect import isclass
 from typing import Type
 
 import docstring_parser
-from openapi_schema_pydantic import Parameter, Schema
+from openapi_schema_pydantic import Parameter, PathItem, Schema
 from openapi_schema_pydantic.util import PydanticSchema
 from pydantic import BaseModel
 from rest_framework import exceptions
 
 from .errors import HttpError
 
 method_mapping = {
@@ -125,7 +125,12 @@
 
 def get_view_version(view) -> str:
     try:
         version, _ = view.determine_version(view.request, **view.kwargs)
         return str(version)
     except exceptions.NotAcceptable:
         return ""
+
+
+class PathItemEx(PathItem):
+    def is_empty(self):
+        return not (self.get or self.post or self.delete or self.head or self.put)
```

### Comparing `drf_pydantic_openapi-0.3.0/drf_pydantic_openapi/views.py` & `drf_pydantic_openapi-0.4.0/drf_pydantic_openapi/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,42 @@
 from rest_framework.response import Response
 from rest_framework.reverse import reverse
 from rest_framework.views import APIView
 
 from .generator import Document
 
 
-class DrfPydanticSchemaView(APIView):
-    authentication_classes = {}
-    permission_classes = {}
-    api_version = None
-    tag_path_regex = None
+def get_schema_view(
+    api_version=None,
+    tag_path_regex=None,
+    permission_classes=None,
+    authentication_classes=None,
+):
+    _api_version = api_version
+    _tag_path_regex = tag_path_regex
+    _permission_classes = permission_classes if permission_classes else {}
+    _authentication_classes = authentication_classes if authentication_classes else {}
+
+    class DrfPydanticSchemaView(APIView):
+        authentication_classes = _authentication_classes
+        permission_classes = _permission_classes
+
+        def get(self, request, *args, **kwargs):
+            version = _api_version
+            if hasattr(request, "version"):
+                version = request.version
+
+            document = Document(
+                api_version=version,
+                tag_path_regex=_tag_path_regex,
+            )
+            schema = document.get_schema(request=request)
+            return Response(json.loads(schema), headers={"Cache-Control": "no-cache, no-store, must-revalidate"})
 
-    def get(self, request, *args, **kwargs):
-        version = self.api_version
-        if hasattr(request, "version"):
-            version = request.version
-
-        document = Document(api_version=version, tag_path_regex=self.tag_path_regex)
-        schema = document.get_schema(request=request)
-        return Response(json.loads(schema), headers={"Cache-Control": "no-cache, no-store, must-revalidate"})
+    return DrfPydanticSchemaView
 
 
 class DrfPydanticRedocView(TemplateView):
     api_version = None
     template_name = "drf_pydantic_openapi/redoc.html"
     url_name = "dpo_schema"
```

### Comparing `drf_pydantic_openapi-0.3.0/pyproject.toml` & `drf_pydantic_openapi-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-pydantic-openapi"
-version = "0.3.0"
+version = "0.4.0"
 description = "OpenAPI (v3) schema generation via Pydantic models using Django REST Framework."
 authors = ["iKlotho <umutkahrimanedu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drf_pydantic_openapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `drf_pydantic_openapi-0.3.0/PKG-INFO` & `drf_pydantic_openapi-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-pydantic-openapi
-Version: 0.3.0
+Version: 0.4.0
 Summary: OpenAPI (v3) schema generation via Pydantic models using Django REST Framework.
 Author: iKlotho
 Author-email: umutkahrimanedu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

