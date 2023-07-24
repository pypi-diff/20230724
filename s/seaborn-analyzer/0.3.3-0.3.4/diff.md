# Comparing `tmp/seaborn-analyzer-0.3.3.tar.gz` & `tmp/seaborn-analyzer-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn-analyzer-0.3.3.tar", last modified: Sat Jun 24 22:37:57 2023, max compression
+gzip compressed data, was "seaborn-analyzer-0.3.4.tar", last modified: Mon Jul 24 02:50:24 2023, max compression
```

## Comparing `seaborn-analyzer-0.3.3.tar` & `seaborn-analyzer-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-24 22:37:57.817271 seaborn-analyzer-0.3.3/
--rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.3/LICENSE
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-24 22:37:57.817079 seaborn-analyzer-0.3.3/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-06-24 22:35:23.000000 seaborn-analyzer-0.3.3/README.rst
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-24 22:37:57.815336 seaborn-analyzer-0.3.3/seaborn_analyzer/
--rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-06-24 22:35:28.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/__init__.py
--rw-r--r--   0 knakamura   (501) staff       (20)    53228 2023-06-22 08:57:33.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/_cv_eval_set.py
--rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/_cv_eval_set_old.py
--rw-r--r--   0 knakamura   (501) staff       (20)    83193 2023-06-22 09:00:50.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/custom_class_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/custom_hist_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/custom_pair_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    98854 2023-06-24 07:21:33.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/custom_reg_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)     1620 2023-06-20 06:33:07.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/multiclass_fitparams.py
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-24 22:37:57.816118 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)      579 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/requires.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/top_level.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-06-24 22:37:57.817317 seaborn-analyzer-0.3.3/setup.cfg
--rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.3/setup.py
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-24 22:37:57.816738 seaborn-analyzer-0.3.3/tests/
--rw-r--r--   0 knakamura   (501) staff       (20)     8536 2023-06-24 22:25:10.000000 seaborn-analyzer-0.3.3/tests/test_class_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)     3376 2023-06-22 05:49:24.000000 seaborn-analyzer-0.3.3/tests/test_cv.py
--rw-r--r--   0 knakamura   (501) staff       (20)     8488 2023-06-24 22:18:27.000000 seaborn-analyzer-0.3.3/tests/test_reg_plot.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 02:50:24.786422 seaborn-analyzer-0.3.4/
+-rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.4/LICENSE
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-07-24 02:50:24.786251 seaborn-analyzer-0.3.4/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-07-24 02:49:57.000000 seaborn-analyzer-0.3.4/README.rst
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 02:50:24.785048 seaborn-analyzer-0.3.4/seaborn_analyzer/
+-rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-07-24 02:50:07.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/__init__.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53228 2023-06-22 08:57:33.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/_cv_eval_set.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/_cv_eval_set_old.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    83256 2023-07-24 02:43:09.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/custom_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/custom_hist_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/custom_pair_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    98934 2023-07-24 02:44:22.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/custom_reg_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     1620 2023-06-20 06:33:07.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/multiclass_fitparams.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 02:50:24.785719 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)      579 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/requires.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-07-24 02:50:24.786463 seaborn-analyzer-0.3.4/setup.cfg
+-rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.4/setup.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 02:50:24.786056 seaborn-analyzer-0.3.4/tests/
+-rw-r--r--   0 knakamura   (501) staff       (20)     8536 2023-06-24 22:25:10.000000 seaborn-analyzer-0.3.4/tests/test_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     3376 2023-06-22 05:49:24.000000 seaborn-analyzer-0.3.4/tests/test_cv.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     8488 2023-06-24 22:18:27.000000 seaborn-analyzer-0.3.4/tests/test_reg_plot.py
```

### Comparing `seaborn-analyzer-0.3.3/LICENSE` & `seaborn-analyzer-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/PKG-INFO` & `seaborn-analyzer-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.3
+Version: 0.3.4
 Summary: seaborn-analyzer: data visualization of regression, classification and distribution
 Home-page: https://github.com/c60evaporator/seaborn-analyzer
 Download-URL: https://github.com/c60evaporator/seaborn-analyzer
 Author: Kenta Nakamura
 Author-email: c60evaporator@gmail.com
 Maintainer: Kenta Nakamura
 Maintainer-email: c60evaporator@gmail.com
@@ -65,15 +65,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.3 requires
+seaborn-analyzer 0.3.4 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.3/README.rst` & `seaborn-analyzer-0.3.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.3 requires
+seaborn-analyzer 0.3.4 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer/_cv_eval_set.py` & `seaborn-analyzer-0.3.4/seaborn_analyzer/_cv_eval_set.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer/_cv_eval_set_old.py` & `seaborn-analyzer-0.3.4/seaborn_analyzer/_cv_eval_set_old.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer/custom_class_plot.py` & `seaborn-analyzer-0.3.4/seaborn_analyzer/custom_class_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         true_marker: str, optional
             Marker style of True label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
 
         false_marker: str, optional
             Marker style of False label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
 
         cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+            Determines the cross-validation splitting strategy. If None, no cross-validation is used and the training data is displayed. If int, to specify the number of folds in a KFold.
 
         cv_seed: int, optional
             Seed for random number generator of cross validation.
 
         cv_group: str, optional
             Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
 
@@ -724,15 +724,15 @@
         true_marker: str, optional
             Marker style of True label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
 
         false_marker: str, optional
             Marker style of False label. Available only if ``plot_scatter`` is set to 'error' or 'class_error'. See https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
 
         cv: int or sklearn.model_selection.*, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+            Determines the cross-validation splitting strategy. If None, no cross-validation is used and the training data is displayed. If int, to specify the number of folds in a KFold.
 
         cv_seed: int, optional
             Seed for random number generator of cross validation.
 
         cv_group: str, optional
             Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
 
@@ -1194,16 +1194,16 @@
 
         data: pd.DataFrame, default=None
             Input data structure.
 
         x_colnames: list[str], default=None
             Names of explanatory variables. Available only if ``data`` is NOT pd.DataFrame
 
-        cv: int or sklearn.model_selection.*, default=5
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+        cv: int or sklearn.model_selection.*, default=None
+            Determines the cross-validation splitting strategy. If None, no cross-validation is used and the training data is displayed. If int, to specify the number of folds in a KFold.
 
         cv_seed: int, default=42
             Seed for random number generator of cross validation.
 
         cv_group: str, optional
             Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
```

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer/custom_hist_plot.py` & `seaborn-analyzer-0.3.4/seaborn_analyzer/custom_hist_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer/custom_pair_plot.py` & `seaborn-analyzer-0.3.4/seaborn_analyzer/custom_pair_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer/custom_reg_plot.py` & `seaborn-analyzer-0.3.4/seaborn_analyzer/custom_reg_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         scores : {'r2', 'mae', 'mse', 'rmse', 'rmsle', 'mape', 'max_error'} or list, optional
             Regression score that are displayed at the lower right of the graph.
 
         cv_stats : {'mean', 'median', 'max', 'min'}, optional
             Statistical method of cross validation score that are displayed at the lower right of the graph.
 
         cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+            Determines the cross-validation splitting strategy. If None, no cross-validation is used and the training data is displayed. If int, to specify the number of folds in a KFold.
 
         cv_seed : int, optional
             Seed for random number generator of cross validation.
 
         cv_group: str, optional
             Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
 
@@ -640,15 +640,15 @@
         hue : str, optional
             Grouping variable that will produce points with different colors.
 
         aggregate : {'mean', 'median'}, optional
             Statistic method of aggregating explanatory variables except x_axis variable.
 
         cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+            Determines the cross-validation splitting strategy. If None, no cross-validation is used and the training data is displayed. If int, to specify the number of folds in a KFold.
 
         cv_seed : int, optional
             Seed for random number generator of cross validation.
 
         cv_group: str, optional
             Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
 
@@ -1001,15 +1001,15 @@
         scores : {'r2', 'mae', 'mse', 'rmse', 'rmsle', 'mape', 'max_error'} or list,, optional
             Regression score that are displayed at the lower right of the graph.
 
         cv_stats : {'mean', 'median', 'max', 'min'}, optional
             Statistical method of cross validation score that are displayed at the lower right of the graph.
 
         cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+            Determines the cross-validation splitting strategy. If None, no cross-validation is used and the training data is displayed. If int, to specify the number of folds in a KFold.
 
         cv_seed : int, optional
             Seed for random number generator of cross validation.
 
         cv_group: str, optional
             Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
 
@@ -1574,15 +1574,15 @@
         rank_number: int, optional
             Number of emphasized data that are in the top posiotions for regression error.
 
         rank_col: str, optional
             Variables that are displayed with emphasized data that are in the top posiotions for regression error.
 
         cv : int, cross-validation generator, or an iterable, optional
-            Determines the cross-validation splitting strategy. If None, to use the default 5-fold cross validation. If int, to specify the number of folds in a KFold.
+            Determines the cross-validation splitting strategy. If None, no cross-validation is used and the training data is displayed. If int, to specify the number of folds in a KFold.
 
         cv_seed : int, optional
             Seed for random number generator of cross validation.
 
         cv_group: str, optional
             Group variable for the samples used while splitting the dataset into train/test set. This argument is passed to ``groups`` argument of cv.split().
```

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer/multiclass_fitparams.py` & `seaborn-analyzer-0.3.4/seaborn_analyzer/multiclass_fitparams.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/PKG-INFO` & `seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.3
+Version: 0.3.4
 Summary: seaborn-analyzer: data visualization of regression, classification and distribution
 Home-page: https://github.com/c60evaporator/seaborn-analyzer
 Download-URL: https://github.com/c60evaporator/seaborn-analyzer
 Author: Kenta Nakamura
 Author-email: c60evaporator@gmail.com
 Maintainer: Kenta Nakamura
 Maintainer-email: c60evaporator@gmail.com
@@ -65,15 +65,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.3 requires
+seaborn-analyzer 0.3.4 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/SOURCES.txt` & `seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/setup.py` & `seaborn-analyzer-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/tests/test_class_plot.py` & `seaborn-analyzer-0.3.4/tests/test_class_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/tests/test_cv.py` & `seaborn-analyzer-0.3.4/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.3/tests/test_reg_plot.py` & `seaborn-analyzer-0.3.4/tests/test_reg_plot.py`

 * *Files identical despite different names*

