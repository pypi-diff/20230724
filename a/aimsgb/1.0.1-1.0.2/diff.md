# Comparing `tmp/aimsgb-1.0.1.tar.gz` & `tmp/aimsgb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimsgb-1.0.1.tar", last modified: Wed Jun 28 17:50:06 2023, max compression
+gzip compressed data, was "aimsgb-1.0.2.tar", last modified: Mon Jul 24 00:15:24 2023, max compression
```

## Comparing `aimsgb-1.0.1.tar` & `aimsgb-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:06.112301 aimsgb-1.0.1/
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:05.843619 aimsgb-1.0.1/.github/
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:05.867120 aimsgb-1.0.1/.github/workflows/
--rw-r--r--   0 Jianli     (501) staff       (20)     1113 2023-06-26 21:37:50.000000 aimsgb-1.0.1/.github/workflows/testing.yml
--rw-r--r--   0 Jianli     (501) staff       (20)     1248 2022-06-20 18:41:58.000000 aimsgb-1.0.1/.gitignore
--rw-r--r--   0 Jianli     (501) staff       (20)     1792 2018-10-27 01:29:57.000000 aimsgb-1.0.1/COPYRIGHT.rst
--rw-r--r--   0 Jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-1.0.1/LICENSE.txt
--rw-r--r--   0 Jianli     (501) staff       (20)     4698 2023-06-28 17:50:06.112629 aimsgb-1.0.1/PKG-INFO
--rw-r--r--   0 Jianli     (501) staff       (20)     3620 2023-05-21 04:14:14.000000 aimsgb-1.0.1/README.rst
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:05.885659 aimsgb-1.0.1/aimsgb/
--rw-r--r--   0 Jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-1.0.1/aimsgb/__init__.py
--rw-r--r--   0 Jianli     (501) staff       (20)     7053 2023-06-26 21:37:50.000000 aimsgb-1.0.1/aimsgb/agb.py
--rw-r--r--   0 Jianli     (501) staff       (20)    14403 2023-06-28 17:38:35.000000 aimsgb-1.0.1/aimsgb/grain.py
--rw-r--r--   0 Jianli     (501) staff       (20)    22255 2023-06-28 17:38:35.000000 aimsgb-1.0.1/aimsgb/grain_bound.py
--rw-r--r--   0 Jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-1.0.1/aimsgb/utils.py
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:05.894696 aimsgb-1.0.1/aimsgb.egg-info/
--rw-r--r--   0 Jianli     (501) staff       (20)     4698 2023-06-28 17:50:05.000000 aimsgb-1.0.1/aimsgb.egg-info/PKG-INFO
--rw-r--r--   0 Jianli     (501) staff       (20)      836 2023-06-28 17:50:05.000000 aimsgb-1.0.1/aimsgb.egg-info/SOURCES.txt
--rw-r--r--   0 Jianli     (501) staff       (20)        1 2023-06-28 17:50:05.000000 aimsgb-1.0.1/aimsgb.egg-info/dependency_links.txt
--rw-r--r--   0 Jianli     (501) staff       (20)       43 2023-06-28 17:50:05.000000 aimsgb-1.0.1/aimsgb.egg-info/entry_points.txt
--rw-r--r--   0 Jianli     (501) staff       (20)       29 2023-06-28 17:50:05.000000 aimsgb-1.0.1/aimsgb.egg-info/requires.txt
--rw-r--r--   0 Jianli     (501) staff       (20)       24 2023-06-28 17:50:05.000000 aimsgb-1.0.1/aimsgb.egg-info/top_level.txt
--rw-r--r--   0 Jianli     (501) staff       (20)       80 2023-06-28 17:50:06.119958 aimsgb-1.0.1/setup.cfg
--rw-r--r--   0 Jianli     (501) staff       (20)     5191 2023-06-28 17:40:11.000000 aimsgb-1.0.1/setup.py
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:05.895925 aimsgb-1.0.1/tests/
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:06.007695 aimsgb-1.0.1/tests/input/
--rw-r--r--   0 Jianli     (501) staff       (20)      356 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/input/POSCAR_mp-13
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:06.038608 aimsgb-1.0.1/tests/non_cubic/
--rw-r--r--   0 Jianli     (501) staff       (20)      578 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp
--rw-r--r--   0 Jianli     (501) staff       (20)      577 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp
--rw-r--r--   0 Jianli     (501) staff       (20)     1606 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp
--rw-r--r--   0 Jianli     (501) staff       (20)     3068 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp
--rw-r--r--   0 Jianli     (501) staff       (20)      878 2023-06-28 17:38:35.000000 aimsgb-1.0.1/tests/test_grain.py
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:06.088384 aimsgb-1.0.1/tests/time/
--rw-r--r--   0 Jianli     (501) staff       (20)    52153 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/time/POSCAR_a
--rw-r--r--   0 Jianli     (501) staff       (20)    52153 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/time/POSCAR_b
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:06.090313 aimsgb-1.0.1/tests/time/out/
--rw-r--r--   0 Jianli     (501) staff       (20)    44157 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/time/out/POSCAR
-drwxr-xr-x   0 Jianli     (501) staff       (20)        0 2023-06-28 17:50:06.110428 aimsgb-1.0.1/tests/time/poscars/
--rw-r--r--   0 Jianli     (501) staff       (20)     1090 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/time/poscars/POSCAR_MASnI3
--rw-r--r--   0 Jianli     (501) staff       (20)      498 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/time/poscars/POSCAR_SrTiO3
--rw-r--r--   0 Jianli     (501) staff       (20)      919 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/time/poscars/POSCAR_TiO2_Anatase
--rw-r--r--   0 Jianli     (501) staff       (20)       44 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/time/readme.txt
--rw-r--r--   0 Jianli     (501) staff       (20)      975 2023-06-26 21:37:50.000000 aimsgb-1.0.1/tests/time/time.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.940379 aimsgb-1.0.2/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.916897 aimsgb-1.0.2/.github/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.922389 aimsgb-1.0.2/.github/workflows/
+-rw-r--r--   0 jianli     (501) staff       (20)     1113 2023-06-26 21:37:50.000000 aimsgb-1.0.2/.github/workflows/testing.yml
+-rw-r--r--   0 jianli     (501) staff       (20)     1248 2022-06-20 18:41:58.000000 aimsgb-1.0.2/.gitignore
+-rw-r--r--   0 jianli     (501) staff       (20)     1792 2018-10-27 01:29:57.000000 aimsgb-1.0.2/COPYRIGHT.rst
+-rw-r--r--   0 jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-1.0.2/LICENSE.txt
+-rw-r--r--   0 jianli     (501) staff       (20)     4698 2023-07-24 00:15:24.940507 aimsgb-1.0.2/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)     3620 2023-05-21 04:14:14.000000 aimsgb-1.0.2/README.rst
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.927077 aimsgb-1.0.2/aimsgb/
+-rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-1.0.2/aimsgb/__init__.py
+-rw-r--r--   0 jianli     (501) staff       (20)     7053 2023-06-26 21:37:50.000000 aimsgb-1.0.2/aimsgb/agb.py
+-rw-r--r--   0 jianli     (501) staff       (20)    13962 2023-07-24 00:01:09.000000 aimsgb-1.0.2/aimsgb/grain.py
+-rw-r--r--   0 jianli     (501) staff       (20)    22255 2023-06-29 19:16:39.000000 aimsgb-1.0.2/aimsgb/grain_bound.py
+-rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-1.0.2/aimsgb/utils.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.929374 aimsgb-1.0.2/aimsgb.egg-info/
+-rw-r--r--   0 jianli     (501) staff       (20)     4698 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)      836 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/SOURCES.txt
+-rw-r--r--   0 jianli     (501) staff       (20)        1 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/dependency_links.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       43 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/entry_points.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       29 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/requires.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       24 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/top_level.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       80 2023-07-24 00:15:24.940950 aimsgb-1.0.2/setup.cfg
+-rw-r--r--   0 jianli     (501) staff       (20)     5191 2023-07-24 00:10:02.000000 aimsgb-1.0.2/setup.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.929754 aimsgb-1.0.2/tests/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.930447 aimsgb-1.0.2/tests/input/
+-rw-r--r--   0 jianli     (501) staff       (20)      356 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/input/POSCAR_mp-13
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.933277 aimsgb-1.0.2/tests/non_cubic/
+-rw-r--r--   0 jianli     (501) staff       (20)      578 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)      577 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)     1606 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)     3068 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)      878 2023-06-28 17:38:35.000000 aimsgb-1.0.2/tests/test_grain.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.936813 aimsgb-1.0.2/tests/time/
+-rw-r--r--   0 jianli     (501) staff       (20)    52153 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/POSCAR_a
+-rw-r--r--   0 jianli     (501) staff       (20)    52153 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/POSCAR_b
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.937447 aimsgb-1.0.2/tests/time/out/
+-rw-r--r--   0 jianli     (501) staff       (20)    44157 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/out/POSCAR
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.939869 aimsgb-1.0.2/tests/time/poscars/
+-rw-r--r--   0 jianli     (501) staff       (20)     1090 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/poscars/POSCAR_MASnI3
+-rw-r--r--   0 jianli     (501) staff       (20)      498 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/poscars/POSCAR_SrTiO3
+-rw-r--r--   0 jianli     (501) staff       (20)      919 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/poscars/POSCAR_TiO2_Anatase
+-rw-r--r--   0 jianli     (501) staff       (20)       44 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/readme.txt
+-rw-r--r--   0 jianli     (501) staff       (20)      975 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/time.py
```

### Comparing `aimsgb-1.0.1/.github/workflows/testing.yml` & `aimsgb-1.0.2/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/.gitignore` & `aimsgb-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/COPYRIGHT.rst` & `aimsgb-1.0.2/COPYRIGHT.rst`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/LICENSE.txt` & `aimsgb-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/PKG-INFO` & `aimsgb-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsgb
-Version: 1.0.1
+Version: 1.0.2
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
 Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimsgb-1.0.1/README.rst` & `aimsgb-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/aimsgb/agb.py` & `aimsgb-1.0.2/aimsgb/agb.py`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/aimsgb/grain.py` & `aimsgb-1.0.2/aimsgb/grain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import re
 import warnings
 import numpy as np
 from numpy import sin, radians
-from functools import reduce
+from functools import reduce, wraps
 from itertools import groupby
 from aimsgb.utils import reduce_vector
 from pymatgen.core.structure import Structure, Lattice, PeriodicSite
 from pymatgen.transformations.advanced_transformations import CubicSupercellTransformation
 from pymatgen.analysis.structure_matcher import StructureMatcher
 
 __author__ = "Jianli CHENG and Kesong YANG"
@@ -18,23 +18,17 @@
 __date__ = "January 26, 2018"
 
 
 class Grain(Structure):
     """
     We use the Structure class from pymatgen and add several new functions.
     """
-    def __init__(self, lattice, species, coords, charge=None,
-                 validate_proximity=False, to_unit_cell=False,
-                 coords_are_cartesian=False, site_properties=None):
-
-        super(Structure, self).__init__(lattice, species, coords, charge=charge,
-                                        validate_proximity=validate_proximity,
-                                        to_unit_cell=to_unit_cell,
-                                        coords_are_cartesian=coords_are_cartesian,
-                                        site_properties=site_properties)
+    @wraps(Structure.__init__)
+    def __init__(self, *args, **kwargs):
+        super(Structure, self).__init__(*args, **kwargs)
 
         self._sites = list(self._sites)
 
     @staticmethod
     def get_b_from_a(grain_a, csl):
         grain_b = grain_a.copy()
         csl_t = csl.transpose()
@@ -70,15 +64,15 @@
         Fix sites in certain layers. The layer by layer direction is given by direction.
         This function is useful for selective dynamics calculations in VASP.
 
         Args:
             layer_indices (list): A list of layer indices.
             tol (float): Tolerance factor in Angstrom to determnine if sites are 
                 in the same layer. Default to 0.25.
-            direction (int): Direction to sort the sites by layers. 0: x, 1: y, 2: z
+            direction (int): Direction to sort the sites by layers. 0: a, 1: b, 2: c
         """
         layers = self.sort_sites_in_layers(tol=tol, direction=direction)
         sd_sites = []
         for i, l in enumerate(layers):
             if i in layer_indices:
                 sd_sites.extend(zip([[False, False, False]] * len(l), [_i[1] for _i in l]))
             else:
@@ -115,15 +109,15 @@
         Delete bottom or top layer of the structure.
 
         Args:
             bt (str): Specify whether it's a top or bottom layer delete. "b"
                 means bottom layer and "t" means top layer.
             tol (float): Tolerance factor in Angstrom to determnine if sites are 
                 in the same layer. Default to 0.25.
-            direction (int): Direction to sort the sites by layers. 0: x, 1: y, 2: z
+            direction (int): Direction to sort the sites by layers. 0: a, 1: b, 2: c
         """
         if bt == "t":
             l1, l2 = (-1, -2)
         else:
             l1, l2 = (0, 1)
 
         l = self.lattice.abc[direction]
@@ -148,15 +142,15 @@
     def sort_sites_in_layers(self, tol=0.25, direction=2):
         """
         Sort the sites in a structure by layers.
 
         Args:
             tol (float): Tolerance factor in Angstrom to determnine if sites are 
                 in the same layer. Default to 0.25.
-            direction (int): Direction to sort the sites by layers. 0: x, 1: y, 2: z
+            direction (int): Direction to sort the sites by layers. 0: a, 1: b, 2: c
 
         Returns:
             Lists with a list of (site, index) in the same plane as one list.
         """
         sites_indices = sorted(zip(self.sites, range(len(self))), 
                                key=lambda x: x[0].frac_coords[direction])
         layers = []
@@ -212,15 +206,15 @@
         """
         Build structures for grain A and B from the coincidnet site lattice (CSL) matrix, 
         number of unit cell of grain A and number of unit cell of grain B. Each grain
         is essentially a supercell of the initial structure.
 
         Args:
             csl (3x3 matrix): CSL matrix (scaling matrix)
-            direction (int): Stacking direction of GB. 0: x, 1: y, 2: z
+            direction (int): Stacking direction of GB. 0: a, 1: b, 2: c
             uc_a (int): Number of unit cell of grain A. Default to 1.
             uc_b (int): Number of unit cell of grain B. Default to 1.
 
         Returns:
             Grain objects for grain A and B
         """
         csl_t = csl.transpose()
@@ -282,15 +276,15 @@
         a- and b-vectors.
 
         Args:
             grain_a (Grain): Substrate for the interface structure
             grain_b (Grain): Film for the interface structure
             vacuum (float): Vacuum space above the film in Angstroms. Default to 0.0
             gap (float): Gap between substrate and film in Angstroms. Default to 0.0
-            direction (int): Stacking direction of the interface structure. 0: x, 1: y, 2: z.
+            direction (int): Stacking direction of the interface structure. 0: a, 1: b, 2: c.
             delete_layer (str): Delete top and bottom layers of the substrate and film.
                 8 characters in total. The first 4 characters is for the substrate and
                 the other 4 is for the film. "b" means bottom layer and "t" means
                 top layer. Integer represents the number of layers to be deleted.
                 Default to "0b0t0b0t", which means no deletion of layers. The
                 direction of top and bottom layers is based on the given direction.
             tol (float): Tolerance factor in Angstrom to determnine if sites are
```

### Comparing `aimsgb-1.0.1/aimsgb/grain_bound.py` & `aimsgb-1.0.2/aimsgb/grain_bound.py`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/aimsgb/utils.py` & `aimsgb-1.0.2/aimsgb/utils.py`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/aimsgb.egg-info/PKG-INFO` & `aimsgb-1.0.2/aimsgb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsgb
-Version: 1.0.1
+Version: 1.0.2
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
 Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimsgb-1.0.1/aimsgb.egg-info/SOURCES.txt` & `aimsgb-1.0.2/aimsgb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/setup.py` & `aimsgb-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 =================================
 http://materials.ucsd.edu/
 """
 
 setup(
     name="aimsgb",
     packages=find_namespace_packages(exclude=["*.tests"]),
-    version="1.0.1",
+    version="1.0.2",
     setup_requires=["setuptools>=18.0"],
     install_requires=["pymatgen", "mp_api", "numpy", "pytest"],
     include_package_data=True,
     author="Jianli Cheng and Kesong YANG",
     maintainer="Jianli Cheng, Sicong JIANG, and Kesong YANG",
     maintainer_email="chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu",
     url="http://aimsgb.org",
```

### Comparing `aimsgb-1.0.1/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp` & `aimsgb-1.0.2/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp` & `aimsgb-1.0.2/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp` & `aimsgb-1.0.2/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp` & `aimsgb-1.0.2/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/test_grain.py` & `aimsgb-1.0.2/tests/test_grain.py`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/time/POSCAR_a` & `aimsgb-1.0.2/tests/time/POSCAR_a`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/time/POSCAR_b` & `aimsgb-1.0.2/tests/time/POSCAR_b`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/time/out/POSCAR` & `aimsgb-1.0.2/tests/time/out/POSCAR`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/time/poscars/POSCAR_MASnI3` & `aimsgb-1.0.2/tests/time/poscars/POSCAR_MASnI3`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/time/poscars/POSCAR_TiO2_Anatase` & `aimsgb-1.0.2/tests/time/poscars/POSCAR_TiO2_Anatase`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.1/tests/time/time.py` & `aimsgb-1.0.2/tests/time/time.py`

 * *Files identical despite different names*

