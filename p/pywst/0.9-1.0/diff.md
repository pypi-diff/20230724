# Comparing `tmp/pywst-0.9.tar.gz` & `tmp/pywst-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywst-0.9.tar", last modified: Thu Jul 16 13:37:19 2020, max compression
+gzip compressed data, was "pywst-1.0.tar", last modified: Mon Jul 24 11:03:22 2023, max compression
```

## Comparing `pywst-0.9.tar` & `pywst-1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-07-16 13:37:19.000000 pywst-0.9/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1925 2020-07-16 13:37:19.000000 pywst-0.9/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1100 2020-07-16 13:24:08.000000 pywst-0.9/README.md
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-07-16 13:37:19.000000 pywst-0.9/pywst/
--rw-r--r--   0 bruno     (1000) bruno     (1000)      257 2020-05-26 10:20:12.000000 pywst-0.9/pywst/__init__.py
--rwxrwxr-x   0 bruno     (1000) bruno     (1000)     7428 2020-05-28 08:45:17.000000 pywst-0.9/pywst/filters.py
--rwxrwxr-x   0 bruno     (1000) bruno     (1000)    22901 2020-07-10 17:29:37.000000 pywst-0.9/pywst/rwst.py
--rwxrwxr-x   0 bruno     (1000) bruno     (1000)    11970 2020-07-06 10:28:18.000000 pywst-0.9/pywst/rwst_models.py
--rwxrwxr-x   0 bruno     (1000) bruno     (1000)     9445 2020-07-10 17:15:58.000000 pywst-0.9/pywst/rwst_operator.py
--rwxrwxr-x   0 bruno     (1000) bruno     (1000)     2000 2020-06-19 09:23:45.000000 pywst-0.9/pywst/utils.py
--rwxrwxr-x   0 bruno     (1000) bruno     (1000)    25280 2020-07-10 13:54:31.000000 pywst-0.9/pywst/wst.py
--rwxrwxr-x   0 bruno     (1000) bruno     (1000)     9807 2020-07-03 09:47:52.000000 pywst-0.9/pywst/wst_operator.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2020-07-16 13:37:19.000000 pywst-0.9/pywst.egg-info/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1925 2020-07-16 13:37:19.000000 pywst-0.9/pywst.egg-info/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      277 2020-07-16 13:37:19.000000 pywst-0.9/pywst.egg-info/SOURCES.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2020-07-16 13:37:19.000000 pywst-0.9/pywst.egg-info/dependency_links.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        6 2020-07-16 13:37:19.000000 pywst-0.9/pywst.egg-info/top_level.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2020-07-16 13:37:19.000000 pywst-0.9/setup.cfg
--rw-r--r--   0 bruno     (1000) bruno     (1000)      679 2020-07-16 13:33:08.000000 pywst-0.9/setup.py
+drwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)        0 2023-07-24 11:03:22.374035 pywst-1.0/
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)     1528 2023-07-24 10:25:17.000000 pywst-1.0/LICENSE.md
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)     1778 2023-07-24 11:03:22.371933 pywst-1.0/PKG-INFO
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)     1312 2023-07-24 10:46:02.000000 pywst-1.0/README.md
+drwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)        0 2023-07-24 11:03:22.349086 pywst-1.0/pywst/
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)      277 2023-07-24 10:44:22.000000 pywst-1.0/pywst/__init__.py
+-rwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)     7425 2023-07-24 10:32:42.000000 pywst-1.0/pywst/filters.py
+-rwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)    23725 2023-07-24 10:25:17.000000 pywst-1.0/pywst/rwst.py
+-rwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)    12892 2023-07-24 10:25:17.000000 pywst-1.0/pywst/rwst_models.py
+-rwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)     9802 2023-07-24 10:25:17.000000 pywst-1.0/pywst/rwst_operator.py
+-rwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)     2000 2023-07-24 10:25:17.000000 pywst-1.0/pywst/utils.py
+-rwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)    27136 2023-07-24 10:35:40.000000 pywst-1.0/pywst/wst.py
+-rwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)     9930 2023-07-24 10:25:17.000000 pywst-1.0/pywst/wst_operator.py
+drwxrwxr-x   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)        0 2023-07-24 11:03:22.367031 pywst-1.0/pywst.egg-info/
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)     1778 2023-07-24 11:03:22.355302 pywst-1.0/pywst.egg-info/PKG-INFO
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)      288 2023-07-24 11:03:22.359502 pywst-1.0/pywst.egg-info/SOURCES.txt
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)        1 2023-07-24 11:03:22.363700 pywst-1.0/pywst.egg-info/dependency_links.txt
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)        6 2023-07-24 11:03:22.368032 pywst-1.0/pywst.egg-info/top_level.txt
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)       38 2023-07-24 11:03:22.375036 pywst-1.0/setup.cfg
+-rw-rw-r--   0 bregaldosaintblancard  (1908) bregaldosaintblancard  (1908)      679 2023-07-24 10:44:02.000000 pywst-1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pywst-0.9/PKG-INFO` & `pywst-1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 Metadata-Version: 2.1
 Name: pywst
-Version: 0.9
+Version: 1.0
 Summary: WST and RWST analyses tools for astrophysical data.
 Home-page: https://github.com/bregaldo/pywst
 Author: Bruno Régaldo-Saint Blancard
 Author-email: bruno.regaldo@phys.ens.fr
-License: UNKNOWN
-Description: # PyWST : WST and RWST for astrophysics
-        
-        PyWST is a public Python package designed to perform statistical analyses of two-dimensional data with the Wavelet Scattering Transform (WST) and the Reduced Wavelet Scattering Transform (RWST).
-        
-        The WST/RWST give you convenient sets of coefficients that describe your non-Gaussian data in a comprehensive way.
-        
-        Install PyWST and check out our [Jupyter notebook tutorial](examples/tutorial.ipynb) in the *examples/* folder.
-        
-        If you use this package, please cite the following paper:
-        
-        B. Regaldo-Saint Blancard, F. Levrier, E. Allys, E. Bellomi, F. Boulanger (2020). Statistical description of dust polarized emission from the diffuse interstellar medium - A WST/RWST approach. arXiv preprint arXiv:????
-        
-        ## Install/Uninstall
-        
-        ### Standard installation (from the Python Package Index)
-        
-        Type in a console:
-        
-        ```
-        pip install pywst
-        ```
-        
-        ### Install from source
-        
-        Clone the repository and type from the main directory:
-        
-        ```
-        pip install -r requirements.txt
-        pip install .
-        ```
-        
-        ### Uninstall
-        
-        ```
-        pip uninstall pywst
-        ```
-        
-        ## Changelog
-        
-        ### 0.9
-        
-        * First public version.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# PyWST : WST and RWST for astrophysics
+
+PyWST is a public Python package designed to perform statistical analyses of two-dimensional data with the Wavelet Scattering Transform (WST) and the Reduced Wavelet Scattering Transform (RWST).
+
+The WST/RWST give you convenient sets of coefficients that describe your non-Gaussian data in a comprehensive way.
+
+Install PyWST and check out our [Jupyter notebook tutorial](examples/tutorial.ipynb) in the *examples/* folder.
+
+If you use this package, please cite the following paper:
+
+B. Regaldo-Saint Blancard, F. Levrier, E. Allys, E. Bellomi, F. Boulanger (2020). Statistical description of dust polarized emission from the diffuse interstellar medium - A RWST approach. arXiv preprint [arXiv:2007.08242](https://arxiv.org/abs/2007.08242)
+
+*Note:* For GPU-accelerated WST computations, take a look at [kymatio](https://github.com/kymatio/kymatio) (on which part of this code is based).
+
+## Install/Uninstall
+
+### Standard installation (from the Python Package Index)
+
+Type in a console:
+
+```
+pip install pywst
+```
+
+### Install from source
+
+Clone the repository and type from the main directory:
+
+```
+pip install -r requirements.txt
+pip install .
+```
+
+### Uninstall
+
+```
+pip uninstall pywst
+```
+
+## Changelog
+
+### 1.0
+
+* Minor updates.
+
+### 0.9
+
+* First public version.
```

### Comparing `pywst-0.9/README.md` & `pywst-1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 The WST/RWST give you convenient sets of coefficients that describe your non-Gaussian data in a comprehensive way.
 
 Install PyWST and check out our [Jupyter notebook tutorial](examples/tutorial.ipynb) in the *examples/* folder.
 
 If you use this package, please cite the following paper:
 
-B. Regaldo-Saint Blancard, F. Levrier, E. Allys, E. Bellomi, F. Boulanger (2020). Statistical description of dust polarized emission from the diffuse interstellar medium - A WST/RWST approach. arXiv preprint arXiv:????
+B. Regaldo-Saint Blancard, F. Levrier, E. Allys, E. Bellomi, F. Boulanger (2020). Statistical description of dust polarized emission from the diffuse interstellar medium - A RWST approach. arXiv preprint [arXiv:2007.08242](https://arxiv.org/abs/2007.08242)
+
+*Note:* For GPU-accelerated WST computations, take a look at [kymatio](https://github.com/kymatio/kymatio) (on which part of this code is based).
 
 ## Install/Uninstall
 
 ### Standard installation (from the Python Package Index)
 
 Type in a console:
 
@@ -33,10 +35,14 @@
 
 ```
 pip uninstall pywst
 ```
 
 ## Changelog
 
+### 1.0
+
+* Minor updates.
+
 ### 0.9
 
 * First public version.
```

### Comparing `pywst-0.9/pywst/filters.py` & `pywst-1.0/pywst/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
         Base class for filters.
     """
     
     def __init__(self, M, N):
         self.M = M
         self.N = N
-        self.data = np.zeros((M, N), np.complex)
+        self.data = np.zeros((M, N), complex)
         self.type = self.__class__.__name__
         
         
 class GaborFilter (Filter):
     """
     Gabor filter.
```

### Comparing `pywst-0.9/pywst/rwst.py` & `pywst-1.0/pywst/rwst.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,52 +8,55 @@
 
 class RWST:
     """
     Reduced Wavelet Scattering Transform (RWST) class contains the output of the RWST of an image or a batch of images.
     This contains the corresponding coefficients and helps to handle and to plot these coefficients.
     """
     
-    def __init__(self, J, L, model, loc_shape=()):
+    def __init__(self, J, L, model, loc_shape=(), j_min=0):
         """
         Constructor.
 
         Parameters
         ----------
         J : int
             Number of dyadic scales.
         L : int
             Number of angles between 0 and pi.
         model : RWSTModelBase
             Chosen RWST model object.
         loc_shape : tuple of ints, optional
             Shape of the local dimensions (batch dimension + local dimensions)
+        j_min : type, optional
+            Minimum dyadic scale. The default is 0.
 
         Returns
         -------
         None.
 
         """
         self.J = J
         self.L = L
         self.model = model
+        self.j_min = j_min
         
         self.coeffs = {}
         self.coeffs_cov = {}
         
         # Information on the original WST coefficients
         self.wst_log2vals = False
         self.wst_normalized = False
         
         # Initialization for each of the three layer of coefficients
         self.coeffs['m0'] = np.zeros((1,) + loc_shape)
-        self.coeffs['m1'] = np.zeros((J, model.layer1_nbparams + 1) + loc_shape)       # +1 to add chi2r coefficients
-        self.coeffs['m2'] = np.zeros((J, J, model.layer2_nbparams + 1) + loc_shape)    # +1 to add chi2r coefficients
+        self.coeffs['m1'] = np.zeros((J - j_min, model.layer1_nbparams + 1) + loc_shape)       # +1 to add chi2r coefficients
+        self.coeffs['m2'] = np.zeros((J - j_min, J - j_min, model.layer2_nbparams + 1) + loc_shape)    # +1 to add chi2r coefficients
         self.coeffs_cov['m0'] = np.zeros((1, 1) + loc_shape) # Actually, it is not possible yet to get local information for this m0 covariance matrix.
-        self.coeffs_cov['m1'] = np.zeros((J, model.layer1_nbparams, model.layer1_nbparams) + loc_shape)
-        self.coeffs_cov['m2'] = np.zeros((J, J, model.layer2_nbparams, model.layer2_nbparams) + loc_shape)
+        self.coeffs_cov['m1'] = np.zeros((J - j_min, model.layer1_nbparams, model.layer1_nbparams) + loc_shape)
+        self.coeffs_cov['m2'] = np.zeros((J - j_min, J - j_min, model.layer2_nbparams, model.layer2_nbparams) + loc_shape)
         
     def _set_mask(self, mask):
         """
         Use MaskedArray objects to deal with masked values when applicable.
 
         Parameters
         ----------
@@ -101,22 +104,22 @@
         None.
 
         """
         if layer == 0:
             self.coeffs['m0'] = coeffs
             self.coeffs_cov['m0'][:] = coeffs_cov
         elif layer == 1:
-            self.coeffs['m1'][jVals, :-1] = coeffs
-            self.coeffs['m1'][jVals, -1:] = chi2r
-            self.coeffs_cov['m1'][jVals] = coeffs_cov
+            self.coeffs['m1'][jVals - self.j_min, :-1] = coeffs
+            self.coeffs['m1'][jVals - self.j_min, -1:] = chi2r
+            self.coeffs_cov['m1'][jVals - self.j_min] = coeffs_cov
         elif layer == 2:
             j1, j2 = jVals
-            self.coeffs['m2'][j1, j2, :-1] = coeffs
-            self.coeffs['m2'][j1, j2, -1:] = chi2r
-            self.coeffs_cov['m2'][j1, j2] = coeffs_cov
+            self.coeffs['m2'][j1 - self.j_min, j2 -self.j_min, :-1] = coeffs
+            self.coeffs['m2'][j1 - self.j_min, j2 - self.j_min, -1:] = chi2r
+            self.coeffs_cov['m2'][j1 - self.j_min, j2 - self.j_min] = coeffs_cov
 
     def get_coeffs(self, name):
         """
         Returns the selected set of RWST coefficients.
 
         Parameters
         ----------
@@ -208,24 +211,24 @@
         """
         if layer == 0:
             return self.coeffs_cov['m0']
         elif layer == 1:
             if j1 is None:
                 return self.coeffs_cov['m1']
             else:
-                return self.coeffs_cov['m1'][j1]
+                return self.coeffs_cov['m1'][j1 - self.j_min]
         elif layer == 2:
             if j1 is None and j2 is None:
                 return self.coeffs_cov['m2']
             elif j1 is None and j2 is not None:
-                return self.coeffs_cov['m2'][:, j2]
+                return self.coeffs_cov['m2'][:, j2 - self.j_min]
             elif j1 is not None and j2 is None:
-                return self.coeffs_cov['m2'][j1, :]
+                return self.coeffs_cov['m2'][j1 - self.j_min, :]
             else:
-                return self.coeffs_cov['m2'][j1, j2]
+                return self.coeffs_cov['m2'][j1 - self.j_min, j2 - self.j_min]
         else:
             raise Exception("Choose a layer between 0 and 2!")
             
     def _finalize(self):
         """
         Internal function that is called by RWSTOp.apply.
         Call the corresponding model finalize function that typically deal with potential model parameters degeneracies
@@ -289,15 +292,15 @@
             
     def plot_compare(self, rwst_list, names=[], labels=[]):
         """
         Plot of the selected set of RWST coefficients of the current object next to those from a given list of other RWST objects.
         
         Default behaviour plots layer 1 and layer 2 coefficients, and the reduced chi square values.
         
-        Note that the current object and the objects of rwst_list must be of consistent J, L, RWST model.
+        Note that the current object and the objects of rwst_list must be of consistent J, L, RWST model, j_min.
 
         Parameters
         ----------
         rwst_list : RWST or list of RWST
             RWST object or list of multiple RWST objects.
         names : str or list of str, optional
             List of coefficients we want to plot on the same figure.
@@ -318,15 +321,15 @@
             rwst_list_loc = [rwst_list] # Easier to make a list in the following
         else:
             rwst_list_loc = rwst_list.copy() # Local shallow copy
         for elt in rwst_list_loc:
             if type(elt) != RWST:
                 raise Exception("rwst_list must be a RWST object or a list of RWST objects!")
             else:
-                if self.J != elt.J or self.L != elt.L or type(self.model) != type(elt.model):
+                if self.J != elt.J or self.L != elt.L or self.j_min != elt.j_min or type(self.model) != type(elt.model):
                     raise Exception("Inconsistent RWST objects.")
             
         if names == []:
             self.plot_compare(rwst_list, names=self.model.layer1_names, labels=labels)
             self.plot_compare(rwst_list, names=self.model.layer2_names, labels=labels)
             self.plot_compare(rwst_list, names=["chi2r1", "chi2r2"], labels=labels)
         else:
@@ -375,20 +378,20 @@
                 
                 color_cnt = 0 # Count for the color cycle
                 
                 for rwst_index, rwst_curr in enumerate(rwst_list_loc): # For every RWST object in rwst_list
                 
                     # Get local parameters
                     loc_shape = rwst_curr.coeffs['m0'].shape[1:]
-                    # Get a mask associated to S0 coefficient if any local coefficient turns out to be masked (we assume uniform mask along coefficient index axis).
-                    mask = ma.getmaskarray(rwst_curr.coeffs['m0'][0])
+                    # Get a mask associated to S2 coefficient if any local coefficient turns out to be masked (we assume uniform mask along coefficient index axis).
+                    mask = ma.getmaskarray(rwst_curr.coeffs['m2'][0,0,0])
                     # Define an index of local positions that are not masked.
                     validLocIndex = [loc for loc in np.ndindex(loc_shape) if mask[loc] == False]
                     
-                    j1Vals = np.arange(rwst_curr.J)
+                    j1Vals = np.arange(rwst_curr.j_min, rwst_curr.J)
                     
                     if ax_index < len(indexLayer1): # Plot instructions for first order coefficients
                         index = indexLayer1[ax_index]
                         for locIndex in validLocIndex:
                             color = colorCycle[color_cnt % len(colorCycle)]
                             
                             coeffs = rwst_curr.coeffs['m1'][np.index_exp[:, index] + locIndex]
@@ -426,32 +429,34 @@
                             color = colorCycle[color_cnt % len(colorCycle)]
                             
                             coeffs = rwst_curr.coeffs['m2'][np.index_exp[:, :, index] + locIndex]
                             if index != rwst_curr.model.layer2_nbparams: # No std for chi2r2
                                 coeffsStd = np.sqrt(rwst_curr.coeffs_cov['m2'][np.index_exp[:, :, index, index] + locIndex])
                             else:
                                 coeffsStd = np.zeros(coeffs.shape)
-                            for j1 in np.arange(rwst_curr.J - 1):
+                            for j1 in np.arange(rwst_curr.j_min, rwst_curr.J - 1):
                                 j2Vals = np.arange(j1 + 1, rwst_curr.J)
                                 if j1 != rwst_curr.J - 2:
                                     
                                     # Label design
                                     label = ""
                                     if j1 == 0:
                                         label = labels[rwst_index]
                                         if label != "" and locIndex != ():
                                             label += " - "
                                         if locIndex != ():
                                             label += str(locIndex)
                                     if label != "": legend = True # Need to display a legend
                                         
-                                    axs[pos].plot(j2Vals, coeffs[j1, j1 + 1:], label=label, color=color)
-                                    axs[pos].fill_between(j2Vals, coeffs[j1, j1 + 1:] - coeffsStd[j1, j1 + 1:], coeffs[j1, j1 + 1:] + coeffsStd[j1, j1 + 1:], alpha=0.2, color=color)
+                                    axs[pos].plot(j2Vals, coeffs[j1 - self.j_min, j1 - self.j_min + 1:], label=label, color=color)
+                                    axs[pos].fill_between(j2Vals, coeffs[j1 - self.j_min, j1 - self.j_min + 1:] - coeffsStd[j1 - self.j_min,j1 - self.j_min + 1:], \
+                                                          coeffs[j1 - self.j_min, j1 -self.j_min + 1:] + coeffsStd[j1 - self.j_min, j1 - self.j_min + 1:], alpha=0.2, color=color)
                                 else:
-                                    axs[pos].errorbar(j2Vals, coeffs[j1, j1 + 1:], fmt='.', yerr=coeffsStd[j1, j1 + 1:], color=color)
+                                    axs[pos].errorbar(j2Vals, coeffs[j1 - self.j_min, j1 - self.j_min + 1:], fmt='.', \
+                                                      yerr=coeffsStd[j1 -self.j_min, j1 - self.j_min + 1:], color=color)
                                     
                             color_cnt += 1
                         
                         axs[pos].set_xlabel("$j_2$")
                         if index != rwst_curr.model.layer2_nbparams:
                             axs[pos].set_ylabel(rwst_curr.model.layer2_pltparams[index][0])
                             if rwst_curr.model.layer2_pltparams[index][1]: # Readable radian ylabels?
@@ -474,56 +479,56 @@
         Returns
         -------
         None.
 
         """
         # Build a WST index
         wst_index = [[0, 0, 0, 0, 0]] # Layer 0
-        for j1 in range(self.J): # Layer 1
+        for j1 in range(self.j_min, self.J): # Layer 1
             for theta1 in range(self.L * (1 + cplx)):
                 wst_index.append([1, j1, theta1, 0, 0])
-        for j1 in range(self.J): # Layer 2
+        for j1 in range(self.j_min, self.J): # Layer 2
             for theta1 in range(self.L * (1 + cplx)):
                 for j2 in range(j1 + 1, self.J):
                     for theta2 in range(self.L):
                         wst_index.append([2, j1, theta1, j2, theta2])
         wst_index = np.array(wst_index).T
         
         # Get local shape and mask
         loc_shape = self.coeffs['m0'][0].shape
-        mask = ma.getmaskarray(self.coeffs['m0'][0])
+        mask = ma.getmaskarray(self.coeffs['m2'][0,0,0])
         valid_loc_index = [loc for loc in np.ndindex(loc_shape) if mask[loc] == False]
         
         # Initialization
         S = np.zeros((wst_index.shape[1],) + loc_shape)
         if mask.sum() != 0: # We have at least one masked value
             S = ma.MaskedArray(S)
             S[:, mask] = ma.masked
         
         # S0 coefficients
         S[0] = self.coeffs['m0'][0]
         
         # S1 coefficients
-        for j1 in range(self.J):
+        for j1 in range(self.j_min, self.J):
             filtering = np.logical_and(wst_index[0] == 1, wst_index[1] == j1)
             theta_vals = wst_index[2, filtering]
-            coeffs = self.coeffs['m1'][j1, :-1]
+            coeffs = self.coeffs['m1'][j1 - self.j_min, :-1]
             for loc_index in np.ndindex(loc_shape):
                 S[(filtering,) + loc_index] = self.model.layer1(theta_vals, *(coeffs[np.index_exp[:] + loc_index]))
             
         # S2 coefficients
-        for j1 in range(self.J):
+        for j1 in range(self.j_min, self.J):
             for j2 in range(j1 + 1, self.J):
                 filtering = np.logical_and(wst_index[1] == j1, wst_index[3] == j2)
                 theta_vals = (wst_index[2, filtering], wst_index[4, filtering])
-                coeffs = self.coeffs['m2'][j1, j2, :-1]
+                coeffs = self.coeffs['m2'][j1 - self.j_min, j2 - self.j_min, :-1]
                 for loc_index in valid_loc_index:
                     S[(filtering,) + loc_index] = self.model.layer2(theta_vals, *(coeffs[np.index_exp[:] + loc_index]))
                 
         # We create the WST object and fill out its attributes
-        wst = pw.WST(self.J, self.L, S, index=wst_index, cplx=cplx)
+        wst = pw.WST(self.J, self.L, S, index=wst_index, cplx=cplx, j_min=self.j_min)
         wst.normalized = self.wst_normalized
         wst.log2vals = self.wst_log2vals
         
         # TODO: add uncertainties to wst
         
         return wst
```

### Comparing `pywst-0.9/pywst/rwst_operator.py` & `pywst-1.0/pywst/rwst_operator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class RWSTOp:
     """
     Reduced Wavelet Scattering Transform (RWST) operator.
     """
     
-    def __init__(self, M, N, J, L=8, OS=0, cplx=False, model_cls=RWSTModel1, wst_op=None):
+    def __init__(self, M, N, J, L=8, OS=0, cplx=False, model_cls=RWSTModel1, wst_op=None, j_min=0):
         """
         Constructor.
         
         Parameters
         ----------
         M : int
             Height of the input images.
@@ -35,28 +35,30 @@
             Oversampling parameter. The default is 0.
         cplx : bool, optional
             Set it to true if the RWSTOp instance will ever apply to complex data. This would load in memory the whole set of bandpass filters. The default is False.
         model_cls : type, optional
             Class of the RWST model of the angular dependencies. The default is RWSTModel1.
         wst_op : WSTOp, optional
             WSTOp object with consistent parameters that avoids multiple filters loading.
+        j_min : type, optional
+            Minimum dyadic scale. The default is 0.
 
         Returns
         -------
         None.
         """
-        self.M, self.N, self.J, self.L, self.OS, self.cplx = M, N, J, L, OS, cplx
+        self.M, self.N, self.J, self.L, self.OS, self.cplx, self.j_min = M, N, J, L, OS, cplx, j_min
         if wst_op is None:
-            self.wst_op = WSTOp(M, N, J, L, OS, cplx)
+            self.wst_op = WSTOp(M, N, J, L, OS, cplx, j_min=j_min)
         else:
-            if wst_op.M == M and wst_op.N == N and wst_op.J == J and wst_op.L == L and wst_op.OS == OS and wst_op.cplx == cplx:
+            if wst_op.M == M and wst_op.N == N and wst_op.J == J and wst_op.L == L and wst_op.OS == OS and wst_op.cplx == cplx and wst_op.j_min == j_min:
                 self.wst_op = wst_op
             else:
                 warnings.warn("Warning! Loading WSTOp new instance because of wst_op inconsistencies.")
-                self.wst_op = WSTOp(M, N, J, L, OS, cplx)
+                self.wst_op = WSTOp(M, N, J, L, OS, cplx, j_min=j_min)
         self.model_cls = model_cls
     
     def apply(self, data, local=False, wst_average=False, crop=0.0, diag_cov=True):
         """
         Compute the RWST of input data or from a set of pre-computed WST coefficients.
         
         Input data can be either an image (2D array), or a batch of images (3D arrays, the first dimension is the image index) or a WST object.
@@ -88,33 +90,35 @@
 
         """
         # Check if data is made of images or is directly a WST object.
         if type(data) == WST:
             wst = data
             if wst.J != self.J:
                 raise Exception("Inconsistent J values between RWST operator and input WST coefficients.")
+            if wst.j_min != self.j_min:
+                raise Exception("Inconsistent j_min values between RWST operator and input WST coefficients.")
             if not wst.log2vals:
                 warnings.warn("Input WST coefficients must have logarithmic values. Auto-computation of logarithmic coefficients...")
                 wst.to_log2()
         else:
             wst = self.wst_op.apply(data, local, crop=crop)
             wst.to_log2()
             wst.normalize()
             if wst_average:
                 wst.average()
         
         # Get the shape of the local information (batch + local coefficients per map)
         loc_shape = wst.coeffs.shape[1:]
-        # Get a mask associated to S0 coefficient if any local coefficient turns out to be masked (we assume uniform mask along coefficient index axis).
-        mask = ma.getmaskarray(wst.coeffs[0])
+        # Get a mask associated to S2 coefficient if any local coefficient turns out to be masked (we assume uniform mask along coefficient index axis).
+        mask = ma.getmaskarray(wst.coeffs[-1])
         # Define an index of local positions that are not masked.
         validLocIndex = [loc for loc in np.ndindex(loc_shape) if mask[loc] == False]
         
         model = self.model_cls(self.L)
-        rwst = RWST(self.J, self.L, model, loc_shape=loc_shape)
+        rwst = RWST(self.J, self.L, model, loc_shape=loc_shape, j_min=self.j_min)
         
         # We keep relevant information on the WST object
         rwst.wst_log2vals = wst.log2vals
         rwst.wst_normalized = wst.normalized
         
         # Layer 0 coefficient
         coeffs, coeffsIndex = wst.get_coeffs(layer=0)
@@ -126,15 +130,15 @@
         # If coeffs_cov is None, we set absolute_sigma to False, otherwise it is True.
         # coeffs_cov absolute values are meaningful, this is why we need absolute_sigma=True,
         # but when coeffs_cov is None, the default value used by curve_fit is an identity matrix,
         # that is why we need absolute_sigma=False in this case.
         ##
 
         # Layer 1 coefficients
-        for j1 in range(self.J):
+        for j1 in range(self.j_min, self.J):
             coeffs, coeffsIndex = wst.get_coeffs(layer=1, j1=j1)
             coeffs_cov, _ = wst.get_coeffs_cov(layer=1, j1=j1, autoremove_offdiag=not diag_cov)
             if diag_cov and coeffs_cov is not None: # Only keep diagonal coefficients if required
                 coeffs_cov = np.diag(np.diag(coeffs_cov))
             theta1Vals = coeffsIndex[2]
             
             paramsOpt = np.zeros((model.layer1_nbparams,) + loc_shape)
@@ -150,15 +154,15 @@
                 if coeffs_cov is not None:
                     chi2r[locIndex] = x.T @ la.inv(coeffs_cov) @ x / (len(x) - model.layer1_nbparams)
                 else:
                     chi2r[locIndex] = x.T @ x / (len(x) - model.layer1_nbparams)
             rwst._set_coeffs(1, j1, paramsOpt, paramsCov, chi2r)
             
         # Layer 2 coefficients
-        for j1 in range(self.J):
+        for j1 in range(self.j_min, self.J):
             for j2 in range(j1 + 1, self.J):
                 coeffs, coeffsIndex = wst.get_coeffs(layer=2, j1=j1, j2=j2)
                 coeffs_cov, _ = wst.get_coeffs_cov(layer=2, j1=j1, j2=j2, autoremove_offdiag=not diag_cov)
                 if diag_cov and coeffs_cov is not None: # Only keep diagonal coefficients if required
                     coeffs_cov = np.diag(np.diag(coeffs_cov))
                 thetaVals = (coeffsIndex[2], coeffsIndex[4])
```

### Comparing `pywst-0.9/pywst/utils.py` & `pywst-1.0/pywst/utils.py`

 * *Files identical despite different names*

### Comparing `pywst-0.9/pywst/wst.py` & `pywst-1.0/pywst/wst.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class WST:
     """
     Wavelet Scattering Transform (WST) class contains the output of the WST of an image or a batch of images.
     This contains the corresponding coefficients and helps to handle and to plot these coefficients.
     """
     
-    def __init__(self, J, L, coeffs, index=None, cplx=False):
+    def __init__(self, J, L, coeffs, index=None, cplx=False, j_min=0):
         """
         Constructor.
 
         Parameters
         ----------
         J : int
             Number of dyadic scales.
@@ -27,33 +27,36 @@
             WST coefficients. 1D, 2D, 3D, 4D arrays are valid depending whether
             we have local coefficients or not, whether we are dealing with the WST
             of a batch of images or not.
         index : array, optional
             Index of the coefficients stored in coeffs. The default is None.
         cplx : bool, optional
             Are these coefficients computed from complex images? The default is False.
+        j_min : type, optional
+            Minimum dyadic scale. The default is 0.
 
         Raises
         ------
         Exception
             DESCRIPTION.
 
         Returns
         -------
         None.
 
         """
         self.J = J
         self.L = L
         self.cplx = cplx
+        self.j_min = j_min
         
         # Number of coefficients
         self.nb_m0 = 1
-        self.nb_m1 = J * L * (1 + cplx)
-        self.nb_m2 = J * (J - 1) * L * L * (1 + cplx) // 2
+        self.nb_m1 = (J - j_min) * L * (1 + cplx)
+        self.nb_m2 = (J - j_min) * (J - j_min - 1) * L * L * (1 + cplx) // 2
         
         self.coeffs = coeffs
         self.coeffs_cov = None
         
         # Check if we are dealing with a batch of images coefficients or not, and if we have local coefficients or not.
         if coeffs.ndim == 1:
             self.batch = False
@@ -71,38 +74,39 @@
             raise Exception("Bad input shape.")
         
         # Reordering and definition of the current index
         if index is not None:
             self.reorder(index)
         self.index = np.zeros((5, self.nb_m0 + self.nb_m1 + self.nb_m2))
         cnt = 1
-        for j1 in range(J):
+        for j1 in range(j_min, J):
             for theta1 in range(L * (1 + cplx)):
                 self.index[:, cnt] = [1, j1, theta1, 0, 0]
                 cnt += 1
-        for j1 in range(J):
+        for j1 in range(j_min, J):
             for theta1 in range(L * (1 + cplx)):
                 for j2 in range(j1 + 1, J):
                     for theta2 in range(L):
                         self.index[:, cnt] = [2, j1, theta1, j2, theta2]
                         cnt += 1
                         
         # Normalization initialization
         self.normalized = False
+        self.normalize_layer1 = None
         self.log2vals = False
         
         # Plot design parameters
         self._xticks, self._xticksMinor, self._xticklabels, self._xticklabelsMinor, self._tickAlignment = [], [], [], [], []
         cnt = 1
-        for j1 in range(J):
+        for j1 in range(j_min, J):
             self._xticks.append(cnt + L * (1 + cplx) // 2) # Tick at the middle
             self._xticklabels.append("$j_1 = " + str(j1) + "$")
             self._tickAlignment.append(0.0)
             cnt += L * (1 + cplx)
-        for j1 in range(J - 1):
+        for j1 in range(j_min, J - 1):
             for theta1 in range(L * (1 + cplx)):
                 for j2 in range(j1 + 1, J):
                     self._xticksMinor.append(cnt + L // 2)
                     self._xticklabelsMinor.append("$j_2 = " + str(j2) + "$")
                     self._tickAlignment.append(-0.1)
                     cnt += L
             self._xticks.append(cnt - L * L * (1 + cplx) * (J - j1 - 1) // 2)
@@ -152,15 +156,15 @@
 
         Returns
         -------
         filtering : array
             Boolean array for coefficients selection.
 
         """
-        filtering = np.ones(self.index.shape[1], np.bool)
+        filtering = np.ones(self.index.shape[1], bool)
         if layer is not None:
             filtering = np.logical_and(filtering, self.index[0] == layer)
         if j1 is not None:
             filtering = np.logical_and(filtering, self.index[1] == j1)
         if theta1 is not None:
             filtering = np.logical_and(filtering, self.index[2] == theta1)
         if j2 is not None:
@@ -201,127 +205,151 @@
         """
         Computation of logarithmic coefficients (binary logarithm).
         
         If coeffs_cov is not None, keep diagonal coefficients and divide them by (coeffs*log(2))^2 to estimate logarithmic errors at first order.
 
         Returns
         -------
-        None.
+        self
 
         """
         if not self.log2vals:
             # Compute the relevant covariance matrix, then compute log2 coefficients.
             if self.coeffs_cov is not None:
                 warnings.warn("Warning! The covariance matrix has already been computed with linear coefficients. We compute logarithmic errors from diagonal coefficients and discard off-diagonal coefficients.")
                 self.coeffs_cov = np.diag(np.diag(self.coeffs_cov)/(self.coeffs*np.log(2))**2)
-            self.coeffs = np.log2(self.coeffs)
+            self.coeffs = ma.log2(self.coeffs)
             self.log2vals = True
+        return self
             
     def to_linear(self):
         """
         Turn binary logarithmic coefficients into linear coefficients.
         
         If coeffs_cov is not None, keep diagonal coefficients and multiply them by (2^coeffs*log(2))^2 to estimate linear errors at first order.
 
         Returns
         -------
-        None.
+        self
 
         """
         if self.log2vals:
             # Compute linear coefficients, then compute the relevant covariance matrix.
             self.coeffs = 2 ** self.coeffs
             if self.coeffs_cov is not None:
                 warnings.warn("Warning! The covariance matrix has already been computed with logarithmic coefficients. We compute linear errors from diagonal coefficients and discard off-diagonal coefficients.")
                 self.coeffs_cov = np.diag(np.diag(self.coeffs_cov)*(self.coeffs*np.log(2))**2)
             self.log2vals = False
+        return self
         
-    def normalize(self):
+    def normalize(self, normalize_layer1=False):
         """
         Normalization of the coefficients.
         
         Layer 0 coefficients are left unchanged.
-        Layer 1 coefficients are normalized by layer 0 coefficients (locally if available):
+        Layer 1 coefficients are left unchanged if normalize_layer1 is False (default). Otherwise normalized by layer 0 coefficients (locally if available):
             
         .. math::
             
             \\bar{S}_1(j_1,\\theta_1) = S_1(j_1,\\theta_1)/S_0
             
         Layer 2 coefficients are normalized by the corresponding layer 1 coefficients (locally if available):
             
         .. math::
             
             \\bar{S}_2(j_1,\\theta_1,j_2,\\theta_2) = S_2(j_1,\\theta_1,j_2,\\theta_2)/S_1(j_1,\\theta_1)
 
+        Parameters
+        ----------
+        normalize_layer1 : bool, optional
+            Should layer 1 be also normalized? The default is False.
+
         Returns
         -------
-        None.
+        self
 
         """
         if self.coeffs_cov is not None:
             warnings.warn("Warning! The covariance matrix has been computed before the normalization and will not be updated.")
         
-        if not self.normalized:
+        # Case where no normalization was done or layer 1 normalization is asked to change
+        if (not self.normalized) or (self.normalize_layer1 == (not normalize_layer1)):
             coeffsCopy = self.coeffs.copy()
             cnt = 1
-            for j1 in range(self.J):
-                if self.log2vals:
-                    self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] -= coeffsCopy[:1, ...]
-                else:
-                    self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] /= coeffsCopy[:1, ...]
-                cnt += self.L * (1 + self.cplx)
-            for j1 in range(self.J):
-                for theta1 in range(self.L * (1 + self.cplx)):
-                    index = 1 + j1 * self.L * (1 + self.cplx) + theta1
+            # Layer 1
+            for j1 in range(self.j_min, self.J):
+                # Case where layer 1 was not normalized but is now asked to be normalized
+                if ((not self.normalized) or (not self.normalize_layer1)) and normalize_layer1:
                     if self.log2vals:
-                        self.coeffs[cnt:cnt + self.L * (self.J - j1 - 1), ...] -= coeffsCopy[index:index + 1, ...]
+                        self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] -= coeffsCopy[:1, ...]
                     else:
-                        self.coeffs[cnt:cnt + self.L * (self.J - j1 - 1), ...] /= coeffsCopy[index:index + 1, ...]
-                    cnt += self.L * (self.J - j1 - 1)
+                        self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] /= coeffsCopy[:1, ...]
+                # Case where normalization was done with layer 1 normalized and layer 1 is asked not to be normalized
+                elif self.normalized and self.normalize_layer1 and (not normalize_layer1):
+                    if self.log2vals:
+                        self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] += coeffsCopy[:1, ...]
+                    else:
+                        self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] *= coeffsCopy[:1, ...]
+                cnt += self.L * (1 + self.cplx)
+            # Layer 2
+            if (not self.normalized):
+                for j1 in range(self.j_min, self.J):
+                    for theta1 in range(self.L * (1 + self.cplx)):
+                        index = 1 + (j1 - self.j_min) * self.L * (1 + self.cplx) + theta1
+                        if self.log2vals:
+                            self.coeffs[cnt:cnt + self.L * (self.J - j1 - 1), ...] -= coeffsCopy[index:index + 1, ...]
+                        else:
+                            self.coeffs[cnt:cnt + self.L * (self.J - j1 - 1), ...] /= coeffsCopy[index:index + 1, ...]
+                        cnt += self.L * (self.J - j1 - 1)
             self.normalized = True
+            self.normalize_layer1 = normalize_layer1
+        return self
             
     def unnormalize(self):
         """
         Cancel the normalization of the coefficients. See normalize() method.
 
         Returns
         -------
-        None.
+        self
 
         """
         if self.coeffs_cov is not None:
             warnings.warn("Warning! The covariance matrix has been computed before the unnormalization and will not be updated.")
         
         if self.normalized:
             cnt = 1
-            for j1 in range(self.J):
-                if self.log2vals:
-                    self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] += self.coeffs[:1, ...]
-                else:
-                    self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] *= self.coeffs[:1, ...]
+            for j1 in range(self.j_min, self.J):
+                if self.normalize_layer1:
+                    if self.log2vals:
+                        self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] += self.coeffs[:1, ...]
+                    else:
+                        self.coeffs[cnt:cnt + self.L * (1 + self.cplx), ...] *= self.coeffs[:1, ...]
                 cnt += self.L * (1 + self.cplx)
-            for j1 in range(self.J):
+            for j1 in range(self.j_min, self.J):
                 for theta1 in range(self.L * (1 + self.cplx)):
-                    index = 1 + j1 * self.L * (1 + self.cplx) + theta1
+                    index = 1 + (j1 - self.j_min) * self.L * (1 + self.cplx) + theta1
                     if self.log2vals:
                         self.coeffs[cnt:cnt + self.L * (self.J - j1 - 1), ...] += self.coeffs[index:index + 1, ...]
                     else:
                         self.coeffs[cnt:cnt + self.L * (self.J - j1 - 1), ...] *= self.coeffs[index:index + 1, ...]
                     cnt += self.L * (self.J - j1 - 1)
             self.normalized = False
+            self.normalize_layer1 = None
+        return self
                 
     def average(self):
         """
         Computation of the mean coefficients and of the corresponding covariance matrix.
         
         This method needs batch data or local coefficients to be effective.
 
         Returns
         -------
-        None.
+        self
 
         """
         if self.batch or self.local: # We need multiple samples to average
             coeffsCopy = self.coeffs.copy()
             coeffsCopy = coeffsCopy.reshape((coeffsCopy.shape[0], -1))
             
             # How many valid samples do we have? (assumed to be the same for every coefficient)
@@ -335,14 +363,15 @@
             
             self.coeffs = coeffsCopy.mean(axis=-1)
             self.coeffs_cov = coeffs_cov
             self.coeffs_cov_nbsamples = samples # Keep in memory the number of samples used to compute the sample covariance matrix.
             
             self.batch = False
             self.local = False
+        return self
         
     def get_coeffs_cov(self, autoremove_offdiag=True, layer=None, j1=None, theta1=None, j2=None, theta2=None):
         """
         Return the covariance matrix corresponding to the selected coefficients.
 
         Parameters
         ----------
@@ -458,18 +487,18 @@
         axis.tick_params(axis='x', which='minor', direction='out', length=5)
         axis.tick_params(axis='x', which='major', bottom=False, top=False)
         axis.set_xlim(x.min() - 1, x.max() + 1)
         axis.margins(0.2)
         
         # Plot separators
         cnt = 1
-        for j1 in range(self.J):
+        for j1 in range(self.j_min, self.J):
             axis.axvline(cnt, color='black', alpha=0.5, linestyle='dashed')
             cnt += self.L * (1 + self.cplx)
-        for j1 in range(self.J):
+        for j1 in range(self.j_min, self.J):
             axis.axvline(cnt, color='black', alpha=0.5, linestyle='dashed')
             for theta1 in range(self.L * (1 + self.cplx)):
                 if theta1 >= 1:
                     axis.axvline(cnt, color='black', alpha=0.2, linestyle='dashed')
                 for j2 in range(j1 + 1, self.J):
                     if j2 > j1 + 1:
                         axis.axvline(cnt, color='black', alpha=0.1, linestyle=':')
@@ -504,15 +533,15 @@
                 
     def plot_compare(self, wst_list, layer=None, j1=None, title="WST", labels=[]):
         """
         Plot of the selected set of WST coefficients of the current object next to those from a given list of other WST or RWST objects.
         
         Default behaviour plots both layer 1 and layer 2 full set of coefficients.
         
-        Note that the current object and the objects of wst_list must be of consistent J, L and cplx parameters.
+        Note that the current object and the objects of wst_list must be of consistent J, L, cplx and j_min parameters.
 
         Parameters
         ----------
         wst_list : (R)WST or list of (R)WST
             WST object or RWST object, or list of multiple WST/RWST objects.
         layer : int, optional
             Layer of coefficients to plot (1 or 2). The default is None.
@@ -536,15 +565,15 @@
         else:
             wst_list_loc = wst_list.copy() # Local shallow copy
 
         for elt in wst_list_loc:
             if type(elt) != WST and type(elt) != RWST:
                 raise Exception("wst_list must be a WST object or a RWST object, or a list of RWST or/and WST objects!")
             else:
-                if self.J != elt.J or self.L != elt.L or (type(elt) == WST and self.cplx != elt.cplx):
+                if self.J != elt.J or self.L != elt.L or self.j_min != elt.j_min or (type(elt) == WST and self.cplx != elt.cplx):
                     raise Exception("Inconsistent (R)WST objects.")
                 if type(elt) == WST and (self.log2vals != elt.log2vals or self.normalized != elt.normalized):
                     raise warnings.warn("Warning! Input (R)WST objects have not consistent normalizations compared to the current WST object.")
             
         if layer is None:
             self.plot(layer=1, j1=j1, title=title)
             self.plot(layer=2, j1=j1, title=title)
@@ -566,26 +595,26 @@
             if layer == 1:
                 fig = plt.figure()
             elif layer == 2:
                 fig = plt.figure(figsize=(30, 5))
             ax = fig.add_subplot(1, 1, 1)
                 
             # ylabel design
-            ylabel = r"$" + self.log2vals * r"\log_2(" + self.normalized * r"\widebar{" + r"S" + self.normalized * r"}" + r"_" + str(layer) + self.log2vals * r")" + r"$"
+            ylabel = r"$" + self.log2vals * r"\log_2(" + self.normalized * (layer==2 or self.normalize_layer1==True) * r"\overline{" + r"S" + self.normalized * (layer==2 or self.normalize_layer1==True) * r"}" + r"_" + str(layer) + self.log2vals * r")" + r"$"
             
             # Plot
             for wst_index, wst_curr in enumerate(wst_list_loc):
                 
                 if type(wst_curr) == RWST:
                     wst_curr = wst_curr.to_wst(cplx=self.cplx) # If RWST object, convert it first to a WST object.
                 
                 # Get the shape of the local information (batch + local coefficients per map)
                 loc_shape = wst_curr.coeffs.shape[1:]
-                # Get a mask associated to S0 coefficient if any local coefficient turns out to be masked (we assume uniform mask along coefficient index axis).
-                mask = ma.getmaskarray(wst_curr.coeffs[0])
+                # Get a mask associated to S2 coefficient if any local coefficient turns out to be masked (we assume uniform mask along coefficient index axis).
+                mask = ma.getmaskarray(wst_curr.coeffs[-1])
                 # Define an index of local positions that are not masked.
                 validLocIndex = [loc for loc in np.ndindex(loc_shape) if mask[loc] == False]
                 
                 for locIndex in validLocIndex:
                     # Label design
                     label = labels[wst_index]
                     if label != "" and locIndex != ():
```

### Comparing `pywst-0.9/pywst/wst_operator.py` & `pywst-1.0/pywst/wst_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class WSTOp:
     """
     Wavelet Scattering Transform (WST) operator.
     """
     
-    def __init__(self, M, N, J, L=8, OS=0, cplx=False, lp_filter_cls=GaussianFilter, bp_filter_cls=MorletWavelet):
+    def __init__(self, M, N, J, L=8, OS=0, cplx=False, lp_filter_cls=GaussianFilter, bp_filter_cls=MorletWavelet, j_min=0):
         """
         Constructor.
         
         M and N must be proportional to 2^J.
 
         Parameters
         ----------
@@ -46,24 +46,26 @@
             Oversampling parameter. The default is 0.
         cplx : bool, optional
             Set it to true if the WSTOp instance will ever apply to complex data. This would load in memory the whole set of bandpass filters. The default is False.
         lp_filter_cls : type, optional
             Class corresponding to the low-pass filter. The default is GaussianFilter.
         bp_filter_cls : type, optional
             Class corresponding to the bandpass filter. The default is MorletWavelet.
+        j_min : type, optional
+            Minimum dyadic scale. The default is 0.
 
         Returns
         -------
         None.
 
         """
         if M % 2 ** J != 0 or N % 2 ** J != 0:
             raise Exception("Choose values for M and N that are proportional to 2^J.")
         
-        self.M, self.N, self.J, self.L, self.OS, self.cplx = M, N, J, L, OS, cplx
+        self.M, self.N, self.J, self.L, self.OS, self.cplx, self.j_min = M, N, J, L, OS, cplx, j_min
         self.load_filters(lp_filter_cls, bp_filter_cls)
         
     def load_filters(self, lp_filter_cls, bp_filter_cls):
         """
         Build the set of low pass and bandpass filters that are used for the transform.
 
         Parameters
@@ -83,36 +85,36 @@
         
         # Filter parameters
         gamma = 4 / self.L  # Aspect ratio
         sigma0 = 0.8        # Std of the envelope
         k0 = 3 * np.pi / 4  # Central wavenumber of the mother wavelet
         
         # Build psi filters
-        for j in range(self.J):
+        for j in range(self.j_min, self.J):
             # Parallel pre-build
             build_bp_para_loc = partial(_build_bp_para, bp_filter_cls=bp_filter_cls, M=self.M, N=self.N, j=j, L=self.L, gamma=gamma, sigma0=sigma0, k0=k0)
             nb_processes = os.cpu_count()
             work_list = np.array_split(np.arange(self.L), nb_processes)
-            pool = mp.get_context("spawn").Pool(processes=nb_processes) # "Spawn" context for macOS compatibility
+            pool = mp.Pool(processes=nb_processes)
             results = pool.map(build_bp_para_loc, work_list)
             bp_filters = []
             for i in range(len(results)):
                 bp_filters += results[i]
             pool.close()
             
             for theta in range(self.L):
                 self.psi[j, theta] = {}
                 w = bp_filters[theta]
                 wF = fft(w).real # The imaginary part is null for Morlet wavelets
-                for res in range(j + 1):
+                for res in range(max(j + 1, 1)):
                     self.psi[j, theta][res] = subsample_fourier(wF, 2 ** res, normalize=True, aa_filter=True)
             if self.cplx: # We also need rotations for theta in [pi, 2*pi)
                 for theta in range(self.L):
                     self.psi[j, theta + self.L] = {}
-                    for res in range(j + 1):
+                    for res in range(max(j + 1, 1)):
                         # Optimization trick for Morlet wavelets
                         self.psi[j, theta + self.L][res] = fft(np.conjugate(ifft(self.psi[j, theta][res]))).real
         
         # Build phi filters
         g = lp_filter_cls(self.M, self.N, self.J - 1, sigma0=sigma0).data
         gF = np.real(fft(g)) # The imaginary part is null for Gaussian filters
         for res in range(self.J):
@@ -148,14 +150,15 @@
         
         J = self.J
         L = self.L
         OS = self.OS
         phi = self.phi
         psi = self.psi
         locCplx = self.cplx
+        j_min = self.j_min
         
         # Check if we are dealing with a batch of images or not.
         if not (data.ndim == 2 or data.ndim == 3):
             raise Exception("Bad input shape.")
             
         # Check endianness for little-endian systems.
         # If input data is big-endian, we swap the byte order.
@@ -190,15 +193,15 @@
         if local:
             S.append(S0)
         else:
             S.append(S0.mean(axis=(-1, -2)))
         SIndex.append([0, 0, 0, 0, 0])
     
         # First layer
-        for j1 in range(J):
+        for j1 in range(j_min, J):
             for theta1 in range((locCplx + 1) * L): # Note the trick to produce 2 when locCplx == True, and 1 otherwise
                 U1 = subsample_fourier(U0 * psi[j1, theta1][resU0], 2 ** max(j1 - resU0 - OS, 0))
                 U1 = fft(modulus(ifft(U1)))
                 resU1 = resU0 + max(j1 - resU0 - OS, 0)
                 
                 if local:
                     S1 = ifft(subsample_fourier(U1 * phi[resU1], 2 ** (max(J - resU1 - OS, 0)))).real
@@ -233,8 +236,8 @@
                     if i < int(crop * 2 ** OS) or i > self.M // 2 ** (J - OS) - int(crop * 2 ** OS) \
                        or j < int(crop * 2 ** OS) or j > self.N // 2 ** (J - OS) - int(crop * 2 ** OS):
                         mask[..., i, j] = True
             if np.sum(~mask) == 0:
                 raise Exception("No valid data remains after cropping.")
             S = ma.MaskedArray(S, mask=mask) # We create a numpy masked array to mask the cropped coefficients.
                         
-        return WST(J, L, S, index=np.array(SIndex).T, cplx=locCplx)
+        return WST(J, L, S, index=np.array(SIndex).T, cplx=locCplx, j_min=j_min)
```

### Comparing `pywst-0.9/pywst.egg-info/PKG-INFO` & `pywst-1.0/pywst.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 Metadata-Version: 2.1
 Name: pywst
-Version: 0.9
+Version: 1.0
 Summary: WST and RWST analyses tools for astrophysical data.
 Home-page: https://github.com/bregaldo/pywst
 Author: Bruno Régaldo-Saint Blancard
 Author-email: bruno.regaldo@phys.ens.fr
-License: UNKNOWN
-Description: # PyWST : WST and RWST for astrophysics
-        
-        PyWST is a public Python package designed to perform statistical analyses of two-dimensional data with the Wavelet Scattering Transform (WST) and the Reduced Wavelet Scattering Transform (RWST).
-        
-        The WST/RWST give you convenient sets of coefficients that describe your non-Gaussian data in a comprehensive way.
-        
-        Install PyWST and check out our [Jupyter notebook tutorial](examples/tutorial.ipynb) in the *examples/* folder.
-        
-        If you use this package, please cite the following paper:
-        
-        B. Regaldo-Saint Blancard, F. Levrier, E. Allys, E. Bellomi, F. Boulanger (2020). Statistical description of dust polarized emission from the diffuse interstellar medium - A WST/RWST approach. arXiv preprint arXiv:????
-        
-        ## Install/Uninstall
-        
-        ### Standard installation (from the Python Package Index)
-        
-        Type in a console:
-        
-        ```
-        pip install pywst
-        ```
-        
-        ### Install from source
-        
-        Clone the repository and type from the main directory:
-        
-        ```
-        pip install -r requirements.txt
-        pip install .
-        ```
-        
-        ### Uninstall
-        
-        ```
-        pip uninstall pywst
-        ```
-        
-        ## Changelog
-        
-        ### 0.9
-        
-        * First public version.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# PyWST : WST and RWST for astrophysics
+
+PyWST is a public Python package designed to perform statistical analyses of two-dimensional data with the Wavelet Scattering Transform (WST) and the Reduced Wavelet Scattering Transform (RWST).
+
+The WST/RWST give you convenient sets of coefficients that describe your non-Gaussian data in a comprehensive way.
+
+Install PyWST and check out our [Jupyter notebook tutorial](examples/tutorial.ipynb) in the *examples/* folder.
+
+If you use this package, please cite the following paper:
+
+B. Regaldo-Saint Blancard, F. Levrier, E. Allys, E. Bellomi, F. Boulanger (2020). Statistical description of dust polarized emission from the diffuse interstellar medium - A RWST approach. arXiv preprint [arXiv:2007.08242](https://arxiv.org/abs/2007.08242)
+
+*Note:* For GPU-accelerated WST computations, take a look at [kymatio](https://github.com/kymatio/kymatio) (on which part of this code is based).
+
+## Install/Uninstall
+
+### Standard installation (from the Python Package Index)
+
+Type in a console:
+
+```
+pip install pywst
+```
+
+### Install from source
+
+Clone the repository and type from the main directory:
+
+```
+pip install -r requirements.txt
+pip install .
+```
+
+### Uninstall
+
+```
+pip uninstall pywst
+```
+
+## Changelog
+
+### 1.0
+
+* Minor updates.
+
+### 0.9
+
+* First public version.
```

### Comparing `pywst-0.9/setup.py` & `pywst-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pywst",
-    version="0.9",
+    version="1.0",
     author="Bruno Régaldo-Saint Blancard",
     author_email="bruno.regaldo@phys.ens.fr",
     description="WST and RWST analyses tools for astrophysical data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bregaldo/pywst",
     packages=setuptools.find_packages(),
```

