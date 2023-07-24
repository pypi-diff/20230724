# Comparing `tmp/MEGNetSparse-0.0.6.tar.gz` & `tmp/megnetsparse-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGNetSparse-0.0.6.tar", last modified: Tue Jul 18 22:03:21 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `MEGNetSparse-0.0.6.tar` & `megnetsparse-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,22 @@
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 22:03:21.886739 MEGNetSparse-0.0.6/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.6/.gitignore
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     1091 2023-07-05 16:12:03.000000 MEGNetSparse-0.0.6/LICENSE
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 22:03:21.197950 MEGNetSparse-0.0.6/MEGNetSparse/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      120 2023-07-03 18:52:42.000000 MEGNetSparse-0.0.6/MEGNetSparse/__init__.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5423 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.6/MEGNetSparse/dense2sparse.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3586 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.6/MEGNetSparse/eos.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5105 2023-06-03 16:16:46.000000 MEGNetSparse-0.0.6/MEGNetSparse/layers.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     1878 2023-07-13 07:21:34.000000 MEGNetSparse-0.0.6/MEGNetSparse/losses.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3015 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.6/MEGNetSparse/model.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     6891 2023-06-03 16:26:00.000000 MEGNetSparse-0.0.6/MEGNetSparse/struct2graph.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     8080 2023-07-18 22:02:31.000000 MEGNetSparse-0.0.6/MEGNetSparse/trainer.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      885 2023-06-18 16:37:50.000000 MEGNetSparse-0.0.6/MEGNetSparse/utils.py
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 22:03:21.444744 MEGNetSparse-0.0.6/MEGNetSparse.egg-info/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-18 22:03:20.000000 MEGNetSparse-0.0.6/MEGNetSparse.egg-info/PKG-INFO
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      635 2023-07-18 22:03:20.000000 MEGNetSparse-0.0.6/MEGNetSparse.egg-info/SOURCES.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        1 2023-07-18 22:03:20.000000 MEGNetSparse-0.0.6/MEGNetSparse.egg-info/dependency_links.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       27 2023-07-18 22:03:20.000000 MEGNetSparse-0.0.6/MEGNetSparse.egg-info/requires.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       13 2023-07-18 22:03:20.000000 MEGNetSparse-0.0.6/MEGNetSparse.egg-info/top_level.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-18 22:03:21.877958 MEGNetSparse-0.0.6/PKG-INFO
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2536 2023-07-05 16:00:57.000000 MEGNetSparse-0.0.6/README.md
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 22:03:21.622279 MEGNetSparse-0.0.6/examples/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       19 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.6/examples/.gitignore
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      812 2023-06-05 21:35:25.000000 MEGNetSparse-0.0.6/examples/MoS2.cif
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      814 2022-09-29 08:35:52.000000 MEGNetSparse-0.0.6/examples/WSe2.cif
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    13944 2022-04-12 22:15:21.000000 MEGNetSparse-0.0.6/examples/descriptors.csv
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    15149 2023-07-03 19:04:43.000000 MEGNetSparse-0.0.6/examples/example.ipynb
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       82 2023-06-05 21:35:26.000000 MEGNetSparse-0.0.6/examples/initial_structures.csv
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 22:03:21.783903 MEGNetSparse-0.0.6/examples/pilot/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)   148416 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.6/examples/pilot/data.pickle.gz
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    10925 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.6/examples/pilot/targets.csv.gz
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      437 2023-07-18 22:02:42.000000 MEGNetSparse-0.0.6/pyproject.toml
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-18 22:03:21.890084 MEGNetSparse-0.0.6/setup.cfg
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/__init__.py
+-rwxr-xr-x   0        0        0     5423 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/dense2sparse.py
+-rwxr-xr-x   0        0        0     3586 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/eos.py
+-rwxr-xr-x   0        0        0     5105 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/layers.py
+-rwxr-xr-x   0        0        0     1878 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/losses.py
+-rwxr-xr-x   0        0        0     3015 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/model.py
+-rwxr-xr-x   0        0        0     6891 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/struct2graph.py
+-rwxr-xr-x   0        0        0     8040 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/trainer.py
+-rwxr-xr-x   0        0        0      885 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/MEGNetSparse/utils.py
+-rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/examples/.gitignore
+-rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/examples/MoS2.cif
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/examples/WSe2.cif
+-rwxr-xr-x   0        0        0    13944 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/examples/descriptors.csv
+-rwxr-xr-x   0        0        0    15149 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/examples/example.ipynb
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/examples/initial_structures.csv
+-rwxr-xr-x   0        0        0   148416 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/examples/pilot/data.pickle.gz
+-rwxr-xr-x   0        0        0    10925 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/examples/pilot/targets.csv.gz
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/.gitignore
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/LICENSE
+-rwxr-xr-x   0        0        0     2536 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/README.md
+-rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 megnetsparse-0.0.8/PKG-INFO
```

### Comparing `MEGNetSparse-0.0.6/LICENSE` & `megnetsparse-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse/dense2sparse.py` & `megnetsparse-0.0.8/MEGNetSparse/dense2sparse.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse/eos.py` & `megnetsparse-0.0.8/MEGNetSparse/eos.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse/layers.py` & `megnetsparse-0.0.8/MEGNetSparse/layers.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse/losses.py` & `megnetsparse-0.0.8/MEGNetSparse/losses.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse/model.py` & `megnetsparse-0.0.8/MEGNetSparse/model.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse/struct2graph.py` & `megnetsparse-0.0.8/MEGNetSparse/struct2graph.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse/trainer.py` & `megnetsparse-0.0.8/MEGNetSparse/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
         if train_weights is not None:
             self.sampler = WeightedRandomSampler(torch.tensor(train_weights).float(), len(train_weights))
 
         self.trainloader = DataLoader(
             self.train_structures,
             batch_size=self.config["model"]["train_batch_size"],
-            shuffle=False if train_weights is not None else True,
+            shuffle=True,
             num_workers=0,
             sampler=self.sampler if train_weights is not None else None
         )
 
         self.testloader = DataLoader(
             self.test_structures,
             batch_size=self.config["model"]["test_batch_size"],
```

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse/utils.py` & `megnetsparse-0.0.8/MEGNetSparse/utils.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/MEGNetSparse.egg-info/PKG-INFO` & `megnetsparse-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: MEGNetSparse
-Version: 0.0.6
-Author-email: Romanov Ignat <romanov.ignat.p@gmail.com>
+Version: 0.0.8
 Project-URL: Homepage, https://github.com/RomanovIgnat/MEGNet_pytorch_test
+Author-email: Romanov Ignat <romanov.ignat.p@gmail.com>
+License-File: LICENSE
 Requires-Python: >=3.8
+Requires-Dist: joblib
+Requires-Dist: numpy
+Requires-Dist: pymatgen
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # MEGNetSparse
 
 ### Installation
 
 ```
 pip install MEGNetSparse
```

### Comparing `MEGNetSparse-0.0.6/README.md` & `megnetsparse-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/examples/MoS2.cif` & `megnetsparse-0.0.8/examples/MoS2.cif`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/examples/WSe2.cif` & `megnetsparse-0.0.8/examples/WSe2.cif`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/examples/descriptors.csv` & `megnetsparse-0.0.8/examples/descriptors.csv`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/examples/example.ipynb` & `megnetsparse-0.0.8/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/examples/pilot/data.pickle.gz` & `megnetsparse-0.0.8/examples/pilot/data.pickle.gz`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.6/examples/pilot/targets.csv.gz` & `megnetsparse-0.0.8/examples/pilot/targets.csv.gz`

 * *Files identical despite different names*

