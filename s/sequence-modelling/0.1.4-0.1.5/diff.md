# Comparing `tmp/sequence_modelling-0.1.4.tar.gz` & `tmp/sequence_modelling-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequence_modelling-0.1.4.tar", max compression
+gzip compressed data, was "sequence_modelling-0.1.5.tar", max compression
```

## Comparing `sequence_modelling-0.1.4.tar` & `sequence_modelling-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1500 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/LICENSE
--rw-r--r--   0        0        0     2306 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/README.md
--rw-r--r--   0        0        0      863 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9871 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/DiscreteOptim.py
--rw-r--r--   0        0        0        0 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/__init__.py
--rw-r--r--   0        0        0     5887 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/emissionplus.py
--rw-r--r--   0        0        0     5211 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/emmissions.py
--rw-r--r--   0        0        0    18426 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/hmm.py
--rw-r--r--   0        0        0     5900 2023-07-10 17:50:48.141160 sequence_modelling-0.1.4/src/sequence_modelling/hmmviz.py
--rw-r--r--   0        0        0    14709 2023-07-10 17:50:48.141160 sequence_modelling-0.1.4/src/sequence_modelling/qdhmm.py
--rw-r--r--   0        0        0    11895 2023-07-10 17:50:48.141160 sequence_modelling-0.1.4/src/sequence_modelling/qdhmm_logscaled.py
--rw-r--r--   0        0        0     1531 2023-07-10 17:50:48.141160 sequence_modelling-0.1.4/src/sequence_modelling/utils.py
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 sequence_modelling-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2306 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/README.md
+-rw-r--r--   0        0        0      863 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     9871 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/DiscreteOptim.py
+-rw-r--r--   0        0        0        0 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/__init__.py
+-rw-r--r--   0        0        0     5887 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/emissionplus.py
+-rw-r--r--   0        0        0     5211 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/emmissions.py
+-rw-r--r--   0        0        0    18380 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/hmm.py
+-rw-r--r--   0        0        0     5900 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/hmmviz.py
+-rw-r--r--   0        0        0    14709 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/qdhmm.py
+-rw-r--r--   0        0        0    11895 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/qdhmm_logscaled.py
+-rw-r--r--   0        0        0     1531 2023-07-24 04:14:18.546913 sequence_modelling-0.1.5/src/sequence_modelling/utils.py
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 sequence_modelling-0.1.5/PKG-INFO
```

### Comparing `sequence_modelling-0.1.4/LICENSE` & `sequence_modelling-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/README.md` & `sequence_modelling-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/pyproject.toml` & `sequence_modelling-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequence_modelling"
-version = "0.1.4"
+version = "0.1.5"
 description = "sequence modelling using HMMs"
 authors = ["Nitin Bhushan <bhushan.nitin@posteo.net>"]
 readme = "README.md"
 license = "BSD-2-Clause"
 
 
 [tool.poetry.dependencies]
```

### Comparing `sequence_modelling-0.1.4/src/sequence_modelling/DiscreteOptim.py` & `sequence_modelling-0.1.5/src/sequence_modelling/DiscreteOptim.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/src/sequence_modelling/emissionplus.py` & `sequence_modelling-0.1.5/src/sequence_modelling/emissionplus.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/src/sequence_modelling/emmissions.py` & `sequence_modelling-0.1.5/src/sequence_modelling/emmissions.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/src/sequence_modelling/hmm.py` & `sequence_modelling-0.1.5/src/sequence_modelling/hmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,20 @@
         """
         self.K = A.shape[1]
         assert A.shape[0] == self.K + 1
         self.O = O
         self.logA = np.log(A)
 
     def __repr__(self):
-        n = "" + "nStates: %d\n" % (self.K)
-        a = "" + "A:\n %s" % (str(np.exp(self.logA[:-1])))
-        pi = "" + "\nPi: \n %s" % (str(np.exp(self.logA[-1])))
-        o = "" + "\nObservation distribution: \n %s" % self.O
-        return n + a + pi + o
+        return (
+            f"nStates: {self.K}\n"
+            f"A:\n {self.logA[:-1].round(2)}\n"
+            f"Pi: \n {self.logA[-1].round(2)}\n"
+            f"Observation distribution: \n {self.O}"
+        )
 
     def sample(self, dim=1, N=1000):
         """Generates an observation sequence of length N.
 
         Parameters
         ----------
         dim : int
```

### Comparing `sequence_modelling-0.1.4/src/sequence_modelling/hmmviz.py` & `sequence_modelling-0.1.5/src/sequence_modelling/hmmviz.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/src/sequence_modelling/qdhmm.py` & `sequence_modelling-0.1.5/src/sequence_modelling/qdhmm.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/src/sequence_modelling/qdhmm_logscaled.py` & `sequence_modelling-0.1.5/src/sequence_modelling/qdhmm_logscaled.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/src/sequence_modelling/utils.py` & `sequence_modelling-0.1.5/src/sequence_modelling/utils.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.4/PKG-INFO` & `sequence_modelling-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequence-modelling
-Version: 0.1.4
+Version: 0.1.5
 Summary: sequence modelling using HMMs
 License: BSD-2-Clause
 Author: Nitin Bhushan
 Author-email: bhushan.nitin@posteo.net
 Requires-Python: >=3.9.0,<3.10.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

