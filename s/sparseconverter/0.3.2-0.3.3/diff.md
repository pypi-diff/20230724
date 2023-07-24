# Comparing `tmp/sparseconverter-0.3.2.tar.gz` & `tmp/sparseconverter-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparseconverter-0.3.2.tar", last modified: Wed Jul 12 07:45:45 2023, max compression
+gzip compressed data, was "sparseconverter-0.3.3.tar", last modified: Mon Jul 24 12:44:21 2023, max compression
```

## Comparing `sparseconverter-0.3.2.tar` & `sparseconverter-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.129136 sparseconverter-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/src/sparseconverter/
--rw-r--r--   0 runner    (1001) docker     (123)    50194 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/src/sparseconverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/src/sparseconverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 07:45:45.000000 sparseconverter-0.3.2/src/sparseconverter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:45:45.133136 sparseconverter-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-07-12 07:45:32.000000 sparseconverter-0.3.2/tests/test_sparseconverters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:44:21.514695 sparseconverter-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-24 12:43:51.000000 sparseconverter-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-24 12:44:21.514695 sparseconverter-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-24 12:43:51.000000 sparseconverter-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-24 12:43:51.000000 sparseconverter-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-24 12:44:21.514695 sparseconverter-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:44:21.514695 sparseconverter-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:44:21.514695 sparseconverter-0.3.3/src/sparseconverter/
+-rw-r--r--   0 runner    (1001) docker     (123)    50552 2023-07-24 12:43:51.000000 sparseconverter-0.3.3/src/sparseconverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:44:21.514695 sparseconverter-0.3.3/src/sparseconverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-24 12:44:21.000000 sparseconverter-0.3.3/src/sparseconverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-24 12:44:21.000000 sparseconverter-0.3.3/src/sparseconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:44:21.000000 sparseconverter-0.3.3/src/sparseconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 12:44:21.000000 sparseconverter-0.3.3/src/sparseconverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 12:44:21.000000 sparseconverter-0.3.3/src/sparseconverter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:44:21.514695 sparseconverter-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-07-24 12:43:51.000000 sparseconverter-0.3.3/tests/test_sparseconverters.py
```

### Comparing `sparseconverter-0.3.2/LICENSE` & `sparseconverter-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparseconverter-0.3.2/PKG-INFO` & `sparseconverter-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseconverter
-Version: 0.3.2
+Version: 0.3.3
 Summary: Converter matrix and type determination for a range of array formats, focusing on sparse arrays
 Author-email: Dieter Weber <d.weber@fz-juelich.de>
 License: MIT License
         
         Copyright (c) 2022 LiberTEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,14 +28,15 @@
 Project-URL: repository, https://github.com/LiberTEM/sparseconverter
 Keywords: numpy,scipy.sparse,sparse,array,matrix,cupy,cupyx.scipy.sparse
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: cupy
 Provides-Extra: test
 License-File: LICENSE
 
@@ -113,14 +114,18 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.3
+
+* Perform feature checks lazily https://github.com/LiberTEM/sparseconverter/issues/15
+
 ### 0.3.2
 
 * Detection and workaround for https://github.com/pydata/sparse/issues/602.
 * Detection and workaround for https://github.com/cupy/cupy/issues/7713.
 * Test with duplicates and scrambled indices.
 * Test correctness of basic array operations.
```

### Comparing `sparseconverter-0.3.2/README.md` & `sparseconverter-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.3
+
+* Perform feature checks lazily https://github.com/LiberTEM/sparseconverter/issues/15
+
 ### 0.3.2
 
 * Detection and workaround for https://github.com/pydata/sparse/issues/602.
 * Detection and workaround for https://github.com/cupy/cupy/issues/7713.
 * Test with duplicates and scrambled indices.
 * Test correctness of basic array operations.
```

### Comparing `sparseconverter-0.3.2/pyproject.toml` & `sparseconverter-0.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Development Status :: 3 - Alpha",
 ]
 authors = [
     {name="Dieter Weber", email="d.weber@fz-juelich.de"},
 ]
 
 [project.urls]
```

### Comparing `sparseconverter-0.3.2/src/sparseconverter/__init__.py` & `sparseconverter-0.3.3/src/sparseconverter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing_extensions import Literal
 
 import numpy as np
 import scipy.sparse as sp
 import sparse
 
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 
 NUMPY = 'numpy'
 NUMPY_MATRIX = 'numpy.matrix'
 CUDA = 'cuda'
 CUPY = 'cupy'
 SPARSE_COO = 'sparse.COO'
 SPARSE_GCXS = 'sparse.GCXS'
@@ -147,14 +147,15 @@
 
 # Exceptions for the above matrix
 _special_mappings = {
     (CUPY_SCIPY_CSR, np.dtype(bool)): bool,
 }
 
 
+@lru_cache(maxsize=None)
 def _test_GCXS_supports_non_canonical():
     # Checks for https://github.com/pydata/sparse/issues/602
     data = np.array((2., 1., 3., 3., 1.))
     indices = np.array((1, 0, 0, 1, 1), dtype=int)
     indptr = np.array((0, 2, 5), dtype=int)
     ref = np.array(((1., 2.), (3., 4.)))
 
@@ -178,15 +179,28 @@
     # Maybe a first "bandaid" for GCXS is throwing an error? In that case we canonicalize
     # the same way as if the bug was present.
     except Exception:
         raise  # FIXME remove
         return False
 
 
-_GCXS_supports_non_canonical = _test_GCXS_supports_non_canonical()
+def _convert_csc_csr_to_pydata_sparse(left, right):
+    """
+    Build conversion function from CSR/CSC (left) to COO/GCXS/DOK
+    (right) which lazily feature-checks for non-canonical support.
+    """
+    def _do_convert(arr):
+        if _test_GCXS_supports_non_canonical():
+            return _classes[right].from_scipy_sparse(arr)
+        else:
+            return chain(
+                _ensure_sorted_dedup,
+                _classes[right].from_scipy_sparse,
+            )(arr)
+    return _do_convert
 
 
 def result_type(*args) -> np.dtype:
     '''
     Find a dtype that fulfills the following properties:
 
     * Can contain :code:`numpy.result_type(...)` of all items in :code:`args`
@@ -303,15 +317,18 @@
     converter function.
 
     The elements that require CuPy support are added dynamically by
     :meth:`_populate_cupy` when any CUDA-based types are requested. That way it
     works also without CuPy.
     '''
     def __init__(self):
+        self._built = False
         self._converters = {}
+
+    def _build_converters(self):
         try:
             for backend in BACKENDS:
                 self._converters[(backend, backend)] = _identity
             # Both are NumPy arrays, distinguished for device selection
             for left in (NUMPY, CUDA):
                 for right in (NUMPY, CUDA):
                     self._converters[(left, right)] = _identity
@@ -343,20 +360,15 @@
             for left in SCIPY_COO, SCIPY_CSR, SCIPY_CSC:
                 for right in NUMPY, CUDA:
                     if (left, right) not in self._converters:
                         self._converters[(left, right)] = _classes[left].toarray
             for left in SCIPY_CSR, SCIPY_CSC:
                 for right in SPARSE_COO, SPARSE_GCXS, SPARSE_DOK:
                     if (left, right) not in self._converters:
-                        if _GCXS_supports_non_canonical:
-                            self._converters[(left, right)] = _classes[right].from_scipy_sparse
-                        else:
-                            self._converters[(left, right)] = chain(
-                                _ensure_sorted_dedup, _classes[right].from_scipy_sparse
-                            )
+                        self._converters[(left, right)] = _convert_csc_csr_to_pydata_sparse(left, right)
             for left in SCIPY_COO, :
                 for right in SPARSE_COO, SPARSE_GCXS, SPARSE_DOK:
                     if (left, right) not in self._converters:
                         self._converters[(left, right)] = _classes[right].from_scipy_sparse
 
             self._converters[(SPARSE_COO, SCIPY_COO)] = chain(_flatsig, sparse.COO.to_scipy_sparse)
             self._converters[(SPARSE_COO, SCIPY_CSR)] = chain(_flatsig, sparse.COO.tocsr)
@@ -385,14 +397,15 @@
                 if (left, right) not in self._converters:
                     c1 = self._converters[(left, proxy)]
                     c2 = self._converters[(proxy, right)]
                     self._converters[(left, right)] = chain(c1, c2)
         except Exception:
             self._converters = None
             raise
+        self._built = True
 
     def _populate_cupy(self):
         import cupy
         import cupyx.scipy
 
         def detect_csr_complex128_bug():
             # https://github.com/cupy/cupy/issues/7035
@@ -542,15 +555,15 @@
             '''
             Use GPU for sparsification if dtype allows, otherwise CPU
             '''
             if arr.dtype in CUPY_SPARSE_CSR_DTYPES:
                 reshaped = arr.reshape((arr.shape[0], -1))
                 intermediate = cupyx.scipy.sparse.csr_matrix(reshaped)
                 intermediate = intermediate.get()
-                if not _GCXS_supports_non_canonical:
+                if not _test_GCXS_supports_non_canonical():
                     intermediate.sort_indices()
                     intermediate.sum_duplicates()
                 return sparse.GCXS(intermediate).reshape(arr.shape)
             else:
                 intermediate = cupy.asnumpy(arr)
                 return sparse.GCXS.from_numpy(intermediate)
 
@@ -855,14 +868,16 @@
             for right in BACKENDS:
                 if (left, right) not in self._converters:
                     raise RuntimeError(f'Missing converter {left} -> {right}')
 
     def __getitem__(self, item):
         if self._converters is None:
             raise RuntimeError('Building the converter matrix has failed previously, aborting.')
+        if not self._built:
+            self._build_converters()
         res = self._converters.get(item, False)
         if res is False:
             left, right = item
             if left in CUDA_BACKENDS or right in CUDA_BACKENDS:
                 self._populate_cupy()
             return self._converters[item]
         else:
```

### Comparing `sparseconverter-0.3.2/src/sparseconverter.egg-info/PKG-INFO` & `sparseconverter-0.3.3/src/sparseconverter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseconverter
-Version: 0.3.2
+Version: 0.3.3
 Summary: Converter matrix and type determination for a range of array formats, focusing on sparse arrays
 Author-email: Dieter Weber <d.weber@fz-juelich.de>
 License: MIT License
         
         Copyright (c) 2022 LiberTEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,14 +28,15 @@
 Project-URL: repository, https://github.com/LiberTEM/sparseconverter
 Keywords: numpy,scipy.sparse,sparse,array,matrix,cupy,cupyx.scipy.sparse
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: cupy
 Provides-Extra: test
 License-File: LICENSE
 
@@ -113,14 +114,18 @@
 
 * PyTorch arrays
 * SciPy sparse arrays as opposed to SciPy sparse matrices.
 * More detailed cost metric based on more real-world use cases and parameters.
 
 ## Changelog
 
+### 0.3.3
+
+* Perform feature checks lazily https://github.com/LiberTEM/sparseconverter/issues/15
+
 ### 0.3.2
 
 * Detection and workaround for https://github.com/pydata/sparse/issues/602.
 * Detection and workaround for https://github.com/cupy/cupy/issues/7713.
 * Test with duplicates and scrambled indices.
 * Test correctness of basic array operations.
```

### Comparing `sparseconverter-0.3.2/tests/test_sparseconverters.py` & `sparseconverter-0.3.3/tests/test_sparseconverters.py`

 * *Files identical despite different names*

