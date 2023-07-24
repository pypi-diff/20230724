# Comparing `tmp/mldsutils-0.0.2.2.tar.gz` & `tmp/mldsutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mldsutils-0.0.2.2.tar", last modified: Tue Jul  4 17:52:07 2023, max compression
+gzip compressed data, was "mldsutils-0.0.3.tar", last modified: Mon Jul 24 11:23:01 2023, max compression
```

## Comparing `mldsutils-0.0.2.2.tar` & `mldsutils-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 17:52:07.554706 mldsutils-0.0.2.2/
--rw-rw-rw-   0        0        0     1091 2023-06-14 15:19:03.000000 mldsutils-0.0.2.2/LICENSE
--rw-rw-rw-   0        0        0       95 2023-07-04 17:48:35.000000 mldsutils-0.0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2320 2023-07-04 17:52:07.553692 mldsutils-0.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1747 2023-06-25 16:37:01.000000 mldsutils-0.0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 17:52:07.482677 mldsutils-0.0.2.2/mldsutils/
--rw-rw-rw-   0        0        0       26 2023-07-04 11:15:33.000000 mldsutils-0.0.2.2/mldsutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:52:07.512683 mldsutils-0.0.2.2/mldsutils/classification/
--rw-rw-rw-   0        0        0       92 2023-06-14 14:32:37.000000 mldsutils-0.0.2.2/mldsutils/classification/__init__.py
--rw-rw-rw-   0        0        0     1199 2023-06-19 14:42:55.000000 mldsutils-0.0.2.2/mldsutils/classification/_classifiers.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:52:07.518693 mldsutils-0.0.2.2/mldsutils/metrics/
--rw-rw-rw-   0        0        0      449 2023-06-14 14:32:37.000000 mldsutils-0.0.2.2/mldsutils/metrics/__init__.py
--rw-rw-rw-   0        0        0     2390 2023-06-14 14:32:37.000000 mldsutils-0.0.2.2/mldsutils/metrics/_classification.py
--rw-rw-rw-   0        0        0    24517 2023-07-04 11:39:14.000000 mldsutils-0.0.2.2/mldsutils/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:52:07.526707 mldsutils-0.0.2.2/mldsutils/preprocessing/
--rw-rw-rw-   0        0        0      277 2023-06-29 16:45:42.000000 mldsutils-0.0.2.2/mldsutils/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1952 2023-06-30 12:09:27.000000 mldsutils-0.0.2.2/mldsutils/preprocessing/_feature_selection.py
--rw-rw-rw-   0        0        0     1008 2023-07-03 19:36:34.000000 mldsutils-0.0.2.2/mldsutils/preprocessing/_resample.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:52:07.531696 mldsutils-0.0.2.2/mldsutils/regression/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:39:15.000000 mldsutils-0.0.2.2/mldsutils/regression/__init__.py
--rw-rw-rw-   0        0        0     1351 2023-06-14 14:32:37.000000 mldsutils-0.0.2.2/mldsutils/regression/_regressors.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:52:07.550701 mldsutils-0.0.2.2/mldsutils/tests/
--rw-rw-rw-   0        0        0        0 2023-07-04 11:11:45.000000 mldsutils-0.0.2.2/mldsutils/tests/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-04 11:21:25.000000 mldsutils-0.0.2.2/mldsutils/tests/test_resampler.py
--rw-rw-rw-   0        0        0     5762 2023-06-27 15:33:13.000000 mldsutils-0.0.2.2/mldsutils/tests/test_scorer.py
--rw-rw-rw-   0        0        0     4669 2023-06-24 16:33:50.000000 mldsutils-0.0.2.2/mldsutils/tests/test_shrinkage_lda_classifier.py
--rw-rw-rw-   0        0        0     1611 2023-06-30 12:29:32.000000 mldsutils-0.0.2.2/mldsutils/tests/test_variable_selector.py
-drwxrwxrwx   0        0        0        0 2023-07-04 17:52:07.506698 mldsutils-0.0.2.2/mldsutils.egg-info/
--rw-rw-rw-   0        0        0     2320 2023-07-04 17:52:07.000000 mldsutils-0.0.2.2/mldsutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-07-04 17:52:07.000000 mldsutils-0.0.2.2/mldsutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 17:52:07.000000 mldsutils-0.0.2.2/mldsutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-04 17:52:07.000000 mldsutils-0.0.2.2/mldsutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      653 2023-07-04 17:51:45.000000 mldsutils-0.0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 17:52:07.555701 mldsutils-0.0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 11:23:01.561339 mldsutils-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-14 15:19:03.000000 mldsutils-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       95 2023-07-04 17:48:35.000000 mldsutils-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2318 2023-07-24 11:23:01.560338 mldsutils-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1747 2023-06-25 16:37:01.000000 mldsutils-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 11:23:01.447459 mldsutils-0.0.3/mldsutils/
+-rw-rw-rw-   0        0        0       26 2023-07-04 11:15:33.000000 mldsutils-0.0.3/mldsutils/__init__.py
+-rw-rw-rw-   0        0        0     5254 2023-07-21 19:10:19.000000 mldsutils-0.0.3/mldsutils/base.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:23:01.486719 mldsutils-0.0.3/mldsutils/classification/
+-rw-rw-rw-   0        0        0       92 2023-06-14 14:32:37.000000 mldsutils-0.0.3/mldsutils/classification/__init__.py
+-rw-rw-rw-   0        0        0     1199 2023-06-19 14:42:55.000000 mldsutils-0.0.3/mldsutils/classification/_classifiers.py
+-rw-rw-rw-   0        0        0     1168 2023-07-23 12:30:59.000000 mldsutils-0.0.3/mldsutils/imblearn-test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:23:01.505392 mldsutils-0.0.3/mldsutils/metrics/
+-rw-rw-rw-   0        0        0      607 2023-07-23 10:44:08.000000 mldsutils-0.0.3/mldsutils/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2390 2023-06-14 14:32:37.000000 mldsutils-0.0.3/mldsutils/metrics/_classification.py
+-rw-rw-rw-   0        0        0      971 2023-07-23 12:29:30.000000 mldsutils-0.0.3/mldsutils/metrics/_regression.py
+-rw-rw-rw-   0        0        0     9622 2023-07-24 10:33:16.000000 mldsutils-0.0.3/mldsutils/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:23:01.523213 mldsutils-0.0.3/mldsutils/preprocessing/
+-rw-rw-rw-   0        0        0      417 2023-07-22 19:51:06.000000 mldsutils-0.0.3/mldsutils/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     1952 2023-07-24 10:46:04.000000 mldsutils-0.0.3/mldsutils/preprocessing/_feature_selection.py
+-rw-rw-rw-   0        0        0     8711 2023-07-23 12:41:08.000000 mldsutils-0.0.3/mldsutils/preprocessing/_outlier_elimination.py
+-rw-rw-rw-   0        0        0      837 2023-07-24 10:36:23.000000 mldsutils-0.0.3/mldsutils/preprocessing/_resample.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:23:01.532730 mldsutils-0.0.3/mldsutils/regression/
+-rw-rw-rw-   0        0        0        0 2023-06-15 18:39:15.000000 mldsutils-0.0.3/mldsutils/regression/__init__.py
+-rw-rw-rw-   0        0        0     1351 2023-06-14 14:32:37.000000 mldsutils-0.0.3/mldsutils/regression/_regressors.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:23:01.557335 mldsutils-0.0.3/mldsutils/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-04 11:11:45.000000 mldsutils-0.0.3/mldsutils/tests/__init__.py
+-rw-rw-rw-   0        0        0     1970 2023-07-24 10:30:13.000000 mldsutils-0.0.3/mldsutils/tests/test_resampler.py
+-rw-rw-rw-   0        0        0     5762 2023-06-27 15:33:13.000000 mldsutils-0.0.3/mldsutils/tests/test_scorer.py
+-rw-rw-rw-   0        0        0     4669 2023-06-24 16:33:50.000000 mldsutils-0.0.3/mldsutils/tests/test_shrinkage_lda_classifier.py
+-rw-rw-rw-   0        0        0     1783 2023-07-04 19:04:18.000000 mldsutils-0.0.3/mldsutils/tests/test_variable_selector.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:23:01.474221 mldsutils-0.0.3/mldsutils.egg-info/
+-rw-rw-rw-   0        0        0     2318 2023-07-24 11:23:01.000000 mldsutils-0.0.3/mldsutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-07-24 11:23:01.000000 mldsutils-0.0.3/mldsutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:23:01.000000 mldsutils-0.0.3/mldsutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-24 11:23:01.000000 mldsutils-0.0.3/mldsutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      651 2023-07-24 11:22:27.000000 mldsutils-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 11:23:01.561339 mldsutils-0.0.3/setup.cfg
```

### Comparing `mldsutils-0.0.2.2/LICENSE` & `mldsutils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mldsutils-0.0.2.2/PKG-INFO` & `mldsutils-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mldsutils
-Version: 0.0.2.2
+Version: 0.0.3
 Summary: A toolkit for various machine learning tasks.
 Author-email: Baris Gün Sürmeli <baris.suermeli@th-owl.de>
 Project-URL: Homepage, https://github.com/barisguns/MachineLearningUtils
 Project-URL: Bug Tracker, https://github.com/barisguns/MachineLearningUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mldsutils-0.0.2.2/README.md` & `mldsutils-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mldsutils-0.0.2.2/mldsutils/classification/_classifiers.py` & `mldsutils-0.0.3/mldsutils/classification/_classifiers.py`

 * *Files identical despite different names*

### Comparing `mldsutils-0.0.2.2/mldsutils/metrics/_classification.py` & `mldsutils-0.0.3/mldsutils/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `mldsutils-0.0.2.2/mldsutils/preprocessing/_feature_selection.py` & `mldsutils-0.0.3/mldsutils/preprocessing/_feature_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         Constructs a manual variable selector object.
         :param variable_range_list:
         """
         self.variable_range_list = variable_range_list
         return
 
     def fit(self, X, y=None):
-        return self
+        return None
 
     def transform(self, X, y=None):
         """
         Takes data matrix and the variable range list and returns the filtered data matrix.
         :param X:
         :param y:
         :return:
```

### Comparing `mldsutils-0.0.2.2/mldsutils/preprocessing/_resample.py` & `mldsutils-0.0.3/mldsutils/preprocessing/_resample.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from sklearn.base import BaseEstimator
 import numpy as np
 
-from imblearn.base import SamplerMixin
+from mldsutils.base import SamplerMixin
 
 
 class NumpyPytorchDatatypeResampler(SamplerMixin, BaseEstimator):
     """
     This is a custom imblearn resampler which basically transforms data
     into formats that would work as Pytorch inputs.
     It is especially useful when outputs of sklearn/imblearn transformers are to be given to Pytorch models as input.
     Imblearn is a library relying on sklearn that implements resampling tools and it is more useful here than sklearn
     because it can also transform "y" in the fit phase, which we need when preparing input for Pytorch.
 
     """
-    def __init__(self):
-        return
 
-    def fit(self, X, y):
-        return
-
-    def fit_resample(self, X, y):
-        return self._fit_resample(X, y)
-
-    def transform(self, X, y=None):
-        return X.astype(np.float32), None, None
+    def _resample(self, X, y=None):
+        return (X.astype(np.float32),)
 
     def _fit_resample(self, X, y):
         return X.astype(np.float32), y.astype(np.int64)
```

### Comparing `mldsutils-0.0.2.2/mldsutils/regression/_regressors.py` & `mldsutils-0.0.3/mldsutils/regression/_regressors.py`

 * *Files identical despite different names*

### Comparing `mldsutils-0.0.2.2/mldsutils/tests/test_resampler.py` & `mldsutils-0.0.3/mldsutils/tests/test_resampler.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,26 +25,23 @@
 def test_custom_resampler():
     # Create a synthetic imbalanced dataset
     X, y = make_classification(n_samples=1000, n_features=20, weights=[0.9, 0.1], random_state=42)
 
     # Define the sklearn transformer
     scaler = StandardScaler()
 
-    # Define your custom resampler
+    # Define the custom resampler
     resampler = NumpyPytorchDatatypeResampler()
-    # Make sure fit function of the resampler returns None
-    x = resampler.fit(X, y)
-    assert x is None
 
     # Create the PyTorch model
     model = MyModel()
 
     X_sc = scaler.fit_transform(X)
 
-    X_transformed, _, _ = resampler.transform(X_sc)
+    X_transformed = resampler.resample(X_sc)[0]
     # Check if the transformed data is in the expected input format for torch models
     assert X_transformed.dtype == np.float32
 
     X_resampled, y_resampled = resampler.fit_resample(X_sc, y)
 
     # Check if the resampled data is in the expected input format for torch models
     assert X_resampled.dtype == np.float32
```

### Comparing `mldsutils-0.0.2.2/mldsutils/tests/test_scorer.py` & `mldsutils-0.0.3/mldsutils/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `mldsutils-0.0.2.2/mldsutils/tests/test_shrinkage_lda_classifier.py` & `mldsutils-0.0.3/mldsutils/tests/test_shrinkage_lda_classifier.py`

 * *Files identical despite different names*

### Comparing `mldsutils-0.0.2.2/mldsutils/tests/test_variable_selector.py` & `mldsutils-0.0.3/mldsutils/tests/test_variable_selector.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,17 +26,22 @@
 def test_manual_range_variable_selector():
     # Generate synthetic data for testing
     X, y = make_regression(n_samples=100, n_features=10, random_state=42)
 
     # Define the variable range list for selection
     variable_range_list = [(1, 3), (7, 9)]
 
+    variable_selector = ManualRangeVariableSelector(variable_range_list)
+    # Make sure fit function of the variable selector returns None
+    x = variable_selector.fit(X, y)
+    assert x is None
+
     # Create the transformer pipeline
     transformer = Pipeline([
-        ('manual_selector', ManualRangeVariableSelector(variable_range_list))
+        ('manual_selector', variable_selector)
     ])
 
     # Apply the transformer
     X_transformed = transformer.transform(X)
 
     # Check the transformed shape and content
     assert X_transformed.shape == (100, 4)
```

### Comparing `mldsutils-0.0.2.2/mldsutils.egg-info/PKG-INFO` & `mldsutils-0.0.3/mldsutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mldsutils
-Version: 0.0.2.2
+Version: 0.0.3
 Summary: A toolkit for various machine learning tasks.
 Author-email: Baris Gün Sürmeli <baris.suermeli@th-owl.de>
 Project-URL: Homepage, https://github.com/barisguns/MachineLearningUtils
 Project-URL: Bug Tracker, https://github.com/barisguns/MachineLearningUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mldsutils-0.0.2.2/mldsutils.egg-info/SOURCES.txt` & `mldsutils-0.0.3/mldsutils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 mldsutils/__init__.py
+mldsutils/base.py
+mldsutils/imblearn-test.py
 mldsutils/pipeline.py
 mldsutils.egg-info/PKG-INFO
 mldsutils.egg-info/SOURCES.txt
 mldsutils.egg-info/dependency_links.txt
 mldsutils.egg-info/top_level.txt
 mldsutils/classification/__init__.py
 mldsutils/classification/_classifiers.py
 mldsutils/metrics/__init__.py
 mldsutils/metrics/_classification.py
+mldsutils/metrics/_regression.py
 mldsutils/preprocessing/__init__.py
 mldsutils/preprocessing/_feature_selection.py
+mldsutils/preprocessing/_outlier_elimination.py
 mldsutils/preprocessing/_resample.py
 mldsutils/regression/__init__.py
 mldsutils/regression/_regressors.py
 mldsutils/tests/__init__.py
 mldsutils/tests/test_resampler.py
 mldsutils/tests/test_scorer.py
 mldsutils/tests/test_shrinkage_lda_classifier.py
```

### Comparing `mldsutils-0.0.2.2/pyproject.toml` & `mldsutils-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools==65.5"]
 
 [project]
 name = "mldsutils"
-version = "0.0.2.2"
+version = "0.0.3"
 authors = [
   { name="Baris Gün Sürmeli", email="baris.suermeli@th-owl.de" },
 ]
 description = "A toolkit for various machine learning tasks."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

