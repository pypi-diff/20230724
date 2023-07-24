# Comparing `tmp/catalogue-2.0.9.tar.gz` & `tmp/catalogue-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalogue-2.0.9.tar", last modified: Mon Jul 24 07:26:24 2023, max compression
+gzip compressed data, was "catalogue-2.1.0.tar", last modified: Wed Jul  6 07:38:23 2022, max compression
```

## Comparing `catalogue-2.0.9.tar` & `catalogue-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-24 07:26:24.780127 catalogue-2.0.9/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-07-24 07:26:09.000000 catalogue-2.0.9/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       16 2023-07-24 07:26:09.000000 catalogue-2.0.9/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    13949 2023-07-24 07:26:24.780127 catalogue-2.0.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    12851 2023-07-24 07:26:09.000000 catalogue-2.0.9/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-24 07:26:24.780127 catalogue-2.0.9/catalogue/
--rw-r--r--   0 vsts      (1001) docker     (122)     8628 2023-07-24 07:26:09.000000 catalogue-2.0.9/catalogue/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-24 07:26:24.780127 catalogue-2.0.9/catalogue/_importlib_metadata/
--rw-r--r--   0 vsts      (1001) docker     (122)    20204 2023-07-24 07:26:09.000000 catalogue-2.0.9/catalogue/_importlib_metadata/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2406 2023-07-24 07:26:09.000000 catalogue-2.0.9/catalogue/_importlib_metadata/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-24 07:26:24.780127 catalogue-2.0.9/catalogue/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-24 07:26:09.000000 catalogue-2.0.9/catalogue/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5153 2023-07-24 07:26:09.000000 catalogue-2.0.9/catalogue/tests/test_catalogue.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-24 07:26:24.780127 catalogue-2.0.9/catalogue.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    13949 2023-07-24 07:26:24.000000 catalogue-2.0.9/catalogue.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      407 2023-07-24 07:26:24.000000 catalogue-2.0.9/catalogue.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-24 07:26:24.000000 catalogue-2.0.9/catalogue.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-07-24 07:26:24.000000 catalogue-2.0.9/catalogue.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-07-24 07:26:24.000000 catalogue-2.0.9/catalogue.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-24 07:26:24.000000 catalogue-2.0.9/catalogue.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)     1356 2023-07-24 07:26:24.780127 catalogue-2.0.9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-24 07:26:09.000000 catalogue-2.0.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 07:38:23.761313 catalogue-2.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1073 2022-07-06 07:38:12.000000 catalogue-2.1.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-07-06 07:38:12.000000 catalogue-2.1.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)    30703 2022-07-06 07:38:23.761313 catalogue-2.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)    29662 2022-07-06 07:38:12.000000 catalogue-2.1.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 07:38:23.757313 catalogue-2.1.0/catalogue/
+-rw-r--r--   0 vsts      (1001) docker     (121)       64 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 07:38:23.757313 catalogue-2.1.0/catalogue/_importlib_metadata/
+-rw-r--r--   0 vsts      (1001) docker     (121)    20204 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/_importlib_metadata/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2406 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/_importlib_metadata/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 07:38:23.757313 catalogue-2.1.0/catalogue/config/
+-rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    46551 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/config/config.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1550 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/config/util.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8710 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 07:38:23.761313 catalogue-2.1.0/catalogue/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      488 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5240 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/tests/test_catalogue.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    51957 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4045 2022-07-06 07:38:12.000000 catalogue-2.1.0/catalogue/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 07:38:23.757313 catalogue-2.1.0/catalogue.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)    30703 2022-07-06 07:38:23.000000 catalogue-2.1.0/catalogue.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      593 2022-07-06 07:38:23.000000 catalogue-2.1.0/catalogue.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-06 07:38:23.000000 catalogue-2.1.0/catalogue.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       62 2022-07-06 07:38:23.000000 catalogue-2.1.0/catalogue.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       10 2022-07-06 07:38:23.000000 catalogue-2.1.0/catalogue.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-06 07:38:23.000000 catalogue-2.1.0/catalogue.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)     1310 2022-07-06 07:38:23.761313 catalogue-2.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      153 2022-07-06 07:38:12.000000 catalogue-2.1.0/setup.py
```

### Comparing `catalogue-2.0.9/LICENSE` & `catalogue-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catalogue-2.0.9/catalogue/__init__.py` & `catalogue-2.1.0/catalogue/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Sequence, Any, Dict, Tuple, Callable, Optional, TypeVar, Union
-from typing import List
 import inspect
 
 try:  # Python 3.8
     import importlib.metadata as importlib_metadata
 except ImportError:
     from . import _importlib_metadata as importlib_metadata  # type: ignore
 
@@ -117,37 +116,31 @@
 
     def get_entry_points(self) -> Dict[str, Any]:
         """Get registered entry points from other packages for this namespace.
 
         RETURNS (Dict[str, Any]): Entry points, keyed by name.
         """
         result = {}
-        for entry_point in self._get_entry_points():
+        for entry_point in AVAILABLE_ENTRY_POINTS.get(self.entry_point_namespace, []):
             result[entry_point.name] = entry_point.load()
         return result
 
     def get_entry_point(self, name: str, default: Optional[Any] = None) -> Any:
         """Check if registered entry point is available for a given name in the
         namespace and load it. Otherwise, return the default value.
 
         name (str): Name of entry point to load.
         default (Any): The default value to return.
         RETURNS (Any): The loaded entry point or the default value.
         """
-        for entry_point in self._get_entry_points():
+        for entry_point in AVAILABLE_ENTRY_POINTS.get(self.entry_point_namespace, []):
             if entry_point.name == name:
                 return entry_point.load()
         return default
 
-    def _get_entry_points(self) -> List[importlib_metadata.EntryPoint]:
-        if hasattr(AVAILABLE_ENTRY_POINTS, "select"):
-            return AVAILABLE_ENTRY_POINTS.select(group=self.entry_point_namespace)
-        else:  # dict
-            return AVAILABLE_ENTRY_POINTS.get(self.entry_point_namespace, [])
-
     def find(self, name: str) -> Dict[str, Optional[Union[str, int]]]:
         """Find the information about a registered function, including the
         module and path to the file it's defined in, the line number and the
         docstring, if available.
 
         name (str): Name of the registered function.
         RETURNS (Dict[str, Optional[Union[str, int]]]): The function info.
@@ -236,9 +229,31 @@
     if namespace not in REGISTRY:
         raise RegistryError(f"Can't get namespace {namespace} (not in registry)")
     removed = REGISTRY[namespace]
     del REGISTRY[namespace]
     return removed
 
 
+def _empty_registry() -> None:
+    """ Empties REGISTRY completely. """
+    global REGISTRY
+    REGISTRY = {}
+
+
 class RegistryError(ValueError):
     pass
+
+
+__all__ = [
+    "AVAILABLE_ENTRY_POINTS",
+    "REGISTRY",
+    "create",
+    "Registry",
+    "check_exists",
+    "_get",
+    "_get_all",
+    "_set",
+    "_remove",
+    "_empty_registry",
+    "RegistryError",
+    "importlib_metadata"
+]
```

### Comparing `catalogue-2.0.9/catalogue/_importlib_metadata/__init__.py` & `catalogue-2.1.0/catalogue/_importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `catalogue-2.0.9/catalogue/_importlib_metadata/_compat.py` & `catalogue-2.1.0/catalogue/_importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `catalogue-2.0.9/catalogue/tests/test_catalogue.py` & `catalogue-2.1.0/catalogue/tests/test_catalogue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,41 @@
+from typing import Dict, Tuple, Any
 import pytest
 import sys
 from pathlib import Path
 import catalogue
 
 
 @pytest.fixture(autouse=True)
 def cleanup():
-    catalogue.REGISTRY = {}
+    # Don't delete entries needed for config tests.
+    for key in set(catalogue.REGISTRY.keys()) - set(filter_registry("config").keys()):
+        catalogue.REGISTRY.pop(key)
     yield
 
 
+def filter_registry(keep: str) -> Dict[Tuple[str, ...], Any]:
+    """
+    Filters registry objects for tests.
+    test_mode (str): One of ("catalogue", "config"). Only entries in the registry belonging to the corresponding tests
+                     will be returned.
+
+    RETURNS (Dict[Tuple[str], Any]): entries in registry without those added for config tests.
+    """
+
+    assert keep in ("catalogue", "config")
+    return {
+        key: val for key, val in catalogue.REGISTRY.items()
+        if ("config_tests" in key) is (keep == "config")
+    }
+
+
 def test_get_set():
     catalogue._set(("a", "b", "c"), "test")
-    assert len(catalogue.REGISTRY) == 1
+    assert len(filter_registry("catalogue")) == 1
     assert ("a", "b", "c") in catalogue.REGISTRY
     assert catalogue.check_exists("a", "b", "c")
     assert catalogue.REGISTRY[("a", "b", "c")] == "test"
     assert catalogue._get(("a", "b", "c")) == "test"
     with pytest.raises(catalogue.RegistryError):
         catalogue._get(("a", "b", "d"))
     with pytest.raises(catalogue.RegistryError):
@@ -57,16 +76,16 @@
     all_items = catalogue._get_all(("a", "b", "c"))
     assert len(all_items) == 1
     assert ("a", "b", "c") in all_items
     assert len(catalogue._get_all(("a", "b", "c", "d"))) == 0
 
 
 def test_create_single_namespace():
+    assert filter_registry("catalogue") == {}
     test_registry = catalogue.create("test")
-    assert catalogue.REGISTRY == {}
 
     @test_registry.register("a")
     def a():
         pass
 
     def b():
         pass
@@ -98,57 +117,33 @@
     items = test_registry.get_all()
     assert len(items) == 1
     assert items["z"] == z
     assert catalogue.check_exists("x", "y", "z")
     assert catalogue._get(("x", "y", "z")) == z
 
 
-def _check_entry_points():
-    # Check entry points for test_entry_points_older() and test_entry_points_newer().
-    assert catalogue.REGISTRY == {}
+@pytest.mark.skipif(sys.version_info >= (3, 10), reason="Test is not yet updated for 3.10 importlib_metadata API")
+def test_entry_points():
+    # Create a new EntryPoint object by pretending we have a setup.cfg and
+    # use one of catalogue's util functions as the advertised function
+    ep_string = "[options.entry_points]test_foo\n    bar = catalogue.registry:check_exists"
+    ep = catalogue.importlib_metadata.EntryPoint._from_text(ep_string)
+    catalogue.AVAILABLE_ENTRY_POINTS["test_foo"] = ep
+    assert filter_registry("catalogue") == {}
     test_registry = catalogue.create("test", "foo", entry_points=True)
     entry_points = test_registry.get_entry_points()
     assert "bar" in entry_points
     assert entry_points["bar"] == catalogue.check_exists
     assert test_registry.get_entry_point("bar") == catalogue.check_exists
-    assert catalogue.REGISTRY == {}
+    assert filter_registry("catalogue") == {}
     assert test_registry.get("bar") == catalogue.check_exists
     assert test_registry.get_all() == {"bar": catalogue.check_exists}
     assert "bar" in test_registry
 
 
-@pytest.mark.skipif(
-    sys.version_info >= (3, 10),
-    reason="Test does not support >=3.10 importlib_metadata API",
-)
-def test_entry_points_older():
-    # Create a new EntryPoint object by pretending we have a setup.cfg and
-    # use one of catalogue's util functions as the advertised function
-    ep_string = "[options.entry_points]test_foo\n    bar = catalogue:check_exists"
-    ep = catalogue.importlib_metadata.EntryPoint._from_text(ep_string)
-    catalogue.AVAILABLE_ENTRY_POINTS["test_foo"] = ep
-    _check_entry_points()
-
-
-@pytest.mark.skipif(
-    sys.version_info < (3, 10),
-    reason="Test does not support <3.10 importlib_metadata API",
-)
-def test_entry_points_newer():
-    # Create a new EntryPoint object by pretending we have a setup.cfg and
-    # use one of catalogue's util functions as the advertised function
-    ep = catalogue.importlib_metadata.EntryPoint(
-        "bar", "catalogue:check_exists", "test_foo"
-    )
-    catalogue.AVAILABLE_ENTRY_POINTS[
-        "test_foo"
-    ] = catalogue.importlib_metadata.EntryPoints([ep])
-    _check_entry_points()
-
-
 def test_registry_find():
     test_registry = catalogue.create("test_registry_find")
     name = "a"
 
     @test_registry.register(name)
     def a():
         """This is a registered function."""
```

### Comparing `catalogue-2.0.9/setup.cfg` & `catalogue-2.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-version = 2.0.9
-description = Super lightweight function registries for your library
+version = 2.1.0
+description = Lightweight function registries for your library
 url = https://github.com/explosion/catalogue
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -18,15 +18,14 @@
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
 install_requires =
```

