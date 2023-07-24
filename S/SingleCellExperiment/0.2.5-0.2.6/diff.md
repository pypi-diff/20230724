# Comparing `tmp/SingleCellExperiment-0.2.5.tar.gz` & `tmp/SingleCellExperiment-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SingleCellExperiment-0.2.5.tar", last modified: Fri Mar 24 05:19:45 2023, max compression
+gzip compressed data, was "SingleCellExperiment-0.2.6.tar", last modified: Mon Jul 24 06:52:44 2023, max compression
```

## Comparing `SingleCellExperiment-0.2.5.tar` & `SingleCellExperiment-0.2.6.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.584852 SingleCellExperiment-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.568851 SingleCellExperiment-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.572851 SingleCellExperiment-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-24 05:19:45.584852 SingleCellExperiment-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.580851 SingleCellExperiment-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.580851 SingleCellExperiment-0.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-24 05:19:45.584852 SingleCellExperiment-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.568851 SingleCellExperiment-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.580851 SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-24 05:19:45.000000 SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-24 05:19:45.000000 SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 05:19:45.000000 SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 05:18:29.000000 SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-24 05:19:45.000000 SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-24 05:19:45.000000 SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.580851 SingleCellExperiment-0.2.5/src/singlecellexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/src/singlecellexperiment/SingleCellExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/src/singlecellexperiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.580851 SingleCellExperiment-0.2.5/src/singlecellexperiment/io/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/src/singlecellexperiment/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/src/singlecellexperiment/io/anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/src/singlecellexperiment/io/tenx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.580851 SingleCellExperiment-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 05:19:45.580851 SingleCellExperiment-0.2.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   311344 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/tests/data/adata.h5ad
--rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/tests/data/tenx.sub.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/tests/test_sce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/tests/test_sce_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/tests/test_sce_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/tests/test_sce_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-24 05:18:20.000000 SingleCellExperiment-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.897818 SingleCellExperiment-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.889819 SingleCellExperiment-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.889819 SingleCellExperiment-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-24 06:52:44.897818 SingleCellExperiment-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.893818 SingleCellExperiment-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.893818 SingleCellExperiment-0.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-24 06:52:44.897818 SingleCellExperiment-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.889819 SingleCellExperiment-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.893818 SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-24 06:52:44.000000 SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 06:52:44.000000 SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:52:44.000000 SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:51:24.000000 SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 06:52:44.000000 SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 06:52:44.000000 SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.893818 SingleCellExperiment-0.2.6/src/singlecellexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    17301 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/src/singlecellexperiment/SingleCellExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/src/singlecellexperiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/src/singlecellexperiment/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.893818 SingleCellExperiment-0.2.6/src/singlecellexperiment/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/src/singlecellexperiment/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/src/singlecellexperiment/io/anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/src/singlecellexperiment/io/tenx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.893818 SingleCellExperiment-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:44.897818 SingleCellExperiment-0.2.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   311344 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/tests/data/adata.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/tests/data/tenx.sub.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/tests/test_sce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/tests/test_sce_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/tests/test_sce_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/tests/test_sce_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-24 06:51:10.000000 SingleCellExperiment-0.2.6/tox.ini
```

### Comparing `SingleCellExperiment-0.2.5/.coveragerc` & `SingleCellExperiment-0.2.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/.github/workflows/pypi-publish.yml` & `SingleCellExperiment-0.2.6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/.github/workflows/pypi-test.yml` & `SingleCellExperiment-0.2.6/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/.gitignore` & `SingleCellExperiment-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/CONTRIBUTING.rst` & `SingleCellExperiment-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/LICENSE.txt` & `SingleCellExperiment-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/PKG-INFO` & `SingleCellExperiment-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SingleCellExperiment
-Version: 0.2.5
+Version: 0.2.6
 Summary: Container class for single-cell experiments
 Home-page: https://github.com/BiocPy/SingleCellExperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/SingleCellExperiment
 Platform: any
```

### Comparing `SingleCellExperiment-0.2.5/README.md` & `SingleCellExperiment-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/docs/Makefile` & `SingleCellExperiment-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/docs/conf.py` & `SingleCellExperiment-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/docs/index.md` & `SingleCellExperiment-0.2.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/docs/readme.md` & `SingleCellExperiment-0.2.6/docs/readme.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/docs/tutorial.md` & `SingleCellExperiment-0.2.6/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/setup.cfg` & `SingleCellExperiment-0.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	summarizedexperiment>=0.2.4
+	summarizedexperiment>=0.2.10
 	anndata
 	h5py
 	mudata
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `SingleCellExperiment-0.2.5/setup.py` & `SingleCellExperiment-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/PKG-INFO` & `SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SingleCellExperiment
-Version: 0.2.5
+Version: 0.2.6
 Summary: Container class for single-cell experiments
 Home-page: https://github.com/BiocPy/SingleCellExperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/SingleCellExperiment
 Platform: any
```

### Comparing `SingleCellExperiment-0.2.5/src/SingleCellExperiment.egg-info/SOURCES.txt` & `SingleCellExperiment-0.2.6/src/SingleCellExperiment.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/SingleCellExperiment.egg-info/SOURCES.txt
 src/SingleCellExperiment.egg-info/dependency_links.txt
 src/SingleCellExperiment.egg-info/not-zip-safe
 src/SingleCellExperiment.egg-info/requires.txt
 src/SingleCellExperiment.egg-info/top_level.txt
 src/singlecellexperiment/SingleCellExperiment.py
 src/singlecellexperiment/__init__.py
+src/singlecellexperiment/_types.py
 src/singlecellexperiment/io/__init__.py
 src/singlecellexperiment/io/anndata.py
 src/singlecellexperiment/io/tenx.py
 tests/conftest.py
 tests/test_sce.py
 tests/test_sce_io.py
 tests/test_sce_methods.py
```

### Comparing `SingleCellExperiment-0.2.5/src/singlecellexperiment/__init__.py` & `SingleCellExperiment-0.2.6/src/singlecellexperiment/__init__.py`

 * *Files 6% similar despite different names*

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
     dist_name = "SingleCellExperiment"
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
```

### Comparing `SingleCellExperiment-0.2.5/src/singlecellexperiment/io/anndata.py` & `SingleCellExperiment-0.2.6/src/singlecellexperiment/io/anndata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import anndata
 from collections import OrderedDict
+
+import anndata
+
 from ..SingleCellExperiment import SingleCellExperiment
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
```

### Comparing `SingleCellExperiment-0.2.5/src/singlecellexperiment/io/tenx.py` & `SingleCellExperiment-0.2.6/src/singlecellexperiment/io/tenx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import h5py
 import pandas as pd
 from scipy.io import mmread
-from scipy.sparse import csr_matrix, csc_matrix
+from scipy.sparse import csc_matrix, csr_matrix
 
 from ..SingleCellExperiment import SingleCellExperiment
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
```

### Comparing `SingleCellExperiment-0.2.5/tests/data/adata.h5ad` & `SingleCellExperiment-0.2.6/tests/data/adata.h5ad`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/tests/data/tenx.sub.h5` & `SingleCellExperiment-0.2.6/tests/data/tenx.sub.h5`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/tests/test_sce.py` & `SingleCellExperiment-0.2.6/tests/test_sce.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/tests/test_sce_io.py` & `SingleCellExperiment-0.2.6/tests/test_sce_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from random import random
 import pandas as pd
 import genomicranges
 from singlecellexperiment.SingleCellExperiment import SingleCellExperiment
 
 import anndata
 from mudata import MuData
+import h5py
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 nrows = 200
```

### Comparing `SingleCellExperiment-0.2.5/tests/test_sce_methods.py` & `SingleCellExperiment-0.2.6/tests/test_sce_methods.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/tests/test_sce_slice.py` & `SingleCellExperiment-0.2.6/tests/test_sce_slice.py`

 * *Files identical despite different names*

### Comparing `SingleCellExperiment-0.2.5/tox.ini` & `SingleCellExperiment-0.2.6/tox.ini`

 * *Files identical despite different names*

