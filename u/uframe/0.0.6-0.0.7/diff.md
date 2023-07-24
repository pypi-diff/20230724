# Comparing `tmp/uframe-0.0.6.tar.gz` & `tmp/uframe-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uframe-0.0.6.tar", last modified: Fri Jul 21 06:52:15 2023, max compression
+gzip compressed data, was "uframe-0.0.7.tar", last modified: Mon Jul 24 11:12:34 2023, max compression
```

## Comparing `uframe-0.0.6.tar` & `uframe-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.364549 uframe-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-07-21 06:52:15.365549 uframe-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.6/README.md
--rw-rw-rw-   0        0        0     1055 2023-07-21 06:51:42.000000 uframe-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      462 2023-07-21 06:52:15.366549 uframe-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.313549 uframe-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.325549 uframe-0.0.6/src/uframe/
--rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.6/src/uframe/__init__.py
--rw-rw-rw-   0        0        0    61223 2023-07-20 11:22:06.000000 uframe-0.0.6/src/uframe/uframe.py
--rw-rw-rw-   0        0        0     7115 2023-07-20 15:56:21.000000 uframe-0.0.6/src/uframe/uframe_from_mice.py
--rw-rw-rw-   0        0        0    12958 2023-07-20 11:30:18.000000 uframe-0.0.6/src/uframe/uframe_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.349549 uframe-0.0.6/src/uframe.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.6/src/uframe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      142 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.363566 uframe-0.0.6/tests/
--rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.6/tests/test_uframe.py
--rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.6/tests/test_uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.880882 uframe-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-07-24 11:12:34.880882 uframe-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1055 2023-07-24 11:02:02.000000 uframe-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      462 2023-07-24 11:12:34.880882 uframe-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.837648 uframe-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.865181 uframe-0.0.7/src/uframe/
+-rw-rw-rw-   0        0        0      583 2023-07-21 13:40:49.000000 uframe-0.0.7/src/uframe/__init__.py
+-rw-rw-rw-   0        0        0    60935 2023-07-21 13:39:57.000000 uframe-0.0.7/src/uframe/uframe.py
+-rw-rw-rw-   0        0        0     6880 2023-07-24 08:36:56.000000 uframe-0.0.7/src/uframe/uframe_from_mice.py
+-rw-rw-rw-   0        0        0    12958 2023-07-24 06:43:12.000000 uframe-0.0.7/src/uframe/uframe_instance.py
+-rw-rw-rw-   0        0        0      123 2023-07-21 13:40:05.000000 uframe-0.0.7/src/uframe/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.880882 uframe-0.0.7/src/uframe.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.7/src/uframe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      142 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 11:12:34.000000 uframe-0.0.7/src/uframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 11:12:34.880882 uframe-0.0.7/tests/
+-rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.7/tests/test_uframe.py
+-rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.7/tests/test_uframe_instance.py
```

### Comparing `uframe-0.0.6/LICENSE` & `uframe-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `uframe-0.0.6/PKG-INFO` & `uframe-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.6/README.md` & `uframe-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `uframe-0.0.6/pyproject.toml` & `uframe-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
 
 [project]
 name = "uframe"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Christian Amesoder", email="christian.amesoeder@informatik.uni-regensburg.de" },
   { name="Michael Hagn", email="michael.hagn@stud.uni-regensburg.de" }
 ]
 description = "Package for handling uncertain data"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `uframe-0.0.6/src/uframe/__init__.py` & `uframe-0.0.7/src/uframe/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 __author__ = """Christian Amesoeder and Michael Hagn"""
 __email__ = 'christian.amesoeder@informatik.uni-regensburg.de'
 __version__ = '0.0.1'
 
 
 from .uframe import uframe
 from .uframe_instance import uframe_instance
-
-from.uframe_from_mice import ( uframe_from_array_mice_2,
+from .utils import load_uframe
+from.uframe_from_mice import (uframe_from_array_mice_2,
             uframe_from_array_mice,
             uframe_noisy_array)
 __all__ = [
     "uframe",
     "uframe_instance",
     "uframe_from_array_mice",
     "uframe_noisy_array",
-    "uframe_from_array_mice_2"]
+    "uframe_from_array_mice_2",
+    "load_uframe"]
```

### Comparing `uframe-0.0.6/src/uframe/uframe.py` & `uframe-0.0.7/src/uframe/uframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1074,31 +1074,18 @@
     #self cat value code dict muss an uframe instances übergeben werden 
     #damit dann auch die label encoder Geschichten ersetzen!
     
     #neue get dummies Funktion, die gleich ein array nimmt, später dann die bisherige Version anpassen 
     
     def save(self, name="saved_uframe.pkl"):
             
-        d = vars(self)
-        print("Save the following dict:", vars(self))
         with open(name, 'wb') as f:
-            pickle.dump(d,f)
+            pickle.dump(self,f)
         return 
-    
-def load_uframe(file):
-    
-    with open(file, 'rb') as f:
-        d = pickle.load(f)
-    
-    frame = uframe()
-    
-    for key in d.keys():
-        setattr(frame, key, d[key])
-    
-    return frame 
+     
 
 def analysis_table(true, preds): 
     residues = true - preds
     true_q= np.array([sum(true[k]<true)/len(true) for k in range(len(true))])
     new_q = np.array([sum(preds[k]<true)/len(true) for k in range(len(true))])
 
     return [["Var",str(round(np.var(residues),2))],
```

### Comparing `uframe-0.0.6/src/uframe/uframe_from_mice.py` & `uframe-0.0.7/src/uframe/uframe_from_mice.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,26 +76,28 @@
     u.append(new=[x, distr])
     
 
     return u
 
 
 
-def generate_missing_values(complete_data, p):
+def generate_missing_values(complete_data, p, seed):
     shape = complete_data.shape
     y = complete_data.copy()
     np.random.seed(seed)
-    missing = np.random.binomial(1, p, shape)
     
-    y[missing.astype('bool')] = np.nan
+    if p >0: 
+        missing = np.random.binomial(1, p, shape)
+        y[missing.astype('bool')] = np.nan
+        
     return y, missing
 
 
 def uframe_from_array_mice_2(a: np.ndarray, p=0.1, mice_iterations=5, kernel="stats.gaussian_kde",
-                           scaler= "min_max", cat_indices=[],seed = None, **kwargs):
+                           scaler= "min_max", cat_indices=[], seed = None, **kwargs):
 
     x, missing = generate_missing_values(a, p,seed)
 
     distr = {}
     cat_distr = {}
     index_dict={}
 
@@ -153,43 +155,36 @@
             
         if len(imp_arrays) == 0:
             continue
         
         imp_array = np.concatenate(imp_arrays, axis=0)
         scaler = MinMaxScaler()
         imp_array = (scaler.fit_transform(imp_array.T)).T
-        #print("Shape of imp array", imp_array.shape)
-
+        
         if kernel == "stats.gaussian_kde":
             kde = stats.gaussian_kde(imp_array)
 
         else:
             imp_array = imp_array.T
             kde = KernelDensity(kernel=kernel, **kwargs).fit(imp_array)
             #print("Dimension of kde", kde.n_features_in_)
 
         imp_distr = kde
 
         distr[i] = imp_distr
 
-    #print(x)
     cont_indices = [i for i in range(x.shape[1]) if i not in cat_indices]
-    #print("Cont indices")
     scaler= MinMaxScaler()
     x_cont = scaler.fit_transform(x[:,cont_indices])
-    #print("X cont scaled", x_cont)
     x[:,cont_indices]=x_cont
-    #print("X after scaling", x, x[:,cat_indices])
-    #a[missing==1]=np.nan
+    
     u = uframe()
     
-    #print("Cat distr", cat_distr)
     u.append(new=[x, distr, cat_distr, index_dict])
 
-    #print("Col dtype", u._col_dtype)
     return u
 
 
 # add Gaussian noise of given std to chosen entries
 # relative=True: multiply std with standard deviation of the column to get the std for a column
 def uframe_noisy_array(a: np.ndarray, std=0.1, relative=False, unc_percentage=0.1):
```

### Comparing `uframe-0.0.6/src/uframe/uframe_instance.py` & `uframe-0.0.7/src/uframe/uframe_instance.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.6/src/uframe.egg-info/PKG-INFO` & `uframe-0.0.7/src/uframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.6/tests/test_uframe_instance.py` & `uframe-0.0.7/tests/test_uframe_instance.py`

 * *Files identical despite different names*

