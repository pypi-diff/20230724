# Comparing `tmp/pydsge-0.2.2.tar.gz` & `tmp/pydsge-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydsge-0.2.2.tar", last modified: Wed Jun 28 18:42:03 2023, max compression
+gzip compressed data, was "pydsge-0.2.3.tar", last modified: Mon Jul 24 21:44:52 2023, max compression
```

## Comparing `pydsge-0.2.2.tar` & `pydsge-0.2.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.901882 pydsge-0.2.2/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.881882 pydsge-0.2.2/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.885215 pydsge-0.2.2/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1252 2023-06-28 17:29:41.000000 pydsge-0.2.2/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      175 2022-09-15 10:25:43.000000 pydsge-0.2.2/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2409 2022-03-02 23:34:07.000000 pydsge-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      612 2023-02-21 10:35:12.000000 pydsge-0.2.2/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2022-03-02 23:34:07.000000 pydsge-0.2.2/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3336 2023-06-28 18:42:03.898549 pydsge-0.2.2/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2860 2023-06-28 12:05:18.000000 pydsge-0.2.2/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.885215 pydsge-0.2.2/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2022-03-02 23:34:07.000000 pydsge-0.2.2/docs/Makefile
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1617 2023-02-21 11:28:14.000000 pydsge-0.2.2/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    33348 2022-10-26 16:09:40.000000 pydsge-0.2.2/docs/estimation_tutorial.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   950754 2023-06-28 18:40:55.000000 pydsge-0.2.2/docs/getting_started.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      174 2023-02-21 11:28:14.000000 pydsge-0.2.2/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2563 2022-03-10 19:53:14.000000 pydsge-0.2.2/docs/installation_guide.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2022-03-02 23:34:07.000000 pydsge-0.2.2/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      278 2023-02-21 09:40:18.000000 pydsge-0.2.2/docs/modules.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       27 2022-03-02 23:34:07.000000 pydsge-0.2.2/docs/readme.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    66702 2022-10-26 16:38:38.000000 pydsge-0.2.2/docs/reprocess.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      149 2023-02-21 10:57:49.000000 pydsge-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.888548 pydsge-0.2.2/pydsge/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      655 2023-06-28 18:41:44.000000 pydsge-0.2.2/pydsge/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     9540 2023-02-21 09:48:54.000000 pydsge-0.2.2/pydsge/clsmethods.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     9232 2023-02-21 09:23:01.000000 pydsge-0.2.2/pydsge/engine.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8057 2023-03-15 17:18:16.000000 pydsge-0.2.2/pydsge/estimation.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.895215 pydsge-0.2.2/pydsge/examples/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3864 2022-03-02 23:34:07.000000 pydsge-0.2.2/pydsge/examples/dfi.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    23376 2022-10-26 16:36:36.000000 pydsge-0.2.2/pydsge/examples/dfi_doc0_meta.npz
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    81163 2022-10-26 16:36:36.000000 pydsge-0.2.2/pydsge/examples/dfi_doc0_res.npz
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)  4859544 2022-10-26 16:36:36.000000 pydsge-0.2.2/pydsge/examples/dfi_doc0_sampler.h5
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      262 2022-03-02 23:34:07.000000 pydsge-0.2.2/pydsge/examples/dfi_funcs.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   444744 2023-06-28 16:58:34.000000 pydsge-0.2.2/pydsge/examples/dfi_sampler.h5
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1325 2022-03-02 23:34:07.000000 pydsge-0.2.2/pydsge/examples/minimal_nk.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3471 2022-03-02 23:34:07.000000 pydsge-0.2.2/pydsge/examples/tsdata.csv
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13194 2023-02-21 09:23:06.000000 pydsge-0.2.2/pydsge/filtering.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     9936 2023-02-21 10:17:18.000000 pydsge-0.2.2/pydsge/gensys.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4844 2023-02-21 10:17:17.000000 pydsge-0.2.2/pydsge/mcmc.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13782 2023-02-21 10:19:27.000000 pydsge-0.2.2/pydsge/mpile.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    27127 2023-06-28 14:38:33.000000 pydsge-0.2.2/pydsge/parser.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8634 2023-02-21 10:17:17.000000 pydsge-0.2.2/pydsge/stats.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3537 2023-06-28 17:27:43.000000 pydsge-0.2.2/pydsge/symbols.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.895215 pydsge-0.2.2/pydsge/tests/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5605 2022-10-12 08:35:38.000000 pydsge-0.2.2/pydsge/tests/export_getting_started_to_pkl.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.895215 pydsge-0.2.2/pydsge/tests/resources/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      216 2023-02-02 19:30:58.000000 pydsge-0.2.2/pydsge/tests/resources/estimation.npz
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)  5302079 2023-06-28 18:40:15.000000 pydsge-0.2.2/pydsge/tests/resources/getting_started_stable.npz
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1241 2022-10-26 21:58:09.000000 pydsge-0.2.2/pydsge/tests/test_estimation.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1923 2022-03-02 23:34:07.000000 pydsge-0.2.2/pydsge/tests/test_model.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      881 2022-03-02 23:34:07.000000 pydsge-0.2.2/pydsge/tests/test_parser.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      670 2022-06-17 17:42:54.000000 pydsge-0.2.2/pydsge/tests/test_processing.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14587 2023-02-21 10:17:18.000000 pydsge-0.2.2/pydsge/tools.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-28 18:42:03.888548 pydsge-0.2.2/pydsge.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3336 2023-06-28 18:42:03.000000 pydsge-0.2.2/pydsge.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1222 2023-06-28 18:42:03.000000 pydsge-0.2.2/pydsge.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-06-28 18:42:03.000000 pydsge-0.2.2/pydsge.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      155 2023-06-28 18:42:03.000000 pydsge-0.2.2/pydsge.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        7 2023-06-28 18:42:03.000000 pydsge-0.2.2/pydsge.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      149 2023-02-21 10:41:44.000000 pydsge-0.2.2/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-06-28 18:42:03.901882 pydsge-0.2.2/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1396 2023-02-21 10:25:16.000000 pydsge-0.2.2/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:52.011055 pydsge-0.2.3/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:51.541047 pydsge-0.2.3/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:51.547714 pydsge-0.2.3/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1289 2023-07-02 18:02:11.000000 pydsge-0.2.3/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      175 2022-09-15 10:25:43.000000 pydsge-0.2.3/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2409 2022-03-02 23:34:07.000000 pydsge-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      612 2023-02-21 10:35:12.000000 pydsge-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2022-03-02 23:34:07.000000 pydsge-0.2.3/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3336 2023-07-24 21:44:52.011055 pydsge-0.2.3/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2860 2023-06-28 12:05:18.000000 pydsge-0.2.3/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:51.604382 pydsge-0.2.3/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2022-03-02 23:34:07.000000 pydsge-0.2.3/docs/Makefile
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1617 2023-02-21 11:28:14.000000 pydsge-0.2.3/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    33348 2022-10-26 16:09:40.000000 pydsge-0.2.3/docs/estimation_tutorial.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   950754 2023-06-28 18:40:55.000000 pydsge-0.2.3/docs/getting_started.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      174 2023-02-21 11:28:14.000000 pydsge-0.2.3/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2563 2022-03-10 19:53:14.000000 pydsge-0.2.3/docs/installation_guide.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2022-03-02 23:34:07.000000 pydsge-0.2.3/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      278 2023-02-21 09:40:18.000000 pydsge-0.2.3/docs/modules.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       27 2022-03-02 23:34:07.000000 pydsge-0.2.3/docs/readme.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    66702 2022-10-26 16:38:38.000000 pydsge-0.2.3/docs/reprocess.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      149 2023-02-21 10:57:49.000000 pydsge-0.2.3/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:51.611049 pydsge-0.2.3/pydsge/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      655 2023-07-24 21:44:36.000000 pydsge-0.2.3/pydsge/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     9540 2023-02-21 09:48:54.000000 pydsge-0.2.3/pydsge/clsmethods.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     9232 2023-02-21 09:23:01.000000 pydsge-0.2.3/pydsge/engine.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8057 2023-03-15 17:18:16.000000 pydsge-0.2.3/pydsge/estimation.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:51.811052 pydsge-0.2.3/pydsge/examples/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3864 2022-03-02 23:34:07.000000 pydsge-0.2.3/pydsge/examples/dfi.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    23376 2022-10-26 16:36:36.000000 pydsge-0.2.3/pydsge/examples/dfi_doc0_meta.npz
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    81163 2022-10-26 16:36:36.000000 pydsge-0.2.3/pydsge/examples/dfi_doc0_res.npz
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)  4859544 2022-10-26 16:36:36.000000 pydsge-0.2.3/pydsge/examples/dfi_doc0_sampler.h5
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      262 2022-03-02 23:34:07.000000 pydsge-0.2.3/pydsge/examples/dfi_funcs.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   444744 2023-06-28 16:58:34.000000 pydsge-0.2.3/pydsge/examples/dfi_sampler.h5
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1325 2022-03-02 23:34:07.000000 pydsge-0.2.3/pydsge/examples/minimal_nk.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3471 2022-03-02 23:34:07.000000 pydsge-0.2.3/pydsge/examples/tsdata.csv
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13194 2023-02-21 09:23:06.000000 pydsge-0.2.3/pydsge/filtering.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     9936 2023-02-21 10:17:18.000000 pydsge-0.2.3/pydsge/gensys.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4844 2023-02-21 10:17:17.000000 pydsge-0.2.3/pydsge/mcmc.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13782 2023-02-21 10:19:27.000000 pydsge-0.2.3/pydsge/mpile.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    27127 2023-06-28 14:38:33.000000 pydsge-0.2.3/pydsge/parser.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8634 2023-02-21 10:17:17.000000 pydsge-0.2.3/pydsge/stats.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3537 2023-06-28 17:27:43.000000 pydsge-0.2.3/pydsge/symbols.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:51.817719 pydsge-0.2.3/pydsge/tests/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5605 2022-10-12 08:35:38.000000 pydsge-0.2.3/pydsge/tests/export_getting_started_to_pkl.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:51.817719 pydsge-0.2.3/pydsge/tests/resources/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      216 2023-02-02 19:30:58.000000 pydsge-0.2.3/pydsge/tests/resources/estimation.npz
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)  5302079 2023-06-28 18:40:15.000000 pydsge-0.2.3/pydsge/tests/resources/getting_started_stable.npz
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1241 2022-10-26 21:58:09.000000 pydsge-0.2.3/pydsge/tests/test_estimation.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1923 2022-03-02 23:34:07.000000 pydsge-0.2.3/pydsge/tests/test_model.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      881 2022-03-02 23:34:07.000000 pydsge-0.2.3/pydsge/tests/test_parser.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      670 2022-06-17 17:42:54.000000 pydsge-0.2.3/pydsge/tests/test_processing.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14587 2023-02-21 10:17:18.000000 pydsge-0.2.3/pydsge/tools.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-07-24 21:44:51.614382 pydsge-0.2.3/pydsge.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3336 2023-07-24 21:44:50.000000 pydsge-0.2.3/pydsge.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1222 2023-07-24 21:44:51.000000 pydsge-0.2.3/pydsge.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-07-24 21:44:50.000000 pydsge-0.2.3/pydsge.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      161 2023-07-24 21:44:50.000000 pydsge-0.2.3/pydsge.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        7 2023-07-24 21:44:50.000000 pydsge-0.2.3/pydsge.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      155 2023-07-24 21:43:26.000000 pydsge-0.2.3/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-07-24 21:44:52.011055 pydsge-0.2.3/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1402 2023-07-24 21:43:10.000000 pydsge-0.2.3/setup.py
```

### Comparing `pydsge-0.2.2/.github/workflows/continuous-integration.yml` & `pydsge-0.2.3/.github/workflows/continuous-integration.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 name: Continuous Integration Workflow
 
 on:
   push:
     branches: [ master ]
   pull_request:
     branches: [ master ]
+  schedule:
+    - cron: '30 5 * * 1'
 
 jobs:
   build:
     name: Run tests for ${{ matrix.os }} on ${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
 
     strategy:
```

### Comparing `pydsge-0.2.2/.pre-commit-config.yaml` & `pydsge-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/.readthedocs.yaml` & `pydsge-0.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/LICENSE` & `pydsge-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/PKG-INFO` & `pydsge-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydsge
-Version: 0.2.2
+Version: 0.2.3
 Summary: Solve, filter and estimate DSGE models with occasionaly binding constraints
 Home-page: https://pydsge.readthedocs.io/en/latest/index.html
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pydsge-0.2.2/README.rst` & `pydsge-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/docs/Makefile` & `pydsge-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/docs/conf.py` & `pydsge-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/docs/estimation_tutorial.ipynb` & `pydsge-0.2.3/docs/estimation_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/docs/getting_started.ipynb` & `pydsge-0.2.3/docs/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/docs/installation_guide.rst` & `pydsge-0.2.3/docs/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/docs/make.bat` & `pydsge-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/docs/reprocess.ipynb` & `pydsge-0.2.3/docs/reprocess.ipynb`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/__init__.py` & `pydsge-0.2.3/pydsge/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .gensys import DSGE, gen_sys_from_dict
 import numpy as np
 import logging
 import os
 
 os.environ["OMP_NUM_THREADS"] = "1"
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 np.set_printoptions(threshold=np.inf)
 logging.basicConfig(level=logging.INFO)
 
 pth = os.path.dirname(__file__)
 
 example_model = os.path.join(pth, "examples", "dfi.yaml")
```

### Comparing `pydsge-0.2.2/pydsge/clsmethods.py` & `pydsge-0.2.3/pydsge/clsmethods.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/engine.py` & `pydsge-0.2.3/pydsge/engine.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/estimation.py` & `pydsge-0.2.3/pydsge/estimation.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/examples/dfi.yaml` & `pydsge-0.2.3/pydsge/examples/dfi.yaml`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/examples/dfi_doc0_meta.npz` & `pydsge-0.2.3/pydsge/examples/dfi_doc0_meta.npz`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/examples/dfi_doc0_res.npz` & `pydsge-0.2.3/pydsge/examples/dfi_doc0_res.npz`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/examples/dfi_doc0_sampler.h5` & `pydsge-0.2.3/pydsge/examples/dfi_doc0_sampler.h5`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/examples/dfi_sampler.h5` & `pydsge-0.2.3/pydsge/examples/dfi_sampler.h5`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/examples/minimal_nk.yaml` & `pydsge-0.2.3/pydsge/examples/minimal_nk.yaml`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/examples/tsdata.csv` & `pydsge-0.2.3/pydsge/examples/tsdata.csv`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/filtering.py` & `pydsge-0.2.3/pydsge/filtering.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/gensys.py` & `pydsge-0.2.3/pydsge/gensys.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/mcmc.py` & `pydsge-0.2.3/pydsge/mcmc.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/mpile.py` & `pydsge-0.2.3/pydsge/mpile.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/parser.py` & `pydsge-0.2.3/pydsge/parser.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/stats.py` & `pydsge-0.2.3/pydsge/stats.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/symbols.py` & `pydsge-0.2.3/pydsge/symbols.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/tests/export_getting_started_to_pkl.py` & `pydsge-0.2.3/pydsge/tests/export_getting_started_to_pkl.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/tests/resources/getting_started_stable.npz` & `pydsge-0.2.3/pydsge/tests/resources/getting_started_stable.npz`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/tests/test_estimation.py` & `pydsge-0.2.3/pydsge/tests/test_estimation.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/tests/test_model.py` & `pydsge-0.2.3/pydsge/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/tests/test_parser.py` & `pydsge-0.2.3/pydsge/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/tests/test_processing.py` & `pydsge-0.2.3/pydsge/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge/tools.py` & `pydsge-0.2.3/pydsge/tools.py`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/pydsge.egg-info/PKG-INFO` & `pydsge-0.2.3/pydsge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydsge
-Version: 0.2.2
+Version: 0.2.3
 Summary: Solve, filter and estimate DSGE models with occasionaly binding constraints
 Home-page: https://pydsge.readthedocs.io/en/latest/index.html
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pydsge-0.2.2/pydsge.egg-info/SOURCES.txt` & `pydsge-0.2.3/pydsge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydsge-0.2.2/setup.py` & `pydsge-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,21 +30,21 @@
     install_requires=[
         "numba",
         "emcee",
         "numpy",
         "pandas",
         "pathos",
         "dill",
-        "scipy",
         "sympy",
         "tqdm",
         "chaospy",
         "cloudpickle",
         "h5py",
         "pyyaml",
+        "scipy>=1.12",
         "emcwrap>=0.2.2",
         "grgrlib>=0.1.15",
         "econsieve>=0.0.8",
         "threadpoolctl>=3.1.0",
     ],
     include_package_data=True,
 )
```

