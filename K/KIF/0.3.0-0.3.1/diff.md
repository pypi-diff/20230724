# Comparing `tmp/KIF-0.3.0.tar.gz` & `tmp/KIF-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KIF-0.3.0.tar", last modified: Fri Jul 14 15:27:55 2023, max compression
+gzip compressed data, was "KIF-0.3.1.tar", last modified: Mon Jul 24 10:11:37 2023, max compression
```

## Comparing `KIF-0.3.0.tar` & `KIF-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 15:27:55.660726 KIF-0.3.0/
-drwxrwxrwx   0        0        0        0 2023-07-14 15:27:55.582602 KIF-0.3.0/KIF.egg-info/
--rw-rw-rw-   0        0        0      439 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      948 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2022-09-22 10:55:30.000000 KIF-0.3.0/LICENSE.md
--rw-rw-rw-   0        0        0      439 2023-07-14 15:27:55.660726 KIF-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    10602 2023-06-06 09:10:36.000000 KIF-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 15:27:55.645132 KIF-0.3.0/key_interactions_finder/
--rw-rw-rw-   0        0        0        0 2021-12-19 18:36:56.000000 KIF-0.3.0/key_interactions_finder/__init__.py
--rw-rw-rw-   0        0        0    12306 2023-07-14 15:10:53.000000 KIF-0.3.0/key_interactions_finder/contact_identification.py
--rw-rw-rw-   0        0        0    10177 2023-07-14 09:23:12.000000 KIF-0.3.0/key_interactions_finder/contact_identification_old.py
--rw-rw-rw-   0        0        0    15396 2023-04-05 11:38:25.000000 KIF-0.3.0/key_interactions_finder/data_preperation.py
--rw-rw-rw-   0        0        0    35948 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/model_building.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:27:55.660726 KIF-0.3.0/key_interactions_finder/model_params/
--rw-rw-rw-   0        0        0      418 2022-08-15 09:07:57.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_custom.json
--rw-rw-rw-   0        0        0     4457 2022-08-15 08:59:17.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_exhaustive.json
--rw-rw-rw-   0        0        0     3003 2022-08-15 09:00:56.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_moderate.json
--rw-rw-rw-   0        0        0     1159 2022-03-02 11:45:57.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_none.json
--rw-rw-rw-   0        0        0     1471 2022-08-15 09:01:34.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_quick.json
--rw-rw-rw-   0        0        0    14426 2023-07-14 15:10:53.000000 KIF-0.3.0/key_interactions_finder/network_analysis.py
--rw-rw-rw-   0        0        0    36620 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/post_proccessing.py
--rw-rw-rw-   0        0        0    17183 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/pycontact_processing.py
--rw-rw-rw-   0        0        0    11503 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/pymol_projections.py
--rw-rw-rw-   0        0        0    19316 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/stat_modelling.py
--rw-rw-rw-   0        0        0     7786 2023-04-05 11:38:25.000000 KIF-0.3.0/key_interactions_finder/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-14 15:27:55.660726 KIF-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-07-14 15:11:43.000000 KIF-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:11:37.176185 KIF-0.3.1/
+drwxrwxrwx   0        0        0        0 2023-07-24 10:11:37.035586 KIF-0.3.1/KIF.egg-info/
+-rw-rw-rw-   0        0        0      439 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      948 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18431 2022-09-22 10:55:30.000000 KIF-0.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0      439 2023-07-24 10:11:37.176185 KIF-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10944 2023-07-24 10:06:40.000000 KIF-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 10:11:37.129335 KIF-0.3.1/key_interactions_finder/
+-rw-rw-rw-   0        0        0        0 2021-12-19 18:36:56.000000 KIF-0.3.1/key_interactions_finder/__init__.py
+-rw-rw-rw-   0        0        0    12253 2023-07-24 10:03:14.000000 KIF-0.3.1/key_interactions_finder/contact_identification.py
+-rw-rw-rw-   0        0        0    10177 2023-07-14 09:23:12.000000 KIF-0.3.1/key_interactions_finder/contact_identification_old.py
+-rw-rw-rw-   0        0        0    15396 2023-04-05 11:38:25.000000 KIF-0.3.1/key_interactions_finder/data_preperation.py
+-rw-rw-rw-   0        0        0    35948 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/model_building.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:11:37.176185 KIF-0.3.1/key_interactions_finder/model_params/
+-rw-rw-rw-   0        0        0      418 2022-08-15 09:07:57.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_custom.json
+-rw-rw-rw-   0        0        0     4457 2022-08-15 08:59:17.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_exhaustive.json
+-rw-rw-rw-   0        0        0     3003 2022-08-15 09:00:56.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_moderate.json
+-rw-rw-rw-   0        0        0     1159 2022-03-02 11:45:57.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_none.json
+-rw-rw-rw-   0        0        0     1471 2022-08-15 09:01:34.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_quick.json
+-rw-rw-rw-   0        0        0    14426 2023-07-14 15:10:53.000000 KIF-0.3.1/key_interactions_finder/network_analysis.py
+-rw-rw-rw-   0        0        0    36620 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/post_proccessing.py
+-rw-rw-rw-   0        0        0    17183 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/pycontact_processing.py
+-rw-rw-rw-   0        0        0    11503 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/pymol_projections.py
+-rw-rw-rw-   0        0        0    19316 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/stat_modelling.py
+-rw-rw-rw-   0        0        0     7786 2023-04-05 11:38:25.000000 KIF-0.3.1/key_interactions_finder/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-24 10:11:37.176185 KIF-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-07-24 10:07:35.000000 KIF-0.3.1/setup.py
```

### Comparing `KIF-0.3.0/KIF.egg-info/SOURCES.txt` & `KIF-0.3.1/KIF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/LICENSE.md` & `KIF-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/README.md` & `KIF-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 # KIF - Key Interactions Finder
  A python package to identify the key molecular interactions that regulate any conformational change.
 
- ### New in Version 0.2.0  - (05/04/2023)
-Now non-covalent interactions can be identified directly from a trajectory using KIF, just make sure your trajectory is [imaged](http://ambermd.org/Questions/periodic2.html), as you would normally do so.
+ ### New in Version 0.3.0  - (14/07/2023)
+The non-covalent interaction detection part of KIF has been rewritten to be much faster. 
+These changes have the biggest effect on larger systems.
+
+#### Example improvements:
+**Small trajectory of 214 residues and 98 frames.**
+- Old code: 5 min 54 seconds
+- New code: 29 seconds
+
+**Larger system of 827 residues, 1 frame. **
+- Old code: more than 20 mins.  
+- New code: 8.4 seconds
 
-**Note** - If you have already used PyContact (the prior method to calculate non-covalent interactions) don't worry, you can still use the PyContact generated dataset in the newer version(s) of KIF.
-
-In order to use this feature you'll need to update your install of KIF to at least 0.2.0 or greater:
+In order to make use of this you'll need to update your install of KIF to at least 0.3.0 or greater:
 ```
 pip install --upgrade KIF
 ```
 
+**Keep in mind** that your trajectory(s) must be [imaged](http://ambermd.org/Questions/periodic2.html) before using KIF, to remove periodic effects. 
+
+**Note**  If you have already used PyContact (the prior method to calculate non-covalent interactions) don't worry, you can still use the PyContact generated dataset in the newer version(s) of KIF.
+
+
 ![KIF_ReadMe_Pic](https://user-images.githubusercontent.com/49672044/207597051-7dcde86a-62bd-4f69-96aa-326cad938a65.png)
 
 
 ## In short, this package allows you to:
  - Identify important non-covalent interactions that are associated with any conformational change you are interested in (as long as you can describe the descriptor and sample the descriptor in your MD simulations). The non-covalent interactions are scored according to their association/importance to the conformational change and you can easily convert the per interaction/feature scores to per residue scores as well.
  - Generate [PyMOL](https://pymol.org/2/) output scripts that enable you to visualise your results on 3D structures.
  - Generate per residue correlation and distance matrices that can be easily applied to the many graph theory methods available in order to study protein interaction networks and allostery within your system (no descriptor/target variable required for this).
```

### Comparing `KIF-0.3.0/key_interactions_finder/contact_identification.py` & `KIF-0.3.1/key_interactions_finder/contact_identification.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,44 +114,40 @@
         """
         warnings.warn(warning_message)
 
         biggest_res = last_res
     else:
         biggest_res = biggest_protein_res
 
-    # some setup steps.
-    hbond_pairs = _determine_hbond_pairs(universe=universe)
-
     trajectory_length = len(universe.trajectory)
     trajectory_of_zeros = np.zeros(trajectory_length)
 
-    all_heavy_atoms_sele = (
-        "not name H* and resid " + str(first_res) + "-" + str(biggest_res)
-    )
+    all_heavy_atoms_sele = "not name H* and resid 1" + "-" + str(biggest_res)
     all_heavy_atoms = universe.select_atoms(all_heavy_atoms_sele)
     residue_names = [names.capitalize() for names in list(universe.residues.resnames)]
 
     # determine which residue each heavy atom belongs to.
     residue_ranges = {}
     for res_numb in range(1, biggest_res + 1):
         residue_range = np.where(all_heavy_atoms.atoms.resids == res_numb)
         residue_ranges[res_numb] = residue_range
 
     print("setup complete, analysing contacts now...")
+    hbond_pairs = _determine_hbond_pairs(universe=universe)
 
     # Now go through each frame.
     all_contact_scores = {}
     for idx, _ in enumerate(universe.trajectory):  # each step is new frame.
         # calculate all heavy atom distances for this trajectory
         heavy_atom_dists = distances.distance_array(
             all_heavy_atoms.positions,
             all_heavy_atoms.positions,
         )
 
-        for res1 in range(1, last_res + 1):
+        for res1 in range(first_res, last_res + 1):
             res_dists = heavy_atom_dists[residue_ranges[res1]]
 
             # +3 here as neighbouring residues not interesting.
             for res2 in range(res1 + 3, biggest_res + 1):
                 res_res_dists = res_dists[:, residue_ranges[res2]]
 
                 # score would be 0 if true.
```

### Comparing `KIF-0.3.0/key_interactions_finder/contact_identification_old.py` & `KIF-0.3.1/key_interactions_finder/contact_identification_old.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/data_preperation.py` & `KIF-0.3.1/key_interactions_finder/data_preperation.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/model_building.py` & `KIF-0.3.1/key_interactions_finder/model_building.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/model_params/gridsearch_exhaustive.json` & `KIF-0.3.1/key_interactions_finder/model_params/gridsearch_exhaustive.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/model_params/gridsearch_moderate.json` & `KIF-0.3.1/key_interactions_finder/model_params/gridsearch_moderate.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/model_params/gridsearch_none.json` & `KIF-0.3.1/key_interactions_finder/model_params/gridsearch_none.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/model_params/gridsearch_quick.json` & `KIF-0.3.1/key_interactions_finder/model_params/gridsearch_quick.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/network_analysis.py` & `KIF-0.3.1/key_interactions_finder/network_analysis.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/post_proccessing.py` & `KIF-0.3.1/key_interactions_finder/post_proccessing.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/pycontact_processing.py` & `KIF-0.3.1/key_interactions_finder/pycontact_processing.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/pymol_projections.py` & `KIF-0.3.1/key_interactions_finder/pymol_projections.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/stat_modelling.py` & `KIF-0.3.1/key_interactions_finder/stat_modelling.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/key_interactions_finder/utils.py` & `KIF-0.3.1/key_interactions_finder/utils.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.0/setup.py` & `KIF-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 DESCRIPTION = "Python package for MD simulation analysis"
 LONG_DESCRIPTION = """
     A python package to identify the key molecular interactions that regulate any conformational change."""
 
 setup(
     name="KIF",
     version=VERSION,
```

