# Comparing `tmp/ciderpolarity-0.2.8.tar.gz` & `tmp/ciderpolarity-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciderpolarity-0.2.8.tar", max compression
+gzip compressed data, was "ciderpolarity-0.2.9.tar", max compression
```

## Comparing `ciderpolarity-0.2.8.tar` & `ciderpolarity-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.8/LICENSE
--rw-r--r--   0        0        0     5197 2023-07-18 07:56:43.733452 ciderpolarity-0.2.8/README.md
--rw-r--r--   0        0        0     9387 2023-07-13 12:33:45.157234 ciderpolarity-0.2.8/ciderpolarity/CIDER.py
--rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.8/ciderpolarity/__init__.py
--rw-r--r--   0        0        0     3260 2023-07-13 12:14:50.023897 ciderpolarity-0.2.8/ciderpolarity/create_embeddings.py
--rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.8/ciderpolarity/create_vader.py
--rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.8/ciderpolarity/load_polarities.py
--rw-r--r--   0        0        0     5331 2023-07-13 12:14:41.635977 ciderpolarity-0.2.8/ciderpolarity/run_bootstrapping.py
--rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.8/ciderpolarity/stopwords.py
--rw-r--r--   0        0        0     4995 2023-07-24 10:05:05.417122 ciderpolarity-0.2.8/ciderpolarity/suggest_seeds.py
--rw-r--r--   0        0        0     1181 2023-07-13 12:14:28.216105 ciderpolarity-0.2.8/ciderpolarity/utils_funcs.py
--rw-r--r--   0        0        0      518 2023-07-24 10:06:14.272474 ciderpolarity-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 ciderpolarity-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5197 2023-07-18 07:56:43.733452 ciderpolarity-0.2.9/README.md
+-rw-r--r--   0        0        0     9464 2023-07-24 10:21:35.250631 ciderpolarity-0.2.9/ciderpolarity/CIDER.py
+-rw-r--r--   0        0        0      204 2023-07-24 10:21:00.550984 ciderpolarity-0.2.9/ciderpolarity/__init__.py
+-rw-r--r--   0        0        0     3260 2023-07-13 12:14:50.023897 ciderpolarity-0.2.9/ciderpolarity/create_embeddings.py
+-rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.9/ciderpolarity/create_vader.py
+-rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.9/ciderpolarity/load_polarities.py
+-rw-r--r--   0        0        0     5331 2023-07-13 12:14:41.635977 ciderpolarity-0.2.9/ciderpolarity/run_bootstrapping.py
+-rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.9/ciderpolarity/stopwords.py
+-rw-r--r--   0        0        0     4995 2023-07-24 10:05:05.417122 ciderpolarity-0.2.9/ciderpolarity/suggest_seeds.py
+-rw-r--r--   0        0        0     1181 2023-07-13 12:14:28.216105 ciderpolarity-0.2.9/ciderpolarity/utils_funcs.py
+-rw-r--r--   0        0        0      518 2023-07-24 10:21:52.670454 ciderpolarity-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 ciderpolarity-0.2.9/PKG-INFO
```

### Comparing `ciderpolarity-0.2.8/LICENSE` & `ciderpolarity-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/README.md` & `ciderpolarity-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/ciderpolarity/CIDER.py` & `ciderpolarity-0.2.9/ciderpolarity/CIDER.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .suggest_seeds import set_seeds, custom_seeds, seed_dict
 from .stopwords import stoplist
 from . import load_polarities
 from . import create_embeddings
 from . import run_bootstrapping
 from . import create_vader
 from . import utils_funcs
+from . import __version__
 import warnings
 import pickle
 import os
 
 
 
 
@@ -62,14 +63,16 @@
                                     ONLY WORKS WITH "preprocessing = 'default'"
         iterations - INT - the number of iterations for label propagation 
 
         verbose - BOOL - display progress
         no_below - INT - exclude words that occur less frequently than this
         keep - LIST/None - List of words to prevent being excluded
         '''
+        self.__version__ = __version__
+        
         if type(fileinput) == str:
             if not os.path.isfile(fileinput):
                 raise FileNotFoundError('No file exists at the location specified')
         self.FILEINPUT = fileinput
         self.ITERATIONS = iterations
         if stopwords == 'default': stopwords = stoplist
         if stopwords == None: stopwords = []
```

### Comparing `ciderpolarity-0.2.8/ciderpolarity/create_embeddings.py` & `ciderpolarity-0.2.9/ciderpolarity/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/ciderpolarity/create_vader.py` & `ciderpolarity-0.2.9/ciderpolarity/create_vader.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/ciderpolarity/load_polarities.py` & `ciderpolarity-0.2.9/ciderpolarity/load_polarities.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/ciderpolarity/run_bootstrapping.py` & `ciderpolarity-0.2.9/ciderpolarity/run_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/ciderpolarity/stopwords.py` & `ciderpolarity-0.2.9/ciderpolarity/stopwords.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/ciderpolarity/suggest_seeds.py` & `ciderpolarity-0.2.9/ciderpolarity/suggest_seeds.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/ciderpolarity/utils_funcs.py` & `ciderpolarity-0.2.9/ciderpolarity/utils_funcs.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.8/pyproject.toml` & `ciderpolarity-0.2.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ciderpolarity"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["jcy204 <jcy204@exeter.ac.uk>"]
 readme = "README.md"
 homepage = "https://github.com/jcy204/ciderPolarity"
 repository = "https://github.com/jcy204/ciderPolarity"
 
 [tool.poetry.dependencies]
```

### Comparing `ciderpolarity-0.2.8/PKG-INFO` & `ciderpolarity-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciderpolarity
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Home-page: https://github.com/jcy204/ciderPolarity
 Author: jcy204
 Author-email: jcy204@exeter.ac.uk
 Requires-Python: >=3.7,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

