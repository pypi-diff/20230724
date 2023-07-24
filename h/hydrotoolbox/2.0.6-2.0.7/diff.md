# Comparing `tmp/hydrotoolbox-2.0.6.tar.gz` & `tmp/hydrotoolbox-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrotoolbox-2.0.6.tar", last modified: Sun Apr 30 00:59:44 2023, max compression
+gzip compressed data, was "hydrotoolbox-2.0.7.tar", last modified: Mon Jul 24 12:03:40 2023, max compression
```

## Comparing `hydrotoolbox-2.0.6.tar` & `hydrotoolbox-2.0.7.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.727897 hydrotoolbox-2.0.6/
--rw-rw-r--   0 tim       (1000) tim       (1000)      155 2023-04-28 04:19:43.000000 hydrotoolbox-2.0.6/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.671890 hydrotoolbox-2.0.6/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.675891 hydrotoolbox-2.0.6/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)      505 2023-04-28 04:19:43.000000 hydrotoolbox-2.0.6/.github/workflows/clean-workflow-runs.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-04-28 04:19:43.000000 hydrotoolbox-2.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      335 2023-03-05 18:51:14.000000 hydrotoolbox-2.0.6/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2736 2023-04-30 00:58:27.000000 hydrotoolbox-2.0.6/.pre-commit-config.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)       50 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.6/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1051 2022-09-28 02:43:28.000000 hydrotoolbox-2.0.6/BADGES.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     1242 2023-04-30 00:58:48.000000 hydrotoolbox-2.0.6/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3187 2021-07-31 11:07:02.000000 hydrotoolbox-2.0.6/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1489 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.6/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     4395 2023-04-30 00:59:44.727897 hydrotoolbox-2.0.6/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     2935 2022-12-11 04:26:43.000000 hydrotoolbox-2.0.6/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-04-30 00:58:48.000000 hydrotoolbox-2.0.6/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.679891 hydrotoolbox-2.0.6/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.6/docs/Makefile
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-07-31 11:07:00.000000 hydrotoolbox-2.0.6/docs/authors.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     2471 2023-03-26 19:47:45.000000 hydrotoolbox-2.0.6/docs/command_line.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     9636 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.6/docs/contributing.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1162 2023-03-26 19:28:44.000000 hydrotoolbox-2.0.6/docs/function_summary.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-07-03 12:45:13.000000 hydrotoolbox-2.0.6/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.6/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2022-02-08 03:38:16.000000 hydrotoolbox-2.0.6/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-07-31 11:07:00.000000 hydrotoolbox-2.0.6/docs/readme.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     2792 2023-04-30 00:58:49.000000 hydrotoolbox-2.0.6/pyproject.toml
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.6/pytest.ini
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-04-30 00:59:44.727897 hydrotoolbox-2.0.6/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      516 2023-03-01 21:50:53.000000 hydrotoolbox-2.0.6/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.671890 hydrotoolbox-2.0.6/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.679891 hydrotoolbox-2.0.6/src/hydrotoolbox/
--rw-rw-r--   0 tim       (1000) tim       (1000)      181 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/__init__.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.695893 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/
--rw-rw-r--   0 tim       (1000) tim       (1000)      172 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3195 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/comparison.py
--rw-rw-r--   0 tim       (1000) tim       (1000)   644797 2022-01-28 18:17:47.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/example.csv
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.695893 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/
--rw-rw-r--   0 tim       (1000) tim       (1000)      815 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Boughton.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      578 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/CM.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      597 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Chapman.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      571 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/EWMA.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      871 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Eckhardt.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      636 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Fixed.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      799 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Furey.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      877 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/LH.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1581 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Local.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      748 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Slide.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1459 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/UKIH.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      933 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Willems.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      323 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      840 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/five_day.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      542 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/ihacres.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      380 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/strict.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3336 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/param_estimate.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2615 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/separation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2791 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/utils.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    21293 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow_sep.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    82189 2023-03-12 15:02:23.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/hydrotoolbox.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.695893 hydrotoolbox-2.0.6/src/hydrotoolbox/indices/
--rw-rw-r--   0 tim       (1000) tim       (1000)    56628 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/indices/indices.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      866 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.6/src/hydrotoolbox/utils.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.683892 hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4395 2023-04-30 00:59:44.000000 hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     2366 2023-04-30 00:59:44.000000 hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-04-30 00:59:44.000000 hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       64 2023-04-30 00:59:44.000000 hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      267 2023-04-30 00:59:44.000000 hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       13 2023-04-30 00:59:44.000000 hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-04-30 00:59:44.727897 hydrotoolbox-2.0.6/tests/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1017 2022-09-29 03:00:21.000000 hydrotoolbox-2.0.6/tests/BEC_test.sh
--rw-rw-r--   0 tim       (1000) tim       (1000)   644797 2022-03-11 23:36:08.000000 hydrotoolbox-2.0.6/tests/data.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1123858 2022-02-25 03:11:09.000000 hydrotoolbox-2.0.6/tests/data_02239501.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1231005 2022-09-05 18:15:22.000000 hydrotoolbox-2.0.6/tests/data_boughton.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1248213 2022-09-05 17:47:34.000000 hydrotoolbox-2.0.6/tests/data_chapman.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1180403 2022-09-05 17:47:42.000000 hydrotoolbox-2.0.6/tests/data_cm.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1230240 2022-09-05 17:53:18.000000 hydrotoolbox-2.0.6/tests/data_eckhardt.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1170952 2022-09-05 17:56:40.000000 hydrotoolbox-2.0.6/tests/data_ewma.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1010905 2022-09-05 18:09:12.000000 hydrotoolbox-2.0.6/tests/data_five_day.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1235656 2022-09-05 18:02:10.000000 hydrotoolbox-2.0.6/tests/data_furey.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   928259 2022-09-05 17:53:27.000000 hydrotoolbox-2.0.6/tests/data_ihacres.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1235555 2022-09-05 18:09:03.000000 hydrotoolbox-2.0.6/tests/data_lh.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)      169 2022-04-06 12:39:07.000000 hydrotoolbox-2.0.6/tests/data_percentile_test.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   712817 2022-09-05 18:09:21.000000 hydrotoolbox-2.0.6/tests/data_strict.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1140492 2022-09-05 18:02:36.000000 hydrotoolbox-2.0.6/tests/data_ukih.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   914278 2022-09-05 17:56:48.000000 hydrotoolbox-2.0.6/tests/data_usgs_hysep_fixed.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1060115 2022-09-05 18:02:19.000000 hydrotoolbox-2.0.6/tests/data_usgs_hysep_local.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   913052 2022-09-05 18:02:27.000000 hydrotoolbox-2.0.6/tests/data_usgs_hysep_slide.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)  1234584 2022-09-05 18:08:54.000000 hydrotoolbox-2.0.6/tests/data_willems.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)    16068 2022-10-09 19:21:06.000000 hydrotoolbox-2.0.6/tests/hydrotoolbox_indices.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     2948 2022-09-29 03:00:20.000000 hydrotoolbox-2.0.6/tests/run_test.sh
--rw-rw-r--   0 tim       (1000) tim       (1000)     2055 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.6/tests/test_baseflow_sep.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1738 2023-01-16 14:50:30.000000 hydrotoolbox-2.0.6/tests/tsproc_hydrologic_indices.inp
--rw-rw-r--   0 tim       (1000) tim       (1000)     1715 2023-01-16 14:50:30.000000 hydrotoolbox-2.0.6/tests/tsproc_hydrologic_indices_percentile_test.inp
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.399933 hydrotoolbox-2.0.7/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      155 2023-06-17 22:11:44.000000 hydrotoolbox-2.0.7/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.383932 hydrotoolbox-2.0.7/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-07-24 05:53:00.000000 hydrotoolbox-2.0.7/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-06-17 22:11:45.000000 hydrotoolbox-2.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      335 2023-03-05 18:51:14.000000 hydrotoolbox-2.0.7/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-07-24 05:53:00.000000 hydrotoolbox-2.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 tim       (1000) tim       (1000)       50 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.7/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1051 2022-09-28 02:43:28.000000 hydrotoolbox-2.0.7/BADGES.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1266 2023-07-24 12:03:33.000000 hydrotoolbox-2.0.7/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3187 2021-07-31 11:07:02.000000 hydrotoolbox-2.0.7/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1489 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.7/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4457 2023-07-24 12:03:40.399933 hydrotoolbox-2.0.7/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     2997 2023-06-10 05:29:49.000000 hydrotoolbox-2.0.7/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-07-24 12:03:33.000000 hydrotoolbox-2.0.7/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/docs/
+-rw-r--r--   0 tim       (1000) tim       (1000)     5712 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.7/docs/Makefile
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-07-31 11:07:00.000000 hydrotoolbox-2.0.7/docs/authors.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     2471 2023-05-13 04:19:38.000000 hydrotoolbox-2.0.7/docs/command_line.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     9636 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.7/docs/contributing.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      866 2023-06-16 14:57:14.000000 hydrotoolbox-2.0.7/docs/function_summary.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-07-03 12:45:13.000000 hydrotoolbox-2.0.7/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2021-01-12 15:43:34.000000 hydrotoolbox-2.0.7/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2022-02-08 03:38:16.000000 hydrotoolbox-2.0.7/docs/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-07-31 11:07:00.000000 hydrotoolbox-2.0.7/docs/readme.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2792 2023-07-24 12:03:34.000000 hydrotoolbox-2.0.7/pyproject.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2021-01-12 15:43:08.000000 hydrotoolbox-2.0.7/pytest.ini
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-07-24 12:03:40.399933 hydrotoolbox-2.0.7/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      516 2023-03-01 21:50:53.000000 hydrotoolbox-2.0.7/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.383932 hydrotoolbox-2.0.7/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      181 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/__init__.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      172 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3195 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/comparison.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)   644797 2022-01-28 18:17:47.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/example.csv
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      815 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Boughton.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      578 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/CM.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      597 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Chapman.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      571 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/EWMA.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      871 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Eckhardt.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      636 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Fixed.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      799 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Furey.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      877 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/LH.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1581 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Local.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      748 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Slide.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1459 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/UKIH.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      933 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Willems.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      323 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      840 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/five_day.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      542 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/ihacres.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      380 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/strict.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3336 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/param_estimate.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2615 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/separation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2791 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/utils.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21293 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow_sep.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    82189 2023-03-12 15:02:23.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/hydrotoolbox.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox/indices/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    56628 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/indices/indices.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      866 2023-01-22 03:38:21.000000 hydrotoolbox-2.0.7/src/hydrotoolbox/utils.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.387932 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4457 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2366 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       64 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      267 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       13 2023-07-24 12:03:40.000000 hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-24 12:03:40.399933 hydrotoolbox-2.0.7/tests/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1017 2022-09-29 03:00:21.000000 hydrotoolbox-2.0.7/tests/BEC_test.sh
+-rw-rw-r--   0 tim       (1000) tim       (1000)   644797 2022-03-11 23:36:08.000000 hydrotoolbox-2.0.7/tests/data.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1123858 2022-02-25 03:11:09.000000 hydrotoolbox-2.0.7/tests/data_02239501.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1231005 2022-09-05 18:15:22.000000 hydrotoolbox-2.0.7/tests/data_boughton.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1248213 2022-09-05 17:47:34.000000 hydrotoolbox-2.0.7/tests/data_chapman.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1180403 2022-09-05 17:47:42.000000 hydrotoolbox-2.0.7/tests/data_cm.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1230240 2022-09-05 17:53:18.000000 hydrotoolbox-2.0.7/tests/data_eckhardt.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1170952 2022-09-05 17:56:40.000000 hydrotoolbox-2.0.7/tests/data_ewma.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1010905 2022-09-05 18:09:12.000000 hydrotoolbox-2.0.7/tests/data_five_day.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1235656 2022-09-05 18:02:10.000000 hydrotoolbox-2.0.7/tests/data_furey.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   928259 2022-09-05 17:53:27.000000 hydrotoolbox-2.0.7/tests/data_ihacres.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1235555 2022-09-05 18:09:03.000000 hydrotoolbox-2.0.7/tests/data_lh.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)      169 2022-04-06 12:39:07.000000 hydrotoolbox-2.0.7/tests/data_percentile_test.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   712817 2022-09-05 18:09:21.000000 hydrotoolbox-2.0.7/tests/data_strict.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1140492 2022-09-05 18:02:36.000000 hydrotoolbox-2.0.7/tests/data_ukih.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   914278 2022-09-05 17:56:48.000000 hydrotoolbox-2.0.7/tests/data_usgs_hysep_fixed.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1060115 2022-09-05 18:02:19.000000 hydrotoolbox-2.0.7/tests/data_usgs_hysep_local.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   913052 2022-09-05 18:02:27.000000 hydrotoolbox-2.0.7/tests/data_usgs_hysep_slide.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1234584 2022-09-05 18:08:54.000000 hydrotoolbox-2.0.7/tests/data_willems.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)    16068 2022-10-09 19:21:06.000000 hydrotoolbox-2.0.7/tests/hydrotoolbox_indices.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2948 2022-09-29 03:00:20.000000 hydrotoolbox-2.0.7/tests/run_test.sh
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2055 2023-02-14 05:26:38.000000 hydrotoolbox-2.0.7/tests/test_baseflow_sep.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1738 2023-01-16 14:50:30.000000 hydrotoolbox-2.0.7/tests/tsproc_hydrologic_indices.inp
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1715 2023-01-16 14:50:30.000000 hydrotoolbox-2.0.7/tests/tsproc_hydrologic_indices_percentile_test.inp
```

### Comparing `hydrotoolbox-2.0.6/.github/workflows/python-package.yml` & `hydrotoolbox-2.0.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/.pre-commit-config.yaml` & `hydrotoolbox-2.0.7/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -19,27 +19,27 @@
           - id: fix-encoding-pragma
             args: [--remove]
           - id: mixed-line-ending
           - id: trailing-whitespace
             exclude: notebooks/tstoolbox_plot_bash.sh
 
     - repo: https://github.com/pappasam/toml-sort
-      rev: v0.23.0
+      rev: v0.23.1
       hooks:
           - id: toml-sort-fix
             args: [--in-place, --spaces-indent-inline-array, '4']
 
     - repo: https://github.com/adrienverge/yamllint.git
-      rev: v1.31.0
+      rev: v1.32.0
       hooks:
           - id: yamllint
             args: [--format, parsable, --strict]
 
     - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
-      rev: 0.2.2
+      rev: 0.2.3
       hooks:
           - id: yamlfmt
 
     - repo: https://github.com/jumanjihouse/pre-commit-hooks
       rev: 3.0.0
       hooks:
           - id: shellcheck
@@ -48,17 +48,18 @@
     - repo: https://github.com/lovesegfault/beautysh
       rev: v6.2.1
       hooks:
           - id: beautysh
             args: [--indent-size, '4']
 
     - repo: https://github.com/psf/black
-      rev: 23.3.0
+      rev: 23.7.0
       hooks:
           - id: black
+          - id: black-jupyter
 
     - repo: https://github.com/pycqa/isort
       rev: 5.12.0
       hooks:
           - id: isort
             name: isort (python)
             args: [--profile, black, --filter-files]
@@ -67,33 +68,28 @@
             types: [cython]
             args: [--profile, black, --filter-files]
           - id: isort
             name: isort (pyi)
             types: [pyi]
             args: [--profile, black, --filter-files]
 
-    - repo: https://github.com/dfm/black_nbconvert
-      rev: v0.4.0
-      hooks:
-          - id: black_nbconvert
-
     - repo: https://github.com/asottile/blacken-docs
-      rev: 1.13.0
+      rev: 1.15.0
       hooks:
           - id: blacken-docs
 
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.3.2
+      rev: v3.9.0
       hooks:
           - id: pyupgrade
 
     - repo: https://github.com/commitizen-tools/commitizen
-      rev: 3.1.0
+      rev: 3.5.3
       hooks:
           - id: commitizen
             stages: [commit-msg]
 
     - repo: https://github.com/mwouts/jupytext
-      rev: v1.14.5
+      rev: v1.14.7
       hooks:
           - id: jupytext
             args: [--from, ipynb, --to, auto:percent, --sync]
```

### Comparing `hydrotoolbox-2.0.6/BADGES.rst` & `hydrotoolbox-2.0.7/BADGES.rst`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/CHANGELOG.md` & `hydrotoolbox-2.0.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+## v2.0.7 (2023-07-24)
+
 ## v2.0.6 (2023-04-29)
 
 ## v2.0.5 (2023-02-14)
 
 ### Refactor
 
 - small refactors
```

### Comparing `hydrotoolbox-2.0.6/CONTRIBUTING.rst` & `hydrotoolbox-2.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/LICENSE.txt` & `hydrotoolbox-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/PKG-INFO` & `hydrotoolbox-2.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrotoolbox
-Version: 2.0.6
+Version: 2.0.7
 Summary: Command line script and Python library for analysis of flow time-series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hydrotoolbox/docs/index.html#hydrotoolbox-documentation
 Project-URL: github, https://github.com/timcera/hydrotoolbox
 Project-URL: bitbucket, https://bitbucket.org/timcera/hydrotoolbox/src/main/
 Keywords: time-series,cli-app,hydrology,baseflow,hydrograph-recession,hydrographic
@@ -67,16 +67,26 @@
 
 Requirements
 ------------
 * python 3.7 or higher
 
 Installation
 ------------
-Should be as easy as running ``pip install hydrotoolbox``
-at any command line.
+pip
+~~~
+.. code-block:: bash
+
+    pip install hydrotoolbox
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge hydrotoolbox
+
 
 Usage - Command Line
 --------------------
 Just run 'hydrotoolbox --help' to get a list of subcommands::
 
 
     usage: hydrotoolbox [-h] [-v] {baseflow_sep,recession,about} ...
```

### Comparing `hydrotoolbox-2.0.6/README.rst` & `hydrotoolbox-2.0.7/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,26 @@
 
 Requirements
 ------------
 * python 3.7 or higher
 
 Installation
 ------------
-Should be as easy as running ``pip install hydrotoolbox``
-at any command line.
+pip
+~~~
+.. code-block:: bash
+
+    pip install hydrotoolbox
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge hydrotoolbox
+
 
 Usage - Command Line
 --------------------
 Just run 'hydrotoolbox --help' to get a list of subcommands::
 
 
     usage: hydrotoolbox [-h] [-v] {baseflow_sep,recession,about} ...
```

### Comparing `hydrotoolbox-2.0.6/docs/Makefile` & `hydrotoolbox-2.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/docs/command_line.rst` & `hydrotoolbox-2.0.7/docs/command_line.rst`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/docs/conf.py` & `hydrotoolbox-2.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/docs/make.bat` & `hydrotoolbox-2.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/pyproject.toml` & `hydrotoolbox-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [project]
 name = "hydrotoolbox"
 dynamic = ["version"]
 readme = "README.rst"
 description = "Command line script and Python library for analysis of flow time-series."
 dependencies = [
     "cltoolbox >= 1.0.0",
-    "toolbox_utils >= 3.0.0, < 4.0.0",
+    "toolbox_utils >= 5.0.0, < 6.0.0",
     "pydantic"
 ]
 authors = [
     {name = "Tim Cera", email = "tim@cerazone.net"}
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -93,15 +93,15 @@
     ".ipynb_checkpoints/*"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "2.0.6"
+version = "2.0.7"
 version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
 license-files = ["LICENSE.txt"]
```

### Comparing `hydrotoolbox-2.0.6/setup.py` & `hydrotoolbox-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/comparison.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/comparison.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/example.csv` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/example.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Boughton.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Boughton.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/CM.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/CM.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Chapman.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Chapman.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/EWMA.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/EWMA.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Eckhardt.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Eckhardt.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Fixed.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Fixed.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Furey.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Furey.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/LH.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/LH.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Local.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Local.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Slide.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Slide.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/UKIH.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/UKIH.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/Willems.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/Willems.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/five_day.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/five_day.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/methods/ihacres.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/methods/ihacres.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/param_estimate.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/param_estimate.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/separation.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/separation.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow/utils.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow/utils.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/baseflow_sep.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/baseflow_sep.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/hydrotoolbox.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/hydrotoolbox.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/indices/indices.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/indices/indices.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox/utils.py` & `hydrotoolbox-2.0.7/src/hydrotoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/PKG-INFO` & `hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrotoolbox
-Version: 2.0.6
+Version: 2.0.7
 Summary: Command line script and Python library for analysis of flow time-series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hydrotoolbox/docs/index.html#hydrotoolbox-documentation
 Project-URL: github, https://github.com/timcera/hydrotoolbox
 Project-URL: bitbucket, https://bitbucket.org/timcera/hydrotoolbox/src/main/
 Keywords: time-series,cli-app,hydrology,baseflow,hydrograph-recession,hydrographic
@@ -67,16 +67,26 @@
 
 Requirements
 ------------
 * python 3.7 or higher
 
 Installation
 ------------
-Should be as easy as running ``pip install hydrotoolbox``
-at any command line.
+pip
+~~~
+.. code-block:: bash
+
+    pip install hydrotoolbox
+
+conda
+~~~~~
+.. code-block:: bash
+
+    conda install -c conda-forge hydrotoolbox
+
 
 Usage - Command Line
 --------------------
 Just run 'hydrotoolbox --help' to get a list of subcommands::
 
 
     usage: hydrotoolbox [-h] [-v] {baseflow_sep,recession,about} ...
```

### Comparing `hydrotoolbox-2.0.6/src/hydrotoolbox.egg-info/SOURCES.txt` & `hydrotoolbox-2.0.7/src/hydrotoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/BEC_test.sh` & `hydrotoolbox-2.0.7/tests/BEC_test.sh`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data.csv` & `hydrotoolbox-2.0.7/tests/data.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_02239501.csv` & `hydrotoolbox-2.0.7/tests/data_02239501.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_boughton.csv` & `hydrotoolbox-2.0.7/tests/data_boughton.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_chapman.csv` & `hydrotoolbox-2.0.7/tests/data_chapman.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_cm.csv` & `hydrotoolbox-2.0.7/tests/data_cm.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_eckhardt.csv` & `hydrotoolbox-2.0.7/tests/data_eckhardt.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_ewma.csv` & `hydrotoolbox-2.0.7/tests/data_ewma.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_five_day.csv` & `hydrotoolbox-2.0.7/tests/data_five_day.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_furey.csv` & `hydrotoolbox-2.0.7/tests/data_furey.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_ihacres.csv` & `hydrotoolbox-2.0.7/tests/data_ihacres.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_lh.csv` & `hydrotoolbox-2.0.7/tests/data_lh.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_strict.csv` & `hydrotoolbox-2.0.7/tests/data_strict.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_ukih.csv` & `hydrotoolbox-2.0.7/tests/data_ukih.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_usgs_hysep_fixed.csv` & `hydrotoolbox-2.0.7/tests/data_usgs_hysep_fixed.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_usgs_hysep_local.csv` & `hydrotoolbox-2.0.7/tests/data_usgs_hysep_local.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_usgs_hysep_slide.csv` & `hydrotoolbox-2.0.7/tests/data_usgs_hysep_slide.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/data_willems.csv` & `hydrotoolbox-2.0.7/tests/data_willems.csv`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/hydrotoolbox_indices.txt` & `hydrotoolbox-2.0.7/tests/hydrotoolbox_indices.txt`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/run_test.sh` & `hydrotoolbox-2.0.7/tests/run_test.sh`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/test_baseflow_sep.py` & `hydrotoolbox-2.0.7/tests/test_baseflow_sep.py`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/tsproc_hydrologic_indices.inp` & `hydrotoolbox-2.0.7/tests/tsproc_hydrologic_indices.inp`

 * *Files identical despite different names*

### Comparing `hydrotoolbox-2.0.6/tests/tsproc_hydrologic_indices_percentile_test.inp` & `hydrotoolbox-2.0.7/tests/tsproc_hydrologic_indices_percentile_test.inp`

 * *Files identical despite different names*

