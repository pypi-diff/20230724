# Comparing `tmp/gpforecaster-0.3.93.tar.gz` & `tmp/gpforecaster-0.3.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpforecaster-0.3.93.tar", last modified: Wed Jul 19 09:37:50 2023, max compression
+gzip compressed data, was "gpforecaster-0.3.94.tar", last modified: Mon Jul 24 14:08:15 2023, max compression
```

## Comparing `gpforecaster-0.3.93.tar` & `gpforecaster-0.3.94.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:50.346622 gpforecaster-0.3.93/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 09:37:50.346622 gpforecaster-0.3.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:50.342622 gpforecaster-0.3.93/gpforecaster/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:50.342622 gpforecaster-0.3.93/gpforecaster/model/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/model/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    39412 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/model/gpf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/model/hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/model/mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/model/mlls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:50.342622 gpforecaster-0.3.93/gpforecaster/results/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/results/calculate_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:50.346622 gpforecaster-0.3.93/gpforecaster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_calculate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_hyperparameter_tuning_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_model_results_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_model_results_police.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_model_results_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_results_partial_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_run_model_with_sampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_sparse_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_store_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_svg_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/tests/test_tourism_gpf_with_local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:50.346622 gpforecaster-0.3.93/gpforecaster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:50.346622 gpforecaster-0.3.93/gpforecaster/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/gpforecaster/visualization/plot_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:37:50.342622 gpforecaster-0.3.93/gpforecaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 09:37:50.000000 gpforecaster-0.3.93/gpforecaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-19 09:37:50.000000 gpforecaster-0.3.93/gpforecaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:37:50.000000 gpforecaster-0.3.93/gpforecaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-19 09:37:50.000000 gpforecaster-0.3.93/gpforecaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 09:37:50.000000 gpforecaster-0.3.93/gpforecaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:37:50.346622 gpforecaster-0.3.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-19 09:37:36.000000 gpforecaster-0.3.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.086636 gpforecaster-0.3.94/gpforecaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.090636 gpforecaster-0.3.94/gpforecaster/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39784 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/gpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/model/mlls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.090636 gpforecaster-0.3.94/gpforecaster/results/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/results/calculate_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/gpforecaster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_calculate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_hyperparameter_tuning_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_model_results_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_model_results_police.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_model_results_prison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_results_partial_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_run_model_with_sampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_sparse_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_store_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_svg_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/tests/test_tourism_gpf_with_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/gpforecaster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/gpforecaster/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/gpforecaster/visualization/plot_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:08:15.086636 gpforecaster-0.3.94/gpforecaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 14:08:14.000000 gpforecaster-0.3.94/gpforecaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 14:08:15.000000 gpforecaster-0.3.94/gpforecaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:08:14.000000 gpforecaster-0.3.94/gpforecaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 14:08:14.000000 gpforecaster-0.3.94/gpforecaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 14:08:14.000000 gpforecaster-0.3.94/gpforecaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:08:15.094636 gpforecaster-0.3.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-24 14:07:58.000000 gpforecaster-0.3.94/setup.py
```

### Comparing `gpforecaster-0.3.93/LICENCE` & `gpforecaster-0.3.94/LICENCE`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/PKG-INFO` & `gpforecaster-0.3.94/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.93
+Version: 0.3.94
 Summary: Hierarchical time series forecasting model using Gaussian Processes
 Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
 Platform: UNKNOWN
```

### Comparing `gpforecaster-0.3.93/README.md` & `gpforecaster-0.3.94/README.md`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/model/gp.py` & `gpforecaster-0.3.94/gpforecaster/model/gp.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/model/gpf.py` & `gpforecaster-0.3.94/gpforecaster/model/gpf.py`

 * *Files 0% similar despite different names*

```diff
@@ -632,14 +632,15 @@
 
     def train(
         self,
         lr: float = 0.00246118,
         epochs: int = 500,
         early_stopping: bool = True,
         cross_validation: bool = True,
+        no_validation: bool = False,
         patience: int = 10,
         weight_decay: float = 0.0008031679,
         verbose: bool = True,
         scheduler_type: str = "cosine",
         gamma_rate: float = 0.304262175,
         random_init: bool = False,
         rbf_kernel_lengthscale: float = 1.0,
@@ -700,17 +701,24 @@
             tscv.split(self.train_x)
         ):
             # If not cross-validation and because min number of folds for tscv is 2
             # we skip the first one
             if not cross_validation and fold_idx == 0:
                 continue
             print(f"\nStarting training for Fold {fold_idx + 1}...\n")
-            train_x = self.train_x[train_indices]
-            train_y = self.train_y[train_indices]
-            train_y_split = concatenated_hierarchical_data[train_indices]
+            if no_validation:
+                # Possibility to use the whole training dataset to train since
+                # there is no real risk of overfitting
+                train_x = self.train_x
+                train_y = self.train_y
+                train_y_split = concatenated_hierarchical_data
+            else:
+                train_x = self.train_x[train_indices]
+                train_y = self.train_y[train_indices]
+                train_y_split = concatenated_hierarchical_data[train_indices]
 
             val_x = self.train_x[val_indices]
             val_y = concatenated_hierarchical_data[val_indices]
 
             likelihood_list, model_list = self._build_model(
                 x=train_x,
                 y=train_y,
```

### Comparing `gpforecaster-0.3.93/gpforecaster/model/hyperparameter_tuning.py` & `gpforecaster-0.3.94/gpforecaster/model/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/model/mean_functions.py` & `gpforecaster-0.3.94/gpforecaster/model/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/model/mlls.py` & `gpforecaster-0.3.94/gpforecaster/model/mlls.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/results/calculate_metrics.py` & `gpforecaster-0.3.94/gpforecaster/results/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_calculate_results.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_calculate_results.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_early_stopping.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_hyperparameter_tuning.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_hyperparameter_tuning_m5.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_hyperparameter_tuning_m5.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_model_results_m5.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_model_results_m5.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_model_results_police.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_model_results_police.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_model_results_prison.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_model_results_prison.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from gpforecaster.model.gpf import GPF
 
 
 class TestModel(unittest.TestCase):
     def setUp(self):
         self.data = tsag.preprocessing.PreprocessDatasets(
-            "prison", freq='Q'
+            "prison", freq="Q"
         ).apply_preprocess()
         self.n = self.data["predict"]["n"]
         self.s = self.data["train"]["s"]
-        self.res_type = 'fitpred'
-        self.res_measure = 'mean'
-        self.input_dir = './results/gpf/'
+        self.res_type = "fitpred"
+        self.res_measure = "mean"
+        self.input_dir = "./results/gpf/"
         self.gpf = GPF("tourism", self.data, input_dir=self.input_dir)
 
     def test_correct_train(self):
         model, like = self.gpf.train(epochs=10)
         self.assertIsNotNone(model)
 
     def test_predict_shape(self):
@@ -39,22 +39,30 @@
         res = self.gpf.metrics(preds[0], preds[1])
         self.assertLess(res["wall_time"]["wall_time_total"], 100)
 
     def test_output_results(self):
         model, like = self.gpf.train(epochs=10)
         preds, preds_scaled = self.gpf.predict(model, like)
         res = self.gpf.metrics(preds[0], preds[1])
-        self.gpf.store_results(res, res_type=self.res_type, res_measure=self.res_measure)
+        self.gpf.store_results(
+            res, res_type=self.res_type, res_measure=self.res_measure
+        )
         with open(
             f"{self.gpf.input_dir}results_{self.res_type}_{self.res_measure}_gp_{self.gpf.gp_type}_cov_{self.gpf.dataset}_{self.gpf.model_version}.pickle",
             "rb",
         ) as handle:
             output_res = pickle.load(file=handle)
         self.assertIsNotNone(output_res["mase"]["bottom"])
 
     def test_plot_loss_xvalidation(self):
         model, like = self.gpf.train(epochs=10)
         self.gpf.plot_losses()
 
     def test_plot_loss(self):
         model, like = self.gpf.train(epochs=10, cross_validation=False)
         self.gpf.plot_losses()
+
+    def test_no_validation(self):
+        model, like = self.gpf.train(
+            epochs=10, cross_validation=False, no_validation=True
+        )
+        self.gpf.plot_losses()
```

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_results_partial_data.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_results_partial_data.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_run_model_with_sampled_dataset.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_run_model_with_sampled_dataset.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_sparse_gps.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_sparse_gps.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_store_results.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_store_results.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_svg_gps.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_svg_gps.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/tests/test_tourism_gpf_with_local_file.py` & `gpforecaster-0.3.94/gpforecaster/tests/test_tourism_gpf_with_local_file.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/utils/logger.py` & `gpforecaster-0.3.94/gpforecaster/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster/visualization/plot_predictions.py` & `gpforecaster-0.3.94/gpforecaster/visualization/plot_predictions.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/gpforecaster.egg-info/PKG-INFO` & `gpforecaster-0.3.94/gpforecaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.93
+Version: 0.3.94
 Summary: Hierarchical time series forecasting model using Gaussian Processes
 Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
 Platform: UNKNOWN
```

### Comparing `gpforecaster-0.3.93/gpforecaster.egg-info/SOURCES.txt` & `gpforecaster-0.3.94/gpforecaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.93/setup.py` & `gpforecaster-0.3.94/setup.py`

 * *Files identical despite different names*

