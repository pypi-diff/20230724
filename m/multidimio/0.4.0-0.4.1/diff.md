# Comparing `tmp/multidimio-0.4.0.tar.gz` & `tmp/multidimio-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidimio-0.4.0.tar", max compression
+gzip compressed data, was "multidimio-0.4.1.tar", max compression
```

## Comparing `multidimio-0.4.0.tar` & `multidimio-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    10203 2023-06-26 20:41:02.942805 multidimio-0.4.0/LICENSE
--rw-r--r--   0        0        0     6043 2023-06-26 20:41:02.946805 multidimio-0.4.0/README.md
--rw-r--r--   0        0        0     2806 2023-06-26 20:41:14.826817 multidimio-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      474 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/__init__.py
--rw-r--r--   0        0        0     2697 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/__main__.py
--rw-r--r--   0        0        0      127 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/api/__init__.py
--rw-r--r--   0        0        0    24779 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/api/accessor.py
--rw-r--r--   0        0        0     2322 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/api/convenience.py
--rw-r--r--   0        0        0     4451 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/api/io_utils.py
--rw-r--r--   0        0        0      105 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/commands/__init__.py
--rw-r--r--   0        0        0    12573 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/commands/segy.py
--rw-r--r--   0        0        0      529 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/constants.py
--rw-r--r--   0        0        0      141 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/converters/__init__.py
--rw-r--r--   0        0        0      597 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/converters/exceptions.py
--rw-r--r--   0        0        0     6510 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/converters/mdio.py
--rw-r--r--   0        0        0    13393 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/converters/segy.py
--rw-r--r--   0        0        0      143 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/core/__init__.py
--rw-r--r--   0        0        0     3811 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/core/dimension.py
--rw-r--r--   0        0        0      268 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/core/exceptions.py
--rw-r--r--   0        0        0     3694 2023-06-26 20:41:02.958805 multidimio-0.4.0/src/mdio/core/grid.py
--rw-r--r--   0        0        0     2917 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/core/indexing.py
--rw-r--r--   0        0        0     2727 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/core/serialization.py
--rw-r--r--   0        0        0      429 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/core/utils_write.py
--rw-r--r--   0        0        0     1646 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/py.typed
--rw-r--r--   0        0        0       44 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/__init__.py
--rw-r--r--   0        0        0      636 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/_standards_common.py
--rw-r--r--   0        0        0     9384 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/_standards_rev0.py
--rw-r--r--   0        0        0     8270 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/_workers.py
--rw-r--r--   0        0        0    11128 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/blocked_io.py
--rw-r--r--   0        0        0     2048 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/byte_utils.py
--rw-r--r--   0        0        0     9408 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/creation.py
--rw-r--r--   0        0        0     4856 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/ebcdic.py
--rw-r--r--   0        0        0     1946 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/exceptions.py
--rw-r--r--   0        0        0    10719 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/geometry.py
--rw-r--r--   0        0        0     2748 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/headers.py
--rw-r--r--   0        0        0     3561 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/headers_text.py
--rw-r--r--   0        0        0     1120 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/helpers_segy.py
--rw-r--r--   0        0        0     5785 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/ibm_float.py
--rw-r--r--   0        0        0     4916 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/parsers.py
--rw-r--r--   0        0        0     5170 2023-06-26 20:41:02.962805 multidimio-0.4.0/src/mdio/segy/utilities.py
--rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 multidimio-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10203 2023-07-24 19:16:15.809080 multidimio-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6043 2023-07-24 19:16:15.809080 multidimio-0.4.1/README.md
+-rw-r--r--   0        0        0     2806 2023-07-24 19:16:29.829316 multidimio-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/__init__.py
+-rw-r--r--   0        0        0     2697 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/__main__.py
+-rw-r--r--   0        0        0      127 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/api/__init__.py
+-rw-r--r--   0        0        0    24779 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/api/accessor.py
+-rw-r--r--   0        0        0     2322 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/api/convenience.py
+-rw-r--r--   0        0        0     4451 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/api/io_utils.py
+-rw-r--r--   0        0        0      105 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/commands/__init__.py
+-rw-r--r--   0        0        0    12573 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/commands/segy.py
+-rw-r--r--   0        0        0      529 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/constants.py
+-rw-r--r--   0        0        0      141 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/converters/__init__.py
+-rw-r--r--   0        0        0      597 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/converters/exceptions.py
+-rw-r--r--   0        0        0     6510 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/converters/mdio.py
+-rw-r--r--   0        0        0    13393 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/converters/segy.py
+-rw-r--r--   0        0        0      143 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/__init__.py
+-rw-r--r--   0        0        0     3811 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/dimension.py
+-rw-r--r--   0        0        0      268 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/exceptions.py
+-rw-r--r--   0        0        0     3694 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/grid.py
+-rw-r--r--   0        0        0     2917 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/indexing.py
+-rw-r--r--   0        0        0     2727 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/serialization.py
+-rw-r--r--   0        0        0      429 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/utils_write.py
+-rw-r--r--   0        0        0     1646 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/py.typed
+-rw-r--r--   0        0        0       44 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/__init__.py
+-rw-r--r--   0        0        0      636 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/_standards_common.py
+-rw-r--r--   0        0        0     9384 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/_standards_rev0.py
+-rw-r--r--   0        0        0     8377 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/_workers.py
+-rw-r--r--   0        0        0    11128 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/blocked_io.py
+-rw-r--r--   0        0        0     2048 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/byte_utils.py
+-rw-r--r--   0        0        0     9408 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/creation.py
+-rw-r--r--   0        0        0     4856 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/ebcdic.py
+-rw-r--r--   0        0        0     1946 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/exceptions.py
+-rw-r--r--   0        0        0    10719 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/geometry.py
+-rw-r--r--   0        0        0     2748 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/headers.py
+-rw-r--r--   0        0        0     3561 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/headers_text.py
+-rw-r--r--   0        0        0     1120 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/helpers_segy.py
+-rw-r--r--   0        0        0     5785 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/ibm_float.py
+-rw-r--r--   0        0        0     4916 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/parsers.py
+-rw-r--r--   0        0        0     5170 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/utilities.py
+-rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 multidimio-0.4.1/PKG-INFO
```

### Comparing `multidimio-0.4.0/LICENSE` & `multidimio-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/README.md` & `multidimio-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/pyproject.toml` & `multidimio-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidimio"
-version = "0.4.0"
+version = "0.4.1"
 description = "Cloud-native, scalable, and user-friendly multi dimensional energy data!"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `multidimio-0.4.0/src/mdio/__main__.py` & `multidimio-0.4.1/src/mdio/__main__.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/api/accessor.py` & `multidimio-0.4.1/src/mdio/api/accessor.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/api/convenience.py` & `multidimio-0.4.1/src/mdio/api/convenience.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/api/io_utils.py` & `multidimio-0.4.1/src/mdio/api/io_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/commands/segy.py` & `multidimio-0.4.1/src/mdio/commands/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/constants.py` & `multidimio-0.4.1/src/mdio/constants.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/converters/exceptions.py` & `multidimio-0.4.1/src/mdio/converters/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/converters/mdio.py` & `multidimio-0.4.1/src/mdio/converters/mdio.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/converters/segy.py` & `multidimio-0.4.1/src/mdio/converters/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/core/dimension.py` & `multidimio-0.4.1/src/mdio/core/dimension.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/core/grid.py` & `multidimio-0.4.1/src/mdio/core/grid.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/core/indexing.py` & `multidimio-0.4.1/src/mdio/core/indexing.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/core/serialization.py` & `multidimio-0.4.1/src/mdio/core/serialization.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/exceptions.py` & `multidimio-0.4.1/src/mdio/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/_standards_common.py` & `multidimio-0.4.1/src/mdio/segy/_standards_common.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/_standards_rev0.py` & `multidimio-0.4.1/src/mdio/segy/_standards_rev0.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/_workers.py` & `multidimio-0.4.1/src/mdio/segy/_workers.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,18 @@
 
     # Flush metadata to zarr
     metadata_array.set_basic_selection(
         selection=chunk_indices[:-1],
         value=tmp_metadata,
     )
 
-    nonzero_z = tmp_data.sum(axis=tuple(range(n_dim - 1))).nonzero()
+    # Find first non-zero index in sample (last) dimension
+    non_sample_axes = tuple(range(n_dim - 1))
+    nonzero_z = np.where(np.any(tmp_data != 0, axis=non_sample_axes))
+
     if len(nonzero_z[0]) == 0:
         return
 
     dimn_start = np.min(nonzero_z)
     dimn_end = np.max(nonzero_z) + 1
 
     z_slice = slice(dimn_start, dimn_end)
```

### Comparing `multidimio-0.4.0/src/mdio/segy/blocked_io.py` & `multidimio-0.4.1/src/mdio/segy/blocked_io.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/byte_utils.py` & `multidimio-0.4.1/src/mdio/segy/byte_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/creation.py` & `multidimio-0.4.1/src/mdio/segy/creation.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/ebcdic.py` & `multidimio-0.4.1/src/mdio/segy/ebcdic.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/exceptions.py` & `multidimio-0.4.1/src/mdio/segy/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/geometry.py` & `multidimio-0.4.1/src/mdio/segy/geometry.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/headers.py` & `multidimio-0.4.1/src/mdio/segy/headers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/headers_text.py` & `multidimio-0.4.1/src/mdio/segy/headers_text.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/helpers_segy.py` & `multidimio-0.4.1/src/mdio/segy/helpers_segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/ibm_float.py` & `multidimio-0.4.1/src/mdio/segy/ibm_float.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/parsers.py` & `multidimio-0.4.1/src/mdio/segy/parsers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/src/mdio/segy/utilities.py` & `multidimio-0.4.1/src/mdio/segy/utilities.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.0/PKG-INFO` & `multidimio-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidimio
-Version: 0.4.0
+Version: 0.4.1
 Summary: Cloud-native, scalable, and user-friendly multi dimensional energy data!
 Home-page: https://mdio.dev
 License: Apache-2.0
 Keywords: mdio,multidimio,seismic,wind,data
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
```

