# Comparing `tmp/rouskinhf-0.1.2.tar.gz` & `tmp/rouskinhf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouskinhf-0.1.2.tar", last modified: Fri Jul 21 17:26:44 2023, max compression
+gzip compressed data, was "rouskinhf-0.1.3.tar", last modified: Mon Jul 24 19:01:36 2023, max compression
```

## Comparing `rouskinhf-0.1.2.tar` & `rouskinhf-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-21 17:26:44.035824 rouskinhf-0.1.2/
--rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.1.2/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)        3 2023-07-01 06:33:39.000000 rouskinhf-0.1.2/MANIFEST.in
--rw-r--r--   0 ymdt       (501) staff       (20)     5839 2023-07-21 17:26:44.035668 rouskinhf-0.1.2/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)     5388 2023-07-21 17:26:25.000000 rouskinhf-0.1.2/README.md
--rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-21 17:26:41.000000 rouskinhf-0.1.2/pyproject.toml
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-21 17:26:44.034415 rouskinhf-0.1.2/rouskinhf/
--rw-r--r--   0 ymdt       (501) staff       (20)     2433 2023-07-20 01:01:23.000000 rouskinhf-0.1.2/rouskinhf/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    15276 2023-07-21 17:26:25.000000 rouskinhf-0.1.2/rouskinhf/datafolder.py
--rw-r--r--   0 ymdt       (501) staff       (20)     5620 2023-07-07 18:09:01.000000 rouskinhf-0.1.2/rouskinhf/datapoint.py
--rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.1.2/rouskinhf/env.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3136 2023-07-01 05:56:29.000000 rouskinhf-0.1.2/rouskinhf/info_file.py
--rw-r--r--   0 ymdt       (501) staff       (20)    10753 2023-07-21 17:26:25.000000 rouskinhf-0.1.2/rouskinhf/list_datapoints.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3672 2023-07-20 00:05:00.000000 rouskinhf-0.1.2/rouskinhf/parsers.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2608 2023-07-20 00:54:02.000000 rouskinhf-0.1.2/rouskinhf/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6222 2023-07-20 00:54:02.000000 rouskinhf-0.1.2/rouskinhf/rnastructure.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3493 2023-07-20 00:54:02.000000 rouskinhf-0.1.2/rouskinhf/util.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-21 17:26:44.035417 rouskinhf-0.1.2/rouskinhf.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)     5839 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      438 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)      136 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-21 17:26:44.035879 rouskinhf-0.1.2/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      430 2023-07-20 04:08:01.000000 rouskinhf-0.1.2/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:01:36.252481 rouskinhf-0.1.3/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.1.3/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)     5990 2023-07-24 19:01:36.252329 rouskinhf-0.1.3/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)     5539 2023-07-24 18:11:26.000000 rouskinhf-0.1.3/README.md
+-rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-24 18:57:38.000000 rouskinhf-0.1.3/pyproject.toml
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:01:36.251050 rouskinhf-0.1.3/rouskinhf/
+-rw-r--r--   0 ymdt       (501) staff       (20)     2697 2023-07-24 18:42:55.000000 rouskinhf-0.1.3/rouskinhf/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    16168 2023-07-24 18:56:06.000000 rouskinhf-0.1.3/rouskinhf/datafolder.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     8225 2023-07-24 18:55:17.000000 rouskinhf-0.1.3/rouskinhf/datapoint.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.1.3/rouskinhf/env.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3136 2023-07-01 05:56:29.000000 rouskinhf-0.1.3/rouskinhf/info_file.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    10871 2023-07-24 18:43:58.000000 rouskinhf-0.1.3/rouskinhf/list_datapoints.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3648 2023-07-24 18:05:45.000000 rouskinhf-0.1.3/rouskinhf/parsers.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2608 2023-07-20 00:54:02.000000 rouskinhf-0.1.3/rouskinhf/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6222 2023-07-20 00:54:02.000000 rouskinhf-0.1.3/rouskinhf/rnastructure.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3819 2023-07-24 18:55:31.000000 rouskinhf-0.1.3/rouskinhf/util.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:01:36.252079 rouskinhf-0.1.3/rouskinhf.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)     5990 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      426 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)      152 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-24 19:01:36.252530 rouskinhf-0.1.3/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      468 2023-07-24 18:15:00.000000 rouskinhf-0.1.3/setup.py
```

### Comparing `rouskinhf-0.1.2/LICENSE` & `rouskinhf-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.2/PKG-INFO` & `rouskinhf-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -19,14 +19,18 @@
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
     - `.ct`
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
+## Important notes
+
+- Sequences with bases different than `A`, `C`, `G`, `U`, `a`, `c`, `g`, `t`, `u` are not supported. The data will be filtered out.
+
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
 ### Create an environment file
@@ -80,23 +84,23 @@
 
 ### Sourcing the environment and keeping your environment variable secret
 
 The variables defined in the `env` file are required by `rouskinhf`. Make that before you use `rouskinhf`, you run in a terminal:
 
 ```bash
 source env
-``` 
+```
  or, in a Jupyter notebook:
 
 ```python
 !pip install python-dotenv
 %load_ext dotenv
 %dotenv env
 ```
- 
+
  The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
 
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
```

### Comparing `rouskinhf-0.1.2/README.md` & `rouskinhf-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
     - `.ct`
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
+## Important notes
+
+- Sequences with bases different than `A`, `C`, `G`, `U`, `a`, `c`, `g`, `t`, `u` are not supported. The data will be filtered out.
+
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
 ### Create an environment file
@@ -67,23 +71,23 @@
 
 ### Sourcing the environment and keeping your environment variable secret
 
 The variables defined in the `env` file are required by `rouskinhf`. Make that before you use `rouskinhf`, you run in a terminal:
 
 ```bash
 source env
-``` 
+```
  or, in a Jupyter notebook:
 
 ```python
 !pip install python-dotenv
 %load_ext dotenv
 %dotenv env
 ```
- 
+
  The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
 
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
```

### Comparing `rouskinhf-0.1.2/pyproject.toml` & `rouskinhf-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['rouskinhf']
 
 [project]
 name =  "rouskinhf"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to manipulate data for our DMS prediction models."
 readme = "README.md"
 classifiers = [
```

### Comparing `rouskinhf-0.1.2/rouskinhf/__init__.py` & `rouskinhf-0.1.3/rouskinhf/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,20 +30,24 @@
     ndarray
         The dataset with the given name for the given type of data.
 
     Example
     -------
 
     >>> import_dataset(name='for_testing', data='structure').keys()
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     dict_keys(['references', 'sequences', 'structure'])
     >>> import_dataset(name='for_testing', data='DMS').keys()
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     dict_keys(['references', 'sequences', 'DMS'])
     >>> import_dataset(name='for_testing', data='structure', force_download=True).keys()
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     dict_keys(['references', 'sequences', 'structure'])
     >>> import_dataset(name='for_testing', data='DMS', force_download=True).keys()
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     dict_keys(['references', 'sequences', 'DMS'])
 
     """
 
     assert data in ['structure', 'DMS'], "data must be either 'structure' or 'DMS'"
 
     # Get the data folder
```

### Comparing `rouskinhf-0.1.2/rouskinhf/datafolder.py` & `rouskinhf-0.1.3/rouskinhf/datafolder.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ROUSKINLAB = 'rouskinlab/'
 
 class DataFolderTemplate(PathDatafolder):
 
     def __init__(self, name, path_out) -> None:
         super().__init__(name, path_out)
         self.name = name
-        self.datapoints = ListofDatapoints([])
+        self.datapoints = ListofDatapoints([], verbose=False)
 
     def generate_npy(self):
         """Generate the npy files:
             - reference.npy
             - sequence.npy
             - base_pairs.npy
             - dms.npy
@@ -35,14 +35,17 @@
         Each file corresponds to a key in the datapoints dictionary contained in the json file.
         For example, if the 1st line of the json file is:
         {"RF02271.fa.csv_1":{"sequence": "AAACCCCAGUAGGGGUUU", "paired_bases": [[6, 11], [5, 12], [4, 13], [3, 14], [2, 15], [1, 16], [0, 17]], "dms": [0.3317625732102161, 0.8619477949493498, 0.9849505502538177, 0.9997828311396947, 0.9999562120800795, 0.9999454042235505, 0.9970246205212348, 3.298876877182004e-10, 1.0113344525791075e-08, 9.30187856307975e-09, 2.1481183689942838e-10, 0.996953491189411, 0.9999737756512344, 0.9999846271614127, 0.9997971647502685, 0.9848757245213886, 0.8618760196213241, 0.3319091664146036]}}
         then the 1st line of the reference.npy file will be:
         AAACCCCAGUAGGGGUUU
         """
 
+        if not len(self.datapoints.datapoints):
+            return None
+
         self.datapoints.to_reference_npy(self.get_references_npy())
         self.datapoints.to_sequence_npy(self.get_sequences_npy())
 
         d1 = self.datapoints.datapoints[0]
 
         if hasattr(d1, 'paired_bases'):
             self.datapoints.to_base_pairs_npy(self.get_base_pairs_npy())
@@ -91,14 +94,15 @@
         private : bool, optional
             If True, the repo is private. Default is True.
 
         Examples
         --------
 
         >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json')
+        Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
         >>> datafolder.create_repo(exist_ok=True)
 
         """
 
         self.api.create_repo(
             repo_id=ROUSKINLAB+self.name,
             token=HUGGINGFACE_TOKEN,
@@ -129,14 +133,15 @@
         run_as_future : bool, optional
             If True, the upload is run asynchonously. The state of the upload can be checked with the returned future. See sample code. Default is False.
 
         Examples
         --------
 
         >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json')
+        Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
         >>> datafolder.upload_folder('main', 'pytest commit', 'A commit generated by pytest for the upload_folder method')
         >>> future = datafolder.upload_folder(run_as_future=True)
         >>> future.result() # wait for the upload to finish
         'https://huggingface.co/datasets/rouskinlab/dreem_output/tree/main/'
         >>> future.done() # check if the upload is done
         True
 
@@ -196,14 +201,15 @@
         If True, a progress bar is displayed. Default is True.
 
 
     Examples
     --------
 
     >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json', generate_npy=True)
+    Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
     >>> datafolder.name
     'dreem_output'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromDreemOutput
     >>> os.path.isfile(datafolder.get_json())
     True
     """
@@ -238,14 +244,15 @@
         If True, the npy files are generated. Default is True.
 
 
     Examples
     --------
 
     >>> datafolder = DataFolder.from_fasta(path_in='data/input_files_for_testing/sequences.fasta', generate_npy=True)
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     >>> datafolder.name
     'sequences'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromFasta
     >>> os.path.isfile(datafolder.get_json())
     True
     """
@@ -281,14 +288,15 @@
         If True, a progress bar is displayed. Default is True.
 
 
     Examples
     --------
 
     >>> datafolder = DataFolder.from_ct_folder(path_in='data/input_files_for_testing/ct_files', generate_npy=True)
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     >>> datafolder.name
     'ct_files'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromCTfolder
     >>> os.path.isfile(datafolder.get_json())
     True
     """
@@ -324,14 +332,15 @@
         Revision of the datafolder. Default is 'main'.
 
 
     Examples
     --------
 
     >>> datafolder = LoadDatafolderFromHF(name='for_testing', path_out='data/datafolders')
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     >>> datafolder.name
     'for_testing'
     """
 
     def __init__(self, name, path_out, revision='main', tqdm=True) -> None:
         super().__init__(name, path_out)
 
@@ -363,14 +372,15 @@
     path : str
         Path to the folder where the datafolder is saved. Defaut is set in the env variable DATAFOLDER_PATH.
 
     Examples
     --------
 
     >>> datafolder = LoadDatafolderFromLocal(name='for_testing', path='data/datafolders')
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     >>> datafolder.name
     'for_testing'
     """
 
     def __init__(self, name, path) -> None:
         super().__init__(name, path)
 
@@ -402,19 +412,24 @@
 
     tqdm : bool, optional
         If True, a progress bar is displayed. Default is True.
 
     Example
     -------
 
-    >>> datafolder = DataFolder.from_fasta('data/input_files_for_testing/sequences.fasta')
     >>> datafolder = DataFolder.from_dreem_output('data/input_files_for_testing/dreem_output.json')
+    Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
+    >>> datafolder = DataFolder.from_fasta('data/input_files_for_testing/sequences.fasta')
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     >>> datafolder = DataFolder.from_ct_folder('data/input_files_for_testing/ct_files')
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     >>> datafolder = DataFolder.from_huggingface('for_testing')
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     >>> datafolder = DataFolder.from_local('for_testing')
+    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     """
 
     def from_fasta(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True)->CreateDatafolderFromFasta:
         """Create a datafolder from a fasta file. See CreateDatafolderFromFasta for more details."""
         return CreateDatafolderFromFasta(path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm=tqdm)
 
     def from_dreem_output(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, generate_npy = GENERATE_NPY, tqdm=True)->CreateDatafolderFromDreemOutput:
```

### Comparing `rouskinhf-0.1.2/rouskinhf/datapoint.py` & `rouskinhf-0.1.3/rouskinhf/datapoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,58 @@
 
 from typing import Any, List
 from .parsers import *
-from .util import add_braces_if_no_braces, dot2int, int2dot, seq2int
+from .util import add_braces_if_no_braces, dot2int, int2dot, seq2int, standardize_sequence, sequence_has_regular_characters
 import numpy as np
 
 class Datapoint:
 
+    """A datapoint is a data structure where:
+    - reference is the name of the sequence in the fasta file
+    - sequence is a string of A, C, G, U
+    - structure is a string of (, ), .
+    - dms is a list of floats corresponding to the reactivity of each base in the sequence
+    - paired_bases is a list of tuples (i,j) where i and j are paired bases.
+
+
+    Example:
+    >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
+    >>> print(datapoint)
+    "reference":{"sequence": "AACCGG", "paired_bases": [[1, 4], [0, 5]], "dms": [1.0, 2.0, 3.0]}
+    >>> datapoint = Datapoint(reference='reference', sequence='not a valid sequence', structure='((..))')
+    >>> print(datapoint)
+    None
+    """
+
+    def __new__(cls, *args, **kwargs):
+        # Check if the conditions are met before creating the object
+        sequence = kwargs.get('sequence', args[0] if len(args) > 0 else None)
+        if sequence is None:
+            raise ValueError("Object creation aborted: sequence is None.")
+        sequence = standardize_sequence(sequence)
+
+        if not sequence_has_regular_characters(sequence):
+            return None
+
+        # If conditions are met, create and return the new instance
+        instance = super().__new__(cls)
+        return instance
+
     def __init__(self, sequence, reference, structure=None, dms=None, paired_bases=None):
         for attr in [sequence, reference]:
             assert isinstance(attr, str), f"Expected {attr} to be a string, got {type(attr)} instead."
             assert len(attr) > 0, f"Expected {attr} to be non-empty."
+
+        # standardize the sequence
+        sequence = standardize_sequence(sequence)
+
+        if not sequence_has_regular_characters(sequence):
+            raise Exception(f"Sequence {sequence} contains characters other than ACGTUacgtu.")
+
+
         self.reference = reference
         self.sequence = sequence
         self.structure = structure
         self.paired_bases = paired_bases if paired_bases is not None else self.structure_to_paired_bases(structure) if structure is not None else None
         self.dms = dms
         self.opt_dict = {'paired_bases': self.paired_bases, 'dms': self.dms}
 
@@ -67,58 +106,80 @@
     - sequence is a string of A, C, G, U
     - structure is a string of (, ), .
     - dms is a list of floats corresponding to the reactivity of each base in the sequence
 
     """
 
     def __call__(sequence, reference, structure=None, dms=None, predict_structure=False, predict_dms=False):
-        if structure is None and predict_structure:
-            structure = Fasta.predict_structure(sequence)
-        return Datapoint(sequence, reference, structure, dms)
+        sequence = standardize_sequence(sequence)
+
+        if sequence_has_regular_characters(sequence):
+            if structure is None and predict_structure:
+                structure = Fasta.predict_structure(sequence)
+            return Datapoint(sequence, reference, structure, dms)
 
     def from_ct(ct_file, predict_dms):
         """Create a datapoint from a ct file. If predict_dms is True, the dms will be predicted using RNAstructure"""
         reference, sequence, paired_bases = Ct.parse(ct_file)
-        return Datapoint(sequence, reference, paired_bases=paired_bases, dms = Ct.predict_dms(ct_file) if predict_dms else None)
+        sequence = standardize_sequence(sequence)
+
+        if sequence_has_regular_characters(sequence):
+            return Datapoint(sequence, reference, paired_bases=paired_bases, dms = Ct.predict_dms(ct_file) if predict_dms else None)
 
     def from_fasta(sequence, reference, predict_structure, predict_dms):
         """Create a datapoint from a fasta file. The structure and dms will be None."""
-        structure, dms = None, None
-        if predict_structure:
-            structure = Fasta.predict_structure(sequence)
-        if predict_dms:
-            dms = Fasta.predict_dms(sequence)
-        return Datapoint(sequence, reference, structure, dms)
+        sequence = standardize_sequence(sequence)
+
+        if sequence_has_regular_characters(sequence):
+            structure, dms = None, None
+            if predict_structure:
+                structure = Fasta.predict_structure(sequence)
+            if predict_dms:
+                dms = Fasta.predict_dms(sequence)
+            return Datapoint(sequence, reference, structure, dms)
 
     def from_dreem_output(reference, sequence, mutation_rate, predict_structure):
         """Create a datapoint from a dreem output file. The structure and dms will be predicted if predict_structure and predict_dms are True."""
-        return Datapoint(
-            sequence=sequence,
-            reference=reference,
-            structure=Fasta.predict_structure(sequence) if predict_structure else None,
-            dms=mutation_rate)
+        sequence = standardize_sequence(sequence)
+
+        if sequence_has_regular_characters(sequence):
+            return Datapoint(
+                sequence=sequence,
+                reference=reference,
+                structure=Fasta.predict_structure(sequence) if predict_structure else None,
+                dms=mutation_rate)
+        print('DatapointFactory.from_dreem_output: sequence is not valid "{}"'.format(set(sequence) - set('ACGTUacgtu')))
 
 
     def from_json_line(string):
         """Create a datapoint from a json line. The json line should have the following format:
         "reference": {"sequence": "sequence", "paired_bases": [[1, 2], [3,4]], "dms": [1.0, 2.0, 3.0]}
 
         Example:
-        >>> DatapointFactory.from_json_line('"reference": {"sequence": "sequence"}')
-        Datapoint('reference', sequence='sequence', paired_bases=None, dms=None)
-        >>> DatapointFactory.from_json_line('"reference": {"sequence": "sequence", "paired_bases": [[1, 2], [3, 4]], "dms": [1.0, 2.0, 3.0]}')
-        Datapoint('reference', sequence='sequence', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])
+        >>> DatapointFactory.from_json_line('"reference": {"sequence": "ACAAGU"}')
+        Datapoint('reference', sequence='ACAAGU', paired_bases=None, dms=None)
+        >>> DatapointFactory.from_json_line('"reference": {"sequence": "ACAAGU", "paired_bases": [[1, 2], [3, 4]], "dms": [1.0, 2.0, 3.0]}')
+        Datapoint('reference', sequence='ACAAGU', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])
+        >>> DatapointFactory.from_json_line('"reference": {"sequence": "something else than ACGTUacgtu", "paired_bases": [[1, 2], [3, 4]], "dms": [1.0, 2.0, 3.0]}')
         """
+
+        # process the string into a dictionary
         string= string.strip()[:-1] if string.strip()[-1] == ',' else string.strip()
         string = add_braces_if_no_braces(string)
         d = json.loads(string)
         ref = list(d.keys())[0]
         d = d[ref]
-        return Datapoint(
-            reference=ref,
-            sequence=d['sequence'],
-            paired_bases=d['paired_bases'] if 'paired_bases' in d else None,
-            dms=d['dms'] if 'dms' in d else None
-        )
+
+        # create the datapoint
+        sequence = d['sequence']
+        sequence = standardize_sequence(sequence)
+
+        if sequence_has_regular_characters(sequence):
+            return Datapoint(
+                reference=ref,
+                sequence=sequence,
+                paired_bases=d['paired_bases'] if 'paired_bases' in d else None,
+                dms=d['dms'] if 'dms' in d else None
+            )
```

### Comparing `rouskinhf-0.1.2/rouskinhf/env.py` & `rouskinhf-0.1.3/rouskinhf/env.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.2/rouskinhf/info_file.py` & `rouskinhf-0.1.3/rouskinhf/info_file.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.2/rouskinhf/list_datapoints.py` & `rouskinhf-0.1.3/rouskinhf/list_datapoints.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,68 +7,60 @@
 from typing import List, Tuple, Union, Optional
 from .parsers import Fasta, DreemOutput
 import pandas as pd
 from tqdm import tqdm as tqdm_parser
 
 class ListofDatapoints:
 
-    def __init__(self, datapoints):
-        self.datapoints = datapoints
+    def __init__(self, datapoints, verbose=True):
+        self.datapoints = list(filter(lambda x: x is not None, datapoints))
+        if verbose:
+            print(f"Loaded {len(self.datapoints)} valid datapoints, filtered out {len(datapoints)-len(self.datapoints)} invalid datapoints.")
 
     def __call__(self) -> List[Datapoint]:
         return self.datapoints
 
     @classmethod
     def from_fasta(cls, fasta_file, predict_structure, predict_dms, tqdm=True):
         """Create a list of datapoint from a fasta file. The structure and dms will be predicted if predict_structure and predict_dms are True."""
         sequences, references = Fasta.parse(fasta_file)
-        if tqdm:
-            return cls([DatapointFactory.from_fasta(sequence, reference, predict_structure, predict_dms)
-                    for sequence, reference in tqdm_parser(zip(sequences, references), total=len(sequences), desc='Parsing fasta file')])
         return cls([DatapointFactory.from_fasta(sequence, reference, predict_structure, predict_dms)
-                    for sequence, reference in zip(sequences, references)])
+                    for sequence, reference in tqdm_parser(zip(sequences, references), total=len(sequences), desc='Parsing fasta file', disable=not tqdm)])
 
     @classmethod
     def from_ct(cls, ct_files, predict_dms, tqdm=True):
         """Create a list of datapoint from a ct file. The dms will be predicted if predict_dms is True."""
-        if tqdm:
-            return cls([DatapointFactory.from_ct(ct_file, predict_dms) for ct_file in tqdm_parser(ct_files, total=len(ct_files), desc='Parsing ct files')])
-        return cls([DatapointFactory.from_ct(ct_file, predict_dms) for ct_file in ct_files])
+        return cls([DatapointFactory.from_ct(ct_file, predict_dms) for ct_file in tqdm_parser(ct_files, total=len(ct_files), desc='Parsing ct files', disable=not tqdm)])
 
     @classmethod
     def from_dreem_output(cls, dreem_output_file, predict_structure, tqdm):
         """Create a list of datapoint from a dreem output file. The structure and dms will be predicted if predict_structure and predict_dms are True."""
-        print('Parsing dreem output file')
-        if tqdm:
-            n_lines = len(list(DreemOutput.parse(dreem_output_file)))
-            return cls([DatapointFactory.from_dreem_output(reference, sequence, mutation_rate, predict_structure)
-            for reference, sequence, mutation_rate in tqdm_parser(DreemOutput.parse(dreem_output_file), total=n_lines, desc='Parsing dreem output file')])
+        n_lines = len(list(DreemOutput.parse(dreem_output_file)))
         return cls([DatapointFactory.from_dreem_output(reference, sequence, mutation_rate, predict_structure)
-            for reference, sequence, mutation_rate in DreemOutput.parse(dreem_output_file)])
+            for reference, sequence, mutation_rate in tqdm_parser(DreemOutput.parse(dreem_output_file), total=n_lines, desc='Parsing dreem output file', disable=not tqdm)])
 
     @classmethod
     def from_json(cls, json_file, tqdm=True):
         """Create a list of datapoint from a json file."""
         with open(json_file) as f:
-            if tqdm:
-                return cls([DatapointFactory.from_json_line(line) for line in tqdm_parser(f, total=sum(1 for line in open(json_file) if line.strip() not in ['{', '}']), desc='Parsing json file') if line.strip() not in ['{', '}']])
-            return cls([DatapointFactory.from_json_line(line) for line in f if line.strip() not in ['{', '}']])
+            return cls([DatapointFactory.from_json_line(line) for line in tqdm_parser(f, total=sum(1 for line in open(json_file) if line.strip() not in ['{', '}']), desc='Parsing json file', disable= not tqdm) if line.strip() not in ['{', '}']])
 
 
     def to_base_pairs_npy(self, path):
         """Writes the structure npy file from the list of datapoints.
 
         Args:
             path (str): path to the npy file
 
         Returns:
             np.array: structure matrix of pairs of 0-based indices.
 
         Examples:
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
+            Loaded 1 valid datapoints, filtered out 0 invalid datapoints.
             >>> datapoints.to_base_pairs_npy('temp/base_pairs.npy')
             array([[[1, 2],
                     [3, 4]]], dtype=object)
         """
 
         arr = np.array([np.array(datapoint.paired_bases) for datapoint in self.datapoints], dtype=object)
         np.save(path, arr)
@@ -82,14 +74,15 @@
             path (str): path to the npy file
 
         Returns:
             np.array: dms matrix of floats arrays.
 
         Examples:
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
+            Loaded 1 valid datapoints, filtered out 0 invalid datapoints.
             >>> datapoints.to_dms_npy('temp/dms.npy')
             array([[1.0, 2.0, 3.0]], dtype=object)
         """
 
         arr = np.array([datapoint.dms for datapoint in self.datapoints], dtype=object)
         np.save(path, arr)
         return arr
@@ -103,14 +96,15 @@
 
         Returns:
             np.array: int-encoded sequence matrix
 
         Examples:
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0]),\
                                                Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
+            Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
             >>> datapoints.to_sequence_npy('temp/sequence.npy')
             array([[1, 1, 2, 2, 3, 3],
                    [1, 1, 2, 2, 3, 3]], dtype=object)
         """
 
         arr = np.array([datapoint.embed_sequence() for datapoint in self.datapoints], dtype=object)
         np.save(path, arr)
@@ -124,14 +118,15 @@
             path (str): path to the npy file
 
         Returns:
             np.array: reference matrix of int-encoded.
 
         Examples:
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
+            Loaded 1 valid datapoints, filtered out 0 invalid datapoints.
             >>> datapoints.to_reference_npy('temp/reference.npy')
             array(['reference'], dtype='<U9')
         """
 
         arr = np.array([datapoint.reference for datapoint in self.datapoints])
         np.save(path, arr)
         return arr
@@ -147,14 +142,15 @@
             f.write('}\n')
 
     def to_pandas(self) -> pd.DataFrame:
         """Converts the list of datapoints into a pandas dataframe.
 
         Example:
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
+            Loaded 1 valid datapoints, filtered out 0 invalid datapoints.
             >>> datapoints.to_pandas()
                reference sequence      paired_bases              dms
             0  reference   AACCGG  [[1, 2], [3, 4]]  [1.0, 2.0, 3.0]
         """
         return pd.DataFrame([datapoint.to_flat_dict() for datapoint in self.datapoints])
 
     def filter_duplicates(self):
@@ -163,18 +159,19 @@
 
         Examples:
             >>> datapoints = ListofDatapoints([ Datapoint(reference='ref1', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0,0,0,0,0,0]),\
                                 Datapoint(reference='ref2', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0,0,0,0,0,0]),\
                                 Datapoint(reference='ref3', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0,0,0,0,0,0]),\
                                 Datapoint(reference='ref4', sequence='AUGGC', paired_bases=[[1, 2]], dms=[0,0,0,0,0]),\
                                 Datapoint(reference='ref5', sequence='GCCUA', paired_bases=[[0, 4], [2, 3]], dms=[0,0,0,0,0]),\
-                                Datapoint(reference='ref6', sequence='GCCUA', paired_bases=[[0, 4]], dms=[0,0,0,0,0]) ])
+                                Datapoint(reference='ref6', sequence='not a regular sequence', paired_bases=[[0, 4]], dms=[0,0,0,0,0]) ])
+            Loaded 5 valid datapoints, filtered out 1 invalid datapoints.
             >>> datapoints.filter_duplicates()
             >>> datapoints.datapoints
-            [Datapoint('ref1', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0, 0, 0, 0, 0, 0]), Datapoint('ref4', sequence='AUGGC', paired_bases=[[1, 2]], dms=[0, 0, 0, 0, 0])]
+            [Datapoint('ref1', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0, 0, 0, 0, 0, 0]), Datapoint('ref4', sequence='AUGGC', paired_bases=[[1, 2]], dms=[0, 0, 0, 0, 0]), Datapoint('ref5', sequence='GCCUA', paired_bases=[[0, 4], [2, 3]], dms=[0, 0, 0, 0, 0])]
         """
 
         # Group datapoints by sequence
         unique_seqs = {}
         for i, datapoint in enumerate(self.datapoints):
 
             struct = np.array(datapoint.paired_bases)
```

### Comparing `rouskinhf-0.1.2/rouskinhf/parsers.py` & `rouskinhf-0.1.3/rouskinhf/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os, json
 import numpy as np
 from .rnastructure import RNAstructure
 from .util import DreemUtils
 import pandas as pd
 
+
 class Ct:
     def parse(ct_file):
         """Parse a ct file and return the sequence and structure
 
         Args:
             ct_file (str): path to ct file
 
@@ -24,15 +25,16 @@
             if line.strip() == '':
                 break
             utr5, base, _, _, utr3, _ = line.split()
             sequence += base
             if int(utr3) > int(utr5) and int(utr3) != 0:
                 paired_bases.append([int(utr5)-1, int(utr3)-1])
 
-        return Ct.get_reference_from_title(ct_file), sequence.upper().replace('T', 'U'), paired_bases
+        return Ct.get_reference_from_title(ct_file), sequence, paired_bases
+
 
     def parse_list(ct_files):
         """Parse a list of ct files and return the sequences and structures"""
         return [Ct.parse(ct_file) for ct_file in ct_files]
 
     def get_reference_from_title(ct_file):
         return os.path.basename(ct_file).split('.')[0]
```

### Comparing `rouskinhf-0.1.2/rouskinhf/path.py` & `rouskinhf-0.1.3/rouskinhf/path.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.2/rouskinhf/rnastructure.py` & `rouskinhf-0.1.3/rouskinhf/rnastructure.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.2/rouskinhf/util.py` & `rouskinhf-0.1.3/rouskinhf/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,7 +117,18 @@
         mut_profiles = {k:mut_profiles[k] for k in sorted(mut_profiles)}
         mut_profiles = dict(sorted(mut_profiles.items(), key=sorting_key))
         for k, v in mut_profiles.items():
             if type(v) is not dict:
                 continue
             mut_profiles[k] = DreemUtils.sort_dict(v)
         return mut_profiles
+
+
+def standardize_sequence(sequence):
+    sequence = sequence.upper()
+    sequence = sequence.replace('T', 'U')
+    # trim the sequence
+    sequence = sequence.replace(' ', '').replace('\n', '').replace('\t', '')
+    return sequence
+
+def sequence_has_regular_characters(sequence):
+    return not (set(sequence) - set('ACGUN'))
```

### Comparing `rouskinhf-0.1.2/rouskinhf.egg-info/PKG-INFO` & `rouskinhf-0.1.3/rouskinhf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -19,14 +19,18 @@
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
     - `.ct`
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
+## Important notes
+
+- Sequences with bases different than `A`, `C`, `G`, `U`, `a`, `c`, `g`, `t`, `u` are not supported. The data will be filtered out.
+
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
 ### Create an environment file
@@ -80,23 +84,23 @@
 
 ### Sourcing the environment and keeping your environment variable secret
 
 The variables defined in the `env` file are required by `rouskinhf`. Make that before you use `rouskinhf`, you run in a terminal:
 
 ```bash
 source env
-``` 
+```
  or, in a Jupyter notebook:
 
 ```python
 !pip install python-dotenv
 %load_ext dotenv
 %dotenv env
 ```
- 
+
  The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
 
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
```

