# Comparing `tmp/structuretoolkit-0.0.6.tar.gz` & `tmp/structuretoolkit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structuretoolkit-0.0.6.tar", last modified: Sat Jul 22 04:33:39 2023, max compression
+gzip compressed data, was "structuretoolkit-0.0.7.tar", last modified: Mon Jul 24 19:44:46 2023, max compression
```

## Comparing `structuretoolkit-0.0.6.tar` & `structuretoolkit-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:33:39.267835 structuretoolkit-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-22 04:33:39.267835 structuretoolkit-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-22 04:33:39.267835 structuretoolkit-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-22 04:33:38.000000 structuretoolkit-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:33:39.267835 structuretoolkit-0.0.6/structuretoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-22 04:33:39.267835 structuretoolkit-0.0.6/structuretoolkit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:33:39.263835 structuretoolkit-0.0.6/structuretoolkit/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/analyse/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    47409 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/analyse/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/analyse/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/analyse/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/analyse/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/analyse/strain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/analyse/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:33:39.263835 structuretoolkit-0.0.6/structuretoolkit/build/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/build/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/build/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/build/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/build/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/build/surface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:33:39.263835 structuretoolkit-0.0.6/structuretoolkit/common/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/common/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/common/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/common/pymatgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/common/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    30764 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/structuretoolkit/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:33:39.263835 structuretoolkit-0.0.6/structuretoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-22 04:33:39.000000 structuretoolkit-0.0.6/structuretoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-22 04:33:39.000000 structuretoolkit-0.0.6/structuretoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 04:33:39.000000 structuretoolkit-0.0.6/structuretoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-22 04:33:39.000000 structuretoolkit-0.0.6/structuretoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 04:33:39.000000 structuretoolkit-0.0.6/structuretoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:33:39.267835 structuretoolkit-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_high_index_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_pyxtal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/tests/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-22 04:33:33.000000 structuretoolkit-0.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:44:46.776481 structuretoolkit-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 19:44:46.776481 structuretoolkit-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-24 19:44:46.776481 structuretoolkit-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-24 19:44:46.000000 structuretoolkit-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:44:46.776481 structuretoolkit-0.0.7/structuretoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 19:44:46.776481 structuretoolkit-0.0.7/structuretoolkit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:44:46.772481 structuretoolkit-0.0.7/structuretoolkit/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/analyse/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47409 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/analyse/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/analyse/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/analyse/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/analyse/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/analyse/strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/analyse/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:44:46.772481 structuretoolkit-0.0.7/structuretoolkit/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/build/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/build/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/build/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/build/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/build/surface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:44:46.776481 structuretoolkit-0.0.7/structuretoolkit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/common/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/common/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/common/pymatgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/common/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30764 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/structuretoolkit/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:44:46.772481 structuretoolkit-0.0.7/structuretoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 19:44:46.000000 structuretoolkit-0.0.7/structuretoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-24 19:44:46.000000 structuretoolkit-0.0.7/structuretoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:44:46.000000 structuretoolkit-0.0.7/structuretoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 19:44:46.000000 structuretoolkit-0.0.7/structuretoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 19:44:46.000000 structuretoolkit-0.0.7/structuretoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:44:46.776481 structuretoolkit-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_high_index_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_pyxtal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-24 19:44:43.000000 structuretoolkit-0.0.7/versioneer.py
```

### Comparing `structuretoolkit-0.0.6/LICENSE` & `structuretoolkit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/PKG-INFO` & `structuretoolkit-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `structuretoolkit-0.0.6/README.md` & `structuretoolkit-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -44,20 +44,28 @@
 
 ### Build
 * `stk.build.get_grainboundary_info()`
 * `stk.build.grainboundary()`
 * `stk.build.high_index_surface()`
 * `stk.build.get_high_index_surface_info()`
 * `stk.build.sqs_structures()`
+* `stk.build.pyxtal()`
 * `stk.build.B2()`
 * `stk.build.C14()`
 * `stk.build.C15()`
 * `stk.build.C36()`
 * `stk.build.D03()`
 
 ### Visualize 
 * `stk.visualize.plot3d()`
 
 ### Common 
 * `stk.common.ase_to_pymatgen()`
 * `stk.common.pymatgen_to_ase()`
+* `stk.common.pymatgen_read_from_file()`
 * `stk.common.ase_to_pyscal()`
+* `stk.common.apply_strain()`
+* `stk.common.center_coordinates_in_unit_cell()`
+* `stk.common.get_extended_positions()`
+* `stk.common.get_vertical_length()`
+* `stk.common.get_wrapped_coordinates()`
+* `stk.common.select_index()`
```

### Comparing `structuretoolkit-0.0.6/setup.py` & `structuretoolkit-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     install_requires=[
         'ase>=3.22.1',
         'matplotlib>=3.7.2',  # ase already requires matplotlib
         'numpy>=1.24.3',  # ase already requires numpy
         'scipy>=1.11.1',  # ase already requires scipy
     ],
     extras_require={
-        "grainboundary": ['aimsgb>=1.0.1', 'pymatgen>=2023.7.20'],
+        "grainboundary": ['aimsgb>=1.0.3', 'pymatgen>=2023.7.20'],
         "pyscal": ['pyscal2>=2.10.18'],
         "nglview": ['nglview>=3.0.6'],
         "plotly": ['plotly>=5.15.0'],
         "clusters": ['scikit-learn>=1.3.0'],
         "symmetry": ['spglib>=2.0.2'],
         "surface": ['spglib>=2.0.2', 'pymatgen>=2023.7.20'],
         "phonopy": ['phonopy>=2.20.0', 'spglib>=2.0.2'],
-        "pyxtal": ['pyxtal>=0.5.8']
+        "pyxtal": ['pyxtal>=0.5.9']
     },
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `structuretoolkit-0.0.6/structuretoolkit/__init__.py` & `structuretoolkit-0.0.7/structuretoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/analyse/__init__.py` & `structuretoolkit-0.0.7/structuretoolkit/analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/analyse/distance.py` & `structuretoolkit-0.0.7/structuretoolkit/analyse/distance.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/analyse/neighbors.py` & `structuretoolkit-0.0.7/structuretoolkit/analyse/neighbors.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/analyse/phonopy.py` & `structuretoolkit-0.0.7/structuretoolkit/analyse/phonopy.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/analyse/pyscal.py` & `structuretoolkit-0.0.7/structuretoolkit/analyse/pyscal.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/analyse/spatial.py` & `structuretoolkit-0.0.7/structuretoolkit/analyse/spatial.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/analyse/strain.py` & `structuretoolkit-0.0.7/structuretoolkit/analyse/strain.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/analyse/symmetry.py` & `structuretoolkit-0.0.7/structuretoolkit/analyse/symmetry.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/build/aimsgb.py` & `structuretoolkit-0.0.7/structuretoolkit/build/aimsgb.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/build/compound.py` & `structuretoolkit-0.0.7/structuretoolkit/build/compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/build/random.py` & `structuretoolkit-0.0.7/structuretoolkit/build/random.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/build/sqs.py` & `structuretoolkit-0.0.7/structuretoolkit/build/sqs.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/build/surface.py` & `structuretoolkit-0.0.7/structuretoolkit/build/surface.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/common/helper.py` & `structuretoolkit-0.0.7/structuretoolkit/common/helper.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit/visualize.py` & `structuretoolkit-0.0.7/structuretoolkit/visualize.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/structuretoolkit.egg-info/PKG-INFO` & `structuretoolkit-0.0.7/structuretoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `structuretoolkit-0.0.6/structuretoolkit.egg-info/SOURCES.txt` & `structuretoolkit-0.0.7/structuretoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_aimsgb.py` & `structuretoolkit-0.0.7/tests/test_aimsgb.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_analyse.py` & `structuretoolkit-0.0.7/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_compound.py` & `structuretoolkit-0.0.7/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_high_index_surface.py` & `structuretoolkit-0.0.7/tests/test_high_index_surface.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_neighbors.py` & `structuretoolkit-0.0.7/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_pyscal.py` & `structuretoolkit-0.0.7/tests/test_pyscal.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_pyxtal.py` & `structuretoolkit-0.0.7/tests/test_pyxtal.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_strain.py` & `structuretoolkit-0.0.7/tests/test_strain.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_symmetry.py` & `structuretoolkit-0.0.7/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/tests/test_visualize.py` & `structuretoolkit-0.0.7/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.6/versioneer.py` & `structuretoolkit-0.0.7/versioneer.py`

 * *Files identical despite different names*

