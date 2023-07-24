# Comparing `tmp/rouskinhf-0.1.3.tar.gz` & `tmp/rouskinhf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouskinhf-0.1.3.tar", last modified: Mon Jul 24 19:01:36 2023, max compression
+gzip compressed data, was "rouskinhf-0.1.4.tar", last modified: Mon Jul 24 19:26:20 2023, max compression
```

## Comparing `rouskinhf-0.1.3.tar` & `rouskinhf-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:01:36.252481 rouskinhf-0.1.3/
--rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.1.3/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)     5990 2023-07-24 19:01:36.252329 rouskinhf-0.1.3/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)     5539 2023-07-24 18:11:26.000000 rouskinhf-0.1.3/README.md
--rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-24 18:57:38.000000 rouskinhf-0.1.3/pyproject.toml
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:01:36.251050 rouskinhf-0.1.3/rouskinhf/
--rw-r--r--   0 ymdt       (501) staff       (20)     2697 2023-07-24 18:42:55.000000 rouskinhf-0.1.3/rouskinhf/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    16168 2023-07-24 18:56:06.000000 rouskinhf-0.1.3/rouskinhf/datafolder.py
--rw-r--r--   0 ymdt       (501) staff       (20)     8225 2023-07-24 18:55:17.000000 rouskinhf-0.1.3/rouskinhf/datapoint.py
--rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.1.3/rouskinhf/env.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3136 2023-07-01 05:56:29.000000 rouskinhf-0.1.3/rouskinhf/info_file.py
--rw-r--r--   0 ymdt       (501) staff       (20)    10871 2023-07-24 18:43:58.000000 rouskinhf-0.1.3/rouskinhf/list_datapoints.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3648 2023-07-24 18:05:45.000000 rouskinhf-0.1.3/rouskinhf/parsers.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2608 2023-07-20 00:54:02.000000 rouskinhf-0.1.3/rouskinhf/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6222 2023-07-20 00:54:02.000000 rouskinhf-0.1.3/rouskinhf/rnastructure.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3819 2023-07-24 18:55:31.000000 rouskinhf-0.1.3/rouskinhf/util.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:01:36.252079 rouskinhf-0.1.3/rouskinhf.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)     5990 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      426 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)      152 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-24 19:01:36.000000 rouskinhf-0.1.3/rouskinhf.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-24 19:01:36.252530 rouskinhf-0.1.3/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      468 2023-07-24 18:15:00.000000 rouskinhf-0.1.3/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:26:20.579578 rouskinhf-0.1.4/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.1.4/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)     6005 2023-07-24 19:26:20.579427 rouskinhf-0.1.4/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)     5554 2023-07-24 19:06:17.000000 rouskinhf-0.1.4/README.md
+-rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-24 19:17:23.000000 rouskinhf-0.1.4/pyproject.toml
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:26:20.578356 rouskinhf-0.1.4/rouskinhf/
+-rw-r--r--   0 ymdt       (501) staff       (20)     2697 2023-07-24 18:42:55.000000 rouskinhf-0.1.4/rouskinhf/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    16973 2023-07-24 19:24:00.000000 rouskinhf-0.1.4/rouskinhf/datafolder.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     8225 2023-07-24 18:55:17.000000 rouskinhf-0.1.4/rouskinhf/datapoint.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.1.4/rouskinhf/env.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3467 2023-07-24 19:25:13.000000 rouskinhf-0.1.4/rouskinhf/info_file.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    10871 2023-07-24 18:43:58.000000 rouskinhf-0.1.4/rouskinhf/list_datapoints.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3648 2023-07-24 18:05:45.000000 rouskinhf-0.1.4/rouskinhf/parsers.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2608 2023-07-20 00:54:02.000000 rouskinhf-0.1.4/rouskinhf/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6222 2023-07-20 00:54:02.000000 rouskinhf-0.1.4/rouskinhf/rnastructure.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3819 2023-07-24 18:55:31.000000 rouskinhf-0.1.4/rouskinhf/util.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:26:20.579201 rouskinhf-0.1.4/rouskinhf.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)     6005 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      426 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)      152 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-24 19:26:20.579628 rouskinhf-0.1.4/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      468 2023-07-24 18:15:00.000000 rouskinhf-0.1.4/setup.py
```

### Comparing `rouskinhf-0.1.3/LICENSE` & `rouskinhf-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/PKG-INFO` & `rouskinhf-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -21,15 +21,15 @@
     - `.fasta`
     - `.ct`
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
 ## Important notes
 
-- Sequences with bases different than `A`, `C`, `G`, `U`, `a`, `c`, `g`, `t`, `u` are not supported. The data will be filtered out.
+- Sequences with bases different than `A`, `C`, `G`, `T`, `U`, `N`, `a`, `c`, `g`, `t`, `u`, `n` are not supported. The data will be filtered out.
 
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
```

### Comparing `rouskinhf-0.1.3/README.md` & `rouskinhf-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     - `.fasta`
     - `.ct`
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
 ## Important notes
 
-- Sequences with bases different than `A`, `C`, `G`, `U`, `a`, `c`, `g`, `t`, `u` are not supported. The data will be filtered out.
+- Sequences with bases different than `A`, `C`, `G`, `T`, `U`, `N`, `a`, `c`, `g`, `t`, `u`, `n` are not supported. The data will be filtered out.
 
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
```

### Comparing `rouskinhf-0.1.3/pyproject.toml` & `rouskinhf-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['rouskinhf']
 
 [project]
 name =  "rouskinhf"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to manipulate data for our DMS prediction models."
 readme = "README.md"
 classifiers = [
```

### Comparing `rouskinhf-0.1.3/rouskinhf/__init__.py` & `rouskinhf-0.1.4/rouskinhf/__init__.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/rouskinhf/datafolder.py` & `rouskinhf-0.1.4/rouskinhf/datafolder.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,20 +134,30 @@
             If True, the upload is run asynchonously. The state of the upload can be checked with the returned future. See sample code. Default is False.
 
         Examples
         --------
 
         >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json')
         Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
+        >>> datafolder.create_repo(exist_ok=True)
         >>> datafolder.upload_folder('main', 'pytest commit', 'A commit generated by pytest for the upload_folder method')
         >>> future = datafolder.upload_folder(run_as_future=True)
         >>> future.result() # wait for the upload to finish
         'https://huggingface.co/datasets/rouskinlab/dreem_output/tree/main/'
         >>> future.done() # check if the upload is done
         True
+        >>> datafolder = DataFolder.from_ct_folder(path_in='data/input_files_for_testing/ct_files')
+        Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
+        >>> datafolder.create_repo(exist_ok=True)
+        >>> datafolder.upload_folder('main', 'pytest commit', 'A commit generated by pytest for the upload_folder method')
+        >>> future = datafolder.upload_folder(run_as_future=True)
+        >>> datafolder = DataFolder.from_fasta(path_in='data/input_files_for_testing/sequences.fasta')
+        Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
+        >>> datafolder.create_repo(exist_ok=True)
+        >>> datafolder.upload_folder('main', 'pytest commit', 'A commit generated by pytest for the upload_folder method')
 
         """
 
         future = self.api.upload_folder(
             repo_id=ROUSKINLAB+self.name,
             folder_path=self.get_main_folder(),
             repo_type="dataset",
```

### Comparing `rouskinhf-0.1.3/rouskinhf/datapoint.py` & `rouskinhf-0.1.4/rouskinhf/datapoint.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/rouskinhf/env.py` & `rouskinhf-0.1.4/rouskinhf/env.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/rouskinhf/info_file.py` & `rouskinhf-0.1.4/rouskinhf/info_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,44 +63,47 @@
         file = json.load(open(path_in, 'r'))
         if 'user' in file:
             file['experimenter'] = file.pop('user')
         for k, v in file.items():
             if type(v) != dict:
                 self.info[k] = v
 
+        self.info['source'] = "`{}` (DREEM output format)".format(os.path.basename(path_in))
         self.info['structure'] = STRUCTURE_FROM_RNASTRUCTURE
         self.info['about structure'] = 'Predicted using RNAstructure and the DMS reactivity data.'
         self.info['DMS'] = DMS_FROM_SOURCE
         self.info['about DMS'] = 'Measured experimentally using the attached experimental conditions.'
 
 
 class InfoFileWriterFromCT(InfoFileWriterTemplate):
 
-    def __init__(self, name, root) -> None:
+    def __init__(self, name, root, path_in) -> None:
         super().__init__(name, root)
 
+        self.info['source'] = "`{}` (CT files format)".format(os.path.basename(path_in))
         self.info['structure'] = STRUCTURE_FROM_SOURCE
         self.info['about structure'] = 'Read from source.'
         self.info['DMS'] = DMS_FROM_RNASTRUCTURE
         self.info['about DMS'] = 'Predicted using RNAstructure at 310K.'
 
 
 class InfoFileWriterFromFasta(InfoFileWriterTemplate):
 
-    def __init__(self, name, root) -> None:
+    def __init__(self, name, root, path_in) -> None:
         super().__init__(name, root)
 
+        self.info['source'] = "`{}` (fasta file format)".format(os.path.basename(path_in))
         self.info['structure'] = STRUCTURE_FROM_RNASTRUCTURE
         self.info['about structure'] = 'Predicted using RNAstructure at 310K.'
         self.info['DMS'] = DMS_FROM_RNASTRUCTURE
         self.info['about DMS'] = 'Predicted using RNAstructure at 310K.'
 
 
 def infoFileWriter(source, datafolder):
     if source == 'dreem_output':
         return InfoFileWriterFromDREEMoutput(datafolder.name, datafolder.path_out, datafolder.path_in)
     if source == 'ct':
-        return InfoFileWriterFromCT(datafolder.name, datafolder.path_out)
+        return InfoFileWriterFromCT(datafolder.name, datafolder.path_out, datafolder.path_in)
     if source == 'fasta':
-        return InfoFileWriterFromFasta(datafolder.name, datafolder.path_out)
+        return InfoFileWriterFromFasta(datafolder.name, datafolder.path_out, datafolder.path_in)
     raise ValueError(f"Unknown source: {source}")
```

### Comparing `rouskinhf-0.1.3/rouskinhf/list_datapoints.py` & `rouskinhf-0.1.4/rouskinhf/list_datapoints.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/rouskinhf/parsers.py` & `rouskinhf-0.1.4/rouskinhf/parsers.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/rouskinhf/path.py` & `rouskinhf-0.1.4/rouskinhf/path.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/rouskinhf/rnastructure.py` & `rouskinhf-0.1.4/rouskinhf/rnastructure.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/rouskinhf/util.py` & `rouskinhf-0.1.4/rouskinhf/util.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.3/rouskinhf.egg-info/PKG-INFO` & `rouskinhf-0.1.4/rouskinhf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -21,15 +21,15 @@
     - `.fasta`
     - `.ct`
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
 ## Important notes
 
-- Sequences with bases different than `A`, `C`, `G`, `U`, `a`, `c`, `g`, `t`, `u` are not supported. The data will be filtered out.
+- Sequences with bases different than `A`, `C`, `G`, `T`, `U`, `N`, `a`, `c`, `g`, `t`, `u`, `n` are not supported. The data will be filtered out.
 
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
```

