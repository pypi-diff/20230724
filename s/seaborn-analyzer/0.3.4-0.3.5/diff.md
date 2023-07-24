# Comparing `tmp/seaborn-analyzer-0.3.4.tar.gz` & `tmp/seaborn-analyzer-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn-analyzer-0.3.4.tar", last modified: Mon Jul 24 02:50:24 2023, max compression
+gzip compressed data, was "seaborn-analyzer-0.3.5.tar", last modified: Mon Jul 24 03:16:21 2023, max compression
```

## Comparing `seaborn-analyzer-0.3.4.tar` & `seaborn-analyzer-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 02:50:24.786422 seaborn-analyzer-0.3.4/
--rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.4/LICENSE
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-07-24 02:50:24.786251 seaborn-analyzer-0.3.4/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-07-24 02:49:57.000000 seaborn-analyzer-0.3.4/README.rst
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 02:50:24.785048 seaborn-analyzer-0.3.4/seaborn_analyzer/
--rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-07-24 02:50:07.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/__init__.py
--rw-r--r--   0 knakamura   (501) staff       (20)    53228 2023-06-22 08:57:33.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/_cv_eval_set.py
--rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/_cv_eval_set_old.py
--rw-r--r--   0 knakamura   (501) staff       (20)    83256 2023-07-24 02:43:09.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/custom_class_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/custom_hist_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/custom_pair_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    98934 2023-07-24 02:44:22.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/custom_reg_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)     1620 2023-06-20 06:33:07.000000 seaborn-analyzer-0.3.4/seaborn_analyzer/multiclass_fitparams.py
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 02:50:24.785719 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)      579 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/requires.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-07-24 02:50:24.000000 seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/top_level.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-07-24 02:50:24.786463 seaborn-analyzer-0.3.4/setup.cfg
--rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.4/setup.py
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 02:50:24.786056 seaborn-analyzer-0.3.4/tests/
--rw-r--r--   0 knakamura   (501) staff       (20)     8536 2023-06-24 22:25:10.000000 seaborn-analyzer-0.3.4/tests/test_class_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)     3376 2023-06-22 05:49:24.000000 seaborn-analyzer-0.3.4/tests/test_cv.py
--rw-r--r--   0 knakamura   (501) staff       (20)     8488 2023-06-24 22:18:27.000000 seaborn-analyzer-0.3.4/tests/test_reg_plot.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 03:16:21.979709 seaborn-analyzer-0.3.5/
+-rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.5/LICENSE
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-07-24 03:16:21.979538 seaborn-analyzer-0.3.5/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-07-24 03:15:51.000000 seaborn-analyzer-0.3.5/README.rst
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 03:16:21.978376 seaborn-analyzer-0.3.5/seaborn_analyzer/
+-rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-07-24 03:15:44.000000 seaborn-analyzer-0.3.5/seaborn_analyzer/__init__.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53228 2023-06-22 08:57:33.000000 seaborn-analyzer-0.3.5/seaborn_analyzer/_cv_eval_set.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.5/seaborn_analyzer/_cv_eval_set_old.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    83256 2023-07-24 02:43:09.000000 seaborn-analyzer-0.3.5/seaborn_analyzer/custom_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.5/seaborn_analyzer/custom_hist_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    12208 2023-07-24 03:13:58.000000 seaborn-analyzer-0.3.5/seaborn_analyzer/custom_pair_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    98934 2023-07-24 02:44:22.000000 seaborn-analyzer-0.3.5/seaborn_analyzer/custom_reg_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     1620 2023-06-20 06:33:07.000000 seaborn-analyzer-0.3.5/seaborn_analyzer/multiclass_fitparams.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 03:16:21.979021 seaborn-analyzer-0.3.5/seaborn_analyzer.egg-info/
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-07-24 03:16:21.000000 seaborn-analyzer-0.3.5/seaborn_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)      579 2023-07-24 03:16:21.000000 seaborn-analyzer-0.3.5/seaborn_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-07-24 03:16:21.000000 seaborn-analyzer-0.3.5/seaborn_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-07-24 03:16:21.000000 seaborn-analyzer-0.3.5/seaborn_analyzer.egg-info/requires.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-07-24 03:16:21.000000 seaborn-analyzer-0.3.5/seaborn_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-07-24 03:16:21.979753 seaborn-analyzer-0.3.5/setup.cfg
+-rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.5/setup.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-07-24 03:16:21.979347 seaborn-analyzer-0.3.5/tests/
+-rw-r--r--   0 knakamura   (501) staff       (20)     8536 2023-06-24 22:25:10.000000 seaborn-analyzer-0.3.5/tests/test_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     3376 2023-06-22 05:49:24.000000 seaborn-analyzer-0.3.5/tests/test_cv.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     8488 2023-06-24 22:18:27.000000 seaborn-analyzer-0.3.5/tests/test_reg_plot.py
```

### Comparing `seaborn-analyzer-0.3.4/LICENSE` & `seaborn-analyzer-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/PKG-INFO` & `seaborn-analyzer-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.4
+Version: 0.3.5
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
-seaborn-analyzer 0.3.4 requires
+seaborn-analyzer 0.3.5 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.4/README.rst` & `seaborn-analyzer-0.3.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.4 requires
+seaborn-analyzer 0.3.5 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer/_cv_eval_set.py` & `seaborn-analyzer-0.3.5/seaborn_analyzer/_cv_eval_set.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer/_cv_eval_set_old.py` & `seaborn-analyzer-0.3.5/seaborn_analyzer/_cv_eval_set_old.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer/custom_class_plot.py` & `seaborn-analyzer-0.3.5/seaborn_analyzer/custom_class_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer/custom_hist_plot.py` & `seaborn-analyzer-0.3.5/seaborn_analyzer/custom_hist_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer/custom_pair_plot.py` & `seaborn-analyzer-0.3.5/seaborn_analyzer/custom_pair_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,31 +185,32 @@
         lower_kws : dict
             Additional parameters passed to seaborn.PairGrid.map_lower(). If ``lowerkind`` is 'scatter', the arguments are applied to seaborn.scatterplot method of the lower subplots.
         diag_kws : dict
             Additional parameters passed to seaborn.PairGrid.map_diag(). If ``lowerkind`` is 'kde', the arguments are applied to seaborn.kdeplot method of the diagonal subplots.
         grid_kws : dict
             Additional parameters passed to seaborn.PairGrid.__init__() other than the above arguments. See https://seaborn.pydata.org/generated/seaborn.PairGrid.html
         """
+        # int, float, bool型の列のみを選択
+        self.df = df.select_dtypes(include=[int, float, bool])
         # bool型の列をintに変換
-        self.df = df.copy()
         bool_cols = self.df.select_dtypes(include=bool).columns
         for col in bool_cols:
             self.df[col] = self.df[col] * 1
         #メンバ変数入力
         self.hue = hue
-        self.corr_mat = df.corr(method="pearson")
+        self.corr_mat = self.df.corr(method="pearson")
         #文字サイズ調整
         sns.set_context("notebook")
 
         #PairGridインスタンス作成
         plt.figure()
         diag_sharey = diag_kind == "hist"
         g = sns.PairGrid(self.df, hue=self.hue,
                  palette=palette, vars=vars, diag_sharey=diag_sharey,
-                 height=height, aspect=aspect, dropna=dropna, size=None, **grid_kws)
+                 height=height, aspect=aspect, dropna=dropna, **grid_kws)
         self.hue_names = g.hue_names
 
         #マーカーを設定
         if markers is not None:
             if g.hue_names is None:
                 n_markers = 1
             else:
```

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer/custom_reg_plot.py` & `seaborn-analyzer-0.3.5/seaborn_analyzer/custom_reg_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer/multiclass_fitparams.py` & `seaborn-analyzer-0.3.5/seaborn_analyzer/multiclass_fitparams.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/PKG-INFO` & `seaborn-analyzer-0.3.5/seaborn_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.4
+Version: 0.3.5
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
-seaborn-analyzer 0.3.4 requires
+seaborn-analyzer 0.3.5 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.4/seaborn_analyzer.egg-info/SOURCES.txt` & `seaborn-analyzer-0.3.5/seaborn_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/setup.py` & `seaborn-analyzer-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/tests/test_class_plot.py` & `seaborn-analyzer-0.3.5/tests/test_class_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/tests/test_cv.py` & `seaborn-analyzer-0.3.5/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.4/tests/test_reg_plot.py` & `seaborn-analyzer-0.3.5/tests/test_reg_plot.py`

 * *Files identical despite different names*

