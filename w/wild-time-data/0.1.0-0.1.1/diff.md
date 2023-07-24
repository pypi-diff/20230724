# Comparing `tmp/wild_time_data-0.1.0.tar.gz` & `tmp/wild_time_data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_time_data-0.1.0.tar", last modified: Tue May  9 16:39:22 2023, max compression
+gzip compressed data, was "wild_time_data-0.1.1.tar", last modified: Mon Jul 24 09:46:48 2023, max compression
```

## Comparing `wild_time_data-0.1.0.tar` & `wild_time_data-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.054627 wild_time_data-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.046626 wild_time_data-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.050626 wild_time_data-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-09 16:39:22.054627 wild_time_data-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.050626 wild_time_data-0.1.0/converter/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/converter/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/converter/fmow.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/converter/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:39:22.054627 wild_time_data-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.050626 wild_time_data-0.1.0/wild_time_data/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/wild_time_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/wild_time_data/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/wild_time_data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/wild_time_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:39:22.054627 wild_time_data-0.1.0/wild_time_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 16:39:22.000000 wild_time_data-0.1.0/wild_time_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   255896 2023-05-09 16:39:11.000000 wild_time_data-0.1.0/yearbook.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:46:48.046292 wild_time_data-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:46:48.042292 wild_time_data-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:46:48.042292 wild_time_data-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-24 09:46:48.046292 wild_time_data-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:46:48.042292 wild_time_data-0.1.1/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/converter/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/converter/fmow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/converter/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:46:48.046292 wild_time_data-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:46:48.046292 wild_time_data-0.1.1/wild_time_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/wild_time_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/wild_time_data/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/wild_time_data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/wild_time_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:46:48.046292 wild_time_data-0.1.1/wild_time_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-24 09:46:48.000000 wild_time_data-0.1.1/wild_time_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 09:46:48.000000 wild_time_data-0.1.1/wild_time_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:46:48.000000 wild_time_data-0.1.1/wild_time_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 09:46:48.000000 wild_time_data-0.1.1/wild_time_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 09:46:48.000000 wild_time_data-0.1.1/wild_time_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   255896 2023-07-24 09:46:38.000000 wild_time_data-0.1.1/yearbook.png
```

### Comparing `wild_time_data-0.1.0/.github/workflows/pypi_publish.yml` & `wild_time_data-0.1.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/.gitignore` & `wild_time_data-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/LICENSE` & `wild_time_data-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/PKG-INFO` & `wild_time_data-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: wild_time_data
-Version: 0.1.0
+Version: 0.1.1
 Summary: WILDS distribution shift data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <=3.10,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Wild-Time-Data: Easy access to the Wild-Time data
 *************************************************
 
 This repository provides a simpler interface to access the
```

### Comparing `wild_time_data-0.1.0/README.rst` & `wild_time_data-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/converter/README.rst` & `wild_time_data-0.1.1/converter/README.rst`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/converter/fmow.py` & `wild_time_data-0.1.1/converter/fmow.py`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/pyproject.toml` & `wild_time_data-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
 ]
-requires-python = ">=3.8, <=3.10"
+requires-python = ">=3.8"
 dynamic = ["version", "readme", "dependencies"]
 
 [tool.setuptools]
 packages = ["wild_time_data"]
 
 [tool.setuptools.dynamic]
 version = {attr = "wild_time_data.__version__"}
```

### Comparing `wild_time_data-0.1.0/wild_time_data/core.py` & `wild_time_data-0.1.1/wild_time_data/core.py`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/wild_time_data/datasets.py` & `wild_time_data-0.1.1/wild_time_data/datasets.py`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/wild_time_data/utils.py` & `wild_time_data-0.1.1/wild_time_data/utils.py`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.1.0/wild_time_data.egg-info/PKG-INFO` & `wild_time_data-0.1.1/wild_time_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: wild-time-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: WILDS distribution shift data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <=3.10,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Wild-Time-Data: Easy access to the Wild-Time data
 *************************************************
 
 This repository provides a simpler interface to access the
```

### Comparing `wild_time_data-0.1.0/yearbook.png` & `wild_time_data-0.1.1/yearbook.png`

 * *Files identical despite different names*

