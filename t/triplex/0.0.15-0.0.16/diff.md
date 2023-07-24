# Comparing `tmp/triplex-0.0.15.tar.gz` & `tmp/triplex-0.0.16.tar.gz`

## Comparing `triplex-0.0.15.tar` & `triplex-0.0.16.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 triplex-0.0.15/PKG-INFO
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/__init__.py
--rwxr-xr-x   0        0        0    11637 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/dfas.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/exceptions.py
--rwxr-xr-x   0        0        0    11214 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/perturbations.py
--rw-r--r--   0        0        0    12391 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/triplex.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/clausie.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/ollie.py
--rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/openie.py
--rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/parsers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/probings/__init__.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/probings/esnli.py
--rwxr-xr-x   0        0        0     5611 2020-02-02 00:00:00.000000 triplex-0.0.15/src/triplex/scripts/extract_from_dataset.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 triplex-0.0.15/LICENSE
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 triplex-0.0.15/README.md
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 triplex-0.0.15/pyproject.toml
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 triplex-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 triplex-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/__init__.py
+-rwxr-xr-x   0        0        0    11637 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/dfas.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/exceptions.py
+-rwxr-xr-x   0        0        0    11220 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/perturbations.py
+-rw-r--r--   0        0        0    12391 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/triplex.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/parsers/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/parsers/clausie.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/parsers/ollie.py
+-rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/parsers/openie.py
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/parsers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/probings/__init__.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/probings/esnli.py
+-rwxr-xr-x   0        0        0     5611 2020-02-02 00:00:00.000000 triplex-0.0.16/src/triplex/scripts/extract_from_dataset.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 triplex-0.0.16/LICENSE
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 triplex-0.0.16/README.md
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 triplex-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 triplex-0.0.16/PKG-INFO
```

### Comparing `triplex-0.0.15/PKG-INFO` & `triplex-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplex
-Version: 0.0.15
+Version: 0.0.16
 Summary: Explaining models, with Triples.
 Project-URL: Homepage, https://github.com/msetzu/triplex
 Project-URL: Bug Tracker, https://github.com/msetzu/triplex/issues
 Author-email: Mattia Setzu <mattia.setzu@unipi.it>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `triplex-0.0.15/src/triplex/README.md` & `triplex-0.0.16/src/triplex/README.md`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/src/triplex/dfas.py` & `triplex-0.0.16/src/triplex/dfas.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/src/triplex/perturbations.py` & `triplex-0.0.16/src/triplex/perturbations.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     nlp = spacy.load('en_core_web_sm')
     tokenizer = RobertaTokenizer.from_pretrained('roberta-large-mnli')
 
     @staticmethod
     def wordnet(text: str) -> spacy.tokens.doc.Doc:
         """Tag `text` with Wordnet."""
-        return WordnetAnnotator(HypernymPerturbator.nlp.lang)(HypernymPerturbator.nlp(text))
+        return WordnetAnnotator(HypernymPerturbator.nlp, name="en")(HypernymPerturbator.nlp(text))
 
     @staticmethod
     def nltk_hypernyms(text: str, branching: int = 1) -> Dict[str, Set[str]]:
         """
         Compute the NLTK hypernyms of the given `text`. Returns a list of pairs (token, hypernyms).
         Args:
             text: The text to perturb.
```

### Comparing `triplex-0.0.15/src/triplex/triplex.py` & `triplex-0.0.16/src/triplex/triplex.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/src/triplex/parsers/ollie.py` & `triplex-0.0.16/src/triplex/parsers/ollie.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/src/triplex/parsers/openie.py` & `triplex-0.0.16/src/triplex/parsers/openie.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/src/triplex/parsers/utils.py` & `triplex-0.0.16/src/triplex/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/src/triplex/probings/esnli.py` & `triplex-0.0.16/src/triplex/probings/esnli.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/src/triplex/scripts/extract_from_dataset.py` & `triplex-0.0.16/src/triplex/scripts/extract_from_dataset.py`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/LICENSE` & `triplex-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/README.md` & `triplex-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `triplex-0.0.15/pyproject.toml` & `triplex-0.0.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "triplex"
-version = "0.0.15"
+version = "0.0.16"
 authors = [
   { name="Mattia Setzu", email="mattia.setzu@unipi.it" },
 ]
 description = "Explaining models, with Triples."
 readme = "README.md"
 requires-python = ">=3.8, <3.11"
 classifiers = [
```

