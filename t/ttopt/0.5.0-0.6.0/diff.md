# Comparing `tmp/ttopt-0.5.0.tar.gz` & `tmp/ttopt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttopt-0.5.0.tar", last modified: Wed Aug 31 16:55:04 2022, max compression
+gzip compressed data, was "ttopt-0.6.0.tar", last modified: Mon Jul 24 16:15:11 2023, max compression
```

## Comparing `ttopt-0.5.0.tar` & `ttopt-0.6.0.tar`

### file list

```diff
@@ -1,71 +1,27 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.539500 ttopt-0.5.0/
--rw-r--r--   0 andrei     (501) staff       (20)     1116 2022-03-11 11:20:02.000000 ttopt-0.5.0/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)      125 2022-08-15 15:56:36.000000 ttopt-0.5.0/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     6662 2022-08-31 16:55:04.539863 ttopt-0.5.0/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     4721 2022-08-31 16:48:20.000000 ttopt-0.5.0/README.md
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.488605 ttopt-0.5.0/demo/
--rw-r--r--   0 andrei     (501) staff       (20)     2406 2022-05-03 20:27:26.000000 ttopt-0.5.0/demo/base.py
--rw-r--r--   0 andrei     (501) staff       (20)     2498 2022-05-03 20:27:17.000000 ttopt-0.5.0/demo/cache.py
--rw-r--r--   0 andrei     (501) staff       (20)     2637 2022-05-03 20:27:07.000000 ttopt-0.5.0/demo/qtt.py
--rw-r--r--   0 andrei     (501) staff       (20)     2521 2022-05-03 20:27:13.000000 ttopt-0.5.0/demo/qtt_100d.py
--rw-r--r--   0 andrei     (501) staff       (20)     2339 2022-07-22 10:45:27.000000 ttopt-0.5.0/demo/qtt_max.py
--rw-r--r--   0 andrei     (501) staff       (20)     2586 2022-05-03 20:26:52.000000 ttopt-0.5.0/demo/tensor.py
--rw-r--r--   0 andrei     (501) staff       (20)     3126 2022-05-03 20:34:09.000000 ttopt-0.5.0/demo/tensor_init_spec.py
--rw-r--r--   0 andrei     (501) staff       (20)     2473 2022-05-03 20:26:45.000000 ttopt-0.5.0/demo/vect.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.489306 ttopt-0.5.0/demo_calc/
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.490215 ttopt-0.5.0/demo_calc/__pycache__/
--rw-r--r--   0 andrei     (501) staff       (20)    11935 2022-04-09 16:42:55.000000 ttopt-0.5.0/demo_calc/__pycache__/demo_func.cpython-38.pyc
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.497469 ttopt-0.5.0/demo_calc/opt/
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.505548 ttopt-0.5.0/demo_calc/opt/__pycache__/
--rw-r--r--   0 andrei     (501) staff       (20)    14303 2022-04-09 16:42:55.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/es.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     3138 2022-05-18 08:33:18.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1201 2022-05-18 09:28:40.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt_de.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1231 2022-05-17 16:50:56.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt_es.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1361 2022-05-17 16:50:56.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt_es_cma.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1215 2022-05-17 16:50:56.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt_ga.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1259 2022-05-18 12:10:21.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt_meta_model.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1218 2022-05-18 12:34:40.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt_nb.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1208 2022-05-18 09:28:39.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt_pso.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1682 2022-05-18 08:33:18.000000 ttopt-0.5.0/demo_calc/opt/__pycache__/opt_tt_opt.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)    19226 2022-01-22 10:21:50.000000 ttopt-0.5.0/demo_calc/opt/es.py
--rw-r--r--   0 andrei     (501) staff       (20)     3045 2022-05-18 08:29:29.000000 ttopt-0.5.0/demo_calc/opt/opt.py
--rw-r--r--   0 andrei     (501) staff       (20)      711 2022-05-18 09:27:17.000000 ttopt-0.5.0/demo_calc/opt/opt_de.py
--rw-r--r--   0 andrei     (501) staff       (20)      856 2022-05-17 15:38:41.000000 ttopt-0.5.0/demo_calc/opt/opt_es.py
--rw-r--r--   0 andrei     (501) staff       (20)      981 2022-05-17 15:39:40.000000 ttopt-0.5.0/demo_calc/opt/opt_es_cma.py
--rw-r--r--   0 andrei     (501) staff       (20)      829 2022-05-17 15:39:43.000000 ttopt-0.5.0/demo_calc/opt/opt_ga.py
--rw-r--r--   0 andrei     (501) staff       (20)      729 2022-05-18 12:32:35.000000 ttopt-0.5.0/demo_calc/opt/opt_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      715 2022-05-18 09:26:21.000000 ttopt-0.5.0/demo_calc/opt/opt_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)     1259 2022-05-18 08:29:39.000000 ttopt-0.5.0/demo_calc/opt/opt_tt_opt.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.512167 ttopt-0.5.0/demo_calc/res_data/
--rw-r--r--   0 andrei     (501) staff       (20)    36385 2022-05-18 17:19:47.000000 ttopt-0.5.0/demo_calc/res_data/calc1_comp_10dim.pickle
--rw-r--r--   0 andrei     (501) staff       (20)     7601 2022-05-24 05:34:13.000000 ttopt-0.5.0/demo_calc/res_data/calc1_dims_500dim.pickle
--rw-r--r--   0 andrei     (501) staff       (20)    38061 2022-05-23 21:14:22.000000 ttopt-0.5.0/demo_calc/res_data/calc1_iter_10dim.pickle
--rw-r--r--   0 andrei     (501) staff       (20)   113953 2022-05-22 19:53:40.000000 ttopt-0.5.0/demo_calc/res_data/calc1_quan_10dim.pickle
--rw-r--r--   0 andrei     (501) staff       (20)    54301 2022-05-22 17:28:28.000000 ttopt-0.5.0/demo_calc/res_data/calc1_rank_10dim.pickle
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.525357 ttopt-0.5.0/demo_calc/res_logs/
--rw-r--r--   0 andrei     (501) staff       (20)    39428 2022-05-18 17:19:47.000000 ttopt-0.5.0/demo_calc/res_logs/calc1_comp_10dim.txt
--rw-r--r--   0 andrei     (501) staff       (20)     4067 2022-05-25 14:48:53.000000 ttopt-0.5.0/demo_calc/res_logs/calc1_dims_500dim.txt
--rw-r--r--   0 andrei     (501) staff       (20)    50808 2022-05-23 21:14:22.000000 ttopt-0.5.0/demo_calc/res_logs/calc1_iter_10dim.txt
--rw-r--r--   0 andrei     (501) staff       (20)   150508 2022-05-22 19:53:40.000000 ttopt-0.5.0/demo_calc/res_logs/calc1_quan_10dim.txt
--rw-r--r--   0 andrei     (501) staff       (20)    72408 2022-05-22 17:28:28.000000 ttopt-0.5.0/demo_calc/res_logs/calc1_rank_10dim.txt
--rw-r--r--   0 andrei     (501) staff       (20)     6535 2022-05-25 14:52:42.000000 ttopt-0.5.0/demo_calc/res_logs/calc1_show_10dim.txt
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.528621 ttopt-0.5.0/demo_calc/res_plot/
--rw-r--r--   0 andrei     (501) staff       (20)    91754 2022-05-25 14:52:42.000000 ttopt-0.5.0/demo_calc/res_plot/calc1_iter_10dim.png
--rw-r--r--   0 andrei     (501) staff       (20)   144990 2022-05-25 14:52:42.000000 ttopt-0.5.0/demo_calc/res_plot/calc1_rank_10dim.png
--rw-r--r--   0 andrei     (501) staff       (20)    14189 2022-08-08 09:54:39.000000 ttopt-0.5.0/demo_calc/run.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.533392 ttopt-0.5.0/demo_calc_2/
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.534254 ttopt-0.5.0/demo_calc_2/__pycache__/
--rw-r--r--   0 andrei     (501) staff       (20)     2226 2022-08-08 09:52:41.000000 ttopt-0.5.0/demo_calc_2/__pycache__/func_demo_brown.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1462 2022-08-08 09:50:15.000000 ttopt-0.5.0/demo_calc_2/func_demo_brown.py
--rw-r--r--   0 andrei     (501) staff       (20)     4278 2022-08-08 10:30:53.000000 ttopt-0.5.0/demo_calc_2/run.py
--rw-r--r--   0 andrei     (501) staff       (20)      107 2022-08-31 16:55:04.540909 ttopt-0.5.0/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2344 2022-08-31 16:48:04.000000 ttopt-0.5.0/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.537121 ttopt-0.5.0/ttopt/
--rw-r--r--   0 andrei     (501) staff       (20)      178 2022-08-31 16:48:42.000000 ttopt-0.5.0/ttopt/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)    22353 2022-07-22 10:42:35.000000 ttopt-0.5.0/ttopt/ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)    11286 2022-07-22 10:42:08.000000 ttopt-0.5.0/ttopt/ttopt_raw.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-08-31 16:55:04.539017 ttopt-0.5.0/ttopt.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     6662 2022-08-31 16:55:04.000000 ttopt-0.5.0/ttopt.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1759 2022-08-31 16:55:04.000000 ttopt-0.5.0/ttopt.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2022-08-31 16:55:04.000000 ttopt-0.5.0/ttopt.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)        6 2022-08-31 16:55:04.000000 ttopt-0.5.0/ttopt.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-24 16:15:11.463343 ttopt-0.6.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1116 2023-05-20 17:13:27.000000 ttopt-0.6.0/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       63 2023-07-24 14:15:32.000000 ttopt-0.6.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     4248 2023-07-24 16:15:11.463508 ttopt-0.6.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     3035 2023-07-24 15:09:50.000000 ttopt-0.6.0/README.md
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-24 16:15:11.459334 ttopt-0.6.0/demo/
+-rw-r--r--   0 andrei     (501) staff       (20)     2414 2023-07-24 16:07:54.000000 ttopt-0.6.0/demo/base.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2509 2023-07-24 16:09:42.000000 ttopt-0.6.0/demo/cache.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2645 2023-07-24 16:08:17.000000 ttopt-0.6.0/demo/qtt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2529 2023-07-24 16:09:08.000000 ttopt-0.6.0/demo/qtt_100d.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2352 2023-07-24 16:08:38.000000 ttopt-0.6.0/demo/qtt_max.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2594 2023-07-24 16:09:58.000000 ttopt-0.6.0/demo/tensor.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3134 2023-07-24 16:10:18.000000 ttopt-0.6.0/demo/tensor_init.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2484 2023-07-24 16:09:22.000000 ttopt-0.6.0/demo/vect.py
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-24 16:15:11.464076 ttopt-0.6.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2412 2023-07-24 14:16:39.000000 ttopt-0.6.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-24 16:15:11.460947 ttopt-0.6.0/ttopt/
+-rw-r--r--   0 andrei     (501) staff       (20)      178 2023-07-24 16:13:50.000000 ttopt-0.6.0/ttopt/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5267 2023-07-24 14:11:36.000000 ttopt-0.6.0/ttopt/maxvol.py
+-rw-r--r--   0 andrei     (501) staff       (20)    22561 2023-07-24 15:59:59.000000 ttopt-0.6.0/ttopt/ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)    10763 2023-07-24 16:06:35.000000 ttopt-0.6.0/ttopt/ttopt_raw.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-24 16:15:11.463059 ttopt-0.6.0/ttopt.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     4248 2023-07-24 16:15:11.000000 ttopt-0.6.0/ttopt.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      384 2023-07-24 16:15:11.000000 ttopt-0.6.0/ttopt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-24 16:15:11.000000 ttopt-0.6.0/ttopt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      163 2023-07-24 16:15:11.000000 ttopt-0.6.0/ttopt.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        6 2023-07-24 16:15:11.000000 ttopt-0.6.0/ttopt.egg-info/top_level.txt
```

### Comparing `ttopt-0.5.0/LICENSE.txt` & `ttopt-0.6.0/LICENSE.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021-2022 Andrei Chertkov, Ivan Oseledets, Roman Schutski, Konstantin Sozykin
+Copyright (C) 2021-2023 Andrei Chertkov, Ivan Oseledets, Roman Schutski, Konstantin Sozykin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `ttopt-0.5.0/README.md` & `ttopt-0.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,64 @@
+Metadata-Version: 2.1
+Name: ttopt
+Version: 0.6.0
+Summary: Multivariate function optimizer based on the tensor train approach.
+Home-page: https://github.com/AndreiChertkov/ttopt
+Author: Andrei Chertkov
+Author-email: andre.chertkov@gmail.com
+Project-URL: Source, https://github.com/AndreiChertkov/ttopt
+Keywords: function optimization function minimization low-rank representation tensor train format TT-decomposition cross approximation
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # ttopt
 
-> Gradient-free optimization method for multivariable functions based on the low rank tensor train (TT) format and maximal-volume principle.
+
+## Description
+
+Gradient-free optimization method for multivariable functions based on the low rank tensor train (TT) format and maximal-volume principle.
+
+> Please, see also our software product [teneva](https://github.com/AndreiChertkov/teneva) which provides a very compact implementation of basic operations in the TT-format.
 
 
 ## Installation
 
-1. Install [python](https://www.python.org) (version >= 3.7; you may use [anaconda](https://www.anaconda.com) package manager);
-2. Install basic dependencies:
-    ```bash
-    pip install numpy cython scipy
-    ```
-3. Install additional dependency [maxvolpy](https://bitbucket.org/muxas/maxvolpy/src/master/) with effective realization of `maxvol` algorithm:
-    ```bash
-    pip install maxvolpy
-    ```
-    > Note that [teneva](https://github.com/AndreiChertkov/teneva) python package may be used instead (`pip install teneva`)
-4. Install dependencies for demo calculations (it is optional):
-    ```bash
-    pip install matplotlib cma nevergrad pyproj teneva
-    ```
-5. Install the `ttopt` package:
-    ```bash
-    python setup.py install
-    ```
-    > You may also use the pip for installation, i.e., `pip install ttopt`
+You can install the `ttopt` package for `python >= 3.7` with pip:
+```bash
+pip install ttopt>=0.6.0
+```
 
 
 ## Examples
 
 The demo-scripts with detailed comments are collected in the folder `demo`:
 
 - `base.py` - we find the minimum for the 10-dimensional function with vectorized input;
 - `qtt.py` - we do almost the same as in the `base.py` script, but use the QTT-based approach (note that results are much more better then in the `base.py` example);
+- `qtt_max.py` - we do almost the same as in the `qtt.py`, but consider the maximization task;
 - `qtt_100d.py` - we do almost the same as in the `qtt.py` script, but approximate the 100-dimensional function;
 - `vect.py` - we find the minimum for the simple analytic function with "simple input" (the function is not vectorized);
-- `cache.py` - we find the minimum for the simple analytic function to demonstrate the usage of cache;
-- `tensor.py` - in this example we find the minimum for the multidimensional array/tensor (i.e., discrete function).
-- `tensor_init_spec` - we do almost the same as in the `tensor.py` script, but use special method of initialization (instead of a random tensor, we select a set of starting multi-indices for the search).
-
-> The folder `check` contains a number of additional calculations related to the study of the algorithm and the evaluation of its performance. A more accurate assessment of the accuracy and efficiency of the TTOpt approach is given in the folder `demo_calc` (see description below).
-
-
-## Calculations for benchmarks
+- `cache.py` - we find the minimum for the simple analytic function to demonstrate the usage of the cache;
+- `tensor.py` - in this example we find the minimum for the multidimensional array/tensor (i.e., discrete function);
+- `tensor_init` - we do almost the same as in the `tensor.py` script, but we use special method of initialization (instead of a random tensor, we select a set of starting multi-indices for the search).
 
-The scripts for comparison of our approach with baselines (ES algorithms and some baselines from the `nevergrad` package) for the analytical benchmark functions are located in the folder `demo_calc`. To run calculations, you can proceed as follows `python demo_calc/run.py --KIND`. Possible values for `KIND`: `comp` - compare different solvers; `dims` - check dependency on dimension number; `iter` - check dependency on number of calls for the target function; `quan` - check effect of the QTT-usage; `rank` - check dependency on the rank; `show` - show results of the previous calculations.
-
-> All results will be collected in the folders `demo_calc/res_data` (saved results in the pickle format), `demo_calc/res_logs` (text files with logs) and `demo_calc/res_plot` (figures with results).
-
-To reproduce the results from the paper (it is currently in the process of being published), run the following scripts from the root folder of the package:
-1. Run `python demo_calc/run.py -d 10 -p 2 -q 25 -r 4 --evals 1.E+5 --reps 10 --kind comp`;
-2. Run `python demo_calc/run.py -p 2 -q 25 -r 4 --reps 1 --kind dims`;
-3. Run `python demo_calc/run.py -d 10 -p 2 -q 25 -r 4 --reps 10 --kind iter`;
-4. Run `python demo_calc/run.py -d 10 -r 4 --evals 1.E+5 --reps 10 --kind quan`;
-5. Run `python demo_calc/run.py -d 10 -p 2 -q 25 --evals 1.E+5 --reps 10 --kind rank`;
-6. Run `python demo_calc/run.py -d 10 --kind show`. The results will be saved to the `demo_calc/res_logs` and `demo_calc/res_plot` folders.
-
-> Additional comparison with gradient-based methods is presented in the `demo_calc_2` folder.
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Ivan Oseledets](https://github.com/oseledets)
 - [Roman Schutski](https://github.com/Qbit-)
 - [Konstantin Sozykin](https://github.com/gogolgrind)
@@ -69,14 +68,22 @@
 
 If you find this approach and/or code useful in your research, please consider citing:
 
 ```bibtex
 @article{sozykin2022ttopt,
     author    = {Sozykin, Konstantin and Chertkov, Andrei and Schutski, Roman and Phan, Anh-Huy and Cichocki, Andrzej and Oseledets, Ivan},
     year      = {2022},
-    title     = {TTOpt: A Maximum Volume Quantized Tensor Train-based Optimization and its Application to Reinforcement Learning},
-    journal   = {ArXiv},
-    volume    = {abs/2205.00293},
-    doi       = {10.48550/ARXIV.2205.00293},
-    url       = {https://arxiv.org/abs/2205.00293}
+    title     = {{TTOpt}: {A} maximum volume quantized tensor train-based optimization and its application to reinforcement learning},
+    journal   = {Advances in Neural Information Processing Systems},
+    volume    = {35},
+    pages     = {26052--26065},
+    url       = {https://proceedings.neurips.cc/paper_files/paper/2022/hash/a730abbcd6cf4a371ca9545db5922442-Abstract-Conference.html}
 }
 ```
+
+> Please, note that the calculations presented in this paper correspond to version `<0.5.0` of the `ttopt` package (and to very old version of the `teneva` package), to run the calculations, please use the appropriate version. In the new versions `>=0.6.0`, we have removed all the corresponding folders in the folder `computations_old`. In the future, we will try to update the interface of these experiments.
+
+
+---
+
+
+> ✭__🚂  The stars that you give to **ttopt**, motivate us to develop faster and add new interesting features to the code 😃
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ttopt-0.5.0/demo/base.py` & `ttopt-0.6.0/demo/tensor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,74 @@
-"""The demo of using ttopt. Basic example.
+"""The demo of using ttopt. Example for tensor minimization.
 
-We'll find the minimum for the 10-dimensional Alpine function with vectorized
-input. The target function for minimization has the form f(X), where input X is
-the [samples, dimension] numpy array.
+We'll find the minimum for the given simple d-dimensional tensor with elements:
+Y[i_1, i_2, ..., i_d] = (i_1 - 2)^2 + (i_2 - 3)^2 + i_2^4 + i_3^4 + ... + i_d^4.
 
-Run it from the root of the project as "python demo/base.py".
+Run it from the root of the project as "python demo/tensor.py".
 
 As a result of the script work we expect the output in console like this:
 "
 ...
-Alpine-10d | k=1.00e+05 | t_cur=2.39e-02 | e_x=5.02e-01 e_y=9.22e-02
+Tensor-10d | evals=1.00e+05 | t_cur=8.64e-03 | e_x=0.00e+00 e_y=0.00e+00
 ----------------------------------------------------------------------
-Alpine-10d | k=1.00e+05 | t_all=1.12e-01 | e_x=5.02e-01 e_y=9.22e-02
+Tensor-10d | evals=1.00e+05 | t_all=2.03e-01 | e_x=0.00e+00 e_y=0.00e+00
+y_opt :  0
+i_opt :  [2 3 0 0 0 0 0 0 0 0]
 "
 
 """
 import numpy as np
 
 
 from ttopt import TTOpt
 from ttopt import ttopt_init
 
 
 np.random.seed(42)
 
 
-d = 10                      # Number of function dimensions:
-rmax = 4                    # Maximum TT-rank while cross-like iterations
-def f(X):                   # Target function
-    return np.sum(np.abs(X * np.sin(X) + 0.1 * X), axis=1)
+d = 10                      # Number of function dimensions
+p = 2
+q = 10
+n = p**q                    # Mode size for the tensor
+rank = 2                    # Maximum TT-rank while cross-like iterations
+def f(I):                   # Target function (return tensor element)
+    return (I[:, 0] - 2)**2 + (I[:, 1] - 3)**2 + np.sum(I[:, 2:]**4, axis=1)
+
+
+# Real value of x-minima:
+x_min_real = np.zeros(d)
+x_min_real[0] = 2
+x_min_real[1] = 3
 
 
 # We initialize the TTOpt class instance with the correct parameters:
 tto = TTOpt(
     f=f,                    # Function for minimization. X is [samples, dim]
     d=d,                    # Number of function dimensions
-    a=-10.,                 # Grid lower bound (number or list of len d)
-    b=+10.,                 # Grid upper bound (number or list of len d)
-    n=2**6,                 # Number of grid points (number or list of len d)
+    n=n,                    # Number of grid points (number or list of len d)
     evals=1.E+5,            # Number of function evaluations
-    name='Alpine',          # Function name for log (this is optional)
-    x_min_real=np.zeros(d), # Real value of x-minima (x; this is for test)
-    y_min_real=0.,          # Real value of y-minima (y=f(x); this is for test)
+    name='Tensor',          # Function name for log (this is optional)
+    x_opt_real=x_min_real,  # Real value of x-minima (x; this is for test)
+    y_opt_real=0.,          # Real value of y-minima (y=f(x); this is for test)
+    is_func=False,          # We approximate the tensor (not a function)
     with_log=True)
 
 
 # And now we launching the minimizer:
-tto.minimize(rmax)
+tto.optimize(rank)
 
 
 # We can extract the results of the computation:
-x = tto.x_min          # The found value of the minimum of the function (x)
-y = tto.y_min          # The found value of the minimum of the function (y=f(x))
+i = tto.i_opt          # The found value of the minimum (multi-index)
+y = tto.y_opt          # The found value of the minimum of the function (y=f(x))
 k_c = tto.k_cache      # Total number of cache usage (should be 0 in this demo)
 k_e = tto.k_evals      # Total number of requests to func (is always = evals)
 k_t = tto.k_total      # Total number of requests (k_cache + k_evals)
 t_f = tto.t_evals_mean # Average time spent to real function call for 1 point
                        # ... (see "ttopt.py" and docs for more details)
 
 
 # We log the final state:
-print('-' * 70 + '\n' + tto.info() +'\n\n')
+print('-' * 70 + '\n' + tto.info())
+print('y_opt : ', y)
+print('i_opt : ', i)
```

### Comparing `ttopt-0.5.0/demo/cache.py` & `ttopt-0.6.0/demo/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 input X is the [samples, dimension] numpy array using the cache.
 
 Run it from the root of the project as "python demo/cache.py".
 
 As a result of the script work we expect the output in console like this:
 "
 ...
-Simple-5d | k=9.86e+03+2.69e+03 | t_cur=7.36e-02 | e_x=3.55e-02 e_y=1.03e-04
+Simple-5d  | evals=9.80e+03+3.01e+03 | t_cur=6.47e-02 | e_x=3.55e-02 e_y=1.03e-04
 ----------------------------------------------------------------------
-Simple-5d | k=9.86e+03+2.69e+03 | t_all=8.88e-02 | e_x=3.55e-02 e_y=1.03e-04
+Simple-5d  | evals=9.80e+03+3.01e+03 | t_all=7.61e-02 | e_x=3.55e-02 e_y=1.03e-04 
 "
 
 """
 import numpy as np
 from scipy.optimize import rosen
 
 
@@ -22,41 +22,41 @@
 from ttopt import ttopt_init
 
 
 np.random.seed(42)
 
 
 d = 5                       # Number of function dimensions:
-rmax = 4                    # Maximum TT-rank while cross-like iterations
+rank = 4                    # Maximum TT-rank while cross-like iterations
 def f(X):                   # Target function
     return np.sin(0.1 * X[:, 0])**2 + 0.1 * np.sum(X[:, 1:]**2, axis=1)
 
 
 # We initialize the TTOpt class instance with the correct parameters:
 tto = TTOpt(
     f=f,                    # Function for minimization. X is [samples, dim]
     d=d,                    # Number of function dimensions
     a=-1.,                  # Grid lower bound (number or list of len d)
     b=+1.,                  # Grid upper bound (number or list of len d)
     n=2**6,                 # Number of grid points (number or list of len d)
     evals=1.E+4,            # Number of function evaluations
     name='Simple',          # Function name for log (this is optional)
-    x_min_real=np.zeros(d), # Real value of x-minima (x; this is for test)
-    y_min_real=0.,          # Real value of y-minima (y=f(x); this is for test)
+    x_opt_real=np.zeros(d), # Real value of x-minima (x; this is for test)
+    y_opt_real=0.,          # Real value of y-minima (y=f(x); this is for test)
     with_cache=True,        # We save all requests into cache
     with_log=True)
 
 
 # And now we launching the minimizer:
-tto.minimize(rmax)
+tto.optimize(rank)
 
 
 # We can extract the results of the computation:
-x = tto.x_min          # The found value of the minimum of the function (x)
-y = tto.y_min          # The found value of the minimum of the function (y=f(x))
+x = tto.x_opt          # The found value of the minimum of the function (x)
+y = tto.y_opt          # The found value of the minimum of the function (y=f(x))
 k_c = tto.k_cache      # Total number of cache usage (should be 0 in this demo)
 k_e = tto.k_evals      # Total number of requests to func (is always = evals)
 k_t = tto.k_total      # Total number of requests (k_cache + k_evals)
 t_f = tto.t_evals_mean # Average time spent to real function call for 1 point
                        # ... (see "ttopt.py" and docs for more details)
```

### Comparing `ttopt-0.5.0/demo/qtt.py` & `ttopt-0.6.0/demo/qtt.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,58 +8,58 @@
 "base.py", except that we replace grid size "n" by grid-factors "p" and "q".
 
 Run it from the root of the project as "python demo/qtt.py".
 
 As a result of the script work we expect the output in console like this:
 "
 ...
-Alpine-10d | k=1.00e+05 | t_cur=1.66e-01 | e_x=3.32e+00 e_y=6.22e-06
+Alpine-10d | evals=1.00e+05 | t_cur=1.62e-01 | e_x=3.42e+00 e_y=4.23e-06
 ----------------------------------------------------------------------
-Alpine-10d | k=1.00e+05 | t_all=2.56e+00 | e_x=3.32e+00 e_y=6.22e-06
+Alpine-10d | evals=1.00e+05 | t_all=2.28e+00 | e_x=3.42e+00 e_y=4.23e-06
 "
 
 """
 import numpy as np
 
 
 from ttopt import TTOpt
 from ttopt import ttopt_init
 
 
 np.random.seed(42)
 
 
 d = 10                      # Number of function dimensions:
-rmax = 4                    # Maximum TT-rank while cross-like iterations
+rank = 4                    # Maximum TT-rank while cross-like iterations
 def f(X):                   # Target function
     return np.sum(np.abs(X * np.sin(X) + 0.1 * X), axis=1)
 
 
 # We initialize the TTOpt class instance with the correct parameters:
 tto = TTOpt(
     f=f,                    # Function for minimization. X is [samples, dim]
     d=d,                    # Number of function dimensions
     a=-10.,                 # Grid lower bound (number or list of len d)
     b=+10.,                 # Grid upper bound (number or list of len d)
     p=2,                    # The grid size factor (there will n=p^q points)
     q=20,                   # The grid size factor (there will n=p^q points)
     evals=1.E+5,            # Number of function evaluations
     name='Alpine',          # Function name for log (this is optional)
-    x_min_real=np.ones(d),  # Real value of x-minima (x; this is for test)
-    y_min_real=0.,          # Real value of y-minima (y=f(x); this is for test)
+    x_opt_real=np.ones(d),  # Real value of x-minima (x; this is for test)
+    y_opt_real=0.,          # Real value of y-minima (y=f(x); this is for test)
     with_log=True)
 
 
 # And now we launching the minimizer:
-tto.minimize(rmax)
+tto.optimize(rank)
 
 
 # We can extract the results of the computation:
-x = tto.x_min          # The found value of the minimum of the function (x)
-y = tto.y_min          # The found value of the minimum of the function (y=f(x))
+x = tto.x_opt          # The found value of the minimum of the function (x)
+y = tto.y_opt          # The found value of the minimum of the function (y=f(x))
 k_c = tto.k_cache      # Total number of cache usage (should be 0 in this demo)
 k_e = tto.k_evals      # Total number of requests to func (is always = evals)
 k_t = tto.k_total      # Total number of requests (k_cache + k_evals)
 t_f = tto.t_evals_mean # Average time spent to real function call for 1 point
                        # ... (see "ttopt.py" and docs for more details)
```

### Comparing `ttopt-0.5.0/demo/qtt_100d.py` & `ttopt-0.6.0/demo/qtt_max.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,60 @@
-"""The demo of using ttopt. Example with QTT for 100-dimensional function.
+"""The demo of using ttopt for maximization. Example with QTT.
 
-We'll find the minimum for the 100-dimensional Alpine function with vectorized
-input. The target function for minimization has the form f(X), where input X is
+We'll find the maximum for the 10-dimensional Alpine function with vectorized
+input. The target function for maximization has the form f(X), where input X is
 the [samples, dimension] numpy array.
 
-Run it from the root of the project as "python demo/qtt_100d.py".
+Run it from the root of the project as "python demo/qtt_max.py".
 
 As a result of the script work we expect the output in console like this:
 "
 ...
-Alpine-100d | k=1.00e+05 | t_cur=3.47e-01 | e_x=1.08e+01 e_y=5.49e-03
+Alpine-10d | evals=1.00e+05 | t_cur=1.65e-01 | y= 8.715206e+01
 ----------------------------------------------------------------------
-Alpine-100d | k=1.00e+05 | t_all=8.98e+00 | e_x=1.08e+01 e_y=5.49e-03
+Alpine-10d | evals=1.00e+05 | t_all=2.22e+00 | y= 8.715206e+01 
 "
 
 """
 import numpy as np
 
 
 from ttopt import TTOpt
 from ttopt import ttopt_init
 
 
 np.random.seed(42)
 
 
-d = 100                     # Number of function dimensions:
-rmax = 4                    # Maximum TT-rank while cross-like iterations
+d = 10                      # Number of function dimensions:
+rank = 4                    # Maximum TT-rank while cross-like iterations
 def f(X):                   # Target function
     return np.sum(np.abs(X * np.sin(X) + 0.1 * X), axis=1)
 
 
 # We initialize the TTOpt class instance with the correct parameters:
 tto = TTOpt(
-    f=f,                    # Function for minimization. X is [samples, dim]
+    f=f,                    # Function for maximization. X is [samples, dim]
     d=d,                    # Number of function dimensions
     a=-10.,                 # Grid lower bound (number or list of len d)
     b=+10.,                 # Grid upper bound (number or list of len d)
     p=2,                    # The grid size factor (there will n=p^q points)
-    q=12,                   # The grid size factor (there will n=p^q points)
+    q=20,                   # The grid size factor (there will n=p^q points)
     evals=1.E+5,            # Number of function evaluations
     name='Alpine',          # Function name for log (this is optional)
-    x_min_real=np.ones(d),  # Real value of x-minima (x; this is for test)
-    y_min_real=0.,          # Real value of y-minima (y=f(x); this is for test)
     with_log=True)
 
 
-# And now we launching the minimizer:
-tto.minimize(rmax)
+# And now we launching the maximizer:
+tto.optimize(rank, is_max=True)
 
 
 # We can extract the results of the computation:
-x = tto.x_min          # The found value of the minimum of the function (x)
-y = tto.y_min          # The found value of the minimum of the function (y=f(x))
+x = tto.x_opt          # The found value of the maximum of the function (x)
+y = tto.y_opt          # The found value of the maximum of the function (y=f(x))
 k_c = tto.k_cache      # Total number of cache usage (should be 0 in this demo)
 k_e = tto.k_evals      # Total number of requests to func (is always = evals)
 k_t = tto.k_total      # Total number of requests (k_cache + k_evals)
 t_f = tto.t_evals_mean # Average time spent to real function call for 1 point
                        # ... (see "ttopt.py" and docs for more details)
```

### Comparing `ttopt-0.5.0/demo/qtt_max.py` & `ttopt-0.6.0/demo/qtt_100d.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,62 @@
-"""The demo of using ttopt for maximization. Example with QTT.
+"""The demo of using ttopt. Example with QTT for 100-dimensional function.
 
-We'll find the maximum for the 10-dimensional Alpine function with vectorized
-input. The target function for maximization has the form f(X), where input X is
+We'll find the minimum for the 100-dimensional Alpine function with vectorized
+input. The target function for minimization has the form f(X), where input X is
 the [samples, dimension] numpy array.
 
-Run it from the root of the project as "python demo/qtt_max.py".
+Run it from the root of the project as "python demo/qtt_100d.py".
 
 As a result of the script work we expect the output in console like this:
 "
 ...
-Alpine-10d | evals=1.00e+05 | t_cur=1.59e-01 | y= 8.715206e+01
+Alpine-100d | evals=1.00e+05 | t_cur=2.87e-01 | e_x=1.16e+01 e_y=2.29e-02
 ----------------------------------------------------------------------
-Alpine-10d | evals=1.00e+05 | t_all=2.38e+00 | y= 8.715206e+01 
+Alpine-100d | evals=1.00e+05 | t_all=6.89e+00 | e_x=1.16e+01 e_y=2.29e-02
 "
 
 """
 import numpy as np
 
 
 from ttopt import TTOpt
 from ttopt import ttopt_init
 
 
 np.random.seed(42)
 
 
-d = 10                      # Number of function dimensions:
-rmax = 4                    # Maximum TT-rank while cross-like iterations
+d = 100                     # Number of function dimensions:
+rank = 4                    # Maximum TT-rank while cross-like iterations
 def f(X):                   # Target function
     return np.sum(np.abs(X * np.sin(X) + 0.1 * X), axis=1)
 
 
 # We initialize the TTOpt class instance with the correct parameters:
 tto = TTOpt(
-    f=f,                    # Function for maximization. X is [samples, dim]
+    f=f,                    # Function for minimization. X is [samples, dim]
     d=d,                    # Number of function dimensions
     a=-10.,                 # Grid lower bound (number or list of len d)
     b=+10.,                 # Grid upper bound (number or list of len d)
     p=2,                    # The grid size factor (there will n=p^q points)
-    q=20,                   # The grid size factor (there will n=p^q points)
+    q=12,                   # The grid size factor (there will n=p^q points)
     evals=1.E+5,            # Number of function evaluations
     name='Alpine',          # Function name for log (this is optional)
+    x_opt_real=np.ones(d),  # Real value of x-minima (x; this is for test)
+    y_opt_real=0.,          # Real value of y-minima (y=f(x); this is for test)
     with_log=True)
 
 
-# And now we launching the maximizer:
-tto.maximize(rmax)
+# And now we launching the minimizer:
+tto.optimize(rank)
 
 
 # We can extract the results of the computation:
-x = tto.x_min          # The found value of the maximum of the function (x)
-y = tto.y_min          # The found value of the maximum of the function (y=f(x))
+x = tto.x_opt          # The found value of the minimum of the function (x)
+y = tto.y_opt          # The found value of the minimum of the function (y=f(x))
 k_c = tto.k_cache      # Total number of cache usage (should be 0 in this demo)
 k_e = tto.k_evals      # Total number of requests to func (is always = evals)
 k_t = tto.k_total      # Total number of requests (k_cache + k_evals)
 t_f = tto.t_evals_mean # Average time spent to real function call for 1 point
                        # ... (see "ttopt.py" and docs for more details)
```

### Comparing `ttopt-0.5.0/demo/tensor.py` & `ttopt-0.6.0/demo/tensor_init.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-"""The demo of using ttopt. Example for tensor minimization.
+"""The demo of using ttopt. Example for tensor minimization (special case).
 
 We'll find the minimum for the given simple d-dimensional tensor with elements:
 Y[i_1, i_2, ..., i_d] = (i_1 - 2)^2 + (i_2 - 3)^2 + i_2^4 + i_3^4 + ... + i_d^4.
 
-Run it from the root of the project as "python demo/tensor.py".
+We will use special method of initialization. Instead of a random tensor, we
+manually construct a set of starting multi-indices for the search.
+
+Run it from the root of the project as "python demo/tensor_init_spec.py".
 
 As a result of the script work we expect the output in console like this:
 "
 ...
-Tensor-10d | k=1.00e+05 | t_cur=9.04e-03 | e_x=0.00e+00 e_y=0.00e+00
+Tensor-10d | evals=1.00e+05 | t_cur=8.92e-03 | e_x=0.00e+00 e_y=0.00e+00
 ----------------------------------------------------------------------
-Tensor-10d | k=1.00e+05 | t_all=1.21e-01 | e_x=0.00e+00 e_y=0.00e+00
+Tensor-10d | evals=1.00e+05 | t_all=1.58e-01 | e_x=0.00e+00 e_y=0.00e+00
 y_opt :  0
 i_opt :  [2 3 0 0 0 0 0 0 0 0]
 "
 
 """
 import numpy as np
 
@@ -26,15 +29,15 @@
 np.random.seed(42)
 
 
 d = 10                      # Number of function dimensions
 p = 2
 q = 10
 n = p**q                    # Mode size for the tensor
-rmax = 2                    # Maximum TT-rank while cross-like iterations
+rank = 2                    # Maximum TT-rank while cross-like iterations
 def f(I):                   # Target function (return tensor element)
     return (I[:, 0] - 2)**2 + (I[:, 1] - 3)**2 + np.sum(I[:, 2:]**4, axis=1)
 
 
 # Real value of x-minima:
 x_min_real = np.zeros(d)
 x_min_real[0] = 2
@@ -44,27 +47,37 @@
 # We initialize the TTOpt class instance with the correct parameters:
 tto = TTOpt(
     f=f,                    # Function for minimization. X is [samples, dim]
     d=d,                    # Number of function dimensions
     n=n,                    # Number of grid points (number or list of len d)
     evals=1.E+5,            # Number of function evaluations
     name='Tensor',          # Function name for log (this is optional)
-    x_min_real=x_min_real,  # Real value of x-minima (x; this is for test)
-    y_min_real=0.,          # Real value of y-minima (y=f(x); this is for test)
+    x_opt_real=x_min_real,  # Real value of x-minima (x; this is for test)
+    y_opt_real=0.,          # Real value of y-minima (y=f(x); this is for test)
     is_func=False,          # We approximate the tensor (not a function)
     with_log=True)
 
 
+# We manually construct a set of starting multi-indices for the search (note
+# that the list contains (d+1) items, the first and last items should be None):
+J0 = [None for _ in range(d+1)]
+J0[1] = np.zeros((rank, 1), dtype=int)
+for k in range(1, d-1):
+    ir = np.ones((rank, 1), dtype=int)
+    ir *= 1 if k % 2 == 1 else 0
+    J0[k+1] = np.hstack((J0[k], ir))
+
+
 # And now we launching the minimizer:
-tto.minimize(rmax)
+tto.optimize(rank, J0=J0)
 
 
 # We can extract the results of the computation:
-i = tto.i_min          # The found value of the minimum (multi-index)
-y = tto.y_min          # The found value of the minimum of the function (y=f(x))
+i = tto.i_opt          # The found value of the minimum (multi-index)
+y = tto.y_opt          # The found value of the minimum of the function (y=f(x))
 k_c = tto.k_cache      # Total number of cache usage (should be 0 in this demo)
 k_e = tto.k_evals      # Total number of requests to func (is always = evals)
 k_t = tto.k_total      # Total number of requests (k_cache + k_evals)
 t_f = tto.t_evals_mean # Average time spent to real function call for 1 point
                        # ... (see "ttopt.py" and docs for more details)
```

### Comparing `ttopt-0.5.0/demo/tensor_init_spec.py` & `ttopt-0.6.0/demo/vect.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,64 @@
-"""The demo of using ttopt. Example for tensor minimization (special case).
+"""The demo of using ttopt. Simple example with "scalar" input.
 
-We'll find the minimum for the given simple d-dimensional tensor with elements:
-Y[i_1, i_2, ..., i_d] = (i_1 - 2)^2 + (i_2 - 3)^2 + i_2^4 + i_3^4 + ... + i_d^4.
+We'll find the minimum for the simple analytic function of the form f(x), where
+input x is the [dimension] numpy array (not vectorized!).
 
-We will use special method of initialization. Instead of a random tensor, we
-manually construct a set of starting multi-indices for the search.
-
-Run it from the root of the project as "python demo/tensor_init_spec.py".
+Run it from the root of the project as "python demo/vect.py".
 
 As a result of the script work we expect the output in console like this:
 "
 ...
-Tensor-10d | k=1.00e+05 | t_cur=9.04e-03 | e_x=0.00e+00 e_y=0.00e+00
+Simple-5d  | evals=1.00e+04 | t_cur=1.38e-01 | e_x=3.55e-02 e_y=1.03e-04
 ----------------------------------------------------------------------
-Tensor-10d | k=1.00e+05 | t_all=1.21e-01 | e_x=0.00e+00 e_y=0.00e+00
-y_opt :  0
-i_opt :  [2 3 0 0 0 0 0 0 0 0]
+Simple-5d  | evals=1.00e+04 | t_all=1.53e-01 | e_x=3.55e-02 e_y=1.03e-04 
 "
 
 """
 import numpy as np
+from scipy.optimize import rosen
 
 
 from ttopt import TTOpt
 from ttopt import ttopt_init
 
 
 np.random.seed(42)
 
 
-d = 10                      # Number of function dimensions
-p = 2
-q = 10
-n = p**q                    # Mode size for the tensor
-rmax = 2                    # Maximum TT-rank while cross-like iterations
-def f(I):                   # Target function (return tensor element)
-    return (I[:, 0] - 2)**2 + (I[:, 1] - 3)**2 + np.sum(I[:, 2:]**4, axis=1)
-
-
-# Real value of x-minima:
-x_min_real = np.zeros(d)
-x_min_real[0] = 2
-x_min_real[1] = 3
+d = 5                       # Number of function dimensions:
+rank = 4                    # Maximum TT-rank while cross-like iterations
+def f(x):                   # Target function
+    return np.sin(0.1 * x[0])**2 + 0.1 * np.sum(x[1:]**2)
 
 
 # We initialize the TTOpt class instance with the correct parameters:
 tto = TTOpt(
     f=f,                    # Function for minimization. X is [samples, dim]
     d=d,                    # Number of function dimensions
-    n=n,                    # Number of grid points (number or list of len d)
-    evals=1.E+5,            # Number of function evaluations
-    name='Tensor',          # Function name for log (this is optional)
-    x_min_real=x_min_real,  # Real value of x-minima (x; this is for test)
-    y_min_real=0.,          # Real value of y-minima (y=f(x); this is for test)
-    is_func=False,          # We approximate the tensor (not a function)
+    a=-1.,                  # Grid lower bound (number or list of len d)
+    b=+1.,                  # Grid upper bound (number or list of len d)
+    n=2**6,                 # Number of grid points (number or list of len d)
+    evals=1.E+4,            # Number of function evaluations
+    name='Simple',          # Function name for log (this is optional)
+    x_opt_real=np.zeros(d), # Real value of x-minima (x; this is for test)
+    y_opt_real=0.,          # Real value of y-minima (y=f(x); this is for test)
+    is_vect=False,          # The function accepts only one spatial point
     with_log=True)
 
 
-# We manually construct a set of starting multi-indices for the search (note
-# that the list contains (d+1) items, the first and last items should be None):
-J0 = [None for _ in range(d+1)]
-J0[1] = np.zeros((rmax, 1), dtype=int)
-for k in range(1, d-1):
-    ir = np.ones((rmax, 1), dtype=int)
-    ir *= 1 if k % 2 == 1 else 0
-    J0[k+1] = np.hstack((J0[k], ir))
-
-
 # And now we launching the minimizer:
-tto.minimize(rmax, J0=J0)
+tto.optimize(rank)
 
 
 # We can extract the results of the computation:
-i = tto.i_min          # The found value of the minimum (multi-index)
-y = tto.y_min          # The found value of the minimum of the function (y=f(x))
+x = tto.x_opt          # The found value of the minimum of the function (x)
+y = tto.y_opt          # The found value of the minimum of the function (y=f(x))
 k_c = tto.k_cache      # Total number of cache usage (should be 0 in this demo)
 k_e = tto.k_evals      # Total number of requests to func (is always = evals)
 k_t = tto.k_total      # Total number of requests (k_cache + k_evals)
 t_f = tto.t_evals_mean # Average time spent to real function call for 1 point
                        # ... (see "ttopt.py" and docs for more details)
 
 
 # We log the final state:
-print('-' * 70 + '\n' + tto.info())
-print('y_opt : ', y)
-print('i_opt : ', i)
+print('-' * 70 + '\n' + tto.info() +'\n\n')
```

### Comparing `ttopt-0.5.0/demo/vect.py` & `ttopt-0.6.0/demo/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-"""The demo of using ttopt. Simple example with "scalar" input.
+"""The demo of using ttopt. Basic example.
 
-We'll find the minimum for the simple analytic function of the form f(x), where
-input x is the [dimension] numpy array (not vectorized!).
+We'll find the minimum for the 10-dimensional Alpine function with vectorized
+input. The target function for minimization has the form f(X), where input X is
+the [samples, dimension] numpy array.
 
-Run it from the root of the project as "python demo/vect.py".
+Run it from the root of the project as "python demo/base.py".
 
 As a result of the script work we expect the output in console like this:
 "
 ...
-Simple-5d | k=1.00e+04 | t_cur=1.54e-01 | e_x=3.55e-02 e_y=1.03e-04
+Alpine-10d | evals=1.00e+05 | t_cur=2.23e-02 | e_x=5.02e-01 e_y=9.22e-02
 ----------------------------------------------------------------------
-Simple-5d | k=1.00e+04 | t_all=1.75e-01 | e_x=3.55e-02 e_y=1.03e-04
+Alpine-10d | evals=1.00e+05 | t_all=8.37e-02 | e_x=5.02e-01 e_y=9.22e-02
 "
 
 """
 import numpy as np
-from scipy.optimize import rosen
 
 
 from ttopt import TTOpt
 from ttopt import ttopt_init
 
 
 np.random.seed(42)
 
 
-d = 5                       # Number of function dimensions:
-rmax = 4                    # Maximum TT-rank while cross-like iterations
-def f(x):                   # Target function
-    return np.sin(0.1 * x[0])**2 + 0.1 * np.sum(x[1:]**2)
+d = 10                      # Number of function dimensions:
+rank = 4                    # Maximum TT-rank while cross-like iterations
+def f(X):                   # Target function
+    return np.sum(np.abs(X * np.sin(X) + 0.1 * X), axis=1)
 
 
 # We initialize the TTOpt class instance with the correct parameters:
 tto = TTOpt(
     f=f,                    # Function for minimization. X is [samples, dim]
     d=d,                    # Number of function dimensions
-    a=-1.,                  # Grid lower bound (number or list of len d)
-    b=+1.,                  # Grid upper bound (number or list of len d)
+    a=-10.,                 # Grid lower bound (number or list of len d)
+    b=+10.,                 # Grid upper bound (number or list of len d)
     n=2**6,                 # Number of grid points (number or list of len d)
-    evals=1.E+4,            # Number of function evaluations
-    name='Simple',          # Function name for log (this is optional)
-    x_min_real=np.zeros(d), # Real value of x-minima (x; this is for test)
-    y_min_real=0.,          # Real value of y-minima (y=f(x); this is for test)
-    is_vect=False,          # The function accepts only one spatial point
+    evals=1.E+5,            # Number of function evaluations
+    name='Alpine',          # Function name for log (this is optional)
+    x_opt_real=np.zeros(d), # Real value of x-minima (x; this is for test)
+    y_opt_real=0.,          # Real value of y-minima (y=f(x); this is for test)
     with_log=True)
 
 
 # And now we launching the minimizer:
-tto.minimize(rmax)
+tto.optimize(rank)
 
 
 # We can extract the results of the computation:
-x = tto.x_min          # The found value of the minimum of the function (x)
-y = tto.y_min          # The found value of the minimum of the function (y=f(x))
+x = tto.x_opt          # The found value of the minimum of the function (x)
+y = tto.y_opt          # The found value of the minimum of the function (y=f(x))
 k_c = tto.k_cache      # Total number of cache usage (should be 0 in this demo)
 k_e = tto.k_evals      # Total number of requests to func (is always = evals)
 k_t = tto.k_total      # Total number of requests (k_cache + k_evals)
 t_f = tto.t_evals_mean # Average time spent to real function call for 1 point
                        # ... (see "ttopt.py" and docs for more details)
```

### Comparing `ttopt-0.5.0/setup.py` & `ttopt-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,30 @@
         if not os.path.isdir(path):
             continue
         packages.extend(find_packages('%s.%s'%(package, name), path))
     return packages
 
 
 here = os.path.abspath(os.path.dirname(__file__))
-desc = 'Multivariate function minimizer based on the tensor train approach.'
+desc = 'Multivariate function optimizer based on the tensor train approach.'
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     desc_long = f.read()
 
 
 with open(os.path.join(here, 'ttopt/__init__.py'), encoding='utf-8') as f:
     text = f.read()
     version = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", text, re.M)
     version = version.group(1)
 
 
+with open(os.path.join(here, 'requirements.txt'), encoding='utf-8') as f:
+    requirements = f.read().split('\n')
+    requirements = [r for r in requirements if len(r) >= 3]
+
+
 setup_args = dict(
     name='ttopt',
     version=version,
     description=desc,
     long_description=desc_long,
     long_description_content_type='text/markdown',
     author='Andrei Chertkov',
@@ -41,27 +46,25 @@
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords='function optimization function minimization low-rank representation tensor train format TT-decomposition cross approximation',
     packages=find_packages('ttopt', './ttopt/'),
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     project_urls={
         'Source': 'https://github.com/AndreiChertkov/ttopt',
     },
 )
 
 
 if __name__ == '__main__':
     setup(
         **setup_args,
-        # Please, install it manually:
-        # install_requires=['numpy', 'scipy', 'maxvolpy'],
+        install_requires=requirements,
         include_package_data=True)
```

### Comparing `ttopt-0.5.0/ttopt/ttopt.py` & `ttopt-0.6.0/ttopt/ttopt.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 
 from .ttopt_raw import ttopt
 from .ttopt_raw import ttopt_find
 
 
 class TTOpt():
-    """Multidimensional minimizer based on the cross-maximum-volume principle.
+    """Multidimensional optimizer based on the cross-maximum-volume principle.
 
-    Class for computation of the minimum for the implicitly given d-dimensional
-    array (tensor) or a function of d-dimensional argument. An adaptive method
-    based on the tensor train (TT) approximation and the cross-maximum volume
-    principle is used. Cache of requested values (its usage leads to faster
-    computation if one point is computed for a long time) and QTT-based
-    representation of the grid (its usage in many cases leads to more accurate
-    results) are supported.
+    Class for computation of the minimum or maximum for the implicitly given
+    d-dimensional array (tensor) or a function of d-dimensional argument. An
+    adaptive method based on the tensor train (TT) approximation and the
+    cross-maximum volume principle is used. Cache of requested values (its
+    usage leads to faster computation if one point is computed for a long time)
+    and QTT-based representation of the grid (its usage in many cases leads to
+    more accurate results) are supported.
 
     Args:
         f (function): the function of interest. Its argument X should represent
             several spatial points for calculation (is 2D numpy array of the
             shape [samples, d]) if "is_vect" flag is True, and it is one
             spatial point for calculation (is 1D numpy array of the shape [d])
             in the case if "is_vect" flag is False. For the case of the tensor
@@ -30,15 +30,15 @@
             shape [samples] of float or only one float value depending on the
             value of "is_vect" flag). If "with_opt" flag is True, then function
             should also return the second argument (is 1D numpy array of the
             shape [samples] of any or just one value depending on the "is_vect"
             flag) which is the auxiliary quantity corresponding to the
             requested points (it is used for debugging and in specific parallel
             calculations; the value of this auxiliary quantity related to the
-            "argmin" point will be passed to "callback" function).
+            "argmin / argmax" point will be passed to "callback" function).
         d (int): number of function dimensions.
         a (float or list of len d of float): grid lower bounds for every
             dimension. If a number is given, then this value will be used for
             each dimension.
         b (float or list of len d of float): grid upper bounds for every
             dimension. If a number is given, then this value will be used for
             each dimension.
@@ -57,25 +57,25 @@
             also be specified, and in this case the QTT-based approach will be
             used.
         evals (int or float): the number of requests to the target function
             that will be made.
         name (str): optional display name for the function of interest. It is
             the empty string by default.
         callback (function): optional function that will be called after each
-            optimization step (in Func.comp.min) with related info (it is used
+            optimization step (in Func.comp_opt) with related info (it is used
             for debugging and in specific parallel calculations).
-        x_min_real (list of len d): optional real value of x-minima (x). If
-            this value is specified, then it will be used to display the
+        x_opt_real (list of len d): optional real value of x-minimum or maximum
+            (x). If this value is specified, then it will be used to display the
             current approximation error within the algorithm iterations (this
             is convenient for debugging and testing/research).
-        y_min_real (float): optional real value of y-minima (y=f(x)). If
+        y_opt_real (float): optional real value of y-optima (y=f(x)). If
             this value is specified, then it will be used to display the
             current approximation error within the algorithm iterations (this
             is convenient for debugging and testing/research).
-        is_func (bool): if flag is True, then we minimize the function (the
+        is_func (bool): if flag is True, then we optimize the function (the
             arguments of f correspond to continuous spatial points), otherwise
             we approximate the tensor (the arguments of f correspond to
             discrete multidimensional tensor multi-indices). It is True by
             default.
         is_vect (bool): if flag is True, then function should accept 2D
             numpy array of the shape [samples, d] (batch of points or indices)
             and return 1D numpy array of the shape [samples]. Otherwise, the
@@ -104,20 +104,24 @@
             presented (in the current version, it can only be messages about
             early convergence when using the cache). It is True by default.
 
     Note:
         Call "calc" to evaluate function for one tensor multi-index and call
         "comp" to evaluate function in the set of multi-indices (both of these
         functions can be called regardless of the value of the flag "is_vect").
-        Call "minimize" to find the global minimum of the function of interest
-        by the TTOpt-algorithm.
+        Call "minimize" / "maximize" to find the global minimum / maximum of
+        the function of interest by the TTOpt-algorithm.
 
     """
 
-    def __init__(self, f, d, a=None, b=None, n=None, p=None, q=None, evals=None, name=None, callback=None, x_min_real=None, y_min_real=None, is_func=True, is_vect=True, with_cache=False, with_log=False, with_opt=False, with_full_info=False, with_wrn=True):
+    def __init__(self, f, d, a=None, b=None, n=None, p=None, q=None,
+                 evals=None, name=None, callback=None, x_opt_real=None,
+                 y_opt_real=None, is_func=True, is_vect=True, with_cache=False,
+                 with_log=False, with_opt=False, with_full_info=False,
+                 with_wrn=True):
         # Set the target function and its dimension:
         self.f = f
         self.d = int(d)
 
         # Set grid lower bound:
         if isinstance(a, (int, float)):
             self.a = np.ones(self.d, dtype=float) * a
@@ -163,16 +167,16 @@
         if self.n_func.size != self.d:
             raise ValueError('Grid size (n/p/q) has invalid shape')
 
         # Set other options according to the input arguments:
         self.evals = int(evals) if evals else None
         self.name = name or ''
         self.callback = callback
-        self.x_min_real = x_min_real
-        self.y_min_real = y_min_real
+        self.x_opt_real = x_opt_real
+        self.y_opt_real = y_opt_real
         self.is_func = bool(is_func)
         self.is_vect = bool(is_vect)
         self.with_cache = bool(with_cache)
         self.with_log = bool(with_log)
         self.with_opt = bool(with_opt)
         self.with_full_info = bool(with_full_info)
         self.with_wrn = bool(with_wrn)
@@ -185,63 +189,63 @@
         self.k_evals = 0    # Number of requests, then function was called
         self.k_evals_curr = 0
         self.t_evals = 0.   # Total time of function calls
         self.t_total = 0.   # Total time of computations (including cache usage)
         self.t_minim = 0    # Total time of work for minimizator
         self._opt = None    # Function opts related to its output
 
-        # Current minima:
-        self.i_min = None
-        self.x_min = None
+        # Current optimum:
+        self.i_opt = None
+        self.x_opt = None
 
-        # Approximations for argmin/min/opts of the function while iterations:
+        # Approximations for argopt/opt/opts of the function while iterations:
         self.I_list = []
-        self.i_min_list = []
-        self.x_min_list = []
-        self.y_min_list = []
-        self.opt_min_list = []
-        self.evals_min_list = []
-        self.cache_min_list = []
+        self.i_opt_list = []
+        self.x_opt_list = []
+        self.y_opt_list = []
+        self.opt_opt_list = []
+        self.evals_opt_list = []
+        self.cache_opt_list = []
 
     @property
     def e_x(self):
-        """Current error for approximation of argmin of the function."""
-        if self.x_min_real is not None and self.x_min is not None:
-            return np.linalg.norm(self.x_min - self.x_min_real)
+        """Current error for approximation of arg-opt of the function."""
+        if self.x_opt_real is not None and self.x_opt is not None:
+            return np.linalg.norm(self.x_opt - self.x_opt_real)
 
     @property
     def e_y(self):
-        """Current error for approximation of the minumum of the function."""
-        if self.y_min_real is not None and self.y_min is not None:
-            return np.abs(self.y_min - self.y_min_real)
+        """Current error for approximation of the optimum of the function."""
+        if self.y_opt_real is not None and self.y_opt is not None:
+            return np.abs(self.y_opt - self.y_opt_real)
 
     @property
     def k_total(self):
         """Total number of requests (both function calls and cache usage)."""
         return self.k_cache + self.k_evals
 
     @property
-    def opt_min(self):
-        """Current value of option of the function related to min-point."""
-        return self.opt_min_list[-1] if len(self.opt_min_list) else None
+    def opt_opt(self):
+        """Current value of option of the function related to opt-point."""
+        return self.opt_opt_list[-1] if len(self.opt_opt_list) else None
 
     @property
     def t_evals_mean(self):
         """Average time spent to real function call for 1 point."""
         return self.t_evals / self.k_evals if self.k_evals else 0.
 
     @property
     def t_total_mean(self):
         """Average time spent to return one function value."""
         return self.t_total / self.k_total if self.k_total else 0.
 
     @property
-    def y_min(self):
-        """Current approximation of min of the function of interest."""
-        return self.y_min_list[-1] if len(self.y_min_list) else None
+    def y_opt(self):
+        """Current approximation of optimum of the function of interest."""
+        return self.y_opt_list[-1] if len(self.y_opt_list) else None
 
     def calc(self, i):
         """Calculate the function for the given multiindex.
 
         Args:
             i (np.ndarray): the input for the function, that is 1D numpy array
                 of the shape [d] of int (indices).
@@ -262,14 +266,16 @@
             self.t_total += tpc() - t_total
             return y
 
         s = self.i2s(i.astype(int).tolist())
 
         if not s in self.cache:
             y = self._eval(i)
+            if y is None:
+                return y
             self.cache[s] = y
             self.cache_opt[s] = self._opt
         else:
             y = self.cache[s]
             self._opt = self.cache_opt[s]
             self.k_cache_curr = 1
             self.k_cache += self.k_cache_curr
@@ -296,15 +302,18 @@
 
         """
         self.k_cache_curr = 0
 
         if not self.is_vect:
             Y, _opt = [], []
             for i in I:
-                Y.append(self.calc(i))
+                y = self.calc(i)
+                if y is None:
+                    return None
+                Y.append(y)
                 _opt.append(self._opt)
             self._opt = _opt
             return np.array(Y)
 
         t_total = tpc()
 
         if not self.with_cache:
@@ -319,35 +328,37 @@
         J = [i for i in I if self.i2s(i) not in self.cache]
         self.k_cache_curr = len(I) - len(J)
         self.k_cache += self.k_cache_curr
 
         # We add new points (J) to the storage:
         if len(J):
             Z = self._eval(J)
+            if Z is None:
+                return None
             for k, j in enumerate(J):
                 s = self.i2s(j)
                 self.cache[s] = Z[k]
                 self.cache_opt[s] = self._opt[k]
 
         # We obtain the values for requested points from the updated storage:
         Y = np.array([self.cache[self.i2s(i)] for i in I])
         self._opt = np.array([self.cache_opt[self.i2s(i)] for i in I])
 
         self.t_total += tpc() - t_total
 
         return Y
 
-    def comp_min(self, I, i_min=None, y_min=None, opt_min=None):
-        """Compute the function for the set of points and save current minimum.
+    def comp_opt(self, I, i_opt=None, y_opt=None, opt_opt=None):
+        """Compute the function for the set of points and save current optimum.
 
         This helper function (this is wrapper for function "comp") can be
         passed to the optimizer. When making requests, the optimizer must pass
         the grid points of interest (I) as arguments, as well as the current
-        approximation of the argmin (i_min), the corresponding value (y_min)
-        and related option value (opt_min).
+        approximation of the argmin / argmax (i_opt), the corresponding value
+        (y_opt) and related option value (opt_opt).
 
         """
         # We return None if the limit for function requests is exceeded:
         if self.evals is not None and self.k_evals >= self.evals:
             return None, None
 
         # We return None if the number of requests to the cache is 2 times
@@ -368,52 +379,52 @@
         if is_last:
             I = I[:(self.evals-self.k_evals), :]
 
         if self.q:
             # The QTT is used, hence we should transform the indices:
             if I is not None:
                 I = self.qtt_parse_many(I)
-            if i_min is not None:
-                i_min = self.qtt_parse_many(i_min.reshape(1, -1))[0, :]
+            if i_opt is not None:
+                i_opt = self.qtt_parse_many(i_opt.reshape(1, -1))[0, :]
 
         Y = self.comp(I)
 
         # If this is last iteration, we should "manually" check for y_opt_new:
         if is_last:
-            i_min, y_min, opt_min = ttopt_find(
-                I, Y, self._opt, i_min, y_min, opt_min, self.is_max)
+            i_opt, y_opt, opt_opt = ttopt_find(
+                I, Y, self._opt, i_opt, y_opt, opt_opt, self.is_max)
 
-        if i_min is None:
+        if i_opt is None:
             return Y, self._opt
 
         if self.is_func:
-            x_min = self.i2x(i_min)
+            x_opt = self.i2x(i_opt)
         else:
-            x_min = i_min.copy()
+            x_opt = i_opt.copy()
 
-        self.i_min = i_min.copy()
-        self.x_min = x_min.copy()
+        self.i_opt = i_opt.copy()
+        self.x_opt = x_opt.copy()
 
-        self.y_min_list.append(y_min)
-        self.opt_min_list.append(opt_min)
-        self.evals_min_list.append(self.k_evals_curr)
-        self.cache_min_list.append(self.k_cache_curr)
+        self.y_opt_list.append(y_opt)
+        self.opt_opt_list.append(opt_opt)
+        self.evals_opt_list.append(self.k_evals_curr)
+        self.cache_opt_list.append(self.k_cache_curr)
 
         if self.with_full_info:
             self.I_list.append(I)
-            self.i_min_list.append(self.i_min.copy())
-            self.x_min_list.append(self.x_min.copy())
+            self.i_opt_list.append(self.i_opt.copy())
+            self.x_opt_list.append(self.x_opt.copy())
 
         if self.is_max:
-            is_better = len(self.y_min_list)==1 or (y_min > self.y_min_list[-2])
+            is_better = len(self.y_opt_list)==1 or (y_opt > self.y_opt_list[-2])
         else:
-            is_better = len(self.y_min_list)==1 or (y_min < self.y_min_list[-2])
+            is_better = len(self.y_opt_list)==1 or (y_opt < self.y_opt_list[-2])
 
         if self.callback and is_better:
-            last = {'last': [x_min, y_min, i_min, opt_min, self.k_evals]}
+            last = {'last': [x_opt, y_opt, i_opt, opt_opt, self.k_evals]}
             self.callback(last)
 
         if self.with_log:
             print(self.info(is_final=False))
 
         return Y, self._opt
 
@@ -451,55 +462,50 @@
             text += f'evals={self.k_total:-8.2e} | '
 
         if is_final:
             text += f't_all={self.t_minim:-8.2e} | '
         else:
             text += f't_cur={self.t_total:-8.2e} | '
 
-        if self.y_min_real is None and self.y_min is not None:
-            text += f'y={self.y_min:-13.6e} '
+        if self.y_opt_real is None and self.y_opt is not None:
+            text += f'y={self.y_opt:-13.6e} '
         else:
             if with_e_x and self.e_x is not None:
                 text += f'e_x={self.e_x:-8.2e} '
             if with_e_y and self.e_y is not None:
                 text += f'e_y={self.e_y:-8.2e} '
 
         return text
 
-    def minimize(self, rmax=10, Y0=None, fs_opt=1., add_opt_inner=True, add_opt_outer=False, add_opt_rect=False, add_rnd_inner=False, add_rnd_outer=False, J0=None, is_max=False):
-        """Perform the function minimization process by TT-based approach.
+    def optimize(self, rank=10, Y0=None, seed=42, fs_opt=1., is_max=False,
+                 add_opt_inner=True, add_opt_outer=False, add_opt_rect=False,
+                 add_rnd_inner=False, add_rnd_outer=False, J0=None):
+        """Perform the function optimization process by TT-based approach.
 
         Args:
-            rmax (int): maximum TT-rank.
+            rank (int): maximum TT-rank.
             Y0 (list of 3D np.ndarrays of float): optional initial tensor in
                 the TT format as a list of the TT-cores.
+            seed (int): random seed for the algorithm initialization. It is
+                used only if Y0 and J0 are not set.
             fs_opt (float): the parameter of the smoothing function. If it is
                 None, then "arctan" function will be used. Otherwise, the
                 function "exp(-1 * fs_opt * (p - p0))" will be used.
+            is_max (bool): if flag is True, then maximization will be performed.
 
         """
         t_minim = tpc()
         self.is_max = is_max
 
-        i_min, y_min = ttopt(self.comp_min, self.n, rmax, None, Y0,
+        i_opt, y_opt = ttopt(self.comp_opt, self.n, rank, None, Y0, seed,
                 fs_opt, add_opt_inner, add_opt_outer, add_opt_rect,
                 add_rnd_inner, add_rnd_outer, J0, is_max)
 
         self.t_minim = tpc() - t_minim
 
-    def maximize(self, rmax=10, Y0=None, fs_opt=1., add_opt_inner=True, add_opt_outer=False, add_opt_rect=False, add_rnd_inner=False, add_rnd_outer=False, J0=None):
-        """Perform the function maximization process by TT-based approach.
-
-        Note:
-            See description of parameters in "minimize" function.
-
-        """
-        return self.minimize(rmax, Y0, fs_opt, add_opt_inner, add_opt_outer,
-            add_opt_rect, add_rnd_inner, add_rnd_outer, J0, is_max=True)
-
     def qtt_parse_many(self, I_qtt):
         """Transform tensor indices from QTT (long) to base (short) format."""
         samples = I_qtt.shape[0]
         n_qtt = [self.n[0]]*self.q
         I = np.zeros((samples, self.d))
         for i in range(self.d):
             J_curr = I_qtt[:, self.q*i:self.q*(i+1)].T
@@ -520,16 +526,20 @@
         if self.is_func:
             x = self.i2x_many(i) if is_many else self.i2x(i)
         else:
             x = i
 
         if self.with_opt:
             y, self._opt = self.f(x)
+            if y is None:
+                return None
         else:
             y = self.f(x)
+            if y is None:
+                return None
             self._opt = [None for _ in range(y.size)] if is_many else None
 
         self.k_evals_curr = y.size if is_many else 1
         self.k_evals += self.k_evals_curr
         self.t_evals += tpc() - t_evals
 
         return y
```

