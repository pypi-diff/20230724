# Comparing `tmp/catsim-polytomous-0.0.1.tar.gz` & `tmp/catsim-polytomous-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catsim-polytomous-0.0.1.tar", last modified: Thu Jul 20 07:48:28 2023, max compression
+gzip compressed data, was "catsim-polytomous-0.1.0.tar", last modified: Mon Jul 24 21:42:27 2023, max compression
```

## Comparing `catsim-polytomous-0.0.1.tar` & `catsim-polytomous-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-20 07:48:28.494817 catsim-polytomous-0.0.1/
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    35147 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/COPYING
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)     7651 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/COPYING.LESSER
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    16259 2023-07-20 07:48:28.494928 catsim-polytomous-0.0.1/PKG-INFO
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)     6281 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/README.md
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    26897 2023-07-20 07:45:17.000000 catsim-polytomous-0.0.1/pyproject.toml
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)       80 2023-07-20 07:48:28.495244 catsim-polytomous-0.0.1/setup.cfg
-drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-20 07:48:28.491032 catsim-polytomous-0.0.1/src/
-drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-20 07:48:28.493621 catsim-polytomous-0.0.1/src/catsim/
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)        0 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/src/catsim/__init__.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)     7346 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/src/catsim/cat.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    15351 2023-07-20 07:37:26.000000 catsim-polytomous-0.0.1/src/catsim/estimation.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)     2416 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/src/catsim/initialization.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    19665 2023-07-20 07:38:49.000000 catsim-polytomous-0.0.1/src/catsim/irt.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    15726 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/src/catsim/plot.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    42332 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/src/catsim/selection.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    19931 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/src/catsim/simulation.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)     2963 2023-07-20 05:11:21.000000 catsim-polytomous-0.0.1/src/catsim/stopping.py
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)     1749 2023-07-20 05:00:45.000000 catsim-polytomous-0.0.1/src/catsim_poly_debug.py
-drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-20 07:48:28.494539 catsim-polytomous-0.0.1/src/catsim_polytomous.egg-info/
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)    16259 2023-07-20 07:48:28.000000 catsim-polytomous-0.0.1/src/catsim_polytomous.egg-info/PKG-INFO
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)      529 2023-07-20 07:48:28.000000 catsim-polytomous-0.0.1/src/catsim_polytomous.egg-info/SOURCES.txt
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)        1 2023-07-20 07:48:28.000000 catsim-polytomous-0.0.1/src/catsim_polytomous.egg-info/dependency_links.txt
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)      269 2023-07-20 07:48:28.000000 catsim-polytomous-0.0.1/src/catsim_polytomous.egg-info/requires.txt
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)       25 2023-07-20 07:48:28.000000 catsim-polytomous-0.0.1/src/catsim_polytomous.egg-info/top_level.txt
-drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-20 07:48:28.494664 catsim-polytomous-0.0.1/tests/
--rw-r--r--   0 vaishakkrishna   (501) staff       (20)     6690 2023-07-18 19:41:59.000000 catsim-polytomous-0.0.1/tests/test_main.py
+drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-24 21:42:27.080592 catsim-polytomous-0.1.0/
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    35147 2023-07-18 19:41:59.000000 catsim-polytomous-0.1.0/COPYING
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)     7651 2023-07-18 19:41:59.000000 catsim-polytomous-0.1.0/COPYING.LESSER
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    16259 2023-07-24 21:42:27.080762 catsim-polytomous-0.1.0/PKG-INFO
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)     6281 2023-07-18 19:41:59.000000 catsim-polytomous-0.1.0/README.md
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    26897 2023-07-24 21:39:46.000000 catsim-polytomous-0.1.0/pyproject.toml
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)       80 2023-07-24 21:42:27.081178 catsim-polytomous-0.1.0/setup.cfg
+drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-24 21:42:27.075552 catsim-polytomous-0.1.0/src/
+drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-24 21:42:27.079021 catsim-polytomous-0.1.0/src/catsim_poly/
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)        0 2023-07-18 19:41:59.000000 catsim-polytomous-0.1.0/src/catsim_poly/__init__.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)     7351 2023-07-24 21:34:06.000000 catsim-polytomous-0.1.0/src/catsim_poly/cat.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    15361 2023-07-24 21:34:06.000000 catsim-polytomous-0.1.0/src/catsim_poly/estimation.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)     2416 2023-07-18 19:41:59.000000 catsim-polytomous-0.1.0/src/catsim_poly/initialization.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    19748 2023-07-24 21:38:18.000000 catsim-polytomous-0.1.0/src/catsim_poly/irt.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    15726 2023-07-18 19:41:59.000000 catsim-polytomous-0.1.0/src/catsim_poly/plot.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    42332 2023-07-18 19:41:59.000000 catsim-polytomous-0.1.0/src/catsim_poly/selection.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    19931 2023-07-18 19:41:59.000000 catsim-polytomous-0.1.0/src/catsim_poly/simulation.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)     2963 2023-07-20 05:11:21.000000 catsim-polytomous-0.1.0/src/catsim_poly/stopping.py
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)     1789 2023-07-24 21:34:06.000000 catsim-polytomous-0.1.0/src/catsim_poly_debug.py
+drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-24 21:42:27.080124 catsim-polytomous-0.1.0/src/catsim_polytomous.egg-info/
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)    16259 2023-07-24 21:42:27.000000 catsim-polytomous-0.1.0/src/catsim_polytomous.egg-info/PKG-INFO
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)      574 2023-07-24 21:42:27.000000 catsim-polytomous-0.1.0/src/catsim_polytomous.egg-info/SOURCES.txt
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)        1 2023-07-24 21:42:27.000000 catsim-polytomous-0.1.0/src/catsim_polytomous.egg-info/dependency_links.txt
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)      269 2023-07-24 21:42:27.000000 catsim-polytomous-0.1.0/src/catsim_polytomous.egg-info/requires.txt
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)       30 2023-07-24 21:42:27.000000 catsim-polytomous-0.1.0/src/catsim_polytomous.egg-info/top_level.txt
+drwxr-xr-x   0 vaishakkrishna   (501) staff       (20)        0 2023-07-24 21:42:27.080312 catsim-polytomous-0.1.0/tests/
+-rw-r--r--   0 vaishakkrishna   (501) staff       (20)     6725 2023-07-24 21:34:06.000000 catsim-polytomous-0.1.0/tests/test_main.py
```

### Comparing `catsim-polytomous-0.0.1/COPYING` & `catsim-polytomous-0.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `catsim-polytomous-0.0.1/COPYING.LESSER` & `catsim-polytomous-0.1.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `catsim-polytomous-0.0.1/PKG-INFO` & `catsim-polytomous-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catsim-polytomous
-Version: 0.0.1
+Version: 0.1.0
 Summary: Computerized Adaptive Testing Simulator w/ support for polytomous items using the Partial Credit Model (PCM)
 Author-email: Douglas De Rizzo Meneghetti <douglasrizzo@gmail.com>, Vaishak Krishna <vaishak.krishna@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `catsim-polytomous-0.0.1/README.md` & `catsim-polytomous-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `catsim-polytomous-0.0.1/pyproject.toml` & `catsim-polytomous-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Topic :: Education :: Testing",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
 ]
 name = "catsim-polytomous"
-version = "0.0.1"
+version = "0.1.0"
 description = "Computerized Adaptive Testing Simulator w/ support for polytomous items using the Partial Credit Model (PCM)"
 dependencies = [
     "scipy",
     "numexpr",
     "matplotlib",
     "scikit-learn",
     "json_tricks",
```

### Comparing `catsim-polytomous-0.0.1/src/catsim/cat.py` & `catsim-polytomous-0.1.0/src/catsim_poly/cat.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import operator
 import random
 from typing import List, Union
 
 import numpy
 
-from catsim import irt
+from catsim_poly import irt
 
 
 def dodd(theta: float, items: numpy.ndarray, correct: bool) -> float:
     """Method proposed by [Dod90]_ for the estimation of :math:`\\hat{\\theta}`
     when the response vector is composed entirely of 1s or 0s.
 
     .. math::
```

### Comparing `catsim-polytomous-0.0.1/src/catsim/estimation.py` & `catsim-polytomous-0.1.0/src/catsim_poly/estimation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import List
 
 import numpy
 from scipy.optimize import minimize_scalar
 
-from catsim import cat, irt
-from catsim.simulation import Estimator
+from catsim_poly import cat, irt
+from catsim_poly.simulation import Estimator
 
 
 class NumericalSearchEstimator(Estimator):
     """Estimator that implements multiple search algorithms in unimodal functions to find the maximum of the log-likelihood function. There are implementations of ternary search, dichotomous search, Fibonacci search and golden-section search, according to [Veliz20]_. Also check [Brent02]_. It is also possible to use the methods from :py:func:`scipy.optimize.minimize_scalar`.
 
     :param precision: number of decimal points of precision, defaults to 6
     :type precision: int, optional
```

### Comparing `catsim-polytomous-0.0.1/src/catsim/initialization.py` & `catsim-polytomous-0.1.0/src/catsim_poly/initialization.py`

 * *Files identical despite different names*

### Comparing `catsim-polytomous-0.0.1/src/catsim/irt.py` & `catsim-polytomous-0.1.0/src/catsim_poly/irt.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,32 +65,32 @@
     '''
     Implementation of :py:func:`pcm` using :py:mod:`numpy` and :py:mod:`numexpr` in which the characteristic
     function for all items in a `numpy.ndarray` are computed at once
 
     :param theta: the individual's ability value.
     :param items: array containing the item difficulty followed 3 rasch-andrich thresholds.
     :returns: a 2-d array of all item characteristic functions, given the current ``theta``.
-    This array has shape (n_items, 4).
+    This array has shape (n_items, n_thresholds).
     '''
     b = items[:, 0] # item difficulty
-    r = items[:, 1:4] # rasch-andrich thresholds
-    output = numpy.zeros((items.shape[0], 4))
+    r = items[:, 1:] # rasch-andrich thresholds
+    # output = numpy.zeros((items.shape[0], ))
+    output = numpy.zeros((items.shape[0], items.shape[1]))
 
-    for i in range(4):
+    for i in range(items.shape[1]):
         r_sum = numpy.sum(r[:, :i], axis=1)
         log_num = (i * theta - b + r_sum).astype(float)
         # numerator = numexpr.evaluate("exp(i * theta - (b + r_sum))")
         numerator = numpy.exp(log_num)
         den_array = numpy.zeros_like(numerator)
         
-        for k in range(4):
+        for k in range(items.shape[1]):
             r_sum_k = numpy.sum(r[:, :k], axis=1)
             log_den = (k * theta - b + r_sum_k).astype(float)
             den_array += numpy.exp(log_den)
-            
         output[:, i] = numerator / den_array
 
     return output
```

### Comparing `catsim-polytomous-0.0.1/src/catsim/plot.py` & `catsim-polytomous-0.1.0/src/catsim_poly/plot.py`

 * *Files identical despite different names*

### Comparing `catsim-polytomous-0.0.1/src/catsim/selection.py` & `catsim-polytomous-0.1.0/src/catsim_poly/selection.py`

 * *Files identical despite different names*

### Comparing `catsim-polytomous-0.0.1/src/catsim/simulation.py` & `catsim-polytomous-0.1.0/src/catsim_poly/simulation.py`

 * *Files identical despite different names*

### Comparing `catsim-polytomous-0.0.1/src/catsim/stopping.py` & `catsim-polytomous-0.1.0/src/catsim_poly/stopping.py`

 * *Files identical despite different names*

### Comparing `catsim-polytomous-0.0.1/src/catsim_poly_debug.py` & `catsim-polytomous-0.1.0/src/catsim_poly_debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ## Using catsim objects outside of a Simulator
 # this function generates an item bank, in case the user cannot provide one
-from catsim.cat import generate_item_bank
+from catsim_poly.cat import generate_item_bank
 # simulation package contains the Simulator and all abstract classes
-from catsim.simulation import *
+from catsim_poly.simulation import *
 # initialization package contains different initial proficiency estimation strategies
-from catsim.initialization import *
+from catsim_poly.initialization import *
 # selection package contains different item selection strategies
-from catsim.selection import *
+from catsim_poly.selection import *
 # estimation package contains different proficiency estimation methods
-from catsim.estimation import *
+from catsim_poly.estimation import *
 # stopping package contains different stopping criteria for the CAT
-from catsim.stopping import *
-import catsim.plot as catplot
-from catsim.irt import icc
+from catsim_poly.stopping import *
+import catsim_poly.plot as catplot
+from catsim_poly.irt import icc
 import random
 
 import matplotlib.pyplot as plt
 import pandas as pd
 items = pd.read_csv('items.csv')
 items = items[['measure', 't1', 't2', 't3']].to_numpy()
 responses =          [0, 2]
```

### Comparing `catsim-polytomous-0.0.1/src/catsim_polytomous.egg-info/PKG-INFO` & `catsim-polytomous-0.1.0/src/catsim_polytomous.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catsim-polytomous
-Version: 0.0.1
+Version: 0.1.0
 Summary: Computerized Adaptive Testing Simulator w/ support for polytomous items using the Partial Credit Model (PCM)
 Author-email: Douglas De Rizzo Meneghetti <douglasrizzo@gmail.com>, Vaishak Krishna <vaishak.krishna@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `catsim-polytomous-0.0.1/tests/test_main.py` & `catsim-polytomous-0.1.0/tests/test_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import random
 from sklearn.cluster import KMeans
 
-from catsim import plot
-from catsim.cat import generate_item_bank
-from catsim.estimation import *
-from catsim.initialization import *
-from catsim.selection import *
-from catsim.simulation import Simulator
-from catsim.stopping import MaxItemStopper, MinErrorStopper
+from catsim_poly import plot
+from catsim_poly.cat import generate_item_bank
+from catsim_poly.estimation import *
+from catsim_poly.initialization import *
+from catsim_poly.selection import *
+from catsim_poly.simulation import Simulator
+from catsim_poly.stopping import MaxItemStopper, MinErrorStopper
 
 
 def one_simulation(items, examinees, initializer, selector, estimator, stopper):
     s = Simulator(items, examinees)
     s.simulate(initializer, selector, estimator, stopper, verbose=True)
     cat.rmse(s.examinees, s.latest_estimations)
```

