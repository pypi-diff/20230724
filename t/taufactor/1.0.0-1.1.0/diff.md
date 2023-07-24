# Comparing `tmp/taufactor-1.0.0.tar.gz` & `tmp/taufactor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taufactor-1.0.0.tar", last modified: Thu Mar 23 12:46:38 2023, max compression
+gzip compressed data, was "taufactor-1.1.0.tar", last modified: Mon Jul 24 09:09:42 2023, max compression
```

## Comparing `taufactor-1.0.0.tar` & `taufactor-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-03-23 12:46:38.509391 taufactor-1.0.0/
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      206 2023-03-08 11:13:00.000000 taufactor-1.0.0/AUTHORS.md
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     3087 2023-03-08 11:13:00.000000 taufactor-1.0.0/CONTRIBUTING.md
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      651 2023-03-23 12:20:50.000000 taufactor-1.0.0/HISTORY.md
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     1071 2023-03-08 11:13:00.000000 taufactor-1.0.0/LICENSE
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      258 2023-03-08 11:13:00.000000 taufactor-1.0.0/MANIFEST.in
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     4070 2023-03-23 12:46:38.509391 taufactor-1.0.0/PKG-INFO
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     2285 2023-03-23 12:18:29.000000 taufactor-1.0.0/README.md
-drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-03-23 12:46:38.505391 taufactor-1.0.0/docs/
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      610 2021-09-02 10:12:14.000000 taufactor-1.0.0/docs/Makefile
-drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-03-23 12:46:38.505391 taufactor-1.0.0/docs/_build/
-drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-03-23 12:46:38.505391 taufactor-1.0.0/docs/_build/html/
-drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-03-23 12:46:38.505391 taufactor-1.0.0/docs/_build/html/_static/
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      286 2021-09-02 12:25:22.000000 taufactor-1.0.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       90 2021-09-02 12:25:22.000000 taufactor-1.0.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       90 2021-09-02 12:25:22.000000 taufactor-1.0.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       59 2023-03-08 11:13:00.000000 taufactor-1.0.0/docs/authors.rst
--rwxrwxr-x   0 isaac     (1000) isaac     (1000)     4825 2023-03-08 11:13:00.000000 taufactor-1.0.0/docs/conf.py
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       64 2023-03-08 11:13:00.000000 taufactor-1.0.0/docs/contributing.rst
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       58 2023-03-08 11:13:00.000000 taufactor-1.0.0/docs/history.rst
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      295 2023-03-08 11:13:00.000000 taufactor-1.0.0/docs/index.rst
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      771 2021-09-02 10:12:14.000000 taufactor-1.0.0/docs/make.bat
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       57 2023-03-08 11:13:00.000000 taufactor-1.0.0/docs/readme.rst
--rw-rw-r--   0 isaac     (1000) isaac     (1000)   551497 2021-09-02 10:12:14.000000 taufactor-1.0.0/docs/tau_example.png
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      103 2021-09-02 10:12:14.000000 taufactor-1.0.0/pyproject.toml
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      406 2023-03-23 12:46:38.509391 taufactor-1.0.0/setup.cfg
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     1850 2023-03-23 12:45:26.000000 taufactor-1.0.0/setup.py
-drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-03-23 12:46:38.505391 taufactor-1.0.0/taufactor/
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      148 2023-03-23 10:39:55.000000 taufactor-1.0.0/taufactor/__init__.py
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      405 2021-09-02 10:12:14.000000 taufactor-1.0.0/taufactor/cli.py
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     4781 2023-03-08 11:13:00.000000 taufactor-1.0.0/taufactor/metrics.py
--rw-rw-r--   0 isaac     (1000) isaac     (1000)    29649 2023-03-23 12:07:52.000000 taufactor-1.0.0/taufactor/taufactor.py
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     1998 2023-03-23 11:14:36.000000 taufactor-1.0.0/taufactor/utils.py
-drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-03-23 12:46:38.509391 taufactor-1.0.0/taufactor.egg-info/
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     4070 2023-03-23 12:46:38.000000 taufactor-1.0.0/taufactor.egg-info/PKG-INFO
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      730 2023-03-23 12:46:38.000000 taufactor-1.0.0/taufactor.egg-info/SOURCES.txt
--rw-rw-r--   0 isaac     (1000) isaac     (1000)        1 2023-03-23 12:46:38.000000 taufactor-1.0.0/taufactor.egg-info/dependency_links.txt
--rw-rw-r--   0 isaac     (1000) isaac     (1000)        1 2022-07-11 14:11:24.000000 taufactor-1.0.0/taufactor.egg-info/not-zip-safe
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       57 2023-03-23 12:46:38.000000 taufactor-1.0.0/taufactor.egg-info/requires.txt
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       10 2023-03-23 12:46:38.000000 taufactor-1.0.0/taufactor.egg-info/top_level.txt
-drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-03-23 12:46:38.509391 taufactor-1.0.0/tests/
--rw-rw-r--   0 isaac     (1000) isaac     (1000)       39 2021-09-02 10:12:14.000000 taufactor-1.0.0/tests/__init__.py
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      150 2023-03-08 11:13:00.000000 taufactor-1.0.0/tests/environment.yml
--rw-rw-r--   0 isaac     (1000) isaac     (1000)     8651 2023-03-23 11:00:49.000000 taufactor-1.0.0/tests/test_taufactor.py
--rw-rw-r--   0 isaac     (1000) isaac     (1000)      397 2023-03-08 11:13:00.000000 taufactor-1.0.0/tests/utils.py
+drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-07-24 09:09:42.544026 taufactor-1.1.0/
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      206 2023-03-08 11:13:00.000000 taufactor-1.1.0/AUTHORS.md
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     3087 2023-03-08 11:13:00.000000 taufactor-1.1.0/CONTRIBUTING.md
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      811 2023-07-24 09:03:37.000000 taufactor-1.1.0/HISTORY.md
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     1071 2023-03-08 11:13:00.000000 taufactor-1.1.0/LICENSE
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      258 2023-03-08 11:13:00.000000 taufactor-1.1.0/MANIFEST.in
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     4331 2023-07-24 09:09:42.544026 taufactor-1.1.0/PKG-INFO
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     2285 2023-07-24 09:00:16.000000 taufactor-1.1.0/README.md
+drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-07-24 09:09:42.544026 taufactor-1.1.0/docs/
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      610 2021-09-02 10:12:14.000000 taufactor-1.1.0/docs/Makefile
+drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-07-24 09:09:42.540026 taufactor-1.1.0/docs/_build/
+drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-07-24 09:09:42.540026 taufactor-1.1.0/docs/_build/html/
+drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-07-24 09:09:42.544026 taufactor-1.1.0/docs/_build/html/_static/
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      286 2021-09-02 12:25:22.000000 taufactor-1.1.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       90 2021-09-02 12:25:22.000000 taufactor-1.1.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       90 2021-09-02 12:25:22.000000 taufactor-1.1.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       59 2023-03-08 11:13:00.000000 taufactor-1.1.0/docs/authors.rst
+-rwxrwxr-x   0 isaac     (1000) isaac     (1000)     4825 2023-03-08 11:13:00.000000 taufactor-1.1.0/docs/conf.py
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       64 2023-03-08 11:13:00.000000 taufactor-1.1.0/docs/contributing.rst
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       58 2023-03-08 11:13:00.000000 taufactor-1.1.0/docs/history.rst
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      308 2023-07-24 09:00:16.000000 taufactor-1.1.0/docs/index.rst
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      771 2021-09-02 10:12:14.000000 taufactor-1.1.0/docs/make.bat
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       57 2023-03-08 11:13:00.000000 taufactor-1.1.0/docs/readme.rst
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)   551497 2021-09-02 10:12:14.000000 taufactor-1.1.0/docs/tau_example.png
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      614 2023-07-24 09:00:16.000000 taufactor-1.1.0/docs/taufactor.rst
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      103 2021-09-02 10:12:14.000000 taufactor-1.1.0/pyproject.toml
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      406 2023-07-24 09:09:42.544026 taufactor-1.1.0/setup.cfg
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     1949 2023-07-24 09:04:54.000000 taufactor-1.1.0/setup.py
+drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-07-24 09:09:42.544026 taufactor-1.1.0/taufactor/
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      148 2023-07-24 09:04:54.000000 taufactor-1.1.0/taufactor/__init__.py
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      405 2021-09-02 10:12:14.000000 taufactor-1.1.0/taufactor/cli.py
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     5054 2023-07-24 09:00:16.000000 taufactor-1.1.0/taufactor/metrics.py
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)    29553 2023-07-24 09:00:16.000000 taufactor-1.1.0/taufactor/taufactor.py
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     1998 2023-07-24 09:00:16.000000 taufactor-1.1.0/taufactor/utils.py
+drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-07-24 09:09:42.544026 taufactor-1.1.0/taufactor.egg-info/
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     4331 2023-07-24 09:09:42.000000 taufactor-1.1.0/taufactor.egg-info/PKG-INFO
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      749 2023-07-24 09:09:42.000000 taufactor-1.1.0/taufactor.egg-info/SOURCES.txt
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)        1 2023-07-24 09:09:42.000000 taufactor-1.1.0/taufactor.egg-info/dependency_links.txt
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)        1 2022-07-11 14:11:24.000000 taufactor-1.1.0/taufactor.egg-info/not-zip-safe
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       57 2023-07-24 09:09:42.000000 taufactor-1.1.0/taufactor.egg-info/requires.txt
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       10 2023-07-24 09:09:42.000000 taufactor-1.1.0/taufactor.egg-info/top_level.txt
+drwxrwxr-x   0 isaac     (1000) isaac     (1000)        0 2023-07-24 09:09:42.544026 taufactor-1.1.0/tests/
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)       39 2021-09-02 10:12:14.000000 taufactor-1.1.0/tests/__init__.py
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      150 2023-03-08 11:13:00.000000 taufactor-1.1.0/tests/environment.yml
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)     9485 2023-07-24 09:00:16.000000 taufactor-1.1.0/tests/test_taufactor.py
+-rw-rw-r--   0 isaac     (1000) isaac     (1000)      397 2023-03-08 11:13:00.000000 taufactor-1.1.0/tests/utils.py
```

### Comparing `taufactor-1.0.0/CONTRIBUTING.md` & `taufactor-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `taufactor-1.0.0/HISTORY.md` & `taufactor-1.1.0/HISTORY.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # History
 
+## 1.1.0 (2023-07-24)
+
+---
+
+-   Added comments from reviewers
+-   Added examples to documentation
+-   Added API documentation
+-   Fix test times on comparison
+
 ## 1.0.0 (2023-03-23)
 
 ---
 
 -   Migrated to PyTorch from CuPy
 -   New convergence criteria
 -   New documentation style
```

### Comparing `taufactor-1.0.0/LICENSE` & `taufactor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taufactor-1.0.0/PKG-INFO` & `taufactor-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taufactor
-Version: 1.0.0
+Version: 1.1.0
 Summary: TauFactor is an application for calculating tortuosity factors from tomographic data
 Home-page: https://github.com/tldr-group/taufactor
 Author: Isaac Squires
 Author-email: is21@ic.ac.uk
 License: MIT license
 Keywords: taufactor
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,16 @@
 Classifier: Environment :: GPU
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # TauFactor
 
@@ -106,14 +108,23 @@
 ## TauFactor MATLAB
 
 The package in this repository refers to a Python implementation of the TauFactor solver. There is a deprecated [MATLAB implementation](https://www.mathworks.com/matlabcentral/fileexchange/57956-taufactor), which is no longer maintained.
 
 
 # History
 
+## 1.1.0 (2023-07-24)
+
+---
+
+-   Added comments from reviewers
+-   Added examples to documentation
+-   Added API documentation
+-   Fix test times on comparison
+
 ## 1.0.0 (2023-03-23)
 
 ---
 
 -   Migrated to PyTorch from CuPy
 -   New convergence criteria
 -   New documentation style
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: taufactor Version: 1.0.0 Summary: TauFactor is an
+Metadata-Version: 2.1 Name: taufactor Version: 1.1.0 Summary: TauFactor is an
 application for calculating tortuosity factors from tomographic data Home-page:
 https://github.com/tldr-group/taufactor Author: Isaac Squires Author-email:
 is21@ic.ac.uk License: MIT license Keywords: taufactor Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing Classifier: Topic :: Scientific/
 Engineering :: Physics Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Image Processing Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Environment :: GPU Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Requires-Python: >=3.5 Description-Content-Type:
-text/markdown License-File: LICENSE License-File: AUTHORS.md # TauFactor
-TauFactor is an application for calculating tortuosity factors from tomographic
-data. - Free software: MIT license - Documentation: [https://
-taufactor.readthedocs.io](https://taufactor.readthedocs.io).
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.5
+Description-Content-Type: text/markdown License-File: LICENSE License-File:
+AUTHORS.md # TauFactor TauFactor is an application for calculating tortuosity
+factors from tomographic data. - Free software: MIT license - Documentation:
+[https://taufactor.readthedocs.io](https://taufactor.readthedocs.io).
                                   [TauFactor]
               [PyPI] [ReadTheDocs] [MIT_LICENSE] [github actions]
 ## Requirements Before installing taufactor, [download the most recent version
 of PyTorch](https://pytorch.org/get-started/locally/). Ensure you have
 `pytorch>=1.10` installed in your Python environment. For example, for a Linux
 machine with CUDA GPU ``` conda install pytorch pytorch-cuda=11.7 -c pytorch -
 c nvidia ``` ## Quickstart To install TauFactor via PyPI ``` pip install
@@ -31,15 +32,17 @@
 (s.D_eff, s.tau) ``` ## Tests To run unit tests navigate to the root directory
 and run ``` pytest ``` ## Credits This package was created by the [tldr group]
 (https://tldr-group.github.io/) at the Dyson School of Design Engineering,
 Imperial College London. ## TauFactor MATLAB The package in this repository
 refers to a Python implementation of the TauFactor solver. There is a
 deprecated [MATLAB implementation](https://www.mathworks.com/matlabcentral/
 fileexchange/57956-taufactor), which is no longer maintained. # History ##
-1.0.0 (2023-03-23) --- - Migrated to PyTorch from CuPy - New convergence
-criteria - New documentation style - CI testing - Includes TauFactor paper ##
-0.1.4 (2022-07-11) --- - Add TauE solver - Add triple phase boundary
-calculations - Fix cuboids not converging - Fix convergence messaging ## 0.1.3
-(2021-03-25) --- - Hotfix code in taufactor.py ## 0.1.2 (2021-03-25) --- -
-Added multi-phase and periodic solvers and metrics calculations ## 0.1.1 (2021-
-02-10) --- - Removed CuPy from requirements and added installation instructions
-to README ## 0.1.0 (2021-02-08) --- - First release on PyPI.
+1.1.0 (2023-07-24) --- - Added comments from reviewers - Added examples to
+documentation - Added API documentation - Fix test times on comparison ## 1.0.0
+(2023-03-23) --- - Migrated to PyTorch from CuPy - New convergence criteria -
+New documentation style - CI testing - Includes TauFactor paper ## 0.1.4 (2022-
+07-11) --- - Add TauE solver - Add triple phase boundary calculations - Fix
+cuboids not converging - Fix convergence messaging ## 0.1.3 (2021-03-25) --- -
+Hotfix code in taufactor.py ## 0.1.2 (2021-03-25) --- - Added multi-phase and
+periodic solvers and metrics calculations ## 0.1.1 (2021-02-10) --- - Removed
+CuPy from requirements and added installation instructions to README ## 0.1.0
+(2021-02-08) --- - First release on PyPI.
```

### Comparing `taufactor-1.0.0/README.md` & `taufactor-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `taufactor-1.0.0/docs/Makefile` & `taufactor-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `taufactor-1.0.0/docs/conf.py` & `taufactor-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `taufactor-1.0.0/docs/make.bat` & `taufactor-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `taufactor-1.0.0/docs/tau_example.png` & `taufactor-1.1.0/docs/tau_example.png`

 * *Files identical despite different names*

### Comparing `taufactor-1.0.0/setup.py` & `taufactor-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,24 +32,26 @@
         'Environment :: GPU',
         'Environment :: GPU :: NVIDIA CUDA',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     description="TauFactor is an application for calculating tortuosity factors from tomographic data",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='taufactor',
     name='taufactor',
     packages=find_packages(include=['taufactor', 'taufactor.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/tldr-group/taufactor',
-    version='1.0.0',
+    version='1.1.0',
     zip_safe=False,
 )
```

### Comparing `taufactor-1.0.0/taufactor/metrics.py` & `taufactor-1.1.0/taufactor/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         periodic.reverse()
     else:
         img = F.pad(img, (1,)*dim*2, 'constant', value=int_not_in_img)
         periodic=[0]*dim
 
     SA_map = torch.zeros_like(img)
     if not isinstance(phases, list):
-        phases = [phases]
+        raise TypeError('phases should be a list')
     for i in range(dim):
         for j in [1, -1]:
             i_rolled = torch.roll(img, j, i)
             if len(phases)==2:
                 SA_map[(i_rolled == phases[0]) & (img == phases[1])] += 1
             else:
                 SA_map[(i_rolled == phases[0]) & (img != phases[0])] += 1
@@ -82,14 +82,21 @@
         total_faces = 2*(x+1)*(y+1)-(x+1)-(y+1)-2*sf
     else:
         total_faces=SA_map.size
     sa = torch.sum(SA_map)/total_faces
     return sa
 
 def triple_phase_boundary(img):
+    """Calculate triple phase boundary density i.e. fraction of voxel verticies that touch at least 3 phases
+
+    Args:
+        img (numpy array): image to calculate metric on     
+    Returns:
+        float: triple phase boundary density 
+    """
     phases = torch.unique(torch.tensor(img))
     if len(phases)!=3:
         raise ValueError('Image must have exactly 3 phases')
     shape = img.shape
     dim = len(shape)
     ph_maps = []
     img = F.pad(torch.tensor(img), (1,)*dim*2, 'constant', value=-1)
```

### Comparing `taufactor-1.0.0/taufactor/taufactor.py` & `taufactor-1.1.0/taufactor/taufactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
     def __init__(self, img, bc=(-0.5, 0.5), D_0=1, device=torch.device('cuda')):
         """
         Initialise parameters, conc map and other tools that can be re-used
         for multiple solves.
 
         :param img: input img with 1s conductive and 0s non-conductive
-        :param precision:  cp.single or cp.double
         :param bc: Upper and lower boundary conditions. Leave as default.
         :param D_0: reference material diffusivity
         :param device: pytorch device, can be cuda or cpu 
         """
         # add batch dim now for consistency
         self.D_0 = D_0
         self.top_bc, self.bot_bc = bc
@@ -162,20 +161,24 @@
             self.end_simulation(iter_limit, verbose, start)
             return self.tau
 
     def check_convergence(self, verbose, conv_crit, start, iter_limit):
         # print progress
         self.semi_converged, self.new_fl, err = self.check_vertical_flux(
             conv_crit)
-        self.D_rel = ((self.new_fl) * self.L_A /
-                      abs(self.top_bc - self.bot_bc)).cpu()
-        self.tau = self.VF / \
-            self.D_rel if self.D_rel != 0 else torch.tensor(torch.inf)
         if self.semi_converged == 'zero_flux':
+            self.D_rel = 0
+            self.tau = np.inf
             return True
+        else:
+            self.D_rel = ((self.new_fl) * self.L_A /
+                        abs(self.top_bc - self.bot_bc)).cpu()
+            self.tau = self.VF / \
+                self.D_rel if self.D_rel != 0 else torch.tensor(torch.inf)
+        
 
         if verbose == 'per_iter':
             print(
                 f'Iter: {self.iter}, conv error: {abs(err.item())}, tau: {self.tau.item()}')
 
         if self.semi_converged:
             self.converged = self.check_rolling_mean(conv_crit=1e-3)
@@ -192,18 +195,18 @@
     def check_vertical_flux(self, conv_crit):
         vert_flux = self.conc[:, 1:-1, 1:-1, 1:-1] - \
             self.conc[:, :-2, 1:-1, 1:-1]
         vert_flux[self.conc[:, :-2, 1:-1, 1:-1] == 0] = 0
         vert_flux[self.conc[:, 1:-1, 1:-1, 1:-1] == 0] = 0
         fl = torch.sum(vert_flux, (0, 2, 3))[1:-1]
         err = (fl.max() - fl.min())*2/(fl.max() + fl.min())
-        if err < conv_crit or torch.isnan(err).item():
-            return True, torch.mean(fl), err
         if fl.min() == 0:
             return 'zero_flux', torch.mean(fl), err
+        if err < conv_crit or torch.isnan(err).item():
+            return True, torch.mean(fl), err
         return False, torch.mean(fl), err
 
     def check_rolling_mean(self, conv_crit):
         err = (self.new_fl - self.old_fl) / (self.new_fl + self.old_fl)
         if err < conv_crit:
             return True
         else:
@@ -229,15 +232,14 @@
 
     def __init__(self, img, bc=(-0.5, 0.5), D_0=1, device=torch.device('cuda:0')):
         """
         Initialise parameters, conc map and other tools that can be re-used
         for multiple solves.
 
         :param img: input img with 1s conductive and 0s non-conductive
-        :param precision:  cp.single or cp.double
         :param bc: Upper and lower boundary conditions. Leave as default.
         :param D_0: reference material diffusivity
 
         """
         super().__init__(img, bc, D_0, device)
         self.conc = self.pad(self.conc)[:, :, 2:-2, 2:-2].to(self.device)
 
@@ -309,15 +311,14 @@
         """
         Initialise parameters, conc map and other tools that can be re-used
         for multiple solves.
 
         :param img: input img with n conductive phases labelled as integers, and 0s for non-conductive
         :param cond: dict with n phase labels as keys, and their corresponding conductivities as values e.g
         for a 2 phase material, {1:0.543, 2: 0.420}, with 1s and 2s in the input img
-        :param precision:  cp.single or cp.double
         :param bc: Upper and lower boundary conditions. Leave as default.
         """
 
         if (0 in cond.values()):
             raise ValueError(
                 '0 conductivity phase: non-conductive phase should be labelled 0 in the input image and ommitted from the cond argument')
         if (0 in cond.keys()):
@@ -491,15 +492,14 @@
         return False
 
     def check_vertical_flux(self, conv_crit):
         vert_flux = (self.conc[:, 1:-1, 1:-1, 1:-1] - self.conc[:,
                      :-2, 1:-1, 1:-1]) * self.pre_factors[1][:, :-2, 1:-1, 1:-1]
         vert_flux[self.nn == torch.inf] = 0
         fl = torch.sum(vert_flux, (0, 2, 3))[2:-2]
-        print(fl.argmin(), fl.argmax())
         err = (fl.max() - fl.min())*2/(fl.max() + fl.min())
         if err < conv_crit or torch.isnan(err).item():
             return True, torch.mean(fl), err
         if fl.min() == 0:
             return 'zero_flux', torch.mean(fl), err
         return False, torch.mean(fl), err
```

### Comparing `taufactor-1.0.0/taufactor/utils.py` & `taufactor-1.1.0/taufactor/utils.py`

 * *Files identical despite different names*

### Comparing `taufactor-1.0.0/taufactor.egg-info/PKG-INFO` & `taufactor-1.1.0/taufactor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taufactor
-Version: 1.0.0
+Version: 1.1.0
 Summary: TauFactor is an application for calculating tortuosity factors from tomographic data
 Home-page: https://github.com/tldr-group/taufactor
 Author: Isaac Squires
 Author-email: is21@ic.ac.uk
 License: MIT license
 Keywords: taufactor
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,16 @@
 Classifier: Environment :: GPU
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # TauFactor
 
@@ -106,14 +108,23 @@
 ## TauFactor MATLAB
 
 The package in this repository refers to a Python implementation of the TauFactor solver. There is a deprecated [MATLAB implementation](https://www.mathworks.com/matlabcentral/fileexchange/57956-taufactor), which is no longer maintained.
 
 
 # History
 
+## 1.1.0 (2023-07-24)
+
+---
+
+-   Added comments from reviewers
+-   Added examples to documentation
+-   Added API documentation
+-   Fix test times on comparison
+
 ## 1.0.0 (2023-03-23)
 
 ---
 
 -   Migrated to PyTorch from CuPy
 -   New convergence criteria
 -   New documentation style
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: taufactor Version: 1.0.0 Summary: TauFactor is an
+Metadata-Version: 2.1 Name: taufactor Version: 1.1.0 Summary: TauFactor is an
 application for calculating tortuosity factors from tomographic data Home-page:
 https://github.com/tldr-group/taufactor Author: Isaac Squires Author-email:
 is21@ic.ac.uk License: MIT license Keywords: taufactor Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing Classifier: Topic :: Scientific/
 Engineering :: Physics Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Image Processing Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Environment :: GPU Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Requires-Python: >=3.5 Description-Content-Type:
-text/markdown License-File: LICENSE License-File: AUTHORS.md # TauFactor
-TauFactor is an application for calculating tortuosity factors from tomographic
-data. - Free software: MIT license - Documentation: [https://
-taufactor.readthedocs.io](https://taufactor.readthedocs.io).
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.5
+Description-Content-Type: text/markdown License-File: LICENSE License-File:
+AUTHORS.md # TauFactor TauFactor is an application for calculating tortuosity
+factors from tomographic data. - Free software: MIT license - Documentation:
+[https://taufactor.readthedocs.io](https://taufactor.readthedocs.io).
                                   [TauFactor]
               [PyPI] [ReadTheDocs] [MIT_LICENSE] [github actions]
 ## Requirements Before installing taufactor, [download the most recent version
 of PyTorch](https://pytorch.org/get-started/locally/). Ensure you have
 `pytorch>=1.10` installed in your Python environment. For example, for a Linux
 machine with CUDA GPU ``` conda install pytorch pytorch-cuda=11.7 -c pytorch -
 c nvidia ``` ## Quickstart To install TauFactor via PyPI ``` pip install
@@ -31,15 +32,17 @@
 (s.D_eff, s.tau) ``` ## Tests To run unit tests navigate to the root directory
 and run ``` pytest ``` ## Credits This package was created by the [tldr group]
 (https://tldr-group.github.io/) at the Dyson School of Design Engineering,
 Imperial College London. ## TauFactor MATLAB The package in this repository
 refers to a Python implementation of the TauFactor solver. There is a
 deprecated [MATLAB implementation](https://www.mathworks.com/matlabcentral/
 fileexchange/57956-taufactor), which is no longer maintained. # History ##
-1.0.0 (2023-03-23) --- - Migrated to PyTorch from CuPy - New convergence
-criteria - New documentation style - CI testing - Includes TauFactor paper ##
-0.1.4 (2022-07-11) --- - Add TauE solver - Add triple phase boundary
-calculations - Fix cuboids not converging - Fix convergence messaging ## 0.1.3
-(2021-03-25) --- - Hotfix code in taufactor.py ## 0.1.2 (2021-03-25) --- -
-Added multi-phase and periodic solvers and metrics calculations ## 0.1.1 (2021-
-02-10) --- - Removed CuPy from requirements and added installation instructions
-to README ## 0.1.0 (2021-02-08) --- - First release on PyPI.
+1.1.0 (2023-07-24) --- - Added comments from reviewers - Added examples to
+documentation - Added API documentation - Fix test times on comparison ## 1.0.0
+(2023-03-23) --- - Migrated to PyTorch from CuPy - New convergence criteria -
+New documentation style - CI testing - Includes TauFactor paper ## 0.1.4 (2022-
+07-11) --- - Add TauE solver - Add triple phase boundary calculations - Fix
+cuboids not converging - Fix convergence messaging ## 0.1.3 (2021-03-25) --- -
+Hotfix code in taufactor.py ## 0.1.2 (2021-03-25) --- - Added multi-phase and
+periodic solvers and metrics calculations ## 0.1.1 (2021-02-10) --- - Removed
+CuPy from requirements and added installation instructions to README ## 0.1.0
+(2021-02-08) --- - First release on PyPI.
```

### Comparing `taufactor-1.0.0/taufactor.egg-info/SOURCES.txt` & `taufactor-1.1.0/taufactor.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/make.bat
 docs/readme.rst
 docs/tau_example.png
+docs/taufactor.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 taufactor/__init__.py
 taufactor/cli.py
 taufactor/metrics.py
 taufactor/taufactor.py
```

### Comparing `taufactor-1.0.0/tests/test_taufactor.py` & `taufactor-1.1.0/tests/test_taufactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 import taufactor as tau
 from taufactor.metrics import volume_fraction, surface_area, triple_phase_boundary
 import torch as pt
 from tests.utils import *
 import numpy as np
 import matplotlib.pyplot as plt
-
+import torch
 #  Testing the main solver
 
 
 def test_solver_on_uniform_block():
     """Run solver on a block of ones."""
     l = 20
     img = np.ones([l, l, l]).reshape(1, l, l, l)
@@ -59,39 +59,60 @@
     img = np.zeros([l, l, l]).reshape(1, l, l, l)
     t = 10
     img[:, :, 0:t, 0:t] = 1
     S = tau.Solver(img, device=pt.device('cpu'))
     S.solve()
     assert np.around(S.tau, decimals=5) == 1
 
+def test_solver_on_slanted_strip_of_ones():
+    """Run solver on a slanted strip of ones"""
+    l = 20
+    img = np.zeros([l, l+1, l+1]).reshape(1, l, l+1, l+1)
+    # t = 10
+    # img[:, :, 0:t, 0:t] = 1
+    for i in range(l):
+        img[:, i, i:i+2, i:i+2] = 1
+    S = tau.Solver(img, device=pt.device('cpu'))
+    S.solve()
+    assert np.around(S.tau, decimals=5) == 4
 #  Testing the periodic solver
 
 
+def test_deadend():
+    """Test deadend pore"""
+    solid  = np.zeros((10,50,50))
+    solid[:8, 25,25] = 1
+    # solve for tau
+    S = tau.Solver(solid)
+    S.solve()
+    assert np.around(S.D_eff, decimals=5) == 0
+    assert S.tau == np.inf
+
 def test_periodic_solver_on_uniform_block():
-    """Run solver on a block of ones."""
+    """Run periodic solver on a block of ones."""
     l = 20
     img = np.ones([l, l, l]).reshape(1, l, l, l)
     img[:, :, 0] = 0
     S = tau.PeriodicSolver(img, device=pt.device('cpu'))
     S.solve()
     assert np.around(S.tau, decimals=5) == 1.0
 
 
 def test_periodic_solver_on_empty_block():
-    """Run solver on a block of zeros."""
+    """Run periodic solver on a block of zeros."""
     l = 20
     img = np.zeros([l, l, l]).reshape(1, l, l, l)
     img[:, 0] = 1
     S = tau.PeriodicSolver(img, device=pt.device('cpu'))
     S.solve(verbose='per_iter', iter_limit=1000)
     assert S.tau == pt.inf
 
 
 def test_periodic_solver_on_strip_of_ones():
-    """Run solver on a strip of ones, 1/4 volume of total"""
+    """Run periodic solver on a strip of ones, 1/4 volume of total"""
     l = 20
     img = np.zeros([l, l, l]).reshape(1, l, l, l)
     t = 10
     img[:, :, 0:t, 0:t] = 1
     S = tau.PeriodicSolver(img, device=pt.device('cpu'))
     S.solve()
     assert np.around(S.tau, decimals=5) == 1
@@ -140,28 +161,27 @@
 # Surface area
 
 
 def test_surface_area_on_uniform_block():
     """Run surface area on uniform block"""
     l = 20
     img = np.ones([l, l, l])
-    sa = surface_area(img, phases=1)
+    sa = surface_area(img, phases=[1])
 
     assert sa == 0
 
 
 def test_surface_area_on_empty_block():
     """Run surface area on empty block"""
     l = 20
     img = np.zeros([l, l, l])
-    sa = surface_area(img, phases=0)
+    sa = surface_area(img, phases=[0])
 
     assert sa == 0
 
-
 def test_surface_area_on_checkerboard():
     """Run surface area on checkerboard block"""
     l = 50
     img = generate_checkerboard(l)
     sa = surface_area(img, phases=[0, 1])
 
     assert sa == 1
@@ -191,52 +211,59 @@
     img = np.array([[0, 0, 0], [1, 1, 0], [0, 0, 0]])
     sa = surface_area(img, phases=[0, 1], periodic=[0, 1])
 
     assert sa == 6/18
 
 
 def test_surface_area_interfactial_3ph():
+    """Run surface area 3 phases """
     l = 3
     img = np.zeros([l, l, l])
     img[1] = 1
     img[2] = 2
     sa = surface_area(img, phases=[1, 2])
     assert sa == 1/6
 
 
 def test_tpb_2d():
+    """Run tpb on 3x3"""
     l = 3
     img = np.zeros([l, l])
     img[0] = 1
     img[:, 0] = 2
     tpb = triple_phase_boundary(img)
     assert tpb == 0.25
 
 
 def test_tpb_3d_corners():
+    """Run tpb on 2x2"""
+
     l = 2
     img = np.zeros([l, l, l])
     img[0, 0, 0] = 1
     img[1, 1, 1] = 1
     img[0, 1, 1] = 2
     img[1, 0, 0] = 2
     tpb = triple_phase_boundary(img)
     assert tpb == 1
 
 
 def test_tpb_3d_corners():
+    """Run tpb on 2x2 corners"""
+
     l = 2
     img = np.zeros([l, l, l])
     img[0] = 1
     img[:, 0] = 2
     tpb = triple_phase_boundary(img)
     assert tpb == 1/3
 
 
 def test_multiphase_and_solver_agree():
+    """test mph and solver agree when Ds are the same"""
     x = 100
     img = np.ones([x, x, x])
     img[50:] = 2
     img[:, :20] = 0
     img[:, 50:] = 1
     s = tau.MultiPhaseSolver(img, {1: 1, 2: 1*10**-4}, device=pt.device('cpu'))
     mph = s.solve(verbose='per_iter', conv_crit=0.02)
@@ -246,44 +273,44 @@
 
     err = (mph-s.tau)
 
     assert err < 0.02
 
 
 def test_mphsolver_on_empty_block():
-    """Run solver on a block of zeros."""
+    """Run mpsolver on a block of zeros."""
     l = 20
     img = np.zeros([l, l, l]).reshape(1, l, l, l)
     S = tau.MultiPhaseSolver(img, device=pt.device('cpu'))
     S.solve(iter_limit=1000)
     assert S.tau == pt.inf
 
 
 def test_mphsolver_on_ones_block():
-    """Run solver on a block of ones."""
+    """Run mpsolver on a block of ones."""
     l = 20
     img = np.ones([l, l, l]).reshape(1, l, l, l)
     S = tau.MultiPhaseSolver(img, device=pt.device('cpu'))
     S.solve(iter_limit=1000)
     assert np.around(S.tau, 4) == 1.0
 
 
 def test_mphsolver_on_halves():
-    """Run solver on a block of halves."""
+    """Run mpsolver on a block of halves."""
     l = 20
     img = np.ones([l, l, l]).reshape(1, l, l, l)
     cond = 0.5
     S = tau.MultiPhaseSolver(img, {1: cond}, device=pt.device('cpu'))
     S.solve(iter_limit=1000)
     print(S.D_eff, S.D_mean)
     assert np.around(S.tau, 4) == 1.0
 
 
 def test_mphsolver_on_strip_of_ones():
-    """Run solver on a strip of ones, 1/4 volume of total"""
+    """Run mpsolver on a strip of ones, 1/4 volume of total"""
     l = 20
     img = np.zeros([l, l, l]).reshape(1, l, l, l)
     x = 10
     img[:, :, 0:x, 0:x] = 1
     S = tau.MultiPhaseSolver(img, device=pt.device('cpu'))
     S.solve()
     assert np.around(S.tau, 4) == 1.0
@@ -312,27 +339,27 @@
     cond = {1: 1, 2: 0.5, 3: 2}
     S = tau.MultiPhaseSolver(img, cond, device=pt.device('cpu'))
     S.solve()
     assert np.around(S.tau, 4) == 1
 
 
 def test_taue_deadend():
-    """Run solver on a strip of ones, 1/4 volume of total"""
+    """Run solver on a deadend strip of ones"""
 
     l = 100
     img = np.zeros((l, l))
     img[:75, 45:55] = 1
     img[img != 1] = 0
     esolver = tau.ElectrodeSolver(img, device=pt.device('cpu'))
     esolver.solve()
     assert np.around(esolver.tau_e, 3) == 0.601
 
 
 def test_taue_throughpore():
-    """Run solver on a strip of ones, 1/4 volume of total"""
+    """Run taue solver on a strip of ones, 1/4 volume of total"""
 
     l = 100
     img = np.zeros((l, l))
     img[:, 45:55] = 1
     img[img != 1] = 0
     esolver = tau.ElectrodeSolver(img, device=pt.device('cpu'))
     esolver.solve()
```

