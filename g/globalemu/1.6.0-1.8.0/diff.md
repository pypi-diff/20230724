# Comparing `tmp/globalemu-1.6.0.tar.gz` & `tmp/globalemu-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalemu-1.6.0.tar", last modified: Fri Apr 21 11:54:26 2023, max compression
+gzip compressed data, was "globalemu-1.8.0.tar", last modified: Mon Jul 24 15:03:48 2023, max compression
```

## Comparing `globalemu-1.6.0.tar` & `globalemu-1.8.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.269770 globalemu-1.6.0/
--rw-r--r--   0 harry      (501) staff       (20)     1082 2022-09-02 15:51:21.000000 globalemu-1.6.0/LICENSE
--rw-r--r--   0 harry      (501) staff       (20)       25 2022-09-02 15:51:21.000000 globalemu-1.6.0/MANIFEST.in
--rw-r--r--   0 harry      (501) staff       (20)    10082 2023-04-21 11:54:26.269607 globalemu-1.6.0/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)     9357 2023-04-21 11:53:48.000000 globalemu-1.6.0/README.rst
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.267839 globalemu-1.6.0/globalemu/
--rw-r--r--   0 harry      (501) staff       (20)        0 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/__init__.py
--rw-r--r--   0 harry      (501) staff       (20)     2331 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/cmSim.py
--rw-r--r--   0 harry      (501) staff       (20)     1854 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/downloads.py
--rw-r--r--   0 harry      (501) staff       (20)    10537 2023-04-21 11:53:48.000000 globalemu-1.6.0/globalemu/eval.py
--rw-r--r--   0 harry      (501) staff       (20)     4689 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/gui_config.py
--rw-r--r--   0 harry      (501) staff       (20)      957 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/losses.py
--rw-r--r--   0 harry      (501) staff       (20)     1594 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/models.py
--rw-r--r--   0 harry      (501) staff       (20)    14428 2023-04-21 11:53:48.000000 globalemu-1.6.0/globalemu/network.py
--rw-r--r--   0 harry      (501) staff       (20)     8446 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/plotter.py
--rw-r--r--   0 harry      (501) staff       (20)    12993 2023-04-21 11:53:48.000000 globalemu-1.6.0/globalemu/preprocess.py
--rw-r--r--   0 harry      (501) staff       (20)     1626 2022-09-02 15:51:21.000000 globalemu-1.6.0/globalemu/resample.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.268452 globalemu-1.6.0/globalemu.egg-info/
--rw-r--r--   0 harry      (501) staff       (20)    10082 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)      628 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/SOURCES.txt
--rw-r--r--   0 harry      (501) staff       (20)        1 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/dependency_links.txt
--rw-r--r--   0 harry      (501) staff       (20)       83 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/requires.txt
--rw-r--r--   0 harry      (501) staff       (20)       10 2023-04-21 11:54:26.000000 globalemu-1.6.0/globalemu.egg-info/top_level.txt
--rw-r--r--   0 harry      (501) staff       (20)       42 2023-04-21 08:08:31.000000 globalemu-1.6.0/requirements.txt
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.268569 globalemu-1.6.0/scripts/
--rw-r--r--   0 harry      (501) staff       (20)     4699 2022-09-02 15:51:21.000000 globalemu-1.6.0/scripts/globalemu
--rw-r--r--   0 harry      (501) staff       (20)       38 2023-04-21 11:54:26.269806 globalemu-1.6.0/setup.cfg
--rw-r--r--   0 harry      (501) staff       (20)     1285 2023-04-21 11:53:48.000000 globalemu-1.6.0/setup.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-04-21 11:54:26.269449 globalemu-1.6.0/tests/
--rw-r--r--   0 harry      (501) staff       (20)      408 2022-09-02 15:51:21.000000 globalemu-1.6.0/tests/test_cmsim.py
--rw-r--r--   0 harry      (501) staff       (20)     1315 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_download.py
--rw-r--r--   0 harry      (501) staff       (20)     2102 2023-04-21 10:57:50.000000 globalemu-1.6.0/tests/test_eval.py
--rw-r--r--   0 harry      (501) staff       (20)     1863 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_gui_config.py
--rw-r--r--   0 harry      (501) staff       (20)     2301 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_network.py
--rw-r--r--   0 harry      (501) staff       (20)     2917 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_plotter.py
--rw-r--r--   0 harry      (501) staff       (20)     2363 2023-04-21 11:53:48.000000 globalemu-1.6.0/tests/test_preprocess.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-07-24 15:03:48.505432 globalemu-1.8.0/
+-rw-r--r--   0 harry      (501) staff       (20)     1082 2022-09-02 15:51:21.000000 globalemu-1.8.0/LICENSE
+-rw-r--r--   0 harry      (501) staff       (20)       25 2022-09-02 15:51:21.000000 globalemu-1.8.0/MANIFEST.in
+-rw-r--r--   0 harry      (501) staff       (20)    10344 2023-07-24 15:03:48.505271 globalemu-1.8.0/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)     9619 2023-07-24 15:01:50.000000 globalemu-1.8.0/README.rst
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-07-24 15:03:48.503107 globalemu-1.8.0/globalemu/
+-rw-r--r--   0 harry      (501) staff       (20)        0 2022-09-02 15:51:21.000000 globalemu-1.8.0/globalemu/__init__.py
+-rw-r--r--   0 harry      (501) staff       (20)     2331 2022-09-02 15:51:21.000000 globalemu-1.8.0/globalemu/cmSim.py
+-rw-r--r--   0 harry      (501) staff       (20)     1854 2022-09-02 15:51:21.000000 globalemu-1.8.0/globalemu/downloads.py
+-rw-r--r--   0 harry      (501) staff       (20)    10537 2023-04-21 11:53:48.000000 globalemu-1.8.0/globalemu/eval.py
+-rw-r--r--   0 harry      (501) staff       (20)     4689 2022-09-02 15:51:21.000000 globalemu-1.8.0/globalemu/gui_config.py
+-rw-r--r--   0 harry      (501) staff       (20)      957 2022-09-02 15:51:21.000000 globalemu-1.8.0/globalemu/losses.py
+-rw-r--r--   0 harry      (501) staff       (20)     1594 2022-09-02 15:51:21.000000 globalemu-1.8.0/globalemu/models.py
+-rw-r--r--   0 harry      (501) staff       (20)    14771 2023-06-21 09:26:00.000000 globalemu-1.8.0/globalemu/network.py
+-rw-r--r--   0 harry      (501) staff       (20)     8446 2022-09-02 15:51:21.000000 globalemu-1.8.0/globalemu/plotter.py
+-rw-r--r--   0 harry      (501) staff       (20)    12993 2023-05-18 10:28:57.000000 globalemu-1.8.0/globalemu/preprocess.py
+-rw-r--r--   0 harry      (501) staff       (20)     1626 2022-09-02 15:51:21.000000 globalemu-1.8.0/globalemu/resample.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-07-24 15:03:48.503706 globalemu-1.8.0/globalemu.egg-info/
+-rw-r--r--   0 harry      (501) staff       (20)    10344 2023-07-24 15:03:48.000000 globalemu-1.8.0/globalemu.egg-info/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)      628 2023-07-24 15:03:48.000000 globalemu-1.8.0/globalemu.egg-info/SOURCES.txt
+-rw-r--r--   0 harry      (501) staff       (20)        1 2023-07-24 15:03:48.000000 globalemu-1.8.0/globalemu.egg-info/dependency_links.txt
+-rw-r--r--   0 harry      (501) staff       (20)      168 2023-07-24 15:03:48.000000 globalemu-1.8.0/globalemu.egg-info/requires.txt
+-rw-r--r--   0 harry      (501) staff       (20)       10 2023-07-24 15:03:48.000000 globalemu-1.8.0/globalemu.egg-info/top_level.txt
+-rw-r--r--   0 harry      (501) staff       (20)      111 2023-07-24 15:01:50.000000 globalemu-1.8.0/requirements.txt
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-07-24 15:03:48.503800 globalemu-1.8.0/scripts/
+-rw-r--r--   0 harry      (501) staff       (20)     4699 2022-09-02 15:51:21.000000 globalemu-1.8.0/scripts/globalemu
+-rw-r--r--   0 harry      (501) staff       (20)       38 2023-07-24 15:03:48.505465 globalemu-1.8.0/setup.cfg
+-rw-r--r--   0 harry      (501) staff       (20)     1685 2023-07-24 15:01:50.000000 globalemu-1.8.0/setup.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-07-24 15:03:48.505077 globalemu-1.8.0/tests/
+-rw-r--r--   0 harry      (501) staff       (20)      408 2022-09-02 15:51:21.000000 globalemu-1.8.0/tests/test_cmsim.py
+-rw-r--r--   0 harry      (501) staff       (20)     1315 2023-04-21 11:53:48.000000 globalemu-1.8.0/tests/test_download.py
+-rw-r--r--   0 harry      (501) staff       (20)     2102 2023-04-21 10:57:50.000000 globalemu-1.8.0/tests/test_eval.py
+-rw-r--r--   0 harry      (501) staff       (20)     1863 2023-04-21 11:53:48.000000 globalemu-1.8.0/tests/test_gui_config.py
+-rw-r--r--   0 harry      (501) staff       (20)     2301 2023-04-21 11:53:48.000000 globalemu-1.8.0/tests/test_network.py
+-rw-r--r--   0 harry      (501) staff       (20)     2917 2023-04-21 11:53:48.000000 globalemu-1.8.0/tests/test_plotter.py
+-rw-r--r--   0 harry      (501) staff       (20)     2363 2023-04-21 11:53:48.000000 globalemu-1.8.0/tests/test_preprocess.py
```

### Comparing `globalemu-1.6.0/LICENSE` & `globalemu-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/PKG-INFO` & `globalemu-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalemu
-Version: 1.6.0
+Version: 1.8.0
 Summary: globalemu: Robust and Fast Global 21-cm Signal Emulation
 Home-page: https://github.com/htjb/globalemu
 Author: Harry T. J. Bevins
 Author-email: htjb2@cam.ac.uk
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -23,15 +23,15 @@
 ========================================================
 
 Introduction
 ------------
 
 :globalemu: Robust Global 21-cm Signal Emulation
 :Author: Harry Thomas Jones Bevins
-:Version: 1.6.0
+:Version: 1.8.0
 :Homepage: https://github.com/htjb/globalemu
 :Documentation: https://globalemu.readthedocs.io/
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/htjb/globalemu/master?filepath=notebooks%2F
 .. image:: https://readthedocs.org/projects/globalemu/badge/?version=latest
  :target: https://globalemu.readthedocs.io/en/latest/?badge=latest
@@ -266,22 +266,28 @@
   signal from the cosmic dawn and epoch of reionisation.” (2021). arXiv:2104.04336
 
 Below is the bibtex,
 
 .. code:: bibtex
 
   @article{Bevins2021,
-    title = {{GLOBALEMU}: {A} novel and robust approach for emulating the sky-averaged 21-cm signal from the cosmic dawn and epoch of reionisation},
-    url = {http://arxiv.org/abs/2104.04336},
-    urldate = {2021-04-12},
-    journal = {arXiv:2104.04336 [astro-ph]},
-    author = {Bevins, H. T. J. and Handley, W. J. and Fialkov, A. and Acedo, E. de Lera and Javid, K.},
-    month = apr,
-    year = {2021},
-    note = {arXiv: 2104.04336}
+        author = {{Bevins}, H.~T.~J. and {Handley}, W.~J. and {Fialkov}, A. and {de Lera Acedo}, E. and {Javid}, K.},
+          title = "{GLOBALEMU: a novel and robust approach for emulating the sky-averaged 21-cm signal from the cosmic dawn and epoch of reionization}",
+        journal = {\mnras},
+          year = 2021,
+          month = dec,
+        volume = {508},
+        number = {2},
+          pages = {2923-2936},
+            doi = {10.1093/mnras/stab2737},
+  archivePrefix = {arXiv},
+        eprint = {2104.04336},
+  primaryClass = {astro-ph.CO},
+        adsurl = {https://ui.adsabs.harvard.edu/abs/2021MNRAS.508.2923B},
+        adsnote = {Provided by the SAO/NASA Astrophysics Data System}
   }
 
 Requirements
 ------------
 
 To run the code you will need to following additional packages:
```

### Comparing `globalemu-1.6.0/README.rst` & `globalemu-1.8.0/globalemu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,37 @@
+Metadata-Version: 2.1
+Name: globalemu
+Version: 1.8.0
+Summary: globalemu: Robust and Fast Global 21-cm Signal Emulation
+Home-page: https://github.com/htjb/globalemu
+Author: Harry T. J. Bevins
+Author-email: htjb2@cam.ac.uk
+License: MIT
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: Topic :: Scientific/Engineering :: Physics
+Provides-Extra: docs
+License-File: LICENSE
+
 ========================================================
 globalemu: Robust and Fast Global 21-cm Signal Emulation
 ========================================================
 
 Introduction
 ------------
 
 :globalemu: Robust Global 21-cm Signal Emulation
 :Author: Harry Thomas Jones Bevins
-:Version: 1.6.0
+:Version: 1.8.0
 :Homepage: https://github.com/htjb/globalemu
 :Documentation: https://globalemu.readthedocs.io/
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/htjb/globalemu/master?filepath=notebooks%2F
 .. image:: https://readthedocs.org/projects/globalemu/badge/?version=latest
  :target: https://globalemu.readthedocs.io/en/latest/?badge=latest
@@ -246,22 +266,28 @@
   signal from the cosmic dawn and epoch of reionisation.” (2021). arXiv:2104.04336
 
 Below is the bibtex,
 
 .. code:: bibtex
 
   @article{Bevins2021,
-    title = {{GLOBALEMU}: {A} novel and robust approach for emulating the sky-averaged 21-cm signal from the cosmic dawn and epoch of reionisation},
-    url = {http://arxiv.org/abs/2104.04336},
-    urldate = {2021-04-12},
-    journal = {arXiv:2104.04336 [astro-ph]},
-    author = {Bevins, H. T. J. and Handley, W. J. and Fialkov, A. and Acedo, E. de Lera and Javid, K.},
-    month = apr,
-    year = {2021},
-    note = {arXiv: 2104.04336}
+        author = {{Bevins}, H.~T.~J. and {Handley}, W.~J. and {Fialkov}, A. and {de Lera Acedo}, E. and {Javid}, K.},
+          title = "{GLOBALEMU: a novel and robust approach for emulating the sky-averaged 21-cm signal from the cosmic dawn and epoch of reionization}",
+        journal = {\mnras},
+          year = 2021,
+          month = dec,
+        volume = {508},
+        number = {2},
+          pages = {2923-2936},
+            doi = {10.1093/mnras/stab2737},
+  archivePrefix = {arXiv},
+        eprint = {2104.04336},
+  primaryClass = {astro-ph.CO},
+        adsurl = {https://ui.adsabs.harvard.edu/abs/2021MNRAS.508.2923B},
+        adsnote = {Provided by the SAO/NASA Astrophysics Data System}
   }
 
 Requirements
 ------------
 
 To run the code you will need to following additional packages:
```

### Comparing `globalemu-1.6.0/globalemu/cmSim.py` & `globalemu-1.8.0/globalemu/cmSim.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu/downloads.py` & `globalemu-1.8.0/globalemu/downloads.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu/eval.py` & `globalemu-1.8.0/globalemu/eval.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu/gui_config.py` & `globalemu-1.8.0/globalemu/gui_config.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu/losses.py` & `globalemu-1.8.0/globalemu/losses.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu/models.py` & `globalemu-1.8.0/globalemu/models.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu/network.py` & `globalemu-1.8.0/globalemu/network.py`

 * *Files 14% similar despite different names*

```diff
@@ -271,14 +271,16 @@
             test_loss_results = list(
                 np.loadtxt(self.base_dir + 'test_loss_history.txt'))
         else:
             train_loss_results = []
             test_loss_results = []
         train_rmse_results = []
         num_epochs = self.epochs
+        c = 0
+        minimum_model = None
         for epoch in range(num_epochs):
             s = time.time()
             epoch_loss_avg = tf.keras.metrics.Mean()
             epoch_rmse_avg = tf.keras.metrics.Mean()
 
             for x, y in train_dataset:
                 loss_values, rmse, grads = grad(model, x, y)
@@ -294,32 +296,41 @@
             test_loss, _ = loss(model, test_data, test_labels, training=False)
             test_loss_results.append(test_loss)
 
             print(
                 'Epoch: {:03d}, Loss: {:.5f}, Test Loss: {:.5f},'
                 .format(epoch, epoch_loss_avg.result(), test_loss_results[-1])
                 + 'RMSE: {:.5f}, Time: {:.3f}'
-                .format(epoch_rmse_avg.result(), e-s))
+                .format(epoch_rmse_avg.result(), e-s), flush=True)
 
             if self.early_stop:
-                if len(test_loss_results) > 20:
-                    delta = 2*np.abs(test_loss_results[-21] -
-                                     test_loss_results[-1]) / \
-                                     (test_loss_results[-21] +
-                                      test_loss_results[-1])
-
-                    if delta*100 < 1e-2:
-                        print('Early Stopped: {:.5f}'.format(delta.numpy()*100)
-                              + ' < 1e-2')
-                        print('Epochs used = ' + str(len(test_loss_results)))
+                c += 1
+                if epoch == 0:
+                    minimum_loss = test_loss_results[-1]
+                    minimum_epoch = epoch
+                    minimum_model = None
+                else:
+                    if test_loss_results[-1] < minimum_loss:
+                        minimum_loss = test_loss_results[-1]
+                        minimum_epoch = epoch
+                        minimum_model = model
+                        c = 0
+                if minimum_model:
+                    if c == round((self.epochs/100)*2):
+                        print('Early stopped. Minimum at = ' +
+                              str(minimum_epoch) +
+                              ' Epochs used = ' + str(epoch))
                         break
 
             if (epoch + 1) % 10 == 0:
                 model.save(self.base_dir + 'model.h5')
                 np.savetxt(
                     self.base_dir + 'loss_history.txt', train_loss_results)
                 np.savetxt(
                     self.base_dir + 'test_loss_history.txt', test_loss_results)
 
-        model.save(self.base_dir + 'model.h5')
+        if minimum_model:
+            minimum_model.save(self.base_dir + 'model.h5')
+        else:
+            model.save(self.base_dir + 'model.h5')
         np.savetxt(self.base_dir + 'loss_history.txt', train_loss_results)
         np.savetxt(self.base_dir + 'test_loss_history.txt', test_loss_results)
```

### Comparing `globalemu-1.6.0/globalemu/plotter.py` & `globalemu-1.8.0/globalemu/plotter.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu/preprocess.py` & `globalemu-1.8.0/globalemu/preprocess.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu/resample.py` & `globalemu-1.8.0/globalemu/resample.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/globalemu.egg-info/PKG-INFO` & `globalemu-1.8.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,17 @@
-Metadata-Version: 2.1
-Name: globalemu
-Version: 1.6.0
-Summary: globalemu: Robust and Fast Global 21-cm Signal Emulation
-Home-page: https://github.com/htjb/globalemu
-Author: Harry T. J. Bevins
-Author-email: htjb2@cam.ac.uk
-License: MIT
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Classifier: Topic :: Scientific/Engineering :: Physics
-Provides-Extra: docs
-License-File: LICENSE
-
 ========================================================
 globalemu: Robust and Fast Global 21-cm Signal Emulation
 ========================================================
 
 Introduction
 ------------
 
 :globalemu: Robust Global 21-cm Signal Emulation
 :Author: Harry Thomas Jones Bevins
-:Version: 1.6.0
+:Version: 1.8.0
 :Homepage: https://github.com/htjb/globalemu
 :Documentation: https://globalemu.readthedocs.io/
 
 .. image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/htjb/globalemu/master?filepath=notebooks%2F
 .. image:: https://readthedocs.org/projects/globalemu/badge/?version=latest
  :target: https://globalemu.readthedocs.io/en/latest/?badge=latest
@@ -266,22 +246,28 @@
   signal from the cosmic dawn and epoch of reionisation.” (2021). arXiv:2104.04336
 
 Below is the bibtex,
 
 .. code:: bibtex
 
   @article{Bevins2021,
-    title = {{GLOBALEMU}: {A} novel and robust approach for emulating the sky-averaged 21-cm signal from the cosmic dawn and epoch of reionisation},
-    url = {http://arxiv.org/abs/2104.04336},
-    urldate = {2021-04-12},
-    journal = {arXiv:2104.04336 [astro-ph]},
-    author = {Bevins, H. T. J. and Handley, W. J. and Fialkov, A. and Acedo, E. de Lera and Javid, K.},
-    month = apr,
-    year = {2021},
-    note = {arXiv: 2104.04336}
+        author = {{Bevins}, H.~T.~J. and {Handley}, W.~J. and {Fialkov}, A. and {de Lera Acedo}, E. and {Javid}, K.},
+          title = "{GLOBALEMU: a novel and robust approach for emulating the sky-averaged 21-cm signal from the cosmic dawn and epoch of reionization}",
+        journal = {\mnras},
+          year = 2021,
+          month = dec,
+        volume = {508},
+        number = {2},
+          pages = {2923-2936},
+            doi = {10.1093/mnras/stab2737},
+  archivePrefix = {arXiv},
+        eprint = {2104.04336},
+  primaryClass = {astro-ph.CO},
+        adsurl = {https://ui.adsabs.harvard.edu/abs/2021MNRAS.508.2923B},
+        adsnote = {Provided by the SAO/NASA Astrophysics Data System}
   }
 
 Requirements
 ------------
 
 To run the code you will need to following additional packages:
```

### Comparing `globalemu-1.6.0/globalemu.egg-info/SOURCES.txt` & `globalemu-1.8.0/globalemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/scripts/globalemu` & `globalemu-1.8.0/scripts/globalemu`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/setup.py` & `globalemu-1.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 from setuptools import setup, find_packages
 
 def readme(short=False):
-    with open('README.rst') as f:
+    with open('README.rst', encoding='utf-8') as f:
         if short:
             return f.readlines()[1].strip()
         else:
             return f.read()
 
+def get_version_from_readme() -> str:
+    """Get current version of package from README.rst"""
+    readme_text = readme()
+    for line in readme_text.splitlines():
+        if ":Version:" in line:
+            current_version = line.split(":")[-1].strip()
+            return current_version
+    raise ValueError("Could not find version in README.rst")
+
 setup(
     name='globalemu',
-    version='1.6.0',
+    version=get_version_from_readme(),
     description='globalemu: Robust and Fast Global 21-cm Signal Emulation',
     long_description=readme(),
     author='Harry T. J. Bevins',
     author_email='htjb2@cam.ac.uk',
     url='https://github.com/htjb/globalemu',
     packages=find_packages(),
     install_requires=open('requirements.txt').read().splitlines(),
     license='MIT',
     scripts=['scripts/globalemu'],
     extras_require={
-          'docs': ['sphinx', 'sphinx_rtd_theme', 'numpydoc'],
+          'docs': ['sphinx', 'sphinx_rtd_theme', 'numpydoc', 'packaging'],
           },
     tests_require=['pytest'],
     classifiers=[
                'Intended Audience :: Science/Research',
                'Natural Language :: English',
                'License :: OSI Approved :: MIT License',
                'Programming Language :: Python :: 3.6',
```

### Comparing `globalemu-1.6.0/tests/test_download.py` & `globalemu-1.8.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/tests/test_eval.py` & `globalemu-1.8.0/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/tests/test_gui_config.py` & `globalemu-1.8.0/tests/test_gui_config.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/tests/test_network.py` & `globalemu-1.8.0/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/tests/test_plotter.py` & `globalemu-1.8.0/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `globalemu-1.6.0/tests/test_preprocess.py` & `globalemu-1.8.0/tests/test_preprocess.py`

 * *Files identical despite different names*

