# Comparing `tmp/SiPMai-0.0.7.tar.gz` & `tmp/SiPMai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiPMai-0.0.7.tar", last modified: Thu Jul 20 03:26:45 2023, max compression
+gzip compressed data, was "SiPMai-0.0.8.tar", last modified: Mon Jul 24 02:49:10 2023, max compression
```

## Comparing `SiPMai-0.0.7.tar` & `SiPMai-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 03:26:45.491459 SiPMai-0.0.7/
--rw-rw-rw-   0        0        0     1086 2023-07-18 06:39:47.000000 SiPMai-0.0.7/LICENSE.md
--rw-rw-rw-   0        0        0     4409 2023-07-20 03:26:45.490458 SiPMai-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3895 2023-07-19 15:22:23.000000 SiPMai-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 03:26:45.415454 SiPMai-0.0.7/SiPMai/
--rw-rw-rw-   0        0        0      107 2023-07-20 03:26:06.000000 SiPMai-0.0.7/SiPMai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:26:45.445486 SiPMai-0.0.7/SiPMai/gen_data/
--rw-rw-rw-   0        0        0       53 2023-07-19 03:54:35.000000 SiPMai-0.0.7/SiPMai/gen_data/__init__.py
--rw-rw-rw-   0        0        0     4687 2023-07-20 02:35:15.000000 SiPMai-0.0.7/SiPMai/gen_data/compute_img.py
--rw-rw-rw-   0        0        0     7272 2023-07-20 02:47:51.000000 SiPMai-0.0.7/SiPMai/gen_data/gen_all_data_pipeline.py
--rw-rw-rw-   0        0        0     3498 2023-07-17 15:04:41.000000 SiPMai-0.0.7/SiPMai/gen_data/prepare_dataset.py
--rw-rw-rw-   0        0        0    10648 2023-07-20 03:22:20.000000 SiPMai-0.0.7/SiPMai/gen_data/ray_generation.py
--rw-rw-rw-   0        0        0    11369 2023-07-19 10:21:20.000000 SiPMai-0.0.7/SiPMai/gen_data/smi_molecule_simulation.py
--rw-rw-rw-   0        0        0     2896 2023-07-19 03:08:31.000000 SiPMai-0.0.7/SiPMai/gen_data/smile_generation.py
--rw-rw-rw-   0        0        0     2063 2023-07-20 02:33:39.000000 SiPMai-0.0.7/SiPMai/gen_data/util_fn.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:26:45.448454 SiPMai-0.0.7/SiPMai/smiles/
--rw-rw-rw-   0        0        0        0 2023-07-19 05:06:31.000000 SiPMai-0.0.7/SiPMai/smiles/__init__.py
--rw-rw-rw-   0        0        0 41963544 2023-07-17 10:17:15.000000 SiPMai-0.0.7/SiPMai/smiles/pubchem_39_200_100k.json
-drwxrwxrwx   0        0        0        0 2023-07-20 03:26:45.486449 SiPMai-0.0.7/SiPMai/unittest/
--rw-rw-rw-   0        0        0        0 2023-07-19 03:45:56.000000 SiPMai-0.0.7/SiPMai/unittest/__init__.py
--rw-rw-rw-   0        0        0     2538 2023-07-19 07:42:46.000000 SiPMai-0.0.7/SiPMai/unittest/test_gen_data.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:26:45.489458 SiPMai-0.0.7/SiPMai/utils/
--rw-rw-rw-   0        0        0        0 2023-07-18 03:21:53.000000 SiPMai-0.0.7/SiPMai/utils/__init__.py
--rw-rw-rw-   0        0        0     6435 2023-07-20 03:25:52.000000 SiPMai-0.0.7/SiPMai/utils/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:26:45.435453 SiPMai-0.0.7/SiPMai.egg-info/
--rw-rw-rw-   0        0        0     4409 2023-07-20 03:26:45.000000 SiPMai-0.0.7/SiPMai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-07-20 03:26:45.000000 SiPMai-0.0.7/SiPMai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 03:26:45.000000 SiPMai-0.0.7/SiPMai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-20 03:26:45.000000 SiPMai-0.0.7/SiPMai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      150 2023-07-20 03:26:45.000000 SiPMai-0.0.7/SiPMai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 03:26:45.000000 SiPMai-0.0.7/SiPMai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 03:26:45.491459 SiPMai-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1815 2023-07-19 05:12:14.000000 SiPMai-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.830535 SiPMai-0.0.8/
+-rw-rw-rw-   0        0        0     1086 2023-07-18 06:39:47.000000 SiPMai-0.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0     4409 2023-07-24 02:49:10.829533 SiPMai-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3895 2023-07-19 15:22:23.000000 SiPMai-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.695988 SiPMai-0.0.8/SiPMai/
+-rw-rw-rw-   0        0        0      107 2023-07-24 02:46:10.000000 SiPMai-0.0.8/SiPMai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.760529 SiPMai-0.0.8/SiPMai/gen_data/
+-rw-rw-rw-   0        0        0       53 2023-07-19 03:54:35.000000 SiPMai-0.0.8/SiPMai/gen_data/__init__.py
+-rw-rw-rw-   0        0        0     4687 2023-07-20 02:35:15.000000 SiPMai-0.0.8/SiPMai/gen_data/compute_img.py
+-rw-rw-rw-   0        0        0     7272 2023-07-20 02:47:51.000000 SiPMai-0.0.8/SiPMai/gen_data/gen_all_data_pipeline.py
+-rw-rw-rw-   0        0        0     3498 2023-07-17 15:04:41.000000 SiPMai-0.0.8/SiPMai/gen_data/prepare_dataset.py
+-rw-rw-rw-   0        0        0    10801 2023-07-24 02:45:33.000000 SiPMai-0.0.8/SiPMai/gen_data/ray_generation.py
+-rw-rw-rw-   0        0        0    11369 2023-07-19 10:21:20.000000 SiPMai-0.0.8/SiPMai/gen_data/smi_molecule_simulation.py
+-rw-rw-rw-   0        0        0     2896 2023-07-19 03:08:31.000000 SiPMai-0.0.8/SiPMai/gen_data/smile_generation.py
+-rw-rw-rw-   0        0        0     2063 2023-07-20 02:33:39.000000 SiPMai-0.0.8/SiPMai/gen_data/util_fn.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.767530 SiPMai-0.0.8/SiPMai/smiles/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:06:31.000000 SiPMai-0.0.8/SiPMai/smiles/__init__.py
+-rw-rw-rw-   0        0        0 41963544 2023-07-17 10:17:15.000000 SiPMai-0.0.8/SiPMai/smiles/pubchem_39_200_100k.json
+drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.814529 SiPMai-0.0.8/SiPMai/unittest/
+-rw-rw-rw-   0        0        0        0 2023-07-19 03:45:56.000000 SiPMai-0.0.8/SiPMai/unittest/__init__.py
+-rw-rw-rw-   0        0        0     2538 2023-07-19 07:42:46.000000 SiPMai-0.0.8/SiPMai/unittest/test_gen_data.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.828534 SiPMai-0.0.8/SiPMai/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-18 03:21:53.000000 SiPMai-0.0.8/SiPMai/utils/__init__.py
+-rw-rw-rw-   0        0        0     6435 2023-07-20 03:25:52.000000 SiPMai-0.0.8/SiPMai/utils/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.733531 SiPMai-0.0.8/SiPMai.egg-info/
+-rw-rw-rw-   0        0        0     4409 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      150 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 02:49:10.830535 SiPMai-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1815 2023-07-19 05:12:14.000000 SiPMai-0.0.8/setup.py
```

### Comparing `SiPMai-0.0.7/LICENSE.md` & `SiPMai-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/PKG-INFO` & `SiPMai-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiPMai
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Simple Yet Effective Scanning Tunnel Microscope Image Simulator
 Home-page: http://github.com/GilesLuo/SiPMai
 Author: Zhiyao Luo, Yaotian Yang, Jiali Li
 Author-email: zhiyao.luo@eng.ox.ac.uk
 License: MIT
 Project-URL: Source Code, https://github.com/my_username/my_package
 Keywords: Chemistry Simulation,STM Image Synthesis
```

### Comparing `SiPMai-0.0.7/README.md` & `SiPMai-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/gen_data/compute_img.py` & `SiPMai-0.0.8/SiPMai/gen_data/compute_img.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/gen_data/gen_all_data_pipeline.py` & `SiPMai-0.0.8/SiPMai/gen_data/gen_all_data_pipeline.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/gen_data/prepare_dataset.py` & `SiPMai-0.0.8/SiPMai/gen_data/prepare_dataset.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/gen_data/ray_generation.py` & `SiPMai-0.0.8/SiPMai/gen_data/ray_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,19 @@
     #         2D molecules were converted into 3D structures,
     #         and mechanical functions were used for Angle correction and optimization
     mol_2D = Chem.MolFromSmiles(smi)
     mol_2D_H = Chem.AddHs(mol_2D)
     atom_num = mol_2D_H.GetNumAtoms()
     bond_num = mol_2D_H.GetNumBonds()
 
-    moleblock_2D = Chem.MolToMolBlock(mol_2D_H)  # Returns the two-dimensional coordinates of the atoms in the molecule
+    try:
+        moleblock_2D = Chem.MolToMolBlock(mol_2D_H)  # Returns the two-dimensional coordinates of the atoms in the molecule
+    except Chem.rdchem.KekulizeException:
+        print("kekulize failed, molecule: ", molecule_name, ", skip...")
+        return False
     if show:
         mol_3D = Chem.MolFromSmiles(smi)
         Draw.ShowMol(mol_3D, size=(550, 550), kekulize=False)
         Draw.ShowMol(mol_2D_H, size=(550, 550), kekulize=False)
     mol_2D_H = Chem.MolFromMolBlock(moleblock_2D, removeHs=False)
     conf = mol_2D_H.GetConformer()
```

### Comparing `SiPMai-0.0.7/SiPMai/gen_data/smi_molecule_simulation.py` & `SiPMai-0.0.8/SiPMai/gen_data/smi_molecule_simulation.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/gen_data/smile_generation.py` & `SiPMai-0.0.8/SiPMai/gen_data/smile_generation.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/gen_data/util_fn.py` & `SiPMai-0.0.8/SiPMai/gen_data/util_fn.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/smiles/pubchem_39_200_100k.json` & `SiPMai-0.0.8/SiPMai/smiles/pubchem_39_200_100k.json`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/unittest/test_gen_data.py` & `SiPMai-0.0.8/SiPMai/unittest/test_gen_data.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai/utils/dataloader.py` & `SiPMai-0.0.8/SiPMai/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/SiPMai.egg-info/PKG-INFO` & `SiPMai-0.0.8/SiPMai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiPMai
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Simple Yet Effective Scanning Tunnel Microscope Image Simulator
 Home-page: http://github.com/GilesLuo/SiPMai
 Author: Zhiyao Luo, Yaotian Yang, Jiali Li
 Author-email: zhiyao.luo@eng.ox.ac.uk
 License: MIT
 Project-URL: Source Code, https://github.com/my_username/my_package
 Keywords: Chemistry Simulation,STM Image Synthesis
```

### Comparing `SiPMai-0.0.7/SiPMai.egg-info/SOURCES.txt` & `SiPMai-0.0.8/SiPMai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.7/setup.py` & `SiPMai-0.0.8/setup.py`

 * *Files identical despite different names*

