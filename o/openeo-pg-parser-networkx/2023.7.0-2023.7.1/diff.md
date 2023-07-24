# Comparing `tmp/openeo_pg_parser_networkx-2023.7.0.tar.gz` & `tmp/openeo_pg_parser_networkx-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openeo_pg_parser_networkx-2023.7.0.tar", max compression
+gzip compressed data, was "openeo_pg_parser_networkx-2023.7.1.tar", max compression
```

## Comparing `openeo_pg_parser_networkx-2023.7.0.tar` & `openeo_pg_parser_networkx-2023.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10765 2023-07-13 12:32:20.062158 openeo_pg_parser_networkx-2023.7.0/LICENSE
--rw-r--r--   0        0        0     5886 2023-07-13 12:32:20.062158 openeo_pg_parser_networkx-2023.7.0/README.md
--rw-r--r--   0        0        0      169 2023-07-13 12:32:20.066158 openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/__init__.py
--rw-r--r--   0        0        0    17457 2023-07-13 12:32:20.066158 openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/graph.py
--rw-r--r--   0        0        0    10134 2023-07-13 12:32:20.066158 openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/pg_schema.py
--rw-r--r--   0        0        0     5125 2023-07-13 12:32:20.066158 openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/process_registry.py
--rw-r--r--   0        0        0     5083 2023-07-13 12:32:20.066158 openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/utils.py
--rw-r--r--   0        0        0     1520 2023-07-13 12:32:20.066158 openeo_pg_parser_networkx-2023.7.0/pyproject.toml
--rw-r--r--   0        0        0     7335 1970-01-01 00:00:00.000000 openeo_pg_parser_networkx-2023.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-07-24 06:52:11.579784 openeo_pg_parser_networkx-2023.7.1/LICENSE
+-rw-r--r--   0        0        0     5886 2023-07-24 06:52:11.583784 openeo_pg_parser_networkx-2023.7.1/README.md
+-rw-r--r--   0        0        0      241 2023-07-24 06:52:11.583784 openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/__init__.py
+-rw-r--r--   0        0        0    17460 2023-07-24 06:52:11.583784 openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/graph.py
+-rw-r--r--   0        0        0    10134 2023-07-24 06:52:11.583784 openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/pg_schema.py
+-rw-r--r--   0        0        0     5125 2023-07-24 06:52:11.583784 openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/process_registry.py
+-rw-r--r--   0        0        0     5083 2023-07-24 06:52:11.583784 openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/utils.py
+-rw-r--r--   0        0        0     1520 2023-07-24 06:52:11.583784 openeo_pg_parser_networkx-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7135 1970-01-01 00:00:00.000000 openeo_pg_parser_networkx-2023.7.1/PKG-INFO
```

### Comparing `openeo_pg_parser_networkx-2023.7.0/LICENSE` & `openeo_pg_parser_networkx-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2023.7.0/README.md` & `openeo_pg_parser_networkx-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/graph.py` & `openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             raw_flat_graph = {"process_graph": raw_flat_graph}
 
         nested_graph = {
             "process_graph": {
                 "root": ProcessGraphUnflattener.unflatten(raw_flat_graph["process_graph"])
             }
         }
-        logger.warning("Deserialised process graph into nested structure")
+        logger.info("Deserialised process graph into nested structure")
         return nested_graph
 
     @staticmethod
     def _parse_datamodel(nested_graph: dict) -> ProcessGraph:
         """
         Parses a nested process graph into the Pydantic datamodel for ProcessGraph.
         """
@@ -214,15 +214,15 @@
         else:
             access_func(new_value=arg, set_bool=True)
 
     def _walk_node(self):
         """
         Parse all the required information from the current node into self.G and recursively walk child nodes.
         """
-        print(f"Walking node {self._EVAL_ENV.node_uid}")
+        logger.info(f"Walking node {self._EVAL_ENV.node_uid}")
 
         self.G.add_node(
             self._EVAL_ENV.node_uid,
             process_id=self._EVAL_ENV.node.process_id,
             resolved_kwargs={},
             node_name=self._EVAL_ENV.node_name,
             process_graph_uid=self._EVAL_ENV.process_graph_uid,
```

### Comparing `openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/pg_schema.py` & `openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/pg_schema.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/process_registry.py` & `openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/process_registry.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2023.7.0/openeo_pg_parser_networkx/utils.py` & `openeo_pg_parser_networkx-2023.7.1/openeo_pg_parser_networkx/utils.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2023.7.0/pyproject.toml` & `openeo_pg_parser_networkx-2023.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openeo-pg-parser-networkx"
-version = "2023.7.0"
+version = "2023.7.1"
 description = "Parse OpenEO process graphs from JSON to traversible Python objects."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/Open-EO/openeo-pg-parser-networkx"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openeo_pg_parser_networkx-2023.7.0/PKG-INFO` & `openeo_pg_parser_networkx-2023.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: openeo-pg-parser-networkx
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Parse OpenEO process graphs from JSON to traversible Python objects.
 Home-page: https://github.com/Open-EO/openeo-pg-parser-networkx
 License: Apache 2.0
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: plot
 Requires-Dist: geojson-pydantic (>=0.5.0,<0.6.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) ; extra == "plot"
 Requires-Dist: networkx (>=2.8.6,<3.0.0)
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
```

