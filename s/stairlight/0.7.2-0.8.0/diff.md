# Comparing `tmp/stairlight-0.7.2.tar.gz` & `tmp/stairlight-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stairlight-0.7.2.tar", max compression
+gzip compressed data, was "stairlight-0.8.0.tar", max compression
```

## Comparing `stairlight-0.7.2.tar` & `stairlight-0.8.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1075 2021-10-23 11:41:32.044924 stairlight-0.7.2/LICENSE
--rw-r--r--   0        0        0    13894 2023-02-25 07:28:37.390494 stairlight-0.7.2/README.md
--rw-r--r--   0        0        0     2073 2023-02-25 07:40:16.165919 stairlight-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      197 2023-02-25 07:40:27.636816 stairlight-0.7.2/src/stairlight/__init__.py
--rw-r--r--   0        0        0      130 2023-02-22 17:10:30.825152 stairlight-0.7.2/src/stairlight/__main__.py
--rw-r--r--   0        0        0     9942 2023-02-25 07:16:33.102595 stairlight-0.7.2/src/stairlight/cli.py
--rw-r--r--   0        0        0     9104 2023-02-25 07:28:37.391148 stairlight-0.7.2/src/stairlight/configurator.py
--rw-r--r--   0        0        0    10480 2023-02-22 17:10:30.825906 stairlight-0.7.2/src/stairlight/map.py
--rw-r--r--   0        0        0        0 2022-06-14 11:44:47.716674 stairlight-0.7.2/src/stairlight/py.typed
--rw-r--r--   0        0        0     4403 2023-02-22 17:10:30.826119 stairlight-0.7.2/src/stairlight/query.py
--rw-r--r--   0        0        0        0 2022-06-14 11:44:47.717317 stairlight-0.7.2/src/stairlight/source/__init__.py
--rw-r--r--   0        0        0     6966 2023-02-25 07:28:37.391528 stairlight-0.7.2/src/stairlight/source/config.py
--rw-r--r--   0        0        0     2486 2023-02-22 17:10:30.826604 stairlight-0.7.2/src/stairlight/source/config_key.py
--rw-r--r--   0        0        0     7405 2023-02-22 17:10:30.826848 stairlight-0.7.2/src/stairlight/source/controller.py
--rw-r--r--   0        0        0        0 2022-06-18 04:24:48.115814 stairlight-0.7.2/src/stairlight/source/dbt/__init__.py
--rw-r--r--   0        0        0      880 2023-02-22 17:10:30.827070 stairlight-0.7.2/src/stairlight/source/dbt/config.py
--rw-r--r--   0        0        0     8166 2023-02-22 17:10:30.827317 stairlight-0.7.2/src/stairlight/source/dbt/template.py
--rw-r--r--   0        0        0        0 2022-06-18 04:24:48.116498 stairlight-0.7.2/src/stairlight/source/file/__init__.py
--rw-r--r--   0        0        0      737 2023-02-22 17:10:30.827555 stairlight-0.7.2/src/stairlight/source/file/config.py
--rw-r--r--   0        0        0     2866 2023-02-22 17:10:30.827814 stairlight-0.7.2/src/stairlight/source/file/template.py
--rw-r--r--   0        0        0        0 2022-06-18 04:24:48.117151 stairlight-0.7.2/src/stairlight/source/gcs/__init__.py
--rw-r--r--   0        0        0      755 2023-02-22 17:10:30.828091 stairlight-0.7.2/src/stairlight/source/gcs/config.py
--rw-r--r--   0        0        0      509 2023-02-22 17:10:30.828319 stairlight-0.7.2/src/stairlight/source/gcs/map.py
--rw-r--r--   0        0        0     3391 2023-02-22 17:10:30.828564 stairlight-0.7.2/src/stairlight/source/gcs/template.py
--rw-r--r--   0        0        0        0 2022-06-18 04:24:48.117695 stairlight-0.7.2/src/stairlight/source/redash/__init__.py
--rw-r--r--   0        0        0      827 2023-02-22 17:10:30.828829 stairlight-0.7.2/src/stairlight/source/redash/config.py
--rw-r--r--   0        0        0      179 2023-02-16 13:21:19.912956 stairlight-0.7.2/src/stairlight/source/redash/sql/redash_queries.sql
--rw-r--r--   0        0        0     5410 2023-02-22 17:10:30.829091 stairlight-0.7.2/src/stairlight/source/redash/template.py
--rw-r--r--   0        0        0        0 2022-06-25 05:53:09.840666 stairlight-0.7.2/src/stairlight/source/s3/__init__.py
--rw-r--r--   0        0        0      751 2023-02-22 17:10:30.829330 stairlight-0.7.2/src/stairlight/source/s3/config.py
--rw-r--r--   0        0        0      516 2023-02-22 17:10:30.829558 stairlight-0.7.2/src/stairlight/source/s3/map.py
--rw-r--r--   0        0        0     3840 2023-02-22 17:10:30.829767 stairlight-0.7.2/src/stairlight/source/s3/template.py
--rw-r--r--   0        0        0     8977 2023-02-22 17:10:30.830026 stairlight-0.7.2/src/stairlight/source/template.py
--rw-r--r--   0        0        0    17919 2023-02-25 07:28:37.392413 stairlight-0.7.2/src/stairlight/stairlight.py
--rw-r--r--   0        0        0     1751 2023-02-25 07:28:37.392887 stairlight-0.7.2/src/stairlight/util.py
--rw-r--r--   0        0        0    15772 1970-01-01 00:00:00.000000 stairlight-0.7.2/setup.py
--rw-r--r--   0        0        0    15265 1970-01-01 00:00:00.000000 stairlight-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2021-10-23 11:41:32.044924 stairlight-0.8.0/LICENSE
+-rw-r--r--   0        0        0    13894 2023-07-24 06:27:53.637920 stairlight-0.8.0/README.md
+-rw-r--r--   0        0        0     2071 2023-07-24 11:56:05.652624 stairlight-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      364 2023-07-24 11:54:58.181852 stairlight-0.8.0/src/stairlight/__init__.py
+-rw-r--r--   0        0        0      130 2023-02-22 17:10:30.825152 stairlight-0.8.0/src/stairlight/__main__.py
+-rw-r--r--   0        0        0    10372 2023-07-24 11:54:58.182114 stairlight-0.8.0/src/stairlight/cli.py
+-rw-r--r--   0        0        0     8537 2023-07-24 11:54:58.182263 stairlight-0.8.0/src/stairlight/configurator.py
+-rw-r--r--   0        0        0    12545 2023-07-24 11:54:58.182542 stairlight-0.8.0/src/stairlight/map.py
+-rw-r--r--   0        0        0        0 2022-06-14 11:44:47.716674 stairlight-0.8.0/src/stairlight/py.typed
+-rw-r--r--   0        0        0     4724 2023-05-04 05:10:54.618092 stairlight-0.8.0/src/stairlight/query.py
+-rw-r--r--   0        0        0        0 2022-06-14 11:44:47.717317 stairlight-0.8.0/src/stairlight/source/__init__.py
+-rw-r--r--   0        0        0     6966 2023-02-25 07:28:37.391528 stairlight-0.8.0/src/stairlight/source/config.py
+-rw-r--r--   0        0        0     2486 2023-02-22 17:10:30.826604 stairlight-0.8.0/src/stairlight/source/config_key.py
+-rw-r--r--   0        0        0     7405 2023-04-30 09:26:10.348398 stairlight-0.8.0/src/stairlight/source/controller.py
+-rw-r--r--   0        0        0        0 2022-06-18 04:24:48.115814 stairlight-0.8.0/src/stairlight/source/dbt/__init__.py
+-rw-r--r--   0        0        0      880 2023-02-22 17:10:30.827070 stairlight-0.8.0/src/stairlight/source/dbt/config.py
+-rw-r--r--   0        0        0     8166 2023-02-22 17:10:30.827317 stairlight-0.8.0/src/stairlight/source/dbt/template.py
+-rw-r--r--   0        0        0        0 2022-06-18 04:24:48.116498 stairlight-0.8.0/src/stairlight/source/file/__init__.py
+-rw-r--r--   0        0        0      737 2023-02-22 17:10:30.827555 stairlight-0.8.0/src/stairlight/source/file/config.py
+-rw-r--r--   0        0        0     2866 2023-02-22 17:10:30.827814 stairlight-0.8.0/src/stairlight/source/file/template.py
+-rw-r--r--   0        0        0        0 2022-06-18 04:24:48.117151 stairlight-0.8.0/src/stairlight/source/gcs/__init__.py
+-rw-r--r--   0        0        0      755 2023-02-22 17:10:30.828091 stairlight-0.8.0/src/stairlight/source/gcs/config.py
+-rw-r--r--   0        0        0      509 2023-02-22 17:10:30.828319 stairlight-0.8.0/src/stairlight/source/gcs/map.py
+-rw-r--r--   0        0        0     3391 2023-02-22 17:10:30.828564 stairlight-0.8.0/src/stairlight/source/gcs/template.py
+-rw-r--r--   0        0        0        0 2022-06-18 04:24:48.117695 stairlight-0.8.0/src/stairlight/source/redash/__init__.py
+-rw-r--r--   0        0        0      827 2023-02-22 17:10:30.828829 stairlight-0.8.0/src/stairlight/source/redash/config.py
+-rw-r--r--   0        0        0      179 2023-02-16 13:21:19.912956 stairlight-0.8.0/src/stairlight/source/redash/sql/redash_queries.sql
+-rw-r--r--   0        0        0     5410 2023-02-22 17:10:30.829091 stairlight-0.8.0/src/stairlight/source/redash/template.py
+-rw-r--r--   0        0        0        0 2022-06-25 05:53:09.840666 stairlight-0.8.0/src/stairlight/source/s3/__init__.py
+-rw-r--r--   0        0        0      751 2023-02-22 17:10:30.829330 stairlight-0.8.0/src/stairlight/source/s3/config.py
+-rw-r--r--   0        0        0      516 2023-02-22 17:10:30.829558 stairlight-0.8.0/src/stairlight/source/s3/map.py
+-rw-r--r--   0        0        0     3840 2023-02-22 17:10:30.829767 stairlight-0.8.0/src/stairlight/source/s3/template.py
+-rw-r--r--   0        0        0     8964 2023-07-24 11:54:58.182818 stairlight-0.8.0/src/stairlight/source/template.py
+-rw-r--r--   0        0        0    23575 2023-07-24 11:54:58.183207 stairlight-0.8.0/src/stairlight/stairlight.py
+-rw-r--r--   0        0        0     1751 2023-02-25 07:28:37.392887 stairlight-0.8.0/src/stairlight/util.py
+-rw-r--r--   0        0        0    15770 1970-01-01 00:00:00.000000 stairlight-0.8.0/setup.py
+-rw-r--r--   0        0        0    15263 1970-01-01 00:00:00.000000 stairlight-0.8.0/PKG-INFO
```

### Comparing `stairlight-0.7.2/LICENSE` & `stairlight-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/README.md` & `stairlight-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/pyproject.toml` & `stairlight-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "stairlight"
-version = "0.7.2"
+version = "0.8.0"
 description = "An end-to-end data lineage tool"
 authors = ["tosh2230 <rev.to12@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src/stairlight" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7.2,<4"
+python = ">=3.8,<4"
 PyYAML = ">=5.0"
 Jinja2 = ">=2.10.3"
 
 # For unit tests
 boto3-stubs = {version = ">=1.24.17", extras = ["s3"]}
 
 # optional dependencies
```

### Comparing `stairlight-0.7.2/src/stairlight/cli.py` & `stairlight-0.8.0/src/stairlight/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import argparse
 import json
 import textwrap
 from typing import Any, Callable
 
 from src import stairlight
+from src.stairlight.map import MappedTemplate
 
 
 def command_init(stairlight: stairlight.StairLight, args: argparse.Namespace) -> str:
     """Execute init command
 
     Args:
         stairlight (StairLight): Stairlight class
@@ -31,20 +32,16 @@
     Args:
         stairlight (StairLight): Stairlight class
         args (argparse.Namespace): CLI arguments
 
     Returns:
         str: return messages
     """
-    message = ""
-    mapping_template_file = stairlight.check()
-    if mapping_template_file:
-        message = mapping_template_file
-
-    return message
+    created_files = stairlight.check()
+    return "\n".join([f for f in created_files if f != ""])
 
 
 def command_list(
     stairlight: stairlight.StairLight, args: argparse.Namespace
 ) -> list[str]:
     """Execute list command
 
@@ -295,15 +292,18 @@
     parser_init.set_defaults(handler=command_init)
     set_general_parser(parser=parser_init)
 
     # map | check
     parser_check = subparsers.add_parser(
         "map",
         aliases=["check"],
-        help="create a new configuration file about undefined mappings",
+        help=(
+            "create a new configuration file about undefined mappings"
+            " and templates not found"
+        ),
     )
     parser_check.set_defaults(handler=command_check)
     set_general_parser(parser=parser_check)
 
     # list
     parser_list = subparsers.add_parser("list", help="return all ( tables | URIs )")
     parser_list.set_defaults(handler=command_list)
@@ -337,30 +337,36 @@
     parser = create_parser()
     args = parser.parse_args()
     _stairlight = stairlight.StairLight(
         config_dir=args.config, load_files=args.load, save_file=args.save
     )
     _stairlight.create_map()
 
-    result = None
+    result_command: Any = None
+    result_mapped: dict[str, dict[str, list[MappedTemplate] | None] | None] = {}
     if hasattr(args, "handler"):
         if args.handler == command_init and _stairlight.has_stairlight_config():
             exit(f"'{args.config}/stairlight.y(a)ml' already exists.")
         elif args.handler != command_init and not _stairlight.has_stairlight_config():
             exit(f"'{args.config}/stairlight.y(a)ml' is not found.")
-        result = args.handler(_stairlight, args)
+        result_command = args.handler(_stairlight, args)
     else:
         if not _stairlight.has_stairlight_config():
             exit(f"'{args.config}/stairlight.y(a)ml' is not found.")
-        result = _stairlight.mapped
+        result_mapped = _stairlight.mapped
 
-    if args.quiet or not result:
+    if args.quiet or (not result_command and not result_mapped):
         return
 
-    if result and isinstance(result, str):
-        print(result)
-    else:
-        print(json.dumps(result, indent=2))
+    if result_command and isinstance(result_command, str):
+        print(result_command)
+    elif result_command:
+        print(json.dumps(result_command, indent=2))
+    elif result_mapped:
+        result_dict: dict[str, Any] = _stairlight.cast_mapped_dict_all(
+            mapped=result_mapped
+        )
+        print(json.dumps(result_dict, indent=2))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `stairlight-0.7.2/src/stairlight/map.py` & `stairlight-0.8.0/src/stairlight/map.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,69 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
 from logging import getLogger
 from typing import Any, Iterator, OrderedDict, Type
 
-from src.stairlight.query import Query
+from src.stairlight.query import Query, UpstairTableReference
 from src.stairlight.source.config import (
     MappingConfig,
     MappingConfigGlobal,
     MappingConfigMappingTable,
     StairlightConfig,
 )
 from src.stairlight.source.config_key import MapKey, MappingConfigKey
 from src.stairlight.source.controller import get_template_source_class
 from src.stairlight.source.template import Template, TemplateSource, TemplateSourceType
 
 logger = getLogger(__name__)
 
 
+@dataclass
+class Stair:
+    name: str
+    mapped_templates: list[MappedTemplate] | None
+
+
+@dataclass
+class MappedTemplate:
+    TemplateSourceType: str
+    Key: str
+    Uri: str
+    Lines: list[dict]
+    Labels: dict[str, str] | None = None
+
+
+@dataclass
+class MappedTemplateObjectStorage(MappedTemplate):
+    BucketName: str | None = None
+
+
+@dataclass
+class MappedTemplateRedash(MappedTemplate):
+    DataSourceType: str | None = None
+
+
 class Map:
     """Manages functions related to dependency map objects"""
 
     def __init__(
         self,
         stairlight_config: StairlightConfig,
         mapping_config: MappingConfig,
-        mapped: dict[str, Any] | None = None,
+        mapped: dict[str, dict[str, list[MappedTemplate]] | None] | None = None,
     ) -> None:
         """Manages functions related to dependency map objects
 
         Args:
             stairlight_config (StairlightConfig): Stairlight configurations.
             mapping_config (MappingConfig):
                 Mapping configurations.
             mapped (dict[str, Any], optional):
-                Mapped table attributes. Defaults to None.
+                Mapped templates. Defaults to None.
         """
         if mapped:
             self.mapped = mapped
         else:
             self.mapped = {}
         self.unmapped: list[dict] = []
         self._stairlight_config = stairlight_config
@@ -45,15 +71,15 @@
 
     def write(self) -> None:
         """Write a dependency map"""
         template_source: TemplateSource
         for template_source in self.find_template_source():
             self.write_by_template_source(template_source=template_source)
 
-        self.mapped = {k: v for k, v in self.mapped.items() if v != {}}
+        self.mapped = {k: v for k, v in self.mapped.items() if v}
 
     def find_template_source(self) -> Iterator[TemplateSource]:
         """find template source
 
         Yields:
             Iterator[TemplateSource]: Template source instance
         """
@@ -73,14 +99,15 @@
     def write_by_template_source(self, template_source: TemplateSource) -> None:
         """Write a dependency map by template source
 
         Args:
             template_source (TemplateSource): Template source
         """
         for template in template_source.search_templates():
+            # Check if the template is in the mapping_config
             if not self._mapping_config:
                 self.add_unmapped_params(template=template)
             elif template.is_mapped():
                 for table_attributes in template.find_mapped_table_attributes():
                     unmapped_params = self.detect_unmapped_params(
                         template=template, table_attributes=table_attributes
                     )
@@ -98,48 +125,82 @@
         """Remap a dependency map
 
         Args:
             template (Template): Query template
             table_attributes (MappingConfigMappingTable):
                 Table attributes from mapping configuration
         """
-        query_str: str = template.render(
-            params=self.merge_global_params(table_attributes=table_attributes),
-            ignore_params=table_attributes.IgnoreParameters,
+        current_floor_name: str = table_attributes.TableName
+        current_floor_label: dict[str, Any] = table_attributes.Labels
+        if self._mapping_config:
+            extra_labels: list[dict[str, Any]] = self._mapping_config.ExtraLabels or []
+
+        current_floor_map: dict[str, Any] = self.mapped.get(current_floor_name) or {}
+        if not current_floor_map:
+            self.mapped[current_floor_name] = {}
+
+        global_params: dict[str, Any] = self.get_global_params()
+        params = self.merge_global_params(
+            table_attributes=table_attributes, global_params=global_params
         )
         query = Query(
-            query_str=query_str,
+            query_str=template.render(
+                params=params,
+                ignore_params=table_attributes.IgnoreParameters,
+            ),
             default_table_prefix=template.default_table_prefix,
         )
 
-        downstairs: str = table_attributes.TableName
-        mapped_labels: dict[str, Any] = table_attributes.Labels
-        if self._mapping_config:
-            extra_labels: list[dict[str, Any]] = self._mapping_config.ExtraLabels
-
-        if downstairs not in self.mapped:
-            self.mapped[downstairs] = {}
+        upstair_table_reference: UpstairTableReference
+        for upstair_table_reference in query.detect_upstair_table_reference():
+            upstair = Stair(
+                name=upstair_table_reference.TableName,
+                mapped_templates=current_floor_map.get(
+                    upstair_table_reference.TableName, []
+                ),
+            )
 
-        for upstairs_attributes in query.detect_upstairs_attributes():
-            upstairs: str = upstairs_attributes[MapKey.TABLE_NAME]
+            upstairs_extra_labels = [
+                extra_label.get(MappingConfigKey.LABELS, {})
+                for extra_label in extra_labels
+                if extra_label.get(MappingConfigKey.TABLE_NAME)
+                == upstair_table_reference.TableName
+            ]
+            upstairs_extra_label = (
+                upstairs_extra_labels[0] if upstairs_extra_labels else []
+            )
+            upstair_template = self.create_upstair_template(
+                template=template,
+                current_floor_label=current_floor_label,
+                extra_label=upstairs_extra_label,
+            )
 
-            if not self.mapped[downstairs].get(upstairs):
-                self.mapped[downstairs][upstairs] = self.create_upstairs_value(
-                    template=template,
-                    mapped_labels=mapped_labels,
-                    extra_labels=extra_labels,
-                    upstairs=upstairs,
+            if upstair and upstair.name == upstair_table_reference.TableName:
+                upstair = Stair(
+                    name=upstair.name,
+                    mapped_templates=upstair.mapped_templates + [upstair_template],
+                )
+            else:
+                upstair = Stair(
+                    name=upstair_table_reference.TableName,
+                    mapped_templates=[upstair_template],
                 )
 
-            self.mapped[downstairs][upstairs][MapKey.LINES].append(
-                {
-                    MapKey.LINE_NUMBER: upstairs_attributes[MapKey.LINE_NUMBER],
-                    MapKey.LINE_STRING: upstairs_attributes[MapKey.LINE_STRING],
-                }
-            )
+            for i, mapped_template in enumerate(upstair.mapped_templates):
+                if (
+                    upstair_table_reference.Line not in mapped_template.Lines
+                    and upstair.name in upstair_table_reference.Line["LineString"]
+                ):
+                    upstair.mapped_templates[i].Lines.append(
+                        upstair_table_reference.Line
+                    )
+
+            self.mapped[current_floor_name][
+                str(upstair.name)
+            ] = upstair.mapped_templates
 
     def get_global_params(self) -> dict[str, Any]:
         """get global parameters in mapping.yaml
 
         Returns:
             dict[str, Any]: Global parameters
         """
@@ -147,84 +208,88 @@
         if self._mapping_config:
             _global: MappingConfigGlobal = self._mapping_config.get_global()
             if _global.Parameters:
                 global_params = _global.Parameters
         return global_params
 
     def merge_global_params(
-        self, table_attributes: MappingConfigMappingTable
+        self,
+        table_attributes: MappingConfigMappingTable,
+        global_params: dict[str, Any],
     ) -> dict[str, Any]:
         """return a combination of global parameters and table parameters
 
         Args:
             table_attributes (MappingConfigMappingTable): table attributes
+            global_params (dict[str, Any]): global params
 
         Returns:
             dict[str, Any]: Combined global parameters
         """
-        global_params: dict[str, Any] = self.get_global_params()
         table_params: OrderedDict[str, Any] = (
             table_attributes.Parameters or OrderedDict()
         )
 
         # Table parameters are prioritized over global parameters
         return {**global_params, **table_params}
 
     @staticmethod
-    def create_upstairs_value(
+    def create_upstair_template(
         template: Template,
-        mapped_labels: dict[str, Any],
-        extra_labels: list[dict[str, Any]],
-        upstairs: str,
-    ) -> dict[str, Any]:
-        """create upstairs table information
+        current_floor_label: dict[str, Any],
+        extra_label: dict[str, Any],
+    ) -> MappedTemplate:
+        """create a upstair template
 
         Args:
             template (Template): Template class
             mapped_labels (dict[str, Any]): Labels in mapping section
             extra_labels (list[dict[str, Any]]): Extra labels
             upstairs (str): Upstairs table's Name
 
         Returns:
-            dict[str, Any]: upstairs table information
+            Table: upstair template
         """
-        target_labels: list[dict[str, Any]] = []
-        upstairs_values = {
-            MapKey.TEMPLATE_SOURCE_TYPE: template.source_type.value,
-            MapKey.KEY: template.key,
-            MapKey.URI: template.uri,
-            MapKey.LINES: [],
+        upstair_labels: dict = {
+            **(current_floor_label or {}),
+            **(extra_label or {}),
         }
 
-        if template.source_type in (TemplateSourceType.GCS, TemplateSourceType.S3):
-            upstairs_values[MapKey.BUCKET_NAME] = template.bucket
+        upstair_template: MappedTemplate
+        if template.source_type in (
+            TemplateSourceType.GCS,
+            TemplateSourceType.S3,
+        ):
+            upstair_template = MappedTemplateObjectStorage(
+                TemplateSourceType=template.source_type.value,
+                Key=template.key,
+                Uri=template.uri,
+                Lines=[],
+                Labels=upstair_labels,
+                BucketName=template.bucket,
+            )
         elif template.source_type == TemplateSourceType.REDASH:
-            upstairs_values[MapKey.DATA_SOURCE_NAME] = template.data_source_name
-
-        if extra_labels:
-            target_labels = [
-                extra_label.get(MappingConfigKey.LABELS, {})
-                for extra_label in extra_labels
-                if extra_label.get(MappingConfigKey.TABLE_NAME) == upstairs
-            ]
-        if mapped_labels or extra_labels:
-            upstairs_values[MapKey.LABELS] = {}
-
-        if mapped_labels:
-            upstairs_values[MapKey.LABELS] = {
-                **upstairs_values[MapKey.LABELS],
-                **mapped_labels,
-            }
+            upstair_template = MappedTemplateRedash(
+                TemplateSourceType=template.source_type.value,
+                Key=template.key,
+                Uri=template.uri,
+                Lines=[],
+                Labels=upstair_labels,
+                DataSourceType=template.data_source_name,
+            )
+        else:
+            upstair_template = MappedTemplate(
+                TemplateSourceType=template.source_type.value,
+                Key=template.key,
+                Uri=template.uri,
+                Lines=[],
+                Labels=upstair_labels,
+            )
 
-        if target_labels:
-            upstairs_values[MapKey.LABELS] = {
-                **upstairs_values[MapKey.LABELS],
-                **target_labels[0],
-            }
-        return upstairs_values
+        return upstair_template
 
     def add_unmapped_params(
         self, template: Template, params: list[str] | None = None
     ) -> None:
         """add to the list of unmapped params
 
         Args:
@@ -255,16 +320,17 @@
             list[str]: Unmapped parameters
         """
         template_str: str = template.get_template_str()
         template_params: list[str] = template.detect_jinja_params(template_str)
         if not template_params:
             return []
 
+        global_params: dict[str, Any] = self.get_global_params()
         mapped_params_dict: dict[str, Any] = self.merge_global_params(
-            table_attributes=table_attributes
+            table_attributes=table_attributes, global_params=global_params
         )
         mapped_params: list[str] = create_dict_key_list(d=mapped_params_dict)
         ignore_params: list[str] = table_attributes.IgnoreParameters or []
         unmapped_params: list[str] = list(
             set(template_params) - set(mapped_params) - set(ignore_params)
         )
 
@@ -276,17 +342,17 @@
 
     Args:
         d (dict[str, Any]): dict
 
     Returns:
         list[str]: key-combined and list-converted results
     """
-    results = []
+    results: list[str] = []
     for key, value in d.items():
         if isinstance(value, dict):
-            recursive_results = create_dict_key_list(d=value)
-            for recursive_result in recursive_results:
-                concat = key + delimiter + recursive_result
-                results.append(concat)
+            results = results + [
+                key + delimiter + recursive_result
+                for recursive_result in create_dict_key_list(d=value)
+            ]
         else:
             results.append(key)
     return results
```

### Comparing `stairlight-0.7.2/src/stairlight/query.py` & `stairlight-0.8.0/src/stairlight/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 from __future__ import annotations
 
 import re
+from dataclasses import asdict, dataclass
 from typing import Iterator
 
-from src.stairlight.source.config import MapKey
+
+@dataclass
+class UpstairTableReference:
+    TableName: str
+    Line: dict
+
+
+@dataclass
+class UpstairTableReferenceLine:
+    LineNumber: int
+    LineString: str
 
 
 class Query:
     """SQL query"""
 
     def __init__(self, query_str: str, default_table_prefix: str = None) -> None:
         """SQL query
@@ -17,43 +28,48 @@
             default_table_prefix (str, optional):
                 If project or dataset that configured table have are omitted,
                 it will be complement this prefix. Defaults to None.
         """
         self.query_str = query_str
         self.default_table_prefix = default_table_prefix
 
-    def detect_upstairs_attributes(self) -> Iterator[dict]:
-        """Parse a query statement and detect upstream table attributes
+    def detect_upstair_table_reference(self) -> Iterator[UpstairTableReference]:
+        """Parse a query statement and detect a upstream table reference
 
         Yields:
-            Iterator[dict]: upstream table attributes
+            Iterator[UpstairsResults]: upstream table results
         """
         upstairs_tables = self.parse_and_get_upstairs_tables()
 
         for upstairs_table in upstairs_tables:
             line_indexes = [
                 i
                 for i, line in enumerate(self.query_str.splitlines())
                 if upstairs_table in line
                 and "--" not in line.split(upstairs_table)[0]  # exclude comments
             ]
 
             for line_index in line_indexes:
-                if self.default_table_prefix:
-                    table_name = solve_table_prefix(
+                table_name = (
+                    solve_table_prefix(
                         table=upstairs_table,
                         default_table_prefix=self.default_table_prefix,
                     )
-                else:
-                    table_name = upstairs_table
-                yield {
-                    MapKey.TABLE_NAME: table_name.replace("`", ""),  # for BigQuery
-                    MapKey.LINE_NUMBER: line_index + 1,
-                    MapKey.LINE_STRING: self.query_str.splitlines()[line_index],
-                }
+                    if self.default_table_prefix
+                    else upstairs_table
+                )
+                yield UpstairTableReference(
+                    TableName=table_name.replace("`", ""),
+                    Line=asdict(
+                        UpstairTableReferenceLine(
+                            LineNumber=line_index + 1,
+                            LineString=self.query_str.splitlines()[line_index],
+                        )
+                    ),
+                )
 
     def parse_and_get_upstairs_tables(self) -> list[str]:
         """Parse query and get upstairs tables
 
         Returns:
             list[str]: A list of upstairs tables
         """
```

### Comparing `stairlight-0.7.2/src/stairlight/source/config.py` & `stairlight-0.8.0/src/stairlight/source/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/config_key.py` & `stairlight-0.8.0/src/stairlight/source/config_key.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/controller.py` & `stairlight-0.8.0/src/stairlight/source/controller.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/dbt/config.py` & `stairlight-0.8.0/src/stairlight/source/dbt/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/dbt/template.py` & `stairlight-0.8.0/src/stairlight/source/dbt/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/file/config.py` & `stairlight-0.8.0/src/stairlight/source/file/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/file/template.py` & `stairlight-0.8.0/src/stairlight/source/file/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/gcs/config.py` & `stairlight-0.8.0/src/stairlight/source/gcs/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/gcs/template.py` & `stairlight-0.8.0/src/stairlight/source/gcs/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/redash/config.py` & `stairlight-0.8.0/src/stairlight/source/redash/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/redash/template.py` & `stairlight-0.8.0/src/stairlight/source/redash/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/s3/config.py` & `stairlight-0.8.0/src/stairlight/source/s3/config.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/s3/map.py` & `stairlight-0.8.0/src/stairlight/source/s3/map.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/s3/template.py` & `stairlight-0.8.0/src/stairlight/source/s3/template.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/src/stairlight/source/template.py` & `stairlight-0.8.0/src/stairlight/source/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,29 +84,29 @@
         """Get mapped tables as iterator
 
         Yields:
             Iterator[dict]: Mapped table attributes
         """
         mapping: Any
         for mapping in self._mapping_config.get_mapping():
-            not_found: bool = True
+            found: bool = False
             if mapping.TemplateSourceType in (
                 TemplateSourceType.FILE.value,
                 TemplateSourceType.DBT.value,
             ):
                 if self.key.endswith(mapping.FileSuffix):
-                    not_found = False
+                    found = True
             elif mapping.TemplateSourceType in (
                 TemplateSourceType.GCS.value,
                 TemplateSourceType.S3.value,
             ):
                 if self.uri == mapping.Uri:
-                    not_found = False
+                    found = True
 
-            if not_found:
+            if not found:
                 continue
 
             for table_attributes in mapping.get_table():
                 yield table_attributes
             break
 
     def is_mapped(self) -> bool:
```

### Comparing `stairlight-0.7.2/src/stairlight/stairlight.py` & `stairlight-0.8.0/src/stairlight/stairlight.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from __future__ import annotations
 
 import enum
-import json
+import os
+from dataclasses import asdict
 from logging import getLogger
 from typing import Any
 
 import src.stairlight.util as sl_util
-from src.stairlight.configurator import (
-    MAPPING_CONFIG_PREFIX_DEFAULT,
-    STAIRLIGHT_CONFIG_PREFIX_DEFAULT,
-    Configurator,
-)
-from src.stairlight.map import Map
+from src.stairlight.configurator import Configurator
+from src.stairlight.map import Map, MappedTemplate
 from src.stairlight.source.config import (
     MapKey,
     MappingConfig,
     StairlightConfig,
     StairlightConfigSettings,
 )
+from src.stairlight.source.config_key import MappingConfigKey
 from src.stairlight.source.controller import LoadMapController, SaveMapController
+from src.stairlight.source.template import TemplateSourceType
+
+STAIRLIGHT_CONFIG_PREFIX_DEFAULT = "stairlight"
+MAPPING_CONFIG_PREFIX_DEFAULT = "mapping"
+CONFIG_UNMAPPED_PREFIX_DEFAULT = "unmapped"
+CONFIG_NOT_FOUND_PREFIX_DEFAULT = "not_found"
 
 logger = getLogger(__name__)
 
 
 class ResponseType(enum.Enum):
     """Enum: Execution result type of up|down command"""
 
@@ -47,37 +51,42 @@
     """A table dependency detector"""
 
     def __init__(
         self,
         config_dir: str = ".",
         load_files: list[str] = None,
         save_file: str = "",
+        stairlight_config_prefix: str = STAIRLIGHT_CONFIG_PREFIX_DEFAULT,
+        mapping_config_prefix: str = MAPPING_CONFIG_PREFIX_DEFAULT,
     ) -> None:
         """A table dependency detector
 
         Args:
             config_dir (str, optional):
                 Stairlight configuration directory. Defaults to ".".
             load_files (list, optional):
                 file names of loading results if load option set. Defaults to None.
             save_file (str, optional):
                 A file name of saving results if save option set. Defaults to None.
         """
         self.load_files = load_files
         self.save_file: str = save_file
         self._configurator = Configurator(dir=config_dir)
-        self._mapped: dict[str, Any] = {}
+        self._mapped: dict[str, dict[str, list[MappedTemplate] | None] | None] = {}
         self._unmapped: list[dict[str, Any]] = []
+        self._not_found: list[str] = []
         self._mapping_config: MappingConfig | None = None
+        self._stairlight_config_prefix: str = stairlight_config_prefix
+        self._mapping_config_prefix: str = mapping_config_prefix
         self._stairlight_config: StairlightConfig = self._configurator.read_stairlight(
-            prefix=STAIRLIGHT_CONFIG_PREFIX_DEFAULT
+            prefix=stairlight_config_prefix
         )
 
     @property
-    def mapped(self) -> dict[str, Any]:
+    def mapped(self) -> dict[str, dict[str, list[MappedTemplate] | None] | None]:
         """Return mapped
 
         Returns:
             dict: Mapped results
         """
         return self._mapped
 
@@ -86,14 +95,23 @@
         """Return unmapped
 
         Returns:
             list[dict]: Unmapped results
         """
         return self._unmapped
 
+    @property
+    def not_found(self) -> list[str]:
+        """Return not_found
+
+        Returns:
+            list[dict]: Results of not found
+        """
+        return self._not_found
+
     def has_stairlight_config(self) -> bool:
         """Exists a stairlight configuration file or not
 
         Returns:
             bool: Exists stairlight configuration file or not
         """
         return len(self._stairlight_config.Include) > 0
@@ -110,15 +128,16 @@
 
         if self.save_file:
             self.save_map()
 
     def save_map(self) -> None:
         """Save mapped results"""
         save_map_controller = SaveMapController(
-            save_file=self.save_file, mapped=self._mapped
+            save_file=self.save_file,
+            mapped=self.cast_mapped_dict_all(mapped=self._mapped),
         )
         save_map_controller.save()
 
     def load_map(self) -> None:
         """Load mapped results"""
         if not self.load_files:
             return
@@ -169,46 +188,80 @@
         )
 
         dependency_map.write()
         if self._mapping_config:
             self._mapped = dependency_map.mapped
 
         self._unmapped = dependency_map.unmapped
+        self._not_found = self.get_templates_not_found()
+
+    def get_templates_not_found(self) -> list[str]:
+        not_found: set[str] = set()
+        mapped_urls: list[str] = self.list_uris()
+        for config in self._mapping_config.Mapping:
+            uri: str = ""
+            if config.get(MappingConfigKey.TEMPLATE_SOURCE_TYPE) in [
+                TemplateSourceType.FILE.value,
+                TemplateSourceType.DBT.value,
+            ]:
+                file_suffix = config.get(MappingConfigKey.File.FILE_SUFFIX)
+                uri = os.path.abspath(f"./{file_suffix}")
+            elif config.get(MappingConfigKey.TEMPLATE_SOURCE_TYPE) in [
+                TemplateSourceType.GCS.value,
+                TemplateSourceType.S3.value,
+            ]:
+                uri = config.get(MappingConfigKey.Gcs.URI)
+
+            if uri not in mapped_urls:
+                not_found.add(uri)
+
+        return sorted(not_found)
 
     def init(self, prefix: str = STAIRLIGHT_CONFIG_PREFIX_DEFAULT) -> str:
         """Create Stairlight template file
 
         Args:
             prefix (str, optional):
                 Template file prefix. Defaults to STAIRLIGHT_CONFIG_PREFIX.
 
         Returns:
             str: Template file name
         """
         return self._configurator.create_stairlight_file(prefix=prefix)
 
-    def check(self, prefix: str = MAPPING_CONFIG_PREFIX_DEFAULT) -> str:
+    def check(
+        self,
+        prefix_unmapped: str = CONFIG_UNMAPPED_PREFIX_DEFAULT,
+        prefix_not_found: str = CONFIG_NOT_FOUND_PREFIX_DEFAULT,
+    ) -> list[str]:
         """Check mapped results and create a mapping template file
 
         Args:
             prefix (str, optional):
                 Template file prefix. Defaults to MAPPING_CONFIG_PREFIX.
 
         Returns:
-            str: Template file name
+            list[str]: Created file names
         """
-        if self.load_files:
-            logger.warning("Load option is used, skip checking.")
-            return ""
-        elif not self._unmapped:
-            return ""
+        unmapped_file = ""
+        not_found_file = ""
+        if self.load_files or (not self._unmapped and not self._unmapped):
+            return []
 
-        return self._configurator.create_mapping_file(
-            unmapped=self._unmapped, prefix=prefix
+        unmapped_config = self._configurator.build_mapping_config(
+            detected_templates=self._unmapped
+        )
+        unmapped_file = self._configurator.create_mapping_file(
+            config=unmapped_config, prefix=prefix_unmapped
         )
+        if self._not_found:
+            not_found_file = self._configurator.create_mapping_file(
+                config=self._not_found, prefix=prefix_not_found
+            )
+        return [unmapped_file, not_found_file]
 
     def list_(self, response_type: str) -> list[str]:
         """show tables or URIs
 
         Args:
             response_type (str): Response type value
 
@@ -225,33 +278,70 @@
     def list_tables(self) -> list[str]:
         """list tables
 
         Returns:
             list[str]: a list of tables
         """
         results: set[str] = set()
-        for downstairs, upstairs_dict in self._mapped.items():
-            results.add(downstairs)
-            for upstairs in upstairs_dict:
-                results.add(upstairs)
+        for table_name, upstairs in self._mapped.items():
+            results.add(table_name)
+            results.update(
+                set([upstair_name for upstair_name in upstairs.keys()]),
+            )
         return sorted(results)
 
     def list_uris(self) -> list[str]:
         """list URIs
 
         Returns:
             list[str]: a list of URIs
         """
         results: set[str] = set()
-        for upstairs_dict in self._mapped.values():
-            for upstairs_attributes in upstairs_dict.values():
-                if upstairs_attributes.get(MapKey.URI):
-                    results.add(upstairs_attributes.get(MapKey.URI))
+        for upstairs in self._mapped.values():
+            for upstair, mapped_templates in upstairs.items():
+                upstair_uri: str = self.get_uri_from_mapping_config(
+                    target_table=upstair
+                )
+                if upstair_uri:
+                    results.add(upstair_uri)
+                results.update(
+                    set(
+                        [
+                            mapped_template.Uri
+                            for mapped_template in mapped_templates
+                            if mapped_templates
+                        ]
+                    )
+                )
         return sorted(results)
 
+    def get_uri_from_mapping_config(self, target_table: str) -> str:
+        for config in self._mapping_config.Mapping:
+            uri: str = ""
+            if config.get(MappingConfigKey.TEMPLATE_SOURCE_TYPE) in [
+                TemplateSourceType.FILE.value,
+                TemplateSourceType.DBT.value,
+            ]:
+                file_suffix = config.get(MappingConfigKey.File.FILE_SUFFIX)
+                uri = os.path.abspath(f"./{file_suffix}")
+            elif config.get(MappingConfigKey.TEMPLATE_SOURCE_TYPE) in [
+                TemplateSourceType.GCS.value,
+                TemplateSourceType.S3.value,
+            ]:
+                uri = config.get(MappingConfigKey.Gcs.URI)
+            table_names = [
+                tables.get(MappingConfigKey.TABLE_NAME)
+                for tables in config.get(MappingConfigKey.TABLES)
+            ]
+
+            if target_table in table_names:
+                return uri
+
+        return ""
+
     def up(
         self,
         table_name: str,
         recursive: bool = False,
         verbose: bool = False,
         response_type: str = ResponseType.TABLE.value,
     ) -> list[str] | dict[str, Any]:
@@ -346,67 +436,76 @@
     def search_verbose(
         self,
         table_name: str,
         recursive: bool,
         direction: SearchDirection,
         searched_tables: list[str],
         head: bool,
-    ) -> dict:
+    ) -> dict[str, Any]:
         """Search nodes and return verbose results
 
         Args:
             table_name (str): Table name
             recursive (bool): Search recursively or not
             direction (SearchDirection): Search direction
             searched_tables (list[str]): a list of searched tables
             head (bool): Current position is head or not
 
         Returns:
             dict: Search results
         """
+        search_results: dict[str, dict[str, Any]] = {}
+        response: dict[str, Any] = {table_name: {}}
+
         relative_map = self.create_relative_map(
-            table_name=table_name, direction=direction
+            target_table_name=table_name, direction=direction
         )
-        response: dict[str, Any] = {table_name: {}}
-        if not relative_map:
-            return response
 
-        if recursive:
-            for next_table_name in relative_map.keys():
+        for next_table_name, templates in relative_map.items():
+            if recursive:
                 if head:
                     searched_tables = [table_name]
 
                 searched_tables.append(next_table_name)
 
                 if sl_util.is_cyclic(tables=searched_tables):
                     details = {
                         "table_name": table_name,
                         "next_table_name": next_table_name,
                         "searched_tables": searched_tables,
                     }
-                    logger.warning(f"Circular reference detected!: {details}")
+                    logger.warning(f"Circular references detected!: {details}")
                     continue
 
-                next_response = self.search_verbose(
-                    table_name=next_table_name,
-                    direction=direction,
-                    recursive=recursive,
-                    searched_tables=searched_tables,
-                    head=False,
-                )
+            search_results[next_table_name] = {}
+            search_results[next_table_name]["Templates"] = []
+            for template in templates:
+                if recursive:
+                    next_response = self.search_verbose(
+                        table_name=next_table_name,
+                        direction=direction,
+                        recursive=recursive,
+                        searched_tables=searched_tables,
+                        head=False,
+                    )
 
-                if not next_response.get(next_table_name):
-                    continue
+                    if not next_response.get(next_table_name):
+                        continue
 
-                relative_map[next_table_name] = {
-                    **relative_map[next_table_name],
-                    **next_response[next_table_name],
-                }
+                    search_results[next_table_name]["Templates"] = relative_map[
+                        next_table_name
+                    ]
+                    if next_response[next_table_name][direction.value]:
+                        search_results[next_table_name][
+                            direction.value
+                        ] = next_response[next_table_name][direction.value]
+                else:
+                    search_results[table_name]["Templates"].append(template)
 
-        response[table_name][direction.value] = relative_map
+        response[table_name][direction.value] = search_results
         return response
 
     def search_plain(
         self,
         table_name: str,
         recursive: bool,
         response_type: str,
@@ -424,74 +523,86 @@
             searched_tables (list[str]): a list of searched tables
             head (bool): Current position is head or not
 
         Returns:
             list[str]: Search results
         """
         relative_map = self.create_relative_map(
-            table_name=table_name, direction=direction
+            target_table_name=table_name, direction=direction
         )
         response: list[str] = []
         if not relative_map:
             return response
 
         next_table_name: str
-        for next_table_name in relative_map.keys():
+        for next_table_name, templates in relative_map.items():
             if recursive:
                 if head:
                     searched_tables = []
                     searched_tables.append(table_name)
 
                 searched_tables.append(next_table_name)
 
                 if sl_util.is_cyclic(tables=searched_tables):
                     details = {
                         "table_name": table_name,
                         "next_table_name": next_table_name,
                         "searched_tables": searched_tables,
                     }
-                    logger.info(f"Circular reference detected!: {details}")
+                    logger.info(f"Circular references detected!: {details}")
                     continue
 
-                next_response = self.search_plain(
-                    table_name=next_table_name,
-                    direction=direction,
-                    recursive=recursive,
-                    response_type=response_type,
-                    searched_tables=searched_tables,
-                    head=False,
-                )
-                response = response + next_response
+            for template in templates:
+                if recursive:
+                    next_response = self.search_plain(
+                        table_name=next_table_name,
+                        direction=direction,
+                        recursive=recursive,
+                        response_type=response_type,
+                        searched_tables=searched_tables,
+                        head=False,
+                    )
+                    response = response + next_response
 
-            if response_type == ResponseType.TABLE.value:
-                response.append(next_table_name)
-            elif response_type == ResponseType.URI.value:
-                response.append(relative_map[next_table_name].get(MapKey.URI))
-            logger.debug(json.dumps(response, indent=2))
+                if response_type == ResponseType.TABLE.value:
+                    response.append(next_table_name)
+                elif response_type == ResponseType.URI.value:
+                    uri = template.get(MapKey.URI)
+                    if uri:
+                        response.append(uri)
 
         return sorted(list(set(response)))
 
     def create_relative_map(
-        self, table_name: str, direction: SearchDirection
-    ) -> dict[str, Any]:
+        self, target_table_name: str, direction: SearchDirection
+    ) -> dict[str, list[dict[str, Any]]]:
         """Create a relative map for the specified direction
 
         Args:
-            table_name (str): Table name
+            target_table_name (str): Target table name
             direction (SearchDirection): Search direction
 
         Returns:
             dict: Relative map
         """
-        relative_map: dict[str, Any] = {}
+        relative_map: dict[str, list[dict[str, Any]]] = {}
         if direction == SearchDirection.UP:
-            relative_map = self._mapped.get(table_name, {})
+            upstairs = self._mapped.get(target_table_name, {})
+            for upstair_name, mapped_templates in upstairs.items():
+                relative_map[upstair_name] = [
+                    asdict(mapped_template) for mapped_template in mapped_templates
+                ]
         elif direction == SearchDirection.DOWN:
-            for key in [k for k, v in self._mapped.items() if v.get(table_name)]:
-                relative_map[key] = self._mapped[key][table_name]
+            for table_name, upstairs in self._mapped.items():
+                for upstair_name, mapped_templates in upstairs.items():
+                    if mapped_templates and upstair_name == target_table_name:
+                        relative_map[table_name] = [
+                            asdict(mapped_template)
+                            for mapped_template in mapped_templates
+                        ]
         return relative_map
 
     def find_tables_by_labels(self, target_labels: list[str]) -> list[str]:
         """Find tables by labels
 
         Args:
             target_labels (list[str]): Target labels
@@ -554,7 +665,23 @@
                 if (
                     target_label_key == configured_label_key
                     and target_label_value == configured_label_value
                 ):
                     found_count += 1
 
         return found_count == len(target_labels)
+
+    @staticmethod
+    def cast_mapped_dict_all(
+        mapped: dict[str, dict[str, list[MappedTemplate] | None]]
+    ) -> dict[str, dict[str, list[dict] | None]]:
+        casted: dict[str, Any] = {}
+        for table_name, upstairs in mapped.items():
+            if not casted.get(table_name):
+                casted[table_name] = {}
+            for upstair_name, mapped_templates in upstairs.items():
+                if not casted[table_name].get(upstair_name):
+                    casted[table_name][upstair_name] = []
+                for mapped_template in mapped_templates:
+                    if mapped_template and isinstance(mapped_template, MappedTemplate):
+                        casted[table_name][upstair_name].append(asdict(mapped_template))
+        return casted
```

### Comparing `stairlight-0.7.2/src/stairlight/util.py` & `stairlight-0.8.0/src/stairlight/util.py`

 * *Files identical despite different names*

### Comparing `stairlight-0.7.2/setup.py` & `stairlight-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,25 +29,25 @@
  's3': ['boto3>=1.24.14']}
 
 entry_points = \
 {'console_scripts': ['stairlight = src.stairlight.cli:main']}
 
 setup_kwargs = {
     'name': 'stairlight',
-    'version': '0.7.2',
+    'version': '0.8.0',
     'description': 'An end-to-end data lineage tool',
     'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/tosh2230/stairlight/main/img/stairlight_white.png" width="400" alt="Stairlight">\n</div>\n\n-----------------\n\n# Stairlight\n\n[![PyPi Version](https://img.shields.io/pypi/v/stairlight.svg?style=flat-square&logo=PyPi)](https://pypi.org/project/stairlight/)\n[![PyPi License](https://img.shields.io/pypi/l/stairlight.svg?style=flat-square)](https://pypi.org/project/stairlight/)\n[![PyPi Python Versions](https://img.shields.io/pypi/pyversions/stairlight.svg?style=flat-square)](https://pypi.org/project/stairlight/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)\n[![CI](https://github.com/tosh2230/stairlight/actions/workflows/ci.yml/badge.svg)](https://github.com/tosh2230/stairlight/actions/workflows/ci.yml)\n\nAn end-to-end data lineage tool, detects table dependencies from SQL statements.\n\n<div align="left">\n  <img src="https://raw.githubusercontent.com/tosh2230/stairlight/main/img/drawio/concepts.drawio.png" width="1080" alt="concepts">\n</div>\n\n## Supported Data Sources\n\n| Data Source | Remarks |\n| --- | --- |\n| Local file system | Python Pathlib module |\n| [Amazon S3](https://aws.amazon.com/s3/) | Available for [Amazon Managed Workflows for Apache Airflow (MWAA)](https://aws.amazon.com/managed-workflows-for-apache-airflow/) |\n| [Google Cloud Storage](https://cloud.google.com/storage) | Available for [Google Cloud Composer](https://cloud.google.com/composer) |\n| [dbt](https://www.getdbt.com/) - [Google BigQuery](https://cloud.google.com/bigquery) | Using `dbt compile` command internally |\n| [Redash](https://redash.io/) | |\n\n## Installation\n\nThis package is distributed on [PyPI](https://pypi.org/project/stairlight/).\n\n```sh\n# The base package is for local file system only.\n$ pip install stairlight\n\n# Set extras when detecting from other data sources.\n# e.g. Amazon S3 and Google Cloud Storage\n$ pip install "stairlight[s3, gcs]"\n```\n\n| Data Source | TemplateSourceType | Extra |\n| --- | --- | --- |\n| Local file system | File | - |\n| Amazon S3 | S3 | s3 |\n| Google Cloud Storage | GCS | gcs |\n| dbt - Google Bigquery | dbt | dbt-bigquery |\n| Redash | Redash | redash |\n\n## Getting Started\n\nThere are 3 steps to use.\n\n```sh\n# 1: Initialize and set your data source settings\n$ stairlight init\n\n# 2: Map your SQL statements and tables\n$ stairlight map\n\n# 3: Get table dependencies\n$ stairlight\n```\n\n## Description\n\n### Input\n\n- SQL statements\n- Configuration YAML files\n    - stairlight.yaml: SQL statements locations and include/exclude conditions.\n    - mapping.yaml: For mapping SQL statements and tables.\n\n### Output\n\nStairlight outputs table dependencies as JSON format.\n\nTop-level keys are table names, and values represents tables that are the data source for each key\'s table.\n\n<details>\n\n<summary>Example</summary>\n\n```json\n{\n  "test_project.beam_streaming.taxirides_aggregation": {\n    "test_project.beam_streaming.taxirides_realtime": {\n      "TemplateSourceType": "File",\n      "Key": "tests/sql/main/union_same_table.sql",\n      "Uri": "/foo/bar/stairlight/tests/sql/main/union_same_table.sql",\n      "Lines": [\n        {\n          "LineNumber": 6,\n          "LineString": "    test_project.beam_streaming.taxirides_realtime"\n        },\n        {\n          "LineNumber": 15,\n          "LineString": "    test_project.beam_streaming.taxirides_realtime"\n        }\n      ]\n    }\n  },\n  "PROJECT_a.DATASET_b.TABLE_c": {\n    "PROJECT_A.DATASET_A.TABLE_A": {\n      "TemplateSourceType": "GCS",\n      "Key": "sql/one_line/one_line.sql",\n      "Uri": "gs://stairlight/sql/one_line/one_line.sql",\n      "Lines": [\n        {\n          "LineNumber": 1,\n          "LineString": "SELECT * FROM PROJECT_A.DATASET_A.TABLE_A WHERE 1 = 1"\n        }\n      ],\n      "BucketName": "stairlight",\n      "Labels": {\n        "Source": null,\n        "Test": "a"\n      }\n    }\n  },\n  "AggregateSales": {\n    "PROJECT_e.DATASET_e.TABLE_e": {\n      "TemplateSourceType": "Redash",\n      "Key": 5,\n      "Uri": "AggregateSales",\n      "Lines": [\n        {\n          "LineNumber": 1,\n          "LineString": "SELECT service, SUM(total_amount) FROM PROJECT_e.DATASET_e.TABLE_e GROUP BY service"\n        }\n      ],\n      "DataSourceName": "BigQuery",\n      "Labels": {\n        "Category": "Sales"\n      }\n    }\n  },\n  "dummy.dummy.example_b": {\n    "PROJECT_t.DATASET_t.TABLE_t": {\n      "TemplateSourceType": "dbt",\n      "Key": "tests/dbt/project_01/target/compiled/project_01/models/b/example_b.sql",\n      "Uri": "/foo/bar/stairlight/tests/dbt/project_01/target/compiled/project_01/models/b/example_b.sql",\n      "Lines": [\n        {\n          "LineNumber": 1,\n          "LineString": "select * from PROJECT_t.DATASET_t.TABLE_t where value_a = 0 and value_b = 0"\n        }\n      ]\n    }\n  },\n  "PROJECT_as.DATASET_bs.TABLE_cs": {\n    "PROJECT_A.DATASET_A.TABLE_A": {\n      "TemplateSourceType": "S3",\n      "Key": "sql/one_line/one_line.sql",\n      "Uri": "s3://stairlight/sql/one_line/one_line.sql",\n      "Lines": [\n        {\n          "LineNumber": 1,\n          "LineString": "SELECT * FROM PROJECT_A.DATASET_A.TABLE_A WHERE 1 = 1"\n        }\n      ],\n      "BucketName": "stairlight",\n      "Labels": {\n        "Source": null,\n        "Test": "a"\n      }\n    }\n  }\n}\n```\n\n</details>\n\n### Collecting patterns\n\n#### Centralization\n\n<div align="left">\n  <img src="https://raw.githubusercontent.com/tosh2230/stairlight/main/img/drawio/centralization.drawio.png" width="800" alt="centralization">\n</div>\n\n#### Agents\n\n<div align="left">\n  <img src="https://raw.githubusercontent.com/tosh2230/stairlight/main/img/drawio/agents.drawio.png" width="800" alt="agents">\n</div>\n\n## Configuration\n\nExamples can be found [here](https://github.com/tosh2230/stairlight/tree/main/tests/config), used for unit testing in CI.\n\n### stairlight.yaml\n\n\'stairlight.yaml\' is for setting up Stairlight itself. It is responsible for specifying SQL statements to be read.\n\n`stairlight init` creates a template of stairlight.yaml.\n\n<details>\n\n<summary>Example</summary>\n\n```yaml\nInclude:\n  - TemplateSourceType: File\n    FileSystemPath: ./tests/sql\n    Regex: .*/*\\.sql$\n    DefaultTablePrefix: "PROJECT_A"\n  - TemplateSourceType: GCS\n    ProjectId: null\n    BucketName: stairlight\n    Regex: ^sql/.*/*\\.sql$\n    DefaultTablePrefix: "PROJECT_A"\n  - TemplateSourceType: Redash\n    DatabaseUrlEnvironmentVariable: REDASH_DATABASE_URL\n    DataSourceName: BigQuery\n    QueryIds:\n      - 1\n      - 3\n      - 5\n  - TemplateSourceType: dbt\n    ProjectDir: tests/dbt/project_01\n    ProfilesDir: tests/dbt\n    Vars:\n      key_a: value_a\n      key_b: value_b\n  - TemplateSourceType: S3\n    BucketName: stairlight\n    Regex: ^sql/.*/*\\.sql$\n    DefaultTablePrefix: "PROJECT_A"\nExclude:\n  - TemplateSourceType: File\n    Regex: main/exclude\\.sql$\nSettings:\n  MappingFilesRegex:\n    - .*/mapping\\_file\\.yaml$\n    - .*/mapping\\_gcs\\.yaml$\n    - .*/mapping\\_dbt\\.yaml$\n    - .*/mapping\\_s3\\.yaml$\n  # Deprecated from v0.7.2\n  MappingPrefix: "mapping"\n```\n\n</details>\n\n### mapping.yaml\n\n\'mapping.yaml\' is used to define relationships between input SELECT statements and tables.\n\n`stairlight map` creates a template of mapping.yaml and attempts to read from data sources specified in stairlight.yaml.\nIf successfully read, it outputs settings that have not yet configured in an existing \'mapping.yaml\' file.\n\n<details>\n\n<summary>Example</summary>\n\n```yaml\nGlobal:\n  Parameters:\n    DESTINATION_PROJECT: stairlight\n    params:\n      PROJECT: 1234567890\n      DATASET: public\n      TABLE: taxirides\nMapping:\n  - TemplateSourceType: File\n    FileSuffix: "tests/sql/main/union_same_table.sql"\n    Tables:\n      - TableName: "test_project.beam_streaming.taxirides_aggregation"\n        Parameters:\n          params:\n            source_table: source\n            destination_table: destination\n        IgnoreParameters:\n          - execution_date.add(days=1).isoformat()\n  - TemplateSourceType: GCS\n    Uri: "gs://stairlight/sql/one_line/one_line.sql"\n    Tables:\n      - TableName: "PROJECT_a.DATASET_b.TABLE_c"\n  - TemplateSourceType: Redash\n    QueryId: 5\n    DataSourceName: metadata\n    Tables:\n      - TableName: New Query\n        Parameters:\n          table: dashboards\n        Labels:\n          Category: Redash test\n  - TemplateSourceType: dbt\n    ProjectName: project_01\n    FileSuffix: tests/dbt/project_01/target/compiled/project_01/models/example/my_first_dbt_model.sql\n    Tables:\n      - TableName: dummy.dummy.my_first_dbt_model\n  - TemplateSourceType: S3\n    Uri: "s3://stairlight/sql/one_line/one_line.sql"\n    Tables:\n      - TableName: "PROJECT_as.DATASET_bs.TABLE_cs"\nExtraLabels:\n  - TableName: "PROJECT_A.DATASET_A.TABLE_A"\n    Labels:\n      Source: Null\n      Test: a\n```\n\n</details>\n\n#### Global Section\n\nThis section is for global configurations.\n\n`Parameters` is used to set common parameters. If conflicts has occurred with `Parameters` in mapping section, mapping section\'s parameters will be used in preference to global.\n\n#### Mapping Section\n\nMapping section is used to define relationships between input SELECT statements and tables that created as a result of query execution.\n\n`Parameters` allows you to reflect settings in [jinja](https://jinja.palletsprojects.com/) template variables embedded in statements. If multiple settings are applied to a statement using jinja template, the statement will be read as if there were the same number of queries as the number of settings.\n\nIn contrast, `IgnoreParameters` handles a list to ignore when rendering queries.\n\n#### Extra labels Section\n\nThis section sets labels to tables that appears only in queries.\n\n## Arguments and Options\n\n```txt\n$ stairlight --help\nusage: stairlight [-h] [-c CONFIG] [--save SAVE] [--load LOAD] {init,check,up,down} ...\n\nAn end-to-end data lineage tool, detects table dependencies by SQL SELECT statements.\nWithout positional arguments, return a table dependency map as JSON format.\n\npositional arguments:\n  {init,map,check,list,up,down}\n    init                create a new Stairlight configuration file\n    map (check)         create a new configuration file about undefined mappings\n    list                return all ( tables | URIs )\n    up                  return upstairs ( tables | URIs )\n    down                return downstairs ( tables | URIs )\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -c CONFIG, --config CONFIG\n                        set a Stairlight configuration directory\n  -q, --quiet           keep silence\n  --save SAVE           A file path where map results will be saved.\n                        You can choose from local file system, GCS, S3.\n  --load LOAD           A file path where map results are saved.\n                        You can choose from local file system, GCS, S3.\n                        It can be specified multiple times.\n```\n\n### init\n\n`stairlight init` creates a new Stairlight configuration file.\n\n```txt\n$ stairlight init --help\nusage: stairlight init [-h] [-c CONFIG]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -c CONFIG, --config CONFIG\n                        set a Stairlight configuration directory\n  -q, --quiet           keep silence\n```\n\n### map(check)\n\n`stairlight map` creates a new configuration file about undefined settings. `stairlight check` is an alias.\nOptions are the same as `stairlight init`.\n\n### list\n\n`stairlight list` outputs all of tables or SQL URIs.\n\n- Output option(`-o`, `--output`) determines the output type, tables or URIs.\n\n### up\n\n`stairlight up` outputs tables or SQL URIs located upstream(upstairs) from the specified table.\n\n- Use table(`-t`, `--table`) or label(`-l`, `--label`) option to specify tables to search.\n- Output option(`-o`, `--output`) is same as `stairlight list`.\n- Recursive option(`-r`, `--recursive`) is set, Stairlight will find dependencies recursively and output as a list.\n- Verbose option(`-v`, `--verbose`) is set, Stairlight will add detailed information and output it as a dict.\n\n```txt\n$ stairlight up --help\nusage: stairlight up [-h] [-c CONFIG] [--save SAVE] [--load LOAD] (-t TABLE | -l LABEL) [-o {table,uri}]\n                     [-v] [-r]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -c CONFIG, --config CONFIG\n                        set a Stairlight configuration directory\n  -q, --quiet           keep silence\n  --save SAVE           A file path where mapped results will be saved.\n                        You can choose from local file system, GCS, S3.\n  --load LOAD           A file path where mapped results are saved.\n                        You can choose from local file system, GCS, S3.\n                        It can be specified multiple times.\n  -t TABLE, --table TABLE\n                        table names that Stairlight searches for, can be specified\n                        multiple times. e.g. -t PROJECT_a.DATASET_b.TABLE_c -t\n                        PROJECT_d.DATASET_e.TABLE_f\n  -l LABEL, --label LABEL\n                        labels set for the table in mapping configuration, can be specified multiple times.\n                        The separator between key and value should be a colon(:).\n                        e.g. -l key_1:value_1 -l key_2:value_2\n  -o {table,uri}, --output {table,uri}\n                        output type\n  -v, --verbose         return verbose results\n  -r, --recursive       search recursively\n```\n\n### down\n\n`stairlight down` outputs tables or SQL URIs located downstream(downstairs) from the specified table.\nOptions are the same as `stairlight up`.\n\n## Use as a library\n\nStairlight can also be used as a library.\n\n[tosh2230/stairlight-app](https://github.com/tosh2230/stairlight-app) is a sample web application rendering table dependency graph with Stairlight, using Graphviz, Streamlit and Google Cloud Run.\n',
     'author': 'tosh2230',
     'author_email': 'rev.to12@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<4',
+    'python_requires': '>=3.8,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `stairlight-0.7.2/PKG-INFO` & `stairlight-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: stairlight
-Version: 0.7.2
+Version: 0.8.0
 Summary: An end-to-end data lineage tool
 License: MIT
 Author: tosh2230
 Author-email: rev.to12@gmail.com
-Requires-Python: >=3.7.2,<4
+Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dbt-bigquery
```

