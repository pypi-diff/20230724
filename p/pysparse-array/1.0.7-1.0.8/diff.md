# Comparing `tmp/pysparse-array-1.0.7.tar.gz` & `tmp/pysparse-array-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-1.0.7.tar", last modified: Tue May 23 16:53:52 2023, max compression
+gzip compressed data, was "pysparse-array-1.0.8.tar", last modified: Mon Jul 24 15:52:28 2023, max compression
```

## Comparing `pysparse-array-1.0.7.tar` & `pysparse-array-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 16:53:52.310155 pysparse-array-1.0.7/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     3228 2023-05-23 16:52:28.000000 pysparse-array-1.0.7/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.7/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.7/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-23 16:53:52.302293 pysparse-array-1.0.7/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.7/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-23 16:52:42.000000 pysparse-array-1.0.7/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 16:53:52.262639 pysparse-array-1.0.7/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-23 16:53:52.000000 pysparse-array-1.0.7/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-23 16:53:52.310404 pysparse-array-1.0.7/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-23 16:52:47.000000 pysparse-array-1.0.7/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-23 16:53:52.299824 pysparse-array-1.0.7/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.7/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     8949 2023-05-23 16:51:47.000000 pysparse-array-1.0.7/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     7531 2023-05-23 14:25:40.000000 pysparse-array-1.0.7/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-07-24 15:52:28.193488 pysparse-array-1.0.8/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     3320 2023-07-24 15:48:49.000000 pysparse-array-1.0.8/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.8/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.8/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-07-24 15:52:28.186073 pysparse-array-1.0.8/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     4694 2023-05-20 21:17:03.000000 pysparse-array-1.0.8/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-07-24 15:48:56.000000 pysparse-array-1.0.8/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-07-24 15:52:28.165466 pysparse-array-1.0.8/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5399 2023-07-24 15:52:28.000000 pysparse-array-1.0.8/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-07-24 15:52:28.000000 pysparse-array-1.0.8/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-07-24 15:52:28.000000 pysparse-array-1.0.8/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-07-24 15:52:28.000000 pysparse-array-1.0.8/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-07-24 15:52:28.000000 pysparse-array-1.0.8/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-07-24 15:52:28.194117 pysparse-array-1.0.8/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-07-24 15:49:10.000000 pysparse-array-1.0.8/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-07-24 15:52:28.181945 pysparse-array-1.0.8/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.8/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     8949 2023-05-23 16:51:47.000000 pysparse-array-1.0.8/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     7595 2023-07-24 15:48:02.000000 pysparse-array-1.0.8/sparse/core.py
```

### Comparing `pysparse-array-1.0.7/HISTORY.md` & `pysparse-array-1.0.8/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 #Changelog
 
 All notable changes to the `PySparse` package will be documented in this file.
 
 ## [Unreleased]
 
+## [1.0.8] - 2023-07-24
+
+### Fixed
+- Fixed problem with small arrays with large chunksizes
+
 ## [1.0.7] - 2023-05-23
 
 ### Fixed
 - Fixed ongoing multi-index issues
 
 ## [1.0.6] - 2023-05-23
```

### Comparing `pysparse-array-1.0.7/LICENSE.txt` & `pysparse-array-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.7/PKG-INFO` & `pysparse-array-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.7/README.md` & `pysparse-array-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.7/pyproject.toml` & `pysparse-array-1.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
```

### Comparing `pysparse-array-1.0.7/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-1.0.8/pysparse_array.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.7/setup.py` & `pysparse-array-1.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='1.0.7',
+    version='1.0.8',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-1.0.7/sparse/array_api.py` & `pysparse-array-1.0.8/sparse/array_api.py`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.7/sparse/core.py` & `pysparse-array-1.0.8/sparse/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,16 @@
     :return:
     """
 
     # Identify the relevant shapes of the dense and sparse arrays
     dense_shape = array.shape
     dense_dtype = array.dtype
     announce_progress('Identifying sparse shape...') if verbose else None
+    if chunksize < dense_shape:
+        chunksize = dense_shape
     nonzero_shape = __calc_sparse_shape(array, chunksize, verbose)
 
     # Create the sparse array binaries (memory-mapped)
     memmap_sparse_data = open_memmap(os.path.join(path, 'sparse_data.npy'),
                                      dtype=dense_dtype,
                                      mode='w+',
                                      shape=(nonzero_shape,))
```

