# Comparing `tmp/SummarizedExperiment-0.2.8.tar.gz` & `tmp/SummarizedExperiment-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SummarizedExperiment-0.2.8.tar", last modified: Wed Jul 19 22:39:00 2023, max compression
+gzip compressed data, was "SummarizedExperiment-0.2.9.tar", last modified: Mon Jul 24 05:14:04 2023, max compression
```

## Comparing `SummarizedExperiment-0.2.8.tar` & `SummarizedExperiment-0.2.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.659809 SummarizedExperiment-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.639808 SummarizedExperiment-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.643808 SummarizedExperiment-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-19 22:39:00.659809 SummarizedExperiment-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.651809 SummarizedExperiment-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.651809 SummarizedExperiment-0.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-19 22:39:00.663809 SummarizedExperiment-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.639808 SummarizedExperiment-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.651809 SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-19 22:39:00.000000 SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-19 22:39:00.000000 SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:39:00.000000 SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:37:41.000000 SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-19 22:39:00.000000 SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 22:39:00.000000 SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.655809 SummarizedExperiment-0.2.8/src/summarizedexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/BaseSE.py
--rw-r--r--   0 runner    (1001) docker     (123)    22285 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/RangeSummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/RangedSummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/SummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/_slicer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/_type_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.655809 SummarizedExperiment-0.2.8/src/summarizedexperiment/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/dispatchers/colnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/src/summarizedexperiment/dispatchers/rownames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.655809 SummarizedExperiment-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:39:00.655809 SummarizedExperiment-0.2.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/data/summarized_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/data/tenx.sub.h5
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/test_RSE.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/test_RSE_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/test_SE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/test_SE_backed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/test_SE_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tests/test_SE_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-19 22:37:29.000000 SummarizedExperiment-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.845854 SummarizedExperiment-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.837854 SummarizedExperiment-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.837854 SummarizedExperiment-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-24 05:14:04.845854 SummarizedExperiment-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.841854 SummarizedExperiment-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.841854 SummarizedExperiment-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-24 05:14:04.845854 SummarizedExperiment-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.837854 SummarizedExperiment-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.841854 SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-24 05:14:04.000000 SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-24 05:14:04.000000 SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:14:04.000000 SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:12:56.000000 SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 05:14:04.000000 SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 05:14:04.000000 SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.841854 SummarizedExperiment-0.2.9/src/summarizedexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/BaseSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/RangeSummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/RangedSummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/SummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/_slicer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/_type_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.841854 SummarizedExperiment-0.2.9/src/summarizedexperiment/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/dispatchers/colnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/dispatchers/rownames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/src/summarizedexperiment/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.845854 SummarizedExperiment-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:14:04.845854 SummarizedExperiment-0.2.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/data/summarized_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/data/tenx.sub.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/test_RSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/test_RSE_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/test_SE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/test_SE_backed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/test_SE_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tests/test_SE_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-24 05:12:44.000000 SummarizedExperiment-0.2.9/tox.ini
```

### Comparing `SummarizedExperiment-0.2.8/.coveragerc` & `SummarizedExperiment-0.2.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/.github/workflows/pypi-publish.yml` & `SummarizedExperiment-0.2.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/.github/workflows/pypi-test.yml` & `SummarizedExperiment-0.2.9/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/.gitignore` & `SummarizedExperiment-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/CHANGELOG.md` & `SummarizedExperiment-0.2.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/CONTRIBUTING.rst` & `SummarizedExperiment-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/LICENSE.txt` & `SummarizedExperiment-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/PKG-INFO` & `SummarizedExperiment-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SummarizedExperiment
-Version: 0.2.8
+Version: 0.2.9
 Summary: Container to represent data from genomic experiments
 Home-page: https://github.com/BiocPy/summarizedexperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/summarizedexperiment
 Platform: any
```

### Comparing `SummarizedExperiment-0.2.8/README.md` & `SummarizedExperiment-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/docs/Makefile` & `SummarizedExperiment-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/docs/changelog.md` & `SummarizedExperiment-0.2.9/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/docs/conf.py` & `SummarizedExperiment-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/docs/index.md` & `SummarizedExperiment-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/docs/readme.md` & `SummarizedExperiment-0.2.9/docs/readme.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/docs/tutorial.md` & `SummarizedExperiment-0.2.9/docs/tutorial.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Tutorial
 
-This package provides classes to represent genomic experiments. Currently supports both `SummarizedExperiment` & `RangeSummarizedExperiment` representations.
+This package provides classes to represent genomic experiments, commonly generated by sequencing experiments. This package tried to provide the same interfaces and functionality as the [Bioconductor equivalent](https://github.com/Bioconductor/SummarizedExperiment).
 
-# Create a `SummarizedExperiment`
-
-To create a `SummarizedExperiment`, we need
+A `SummarizedExperiment` contains three slots,
 
+- `rowData`: feature information e.g. genes, transcripts, exons, etc.
+- `colData`: sample information about the columns of the matrices.
 - `Assays`: a dictionary of matrices with keys specifying the assay name. 
-- `rows`: feature information about the rows of the matrices.
-- `cols`: sample information about the columns of the matrices.
 
-Lets create these three objects. we first create a mock dataset of 200 rows and 6 columns, also adding a few sample data.
+
+The package currently provides both `SummarizedExperiment` & `RangeSummarizedExperiment` representations, a fundamental difference between these two is the rows of a `RangedSummarizedExperiment` object represent [GenomicRanges](https://github.com/BiocPy/GenomicRanges) of interest.
+
+## Construct a `SummarizedExperiment` object
+
+First, lets create some example matrices along with their feature and sample information.
 
 ```python
 nrows = 200
 ncols = 6
 counts = np.random.rand(nrows, ncols)
 
 df_gr = pd.DataFrame(
@@ -45,37 +48,38 @@
         "treatment": ["ChIP", "Input"] * 3,
     }
 )
 ```
 
 Finally, create an appropriate summarized experiment class. 
 
-## `SummarizedExperiment`
+### `SummarizedExperiment`
 
-A `SummarizedExperiment` is a relaxed variant to represent genomic experiments. This class expects features (`rowData`) to be either a pandas `DataFrame` or any variant of `BiocFrame`.
+A `SummarizedExperiment` is a base class to represent any genomic experiment. This class expects features (`rowData`) to be either a pandas `DataFrame` or any variant of `BiocFrame`.
 
 ```python
-tse = SummarizedExperiment(
+se = SummarizedExperiment(
     assays={"counts": counts}, rowData=df_gr, colData=colData
 )
 ```
 
-##  `RangeSummarizedExperiment`
+###  `RangeSummarizedExperiment`
 
-`RangeSummarizedExperiment` represents features as [`GenomicRanges`](https://github.com/BiocPy/GenomicRanges).
+`RangeSummarizedExperiment` requires features to be a [`GenomicRanges`](https://github.com/BiocPy/GenomicRanges) object.
 
 ```python
+# convert our pandas dataframe to genomic ranges.
 gr = GenomicRanges.fromPandas(df_gr)
 
-trse = SummarizedExperiment(
+rse = SummarizedExperiment(
     assays={"counts": counts}, rowRanges=gr, colData=colData
 )
 ```
 
-## File backed mode for large datasets
+### File backed mode for large datasets
 
 In addition to fully realized matrices in memory, SE/RSE also supports file backed arrays and matrices. [FileBackedArray](https://github.com/BiocPy/FileBackedArray) package provides lazy representation for matrices stored in hdf5 files.
 
 ```python
 from filebackedarray import H5BackedSparseData
 
 df_gr = pd.DataFrame(
@@ -111,37 +115,38 @@
     colData=colData,
 )
 ```
 
 
 ## Accessors
 
-Many properties can be accessed directly from the class instance. Checkout the API for all available methods.
+Many properties can be accessed directly from the class instance.
 
 ```python
 tse.assays
 tse.rowData or # tse.rowRanges
 tse.colData
+tse.metadata
 
 # Access the counts assay
 tse.assay("counts")
 ```
 
-# Subset an experiment
+## Subset an experiment
 
-## `SummarizedExperiment`
+You can subset a `SummarizedExperiment` object using the `[]` slice operator.
 
-Use `[ ]` notation to subset a `SummarizedExperiment` object.
+### slice by index position
 
 ```python
 # subset the first 10 rows and the first 3 samples
 subset_tse = tse[0:10, 0:3]
 ```
-
-Alternatively, we can use a sequence of names or a boolean array. To show this, we create a `SummarizedExperiment` object with index names.
+### slice by row names or column names
+Alternatively, we can use a sequence of row (feature) or column (sample) names to subset a `SummarizedExperiment` . To demonstrate this, we create a `SummarizedExperiment` object with index names.
 
 ```python
 rowData_with_index_names = pd.DataFrame(
     {
         "seqnames": ["chr_5", "chr_3", "chr_2"],
         "start": [100, 200, 300],
         "end": [110, 210, 310]
@@ -164,37 +169,43 @@
     colData=colData_with_index_names
 )
 
 # subset by name
 subset_se_with_index_names = se_with_index_names[
     ["HER2", "BRCA1"], ["cell_1", "cell_3"]
 ]
-
-# subset with boolean array
-subset_se_with_bools = se_with_index_names[
-    [True, True, False], [True, False, True]
-]
 ```
 
 In the case a name does not exist, an error will be thrown:
 
 ```python
 # throws error because "RAND" does not exist
 subset_se_with_index_names = se_with_index_names[
     ["HER2", "BRCA1", "RAND"], ["cell_1", "cell_3"]
 ]
 ```
 
-## `RangedSummarizedExperiment`
+### slice by a boolean vector
+
+similarly you could also slice by a boolean array. Note, the boolean vectors should contain the same number of features for the row slice and the same number of samples for the column slice.
+
+```python
+# subset with boolean array
+subset_se_with_bools = se_with_index_names[
+    [True, True, False], [True, False, True]
+]
+```
+
+## Range based operations
 
-`RangeSummarizedExperiment` objects on the other hand support interval based operations.
+`RangeSummarizedExperiment` objects on the other hand supports many interval based operations similar to `GenomicRanges`.
 
 
 ```python
 query = {"seqnames": ["chr2",], "starts": [4], "ends": [6], "strand": ["+"]}
 
 query = GenomicRanges(query)
 
-tse.subsetOverlaps(query)
+tse.subsetByOverlaps(query)
 ```
 
 Checkout the API docs or GenomicRanges for list of interval based operations.
```

### Comparing `SummarizedExperiment-0.2.8/setup.cfg` & `SummarizedExperiment-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/setup.py` & `SummarizedExperiment-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/PKG-INFO` & `SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SummarizedExperiment
-Version: 0.2.8
+Version: 0.2.9
 Summary: Container to represent data from genomic experiments
 Home-page: https://github.com/BiocPy/summarizedexperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/summarizedexperiment
 Platform: any
```

### Comparing `SummarizedExperiment-0.2.8/src/SummarizedExperiment.egg-info/SOURCES.txt` & `SummarizedExperiment-0.2.9/src/SummarizedExperiment.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 src/summarizedexperiment/BaseSE.py
 src/summarizedexperiment/RangeSummarizedExperiment.py
 src/summarizedexperiment/RangedSummarizedExperiment.py
 src/summarizedexperiment/SummarizedExperiment.py
 src/summarizedexperiment/__init__.py
 src/summarizedexperiment/_slicer_utils.py
 src/summarizedexperiment/_type_checks.py
-src/summarizedexperiment/_types.py
+src/summarizedexperiment/types.py
 src/summarizedexperiment/dispatchers/__init__.py
 src/summarizedexperiment/dispatchers/colnames.py
 src/summarizedexperiment/dispatchers/rownames.py
 tests/conftest.py
 tests/test_RSE.py
 tests/test_RSE_methods.py
 tests/test_SE.py
```

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/BaseSE.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/BaseSE.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 import pandas as pd
 from biocframe import BiocFrame
 from filebackedarray import H5BackedDenseData, H5BackedSparseData
 from genomicranges import GenomicRanges
 
 from ._slicer_utils import get_indexes_from_bools, get_indexes_from_names
 from ._type_checks import is_bioc_or_pandas_frame, is_list_of_type, is_matrix_like
-from ._types import (
+from .dispatchers.colnames import get_colnames, set_colnames
+from .dispatchers.rownames import get_rownames, set_rownames
+from .types import (
     BiocOrPandasFrame,
     MatrixSlicerTypes,
     MatrixTypes,
     SlicerArgTypes,
 )
-from .dispatchers.colnames import get_colnames, set_colnames
-from .dispatchers.rownames import get_rownames, set_rownames
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 class BaseSE:
```

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/RangeSummarizedExperiment.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/RangeSummarizedExperiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import MutableMapping, Optional, Sequence, Union
 
 import numpy as np
 from genomicranges import GenomicRanges, SeqInfo
 
-from ._types import BiocOrPandasFrame, MatrixTypes, SlicerArgTypes
 from .BaseSE import BaseSE
+from .types import BiocOrPandasFrame, MatrixTypes, SlicerArgTypes
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 GRangesOrRangeSE = Union[GenomicRanges, "RangeSummarizedExperiment"]
```

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/SummarizedExperiment.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/SummarizedExperiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import MutableMapping, Optional
 
-from ._types import BiocOrPandasFrame, MatrixTypes, SlicerArgTypes
 from .BaseSE import BaseSE
+from .types import BiocOrPandasFrame, MatrixTypes, SlicerArgTypes
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 class SummarizedExperiment(BaseSE):
```

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/__init__.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/__init__.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/_slicer_utils.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/_slicer_utils.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/_type_checks.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/_type_checks.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/_types.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/types.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/dispatchers/colnames.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/dispatchers/colnames.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/src/summarizedexperiment/dispatchers/rownames.py` & `SummarizedExperiment-0.2.9/src/summarizedexperiment/dispatchers/rownames.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tests/data/summarized_experiments.py` & `SummarizedExperiment-0.2.9/tests/data/summarized_experiments.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tests/data/tenx.sub.h5` & `SummarizedExperiment-0.2.9/tests/data/tenx.sub.h5`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tests/test_RSE.py` & `SummarizedExperiment-0.2.9/tests/test_RSE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tests/test_RSE_methods.py` & `SummarizedExperiment-0.2.9/tests/test_RSE_methods.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tests/test_SE.py` & `SummarizedExperiment-0.2.9/tests/test_SE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tests/test_SE_backed.py` & `SummarizedExperiment-0.2.9/tests/test_SE_backed.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tests/test_SE_methods.py` & `SummarizedExperiment-0.2.9/tests/test_SE_methods.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tests/test_SE_subset.py` & `SummarizedExperiment-0.2.9/tests/test_SE_subset.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.8/tox.ini` & `SummarizedExperiment-0.2.9/tox.ini`

 * *Files identical despite different names*

