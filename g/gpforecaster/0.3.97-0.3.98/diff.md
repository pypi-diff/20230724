# Comparing `tmp/gpforecaster-0.3.97.tar.gz` & `tmp/gpforecaster-0.3.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpforecaster-0.3.97.tar", last modified: Mon Jul 24 19:30:56 2023, max compression
+gzip compressed data, was "gpforecaster-0.3.98.tar", last modified: Mon Jul 24 19:55:28 2023, max compression
```

## Comparing `gpforecaster-0.3.97.tar` & `gpforecaster-0.3.98.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:56.512311 gpforecaster-0.3.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 19:30:56.512311 gpforecaster-0.3.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:56.508311 gpforecaster-0.3.97/gpforecaster/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:56.508311 gpforecaster-0.3.97/gpforecaster/model/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/model/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    42908 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/model/gpf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/model/hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/model/mean_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/model/mlls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:56.508311 gpforecaster-0.3.97/gpforecaster/results/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/results/calculate_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:56.512311 gpforecaster-0.3.97/gpforecaster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_calculate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_hyperparameter_tuning_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_model_results_m5.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_model_results_police.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_model_results_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_results_partial_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_run_model_with_sampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_sparse_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_store_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_svg_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/tests/test_tourism_gpf_with_local_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:56.512311 gpforecaster-0.3.97/gpforecaster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:56.512311 gpforecaster-0.3.97/gpforecaster/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/gpforecaster/visualization/plot_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:30:56.508311 gpforecaster-0.3.97/gpforecaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 19:30:56.000000 gpforecaster-0.3.97/gpforecaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 19:30:56.000000 gpforecaster-0.3.97/gpforecaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:30:56.000000 gpforecaster-0.3.97/gpforecaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 19:30:56.000000 gpforecaster-0.3.97/gpforecaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 19:30:56.000000 gpforecaster-0.3.97/gpforecaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:30:56.512311 gpforecaster-0.3.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-24 19:30:44.000000 gpforecaster-0.3.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:28.518133 gpforecaster-0.3.98/gpforecaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/gpforecaster/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/model/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42908 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/model/gpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/model/hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/model/mean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/model/mlls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/gpforecaster/results/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/results/calculate_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/gpforecaster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_calculate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_hyperparameter_tuning_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_model_results_m5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_model_results_police.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_model_results_prison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_results_partial_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_run_model_with_sampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_sparse_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_store_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_svg_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/tests/test_tourism_gpf_with_local_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/gpforecaster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/gpforecaster/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/gpforecaster/visualization/plot_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/gpforecaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 19:55:28.000000 gpforecaster-0.3.98/gpforecaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 19:55:28.000000 gpforecaster-0.3.98/gpforecaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:55:28.000000 gpforecaster-0.3.98/gpforecaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 19:55:28.000000 gpforecaster-0.3.98/gpforecaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 19:55:28.000000 gpforecaster-0.3.98/gpforecaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:55:28.522133 gpforecaster-0.3.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-24 19:55:15.000000 gpforecaster-0.3.98/setup.py
```

### Comparing `gpforecaster-0.3.97/LICENCE` & `gpforecaster-0.3.98/LICENCE`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/PKG-INFO` & `gpforecaster-0.3.98/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.97
+Version: 0.3.98
 Summary: Hierarchical time series forecasting model using Gaussian Processes
 Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
 Platform: UNKNOWN
```

### Comparing `gpforecaster-0.3.97/README.md` & `gpforecaster-0.3.98/README.md`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/model/gp.py` & `gpforecaster-0.3.98/gpforecaster/model/gp.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/model/gpf.py` & `gpforecaster-0.3.98/gpforecaster/model/gpf.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/model/hyperparameter_tuning.py` & `gpforecaster-0.3.98/gpforecaster/model/hyperparameter_tuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     # Define the search space for hyperparameters
     search_space = [
         Real(1e-3, 1e-2, name="learning_rates"),
         Real(1e-6, 1e-3, name="weight_decays"),
         Categorical(["step", "exponential", "cosine", "none"], name="scheduler_types"),
         Real(0.1, 0.95, name="gamma_rates"),
-        Integer(5, 6, name="patiences"), # patience is not very relevant to GPs and our setup
+        Integer(15, 16, name="patiences"), # patience is not very relevant to GPs and our setup
         Real(0.85, 1.15, name="rbf_kernel_lengthscale"),
         Real(0.35, 0.6, name="scale_rbf_kernel_outputscale"),
         Real(0.35, 0.6, name="periodic_kernel_lengthscale"),
         Real(1.4, 1.75, name="scale_periodic_kernel_outputscale"),
         Real(0.075, 0.3, name="m"),
         Real(0.075, 0.3, name="k"),
         Real(0.075, 0.35, name="b")
```

### Comparing `gpforecaster-0.3.97/gpforecaster/model/mean_functions.py` & `gpforecaster-0.3.98/gpforecaster/model/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/model/mlls.py` & `gpforecaster-0.3.98/gpforecaster/model/mlls.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/results/calculate_metrics.py` & `gpforecaster-0.3.98/gpforecaster/results/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_calculate_results.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_calculate_results.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_early_stopping.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_hyperparameter_tuning.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_hyperparameter_tuning_m5.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_hyperparameter_tuning_m5.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_model_results_m5.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_model_results_m5.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_model_results_police.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_model_results_police.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_model_results_prison.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_model_results_prison.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_results_partial_data.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_results_partial_data.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_run_model_with_sampled_dataset.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_run_model_with_sampled_dataset.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_sparse_gps.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_sparse_gps.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_store_results.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_store_results.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_svg_gps.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_svg_gps.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/tests/test_tourism_gpf_with_local_file.py` & `gpforecaster-0.3.98/gpforecaster/tests/test_tourism_gpf_with_local_file.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/utils/logger.py` & `gpforecaster-0.3.98/gpforecaster/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster/visualization/plot_predictions.py` & `gpforecaster-0.3.98/gpforecaster/visualization/plot_predictions.py`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/gpforecaster.egg-info/PKG-INFO` & `gpforecaster-0.3.98/gpforecaster.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpforecaster
-Version: 0.3.97
+Version: 0.3.98
 Summary: Hierarchical time series forecasting model using Gaussian Processes
 Home-page: UNKNOWN
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 License: UNKNOWN
 Keywords: python,time series,hierarchical,forecasting,gaussian process,machine learning
 Platform: UNKNOWN
```

### Comparing `gpforecaster-0.3.97/gpforecaster.egg-info/SOURCES.txt` & `gpforecaster-0.3.98/gpforecaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpforecaster-0.3.97/setup.py` & `gpforecaster-0.3.98/setup.py`

 * *Files identical despite different names*

