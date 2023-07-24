# Comparing `tmp/triplex-0.0.14.tar.gz` & `tmp/triplex-0.0.15.tar.gz`

## Comparing `triplex-0.0.14.tar` & `triplex-0.0.15.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/__init__.py
--rwxr-xr-x   0        0        0    11637 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/dfas.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/exceptions.py
--rwxr-xr-x   0        0        0    11214 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/perturbations.py
--rw-r--r--   0        0        0    12391 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/triplex.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/parsers/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/parsers/clausie.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/parsers/ollie.py
--rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/parsers/openie.py
--rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/parsers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/probings/__init__.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/probings/esnli.py
--rwxr-xr-x   0        0        0     5611 2020-02-02 00:00:00.000000 triplex-0.0.14/src/triplex/scripts/extract_from_dataset.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 triplex-0.0.14/LICENSE
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 triplex-0.0.14/README.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 triplex-0.0.14/pyproject.toml
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 triplex-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 triplex-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/__init__.py
+-rwxr-xr-x   0        0        0    11637 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/dfas.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/exceptions.py
+-rwxr-xr-x   0        0        0    11214 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/perturbations.py
+-rw-r--r--   0        0        0    12391 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/triplex.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/clausie.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/ollie.py
+-rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/openie.py
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/probings/__init__.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/probings/esnli.py
+-rwxr-xr-x   0        0        0     5611 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/scripts/extract_from_dataset.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 triplex-0.0.15/LICENSE
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 triplex-0.0.15/README.md
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 triplex-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 triplex-0.0.15/PKG-INFO
```

### Comparing `triplex-0.0.14/src/triplex/README.md` & `triplex-0.0.15/src/triplex/README.md`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/src/triplex/dfas.py` & `triplex-0.0.15/src/triplex/dfas.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/src/triplex/perturbations.py` & `triplex-0.0.15/src/triplex/perturbations.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/src/triplex/triplex.py` & `triplex-0.0.15/src/triplex/triplex.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/src/triplex/parsers/ollie.py` & `triplex-0.0.15/src/triplex/parsers/ollie.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/src/triplex/parsers/openie.py` & `triplex-0.0.15/src/triplex/parsers/openie.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/src/triplex/parsers/utils.py` & `triplex-0.0.15/src/triplex/parsers/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import spacy
 
 import itertools
 import re
 from abc import abstractmethod
 from typing import List, Tuple
 
-from dfas import DFA
+from ..dfas import DFA
 
 DOC = spacy.load("en_core_web_sm")
 
 
 class Parser:
     @abstractmethod
     def parse(self, text: str) -> DFA:
```

### Comparing `triplex-0.0.14/src/triplex/probings/esnli.py` & `triplex-0.0.15/src/triplex/probings/esnli.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/src/triplex/scripts/extract_from_dataset.py` & `triplex-0.0.15/src/triplex/scripts/extract_from_dataset.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/LICENSE` & `triplex-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/README.md` & `triplex-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `triplex-0.0.14/pyproject.toml` & `triplex-0.0.15/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "triplex"
-version = "0.0.14"
+version = "0.0.15"
 authors = [
   { name="Mattia Setzu", email="mattia.setzu@unipi.it" },
 ]
 description = "Explaining models, with Triples."
 readme = "README.md"
 requires-python = ">=3.8, <3.11"
 classifiers = [
@@ -27,14 +27,15 @@
     "logzero",
     "nltk",
     "numpy",
     "pandas",
     "pyarrow",
     "pylint",
     "smart-open==6.3.0",
+    "scipy",
     "spacy",
     "spacy-legacy",
     "spacy-wordnet",
     "srsly",
     "stanford-openie",
     "stanfordnlp",
     "torch",
```

### Comparing `triplex-0.0.14/PKG-INFO` & `triplex-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplex
-Version: 0.0.14
+Version: 0.0.15
 Summary: Explaining models, with Triples.
 Project-URL: Homepage, https://github.com/msetzu/triplex
 Project-URL: Bug Tracker, https://github.com/msetzu/triplex/issues
 Author-email: Mattia Setzu <mattia.setzu@unipi.it>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Requires-Dist: huggingface-hub
 Requires-Dist: logzero
 Requires-Dist: nltk
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pylint
+Requires-Dist: scipy
 Requires-Dist: smart-open==6.3.0
 Requires-Dist: spacy
 Requires-Dist: spacy-legacy
 Requires-Dist: spacy-wordnet
 Requires-Dist: srsly
 Requires-Dist: stanford-openie
 Requires-Dist: stanfordnlp
```

