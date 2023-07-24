# Comparing `tmp/aimsgb-1.0.2.tar.gz` & `tmp/aimsgb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimsgb-1.0.2.tar", last modified: Mon Jul 24 00:15:24 2023, max compression
+gzip compressed data, was "aimsgb-1.0.3.tar", last modified: Mon Jul 24 16:35:14 2023, max compression
```

## Comparing `aimsgb-1.0.2.tar` & `aimsgb-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.940379 aimsgb-1.0.2/
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.916897 aimsgb-1.0.2/.github/
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.922389 aimsgb-1.0.2/.github/workflows/
--rw-r--r--   0 jianli     (501) staff       (20)     1113 2023-06-26 21:37:50.000000 aimsgb-1.0.2/.github/workflows/testing.yml
--rw-r--r--   0 jianli     (501) staff       (20)     1248 2022-06-20 18:41:58.000000 aimsgb-1.0.2/.gitignore
--rw-r--r--   0 jianli     (501) staff       (20)     1792 2018-10-27 01:29:57.000000 aimsgb-1.0.2/COPYRIGHT.rst
--rw-r--r--   0 jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-1.0.2/LICENSE.txt
--rw-r--r--   0 jianli     (501) staff       (20)     4698 2023-07-24 00:15:24.940507 aimsgb-1.0.2/PKG-INFO
--rw-r--r--   0 jianli     (501) staff       (20)     3620 2023-05-21 04:14:14.000000 aimsgb-1.0.2/README.rst
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.927077 aimsgb-1.0.2/aimsgb/
--rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-1.0.2/aimsgb/__init__.py
--rw-r--r--   0 jianli     (501) staff       (20)     7053 2023-06-26 21:37:50.000000 aimsgb-1.0.2/aimsgb/agb.py
--rw-r--r--   0 jianli     (501) staff       (20)    13962 2023-07-24 00:01:09.000000 aimsgb-1.0.2/aimsgb/grain.py
--rw-r--r--   0 jianli     (501) staff       (20)    22255 2023-06-29 19:16:39.000000 aimsgb-1.0.2/aimsgb/grain_bound.py
--rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-1.0.2/aimsgb/utils.py
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.929374 aimsgb-1.0.2/aimsgb.egg-info/
--rw-r--r--   0 jianli     (501) staff       (20)     4698 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/PKG-INFO
--rw-r--r--   0 jianli     (501) staff       (20)      836 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/SOURCES.txt
--rw-r--r--   0 jianli     (501) staff       (20)        1 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/dependency_links.txt
--rw-r--r--   0 jianli     (501) staff       (20)       43 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/entry_points.txt
--rw-r--r--   0 jianli     (501) staff       (20)       29 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/requires.txt
--rw-r--r--   0 jianli     (501) staff       (20)       24 2023-07-24 00:15:24.000000 aimsgb-1.0.2/aimsgb.egg-info/top_level.txt
--rw-r--r--   0 jianli     (501) staff       (20)       80 2023-07-24 00:15:24.940950 aimsgb-1.0.2/setup.cfg
--rw-r--r--   0 jianli     (501) staff       (20)     5191 2023-07-24 00:10:02.000000 aimsgb-1.0.2/setup.py
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.929754 aimsgb-1.0.2/tests/
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.930447 aimsgb-1.0.2/tests/input/
--rw-r--r--   0 jianli     (501) staff       (20)      356 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/input/POSCAR_mp-13
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.933277 aimsgb-1.0.2/tests/non_cubic/
--rw-r--r--   0 jianli     (501) staff       (20)      578 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp
--rw-r--r--   0 jianli     (501) staff       (20)      577 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp
--rw-r--r--   0 jianli     (501) staff       (20)     1606 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp
--rw-r--r--   0 jianli     (501) staff       (20)     3068 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp
--rw-r--r--   0 jianli     (501) staff       (20)      878 2023-06-28 17:38:35.000000 aimsgb-1.0.2/tests/test_grain.py
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.936813 aimsgb-1.0.2/tests/time/
--rw-r--r--   0 jianli     (501) staff       (20)    52153 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/POSCAR_a
--rw-r--r--   0 jianli     (501) staff       (20)    52153 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/POSCAR_b
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.937447 aimsgb-1.0.2/tests/time/out/
--rw-r--r--   0 jianli     (501) staff       (20)    44157 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/out/POSCAR
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 00:15:24.939869 aimsgb-1.0.2/tests/time/poscars/
--rw-r--r--   0 jianli     (501) staff       (20)     1090 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/poscars/POSCAR_MASnI3
--rw-r--r--   0 jianli     (501) staff       (20)      498 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/poscars/POSCAR_SrTiO3
--rw-r--r--   0 jianli     (501) staff       (20)      919 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/poscars/POSCAR_TiO2_Anatase
--rw-r--r--   0 jianli     (501) staff       (20)       44 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/readme.txt
--rw-r--r--   0 jianli     (501) staff       (20)      975 2023-06-26 21:37:50.000000 aimsgb-1.0.2/tests/time/time.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.558483 aimsgb-1.0.3/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.532656 aimsgb-1.0.3/.github/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.538958 aimsgb-1.0.3/.github/workflows/
+-rw-r--r--   0 jianli     (501) staff       (20)     1113 2023-06-26 21:37:50.000000 aimsgb-1.0.3/.github/workflows/testing.yml
+-rw-r--r--   0 jianli     (501) staff       (20)     1248 2022-06-20 18:41:58.000000 aimsgb-1.0.3/.gitignore
+-rw-r--r--   0 jianli     (501) staff       (20)     1792 2018-10-27 01:29:57.000000 aimsgb-1.0.3/COPYRIGHT.rst
+-rw-r--r--   0 jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-1.0.3/LICENSE.txt
+-rw-r--r--   0 jianli     (501) staff       (20)     4698 2023-07-24 16:35:14.558643 aimsgb-1.0.3/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)     3620 2023-05-21 04:14:14.000000 aimsgb-1.0.3/README.rst
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.544284 aimsgb-1.0.3/aimsgb/
+-rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-1.0.3/aimsgb/__init__.py
+-rw-r--r--   0 jianli     (501) staff       (20)     7053 2023-06-26 21:37:50.000000 aimsgb-1.0.3/aimsgb/agb.py
+-rw-r--r--   0 jianli     (501) staff       (20)    13957 2023-07-24 16:26:04.000000 aimsgb-1.0.3/aimsgb/grain.py
+-rw-r--r--   0 jianli     (501) staff       (20)    22255 2023-07-24 05:24:59.000000 aimsgb-1.0.3/aimsgb/grain_bound.py
+-rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-1.0.3/aimsgb/utils.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.547056 aimsgb-1.0.3/aimsgb.egg-info/
+-rw-r--r--   0 jianli     (501) staff       (20)     4698 2023-07-24 16:35:14.000000 aimsgb-1.0.3/aimsgb.egg-info/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)      836 2023-07-24 16:35:14.000000 aimsgb-1.0.3/aimsgb.egg-info/SOURCES.txt
+-rw-r--r--   0 jianli     (501) staff       (20)        1 2023-07-24 16:35:14.000000 aimsgb-1.0.3/aimsgb.egg-info/dependency_links.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       43 2023-07-24 16:35:14.000000 aimsgb-1.0.3/aimsgb.egg-info/entry_points.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       29 2023-07-24 16:35:14.000000 aimsgb-1.0.3/aimsgb.egg-info/requires.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       24 2023-07-24 16:35:14.000000 aimsgb-1.0.3/aimsgb.egg-info/top_level.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       80 2023-07-24 16:35:14.559364 aimsgb-1.0.3/setup.cfg
+-rw-r--r--   0 jianli     (501) staff       (20)     5191 2023-07-24 16:34:08.000000 aimsgb-1.0.3/setup.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.547365 aimsgb-1.0.3/tests/
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.547962 aimsgb-1.0.3/tests/input/
+-rw-r--r--   0 jianli     (501) staff       (20)      356 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/input/POSCAR_mp-13
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.550585 aimsgb-1.0.3/tests/non_cubic/
+-rw-r--r--   0 jianli     (501) staff       (20)      578 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)      577 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)     1606 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)     3068 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp
+-rw-r--r--   0 jianli     (501) staff       (20)      878 2023-06-28 17:38:35.000000 aimsgb-1.0.3/tests/test_grain.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.553847 aimsgb-1.0.3/tests/time/
+-rw-r--r--   0 jianli     (501) staff       (20)    52153 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/time/POSCAR_a
+-rw-r--r--   0 jianli     (501) staff       (20)    52153 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/time/POSCAR_b
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.554723 aimsgb-1.0.3/tests/time/out/
+-rw-r--r--   0 jianli     (501) staff       (20)    44157 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/time/out/POSCAR
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-07-24 16:35:14.557732 aimsgb-1.0.3/tests/time/poscars/
+-rw-r--r--   0 jianli     (501) staff       (20)     1090 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/time/poscars/POSCAR_MASnI3
+-rw-r--r--   0 jianli     (501) staff       (20)      498 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/time/poscars/POSCAR_SrTiO3
+-rw-r--r--   0 jianli     (501) staff       (20)      919 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/time/poscars/POSCAR_TiO2_Anatase
+-rw-r--r--   0 jianli     (501) staff       (20)       44 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/time/readme.txt
+-rw-r--r--   0 jianli     (501) staff       (20)      975 2023-06-26 21:37:50.000000 aimsgb-1.0.3/tests/time/time.py
```

### Comparing `aimsgb-1.0.2/.github/workflows/testing.yml` & `aimsgb-1.0.3/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/.gitignore` & `aimsgb-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/COPYRIGHT.rst` & `aimsgb-1.0.3/COPYRIGHT.rst`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/LICENSE.txt` & `aimsgb-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/PKG-INFO` & `aimsgb-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsgb
-Version: 1.0.2
+Version: 1.0.3
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
 Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimsgb-1.0.2/README.rst` & `aimsgb-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/aimsgb/agb.py` & `aimsgb-1.0.3/aimsgb/agb.py`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/aimsgb/grain.py` & `aimsgb-1.0.3/aimsgb/grain.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         layers = self.sort_sites_in_layers(tol=tol, direction=direction)
         l_dist = abs(layers[l1][0][0].coords[direction] - layers[l2][0][0].coords[direction])
         l_vector = [1, 1]
         l_vector.insert(direction, (l - l_dist) / l)
         new_lat = Lattice(self.lattice.matrix * np.array(l_vector)[:, None])
 
         layers.pop(l1)
-        sites = reduce(lambda x, y: np.concatenate((x, y), direction=0), layers)
+        sites = reduce(lambda x, y: np.concatenate((x, y), axis=0), layers)
         new_sites = []
         l_dist = 0 if bt == "t" else l_dist
         l_vector = [0, 0]
         l_vector.insert(direction, l_dist)
         for site, _ in sites:
             new_sites.append(PeriodicSite(site.specie, site.coords - l_vector,
                                           new_lat, coords_are_cartesian=True))
```

### Comparing `aimsgb-1.0.2/aimsgb/grain_bound.py` & `aimsgb-1.0.3/aimsgb/grain_bound.py`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/aimsgb/utils.py` & `aimsgb-1.0.3/aimsgb/utils.py`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/aimsgb.egg-info/PKG-INFO` & `aimsgb-1.0.3/aimsgb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsgb
-Version: 1.0.2
+Version: 1.0.3
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
 Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimsgb-1.0.2/aimsgb.egg-info/SOURCES.txt` & `aimsgb-1.0.3/aimsgb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/setup.py` & `aimsgb-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 =================================
 http://materials.ucsd.edu/
 """
 
 setup(
     name="aimsgb",
     packages=find_namespace_packages(exclude=["*.tests"]),
-    version="1.0.2",
+    version="1.0.3",
     setup_requires=["setuptools>=18.0"],
     install_requires=["pymatgen", "mp_api", "numpy", "pytest"],
     include_package_data=True,
     author="Jianli Cheng and Kesong YANG",
     maintainer="Jianli Cheng, Sicong JIANG, and Kesong YANG",
     maintainer_email="chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu",
     url="http://aimsgb.org",
```

### Comparing `aimsgb-1.0.2/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp` & `aimsgb-1.0.3/tests/non_cubic/POSCAR_Ba1Fe1O3_ICSD_262132_CUB.vasp`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp` & `aimsgb-1.0.3/tests/non_cubic/POSCAR_Bi1Fe1O3_ICSD_168320_MCL.vasp`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp` & `aimsgb-1.0.3/tests/non_cubic/POSCAR_GB_Ba1Fe1O3_ICSD_262132_CUB.vasp`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp` & `aimsgb-1.0.3/tests/non_cubic/POSCAR_GB_Bi1Fe1O3_ICSD_168320_MCL.vasp`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/test_grain.py` & `aimsgb-1.0.3/tests/test_grain.py`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/time/POSCAR_a` & `aimsgb-1.0.3/tests/time/POSCAR_a`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/time/POSCAR_b` & `aimsgb-1.0.3/tests/time/POSCAR_b`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/time/out/POSCAR` & `aimsgb-1.0.3/tests/time/out/POSCAR`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/time/poscars/POSCAR_MASnI3` & `aimsgb-1.0.3/tests/time/poscars/POSCAR_MASnI3`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/time/poscars/POSCAR_TiO2_Anatase` & `aimsgb-1.0.3/tests/time/poscars/POSCAR_TiO2_Anatase`

 * *Files identical despite different names*

### Comparing `aimsgb-1.0.2/tests/time/time.py` & `aimsgb-1.0.3/tests/time/time.py`

 * *Files identical despite different names*

