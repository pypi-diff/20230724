# Comparing `tmp/Connectome-Utilities-0.3.2.tar.gz` & `tmp/Connectome-Utilities-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Connectome-Utilities-0.3.2.tar", last modified: Sun Jul 23 15:55:47 2023, max compression
+gzip compressed data, was "Connectome-Utilities-0.4.0.tar", last modified: Mon Jul 24 11:04:58 2023, max compression
```

## Comparing `Connectome-Utilities-0.3.2.tar` & `Connectome-Utilities-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:47.775704 Connectome-Utilities-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/AUTHORS.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:47.771704 Connectome-Utilities-0.3.2/Connectome_Utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-07-23 15:55:47.000000 Connectome-Utilities-0.3.2/Connectome_Utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-23 15:55:47.000000 Connectome-Utilities-0.3.2/Connectome_Utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 15:55:47.000000 Connectome-Utilities-0.3.2/Connectome_Utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-23 15:55:47.000000 Connectome-Utilities-0.3.2/Connectome_Utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-23 15:55:47.000000 Connectome-Utilities-0.3.2/Connectome_Utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-07-23 15:55:47.771704 Connectome-Utilities-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:47.771704 Connectome-Utilities-0.3.2/conntility/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/conntility/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    83760 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/conntility/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/conntility/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/conntility/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 15:55:47.775704 Connectome-Utilities-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:47.771704 Connectome-Utilities-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/tests/test_analysis_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/tests/test_connectivity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-23 15:55:39.000000 Connectome-Utilities-0.3.2/tests/test_neuron_groups.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:03.405825 Connectome-Utilities-0.4.0/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)       77 2023-06-07 08:34:43.000000 Connectome-Utilities-0.4.0/AUTHORS.txt
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:00.691327 Connectome-Utilities-0.4.0/Connectome_Utilities.egg-info/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    19962 2023-07-24 11:05:59.000000 Connectome-Utilities-0.4.0/Connectome_Utilities.egg-info/PKG-INFO
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     2018 2023-07-24 11:06:00.000000 Connectome-Utilities-0.4.0/Connectome_Utilities.egg-info/SOURCES.txt
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)        1 2023-07-24 11:05:59.000000 Connectome-Utilities-0.4.0/Connectome_Utilities.egg-info/dependency_links.txt
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      145 2023-07-24 11:05:59.000000 Connectome-Utilities-0.4.0/Connectome_Utilities.egg-info/requires.txt
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)       11 2023-07-24 11:05:59.000000 Connectome-Utilities-0.4.0/Connectome_Utilities.egg-info/top_level.txt
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    11353 2023-06-07 11:54:58.000000 Connectome-Utilities-0.4.0/LICENSE
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    19962 2023-07-24 11:06:03.401364 Connectome-Utilities-0.4.0/PKG-INFO
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    19296 2023-06-30 11:34:22.000000 Connectome-Utilities-0.4.0/README.md
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:01.020216 Connectome-Utilities-0.4.0/conntility/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      259 2023-06-07 08:13:49.000000 Connectome-Utilities-0.4.0/conntility/__init__.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:01.278966 Connectome-Utilities-0.4.0/conntility/analysis/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      181 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/analysis/__init__.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     6514 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/analysis/analysis.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    11611 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/analysis/analysis_decorators.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     2305 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/analysis/clustering.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:01.423471 Connectome-Utilities-0.4.0/conntility/analysis/library/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)       83 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/analysis/library/__init__.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     3238 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/analysis/library/diffusion_mapping.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:01.696152 Connectome-Utilities-0.4.0/conntility/circuit_models/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      573 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/__init__.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    29686 2023-07-23 15:50:44.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/connection_matrix.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     4213 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/input_spikes.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:02.420611 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      495 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/__init__.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      402 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/defaults.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     5054 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/extra_properties.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     2269 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/from_atlas.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     5683 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/grouping_config.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     6223 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/loader.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     9112 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/make_groups.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     1967 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/sonata_extensions.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    17520 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/neuron_groups/tessellate.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     3441 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/circuit_models/sonata_helpers.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    83760 2023-07-23 15:50:44.000000 Connectome-Utilities-0.4.0/conntility/connectivity.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:02.759683 Connectome-Utilities-0.4.0/conntility/flatmapping/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      363 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/flatmapping/__init__.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     4917 2023-06-13 09:42:59.000000 Connectome-Utilities-0.4.0/conntility/flatmapping/_supersample_utility.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     4850 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/flatmapping/flatmap_utility.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     9522 2023-06-12 16:33:16.000000 Connectome-Utilities-0.4.0/conntility/flatmapping/supersampling.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     3387 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/flatmapping/wm_recipe_utility.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:02.970943 Connectome-Utilities-0.4.0/conntility/io/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      113 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/io/__init__.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     1519 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/io/logging.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     3026 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/io/sparse_matrices.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    10990 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/multi_scale.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     2743 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/plugins.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:03.038602 Connectome-Utilities-0.4.0/conntility/randomization/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)       38 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/randomization/__init__.py
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:03.160635 Connectome-Utilities-0.4.0/conntility/subcellular/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      116 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/conntility/subcellular/__init__.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)    16841 2023-07-07 09:22:34.000000 Connectome-Utilities-0.4.0/conntility/subcellular/neuron_morphology_path_distance.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     1106 2023-07-23 15:51:23.000000 Connectome-Utilities-0.4.0/pyproject.toml
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)       38 2023-07-24 11:06:03.407828 Connectome-Utilities-0.4.0/setup.cfg
+drwxrwxrwx   0 reimann   (1000) reimann   (1000)        0 2023-07-24 11:06:03.366721 Connectome-Utilities-0.4.0/tests/
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)      568 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/tests/test_analysis.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     3203 2023-06-07 08:15:28.000000 Connectome-Utilities-0.4.0/tests/test_analysis_decorator.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     7250 2023-06-09 14:26:32.000000 Connectome-Utilities-0.4.0/tests/test_connectivity_matrix.py
+-rwxrwxrwx   0 reimann   (1000) reimann   (1000)     1348 2023-06-09 14:55:41.000000 Connectome-Utilities-0.4.0/tests/test_neuron_groups.py
```

### Comparing `Connectome-Utilities-0.3.2/Connectome_Utilities.egg-info/PKG-INFO` & `Connectome-Utilities-0.4.0/Connectome_Utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Connectome-Utilities
-Version: 0.3.2
+Version: 0.4.0
 Summary: Complex network representation and analysis layer
 Author-email: "Blue Brain Project, EPFL" <conntility.645co@simplelogin.com>
 Project-URL: Homepage, https://github.com/BlueBrain/ConnectomeUtilities
 Project-URL: Bug Tracker, https://github.com/BlueBrain/ConnectomeUtilities/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Connectome-Utilities-0.3.2/LICENSE` & `Connectome-Utilities-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.3.2/PKG-INFO` & `Connectome-Utilities-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Connectome-Utilities
-Version: 0.3.2
+Version: 0.4.0
 Summary: Complex network representation and analysis layer
 Author-email: "Blue Brain Project, EPFL" <conntility.645co@simplelogin.com>
 Project-URL: Homepage, https://github.com/BlueBrain/ConnectomeUtilities
 Project-URL: Bug Tracker, https://github.com/BlueBrain/ConnectomeUtilities/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Connectome-Utilities-0.3.2/README.md` & `Connectome-Utilities-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.3.2/conntility/connectivity.py` & `Connectome-Utilities-0.4.0/conntility/connectivity.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.3.2/conntility/multi_scale.py` & `Connectome-Utilities-0.4.0/conntility/multi_scale.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.3.2/conntility/plugins.py` & `Connectome-Utilities-0.4.0/conntility/plugins.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.3.2/pyproject.toml` & `Connectome-Utilities-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Connectome-Utilities"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   { name="Blue Brain Project, EPFL", email="conntility.645co@simplelogin.com" },
 ]
 description = "Complex network representation and analysis layer"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -30,8 +30,8 @@
                 "voxcell"]
 
 [project.urls]
 "Homepage" = "https://github.com/BlueBrain/ConnectomeUtilities"
 "Bug Tracker" = "https://github.com/BlueBrain/ConnectomeUtilities/issues"
 
 [tool.setuptools]
-packages = ["conntility"]
+packages = ["conntility"]
```

### Comparing `Connectome-Utilities-0.3.2/tests/test_analysis.py` & `Connectome-Utilities-0.4.0/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.3.2/tests/test_analysis_decorator.py` & `Connectome-Utilities-0.4.0/tests/test_analysis_decorator.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.3.2/tests/test_connectivity_matrix.py` & `Connectome-Utilities-0.4.0/tests/test_connectivity_matrix.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.3.2/tests/test_neuron_groups.py` & `Connectome-Utilities-0.4.0/tests/test_neuron_groups.py`

 * *Files identical despite different names*

