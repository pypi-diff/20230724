# Comparing `tmp/geosss-0.1.0.tar.gz` & `tmp/geosss-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosss-0.1.0.tar", max compression
+gzip compressed data, was "geosss-0.1.1.tar", max compression
```

## Comparing `geosss-0.1.0.tar` & `geosss-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1482 2023-07-21 12:26:29.062740 geosss-0.1.0/LICENSE
--rw-r--r--   0        0        0     4060 2023-07-24 11:44:30.329072 geosss-0.1.0/README.md
--rw-r--r--   0        0        0      874 2023-07-24 13:15:40.474358 geosss-0.1.0/geosss/__init__.py
--rw-r--r--   0        0        0     2008 2023-07-24 10:44:27.723589 geosss-0.1.0/geosss/demo_vis.py
--rw-r--r--   0        0        0     5526 2023-07-24 13:15:34.178370 geosss-0.1.0/geosss/distributions.py
--rw-r--r--   0        0        0    10315 2023-07-21 12:56:08.777564 geosss-0.1.0/geosss/mcmc.py
--rw-r--r--   0        0        0     5077 2023-07-20 16:23:21.588897 geosss-0.1.0/geosss/rand.py
--rw-r--r--   0        0        0     2970 2023-07-12 13:13:10.029358 geosss-0.1.0/geosss/sphere.py
--rw-r--r--   0        0        0     7405 2023-07-24 13:38:26.469573 geosss-0.1.0/geosss/testing.py
--rw-r--r--   0        0        0     5208 2023-07-21 12:35:35.101993 geosss-0.1.0/geosss/utils.py
--rw-r--r--   0        0        0     9267 2023-07-20 16:22:12.304818 geosss-0.1.0/geosss/vMF_diagnostics.py
--rw-r--r--   0        0        0      804 2023-07-24 09:27:24.741352 geosss-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 geosss-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1482 2023-07-21 12:26:29.062740 geosss-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4227 2023-07-24 15:37:23.076397 geosss-0.1.1/README.md
+-rw-r--r--   0        0        0      874 2023-07-24 13:15:40.474358 geosss-0.1.1/geosss/__init__.py
+-rw-r--r--   0        0        0     2008 2023-07-24 10:44:27.723589 geosss-0.1.1/geosss/demo_vis.py
+-rw-r--r--   0        0        0     5526 2023-07-24 13:15:34.178370 geosss-0.1.1/geosss/distributions.py
+-rw-r--r--   0        0        0    10315 2023-07-21 12:56:08.777564 geosss-0.1.1/geosss/mcmc.py
+-rw-r--r--   0        0        0     5077 2023-07-20 16:23:21.588897 geosss-0.1.1/geosss/rand.py
+-rw-r--r--   0        0        0     2970 2023-07-12 13:13:10.029358 geosss-0.1.1/geosss/sphere.py
+-rw-r--r--   0        0        0     7405 2023-07-24 13:38:26.469573 geosss-0.1.1/geosss/testing.py
+-rw-r--r--   0        0        0     5208 2023-07-21 12:35:35.101993 geosss-0.1.1/geosss/utils.py
+-rw-r--r--   0        0        0     9267 2023-07-20 16:22:12.304818 geosss-0.1.1/geosss/vMF_diagnostics.py
+-rw-r--r--   0        0        0      872 2023-07-24 15:43:01.580483 geosss-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5145 1970-01-01 00:00:00.000000 geosss-0.1.1/PKG-INFO
```

### Comparing `geosss-0.1.0/LICENSE` & `geosss-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/README.md` & `geosss-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <p align="center">
-<img src="assets/logo.svg" width="300">
+<img src="https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
 
 [![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.48550/arXiv.2301.08056)
 
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
 This Python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
 This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
-![animation_vMF](assets/animation_vMF.gif)
+![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif)
 
 ## Installation
 
-GeoSSS is available for installation from PyPI (TODO: Add a link here later, when on PyPI). Therefore, simply type:
+GeoSSS is available for installation from PyPI. Therefore, simply type:
 
 ```
 pip install geosss
 ```
 
 ## Getting Started
 
@@ -79,15 +79,15 @@
 The plots in the [paper](https://doi.org/10.48550/arXiv.2301.08056) under numerical illustrations section were generated using [`bingham.py`](scripts/bingham.py), [`mixture_vMF.py`](scripts/mixture_vMF.py), [`ess_vMF.py`](scripts/ess_vMF.py) and [`curve.py`](scripts/curve.py).
 
 ## Development
 
 The package is maintained by [Poetry](https://python-poetry.org/). To install this package and its dependencies in a dedicated virtual environment, please do the following
 
 ```
-git clone https://github.com/ShantanuKodgirwar/geosss
+git clone https://github.com/microscopic-image-analysis/geosss.git
 cd geosss
 poetry install
 ```
 
 ## Citation
 
 If you use this package, or ideas from the paper, please consider citing us.
```

### Comparing `geosss-0.1.0/geosss/__init__.py` & `geosss-0.1.1/geosss/__init__.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/geosss/demo_vis.py` & `geosss-0.1.1/geosss/demo_vis.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/geosss/distributions.py` & `geosss-0.1.1/geosss/distributions.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/geosss/mcmc.py` & `geosss-0.1.1/geosss/mcmc.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/geosss/rand.py` & `geosss-0.1.1/geosss/rand.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/geosss/sphere.py` & `geosss-0.1.1/geosss/sphere.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/geosss/testing.py` & `geosss-0.1.1/geosss/testing.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/geosss/utils.py` & `geosss-0.1.1/geosss/utils.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/geosss/vMF_diagnostics.py` & `geosss-0.1.1/geosss/vMF_diagnostics.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.0/pyproject.toml` & `geosss-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "geosss"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere."
 authors = ["Michael Habeck <michael.habeck@uni-jena.de>",
            "Shantanu Kodgirwar <shantanu.kodgirwar@uni-jena.de>", 
            "Mareike Hasenpflug <mareike.hasenpflug@uni-passau.de>",
            "Daniel Rudolf <daniel.rudolf@uni-passau.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
+repository = "https://github.com/microscopic-image-analysis/geosss"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
 scipy = "^1.11.1"
 numpy = "^1.25.1"
 matplotlib = "^3.7.2"
 seaborn = "^0.12.2"
```

### Comparing `geosss-0.1.0/PKG-INFO` & `geosss-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: geosss
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere.
+Home-page: https://github.com/microscopic-image-analysis/geosss
 License: BSD-3-Clause
 Author: Michael Habeck
 Author-email: michael.habeck@uni-jena.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,35 +16,36 @@
 Requires-Dist: csb (>=1.2.5,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tsp-solver (>=0.1,<0.2)
+Project-URL: Repository, https://github.com/microscopic-image-analysis/geosss
 Description-Content-Type: text/markdown
 
 <p align="center">
-<img src="assets/logo.svg" width="300">
+<img src="https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
 
 [![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.48550/arXiv.2301.08056)
 
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
 This Python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
 This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
-![animation_vMF](assets/animation_vMF.gif)
+![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif)
 
 ## Installation
 
-GeoSSS is available for installation from PyPI (TODO: Add a link here later, when on PyPI). Therefore, simply type:
+GeoSSS is available for installation from PyPI. Therefore, simply type:
 
 ```
 pip install geosss
 ```
 
 ## Getting Started
 
@@ -102,15 +104,15 @@
 The plots in the [paper](https://doi.org/10.48550/arXiv.2301.08056) under numerical illustrations section were generated using [`bingham.py`](scripts/bingham.py), [`mixture_vMF.py`](scripts/mixture_vMF.py), [`ess_vMF.py`](scripts/ess_vMF.py) and [`curve.py`](scripts/curve.py).
 
 ## Development
 
 The package is maintained by [Poetry](https://python-poetry.org/). To install this package and its dependencies in a dedicated virtual environment, please do the following
 
 ```
-git clone https://github.com/ShantanuKodgirwar/geosss
+git clone https://github.com/microscopic-image-analysis/geosss.git
 cd geosss
 poetry install
 ```
 
 ## Citation
 
 If you use this package, or ideas from the paper, please consider citing us.
```

