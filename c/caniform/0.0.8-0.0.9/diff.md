# Comparing `tmp/caniform-0.0.8.tar.gz` & `tmp/caniform-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caniform-0.0.8.tar", last modified: Thu Jun 15 20:54:46 2023, max compression
+gzip compressed data, was "caniform-0.0.9.tar", last modified: Mon Jul 24 20:04:12 2023, max compression
```

## Comparing `caniform-0.0.8.tar` & `caniform-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:54:46.010411 caniform-0.0.8/
--rw-r--r--   0 dev        (501) staff       (20)     1112 2022-06-02 18:33:45.000000 caniform-0.0.8/LICENSE
--rw-r--r--   0 dev        (501) staff       (20)      610 2023-06-15 20:54:46.010517 caniform-0.0.8/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)       93 2022-06-02 18:36:10.000000 caniform-0.0.8/README.md
--rw-r--r--   0 dev        (501) staff       (20)      151 2022-06-07 15:32:34.000000 caniform-0.0.8/pyproject.toml
--rw-r--r--   0 dev        (501) staff       (20)      642 2023-06-15 20:54:46.011236 caniform-0.0.8/setup.cfg
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:54:46.006433 caniform-0.0.8/src/
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:54:46.008717 caniform-0.0.8/src/caniform/
--rw-r--r--   0 dev        (501) staff       (20)     9305 2023-06-15 20:53:47.000000 caniform-0.0.8/src/caniform/Extend.py
--rw-r--r--   0 dev        (501) staff       (20)        0 2022-06-02 18:32:13.000000 caniform-0.0.8/src/caniform/__init__.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:54:46.010191 caniform-0.0.8/src/caniform.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)      610 2023-06-15 20:54:45.000000 caniform-0.0.8/src/caniform.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      234 2023-06-15 20:54:46.000000 caniform-0.0.8/src/caniform.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2023-06-15 20:54:45.000000 caniform-0.0.8/src/caniform.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (501) staff       (20)        9 2023-06-15 20:54:45.000000 caniform-0.0.8/src/caniform.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-07-24 20:04:12.808055 caniform-0.0.9/
+-rw-r--r--   0 dev        (501) staff       (20)     1112 2022-06-02 18:33:45.000000 caniform-0.0.9/LICENSE
+-rw-r--r--   0 dev        (501) staff       (20)      610 2023-07-24 20:04:12.808167 caniform-0.0.9/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)       93 2022-06-02 18:36:10.000000 caniform-0.0.9/README.md
+-rw-r--r--   0 dev        (501) staff       (20)      131 2023-07-24 20:03:21.000000 caniform-0.0.9/pyproject.toml
+-rw-r--r--   0 dev        (501) staff       (20)      642 2023-07-24 20:04:12.808919 caniform-0.0.9/setup.cfg
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-07-24 20:04:12.803870 caniform-0.0.9/src/
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-07-24 20:04:12.806358 caniform-0.0.9/src/caniform/
+-rw-r--r--   0 dev        (501) staff       (20)     9399 2023-07-24 20:03:26.000000 caniform-0.0.9/src/caniform/Extend.py
+-rw-r--r--   0 dev        (501) staff       (20)        0 2022-06-02 18:32:13.000000 caniform-0.0.9/src/caniform/__init__.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-07-24 20:04:12.807789 caniform-0.0.9/src/caniform.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)      610 2023-07-24 20:04:12.000000 caniform-0.0.9/src/caniform.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      234 2023-07-24 20:04:12.000000 caniform-0.0.9/src/caniform.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2023-07-24 20:04:12.000000 caniform-0.0.9/src/caniform.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)        9 2023-07-24 20:04:12.000000 caniform-0.0.9/src/caniform.egg-info/top_level.txt
```

### Comparing `caniform-0.0.8/LICENSE` & `caniform-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `caniform-0.0.8/PKG-INFO` & `caniform-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caniform
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package that extends the functionality of Pandas.
 Home-page: https://gitlab.com/tomathon/caniform/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/caniform/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caniform-0.0.8/setup.cfg` & `caniform-0.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = caniform
-version = 0.0.8
+version = 0.0.9
 author = tomathon
 author_email = tomathon.dev@pm.me
 description = A package that extends the functionality of Pandas.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/tomathon/caniform/
 project_urls =
```

### Comparing `caniform-0.0.8/src/caniform/Extend.py` & `caniform-0.0.9/src/caniform/Extend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sklearn.linear_model import LinearRegression
+# from sklearn.linear_model import LinearRegression
 import pandas as pd
 import numpy as np
 import re
 import json
 import requests
 from concurrent.futures import ThreadPoolExecutor
 
@@ -55,24 +55,25 @@
         for f in [*args]:
             tmp = rematch(clist, f)
             new_cols.extend(tmp)
         ret = df[new_cols]
         return ret
     
     
-    def cols_paste(self, *args, sep = "-", new_name = "auto", drop_ori = True, verbose = True):
+    def cols_paste(self, *args, sep = "-", new_name = "auto", drop_ori = True, show_verbose = True):
         df = self._obj
         idx = df.index
         df = df.reset_index(drop = True)
         join_cols = [*args]
         if new_name == "auto":
             new_name = "_".join(join_cols)
         tmp_df = df[join_cols].applymap(str)
         new_col = []
-        print(f"Pasting columns {', '.join(join_cols)} using sep = '{sep}' into new column '{new_name}'")
+        if show_verbose:
+            print(f"Pasting columns {', '.join(join_cols)} using sep = '{sep}' into new column '{new_name}'")
         for r in range(0, tmp_df.shape[0]):
             tmp = sep.join(tmp_df.loc[r].tolist())
             new_col.append(tmp)
         ret = df.assign(auto = new_col).rename(columns = {"auto": new_name})
         if drop_ori:
             ret = ret.drop(join_cols, axis = 1)
         ret.index = idx
@@ -147,43 +148,43 @@
             )
             if add_prop:
                 ret["prop"] = np.round(ret.n / df.shape[0], round_to)
         ret = ret.reset_index(drop = True)
         return ret
     
     
-    def lm(self, x, y, ret = "rsquared", round_to = 3, show_verbose = True):
-        df = self._obj
-        x_name = x
-        y_name = y
-        X = df[x]
-        y = df[y]
-        if type(X) != np.ndarray:
-            X = np.array(X).reshape((-1, 1))
-        if type(y) != np.ndarray:
-            y = np.array(y).reshape((-1, 1))
-        mod = LinearRegression().fit(X, y)
-        ret = ret.lower()
-        if ret not in ["rsquared", "coef", "intercept"]:
-            raise TypeError("Arg 'ret' must be one of 'rsquared', 'coef', or 'intercept'")
-        if ret == "rsquared":
-            rsquared = np.round(mod.score(X, y), round_to)
-            if show_verbose:
-                print(f"The change in '{y_name}' is ~{np.round(rsquared*100, round_to)}% explained by a change in '{x_name}'")
-            return rsquared
-        elif ret == "coef":
-            coef = np.round(mod.coef_[0][0], round_to)
-            if show_verbose:
-                print(f"For every incremental change in '{x_name}', '{y_name}' changes by {coef}")
-            return coef
-        else:
-            intercept = np.round(mod.intercept_[0], round_to)
-            if show_verbose:
-                print(f"With a y-intercept of {intercept}, '{y_name}' is independent of '{x_name}' when it is {intercept}")
-            return intercept
+    # def lm(self, x, y, ret = "rsquared", round_to = 3, show_verbose = True):
+    #     df = self._obj
+    #     x_name = x
+    #     y_name = y
+    #     X = df[x]
+    #     y = df[y]
+    #     if type(X) != np.ndarray:
+    #         X = np.array(X).reshape((-1, 1))
+    #     if type(y) != np.ndarray:
+    #         y = np.array(y).reshape((-1, 1))
+    #     mod = LinearRegression().fit(X, y)
+    #     ret = ret.lower()
+    #     if ret not in ["rsquared", "coef", "intercept"]:
+    #         raise TypeError("Arg 'ret' must be one of 'rsquared', 'coef', or 'intercept'")
+    #     if ret == "rsquared":
+    #         rsquared = np.round(mod.score(X, y), round_to)
+    #         if show_verbose:
+    #             print(f"The change in '{y_name}' is ~{np.round(rsquared*100, round_to)}% explained by a change in '{x_name}'")
+    #         return rsquared
+    #     elif ret == "coef":
+    #         coef = np.round(mod.coef_[0][0], round_to)
+    #         if show_verbose:
+    #             print(f"For every incremental change in '{x_name}', '{y_name}' changes by {coef}")
+    #         return coef
+    #     else:
+    #         intercept = np.round(mod.intercept_[0], round_to)
+    #         if show_verbose:
+    #             print(f"With a y-intercept of {intercept}, '{y_name}' is independent of '{x_name}' when it is {intercept}")
+    #         return intercept
         
     
     def to_month(self, col, use_abbr = True):
         df = self._obj
         if use_abbr:
             month_index = {
                 1: "Jan", 2: "Feb", 3: "Mar", 4: "Apr",
```

### Comparing `caniform-0.0.8/src/caniform.egg-info/PKG-INFO` & `caniform-0.0.9/src/caniform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caniform
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package that extends the functionality of Pandas.
 Home-page: https://gitlab.com/tomathon/caniform/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/caniform/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

