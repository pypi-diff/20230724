# Comparing `tmp/pyviscous-1.2.1.tar.gz` & `tmp/pyviscous-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviscous-1.2.1.tar", last modified: Tue Jul 18 03:39:49 2023, max compression
+gzip compressed data, was "pyviscous-2.1.0.tar", last modified: Mon Jul 24 17:40:11 2023, max compression
```

## Comparing `pyviscous-1.2.1.tar` & `pyviscous-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 03:39:49.175521 pyviscous-1.2.1/
--rw-r--r--   0 hongliliu   (501) staff       (20)     1603 2023-07-18 02:24:06.000000 pyviscous-1.2.1/LICENSE
--rw-r--r--   0 hongliliu   (501) staff       (20)     2625 2023-07-18 03:39:49.175281 pyviscous-1.2.1/PKG-INFO
--rw-r--r--   0 hongliliu   (501) staff       (20)     1830 2023-07-18 02:24:06.000000 pyviscous-1.2.1/README.md
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 03:39:49.172574 pyviscous-1.2.1/pyviscous/
--rwxr-xr-x   0 hongliliu   (501) staff       (20)       85 2023-07-18 02:24:06.000000 pyviscous-1.2.1/pyviscous/__init__.py
--rw-r--r--   0 hongliliu   (501) staff       (20)    24534 2023-07-18 02:24:06.000000 pyviscous-1.2.1/pyviscous/plot.py
--rwxr-xr-x   0 hongliliu   (501) staff       (20)    22364 2023-07-18 02:24:06.000000 pyviscous-1.2.1/pyviscous/pyviscous.py
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 03:39:49.174947 pyviscous-1.2.1/pyviscous.egg-info/
--rw-r--r--   0 hongliliu   (501) staff       (20)     2625 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/PKG-INFO
--rw-r--r--   0 hongliliu   (501) staff       (20)      321 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/SOURCES.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/dependency_links.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       49 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/entry_points.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-18 02:27:23.000000 pyviscous-1.2.1/pyviscous.egg-info/not-zip-safe
--rw-r--r--   0 hongliliu   (501) staff       (20)       59 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/requires.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       10 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/top_level.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       38 2023-07-18 03:39:49.175590 pyviscous-1.2.1/setup.cfg
--rwxr-xr-x   0 hongliliu   (501) staff       (20)     1697 2023-07-18 03:36:48.000000 pyviscous-1.2.1/setup.py
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-24 17:40:11.383361 pyviscous-2.1.0/
+-rw-r--r--   0 hongliliu   (501) staff       (20)     1603 2023-07-24 17:30:37.000000 pyviscous-2.1.0/LICENSE
+-rw-r--r--   0 hongliliu   (501) staff       (20)     2637 2023-07-24 17:40:11.382907 pyviscous-2.1.0/PKG-INFO
+-rw-r--r--   0 hongliliu   (501) staff       (20)     1842 2023-07-24 17:30:37.000000 pyviscous-2.1.0/README.md
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-24 17:40:11.379304 pyviscous-2.1.0/pyviscous/
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)       85 2023-07-24 17:30:37.000000 pyviscous-2.1.0/pyviscous/__init__.py
+-rw-r--r--   0 hongliliu   (501) staff       (20)    24534 2023-07-24 17:30:37.000000 pyviscous-2.1.0/pyviscous/plot.py
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)    22344 2023-07-24 17:30:37.000000 pyviscous-2.1.0/pyviscous/pyviscous.py
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-24 17:40:11.382341 pyviscous-2.1.0/pyviscous.egg-info/
+-rw-r--r--   0 hongliliu   (501) staff       (20)     2637 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/PKG-INFO
+-rw-r--r--   0 hongliliu   (501) staff       (20)      321 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/SOURCES.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/dependency_links.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       49 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/entry_points.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/not-zip-safe
+-rw-r--r--   0 hongliliu   (501) staff       (20)       59 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/requires.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       10 2023-07-24 17:40:11.000000 pyviscous-2.1.0/pyviscous.egg-info/top_level.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       38 2023-07-24 17:40:11.383491 pyviscous-2.1.0/setup.cfg
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)     1697 2023-07-24 17:37:16.000000 pyviscous-2.1.0/setup.py
```

### Comparing `pyviscous-1.2.1/LICENSE` & `pyviscous-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviscous-1.2.1/PKG-INFO` & `pyviscous-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviscous
-Version: 1.2.1
+Version: 2.1.0
 Summary: Python codes to implement the VISCOUSm global sensitivity analysis framework
 Home-page: https://github.com/CH-Earth/pyviscous
 Author: Hongli Liu
 Author-email: hongliliu68@gmail.com
 License: GNU General Public License v3
 Keywords: pyviscous
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,33 +16,33 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Abstract
-pyVISCOUS is the open-source code of VISCOUSm in Python. VISCOUSm is an improved copula-based framework for efficient global sensitivity analysis. It has the advantage that it can use existing model input (e.g., model parameters) and output (e.g., model responses) data to estimate Sobol’ sensitivity indices. In comparison with the VISCOUS of Sheikholeslami et al. ([2021](https://doi.org/10.1029/2020WR028435)), VISCOUSm improves the handling of marginal densities of the GMCM (Gaussian mixture copula model). 
+pyVISCOUS is the open-source code of VISCOUS in Python. VISCOUS (VarIance-based Sensitivity analysis using COpUlaS) is a variance-based global sensitivity analysis framework. It was developed by Sheikholeslami et al. ([2021](https://doi.org/10.1029/2020WR028435)) and improved by Liu et al. (2023).The advantage of VISCOUS is that it can use existing model input-output data (e.g., water model parameters-responses) to estimate the first- and total-order Sobol’ sensitivity indices. 
 
-Within the VISCOUSm framework, the following steps are included.
+Within the VISCOUS framework, the following steps are included. Details can be found in Liu et al. (2023).
 
 ![flowchart](https://github.com/CH-Earth/pyviscous/assets/48458815/2e8f7575-41d4-4e6a-bac8-fadc2a5b9c7a)
 
 ### Installation
 #### From PyPI
 ```pip install pyviscous```
 
 #### From source
 
 Clone pyviscous with: ```git clone https://github.com/CH-Earth/pyviscous.git```
 
 Then navigate to the pyviscous directory and install with: ```python setup.py install```
 
 ### Examples
-We provide four example notebooks in the example directory. In each example, there are scripts to generate input-output data, set up and run VISCOUSm, and evaluate the sensitivity results.
+We provide four example notebooks in the example directory. In each example, there are scripts to generate input-output data, set up and run VISCOUS, and evaluate the sensitivity results.
 
 ### References
-Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Freer, J., Knoben, W. J. M., Marsh C. B., & Papalexiou, S. M. (2022) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
+Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Knoben, W. J. M., Freer, J., Marsh C. B., & Papalexiou, S. M. (2023) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
 
 Sheikholeslami, R., Gharari, S., Papalexiou, S. M., & Clark, M. P. (2021) VISCOUS: A variance-based sensitivity analysis using copulas for efficient identification of dominant hydrological processes. Water Resources Research, 57, e2020WR028435, https://doi.org/10.1029/2020WR028435
 
 ---
 This package was created with Cookiecutter and the `https://github.com/audreyr/cookiecutter-pypackage` project template.
```

### Comparing `pyviscous-1.2.1/README.md` & `pyviscous-2.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ### Abstract
-pyVISCOUS is the open-source code of VISCOUSm in Python. VISCOUSm is an improved copula-based framework for efficient global sensitivity analysis. It has the advantage that it can use existing model input (e.g., model parameters) and output (e.g., model responses) data to estimate Sobol’ sensitivity indices. In comparison with the VISCOUS of Sheikholeslami et al. ([2021](https://doi.org/10.1029/2020WR028435)), VISCOUSm improves the handling of marginal densities of the GMCM (Gaussian mixture copula model). 
+pyVISCOUS is the open-source code of VISCOUS in Python. VISCOUS (VarIance-based Sensitivity analysis using COpUlaS) is a variance-based global sensitivity analysis framework. It was developed by Sheikholeslami et al. ([2021](https://doi.org/10.1029/2020WR028435)) and improved by Liu et al. (2023).The advantage of VISCOUS is that it can use existing model input-output data (e.g., water model parameters-responses) to estimate the first- and total-order Sobol’ sensitivity indices. 
 
-Within the VISCOUSm framework, the following steps are included.
+Within the VISCOUS framework, the following steps are included. Details can be found in Liu et al. (2023).
 
 ![flowchart](https://github.com/CH-Earth/pyviscous/assets/48458815/2e8f7575-41d4-4e6a-bac8-fadc2a5b9c7a)
 
 ### Installation
 #### From PyPI
 ```pip install pyviscous```
 
 #### From source
 
 Clone pyviscous with: ```git clone https://github.com/CH-Earth/pyviscous.git```
 
 Then navigate to the pyviscous directory and install with: ```python setup.py install```
 
 ### Examples
-We provide four example notebooks in the example directory. In each example, there are scripts to generate input-output data, set up and run VISCOUSm, and evaluate the sensitivity results.
+We provide four example notebooks in the example directory. In each example, there are scripts to generate input-output data, set up and run VISCOUS, and evaluate the sensitivity results.
 
 ### References
-Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Freer, J., Knoben, W. J. M., Marsh C. B., & Papalexiou, S. M. (2022) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
+Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Knoben, W. J. M., Freer, J., Marsh C. B., & Papalexiou, S. M. (2023) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
 
 Sheikholeslami, R., Gharari, S., Papalexiou, S. M., & Clark, M. P. (2021) VISCOUS: A variance-based sensitivity analysis using copulas for efficient identification of dominant hydrological processes. Water Resources Research, 57, e2020WR028435, https://doi.org/10.1029/2020WR028435
 
 ---
 This package was created with Cookiecutter and the `https://github.com/audreyr/cookiecutter-pypackage` project template.
```

### Comparing `pyviscous-1.2.1/pyviscous/plot.py` & `pyviscous-2.1.0/pyviscous/plot.py`

 * *Files identical despite different names*

### Comparing `pyviscous-1.2.1/pyviscous/pyviscous.py` & `pyviscous-2.1.0/pyviscous/pyviscous.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-from   scipy.stats import multivariate_normal, norm, gaussian_kde
+from   scipy.stats import multivariate_normal
 from   sklearn.cluster import KMeans
 from   scipy.interpolate import interp1d     # used to estimate the empirical relationship between y_norm and y_cdf
 
 import copulae
 from   copulae import GaussianMixtureCopula  # used to apply GMCM more flexibly
 from   copulae.core import pseudo_obs        # used to get data rank-based CDF
 from   copulae.mixtures.gmc import GMCParam  # used to generate initial GMCM parameter estiamtes
```

### Comparing `pyviscous-1.2.1/pyviscous.egg-info/PKG-INFO` & `pyviscous-2.1.0/pyviscous.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviscous
-Version: 1.2.1
+Version: 2.1.0
 Summary: Python codes to implement the VISCOUSm global sensitivity analysis framework
 Home-page: https://github.com/CH-Earth/pyviscous
 Author: Hongli Liu
 Author-email: hongliliu68@gmail.com
 License: GNU General Public License v3
 Keywords: pyviscous
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,33 +16,33 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Abstract
-pyVISCOUS is the open-source code of VISCOUSm in Python. VISCOUSm is an improved copula-based framework for efficient global sensitivity analysis. It has the advantage that it can use existing model input (e.g., model parameters) and output (e.g., model responses) data to estimate Sobol’ sensitivity indices. In comparison with the VISCOUS of Sheikholeslami et al. ([2021](https://doi.org/10.1029/2020WR028435)), VISCOUSm improves the handling of marginal densities of the GMCM (Gaussian mixture copula model). 
+pyVISCOUS is the open-source code of VISCOUS in Python. VISCOUS (VarIance-based Sensitivity analysis using COpUlaS) is a variance-based global sensitivity analysis framework. It was developed by Sheikholeslami et al. ([2021](https://doi.org/10.1029/2020WR028435)) and improved by Liu et al. (2023).The advantage of VISCOUS is that it can use existing model input-output data (e.g., water model parameters-responses) to estimate the first- and total-order Sobol’ sensitivity indices. 
 
-Within the VISCOUSm framework, the following steps are included.
+Within the VISCOUS framework, the following steps are included. Details can be found in Liu et al. (2023).
 
 ![flowchart](https://github.com/CH-Earth/pyviscous/assets/48458815/2e8f7575-41d4-4e6a-bac8-fadc2a5b9c7a)
 
 ### Installation
 #### From PyPI
 ```pip install pyviscous```
 
 #### From source
 
 Clone pyviscous with: ```git clone https://github.com/CH-Earth/pyviscous.git```
 
 Then navigate to the pyviscous directory and install with: ```python setup.py install```
 
 ### Examples
-We provide four example notebooks in the example directory. In each example, there are scripts to generate input-output data, set up and run VISCOUSm, and evaluate the sensitivity results.
+We provide four example notebooks in the example directory. In each example, there are scripts to generate input-output data, set up and run VISCOUS, and evaluate the sensitivity results.
 
 ### References
-Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Freer, J., Knoben, W. J. M., Marsh C. B., & Papalexiou, S. M. (2022) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
+Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Knoben, W. J. M., Freer, J., Marsh C. B., & Papalexiou, S. M. (2023) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
 
 Sheikholeslami, R., Gharari, S., Papalexiou, S. M., & Clark, M. P. (2021) VISCOUS: A variance-based sensitivity analysis using copulas for efficient identification of dominant hydrological processes. Water Resources Research, 57, e2020WR028435, https://doi.org/10.1029/2020WR028435
 
 ---
 This package was created with Cookiecutter and the `https://github.com/audreyr/cookiecutter-pypackage` project template.
```

### Comparing `pyviscous-1.2.1/setup.py` & `pyviscous-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,14 @@
     include_package_data=True,
     keywords='pyviscous',
     name='pyviscous',
     packages=find_packages(include=['pyviscous', 'pyviscous.*', 'plot.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/CH-Earth/pyviscous',
-    version='1.2.1',
+    version='2.1.0',
     zip_safe=False,
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

