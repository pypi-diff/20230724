# Comparing `tmp/BiocPy-0.2.1.tar.gz` & `tmp/BiocPy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BiocPy-0.2.1.tar", last modified: Fri Jan 20 21:48:04 2023, max compression
+gzip compressed data, was "BiocPy-0.2.2.tar", last modified: Mon Jul 24 05:00:06 2023, max compression
```

## Comparing `BiocPy-0.2.1.tar` & `BiocPy-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.889261 BiocPy-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-20 21:46:19.000000 BiocPy-0.2.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.877261 BiocPy-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.881261 BiocPy-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-01-20 21:46:19.000000 BiocPy-0.2.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-20 21:46:19.000000 BiocPy-0.2.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-20 21:46:19.000000 BiocPy-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-20 21:46:19.000000 BiocPy-0.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-20 21:46:19.000000 BiocPy-0.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-20 21:46:19.000000 BiocPy-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-01-20 21:46:19.000000 BiocPy-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-20 21:46:19.000000 BiocPy-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-01-20 21:48:04.889261 BiocPy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-20 21:46:19.000000 BiocPy-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.885261 BiocPy-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.885261 BiocPy-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-20 21:46:19.000000 BiocPy-0.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-01-20 21:46:19.000000 BiocPy-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-01-20 21:48:04.889261 BiocPy-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-20 21:46:19.000000 BiocPy-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.877261 BiocPy-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.885261 BiocPy-0.2.1/src/BiocPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-01-20 21:48:04.000000 BiocPy-0.2.1/src/BiocPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-01-20 21:48:04.000000 BiocPy-0.2.1/src/BiocPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 21:48:04.000000 BiocPy-0.2.1/src/BiocPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 21:46:29.000000 BiocPy-0.2.1/src/BiocPy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-20 21:48:04.000000 BiocPy-0.2.1/src/BiocPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-20 21:48:04.000000 BiocPy-0.2.1/src/BiocPy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.885261 BiocPy-0.2.1/src/biocpy/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-20 21:46:19.000000 BiocPy-0.2.1/src/biocpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.889261 BiocPy-0.2.1/src/biocpy/genomicranges/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-20 21:46:19.000000 BiocPy-0.2.1/src/biocpy/genomicranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.889261 BiocPy-0.2.1/src/biocpy/multiassayexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-20 21:46:19.000000 BiocPy-0.2.1/src/biocpy/multiassayexperiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.889261 BiocPy-0.2.1/src/biocpy/singlecellexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-20 21:46:19.000000 BiocPy-0.2.1/src/biocpy/singlecellexperiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.889261 BiocPy-0.2.1/src/biocpy/summarizedexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-01-20 21:46:19.000000 BiocPy-0.2.1/src/biocpy/summarizedexperiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 21:48:04.889261 BiocPy-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-20 21:46:19.000000 BiocPy-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-20 21:46:19.000000 BiocPy-0.2.1/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-01-20 21:46:19.000000 BiocPy-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-24 04:58:18.000000 BiocPy-0.2.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.543683 BiocPy-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.547684 BiocPy-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-24 04:58:18.000000 BiocPy-0.2.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 04:58:18.000000 BiocPy-0.2.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-24 04:58:18.000000 BiocPy-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-24 04:58:18.000000 BiocPy-0.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 04:58:18.000000 BiocPy-0.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 04:58:18.000000 BiocPy-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-24 04:58:18.000000 BiocPy-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 04:58:18.000000 BiocPy-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-24 05:00:06.551684 BiocPy-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-24 04:58:18.000000 BiocPy-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.547684 BiocPy-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-24 04:58:18.000000 BiocPy-0.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-24 04:58:18.000000 BiocPy-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 05:00:06.551684 BiocPy-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-24 04:58:18.000000 BiocPy-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.543683 BiocPy-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/src/BiocPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-24 05:00:06.000000 BiocPy-0.2.2/src/BiocPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-24 05:00:06.000000 BiocPy-0.2.2/src/BiocPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:00:06.000000 BiocPy-0.2.2/src/BiocPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 04:58:32.000000 BiocPy-0.2.2/src/BiocPy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-24 05:00:06.000000 BiocPy-0.2.2/src/BiocPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 05:00:06.000000 BiocPy-0.2.2/src/BiocPy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/src/biocpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-24 04:58:18.000000 BiocPy-0.2.2/src/biocpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/src/biocpy/genomicranges/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-24 04:58:18.000000 BiocPy-0.2.2/src/biocpy/genomicranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/src/biocpy/multiassayexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 04:58:18.000000 BiocPy-0.2.2/src/biocpy/multiassayexperiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/src/biocpy/singlecellexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 04:58:18.000000 BiocPy-0.2.2/src/biocpy/singlecellexperiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/src/biocpy/summarizedexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 04:58:18.000000 BiocPy-0.2.2/src/biocpy/summarizedexperiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:00:06.551684 BiocPy-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 04:58:18.000000 BiocPy-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-24 04:58:18.000000 BiocPy-0.2.2/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-24 04:58:18.000000 BiocPy-0.2.2/tox.ini
```

### Comparing `BiocPy-0.2.1/.coveragerc` & `BiocPy-0.2.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/.github/workflows/pypi-publish.yml` & `BiocPy-0.2.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/.github/workflows/pypi-test.yml` & `BiocPy-0.2.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/.gitignore` & `BiocPy-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/CONTRIBUTING.rst` & `BiocPy-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/LICENSE.txt` & `BiocPy-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/PKG-INFO` & `BiocPy-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiocPy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interface to all [BiocPy](https://github.com/BiocPy) packages
 Home-page: https://github.com/BiocPy/BiocPy
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/BiocPy
 Platform: any
```

### Comparing `BiocPy-0.2.1/README.md` & `BiocPy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/docs/Makefile` & `BiocPy-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/docs/conf.py` & `BiocPy-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/docs/index.md` & `BiocPy-0.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/docs/readme.md` & `BiocPy-0.2.2/docs/readme.md`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/setup.cfg` & `BiocPy-0.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	biocframe
 	genomicranges
 	summarizedexperiment
 	singlecellexperiment
 	multiassayexperiment
+	rds2py
 	mopsy
 	pybiocfilecache
 	numpy
 	scipy
 	pandas
 
 [options.packages.find]
```

### Comparing `BiocPy-0.2.1/setup.py` & `BiocPy-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/src/BiocPy.egg-info/PKG-INFO` & `BiocPy-0.2.2/src/BiocPy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiocPy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interface to all [BiocPy](https://github.com/BiocPy) packages
 Home-page: https://github.com/BiocPy/BiocPy
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/BiocPy
 Platform: any
```

### Comparing `BiocPy-0.2.1/src/BiocPy.egg-info/SOURCES.txt` & `BiocPy-0.2.2/src/BiocPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BiocPy-0.2.1/src/biocpy/__init__.py` & `BiocPy-0.2.2/src/biocpy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 
 if sys.version_info[:2] >= (3, 8):
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import (
         PackageNotFoundError,
         version,
-    )  # pragma: no cover
+    )
 else:
     from importlib_metadata import (
         PackageNotFoundError,
         version,
-    )  # pragma: no cover
+    )
 
 try:
     # Change here if project is renamed and does not equal the package name
     dist_name = "BiocPy"
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
```

### Comparing `BiocPy-0.2.1/tox.ini` & `BiocPy-0.2.2/tox.ini`

 * *Files identical despite different names*

