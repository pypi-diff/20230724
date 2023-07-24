# Comparing `tmp/geosss-0.1.1.tar.gz` & `tmp/geosss-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosss-0.1.1.tar", max compression
+gzip compressed data, was "geosss-0.1.2.tar", max compression
```

## Comparing `geosss-0.1.1.tar` & `geosss-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1482 2023-07-21 12:26:29.062740 geosss-0.1.1/LICENSE
--rw-r--r--   0        0        0     4227 2023-07-24 15:37:23.076397 geosss-0.1.1/README.md
--rw-r--r--   0        0        0      874 2023-07-24 13:15:40.474358 geosss-0.1.1/geosss/__init__.py
--rw-r--r--   0        0        0     2008 2023-07-24 10:44:27.723589 geosss-0.1.1/geosss/demo_vis.py
--rw-r--r--   0        0        0     5526 2023-07-24 13:15:34.178370 geosss-0.1.1/geosss/distributions.py
--rw-r--r--   0        0        0    10315 2023-07-21 12:56:08.777564 geosss-0.1.1/geosss/mcmc.py
--rw-r--r--   0        0        0     5077 2023-07-20 16:23:21.588897 geosss-0.1.1/geosss/rand.py
--rw-r--r--   0        0        0     2970 2023-07-12 13:13:10.029358 geosss-0.1.1/geosss/sphere.py
--rw-r--r--   0        0        0     7405 2023-07-24 13:38:26.469573 geosss-0.1.1/geosss/testing.py
--rw-r--r--   0        0        0     5208 2023-07-21 12:35:35.101993 geosss-0.1.1/geosss/utils.py
--rw-r--r--   0        0        0     9267 2023-07-20 16:22:12.304818 geosss-0.1.1/geosss/vMF_diagnostics.py
--rw-r--r--   0        0        0      872 2023-07-24 15:43:01.580483 geosss-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5145 1970-01-01 00:00:00.000000 geosss-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1482 2023-07-21 12:26:29.062740 geosss-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4501 2023-07-24 16:17:29.278461 geosss-0.1.2/README.md
+-rw-r--r--   0        0        0      874 2023-07-24 13:15:40.474358 geosss-0.1.2/geosss/__init__.py
+-rw-r--r--   0        0        0     2008 2023-07-24 10:44:27.723589 geosss-0.1.2/geosss/demo_vis.py
+-rw-r--r--   0        0        0     5526 2023-07-24 13:15:34.178370 geosss-0.1.2/geosss/distributions.py
+-rw-r--r--   0        0        0    10315 2023-07-21 12:56:08.777564 geosss-0.1.2/geosss/mcmc.py
+-rw-r--r--   0        0        0     5077 2023-07-20 16:23:21.588897 geosss-0.1.2/geosss/rand.py
+-rw-r--r--   0        0        0     2970 2023-07-12 13:13:10.029358 geosss-0.1.2/geosss/sphere.py
+-rw-r--r--   0        0        0     7405 2023-07-24 13:38:26.469573 geosss-0.1.2/geosss/testing.py
+-rw-r--r--   0        0        0     5208 2023-07-21 12:35:35.101993 geosss-0.1.2/geosss/utils.py
+-rw-r--r--   0        0        0     9267 2023-07-20 16:22:12.304818 geosss-0.1.2/geosss/vMF_diagnostics.py
+-rw-r--r--   0        0        0      872 2023-07-24 16:04:48.194025 geosss-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5416 1970-01-01 00:00:00.000000 geosss-0.1.2/PKG-INFO
```

### Comparing `geosss-0.1.1/LICENSE` & `geosss-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/README.md` & `geosss-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 <p align="center">
 <img src="https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
 
+![PyPI](https://img.shields.io/pypi/v/geosss)
+![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
 [![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.48550/arXiv.2301.08056)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
 This Python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
 This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
 ![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif)
 
 ## Installation
 
-GeoSSS is available for installation from PyPI. Therefore, simply type:
+GeoSSS is available for installation from [PyPI](https://pypi.org/project/geosss/). Therefore, simply type:
 
 ```
 pip install geosss
 ```
 
 ## Getting Started
```

### Comparing `geosss-0.1.1/geosss/__init__.py` & `geosss-0.1.2/geosss/__init__.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/geosss/demo_vis.py` & `geosss-0.1.2/geosss/demo_vis.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/geosss/distributions.py` & `geosss-0.1.2/geosss/distributions.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/geosss/mcmc.py` & `geosss-0.1.2/geosss/mcmc.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/geosss/rand.py` & `geosss-0.1.2/geosss/rand.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/geosss/sphere.py` & `geosss-0.1.2/geosss/sphere.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/geosss/testing.py` & `geosss-0.1.2/geosss/testing.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/geosss/utils.py` & `geosss-0.1.2/geosss/utils.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/geosss/vMF_diagnostics.py` & `geosss-0.1.2/geosss/vMF_diagnostics.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.1/pyproject.toml` & `geosss-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geosss"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere."
 authors = ["Michael Habeck <michael.habeck@uni-jena.de>",
            "Shantanu Kodgirwar <shantanu.kodgirwar@uni-jena.de>", 
            "Mareike Hasenpflug <mareike.hasenpflug@uni-passau.de>",
            "Daniel Rudolf <daniel.rudolf@uni-passau.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `geosss-0.1.1/PKG-INFO` & `geosss-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosss
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere.
 Home-page: https://github.com/microscopic-image-analysis/geosss
 License: BSD-3-Clause
 Author: Michael Habeck
 Author-email: michael.habeck@uni-jena.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: BSD License
@@ -23,29 +23,32 @@
 Project-URL: Repository, https://github.com/microscopic-image-analysis/geosss
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
 
+![PyPI](https://img.shields.io/pypi/v/geosss)
+![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
 [![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.48550/arXiv.2301.08056)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
 This Python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
 This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
 ![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif)
 
 ## Installation
 
-GeoSSS is available for installation from PyPI. Therefore, simply type:
+GeoSSS is available for installation from [PyPI](https://pypi.org/project/geosss/). Therefore, simply type:
 
 ```
 pip install geosss
 ```
 
 ## Getting Started
```

