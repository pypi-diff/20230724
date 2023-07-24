# Comparing `tmp/easier-1.3.5.tar.gz` & `tmp/easier-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easier-1.3.5.tar", last modified: Wed Jul  5 18:37:37 2023, max compression
+gzip compressed data, was "easier-1.3.6.tar", last modified: Mon Jul 24 14:59:55 2023, max compression
```

## Comparing `easier-1.3.5.tar` & `easier-1.3.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-05 18:37:37.105710 easier-1.3.5/
--rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.5/CONTRIBUTORS.txt
--rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.5/LICENSE
--rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.5/MANIFEST.in
--rw-rw-r--   0 rob        (501) staff       (20)      448 2023-07-05 18:37:37.105757 easier-1.3.5/PKG-INFO
--rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.5/README.md
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-05 18:37:37.104152 easier-1.3.5/easier/
--rw-rw-r--   0 rob        (501) staff       (20)      685 2022-08-17 21:35:50.000000 easier-1.3.5/easier/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5869 2023-07-03 14:15:05.000000 easier-1.3.5/easier/api.py
--rw-rw-r--   0 rob        (501) staff       (20)    10490 2022-09-21 18:47:14.000000 easier-1.3.5/easier/bernstein.py
--rw-rw-r--   0 rob        (501) staff       (20)    15283 2021-08-04 15:44:52.000000 easier-1.3.5/easier/bigquery.py
--rw-rw-r--   0 rob        (501) staff       (20)     1449 2021-01-14 22:38:24.000000 easier-1.3.5/easier/cli.py
--rw-rw-r--   0 rob        (501) staff       (20)     4453 2019-12-12 19:11:35.000000 easier-1.3.5/easier/clock.py
--rw-rw-r--   0 rob        (501) staff       (20)     2118 2020-05-29 19:14:34.000000 easier-1.3.5/easier/crypt.py
--rw-rw-r--   0 rob        (501) staff       (20)    11828 2023-07-04 18:30:46.000000 easier-1.3.5/easier/dataframe_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     4416 2021-10-25 19:35:54.000000 easier-1.3.5/easier/distributions.py
--rw-rw-r--   0 rob        (501) staff       (20)     3729 2022-11-06 22:52:50.000000 easier-1.3.5/easier/duck.py
--rw-rw-r--   0 rob        (501) staff       (20)     6934 2023-01-04 21:20:27.000000 easier-1.3.5/easier/duck_model.py
--rw-rw-r--   0 rob        (501) staff       (20)     1312 2022-12-27 18:28:43.000000 easier-1.3.5/easier/ecdf_lib.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-05 18:37:37.105524 easier-1.3.5/easier/filtering/
--rw-rw-r--   0 rob        (501) staff       (20)       89 2021-09-24 01:20:15.000000 easier-1.3.5/easier/filtering/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5693 2021-09-24 01:20:25.000000 easier-1.3.5/easier/filtering/elliptic_filter.py
--rw-rw-r--   0 rob        (501) staff       (20)     2106 2021-11-24 17:03:48.000000 easier-1.3.5/easier/filtering/tvd.py
--rw-rw-r--   0 rob        (501) staff       (20)    14061 2022-08-17 21:35:50.000000 easier-1.3.5/easier/fit_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     8505 2021-01-14 20:54:34.000000 easier-1.3.5/easier/gsheet.py
--rw-rw-r--   0 rob        (501) staff       (20)     7770 2022-08-16 22:01:30.000000 easier-1.3.5/easier/hvtools.py
--rw-rw-r--   0 rob        (501) staff       (20)     3749 2023-07-01 21:46:38.000000 easier-1.3.5/easier/ibis_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     1794 2020-03-27 15:13:42.000000 easier-1.3.5/easier/item.py
--rw-rw-r--   0 rob        (501) staff       (20)     2136 2020-05-29 19:14:34.000000 easier-1.3.5/easier/iterify.py
--rw-rw-r--   0 rob        (501) staff       (20)      208 2020-05-29 19:14:34.000000 easier-1.3.5/easier/memory.py
--rw-rw-r--   0 rob        (501) staff       (20)    11444 2022-11-07 18:39:22.000000 easier-1.3.5/easier/minimodel.py
--rw-rw-r--   0 rob        (501) staff       (20)     8148 2022-08-11 18:33:31.000000 easier-1.3.5/easier/minimodel_orig.py
--rw-rw-r--   0 rob        (501) staff       (20)     4950 2021-12-08 22:15:51.000000 easier-1.3.5/easier/nice_dates.py
--rw-rw-r--   0 rob        (501) staff       (20)     2087 2020-05-29 19:14:34.000000 easier-1.3.5/easier/outlier_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     3186 2022-08-17 21:35:50.000000 easier-1.3.5/easier/parallel.py
--rw-rw-r--   0 rob        (501) staff       (20)     7743 2019-12-12 19:22:12.000000 easier-1.3.5/easier/param_state.py
--rw-rw-r--   0 rob        (501) staff       (20)     1195 2022-08-17 21:35:50.000000 easier-1.3.5/easier/plotting.py
--rw-rw-r--   0 rob        (501) staff       (20)     9482 2022-12-11 17:05:42.000000 easier-1.3.5/easier/postgres.py
--rw-rw-r--   0 rob        (501) staff       (20)      663 2018-08-08 19:33:34.000000 easier-1.3.5/easier/print_catcher.py
--rw-rw-r--   0 rob        (501) staff       (20)     6150 2022-11-10 16:40:03.000000 easier-1.3.5/easier/proportion_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     3178 2022-09-23 20:00:52.000000 easier-1.3.5/easier/salesforce.py
--rw-rw-r--   0 rob        (501) staff       (20)     3231 2020-05-29 19:14:34.000000 easier-1.3.5/easier/shaper.py
--rw-rw-r--   0 rob        (501) staff       (20)     2902 2019-12-12 19:11:38.000000 easier-1.3.5/easier/timer.py
--rw-rw-r--   0 rob        (501) staff       (20)    19244 2023-01-03 20:00:58.000000 easier-1.3.5/easier/utils.py
--rw-rw-r--   0 rob        (501) staff       (20)       22 2023-07-05 18:36:50.000000 easier-1.3.5/easier/version.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-05 18:37:37.104997 easier-1.3.5/easier.egg-info/
--rw-r--r--   0 rob        (501) staff       (20)      448 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/PKG-INFO
--rw-r--r--   0 rob        (501) staff       (20)     1018 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/SOURCES.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/dependency_links.txt
--rw-r--r--   0 rob        (501) staff       (20)      117 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/entry_points.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.3.5/easier.egg-info/not-zip-safe
--rw-r--r--   0 rob        (501) staff       (20)       36 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/requires.txt
--rw-r--r--   0 rob        (501) staff       (20)        7 2023-07-05 18:37:37.000000 easier-1.3.5/easier.egg-info/top_level.txt
--rw-rw-r--   0 rob        (501) staff       (20)      504 2023-07-05 18:37:37.105990 easier-1.3.5/setup.cfg
--rw-rw-r--   0 rob        (501) staff       (20)     1638 2021-01-14 22:24:18.000000 easier-1.3.5/setup.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-24 14:59:55.133126 easier-1.3.6/
+-rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.6/CONTRIBUTORS.txt
+-rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.6/LICENSE
+-rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.6/MANIFEST.in
+-rw-rw-r--   0 rob        (501) staff       (20)      448 2023-07-24 14:59:55.133176 easier-1.3.6/PKG-INFO
+-rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.6/README.md
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-24 14:59:55.131475 easier-1.3.6/easier/
+-rw-rw-r--   0 rob        (501) staff       (20)      685 2022-08-17 21:35:50.000000 easier-1.3.6/easier/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5869 2023-07-03 14:15:05.000000 easier-1.3.6/easier/api.py
+-rw-rw-r--   0 rob        (501) staff       (20)    11673 2023-07-24 14:57:37.000000 easier-1.3.6/easier/bernstein.py
+-rw-rw-r--   0 rob        (501) staff       (20)    15283 2021-08-04 15:44:52.000000 easier-1.3.6/easier/bigquery.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1449 2021-01-14 22:38:24.000000 easier-1.3.6/easier/cli.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4453 2019-12-12 19:11:35.000000 easier-1.3.6/easier/clock.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2118 2020-05-29 19:14:34.000000 easier-1.3.6/easier/crypt.py
+-rw-rw-r--   0 rob        (501) staff       (20)    11821 2023-07-24 14:55:29.000000 easier-1.3.6/easier/dataframe_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4416 2021-10-25 19:35:54.000000 easier-1.3.6/easier/distributions.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3729 2022-11-06 22:52:50.000000 easier-1.3.6/easier/duck.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6934 2023-01-04 21:20:27.000000 easier-1.3.6/easier/duck_model.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1312 2022-12-27 18:28:43.000000 easier-1.3.6/easier/ecdf_lib.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-24 14:59:55.132890 easier-1.3.6/easier/filtering/
+-rw-rw-r--   0 rob        (501) staff       (20)       89 2021-09-24 01:20:15.000000 easier-1.3.6/easier/filtering/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5693 2021-09-24 01:20:25.000000 easier-1.3.6/easier/filtering/elliptic_filter.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2106 2021-11-24 17:03:48.000000 easier-1.3.6/easier/filtering/tvd.py
+-rw-rw-r--   0 rob        (501) staff       (20)    14061 2022-08-17 21:35:50.000000 easier-1.3.6/easier/fit_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8505 2021-01-14 20:54:34.000000 easier-1.3.6/easier/gsheet.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7770 2022-08-16 22:01:30.000000 easier-1.3.6/easier/hvtools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3749 2023-07-01 21:46:38.000000 easier-1.3.6/easier/ibis_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1794 2020-03-27 15:13:42.000000 easier-1.3.6/easier/item.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2136 2020-05-29 19:14:34.000000 easier-1.3.6/easier/iterify.py
+-rw-rw-r--   0 rob        (501) staff       (20)      208 2020-05-29 19:14:34.000000 easier-1.3.6/easier/memory.py
+-rw-rw-r--   0 rob        (501) staff       (20)    11444 2022-11-07 18:39:22.000000 easier-1.3.6/easier/minimodel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8148 2022-08-11 18:33:31.000000 easier-1.3.6/easier/minimodel_orig.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4950 2021-12-08 22:15:51.000000 easier-1.3.6/easier/nice_dates.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2087 2020-05-29 19:14:34.000000 easier-1.3.6/easier/outlier_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3186 2022-08-17 21:35:50.000000 easier-1.3.6/easier/parallel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7743 2019-12-12 19:22:12.000000 easier-1.3.6/easier/param_state.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1195 2022-08-17 21:35:50.000000 easier-1.3.6/easier/plotting.py
+-rw-rw-r--   0 rob        (501) staff       (20)     9482 2022-12-11 17:05:42.000000 easier-1.3.6/easier/postgres.py
+-rw-rw-r--   0 rob        (501) staff       (20)      663 2018-08-08 19:33:34.000000 easier-1.3.6/easier/print_catcher.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6150 2022-11-10 16:40:03.000000 easier-1.3.6/easier/proportion_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3178 2022-09-23 20:00:52.000000 easier-1.3.6/easier/salesforce.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3231 2020-05-29 19:14:34.000000 easier-1.3.6/easier/shaper.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2902 2019-12-12 19:11:38.000000 easier-1.3.6/easier/timer.py
+-rw-rw-r--   0 rob        (501) staff       (20)    19244 2023-01-03 20:00:58.000000 easier-1.3.6/easier/utils.py
+-rw-rw-r--   0 rob        (501) staff       (20)       22 2023-07-24 14:58:45.000000 easier-1.3.6/easier/version.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-24 14:59:55.132255 easier-1.3.6/easier.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)      448 2023-07-24 14:59:55.000000 easier-1.3.6/easier.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)     1018 2023-07-24 14:59:55.000000 easier-1.3.6/easier.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-07-24 14:59:55.000000 easier-1.3.6/easier.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)      117 2023-07-24 14:59:55.000000 easier-1.3.6/easier.egg-info/entry_points.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.3.6/easier.egg-info/not-zip-safe
+-rw-r--r--   0 rob        (501) staff       (20)       36 2023-07-24 14:59:55.000000 easier-1.3.6/easier.egg-info/requires.txt
+-rw-r--r--   0 rob        (501) staff       (20)        7 2023-07-24 14:59:55.000000 easier-1.3.6/easier.egg-info/top_level.txt
+-rw-rw-r--   0 rob        (501) staff       (20)      504 2023-07-24 14:59:55.133409 easier-1.3.6/setup.cfg
+-rw-rw-r--   0 rob        (501) staff       (20)     1638 2021-01-14 22:24:18.000000 easier-1.3.6/setup.py
```

### Comparing `easier-1.3.5/LICENSE` & `easier-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/README.md` & `easier-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/__init__.py` & `easier-1.3.6/easier/__init__.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/api.py` & `easier-1.3.6/easier/api.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/bernstein.py` & `easier-1.3.6/easier/bernstein.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,21 @@
     def compress(self, x, learn_limits=True):
         """
         Compresses the array to [0, 1]
         """
         import numpy as np
 
         if not isinstance(x, np.ndarray):
-            raise ValueError('Input must be numpy array')
+            raise ValueError("Input must be numpy array")
 
         if learn_limits:
             self._set_limits(x)
 
         if None in {self.xmin, self.xmax}:
-            raise ValueError('Compressor never learned range limit')
+            raise ValueError("Compressor never learned range limit")
 
         return (x - self.xmin) / (self.xmax - self.xmin)
 
     def expand(self, x):
         """
         Expands an array to go from [0, 1] interval to original interval
         """
@@ -92,66 +92,73 @@
         self._x = self.compress(x)
         self._y = y
 
         self._func = self._get_interp_function()
 
     def _get_interp_function(self):
         from scipy.interpolate import interp1d
-        return interp1d(self._x, self._y, fill_value=(self._y[0], self._y[-1]), bounds_error=False)
+
+        return interp1d(
+            self._x, self._y, fill_value=(self._y[0], self._y[-1]), bounds_error=False
+        )
 
     def _validate_inputs(self, x, y):
         import numpy as np
 
         if not all(isinstance(v, np.ndarray) for v in [x, y]):
-            raise ValueError('x and y must both be numpy arrays')
+            raise ValueError("x and y must both be numpy arrays")
 
         if not all(len(v) > 2 for v in [x, y]):
-            raise ValueError('x and y must both have at least 3 elements')
+            raise ValueError("x and y must both have at least 3 elements")
 
     def _bern_term(self, n, k, x):
         """
         This function uses logs to make the following code
         safe for large n.
 
         cc = comb(n, k)
         return cc * (1 + self._EPS - x) ** (n - k) * (x + self._EPS) ** k
         """
         import numpy as np
         from scipy.special import gammaln
+
         x = np.clip(x, self._EPS, 1 - self._EPS)
 
         out = gammaln(n + 1) - gammaln(n - k + 1) - gammaln(k + 1)
         out += k * np.log(x) + (n - k) * np.log(1 - x)
         return np.exp(out)
 
     def _get_fit_func(self, infunc):
         """
         Returns a callable of the bernstein approximator
         """
         import numpy as np
+
         N = self.N
         k_vec = np.arange(N + 1)
         coeff_vec = infunc(k_vec / N)
 
         def bern_sum(x):
             x = x.flatten()
             X, K = np.meshgrid(x, k_vec)
             _, C = np.meshgrid(x, coeff_vec)
             B = self._bern_term(N, K, X)
 
             terms = C * B
             out = np.sum(terms, axis=0)
             return out
+
         return bern_sum
 
     def _get_fit_deriv(self, infunc):
         """
         Returns a callable of the bernstein derivative approximator
         """
         import numpy as np
+
         N = self.N
         k_vec = np.arange(N + 1)
         coeff_vec = infunc(k_vec / N)
 
         def bern_sum(x):
             x = x.flatten()
             X, K = np.meshgrid(x, k_vec)
@@ -189,21 +196,32 @@
 
 class BernsteinFitter(BlobMixin):
     _EPS = 1e-15
 
     w = BlobAttr(None)
     scaler_blob = BlobAttr(None)
 
-    def __init__(self, non_negative=True, monotonic=True, increasing=True, match_left=True, match_right=True):
+    def __init__(
+        self,
+        non_negative=False,
+        monotonic=False,
+        increasing=False,
+        match_left=False,
+        match_right=False,
+        match_endpoint_values=False,
+        match_endpoint_derivatives=False,
+    ):
         super().__init__()
         self._non_negative = non_negative
         self._monotonic = monotonic
         self._increasing = increasing
         self._match_left = match_left
         self._match_right = match_right
+        self._match_endpoint_values = match_endpoint_values
+        self._match_endpoint_derivatives = match_endpoint_derivatives
 
     def _bern_term(self, n, k, x):
         """
         This function uses logs to make the following code
         safe for large n.
 
         cc = comb(n, k)
@@ -223,24 +241,26 @@
 
     def _get_design_matrix(self, x, degree):
         """
         x is the array of x points
         n is degree of fitter
         """
         import numpy as np
+
         x = np.array(x)
         A = np.zeros((len(x), degree + 1))
         for k in range(0, degree + 1):
             A[:, k] = self._bern_term(degree, k, x)
         return A
 
     def _get_derivative_matrix(self, x, degree):
         import numpy as np
+
         n = degree
-        if hasattr(x, '__iter__'):
+        if hasattr(x, "__iter__"):
             B = np.zeros((len(x), degree + 1))
         else:
             B = np.zeros((1, degree + 1))
 
         for k in range(0, degree + 1):
             term1 = self._bern_term(n - 1, k - 1, x)
             term2 = self._bern_term(n - 1, k, x)
@@ -259,15 +279,15 @@
         self.scaler_blob = scaler.to_blob()
 
         yv = np.reshape(y, (-1, 1))
         A = self._get_design_matrix(x, degree)
         B = self._get_derivative_matrix(x, degree)
 
         # Define a weight variable to be optimized
-        w = cp.Variable(name='w', shape=(degree + 1, 1))
+        w = cp.Variable(name="w", shape=(degree + 1, 1))
 
         # The objective is the mininum squared error
         objective = cp.Minimize(cp.sum_squares(A @ w - yv))
 
         # Default to unconstrained
         constraints = []
 
@@ -282,64 +302,88 @@
 
         if self._match_left:
             constraints.append(w[0, 0] == y[0])
 
         if self._match_right:
             constraints.append(w[-1, 0] == y[-1])
 
+        # These constraints ensure matching values at end points (periodic)
+        if self._match_endpoint_values:
+            if self._match_left or self._match_right:
+                raise ValueError(
+                    "Cannot have match_left or match_right with match_endpoint_values"
+                )
+            # Constrain the values at the endpoints to match
+            constraints.append(w[0, 0] == w[-1, 0])
+
+        # These constraints ensure matching derivative at end points (periodic)
+        if self._match_endpoint_derivatives:
+            # Get the derivative matrix
+            B = self._get_derivative_matrix(x, degree)
+
+            # Constrain the derivatives at the endpoints to match
+            term1 = B[0, :] @ w
+            term2 = B[-1, :] @ w
+            constraints.append(term1 == term2)
+
         # Add any desired constraints
         kwargs = {}
         if constraints:
-            kwargs['constraints'] = constraints
+            kwargs["constraints"] = constraints
 
         # Solve the problem
         problem = cp.Problem(objective, **kwargs)
         problem.solve(verbose=verbose)
 
         self.w = w.value.flatten()
 
         return self
 
     def predict(self, x):
         """
         Values that fall outside the fiited x range will be pegged to
         the terminal values of the fitter.
         """
-        return self._get_prediction(x, 'value')
+        return self._get_prediction(x, "value")
 
     def predict_derivative(self, x):
         if self.w is None:
-            raise ValueError('You must run fit() or load a blob before running predict()')
+            raise ValueError(
+                "You must run fit() or load a blob before running predict()"
+            )
 
         scaler = Scaler()
         scaler.from_blob(self.scaler_blob)
-        diffs = self._get_prediction(x, 'derivative')
+        diffs = self._get_prediction(x, "derivative")
         return diffs / (scaler.limits[1] - scaler.limits[0])
 
     def _get_prediction(self, x, what):
         import numpy as np
+
         if self.w is None:
-            raise ValueError('You must run fit() or load a blob before running predict()')
+            raise ValueError(
+                "You must run fit() or load a blob before running predict()"
+            )
 
         is_scalar = False
-        if not hasattr(x, '__iter__'):
+        if not hasattr(x, "__iter__"):
             is_scalar = True
             x = [x]
 
         x = np.array(x)
         scaler = Scaler()
         scaler.from_blob(self.scaler_blob)
         x = scaler.transform(x)
 
         degree = len(self.w) - 1
         wv = np.reshape(self.w, (-1, 1))
-        if what == 'value':
+        if what == "value":
             A = self._get_design_matrix(x, degree)
             yv = A @ wv
-        elif what == 'derivative':
+        elif what == "derivative":
             B = self._get_derivative_matrix(x, degree)
             yv = B @ wv
         else:
             raise ValueError('Nope!  Bad "what" argument')
 
         yv = yv.flatten()
         if is_scalar:
@@ -349,15 +393,16 @@
 
     def fit_predict(self, x, y, degree):
         self.fit(x, y, degree)
         return self.predict(x)
 
     def to_blob(self):
         blob = super().to_blob()
-        blob['w'] = list(blob['w'])
+        blob["w"] = list(blob["w"])
         return blob
 
     def from_blob(self, blob):
         import numpy as np
+
         super().from_blob(blob)
         self.w = np.array(self.w)
         return self
```

### Comparing `easier-1.3.5/easier/bigquery.py` & `easier-1.3.6/easier/bigquery.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/cli.py` & `easier-1.3.6/easier/cli.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/clock.py` & `easier-1.3.6/easier/clock.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/crypt.py` & `easier-1.3.6/easier/crypt.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/dataframe_tools.py` & `easier-1.3.6/easier/dataframe_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
             # Create the Pandera DataFrameSchema object and assign it to the schema attribute
             self.schema = pa.DataFrameSchema(typed_cols, **kwargs)
 
         @property
         def ibis_schema(self):
             from ibis.expr import schema as sch
 
-            return sch.schema_from_mapping(
+            return sch.from_mapping(
                 {
                     col: self.schema.dtypes[col].type
                     for col in self.schema.columns.keys()
                 }
             )
 
         def __repr__(self):
```

### Comparing `easier-1.3.5/easier/distributions.py` & `easier-1.3.6/easier/distributions.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/duck.py` & `easier-1.3.6/easier/duck.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/duck_model.py` & `easier-1.3.6/easier/duck_model.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/ecdf_lib.py` & `easier-1.3.6/easier/ecdf_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/filtering/elliptic_filter.py` & `easier-1.3.6/easier/filtering/elliptic_filter.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/filtering/tvd.py` & `easier-1.3.6/easier/filtering/tvd.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/fit_lib.py` & `easier-1.3.6/easier/fit_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/gsheet.py` & `easier-1.3.6/easier/gsheet.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/hvtools.py` & `easier-1.3.6/easier/hvtools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/ibis_tools.py` & `easier-1.3.6/easier/ibis_tools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/item.py` & `easier-1.3.6/easier/item.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/iterify.py` & `easier-1.3.6/easier/iterify.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/minimodel.py` & `easier-1.3.6/easier/minimodel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/minimodel_orig.py` & `easier-1.3.6/easier/minimodel_orig.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/nice_dates.py` & `easier-1.3.6/easier/nice_dates.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/outlier_tools.py` & `easier-1.3.6/easier/outlier_tools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/parallel.py` & `easier-1.3.6/easier/parallel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/param_state.py` & `easier-1.3.6/easier/param_state.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/plotting.py` & `easier-1.3.6/easier/plotting.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/postgres.py` & `easier-1.3.6/easier/postgres.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/print_catcher.py` & `easier-1.3.6/easier/print_catcher.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/proportion_lib.py` & `easier-1.3.6/easier/proportion_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/salesforce.py` & `easier-1.3.6/easier/salesforce.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/shaper.py` & `easier-1.3.6/easier/shaper.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/timer.py` & `easier-1.3.6/easier/timer.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier/utils.py` & `easier-1.3.6/easier/utils.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/easier.egg-info/SOURCES.txt` & `easier-1.3.6/easier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easier-1.3.5/setup.py` & `easier-1.3.6/setup.py`

 * *Files identical despite different names*

