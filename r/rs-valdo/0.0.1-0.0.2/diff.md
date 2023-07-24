# Comparing `tmp/rs-valdo-0.0.1.tar.gz` & `tmp/rs-valdo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rs-valdo-0.0.1.tar", last modified: Fri May 19 16:05:11 2023, max compression
+gzip compressed data, was "rs-valdo-0.0.2.tar", last modified: Mon Jul 24 02:39:25 2023, max compression
```

## Comparing `rs-valdo-0.0.1.tar` & `rs-valdo-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:05:11.493922 rs-valdo-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-19 16:05:11.493922 rs-valdo-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:05:11.489922 rs-valdo-0.0.1/rs_valdo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-19 16:05:11.000000 rs-valdo-0.0.1/rs_valdo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-19 16:05:11.000000 rs-valdo-0.0.1/rs_valdo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:05:11.000000 rs-valdo-0.0.1/rs_valdo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 16:05:11.000000 rs-valdo-0.0.1/rs_valdo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 16:05:11.000000 rs-valdo-0.0.1/rs_valdo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:05:11.493922 rs-valdo-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:05:11.493922 rs-valdo-0.0.1/valdo/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/blobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/reindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/vae_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-05-19 16:04:59.000000 rs-valdo-0.0.1/valdo/vae_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:39:25.221716 rs-valdo-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-24 02:39:25.221716 rs-valdo-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:39:25.221716 rs-valdo-0.0.2/rs_valdo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-24 02:39:25.000000 rs-valdo-0.0.2/rs_valdo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 02:39:25.000000 rs-valdo-0.0.2/rs_valdo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:39:25.000000 rs-valdo-0.0.2/rs_valdo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 02:39:25.000000 rs-valdo-0.0.2/rs_valdo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 02:39:25.000000 rs-valdo-0.0.2/rs_valdo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 02:39:25.000000 rs-valdo-0.0.2/rs_valdo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:39:25.221716 rs-valdo-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:39:25.221716 rs-valdo-0.0.2/valdo/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/blobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/reindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/vae_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-24 02:39:12.000000 rs-valdo-0.0.2/valdo/vae_networks.py
```

### Comparing `rs-valdo-0.0.1/license` & `rs-valdo-0.0.2/license`

 * *Files identical despite different names*

### Comparing `rs-valdo-0.0.1/setup.py` & `rs-valdo-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,9 +17,15 @@
     author_email='phylliszhang@college.harvard.edu, minhuanli@g.harvard.edu',
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.10",
     install_requires=[
         "torch>=1.13.0",
         "reciprocalspaceship>=0.9.18",
+        "tqdm"
     ],
+    entry_points={
+        "console_scripts": [
+            "valdo.refine=valdo.commandline.refine:main",
+        ]
+    }
 )
```

### Comparing `rs-valdo-0.0.1/valdo/reindex.py` & `rs-valdo-0.0.2/valdo/reindex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 import pandas as pd
 import reciprocalspaceship as rs
+import gemmi
 import numpy as np
 import os
 from tqdm import tqdm
 import pickle
 
-def reindex_files(input_files, reference_file, output_folder):
+def reindex_files(input_files, reference_file, output_folder, columns=['F-obs', 'SIGF-obs']):
     """
     Reindexes a list of input MTZ files to a reference MTZ file using gemmi.
 
     Parameters:
-    input_files (list of str): List of paths to input MTZ files.
-    reference_file (str): Path to reference MTZ file.
-    output_folder (str): Path to folder where reindexed MTZ files will be saved.
+    input_files (list of str) : List of paths to input MTZ files.
+    reference_file (str) : Path to reference MTZ file.
+    output_folder (str) : Path to folder where reindexed MTZ files will be saved.
 
     Returns:
-    list of str: List of paths to reindexed MTZ files.
+    List[List[str]]: [[i, path_to_file],...]
+    if i == 0, no reindex
     """
 
     # Read the reference MTZ file
-    reference = rs.read_mtz(reference_file)[['F-obs', 'SIGF-obs']]
+    reference = rs.read_mtz(reference_file)[columns]
     reference_asu = reference.hkl_to_asu()
 
-    # Reindex each input MTZ file
-    reindexed_files = []
+    # Find the possible reindex ambiguity ops
+    unit_ops = [gemmi.Op("x,y,z")]
+    alt_ops = gemmi.find_twin_laws(reference.cell, reference_asu.spacegroup, max_obliq=3, all_ops=False)
+    if len(alt_ops) == 0:
+        print("No ambiguity for this spacegroup! No need to reindex!")
+        return None
+    else:
+        try_ops = unit_ops + alt_ops
+
+    # Reindex each input MTZ file with all possible ops
+    reindexed_record = []
     for input_file in tqdm(input_files):
         try:
             # Read the input MTZ file
-            input_df = rs.read_mtz(input_file)[['F-obs', 'SIGF-obs']]
-            symop1_asu = input_df.apply_symop(gemmi.Op("x,y,z")).hkl_to_asu()
-            symop2_asu = input_df.apply_symop(gemmi.Op("-x,-y,z")).hkl_to_asu()
-
-            # Merge with reference MTZ file
-            merged1 = reference_asu.merge(symop1_asu, left_index=True, right_index=True, suffixes=('_ref', '_input'), check_isomorphous=False)
-            merged2 = reference_asu.merge(symop2_asu, left_index=True, right_index=True, suffixes=('_ref', '_input'), check_isomorphous=False)
-            
-            # Compute correlations
-            corr_ref_input1 = np.corrcoef(merged1['F-obs_ref'], merged1['F-obs_input'])[0][1]
-            corr_ref_input2 = np.corrcoef(merged2['F-obs_ref'], merged2['F-obs_input'])[0][1]
-            # Choose the better correlation and write the reindexed file
-            if corr_ref_input1 > corr_ref_input2:
-                output_file = os.path.join(output_folder, os.path.basename(input_file))
-                symop1_asu.write_mtz(output_file)
-            else:
-                output_file = os.path.join(output_folder, os.path.basename(input_file))
-                symop2_asu.write_mtz(output_file)
-                reindexed_files.append(output_file)
-        except:
+            input_df = rs.read_mtz(input_file)[columns]
+            corr_ref = []
+            for op in try_ops:
+                symopi_asu = input_df.apply_symop(op).hkl_to_asu()
+                mergedi = reference_asu.merge(symopi_asu, left_index=True, right_index=True, suffixes=('_ref', '_input'), check_isomorphous=False)
+                corr_ref.append(np.corrcoef(mergedi[columns[0]+'_ref'], mergedi[columns[0]+'_input'])[0][1])
+            i = np.argmax(corr_ref)
+            output_file = os.path.join(output_folder, os.path.basename(input_file))
+            symopi_asu = input_df.apply_symop(try_ops[i]).hkl_to_asu()
+            symopi_asu.write_mtz(output_file)
+            reindexed_record.append([i,output_file]) # if i == 0, no reindex
+        except Exception as e:
+            print(input_file + e)
             continue
-    with open(os.path.join(output_folder, 'reindexed_files.pkl'), "wb") as f:
+    
+    with open(os.path.join(output_folder, 'reindex_record.pkl'), "wb") as f:
         # Use the pickle module to dump the list to the file
-        pickle.dump(reindexed_files, f)    
+        pickle.dump(reindexed_record, f)    
         
-    return reindexed_files
+    return reindexed_record
```

### Comparing `rs-valdo-0.0.1/valdo/scaling.py` & `rs-valdo-0.0.2/valdo/scaling.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,18 @@
     )
     return args
 
 
 class Scaler(object):
     """
     reference_mtz : path to mtz file as the reference dataset
-    columns : list of columns to be used in downstreaming tasks
+    
+    columns : list of column names to be used
+        The first name is used for scaling, while the remaining 
+        names will be saved as is without any alterations.
     """
     def __init__(self, reference_mtz, columns=['F-obs', 'SIGF-obs']):
         self.columns = columns
         self.base_mtz = rs.read_mtz(reference_mtz)[columns]
         self.base_mtz.dropna(inplace=True)
 
         # Record reciprocal space parameters
@@ -91,30 +94,30 @@
         for path in mtz_path_list:
             start_time = time.time()
             concrete_filename = path.split('/')[-1].replace(".mtz", "") # "PTP1B_yxxx_idxs"
             temp_mtz = rs.read_mtz(path)[self.columns].dropna()
             merge = self.base_mtz.merge(temp_mtz, left_index=True, right_index=True, 
                                         suffixes=('ref', 'target'), check_isomorphous=False)
             
-            FA = merge["F-obsref"].to_numpy()
-            FB = merge["F-obstarget"].to_numpy()
+
+            FA = merge[self.columns[0]+"ref"].to_numpy()
+            FB = merge[self.columns[0]+"target"].to_numpy()
             hkl = merge.get_hkls()
 
             ln_k, uaniso = self.ana_getku(FA, FB, hkl, n_iter=n_iter)
             metric = self.get_metric(FA, FB, uaniso, ln_k, hkl)
-            # TODO: A decent way to save the metric
 
-            FB_complete = temp_mtz["F-obs"].to_numpy() 
+            FB_complete = temp_mtz[self.columns[0]].to_numpy() 
             hkl_complete = temp_mtz.get_hkls()
             
             temp_mtz = temp_mtz.reset_index()
-            temp_mtz['F-obs-scaled'] = rs.DataSeries(self.scaleit(FB_complete, ln_k, uaniso, hkl_complete), dtype="SFAmplitude")
+            temp_mtz[self.columns[0]+'-scaled'] = rs.DataSeries(self.scaleit(FB_complete, ln_k, uaniso, hkl_complete), dtype="SFAmplitude")
             temp_mtz = temp_mtz.set_index(['H', 'K', 'L'])
             # Save the scaled mtz file
-            temp_mtz.write_mtz(outputmtz_path+concrete_filename+"_scaled.mtz")
+            temp_mtz.write_mtz(outputmtz_path+concrete_filename+".mtz")
 
             str_ = f"Time: {time.time()-start_time:.3f}"
             if verbose:
                 print(f"LS before:  {metric[0]:.1f}", f"LS after: {metric[2]:.0f}", flush=True)
                 print(f"Corr before:  {metric[1]:.3f}", f"Corr after: {metric[3]:.3f}", flush=True)
                 print(str_, flush=True)
                 print("="*20)
```

### Comparing `rs-valdo-0.0.1/valdo/vae_basics.py` & `rs-valdo-0.0.2/valdo/vae_basics.py`

 * *Files identical despite different names*

### Comparing `rs-valdo-0.0.1/valdo/vae_networks.py` & `rs-valdo-0.0.2/valdo/vae_networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         elif len(n_hidden_size) == 2:
             self.n_size_encoder = [n_hidden_size[0]]*self.n_layer_encoder
             self.n_size_decoder = [n_hidden_size[1]]*self.n_layer_decoder
         elif len(n_hidden_size) == self.n_layer_encoder+self.n_layer_decoder:
             self.n_size_encoder = n_hidden_size[:self.n_layer_encoder]
             self.n_size_decoder = n_hidden_size[self.n_layer_encoder:]
         else: 
-            raise ValueError("Pleas provide legal n_hidden_size!")
+            raise ValueError("Please provide legal n_hidden_size!")
         
         self.dim_x = n_dim_i
         self.dim_y = n_dim_o
         self.activation = activation
         self.dim_z = n_dim_latent
         self.device = device
```

