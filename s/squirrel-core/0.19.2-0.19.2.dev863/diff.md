# Comparing `tmp/squirrel_core-0.19.2.tar.gz` & `tmp/squirrel_core-0.19.2.dev863.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrel_core-0.19.2.tar", max compression
+gzip compressed data, was "squirrel_core-0.19.2.dev863.tar", max compression
```

## Comparing `squirrel_core-0.19.2.tar` & `squirrel_core-0.19.2.dev863.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11348 2023-07-24 11:05:24.845599 squirrel_core-0.19.2/LICENSE
--rw-r--r--   0        0        0     5424 2023-07-24 11:05:24.845599 squirrel_core-0.19.2/README.md
--rw-r--r--   0        0        0     2999 2023-07-24 11:09:48.985567 squirrel_core-0.19.2/pyproject.toml
--rw-r--r--   0        0        0       80 2023-07-24 11:05:24.857600 squirrel_core-0.19.2/squirrel/__init__.py
--rw-r--r--   0        0        0     3253 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/benchmark/quantify_randomness.py
--rw-r--r--   0        0        0      147 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/catalog/__init__.py
--rw-r--r--   0        0        0    14080 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/catalog/catalog.py
--rw-r--r--   0        0        0      937 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/catalog/source.py
--rw-r--r--   0        0        0     2208 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/catalog/yaml.py
--rw-r--r--   0        0        0      581 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/constants.py
--rw-r--r--   0        0        0      887 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/csv.py
--rw-r--r--   0        0        0     4511 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/data_frame.py
--rw-r--r--   0        0        0     8479 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/driver.py
--rw-r--r--   0        0        0      977 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/excel.py
--rw-r--r--   0        0        0     1045 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/feather.py
--rw-r--r--   0        0        0     2127 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/file.py
--rw-r--r--   0        0        0     2192 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/jsonl.py
--rw-r--r--   0        0        0     1099 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/msgpack.py
--rw-r--r--   0        0        0     1203 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/parquet.py
--rw-r--r--   0        0        0     5113 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/source_combiner.py
--rw-r--r--   0        0        0     4586 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/store.py
--rw-r--r--   0        0        0     3230 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/driver/zarr.py
--rw-r--r--   0        0        0        0 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/framework/__init__.py
--rw-r--r--   0        0        0      165 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/framework/exceptions.py
--rw-r--r--   0        0        0     2234 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/framework/io.py
--rw-r--r--   0        0        0       30 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/framework/plugins/__init__.py
--rw-r--r--   0        0        0      788 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/framework/plugins/hookimpl.py
--rw-r--r--   0        0        0      644 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/framework/plugins/hookspec.py
--rw-r--r--   0        0        0     1566 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/framework/plugins/plugin_manager.py
--rw-r--r--   0        0        0      410 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/fsspec/__init__.py
--rw-r--r--   0        0        0     1313 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/fsspec/custom_gcsfs.py
--rw-r--r--   0        0        0     2211 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/fsspec/fs.py
--rw-r--r--   0        0        0        0 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/integration_test/__init__.py
--rw-r--r--   0        0        0      466 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/integration_test/conftest.py
--rw-r--r--   0        0        0     1747 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/integration_test/helpers.py
--rw-r--r--   0        0        0     3837 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/integration_test/shared_fixtures.py
--rw-r--r--   0        0        0     5841 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
--rw-r--r--   0        0        0      471 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/iterstream/__init__.py
--rw-r--r--   0        0        0    23773 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/iterstream/base.py
--rw-r--r--   0        0        0     9230 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/iterstream/iterators.py
--rw-r--r--   0        0        0     2289 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/iterstream/metrics.py
--rw-r--r--   0        0        0     5999 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/iterstream/source.py
--rw-r--r--   0        0        0     5202 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/iterstream/torch_composables.py
--rw-r--r--   0        0        0      224 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/py.typed
--rw-r--r--   0        0        0      263 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/serialization/__init__.py
--rw-r--r--   0        0        0     4805 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/serialization/jsonl.py
--rw-r--r--   0        0        0     3471 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/serialization/msgpack.py
--rw-r--r--   0        0        0      750 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/serialization/serializer.py
--rw-r--r--   0        0        0      222 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/store/__init__.py
--rw-r--r--   0        0        0     4588 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/store/filesystem.py
--rw-r--r--   0        0        0     4864 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/store/squirrel_store.py
--rw-r--r--   0        0        0     1880 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/store/store.py
--rw-r--r--   0        0        0      110 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/zarr/__init__.py
--rw-r--r--   0        0        0     6137 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/zarr/group.py
--rw-r--r--   0        0        0     2041 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/zarr/key.py
--rw-r--r--   0        0        0     3794 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/zarr/store.py
--rw-r--r--   0        0        0      832 2023-07-24 11:05:24.861601 squirrel_core-0.19.2/squirrel/zarr/sync.py
--rw-r--r--   0        0        0     8032 1970-01-01 00:00:00.000000 squirrel_core-0.19.2/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-07-21 14:00:48.501347 squirrel_core-0.19.2.dev863/LICENSE
+-rw-r--r--   0        0        0     5424 2023-07-21 14:00:48.501347 squirrel_core-0.19.2.dev863/README.md
+-rw-r--r--   0        0        0     3006 2023-07-21 14:06:11.503828 squirrel_core-0.19.2.dev863/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/__init__.py
+-rw-r--r--   0        0        0     3253 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/benchmark/quantify_randomness.py
+-rw-r--r--   0        0        0      147 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/__init__.py
+-rw-r--r--   0        0        0    14080 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/catalog.py
+-rw-r--r--   0        0        0      937 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/source.py
+-rw-r--r--   0        0        0     2208 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/catalog/yaml.py
+-rw-r--r--   0        0        0      581 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/constants.py
+-rw-r--r--   0        0        0      887 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/csv.py
+-rw-r--r--   0        0        0     4511 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/data_frame.py
+-rw-r--r--   0        0        0     8479 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/driver.py
+-rw-r--r--   0        0        0      977 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/excel.py
+-rw-r--r--   0        0        0     1045 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/feather.py
+-rw-r--r--   0        0        0     2127 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/file.py
+-rw-r--r--   0        0        0     2192 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/jsonl.py
+-rw-r--r--   0        0        0     1099 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/msgpack.py
+-rw-r--r--   0        0        0     1203 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/parquet.py
+-rw-r--r--   0        0        0     5113 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/source_combiner.py
+-rw-r--r--   0        0        0     4586 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/store.py
+-rw-r--r--   0        0        0     3230 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/driver/zarr.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/exceptions.py
+-rw-r--r--   0        0        0     2234 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/io.py
+-rw-r--r--   0        0        0       30 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/__init__.py
+-rw-r--r--   0        0        0      788 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookimpl.py
+-rw-r--r--   0        0        0      644 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookspec.py
+-rw-r--r--   0        0        0     1566 2023-07-21 14:00:48.513348 squirrel_core-0.19.2.dev863/squirrel/framework/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      410 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/__init__.py
+-rw-r--r--   0        0        0     1313 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/custom_gcsfs.py
+-rw-r--r--   0        0        0     2211 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/fsspec/fs.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/__init__.py
+-rw-r--r--   0        0        0      466 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/conftest.py
+-rw-r--r--   0        0        0     1747 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/helpers.py
+-rw-r--r--   0        0        0     3837 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/shared_fixtures.py
+-rw-r--r--   0        0        0     5841 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
+-rw-r--r--   0        0        0      471 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/__init__.py
+-rw-r--r--   0        0        0    23773 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/base.py
+-rw-r--r--   0        0        0     9230 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/iterators.py
+-rw-r--r--   0        0        0     2289 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/metrics.py
+-rw-r--r--   0        0        0     5999 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/source.py
+-rw-r--r--   0        0        0     5202 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/iterstream/torch_composables.py
+-rw-r--r--   0        0        0      224 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/py.typed
+-rw-r--r--   0        0        0      263 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/__init__.py
+-rw-r--r--   0        0        0     4805 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/jsonl.py
+-rw-r--r--   0        0        0     3471 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/msgpack.py
+-rw-r--r--   0        0        0      750 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/serialization/serializer.py
+-rw-r--r--   0        0        0      222 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/__init__.py
+-rw-r--r--   0        0        0     4588 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/filesystem.py
+-rw-r--r--   0        0        0     4864 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/squirrel_store.py
+-rw-r--r--   0        0        0     1880 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/store/store.py
+-rw-r--r--   0        0        0      110 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/__init__.py
+-rw-r--r--   0        0        0     6137 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/group.py
+-rw-r--r--   0        0        0     2041 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/key.py
+-rw-r--r--   0        0        0     3794 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/store.py
+-rw-r--r--   0        0        0      832 2023-07-21 14:00:48.517348 squirrel_core-0.19.2.dev863/squirrel/zarr/sync.py
+-rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 squirrel_core-0.19.2.dev863/PKG-INFO
```

### Comparing `squirrel_core-0.19.2/LICENSE` & `squirrel_core-0.19.2.dev863/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/README.md` & `squirrel_core-0.19.2.dev863/README.md`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/pyproject.toml` & `squirrel_core-0.19.2.dev863/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squirrel-core"
-version = "0.19.2"
+version = "0.19.2-dev863"
 description = "Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way."
 authors = ["Merantix Momentum"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "squirrel"}]
 homepage = "https://merantix-momentum.com/technology/squirrel/"
 repository = "https://github.com/merantix-momentum/squirrel-core"
```

### Comparing `squirrel_core-0.19.2/squirrel/benchmark/quantify_randomness.py` & `squirrel_core-0.19.2.dev863/squirrel/benchmark/quantify_randomness.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/catalog/catalog.py` & `squirrel_core-0.19.2.dev863/squirrel/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/catalog/source.py` & `squirrel_core-0.19.2.dev863/squirrel/catalog/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/catalog/yaml.py` & `squirrel_core-0.19.2.dev863/squirrel/catalog/yaml.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/constants.py` & `squirrel_core-0.19.2.dev863/squirrel/constants.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/__init__.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/csv.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/csv.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/data_frame.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/data_frame.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/driver.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/excel.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/excel.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/feather.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/feather.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/file.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/file.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/jsonl.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/msgpack.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/parquet.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/parquet.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/source_combiner.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/source_combiner.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/store.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/driver/zarr.py` & `squirrel_core-0.19.2.dev863/squirrel/driver/zarr.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/framework/io.py` & `squirrel_core-0.19.2.dev863/squirrel/framework/io.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/framework/plugins/hookimpl.py` & `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookimpl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/framework/plugins/hookspec.py` & `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/hookspec.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/framework/plugins/plugin_manager.py` & `squirrel_core-0.19.2.dev863/squirrel/framework/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/fsspec/custom_gcsfs.py` & `squirrel_core-0.19.2.dev863/squirrel/fsspec/custom_gcsfs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/fsspec/fs.py` & `squirrel_core-0.19.2.dev863/squirrel/fsspec/fs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/integration_test/helpers.py` & `squirrel_core-0.19.2.dev863/squirrel/integration_test/helpers.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/integration_test/shared_fixtures.py` & `squirrel_core-0.19.2.dev863/squirrel/integration_test/shared_fixtures.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py` & `squirrel_core-0.19.2.dev863/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/iterstream/base.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/base.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/iterstream/iterators.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/iterators.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/iterstream/metrics.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/metrics.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/iterstream/source.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/iterstream/torch_composables.py` & `squirrel_core-0.19.2.dev863/squirrel/iterstream/torch_composables.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/serialization/jsonl.py` & `squirrel_core-0.19.2.dev863/squirrel/serialization/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/serialization/msgpack.py` & `squirrel_core-0.19.2.dev863/squirrel/serialization/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/serialization/serializer.py` & `squirrel_core-0.19.2.dev863/squirrel/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/store/filesystem.py` & `squirrel_core-0.19.2.dev863/squirrel/store/filesystem.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/store/squirrel_store.py` & `squirrel_core-0.19.2.dev863/squirrel/store/squirrel_store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/store/store.py` & `squirrel_core-0.19.2.dev863/squirrel/store/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/zarr/group.py` & `squirrel_core-0.19.2.dev863/squirrel/zarr/group.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/zarr/key.py` & `squirrel_core-0.19.2.dev863/squirrel/zarr/key.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/zarr/store.py` & `squirrel_core-0.19.2.dev863/squirrel/zarr/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/squirrel/zarr/sync.py` & `squirrel_core-0.19.2.dev863/squirrel/zarr/sync.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.2/PKG-INFO` & `squirrel_core-0.19.2.dev863/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squirrel-core
-Version: 0.19.2
+Version: 0.19.2.dev863
 Summary: Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way.
 Home-page: https://merantix-momentum.com/technology/squirrel/
 License: Apache 2.0
 Author: Merantix Momentum
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

