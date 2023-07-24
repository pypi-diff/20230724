# Comparing `tmp/pinject_design-0.1.94.tar.gz` & `tmp/pinject_design-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinject_design-0.1.94.tar", max compression
+gzip compressed data, was "pinject_design-0.1.95.tar", max compression
```

## Comparing `pinject_design-0.1.94.tar` & `pinject_design-0.1.95.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.94/LICENSE
--rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.94/pinject_design/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.94/pinject_design/di/__init__.py
--rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.94/pinject_design/di/app_designed.py
--rw-r--r--   0        0        0     2536 2023-07-12 11:43:38.344272 pinject_design-0.1.94/pinject_design/di/app_injected.py
--rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.94/pinject_design/di/applicative.py
--rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.94/pinject_design/di/ast.py
--rw-r--r--   0        0        0     7402 2023-07-12 11:43:38.344766 pinject_design-0.1.94/pinject_design/di/design.py
--rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.94/pinject_design/di/designed.py
--rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.94/pinject_design/di/dynamic_proxy.py
--rw-r--r--   0        0        0    29449 2023-07-13 04:36:34.812657 pinject_design-0.1.94/pinject_design/di/graph.py
--rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.94/pinject_design/di/implicit_globals.py
--rw-r--r--   0        0        0    32106 2023-07-12 11:43:38.345979 pinject_design-0.1.94/pinject_design/di/injected.py
--rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.94/pinject_design/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.94/pinject_design/di/permissioned/__init__.py
--rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.94/pinject_design/di/permissioned/blueprint.py
--rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.94/pinject_design/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.94/pinject_design/di/provider.py
--rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.94/pinject_design/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.94/pinject_design/di/session.py
--rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.94/pinject_design/di/sessioned.py
--rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.94/pinject_design/di/static_proxy.py
--rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.94/pinject_design/di/test_ast.py
--rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.94/pinject_design/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.94/pinject_design/di/test_graph.py
--rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.94/pinject_design/di/test_injected.py
--rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.94/pinject_design/di/test_proxiable.py
--rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.94/pinject_design/di/util.py
--rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.94/pinject_design/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.94/pinject_design/global_configs
--rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.94/pinject_design/global_configs.py
--rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.94/pinject_design/graph_inspection.py
--rw-r--r--   0        0        0     1612 2023-07-13 03:15:00.373837 pinject_design-0.1.94/pinject_design/helper_structure.py
--rw-r--r--   0        0        0     6272 2023-07-11 12:13:24.403516 pinject_design-0.1.94/pinject_design/helpers.py
--rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinject_design-0.1.94/pinject_design/module_inspector.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.94/pinject_design/nx_graph_util.py
--rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.94/pinject_design/pinject_design.iml
--rw-r--r--   0        0        0    21597 2023-07-13 03:19:07.943777 pinject_design-0.1.94/pinject_design/run_config_utils.py
--rw-r--r--   0        0        0     1590 2023-07-11 12:13:24.405223 pinject_design-0.1.94/pinject_design/run_config_utils_v2.py
--rw-r--r--   0        0        0      938 2023-07-11 12:13:24.405644 pinject_design-0.1.94/pinject_design/test_package/__init__.py
--rw-r--r--   0        0        0      234 2023-07-11 12:13:24.406011 pinject_design-0.1.94/pinject_design/test_package/child/__init__.py
--rw-r--r--   0        0        0      284 2023-07-11 12:13:24.406483 pinject_design-0.1.94/pinject_design/test_package/child/module1.py
--rw-r--r--   0        0        0    17998 2023-07-12 11:43:38.346496 pinject_design-0.1.94/pinject_design/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.94/pinject_design/viz/__init__.py
--rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.94/pinject_design/viz/graph.py
--rw-r--r--   0        0        0      639 2023-07-13 04:36:49.153385 pinject_design-0.1.94/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.94/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.95/LICENSE
+-rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.95/pinject_design/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.95/pinject_design/di/__init__.py
+-rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.95/pinject_design/di/app_designed.py
+-rw-r--r--   0        0        0     2536 2023-07-12 11:43:38.344272 pinject_design-0.1.95/pinject_design/di/app_injected.py
+-rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.95/pinject_design/di/applicative.py
+-rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.95/pinject_design/di/ast.py
+-rw-r--r--   0        0        0     7402 2023-07-12 11:43:38.344766 pinject_design-0.1.95/pinject_design/di/design.py
+-rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.95/pinject_design/di/designed.py
+-rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.95/pinject_design/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    29449 2023-07-13 04:36:34.812657 pinject_design-0.1.95/pinject_design/di/graph.py
+-rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.95/pinject_design/di/implicit_globals.py
+-rw-r--r--   0        0        0    32995 2023-07-18 14:14:44.081504 pinject_design-0.1.95/pinject_design/di/injected.py
+-rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.95/pinject_design/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.95/pinject_design/di/permissioned/__init__.py
+-rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.95/pinject_design/di/permissioned/blueprint.py
+-rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.95/pinject_design/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.95/pinject_design/di/provider.py
+-rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.95/pinject_design/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.95/pinject_design/di/session.py
+-rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.95/pinject_design/di/sessioned.py
+-rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.95/pinject_design/di/static_proxy.py
+-rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.95/pinject_design/di/test_ast.py
+-rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.95/pinject_design/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.95/pinject_design/di/test_graph.py
+-rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.95/pinject_design/di/test_injected.py
+-rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.95/pinject_design/di/test_proxiable.py
+-rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.95/pinject_design/di/util.py
+-rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.95/pinject_design/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.95/pinject_design/global_configs
+-rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.95/pinject_design/global_configs.py
+-rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.95/pinject_design/graph_inspection.py
+-rw-r--r--   0        0        0     1612 2023-07-13 03:15:00.373837 pinject_design-0.1.95/pinject_design/helper_structure.py
+-rw-r--r--   0        0        0     7062 2023-07-20 01:22:08.231237 pinject_design-0.1.95/pinject_design/helpers.py
+-rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinject_design-0.1.95/pinject_design/module_inspector.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.95/pinject_design/nx_graph_util.py
+-rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.95/pinject_design/pinject_design.iml
+-rw-r--r--   0        0        0    22722 2023-07-24 01:52:06.028256 pinject_design-0.1.95/pinject_design/run_config_utils.py
+-rw-r--r--   0        0        0     1590 2023-07-11 12:13:24.405223 pinject_design-0.1.95/pinject_design/run_config_utils_v2.py
+-rw-r--r--   0        0        0      938 2023-07-11 12:13:24.405644 pinject_design-0.1.95/pinject_design/test_package/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-11 12:13:24.406011 pinject_design-0.1.95/pinject_design/test_package/child/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-11 12:13:24.406483 pinject_design-0.1.95/pinject_design/test_package/child/module1.py
+-rw-r--r--   0        0        0    17998 2023-07-12 11:43:38.346496 pinject_design-0.1.95/pinject_design/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.95/pinject_design/viz/__init__.py
+-rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.95/pinject_design/viz/graph.py
+-rw-r--r--   0        0        0      639 2023-07-24 01:57:05.073972 pinject_design-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.95/PKG-INFO
```

### Comparing `pinject_design-0.1.94/LICENSE` & `pinject_design-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/app_designed.py` & `pinject_design-0.1.95/pinject_design/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/app_injected.py` & `pinject_design-0.1.95/pinject_design/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/applicative.py` & `pinject_design-0.1.95/pinject_design/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/ast.py` & `pinject_design-0.1.95/pinject_design/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/design.py` & `pinject_design-0.1.95/pinject_design/di/design.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/designed.py` & `pinject_design-0.1.95/pinject_design/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/dynamic_proxy.py` & `pinject_design-0.1.95/pinject_design/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/graph.py` & `pinject_design-0.1.95/pinject_design/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/injected.py` & `pinject_design-0.1.95/pinject_design/di/injected.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,43 @@
     # Implementing these might end up with pickling issues. due to recursive getattr..?
     # def __call__(self, *args, **kwargs):
     #     return self.proxy(*args, **kwargs)
     #
     # def __getitem__(self, item):
     #     return self.proxy[item]
 
+    @staticmethod
+    def conditional(condition: "Injected[bool]", true_case: "Injected", false_case: "Injected"):
+        return ConditionalInjected(condition, true_case, false_case)
+
+    @staticmethod
+    def procedure(*targets: "Injected"):
+        """
+        Runs the targets in order, and returns the last one.
+        This is useful for running injecteds which performs side effects.
+        :param targets:
+        :return:
+        """
+        return Injected.list(*targets).map(lambda items: items[-1])
+
+    @staticmethod
+    def conditional_preparation(
+            condition: "Injected[bool]",
+            preparation: "Injected",
+            utilization: "Injected"
+    ):
+        return Injected.conditional(
+            condition,
+            utilization,
+            Injected.procedure(
+                preparation,
+                utilization
+            )
+        )
+
 
 @dataclass
 class ConditionalInjected(Injected):
     condition: Injected[bool]
     true: Injected
     false: Injected
 
@@ -425,14 +454,15 @@
 class InjectedCache(Injected[T]):
     cache: Injected[Dict]
     program: Injected[T]
     program_dependencies: List[Injected]
 
     def __post_init__(self):
         self.program = Injected.ensure_injected(self.program)
+
         def impl(session, cache: Dict, *deps):
             logger.info(f"Checking for cache with deps:{deps}")
             sha256_key = hashlib.sha256(str(deps).encode()).hexdigest()
             hash_key = sha256_key
             if hash_key not in cache:
                 logger.info(f"Cache miss for {deps}")
                 data = session[self.program]
@@ -837,14 +867,16 @@
 def injected_class(cls):
     return injected_function(cls)
 
 
 def injected(name: str):
     return Injected.by_name(name).proxy
 
+
 def add_viz_metadata(metadata: Dict[str, Any]):
-    def impl(tgt:Injected):
+    def impl(tgt: Injected):
         if not hasattr(tgt, '__viz_metadata__'):
             tgt.__viz_metadata__ = dict()
         tgt.__viz_metadata__.update(metadata)
         return tgt
-    return impl
+
+    return impl
```

### Comparing `pinject_design-0.1.94/pinject_design/di/injected_analysis.py` & `pinject_design-0.1.95/pinject_design/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/permissioned/blueprint.py` & `pinject_design-0.1.95/pinject_design/di/permissioned/blueprint.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/proxiable.py` & `pinject_design-0.1.95/pinject_design/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/session.py` & `pinject_design-0.1.95/pinject_design/di/session.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/sessioned.py` & `pinject_design-0.1.95/pinject_design/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/static_proxy.py` & `pinject_design-0.1.95/pinject_design/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/test_dynamic_proxy.py` & `pinject_design-0.1.95/pinject_design/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/test_graph.py` & `pinject_design-0.1.95/pinject_design/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/test_injected.py` & `pinject_design-0.1.95/pinject_design/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/test_proxiable.py` & `pinject_design-0.1.95/pinject_design/di/test_proxiable.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/di/util.py` & `pinject_design-0.1.95/pinject_design/di/util.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/exceptions.py` & `pinject_design-0.1.95/pinject_design/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/graph_inspection.py` & `pinject_design-0.1.95/pinject_design/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/helper_structure.py` & `pinject_design-0.1.95/pinject_design/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/helpers.py` & `pinject_design-0.1.95/pinject_design/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from returns.maybe import maybe
 
 from pinject_design import injected_function, Injected, Designed, Design
 from pinject_design.di.app_injected import InjectedEvalContext
 from pinject_design.di.proxiable import DelegatedVar
 from pinject_design.module_inspector import ModuleVarSpec, inspect_module_for_type, get_project_root
 from pinject_design.helper_structure import IdeaRunConfigurations, MetaContext
-
-
+from loguru import logger
+from dataclasses import dataclass
 @injected_function
 def inspect_and_make_configurations(
         injected_to_idea_configs,
         logger,
         /,
         module_path
 ) -> IdeaRunConfigurations:
@@ -26,14 +26,24 @@
     logger.info(f"found {len(runnables)} injecteds")
     for tgt in runnables:
         if isinstance(tgt, ModuleVarSpec):
             results.update(injected_to_idea_configs(tgt).configs)
     return IdeaRunConfigurations(configs=results)
 
 
+@dataclass
+class ModulePath:
+    """
+    represents a path where a variable is defined.
+    like a.b.c.d
+    """
+    path:str
+    def load(self):
+        return load_variable_by_module_path(self.path)
+
 def load_variable_by_module_path(full_module_path):
     from loguru import logger
     logger.info(f"loading {full_module_path}")
     module_path_parts = full_module_path.split('.')
     variable_name = module_path_parts[-1]
     module_path = '.'.join(module_path_parts[:-1])
 
@@ -123,22 +133,30 @@
     :param file_path:
     :param attr_name:
     :return:
     """
     from loguru import logger
     if root_module_path is None:
         root_module_path = Path(get_project_root(str(file_path)))
+    file_path = file_path.absolute()
+    assert str(file_path).endswith(".py"),f"a python file path must be provided, got:{file_path}"
+    logger.debug(f"project root path:{root_module_path}")
     if not str(file_path).startswith(str(root_module_path)):
+        # logger.error(f"file path {file_path} is not under root module path {root_module_path}")
         return
 
     relative_path = file_path.relative_to(root_module_path)
+    logger.debug(f"relative path:{relative_path}")
     module_name = os.path.splitext(str(relative_path).replace(os.sep, '.'))[0]
     if module_name not in sys.modules:
         logger.info(f"importing module: {module_name}")
         spec = importlib.util.spec_from_file_location(module_name, file_path)
+        if spec is None:
+            logger.error(f"cannot find spec for {module_name} at {file_path}")
+            return
         module = importlib.util.module_from_spec(spec)
         sys.modules[module_name] = module
         spec.loader.exec_module(module)
     module = sys.modules[module_name]
     if hasattr(module, attr_name):
         yield ModuleVarSpec(
             var=getattr(module, attr_name),
@@ -153,17 +171,18 @@
         else:
             grandparent_dir = parent_dir.parent
             grandparent_file_path = grandparent_dir / '__init__.py'
             if grandparent_file_path.exists():
                 yield from walk_module_attr(grandparent_file_path, attr_name, root_module_path)
 
 
-def gather_meta_design(file_path: Path, meta_design_name: str = "__meta_design__") -> MetaContext:
+def gather_meta_context(file_path: Path, meta_design_name: str = "__meta_design__") -> MetaContext:
     designs = list(walk_module_attr(file_path, meta_design_name))
     designs.reverse()
     res = Design()
     for item in designs:
+        logger.debug(f"{meta_design_name} at :{item.var_path}")
         res = res + item.var
     return MetaContext(
         trace=designs,
         accumulated=res
     )
```

### Comparing `pinject_design-0.1.94/pinject_design/module_inspector.py` & `pinject_design-0.1.95/pinject_design/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/nx_graph_util.py` & `pinject_design-0.1.95/pinject_design/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/run_config_utils.py` & `pinject_design-0.1.95/pinject_design/run_config_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 So I guess I need to introduce a new data structure.
 """
 import asyncio
 import importlib
 import inspect
 import json
 import os
+import sys
 from collections import defaultdict
 from datetime import datetime
 from pathlib import Path
 from pprint import pformat
 from typing import Optional, List, Dict, Coroutine, OrderedDict, Callable
 
+from loguru import logger
 import fire
 import loguru
 import returns.maybe as raybe
 from cytoolz import memoize
 from expression import Nothing
 from returns.maybe import Maybe, Some, maybe
 from returns.result import safe, Success, Failure
@@ -46,17 +48,18 @@
 from pinject_design import Injected, Design
 from pinject_design.di.injected import injected_function
 from pinject_design.di.proxiable import DelegatedVar
 from pinject_design.di.util import instances, providers
 from pinject_design.helper_structure import IdeaRunConfigurations, RunnablePair, RunnableValue, \
     IdeaRunConfiguration
 from pinject_design.helpers import inspect_and_make_configurations, load_variable_by_module_path, \
-    get_design_path_from_var_path, get_runnables, find_default_design_paths, gather_meta_design
+    get_design_path_from_var_path, get_runnables, find_default_design_paths, gather_meta_context
 from pinject_design.module_inspector import ModuleVarSpec, inspect_module_for_type, get_project_root
 from pinject_design.run_config_utils_v2 import RunInjected
+from dataclasses import dataclass
 
 
 def maybe__or__(self, other):
     match self:
         case Some(x):
             return self
         case raybe.Nothing:
@@ -157,14 +160,15 @@
         default_working_dir: Maybe[str],
         extract_args_for_runnable,
         logger,
         custom_idea_config_creator: IdeaConfigCreator,
         /,
         tgt: ModuleVarSpec
 ):
+    # question is: how can we pass the override to run_injected?
     logger.info(f"using custom_idea_config_creator {custom_idea_config_creator} for {tgt}")
     name = tgt.var_path.split(".")[-1]
     config_args = {
         'script_path': entrypoint_path,
         'interpreter_path': interpreter_path,
         'working_dir': default_working_dir.value_or(os.getcwd())
     }
@@ -236,15 +240,15 @@
     cmd = f"""osascript -e {script} """
     os.system(cmd)
     return f"Notified user with text: {org}"
 
 
 # maybe we want to distinguish the error with its complexity and pass it to gpt if required.
 
-def run_anything(cmd: str, var_path, design_path, *args, **kwargs):
+def run_anything(cmd: str, var_path, design_path, return_result=False, *args, **kwargs):
     # TODO pass the resulting errors into gpt to give better error messages.
     # for that, I need to capture the stderr/stdout
     # get the var and design
     # then run it based on cmd with args/kwargs
     # TODO I need a way to hook the run configurations
     # 1. add hooks for create_configurations => let the create_configurations load hook_design.
     # - this can make it possible to return a design runner that submits the design to cluster / local / docker etc.
@@ -258,15 +262,15 @@
         meta = {}
     overrides = meta.get("overrides", instances())
     var: Injected = Injected.ensure_injected(load_variable_by_module_path(var_path))
     design: Design = load_variable_by_module_path(design_path)
     design = design + overrides
     # if you return python object, fire will try to use it as a command object
     # we need to inspect __runnable_metadata__
-    logger.info(f"running target:{var}")
+    logger.info(f"running target:{var} with cmd {cmd}, args {args}, kwargs {kwargs}")
     logger.info(f"metadata obtained from injected: {meta}")
     res = None
     try:
         if cmd == 'call':
             res = design.provide(var)(*args, **kwargs)
             if isinstance(res, Coroutine):
                 res = asyncio.run(res)
@@ -286,26 +290,29 @@
             logger.info(f"visualizing {var_path} with design {design_path}")
             logger.info(f"deps:{var.dependencies()}")
             design.to_vis_graph().show_injected_html(var)
     except Exception as e:
         notify(f"Run failed with error:\n{e}", sound='Frog')
         raise e
     notify(f"Run result:\n{str(res)[:100]}")
+    if return_result:
+        return res
 
 
 def run_injected(
         cmd,
         var_path,
         design_path: str = None,
+        return_result=False,
         *args, **kwargs
 ):
     if design_path is None:
         design_path = get_design_path_from_var_path(var_path)
     assert design_path, f"design path must be a valid module path, got:{design_path}"
-    return run_anything(cmd, var_path, design_path, *args, **kwargs)
+    return run_anything(cmd, var_path, design_path,return_result=return_result, *args, **kwargs)
 
 
 def run_with_kotlin(module_path: str, kotlin_zmq_address: str = None):
     d = instances()
     if kotlin_zmq_address is not None:
         d += instances(
             kotlin_zmq_address=kotlin_zmq_address
@@ -328,52 +335,62 @@
 def find_injecteds(
         module_path
 ):
     injecteds = get_runnables(module_path)
     return print(json.dumps([i.var_path for i in injecteds]))
 
 
+@dataclass
+class ConfigCreationArgs:
+    module_path: str
+    default_design_path: str = None
+    entrypoint_path: str = None
+    interpreter_path: str = None
+    working_dir: str = None
+
+    def to_design(self):
+        logger.debug(f"python paths:{sys.path}")
+        meta_context = gather_meta_context(Path(self.module_path))
+
+        design = providers(
+            project_root=lambda: Path(get_project_root(self.module_path)),
+            entrypoint_path=lambda: self.entrypoint_path or __file__,
+            interpreter_path=lambda: self.interpreter_path or sys.executable,
+            default_design_paths=lambda: find_default_design_paths(self.module_path, self.default_design_path),
+            default_working_dir=lambda project_root: maybe(lambda: self.working_dir)() | Some(
+                str(project_root)),
+            default_design_path=lambda default_design_paths: default_design_paths[0]
+        ) + instances(
+            logger=loguru.logger,
+            custom_idea_config_creator=lambda x: [],  # type ConfigCreator
+            meta_context=meta_context,
+        ) + meta_context.accumulated
+        logger.info(f"using meta design:{meta_context.accumulated}")
+        logger.info(f"custom_idea_config_creator:{design['custom_idea_config_creator']}")
+        return design
+
+
+# since this is an entrypoint, we can't use @injected_function here.
 def create_idea_configurations(
         module_path,
         default_design_path=None,
         entrypoint_path=None,
         interpreter_path=None,
         working_dir=None,
         print_to_stdout=True,
 ):
-    from loguru import logger
-    import sys
     pinject_design.global_configs.PINJECT_DESIGN_TRACK_ORIGIN = False
-    logger.debug(f"python paths:{sys.path}")
-    project_root = get_project_root(module_path)
-    # logger.debug(f"env python_path:{os.environ['PYTHONPATH']}")
-    entrypoint_path = entrypoint_path or __file__
-    interpreter_path = interpreter_path or sys.executable
-    logger.info(f"looking for default design paths from {module_path}")
-    default_design_paths = find_default_design_paths(module_path, default_design_path)
-    default_working_dir = maybe(lambda: working_dir)() | maybe(get_project_root)(module_path)
-
-    # somehow find the default design
-    # for example by looking at a config file in the project root
-    # 1. look for default design path string
-    # 2. look for default working dir string
-    meta_context = gather_meta_design(Path(module_path))
-
-    design = instances(
+    args = ConfigCreationArgs(
+        module_path=module_path,
+        default_design_path=default_design_path,
         entrypoint_path=entrypoint_path,
         interpreter_path=interpreter_path,
-        default_design_paths=default_design_paths,
-        default_working_dir=default_working_dir,
-        logger=loguru.logger,
-        custom_idea_config_creator=lambda x: [],  # type ConfigCreator
-        meta_context=meta_context,
-        project_root=Path(project_root),
-    ) + meta_context.accumulated
-    logger.info(f"using meta design:{meta_context.accumulated}")
-    logger.info(f"custom_idea_config_creator:{design['custom_idea_config_creator']}")
+        working_dir=working_dir,
+    )
+    design = args.to_design()
     g = design.to_graph()
     configs: IdeaRunConfigurations = g[inspect_and_make_configurations(module_path)]
     pinject_design.global_configs.PINJECT_DESIGN_TRACK_ORIGIN = True
     if print_to_stdout:
         print(configs.json())
     else:
         return configs
@@ -391,20 +408,29 @@
 def retrieve_design_path_from_injected(tgt: Injected):
     meta = safe(getattr)(tgt, '__runnable_metadata__')
     match meta:
         case {"default_design_path": design_path}:
             return design_path
 
 
-def make_sandbox(module_file_path, var_name):
-    tgts = get_runnables(module_file_path)
+def get_var_spec_from_module_path_and_name(module_path: str, var_name: str) -> ModuleVarSpec:
+    tgts = get_runnables(module_path)
     name_to_tgt = {tgt.var_path.split(".")[-1]: tgt for tgt in tgts}
     tgt: ModuleVarSpec = name_to_tgt[var_name]
-    default_design_paths = find_default_design_paths(module_file_path, None)
-    default_design_path = default_design_paths[0]
+    return tgt
+
+
+@injected_function
+def _make_sandbox_impl(
+        default_design_path: str,
+        /,
+        module_file_path: str,
+        var_name: str,
+):
+    tgt: ModuleVarSpec = get_var_spec_from_module_path_and_name(module_file_path, var_name)
     default_design_path_parent = ".".join(default_design_path.split('.')[:-1])
     var_path_parent = ".".join(tgt.var_path.split('.')[:-1])
     # let's make a file for sandbox,
     # format datetime like 20230101_010101
     datetime_str_as_name = datetime.now().strftime("%Y%m%d_%H%M%S")
     sandbox_name = f"{var_name}_sandbox_{datetime_str_as_name}.py"
     sandbox_path = os.path.join(os.path.dirname(module_file_path), sandbox_name)
@@ -414,14 +440,27 @@
             design_name=default_design_path.split('.')[-1],
             var_path=var_path_parent,
             var_name=var_name
         ))
     print(sandbox_path)
 
 
+def make_sandbox(module_file_path, var_name):
+    args = ConfigCreationArgs(
+        module_path=module_file_path,
+        default_design_path=None,
+        entrypoint_path=None,
+        interpreter_path=None,
+        working_dir=None,
+    )
+    design = args.to_design()
+    g = design.to_graph()
+    return g[_make_sandbox_impl](module_file_path=module_file_path, var_name=var_name)
+
+
 def create_main_command(
         targets: OrderedDict[str, Injected],
         design_paths: OrderedDict[str, str],
 ):
     def main(target: str, design_path: Optional[str] = None):
         tgt = targets[target]
         if design_path is None:
@@ -440,15 +479,14 @@
         main_override_resolver,
         /,
         target: str,
         design_path: Optional[str] = None,
         overrides: str = None,
         show_graph: bool = False
 ) -> Optional[RunnablePair]:
-
     tgt = main_targets[target]
     if design_path is None:
         design_path = main_design_paths[list(main_design_paths.keys())[0]]
     main_overrides = main_override_resolver(overrides)
     design = load_variable_by_module_path(design_path) + main_overrides
     pair = RunnablePair(target=tgt, design=design)
     if show_graph:
@@ -475,22 +513,23 @@
 
 def provide_design_paths(logger, module_path) -> OrderedDict[str, str]:
     design_paths = find_default_design_paths(module_path, None)
     design_paths = {design_path.split('.')[-1]: design_path for design_path in design_paths}
     logger.info(f"main design paths:{pformat(design_paths.keys())}")
     return design_paths
 
+
 @injected_function
 def main_override_resolver(query) -> Design:
     """
     :param query: can be filename with .json, .yaml.
     we can also try parsing it as json.
     :return:
     """
-    if isinstance(query,dict):
+    if isinstance(query, dict):
         return instances(**query)
     elif query is None:
         return Design()
     elif query.endswith('.json'):
         import json
         if not Path(query).exists():
             raise ValueError(f"cannot find {query} for configuration.")
@@ -589,15 +628,15 @@
     return fire.Fire({
         k: make_enetrypoint(conf[0]) for k, conf in confs.configs.items()
     })
 
 
 def run_idea_conf(conf: IdeaRunConfiguration, *args, **kwargs):
     pre_args = conf.arguments[1:]
-    return run_injected(*pre_args, *args, **kwargs)
+    return run_injected(*pre_args,return_result=True, *args, **kwargs)
 
 
 @memoize
 def get_designs_from_module(module_path: Path):
     from loguru import logger
     logger.info(f"trying to import designs from {module_path}")
```

### Comparing `pinject_design-0.1.94/pinject_design/run_config_utils_v2.py` & `pinject_design-0.1.95/pinject_design/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/test_package/__init__.py` & `pinject_design-0.1.95/pinject_design/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pinject_design/visualize_di.py` & `pinject_design-0.1.95/pinject_design/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.94/pyproject.toml` & `pinject_design-0.1.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinject-design"
-version = "0.1.94"
+version = "0.1.95"
 description = "immutable wrapper for pinject"
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 makefun = "*"
```

### Comparing `pinject_design-0.1.94/PKG-INFO` & `pinject_design-0.1.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinject-design
-Version: 0.1.94
+Version: 0.1.95
 Summary: immutable wrapper for pinject
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

