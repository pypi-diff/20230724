# Comparing `tmp/calibrated_explanations-0.0.6a0.tar.gz` & `tmp/calibrated_explanations-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibrated_explanations-0.0.6a0.tar", last modified: Thu Jul 20 12:54:34 2023, max compression
+gzip compressed data, was "calibrated_explanations-0.0.8.tar", last modified: Mon Jul 24 11:47:00 2023, max compression
```

## Comparing `calibrated_explanations-0.0.6a0.tar` & `calibrated_explanations-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.808170 calibrated_explanations-0.0.6a0/
--rw-rw-rw-   0        0        0     1085 2023-07-12 12:35:31.000000 calibrated_explanations-0.0.6a0/LICENSE
--rw-rw-rw-   0        0        0     2660 2023-07-20 12:54:34.807164 calibrated_explanations-0.0.6a0/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/README.md
--rw-rw-rw-   0        0        0      979 2023-07-20 12:49:04.000000 calibrated_explanations-0.0.6a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 12:54:34.808170 calibrated_explanations-0.0.6a0/setup.cfg
--rw-rw-rw-   0        0        0      179 2023-07-12 12:35:32.000000 calibrated_explanations-0.0.6a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.756162 calibrated_explanations-0.0.6a0/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.781161 calibrated_explanations-0.0.6a0/src/calibrated_explanations/
--rw-rw-rw-   0        0        0     2533 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/VennAbers.py
--rw-rw-rw-   0        0        0      509 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/__init__.py
--rw-rw-rw-   0        0        0     1957 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/_discretizers.py
--rw-rw-rw-   0        0        0    38940 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/_explanations.py
--rw-rw-rw-   0        0        0    36850 2023-07-20 12:36:38.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/core.py
--rw-rw-rw-   0        0        0     3039 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.800161 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/
--rw-rw-rw-   0        0        0     2660 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.804163 calibrated_explanations-0.0.6a0/tests/
--rw-rw-rw-   0        0        0     8692 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/tests/test_classification.py
--rw-rw-rw-   0        0        0    15625 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:47:00.480973 calibrated_explanations-0.0.8/
+-rw-rw-rw-   0        0        0     1085 2023-07-12 12:35:31.000000 calibrated_explanations-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     8454 2023-07-24 11:47:00.479950 calibrated_explanations-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7772 2023-07-24 11:18:15.000000 calibrated_explanations-0.0.8/README.md
+-rw-rw-rw-   0        0        0      977 2023-07-24 11:44:17.000000 calibrated_explanations-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 11:47:00.480973 calibrated_explanations-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      179 2023-07-12 12:35:32.000000 calibrated_explanations-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:47:00.303951 calibrated_explanations-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 11:47:00.409951 calibrated_explanations-0.0.8/src/calibrated_explanations/
+-rw-rw-rw-   0        0        0     2533 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.8/src/calibrated_explanations/VennAbers.py
+-rw-rw-rw-   0        0        0      509 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.8/src/calibrated_explanations/__init__.py
+-rw-rw-rw-   0        0        0     1957 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.8/src/calibrated_explanations/_discretizers.py
+-rw-rw-rw-   0        0        0    38948 2023-07-24 08:31:30.000000 calibrated_explanations-0.0.8/src/calibrated_explanations/_explanations.py
+-rw-rw-rw-   0        0        0    37891 2023-07-24 11:44:16.000000 calibrated_explanations-0.0.8/src/calibrated_explanations/core.py
+-rw-rw-rw-   0        0        0     3039 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.8/src/calibrated_explanations/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:47:00.450949 calibrated_explanations-0.0.8/src/calibrated_explanations.egg-info/
+-rw-rw-rw-   0        0        0     8454 2023-07-24 11:47:00.000000 calibrated_explanations-0.0.8/src/calibrated_explanations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-07-24 11:47:00.000000 calibrated_explanations-0.0.8/src/calibrated_explanations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:47:00.000000 calibrated_explanations-0.0.8/src/calibrated_explanations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-24 11:47:00.000000 calibrated_explanations-0.0.8/src/calibrated_explanations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-07-24 11:47:00.000000 calibrated_explanations-0.0.8/src/calibrated_explanations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 11:47:00.476950 calibrated_explanations-0.0.8/tests/
+-rw-rw-rw-   0        0        0     8692 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.8/tests/test_classification.py
+-rw-rw-rw-   0        0        0    15625 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.8/tests/test_regression.py
```

### Comparing `calibrated_explanations-0.0.6a0/LICENSE` & `calibrated_explanations-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6a0/pyproject.toml` & `calibrated_explanations-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calibrated_explanations"
-version = "0.0.6a0"
+version = "0.0.8"
 authors = [
   { name="Helena Löfström", email="helena.lofstrom@ju.se" },
   { name="Tuwe Löfström", email="tuwe.lofstrom@ju.se" },
 ]
 description = "Extract calibrated explanations from machine learning models."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `calibrated_explanations-0.0.6a0/src/calibrated_explanations/VennAbers.py` & `calibrated_explanations-0.0.8/src/calibrated_explanations/VennAbers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6a0/src/calibrated_explanations/_discretizers.py` & `calibrated_explanations-0.0.8/src/calibrated_explanations/_discretizers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6a0/src/calibrated_explanations/_explanations.py` & `calibrated_explanations-0.0.8/src/calibrated_explanations/_explanations.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,36 +569,36 @@
         xl = np.linspace(-0.5, x[0], 2)
         xh = np.linspace(x[-1], x[-1]+0.5, 2)
         ax1.fill_betweenx(x, [0], [0], color='k')
         ax1.fill_betweenx(xl, [0], [0], color='k')
         ax1.fill_betweenx(xh, [0], [0], color='k')
         if interval:
             p = predict['predict'][idx]
-            gwl = predict['low'][idx] - p
-            gwh = predict['high'][idx] - p
+            gwl = p - predict['low'][idx]
+            gwh = p - predict['high'][idx]
             
             gwh, gwl = np.max([gwh, gwl]), np.min([gwh, gwl])
             ax1.fill_betweenx([-0.5,num_to_show-0.5], gwl, gwh, color='k', alpha=0.2)
 
         for jx, j in enumerate(features_to_plot):
             xj = np.linspace(x[jx]-0.2, x[jx]+0.2,2)
             mn,mx = 0,0
             if interval:
-                w = feature_weights['predict'][j]
-                wl = feature_weights['low'][j] 
-                wh = feature_weights['high'][j]
+                w = - feature_weights['predict'][j]
+                wl = - feature_weights['low'][j] 
+                wh = - feature_weights['high'][j]
                 wh, wl = np.max([wh, wl]), np.min([wh, wl]) 
-                mn = wh if w < 0 else 0
-                mx = wl if w > 0 else 0
+                mx = wh if w < 0 else 0
+                mn = wl if w > 0 else 0
                 # If uncertainty cover zero, then set to w to avoid solid plotting
                 if wh > 0 and wl < 0:
                     mn = w
                     mx = w
             else:
-                w = feature_weights[j]
+                w = - feature_weights[j]
                 mn = w if w < 0 else 0
                 mx = w if w > 0 else 0
             color = 'b' if w > 0 else 'r'
             ax1.fill_betweenx(xj, mn,mx,color=color)
             ax1.fill_betweenx(xj, w,w,color=color)
             if interval:
                 if wh > 0 and wl < 0 and self.CE.mode == 'classification':
```

### Comparing `calibrated_explanations-0.0.6a0/src/calibrated_explanations/core.py` & `calibrated_explanations-0.0.8/src/calibrated_explanations/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from lime.lime_tabular import LimeTabularExplainer
 from shap import Explainer
 
 from ._explanations import CalibratedExplanation
 from ._discretizers import BinaryDiscretizer, BinaryEntropyDiscretizer, DecileDiscretizer, QuartileDiscretizer, EntropyDiscretizer 
 from .VennAbers import VennAbers
 
-__version__ = 'v0.0.6'
+__version__ = 'v0.0.8'
 
 class CalibratedExplainer:
     """
     Calibrated Explainer for black-box models.
 
     """
     def __init__(self, 
@@ -248,15 +248,39 @@
                 for i,x in enumerate(testX):                    
                     interval[i,0] = self.interval_model.predict(y_hat=[predict[i]], sigmas=sigma_test, y=float(interval_[i,0] - median[i] + y))
                     interval[i,1] = self.interval_model.predict(y_hat=[predict[i]], sigmas=sigma_test, y=float(interval_[i,2] - median[i] + y))
                 predict = y_prob
                 # Changed to 1-p so that high probability means high prediction and vice versa
                 return [1-predict[0]], 1-interval[:,1], 1-interval[:,0], None
 
-
+    def get_factuals(self, 
+                 testX: Any,
+                 y: Optional[List or float] = None, # The same meaning as y has for cps in crepes.
+                 low_high_percentiles: Tuple[float,float] = (5, 95),
+                 ) -> CalibratedExplanation:
+        
+        if 'regression' in self.mode:
+            discretizer = 'binary'
+        else:
+            discretizer = 'binaryEntropy'
+        self.set_discretizer(discretizer)
+        return self(testX, y, low_high_percentiles)
+        
+    def get_counterfactuals(self, 
+                 testX: Any,
+                 y: Optional[List or float] = None, # The same meaning as y has for cps in crepes.
+                 low_high_percentiles: Tuple[float,float] = (5, 95),
+                 ) -> CalibratedExplanation:
+        
+        if 'regression' in self.mode:
+            discretizer = 'decile'
+        else:
+            discretizer = 'entropy'
+        self.set_discretizer(discretizer)
+        return self(testX, y, low_high_percentiles)    
 
     def __call__(self, 
                  testX: Any,
                  y: Optional[List or float] = None, # The same meaning as y has for cps in crepes.
                  low_high_percentiles: Tuple[float,float] = (5, 95),
                  ) -> CalibratedExplanation:
         """Creates a CalibratedExplanation object for the test data.
```

### Comparing `calibrated_explanations-0.0.6a0/src/calibrated_explanations/wrappers.py` & `calibrated_explanations-0.0.8/src/calibrated_explanations/wrappers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/SOURCES.txt` & `calibrated_explanations-0.0.8/src/calibrated_explanations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6a0/tests/test_classification.py` & `calibrated_explanations-0.0.8/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6a0/tests/test_regression.py` & `calibrated_explanations-0.0.8/tests/test_regression.py`

 * *Files identical despite different names*

