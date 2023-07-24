# Comparing `tmp/CKAstroTools-0.0.6.tar.gz` & `tmp/ckastrotools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CKAstroTools-0.0.6.tar", last modified: Sat Jun 24 05:44:42 2023, max compression
+gzip compressed data, was "ckastrotools-0.0.7.tar", last modified: Mon Jul 24 18:44:34 2023, max compression
```

## Comparing `CKAstroTools-0.0.6.tar` & `ckastrotools-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.340756 CKAstroTools-0.0.6/
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/CKAstroTools.egg-info/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1476 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      443 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/SOURCES.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/dependency_links.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/requires.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/top_level.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.6/LICENSE
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1476 2023-06-24 05:44:42.340756 CKAstroTools-0.0.6/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      874 2023-06-22 09:22:37.000000 CKAstroTools-0.0.6/README.md
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/ckastrotools/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       33 2023-06-23 04:41:23.000000 CKAstroTools-0.0.6/ckastrotools/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.6/ckastrotools/__main__.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/ckastrotools/io/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       36 2023-06-23 04:40:16.000000 CKAstroTools-0.0.6/ckastrotools/io/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1319 2023-06-23 04:43:12.000000 CKAstroTools-0.0.6/ckastrotools/io/subcube.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/ckastrotools/milkyway/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       49 2023-06-23 04:37:12.000000 CKAstroTools-0.0.6/ckastrotools/milkyway/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      835 2023-06-24 05:41:45.000000 CKAstroTools-0.0.6/ckastrotools/milkyway/galactic_bar.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)    17778 2023-06-23 04:38:15.000000 CKAstroTools-0.0.6/ckastrotools/milkyway/spiralarms.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-24 05:43:35.000000 CKAstroTools-0.0.6/pyproject.toml
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-24 05:44:42.340756 CKAstroTools-0.0.6/setup.cfg
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/tests/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.6/tests/test_main.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-07-24 18:44:34.510244 ckastrotools-0.0.7/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 ckastrotools-0.0.7/LICENSE
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1470 2023-07-24 18:44:34.510244 ckastrotools-0.0.7/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      869 2023-07-24 18:43:30.000000 ckastrotools-0.0.7/README.md
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-07-24 18:44:34.506244 ckastrotools-0.0.7/ckastrotools/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       33 2023-06-23 04:41:23.000000 ckastrotools-0.0.7/ckastrotools/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 ckastrotools-0.0.7/ckastrotools/__main__.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-07-24 18:44:34.510244 ckastrotools-0.0.7/ckastrotools/io/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       37 2023-06-25 04:09:24.000000 ckastrotools-0.0.7/ckastrotools/io/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1319 2023-06-23 04:43:12.000000 ckastrotools-0.0.7/ckastrotools/io/subcube.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-07-24 18:44:34.510244 ckastrotools-0.0.7/ckastrotools/milkyway/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       49 2023-06-23 04:37:12.000000 ckastrotools-0.0.7/ckastrotools/milkyway/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     5092 2023-07-24 18:12:39.000000 ckastrotools-0.0.7/ckastrotools/milkyway/coordinates.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      924 2023-07-24 18:07:18.000000 ckastrotools-0.0.7/ckastrotools/milkyway/galactic_bar.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)    17997 2023-06-25 04:07:31.000000 ckastrotools-0.0.7/ckastrotools/milkyway/spiralarms.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-07-24 18:44:34.510244 ckastrotools-0.0.7/ckastrotools.egg-info/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1470 2023-07-24 18:44:34.000000 ckastrotools-0.0.7/ckastrotools.egg-info/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      480 2023-07-24 18:44:34.000000 ckastrotools-0.0.7/ckastrotools.egg-info/SOURCES.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-07-24 18:44:34.000000 ckastrotools-0.0.7/ckastrotools.egg-info/dependency_links.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-07-24 18:44:34.000000 ckastrotools-0.0.7/ckastrotools.egg-info/requires.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-07-24 18:44:34.000000 ckastrotools-0.0.7/ckastrotools.egg-info/top_level.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      822 2023-07-24 18:41:32.000000 ckastrotools-0.0.7/pyproject.toml
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-07-24 18:44:34.510244 ckastrotools-0.0.7/setup.cfg
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-07-24 18:44:34.510244 ckastrotools-0.0.7/tests/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 ckastrotools-0.0.7/tests/test_main.py
```

### Comparing `CKAstroTools-0.0.6/CKAstroTools.egg-info/PKG-INFO` & `ckastrotools-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: CKAstroTools
-Version: 0.0.6
-Summary: General toolks for astronomy I personally use regularly for data analysis.
+Name: ckastrotools
+Version: 0.0.7
+Summary: General tools for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
@@ -18,15 +18,15 @@
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
 **Repository:** https://gitlab.com/ck2go/ckastrotools \
-**PyPi:** https://test.pypi.org/project/CKAstroTools/ \
+**PyPi:** https://pypi.org/project/CKAstroTools/ \
 **Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.6/LICENSE` & `ckastrotools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.6/PKG-INFO` & `ckastrotools-0.0.7/ckastrotools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: CKAstroTools
-Version: 0.0.6
-Summary: General toolks for astronomy I personally use regularly for data analysis.
+Name: ckastrotools
+Version: 0.0.7
+Summary: General tools for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
@@ -18,15 +18,15 @@
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
 **Repository:** https://gitlab.com/ck2go/ckastrotools \
-**PyPi:** https://test.pypi.org/project/CKAstroTools/ \
+**PyPi:** https://pypi.org/project/CKAstroTools/ \
 **Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.6/README.md` & `ckastrotools-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
 **Repository:** https://gitlab.com/ck2go/ckastrotools \
-**PyPi:** https://test.pypi.org/project/CKAstroTools/ \
+**PyPi:** https://pypi.org/project/CKAstroTools/ \
 **Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.6/ckastrotools/io/subcube.py` & `ckastrotools-0.0.7/ckastrotools/io/subcube.py`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.6/ckastrotools/milkyway/spiralarms.py` & `ckastrotools-0.0.7/ckastrotools/milkyway/spiralarms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Module for the spiral arms of the Milky Way."""
 
 import numpy as np
 from astropy.coordinates import SkyCoord
+from astropy.coordinates import Galactocentric
 from astropy import units as u
+from typing import Optional
 
 
 def _getSpiralParameters(model):
     # Spiral arm params from Reid et al. (2014)
     reid2014 = {'perseus': {'R_ref': 9.9,  # kpc
                             'beta_ref': 14.2,  # deg (from Galactic center to sun =0)
                             'beta_min': -160.0,  # deg
@@ -219,18 +221,18 @@
         spiral_arm_params = vallee2015
     elif model == 'ck2021':
         spiral_arm_params = ck2021
 
     return spiral_arm_params
 
 
-def getSpiralArm(name, model='reid2014',
-                 glon_min=-np.inf, glon_max=np.inf,
-                 r_gal_min=0., r_gal_max=np.inf,
-                 resolution=0.0001, R_0=8.34):
+def getSpiralArm(name:str, model:str='reid2014',
+                 glon_min:Optional[float]=-np.inf, glon_max:Optional[float]=np.inf,
+                 r_gal_min:Optional[float]=0., r_gal_max:Optional[float]=np.inf,
+                 resolution:Optional[float]=0.0001, R_0:Optional[float]=8.34) -> Galactocentric:
     """
     Get the spiral arm model for a given arm name.
 
     Parameters
     ----------
     name: str
         Name of the spiral arm.
@@ -342,15 +344,15 @@
     # per_x = list(pckx) + list(pvx2) + list(px) + list(pvx)
     # per_y = list(pcky) + list(pvy2) + list(py) + list(pvy)
     perseus = getSpiralArm('perseus', model=model)
 
     return sagittarius, scutum, outer, perseus
 
 
-def getSpiralArms(model='reid2014'):
+def getSpiralArms(model:Optional[str]='reid2014') -> dict:
     """
     Returns the spiral arms in a dictionary.
 
     Parameters
     ----------
     model: str
         The model to use
```

### Comparing `CKAstroTools-0.0.6/pyproject.toml` & `ckastrotools-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools",
             "pytest",
             "pytest-mock"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "CKAstroTools"
-description = "General toolks for astronomy I personally use regularly for data analysis."
-version = "0.0.6"
+name = "ckastrotools"
+description = "General tools for astronomy I personally use regularly for data analysis."
+version = "0.0.7"
 requires-python = ">=3.7"
 dependencies = ["spectral-cube"]
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -24,10 +24,7 @@
 authors = [{name="Carsten König"}]
 
 [project.urls]
 Homepage = "https://gitlab.com/ck2go/ckastrotools"
 
 #[project.scripts]
 #myscript = "ckastrotools.__main__:main"
-
-
-
```

