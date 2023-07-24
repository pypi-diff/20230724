# Comparing `tmp/PDStoolkit-0.0.1.tar.gz` & `tmp/PDStoolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDStoolkit-0.0.1.tar", last modified: Sun May 15 13:36:02 2022, max compression
+gzip compressed data, was "PDStoolkit-0.0.2.tar", last modified: Mon Jul 24 20:54:03 2023, max compression
```

## Comparing `PDStoolkit-0.0.1.tar` & `PDStoolkit-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-05-15 13:36:02.860983 PDStoolkit-0.0.1/
--rw-rw-rw-   0        0        0     1091 2022-05-13 18:06:55.000000 PDStoolkit-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4650 2022-05-15 13:36:02.860983 PDStoolkit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4007 2022-05-14 21:59:01.000000 PDStoolkit-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2022-05-13 17:51:27.000000 PDStoolkit-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      782 2022-05-15 13:36:02.861984 PDStoolkit-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-05-15 13:36:02.835984 PDStoolkit-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-05-15 13:36:02.850983 PDStoolkit-0.0.1/src/PDStoolkit/
--rw-rw-rw-   0        0        0    14264 2022-05-14 20:46:54.000000 PDStoolkit-0.0.1/src/PDStoolkit/PDS_PCA.py
--rw-rw-rw-   0        0        0    16285 2022-05-11 22:00:28.000000 PDStoolkit-0.0.1/src/PDStoolkit/PDS_PLS.py
--rw-rw-rw-   0        0        0      118 2022-05-14 20:12:21.000000 PDStoolkit-0.0.1/src/PDStoolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-15 13:36:02.858984 PDStoolkit-0.0.1/src/PDStoolkit.egg-info/
--rw-rw-rw-   0        0        0     4650 2022-05-15 13:36:02.000000 PDStoolkit-0.0.1/src/PDStoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2022-05-15 13:36:02.000000 PDStoolkit-0.0.1/src/PDStoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-15 13:36:02.000000 PDStoolkit-0.0.1/src/PDStoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-05-15 13:36:02.000000 PDStoolkit-0.0.1/src/PDStoolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 20:54:03.349959 PDStoolkit-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2022-05-13 18:06:55.000000 PDStoolkit-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6735 2023-07-24 20:54:03.350948 PDStoolkit-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6092 2023-07-24 20:48:32.000000 PDStoolkit-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2022-05-13 17:51:27.000000 PDStoolkit-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      782 2023-07-24 20:54:03.353948 PDStoolkit-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 20:54:03.310963 PDStoolkit-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 20:54:03.338948 PDStoolkit-0.0.2/src/PDStoolkit/
+-rw-rw-rw-   0        0        0    17321 2023-07-18 18:21:08.000000 PDStoolkit-0.0.2/src/PDStoolkit/PDS_CVA.py
+-rw-rw-rw-   0        0        0    18481 2023-07-14 20:56:49.000000 PDStoolkit-0.0.2/src/PDStoolkit/PDS_DPCA.py
+-rw-rw-rw-   0        0        0    24631 2023-07-17 15:14:08.000000 PDStoolkit-0.0.2/src/PDStoolkit/PDS_DPLS.py
+-rw-rw-rw-   0        0        0    14426 2023-07-14 20:57:06.000000 PDStoolkit-0.0.2/src/PDStoolkit/PDS_PCA.py
+-rw-rw-rw-   0        0        0    16301 2023-07-14 20:57:17.000000 PDStoolkit-0.0.2/src/PDStoolkit/PDS_PLS.py
+-rw-rw-rw-   0        0        0      277 2023-07-24 20:45:35.000000 PDStoolkit-0.0.2/src/PDStoolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:54:03.348948 PDStoolkit-0.0.2/src/PDStoolkit.egg-info/
+-rw-rw-rw-   0        0        0     6735 2023-07-24 20:54:03.000000 PDStoolkit-0.0.2/src/PDStoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-07-24 20:54:03.000000 PDStoolkit-0.0.2/src/PDStoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 20:54:03.000000 PDStoolkit-0.0.2/src/PDStoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 20:54:03.000000 PDStoolkit-0.0.2/src/PDStoolkit.egg-info/top_level.txt
```

### Comparing `PDStoolkit-0.0.1/LICENSE` & `PDStoolkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PDStoolkit-0.0.1/PKG-INFO` & `PDStoolkit-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDStoolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to facilitate building process data science solutions including process modeling, monitoring, fault diagnosis, etc.
 Home-page: https://mlforpse.com/intro-to-pdstoolkit-python-package/
 Author: Ankur Kumar
 Author-email: MLforPSE@gmail.com
 Project-URL: Source Code:, https://github.com/ML-PSE/PDStoolkit-Python-Package
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -22,14 +22,15 @@
 4. [Installation](#install)
 5. [Usage](#usage)
 
 ## Description <a name="desc"></a>
 The PDStoolkit (Process Data Science Toolkit) package has been created to provide easy-to-use modules to help quickly build data-based solutions for process systems such as those for process monitoring, modeling, fault diagnosis, system identification, etc. Current modules in the package are wrappers around pre-existing Sklearn's classes and provide several additional methods to facilitate a process data scientist's job. Details on these are provided in the following section. More modules relevant for process data science will be added over time.
 
 ## Documentation and Tutorials <a name="docs"></a>
+- PDStoolkit_Manual.pdf (in Github repository) provides some quick information on the algorithms implemented in the package
 - Class documentations are provided in the 'docs' folder in Github (Source Code) repository
 - Tutorials are provided in the 'tutorials' folder in Github (Source Code) repository
 - The blog post (https://mlforpse.com/intro-to-pdstoolkit-python-package/) gives some perspective behind the motivation for development of PDStoolkit package 
 - Theoretical and conceptual details on specific algorithms can be found in our book (https://leanpub.com/machineLearningPSE) 
 
 ## Package Contents <a name="content"></a>
 The main modules in the package currently are:
@@ -38,21 +39,46 @@
    - This class is a child of [sklearn.decomposition.PCA class](http://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) 
    - The following additional methods are provided
      - *computeMetrics*: computes the monitoring indices (Q or SPE, T2) for the supplied data
      - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
      - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
      - *detect_abnormalities*: detects if the observations are abnormal or normal samples
      - *get_contributions*: returns abnormality contributions for T2 and SPE for an observation sample
+	 
  - **PDS_PLS: Partial Least Squares regression for Process Data Science**
    - This class is a child of [sklearn.cross_decomposition.PLSRegression class](http://scikit-learn.org/stable/modules/generated/sklearn.cross_decomposition.PLSRegression.html) 
    - The following additional methods are provided
      - *computeMetrics*: computes the monitoring indices (SPEx, SPEy, T2) for the supplied data
      - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
      - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
      - *detect_abnormalities*: detects if the observations are abnormal or normal samples
+	 
+ - **PDS_DPCA: Dynamic Principal Component analysis for Process Data Science**
+   - This class is a child of [sklearn.decomposition.PCA class](http://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) 
+   - The following additional methods are provided
+     - *computeMetrics*: computes the monitoring indices (Q or SPE, T2) for the supplied data
+     - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
+     - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
+     - *detect_abnormalities*: detects if the observations are abnormal or normal samples
+       
+ - **PDS_DPLS: Dynamic Partial Least Squares regression for Process Data Science**
+   - This class is a child of [sklearn.cross_decomposition.PLSRegression class](http://scikit-learn.org/stable/modules/generated/sklearn.cross_decomposition.PLSRegression.html) 
+   - The following additional methods are provided
+     - *computeMetrics*: computes the monitoring indices (SPEx, SPEy, T2) for the supplied data
+     - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
+     - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
+     - *detect_abnormalities*: detects if the observations are abnormal or normal samples
+       
+ - **PDS_CVA: Canonical Variate Analysis for Process Data Science**
+   - This class is written from scratch 
+   - The following additional methods are provided
+     - *computeMetrics*: computes the monitoring indices (Ts2, Te2, Q) for the supplied data
+     - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
+     - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
+     - *detect_abnormalities*: detects if the observations are abnormal or normal samples
  
 ## Instalation <a name="install"></a>
 Installation from Pypi:
 
     pip install PDStoolkit
 
 Import modules
@@ -73,12 +99,12 @@
 
 T2_train, SPE_train = pca.computeMetrics(data_train_normal, isTrainingData=True)
 T2_CL, SPE_CL = pca.computeThresholds(method='statistical', alpha=0.01)
 pca.draw_monitoring_charts(title='training data')
 
 # fault detectiona and fault diagnosis on test data
 pca.detect_abnormalities(data_test_normal, title='test data')
-T2_contri, SPE_contri = pca.get_contributions(data_test_normal[15,:])
+T2_contri, SPE_contri = pca.get_contributions(data_test_normal)
 ```
     
 ### License
 All code is provided under a BSD 3-clause license. See LICENSE file for more information.
```

### Comparing `PDStoolkit-0.0.1/README.md` & `PDStoolkit-0.0.2/src/PDStoolkit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,36 @@
+Metadata-Version: 2.1
+Name: PDStoolkit
+Version: 0.0.2
+Summary: A Python package to facilitate building process data science solutions including process modeling, monitoring, fault diagnosis, etc.
+Home-page: https://mlforpse.com/intro-to-pdstoolkit-python-package/
+Author: Ankur Kumar
+Author-email: MLforPSE@gmail.com
+Project-URL: Source Code:, https://github.com/ML-PSE/PDStoolkit-Python-Package
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PDStoolkit
 
 ### Table of Contents
 1. [Project Description](#desc)
 2. [Documentation & Tutorials](#docs)
 3. [Package Contents](#content)
 4. [Installation](#install)
 5. [Usage](#usage)
 
 ## Description <a name="desc"></a>
 The PDStoolkit (Process Data Science Toolkit) package has been created to provide easy-to-use modules to help quickly build data-based solutions for process systems such as those for process monitoring, modeling, fault diagnosis, system identification, etc. Current modules in the package are wrappers around pre-existing Sklearn's classes and provide several additional methods to facilitate a process data scientist's job. Details on these are provided in the following section. More modules relevant for process data science will be added over time.
 
 ## Documentation and Tutorials <a name="docs"></a>
+- PDStoolkit_Manual.pdf (in Github repository) provides some quick information on the algorithms implemented in the package
 - Class documentations are provided in the 'docs' folder in Github (Source Code) repository
 - Tutorials are provided in the 'tutorials' folder in Github (Source Code) repository
 - The blog post (https://mlforpse.com/intro-to-pdstoolkit-python-package/) gives some perspective behind the motivation for development of PDStoolkit package 
 - Theoretical and conceptual details on specific algorithms can be found in our book (https://leanpub.com/machineLearningPSE) 
 
 ## Package Contents <a name="content"></a>
 The main modules in the package currently are:
@@ -23,21 +39,46 @@
    - This class is a child of [sklearn.decomposition.PCA class](http://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) 
    - The following additional methods are provided
      - *computeMetrics*: computes the monitoring indices (Q or SPE, T2) for the supplied data
      - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
      - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
      - *detect_abnormalities*: detects if the observations are abnormal or normal samples
      - *get_contributions*: returns abnormality contributions for T2 and SPE for an observation sample
+	 
  - **PDS_PLS: Partial Least Squares regression for Process Data Science**
    - This class is a child of [sklearn.cross_decomposition.PLSRegression class](http://scikit-learn.org/stable/modules/generated/sklearn.cross_decomposition.PLSRegression.html) 
    - The following additional methods are provided
      - *computeMetrics*: computes the monitoring indices (SPEx, SPEy, T2) for the supplied data
      - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
      - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
      - *detect_abnormalities*: detects if the observations are abnormal or normal samples
+	 
+ - **PDS_DPCA: Dynamic Principal Component analysis for Process Data Science**
+   - This class is a child of [sklearn.decomposition.PCA class](http://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) 
+   - The following additional methods are provided
+     - *computeMetrics*: computes the monitoring indices (Q or SPE, T2) for the supplied data
+     - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
+     - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
+     - *detect_abnormalities*: detects if the observations are abnormal or normal samples
+       
+ - **PDS_DPLS: Dynamic Partial Least Squares regression for Process Data Science**
+   - This class is a child of [sklearn.cross_decomposition.PLSRegression class](http://scikit-learn.org/stable/modules/generated/sklearn.cross_decomposition.PLSRegression.html) 
+   - The following additional methods are provided
+     - *computeMetrics*: computes the monitoring indices (SPEx, SPEy, T2) for the supplied data
+     - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
+     - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
+     - *detect_abnormalities*: detects if the observations are abnormal or normal samples
+       
+ - **PDS_CVA: Canonical Variate Analysis for Process Data Science**
+   - This class is written from scratch 
+   - The following additional methods are provided
+     - *computeMetrics*: computes the monitoring indices (Ts2, Te2, Q) for the supplied data
+     - *computeThresholds*: computes the thresholds / control limits for the monitoring indices from training data
+     - *draw_monitoring_charts*: draws the monitoring charts for the training or test data
+     - *detect_abnormalities*: detects if the observations are abnormal or normal samples
  
 ## Instalation <a name="install"></a>
 Installation from Pypi:
 
     pip install PDStoolkit
 
 Import modules
@@ -58,12 +99,12 @@
 
 T2_train, SPE_train = pca.computeMetrics(data_train_normal, isTrainingData=True)
 T2_CL, SPE_CL = pca.computeThresholds(method='statistical', alpha=0.01)
 pca.draw_monitoring_charts(title='training data')
 
 # fault detectiona and fault diagnosis on test data
 pca.detect_abnormalities(data_test_normal, title='test data')
-T2_contri, SPE_contri = pca.get_contributions(data_test_normal[15,:])
+T2_contri, SPE_contri = pca.get_contributions(data_test_normal)
 ```
     
 ### License
 All code is provided under a BSD 3-clause license. See LICENSE file for more information.
```

### Comparing `PDStoolkit-0.0.1/setup.cfg` & `PDStoolkit-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 4453 746f 6f6c 6b69 740d 0a76   = PDStoolkit..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e31 0d0a  ersion = 0.0.1..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
 00000030: 6175 7468 6f72 203d 2041 6e6b 7572 204b  author = Ankur K
 00000040: 756d 6172 0d0a 6175 7468 6f72 5f65 6d61  umar..author_ema
 00000050: 696c 203d 204d 4c66 6f72 5053 4540 676d  il = MLforPSE@gm
 00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000070: 7469 6f6e 203d 2041 2050 7974 686f 6e20  tion = A Python 
 00000080: 7061 636b 6167 6520 746f 2066 6163 696c  package to facil
 00000090: 6974 6174 6520 6275 696c 6469 6e67 2070  itate building p
```

### Comparing `PDStoolkit-0.0.1/src/PDStoolkit/PDS_PCA.py` & `PDStoolkit-0.0.2/src/PDStoolkit/PDS_PCA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 A module for customized PCA class for process monitoring and fault diagnosis.
-Monitoring methodology is described is our book  'Machine Learning for Process Systems Engineering' (https://leanpub.com/machineLearningPSE)
+Monitoring methodology is described in our book  'Machine Learning for Process Systems Engineering' (https://mlforpse.com/books/)
 ============================================================================
 """
 
 # Version: 2022
 # Author: Ankur Kumar @ MLforPSE.com
 # License: BSD 3 clause
 
@@ -22,15 +22,15 @@
     2) computeThresholds: computes the thresholds / control limits for the monitoring indices from training data
     3) draw_monitoring_charts: Draw the monitoring charts for the training or test data
     4) detect_abnormalities: Detects if the observations are abnormal or normal samples
     5) get_contributions: Returns abnormality contributions for T2 and SPE for an observation vector
     
     Usage Example
     --------
-    >>> from PDS_PCA import PDS_PCA
+    >>> from PDStoolkit import PDS_PCA
     >>> from sklearn.preprocessing import StandardScaler
     
     >>> X = np.random.rand(30,5)
     >>> scaler = StandardScaler()
     >>> X_normal = scaler.fit_transform(X)
     
     >>> pca = PDS_PCA()
@@ -39,17 +39,17 @@
     >>> T2_CL, SPE_CL = pca.computeThresholds(method='percentile')
     >>> pca.draw_monitoring_charts(metrics=metrics_train, title='training data')
     
     >>> X_test = scaler.transform(np.random.rand(30,5))
     >>> abnormalityFlags = pca.detect_abnormalities(X_test, title='Test data')
     '''
     
-    def __init(self, **kws):
+    def __init__(self, **kws):
         self.eig_vals_all = None 
-        PCA.__init__(**kws)
+        super().__init__(**kws)
     
     def fit(self, X, autoFindNLatents=False, varianceThreshold=0.9):
         """
         Extends the fit method of Sklearn PCA to allow in-built computation of the 'optimal' number of latents.
         
         Parameters:
         ---------------------
@@ -67,14 +67,15 @@
         Returns
         ---------------------
         self: object
             fitted model
         """
         
         if autoFindNLatents:
+            self.n_components = X.shape[1] 
             PCA.fit(self, X)
             self.eig_vals_all = self.explained_variance_ # to be used later for threshold calculations 
             
             # decide # of PCs to retain
             explained_variance = 100*self.explained_variance_ratio_ # in percentage
             cum_explained_variance = np.cumsum(explained_variance) # cumulative % variance explained
             selected_Nlatent = np.argmax(cum_explained_variance >= varianceThreshold*100) + 1
@@ -91,19 +92,22 @@
             plt.show()
             
             # store the computed optimal_Nlatents
             self.n_components = selected_Nlatent
         
         # call the original fit method of PCA class
         PCA.fit(self, X)
-        if self.n_components == X.shape[1]:
-            self.eig_vals_all = self.explained_variance_
-        else:
-            PCA_temp = PCA().fit(X)
-            self.eig_vals_all = PCA_temp.explained_variance_
+        
+        # ensure eig_vals_all attribute is assigned
+        if not autoFindNLatents:
+            if self.n_components == X.shape[1]:
+                self.eig_vals_all = self.explained_variance_
+            else:
+                PCA_temp = PCA().fit(X)
+                self.eig_vals_all = PCA_temp.explained_variance_
             
         return self
         
     def computeMetrics(self, X, isTrainingData=False):
         """
         computes the monitoring indices for the supplied data
         
@@ -287,15 +291,15 @@
         if drawMonitoringChart:
             self.draw_monitoring_charts(metrics=(T2, SPE), title=title)
                 
         return abnormalityFlags
     
     def get_contributions(self, x, plotContributions=True, title=''):
         """
-        Returns abnormality contributions for T2 and SPE metrics for an observation vector.
+        Returns abnormality contributions for T2 and SPE metrics for an observation vector x.
         
         Parameters:
         ---------------------
         x: ndarray of shape (n_features,)
             Observation sample where n_features is the number of features
                                           
         Returns:
```

### Comparing `PDStoolkit-0.0.1/src/PDStoolkit/PDS_PLS.py` & `PDStoolkit-0.0.2/src/PDStoolkit/PDS_PLS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 A module for customized PLS class for process monitoring. 
-Monitoring methodology is described is our book  'Machine Learning for Process Systems Engineering' (https://leanpub.com/machineLearningPSE)
+Monitoring methodology is described in our book  'Machine Learning for Process Systems Engineering' (https://mlforpse.com/books/)
 =======================================================
 """
 
 # Version: 2022
 # Author: Ankur Kumar @ MLforPSE.com
 # License: BSD 3 clause
 
@@ -16,24 +16,24 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import scipy.stats
 import sys
 
 #%% define class
 class PDS_PLS(PLSRegression):
-    ''' This class wraps Sklearn's PLS class to provide the following addiitonal methods
+    ''' This class wraps Sklearn's PLSRegression class to provide the following addiitonal methods
     
     1) computeMetrics: computes the monitoring indices for the supplied data
     2) computeThresholds: computes the thresholds / control limits for the monitoring indices from training data
     3) draw_monitoring_charts: Draw the monitoring charts for the training or test data
     4) detect_abnormalities: Detects if the observations are abnormal or normal samples
     
     Usage Example
     --------
-    >>> from PDS_PLS import PDS_PLS
+    >>> from PDStoolkit import PDS_PLS
     >>> X = np.random.rand(30,5)
     >>> Y = np.random.rand(30,2)
     >>> pls = PDS_PLS()
     >>> pls.fit(X, Y, autoFindNLatents=True)
     >>> metrics_train = pls.computeMetrics(X, Y, isTrainingData=True)
     >>> T2_CL, SPEx_CL, SPEy_CL = pls.computeThresholds(method='statistical', alpha=0.01)
     >>> pls.draw_monitoring_charts(metrics=metrics_train, title='training data')
@@ -44,23 +44,23 @@
     '''
     
     def __init(self, **kws):
         PLSRegression.__init__(**kws)
     
     def fit(self, X, Y, autoFindNLatents=False, n_CVsplits=10, ratioThreshold=0.0):
         """
-        Extends the fit method of Sklearn PLS to allow in-built computation of the 'optimal' number of latents.
+        Extends the fit method of Sklearn PLSRegression to allow in-built computation of the 'optimal' number of latents.
         
         Parameters:
         ---------------------
         X: ndarray of shape (n_samples, n_features)
-            Training vectors, where n_samples is the number of samples and n_features is the number of predictors
+            Training predictor data, where n_samples is the number of samples and n_features is the number of predictors
             
         Y: ndarray of shape (n_samples,) or (n_samples, n_targets)
-            Target vectors, where n_samples is the number of samples and n_targets is the number of response variables.
+            Target data, where n_samples is the number of samples and n_targets is the number of response variables.
                 
         autoFindNLatents: bool, optional (default False)
             Decides whether to compute the 'optimal' number of latents or not. 
             If True, cross-validation is used and by default, number of latents corresponding to the lowest validation MSE is chosen.
             
         n_CVsplits: int, optional (default 10) 
             The number of cross-validation splits to use if autoFindNLatents is True
@@ -95,22 +95,22 @@
                 local_validate_MSEs = []
                 
                 kfold = KFold(n_splits = n_CVsplits, shuffle = True, random_state = 100)
                 for fit_index, validate_index in kfold.split(Y):
                     X_fit_normal = scaler.fit_transform(X[fit_index])
                     X_validate_normal = scaler.transform(X[validate_index])
                     
-                    y_fit_normal = scaler.fit_transform(Y[fit_index])
-                    y_validate_normal = scaler.transform(Y[validate_index])
+                    Y_fit_normal = scaler.fit_transform(Y[fit_index])
+                    Y_validate_normal = scaler.transform(Y[validate_index])
                     
                     pls = PLSRegression(n_components = Nlatent)
-                    pls.fit(X_fit_normal, y_fit_normal)
+                    pls.fit(X_fit_normal, Y_fit_normal)
                     
-                    local_fit_MSEs.append(mean_squared_error(y_fit_normal, pls.predict(X_fit_normal)))
-                    local_validate_MSEs.append(mean_squared_error(y_validate_normal, 
+                    local_fit_MSEs.append(mean_squared_error(Y_fit_normal, pls.predict(X_fit_normal)))
+                    local_validate_MSEs.append(mean_squared_error(Y_validate_normal, 
                                                                     pls.predict(X_validate_normal)))
                 
                 fit_MSE.append(np.mean(local_fit_MSEs))
                 validate_MSE.append(np.mean(local_validate_MSEs))
                 
                 # check if threshold criteria needs to be used
                 if ratioThreshold > 0:
```

