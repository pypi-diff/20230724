# Comparing `tmp/geosss-0.1.2.tar.gz` & `tmp/geosss-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosss-0.1.2.tar", max compression
+gzip compressed data, was "geosss-0.1.3.tar", max compression
```

## Comparing `geosss-0.1.2.tar` & `geosss-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1482 2023-07-21 12:26:29.062740 geosss-0.1.2/LICENSE
--rw-r--r--   0        0        0     4501 2023-07-24 16:17:29.278461 geosss-0.1.2/README.md
--rw-r--r--   0        0        0      874 2023-07-24 13:15:40.474358 geosss-0.1.2/geosss/__init__.py
--rw-r--r--   0        0        0     2008 2023-07-24 10:44:27.723589 geosss-0.1.2/geosss/demo_vis.py
--rw-r--r--   0        0        0     5526 2023-07-24 13:15:34.178370 geosss-0.1.2/geosss/distributions.py
--rw-r--r--   0        0        0    10315 2023-07-21 12:56:08.777564 geosss-0.1.2/geosss/mcmc.py
--rw-r--r--   0        0        0     5077 2023-07-20 16:23:21.588897 geosss-0.1.2/geosss/rand.py
--rw-r--r--   0        0        0     2970 2023-07-12 13:13:10.029358 geosss-0.1.2/geosss/sphere.py
--rw-r--r--   0        0        0     7405 2023-07-24 13:38:26.469573 geosss-0.1.2/geosss/testing.py
--rw-r--r--   0        0        0     5208 2023-07-21 12:35:35.101993 geosss-0.1.2/geosss/utils.py
--rw-r--r--   0        0        0     9267 2023-07-20 16:22:12.304818 geosss-0.1.2/geosss/vMF_diagnostics.py
--rw-r--r--   0        0        0      872 2023-07-24 16:04:48.194025 geosss-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5416 1970-01-01 00:00:00.000000 geosss-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1474 2023-07-24 16:27:27.579099 geosss-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4520 2023-07-24 17:29:37.459846 geosss-0.1.3/README.md
+-rw-r--r--   0        0        0      874 2023-07-24 13:15:40.474358 geosss-0.1.3/geosss/__init__.py
+-rw-r--r--   0        0        0     2008 2023-07-24 10:44:27.723589 geosss-0.1.3/geosss/demo_vis.py
+-rw-r--r--   0        0        0     5526 2023-07-24 13:15:34.178370 geosss-0.1.3/geosss/distributions.py
+-rw-r--r--   0        0        0    10315 2023-07-21 12:56:08.777564 geosss-0.1.3/geosss/mcmc.py
+-rw-r--r--   0        0        0     5077 2023-07-20 16:23:21.588897 geosss-0.1.3/geosss/rand.py
+-rw-r--r--   0        0        0     2970 2023-07-12 13:13:10.029358 geosss-0.1.3/geosss/sphere.py
+-rw-r--r--   0        0        0     7405 2023-07-24 13:38:26.469573 geosss-0.1.3/geosss/testing.py
+-rw-r--r--   0        0        0     5208 2023-07-21 12:35:35.101993 geosss-0.1.3/geosss/utils.py
+-rw-r--r--   0        0        0     9267 2023-07-20 16:22:12.304818 geosss-0.1.3/geosss/vMF_diagnostics.py
+-rw-r--r--   0        0        0      872 2023-07-24 17:29:49.055858 geosss-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 geosss-0.1.3/PKG-INFO
```

### Comparing `geosss-0.1.2/LICENSE` & `geosss-0.1.3/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023-present, Michael Habeck
+Copyright (c) 2023, Michael Habeck
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
     1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
     2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
     3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

### Comparing `geosss-0.1.2/README.md` & `geosss-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-<img src="https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
+<img src="https://raw.githubusercontent.com/microscopic-image-analysis/geosss/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
 
 ![PyPI](https://img.shields.io/pypi/v/geosss)
 ![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
 [![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.48550/arXiv.2301.08056)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
@@ -11,15 +11,15 @@
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
 This Python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
 This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
-![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif)
+![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif?raw=true)
 
 ## Installation
 
 GeoSSS is available for installation from [PyPI](https://pypi.org/project/geosss/). Therefore, simply type:
 
 ```
 pip install geosss
```

### Comparing `geosss-0.1.2/geosss/__init__.py` & `geosss-0.1.3/geosss/__init__.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/geosss/demo_vis.py` & `geosss-0.1.3/geosss/demo_vis.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/geosss/distributions.py` & `geosss-0.1.3/geosss/distributions.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/geosss/mcmc.py` & `geosss-0.1.3/geosss/mcmc.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/geosss/rand.py` & `geosss-0.1.3/geosss/rand.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/geosss/sphere.py` & `geosss-0.1.3/geosss/sphere.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/geosss/testing.py` & `geosss-0.1.3/geosss/testing.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/geosss/utils.py` & `geosss-0.1.3/geosss/utils.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/geosss/vMF_diagnostics.py` & `geosss-0.1.3/geosss/vMF_diagnostics.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.2/pyproject.toml` & `geosss-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geosss"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere."
 authors = ["Michael Habeck <michael.habeck@uni-jena.de>",
            "Shantanu Kodgirwar <shantanu.kodgirwar@uni-jena.de>", 
            "Mareike Hasenpflug <mareike.hasenpflug@uni-passau.de>",
            "Daniel Rudolf <daniel.rudolf@uni-passau.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `geosss-0.1.2/PKG-INFO` & `geosss-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosss
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere.
 Home-page: https://github.com/microscopic-image-analysis/geosss
 License: BSD-3-Clause
 Author: Michael Habeck
 Author-email: michael.habeck@uni-jena.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: BSD License
@@ -20,15 +20,15 @@
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tsp-solver (>=0.1,<0.2)
 Project-URL: Repository, https://github.com/microscopic-image-analysis/geosss
 Description-Content-Type: text/markdown
 
 <p align="center">
-<img src="https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
+<img src="https://raw.githubusercontent.com/microscopic-image-analysis/geosss/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
 
 ![PyPI](https://img.shields.io/pypi/v/geosss)
 ![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
 [![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.48550/arXiv.2301.08056)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
@@ -36,15 +36,15 @@
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
 This Python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
 This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
-![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif)
+![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif?raw=true)
 
 ## Installation
 
 GeoSSS is available for installation from [PyPI](https://pypi.org/project/geosss/). Therefore, simply type:
 
 ```
 pip install geosss
```

