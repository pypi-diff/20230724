# Comparing `tmp/Patchview-0.2.9.tar.gz` & `tmp/Patchview-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Patchview-0.2.9.tar", last modified: Fri Dec 23 17:54:22 2022, max compression
+gzip compressed data, was "/home/miluky/Documents/patchview/dist/.tmp-8659qwdf/Patchview-0.3.0.tar", last modified: Mon Jul 24 18:25:07 2023, max compression
```

## Comparing `Patchview-0.2.9.tar` & `Patchview-0.3.0.tar`

### file list

```diff
@@ -1,105 +1,137 @@
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.281099 Patchview-0.2.9/
--rw-rw-rw-   0        0        0     1307 2022-12-21 21:23:12.000000 Patchview-0.2.9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       25 2022-12-21 21:23:12.000000 Patchview-0.2.9/HISTORY.rst
--rw-rw-rw-   0        0        0     1555 2022-12-21 21:23:12.000000 Patchview-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      473 2022-12-23 17:51:31.000000 Patchview-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3038 2022-12-23 17:54:22.281099 Patchview-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.188099 Patchview-0.2.9/Patchview.egg-info/
--rw-rw-rw-   0        0        0     3038 2022-12-23 17:54:22.000000 Patchview-0.2.9/Patchview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2800 2022-12-23 17:54:22.000000 Patchview-0.2.9/Patchview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-23 17:54:22.000000 Patchview-0.2.9/Patchview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-12-23 17:54:22.000000 Patchview-0.2.9/Patchview.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-21 23:00:40.000000 Patchview-0.2.9/Patchview.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      415 2022-12-23 17:54:22.000000 Patchview-0.2.9/Patchview.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-23 17:54:22.000000 Patchview-0.2.9/Patchview.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2446 2022-12-23 17:53:40.000000 Patchview-0.2.9/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.201098 Patchview-0.2.9/docs/
--rw-rw-rw-   0        0        0     1766 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/APIs.rst
--rw-rw-rw-   0        0        0      630 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/Makefile
--rw-rw-rw-   0        0        0     6338 2022-12-23 17:18:44.000000 Patchview-0.2.9/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/credits.rst
--rw-rw-rw-   0        0        0      346 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/index.rst
--rw-rw-rw-   0        0        0     6334 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/installation.rst
--rw-rw-rw-   0        0        0     5218 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/introduction.rst
--rwxrwxrwx   0        0        0      807 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/make.bat
--rw-rw-rw-   0        0        0       28 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/readme.rst
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.167099 Patchview-0.2.9/docs/resources/
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.206098 Patchview-0.2.9/docs/resources/icons/
--rw-rw-rw-   0        0        0     1146 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/icons/GP1.png
--rw-rw-rw-   0        0        0      732 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/icons/GPcorr.png
--rw-rw-rw-   0        0        0      383 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/icons/navigation.png
--rw-rw-rw-   0        0        0    42415 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/icons/neuron.png
--rw-rw-rw-   0        0        0      999 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/icons/rectangle.png
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.239099 Patchview-0.2.9/docs/resources/images/
--rw-rw-rw-   0        0        0   263017 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/FP_stats.png
--rw-rw-rw-   0        0        0   235641 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/FP_trace.png
--rw-rw-rw-   0        0        0    11902 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/PatchViewer.png
--rw-rw-rw-   0        0        0    12435 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/images/connectionTraces_loaded2.png
--rw-rw-rw-   0        0        0   102223 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/images/connections.png
--rw-rw-rw-   0        0        0    78021 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/images/couplingRatio.png
--rw-rw-rw-   0        0        0   139763 2022-12-23 17:13:40.000000 Patchview-0.2.9/docs/resources/images/density.png
--rw-rw-rw-   0        0        0  1312222 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/event_curate.png
--rw-rw-rw-   0        0        0   212714 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/event_detec.png
--rw-rw-rw-   0        0        0   890804 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/event_histExport.png
--rw-rw-rw-   0        0        0  1783491 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/event_sweep.png
--rw-rw-rw-   0        0        0  1140759 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/event_template.png
--rw-rw-rw-   0        0        0    31835 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/fp.png
--rw-rw-rw-   0        0        0   927525 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/images/measurePiaToSomas.png
--rw-rw-rw-   0        0        0    62169 2022-12-23 17:03:33.000000 Patchview-0.2.9/docs/resources/images/morphor_polar.png
--rw-rw-rw-   0        0        0    64865 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/images/morphor_tree.png
--rw-rw-rw-   0        0        0    86547 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/pasedavian_001_trace.png
--rw-rw-rw-   0        0        0    95936 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/pasedavian_002_multTraces.png
--rw-rw-rw-   0        0        0   211264 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/pasedavian_003_series.png
--rw-rw-rw-   0        0        0   152373 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/pasedavian_004_morphology.png
--rw-rw-rw-   0        0        0   123755 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources/images/pasedavian_004_morphology_soma.png
--rw-rw-rw-   0        0        0    96533 2022-12-22 23:41:51.000000 Patchview-0.2.9/docs/resources/images/shollAna1.png
--rw-rw-rw-   0        0        0    78834 2022-12-22 21:50:13.000000 Patchview-0.2.9/docs/resources/images/test_CR.png
--rw-rw-rw-   0        0        0     1806 2022-12-21 21:23:12.000000 Patchview-0.2.9/docs/resources.rst
--rw-rw-rw-   0        0        0    10623 2022-12-23 17:22:57.000000 Patchview-0.2.9/docs/tutorials.rst
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.247099 Patchview-0.2.9/patchview/
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.250099 Patchview-0.2.9/patchview/Data/
--rw-rw-rw-   0        0        0     1535 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.263100 Patchview-0.2.9/patchview/Data/icons/
--rw-rw-rw-   0        0        0     1146 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/GP1.png
--rw-rw-rw-   0        0        0      732 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/GP2.png
--rw-rw-rw-   0        0        0      732 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/GPcorr.png
--rw-rw-rw-   0        0        0    16958 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/PatchViewer.ico
--rw-rw-rw-   0        0        0    47689 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/connection.png
--rw-rw-rw-   0        0        0    17889 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/connection2.png
--rw-rw-rw-   0        0        0      383 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/navigation.png
--rw-rw-rw-   0        0        0    42415 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/neuron.png
--rw-rw-rw-   0        0        0      999 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/rectangle.png
--rw-rw-rw-   0        0        0     4565 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/settings.png
--rw-rw-rw-   0        0        0     1257 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/spikes.png
--rw-rw-rw-   0        0        0    12832 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/Data/icons/tree.png
--rw-rw-rw-   0        0        0      873 2022-12-22 21:50:13.000000 Patchview-0.2.9/patchview/Data/patchview.yaml
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.267099 Patchview-0.2.9/patchview/HekaIO/
--rw-rw-rw-   0        0        0    46768 2022-12-22 21:50:13.000000 Patchview-0.2.9/patchview/HekaIO/HEKA_Reader_MAIN.py
--rw-rw-rw-   0        0        0     6629 2022-12-22 21:50:13.000000 Patchview-0.2.9/patchview/HekaIO/HekaHelpers.py
--rw-rw-rw-   0        0        0        0 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/HekaIO/__init__.py
--rw-rw-rw-   0        0        0    16958 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/PatchViewer.ico
--rw-rw-rw-   0        0        0      338 2022-12-22 23:41:51.000000 Patchview-0.2.9/patchview/__init__.py
--rw-rw-rw-   0        0        0       17 2022-12-22 23:41:51.000000 Patchview-0.2.9/patchview/__version__.py
--rw-rw-rw-   0        0        0      483 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/enviroment-dev.yml
--rw-rw-rw-   0        0        0      486 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/enviroment.yml
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.270099 Patchview-0.2.9/patchview/ephys/
--rw-rw-rw-   0        0        0        0 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/ephys/__init__.py
--rw-rw-rw-   0        0        0    54924 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/ephys/ephys_extractor.py
--rw-rw-rw-   0        0        0    60732 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/ephys/ephys_features.py
--rw-rw-rw-   0        0        0   110395 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/ephys/extraEhpys_PV.py
--rw-rw-rw-   0        0        0       37 2022-12-21 21:23:12.000000 Patchview-0.2.9/patchview/main.py
--rw-rw-rw-   0        0        0   307458 2022-12-23 16:51:56.000000 Patchview-0.2.9/patchview/patchview.py
-drwxrwxrwx   0        0        0        0 2022-12-23 17:54:22.280099 Patchview-0.2.9/patchview/utilitis/
--rw-rw-rw-   0        0        0    35252 2022-12-23 00:00:37.000000 Patchview-0.2.9/patchview/utilitis/AllMyParsHere.py
--rw-rw-rw-   0        0        0     9135 2022-12-22 23:41:51.000000 Patchview-0.2.9/patchview/utilitis/AnalysisMethods.py
--rw-rw-rw-   0        0        0     8690 2022-09-09 18:27:05.000000 Patchview-0.2.9/patchview/utilitis/PVdat2NWB.py
--rw-rw-rw-   0        0        0        0 2022-12-21 21:23:13.000000 Patchview-0.2.9/patchview/utilitis/__init__.py
--rw-rw-rw-   0        0        0      342 2022-09-09 18:27:05.000000 Patchview-0.2.9/patchview/utilitis/debugHelpers.py
--rw-rw-rw-   0        0        0    11238 2022-09-09 18:27:05.000000 Patchview-0.2.9/patchview/utilitis/fitFuncs.py
--rw-rw-rw-   0        0        0    14373 2022-12-22 23:41:51.000000 Patchview-0.2.9/patchview/utilitis/morphorFeatureExtrator.py
--rw-rw-rw-   0        0        0    52281 2022-12-23 00:04:05.000000 Patchview-0.2.9/patchview/utilitis/patchviewObjects.py
--rw-rw-rw-   0        0        0      679 2022-12-21 21:23:13.000000 Patchview-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0      438 2022-12-23 17:38:36.000000 Patchview-0.2.9/requirements.txt
--rw-rw-rw-   0        0        0      639 2022-12-23 17:54:22.282099 Patchview-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2552 2022-12-23 17:54:11.000000 Patchview-0.2.9/setup.py
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.068726 Patchview-0.3.0/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      313 2023-07-24 15:57:38.000000 Patchview-0.3.0/.editorconfig
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.036726 Patchview-0.3.0/.github/
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.044726 Patchview-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      872 2023-07-24 15:57:38.000000 Patchview-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      615 2023-07-24 15:57:38.000000 Patchview-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      591 2023-07-24 16:06:50.000000 Patchview-0.3.0/.readthedocs.yaml
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      344 2023-07-24 15:57:38.000000 Patchview-0.3.0/.travis.yml
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     5343 2023-07-24 15:57:38.000000 Patchview-0.3.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1307 2023-07-24 15:57:38.000000 Patchview-0.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1514 2023-07-24 15:57:38.000000 Patchview-0.3.0/Credits.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)       25 2023-07-24 15:57:38.000000 Patchview-0.3.0/HISTORY.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1555 2023-07-24 15:57:38.000000 Patchview-0.3.0/LICENSE
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      473 2023-07-24 15:57:38.000000 Patchview-0.3.0/MANIFEST.in
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     2484 2023-07-24 15:57:38.000000 Patchview-0.3.0/Makefile
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     2880 2023-07-24 18:25:07.068726 Patchview-0.3.0/PKG-INFO
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.044726 Patchview-0.3.0/Patchview.egg-info/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     2880 2023-07-24 18:25:07.000000 Patchview-0.3.0/Patchview.egg-info/PKG-INFO
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     3641 2023-07-24 18:25:07.000000 Patchview-0.3.0/Patchview.egg-info/SOURCES.txt
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)        1 2023-07-24 18:25:07.000000 Patchview-0.3.0/Patchview.egg-info/dependency_links.txt
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)       42 2023-07-24 18:25:07.000000 Patchview-0.3.0/Patchview.egg-info/entry_points.txt
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)        1 2023-07-24 18:18:07.000000 Patchview-0.3.0/Patchview.egg-info/not-zip-safe
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      354 2023-07-24 18:25:07.000000 Patchview-0.3.0/Patchview.egg-info/requires.txt
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)       10 2023-07-24 18:25:07.000000 Patchview-0.3.0/Patchview.egg-info/top_level.txt
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     2519 2023-07-24 16:15:47.000000 Patchview-0.3.0/README.rst
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.048726 Patchview-0.3.0/docs/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1766 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/APIs.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      630 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/Makefile
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     6341 2023-07-24 16:10:12.000000 Patchview-0.3.0/docs/conf.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)       34 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/contributing.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)       29 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/credits.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      346 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/index.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     6824 2023-07-24 16:15:12.000000 Patchview-0.3.0/docs/installation.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     5218 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/introduction.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      807 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/make.bat
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)       28 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/readme.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)        4 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/requirements.txt
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.040726 Patchview-0.3.0/docs/resources/
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.048726 Patchview-0.3.0/docs/resources/icons/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1146 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/icons/GP1.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      732 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/icons/GPcorr.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      383 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/icons/navigation.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    42415 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/icons/neuron.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      999 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/icons/rectangle.png
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.060726 Patchview-0.3.0/docs/resources/images/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   263017 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/FP_stats.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   235641 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/FP_trace.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    16958 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/PatchViewer.ico
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    11902 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/PatchViewer.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    12435 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/connectionTraces_loaded2.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   102223 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/connections.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    78021 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/couplingRatio.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   139763 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/density.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)  1312222 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/event_curate.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   212714 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/event_detec.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   890804 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/event_histExport.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)  1783491 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/event_sweep.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)  1140759 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/event_template.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    31835 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/fp.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   927525 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/measurePiaToSomas.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    62169 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/morphor_polar.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    64865 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/morphor_tree.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    86547 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/pasedavian_001_trace.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    95936 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/pasedavian_002_multTraces.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   211264 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/pasedavian_003_series.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   152373 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/pasedavian_004_morphology.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   123755 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/pasedavian_004_morphology_soma.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)  1460027 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/patchview_ads.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    96533 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/shollAna1.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    78834 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources/images/test_CR.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1806 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/resources.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    10657 2023-07-24 15:57:38.000000 Patchview-0.3.0/docs/tutorials.rst
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      439 2023-07-24 15:57:38.000000 Patchview-0.3.0/enviroment-dev.yml
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      448 2023-07-24 15:57:38.000000 Patchview-0.3.0/environment.yml
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.060726 Patchview-0.3.0/patchview/
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.064726 Patchview-0.3.0/patchview/Data/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      508 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/JiangLab_protocols.yaml
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1535 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/LICENSE.txt
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      229 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/NDX_files
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1586 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/Navigator.ui
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.064726 Patchview-0.3.0/patchview/Data/icons/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1146 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/GP1.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      732 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/GP2.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      732 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/GPcorr.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    16958 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/PatchViewer.ico
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    47689 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/connection.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    17889 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/connection2.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      383 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/navigation.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    42415 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/neuron.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      999 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/rectangle.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     4565 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/settings.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1257 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/spikes.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    12832 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/icons/tree.png
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      973 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/Data/patchview.yaml
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.064726 Patchview-0.3.0/patchview/HekaIO/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    46768 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/HekaIO/HEKA_Reader_MAIN.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     7116 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/HekaIO/HekaHelpers.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)        0 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/HekaIO/__init__.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    16958 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/PatchViewer.ico
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      338 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/__init__.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)       17 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/__version__.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      483 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/enviroment-dev.yml
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      486 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/enviroment.yml
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.068726 Patchview-0.3.0/patchview/ephys/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)        0 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/ephys/__init__.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    55305 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/ephys/ephys_extractor.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    60946 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/ephys/ephys_features.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   110595 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/ephys/extraEhpys_PV.py
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.068726 Patchview-0.3.0/patchview/examples/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1348 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/examples/load_spike_list.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)       37 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/main.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)   357851 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/patchview.py
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.068726 Patchview-0.3.0/patchview/utilitis/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    39404 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/AllMyParsHere.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     9135 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/AnalysisMethods.py
+drwxrwxr-x   0 miluky    (1000) miluky    (1000)        0 2023-07-24 18:25:07.068726 Patchview-0.3.0/patchview/utilitis/NDX_files/
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     1766 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/NDX_files/XiaolongJiangLab.extensions.yaml
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      229 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/NDX_files/XiaolongJiangLab.namespace.yaml
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    14476 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/PVdat2NWB.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)        0 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/__init__.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     4925 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/dandi2pvNWB.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      342 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/debugHelpers.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    10281 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/emfDraw.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    11238 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/fitFuncs.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      749 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/graphictools.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     2827 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/linecollection_update.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    29249 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/morphorFeatureExtrator.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    55429 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/patchviewObjects.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     6781 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/patchview_ndx.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)    25164 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/pvEphy.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     7536 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/pvNDX_class.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      432 2023-07-24 15:57:38.000000 Patchview-0.3.0/patchview/utilitis/pyqtgraph_helpers.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      480 2023-07-24 18:21:55.000000 Patchview-0.3.0/pyproject.toml
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      377 2023-07-24 16:02:24.000000 Patchview-0.3.0/requirements.txt
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      603 2023-07-24 18:25:07.072726 Patchview-0.3.0/setup.cfg
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)     2594 2023-07-24 18:24:51.000000 Patchview-0.3.0/setup.py
+-rw-rw-r--   0 miluky    (1000) miluky    (1000)      574 2023-07-24 15:57:38.000000 Patchview-0.3.0/tox.ini
```

### Comparing `Patchview-0.2.9/CONTRIBUTING.rst` & `Patchview-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/LICENSE` & `Patchview-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/PKG-INFO` & `Patchview-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,70 @@
-Metadata-Version: 2.1
-Name: Patchview
-Version: 0.2.9
-Summary: GUI software for data analysis and visualization on whole-cell recording data
-Home-page: https://github.com/zeitgeberH/patchview
-Author: Ming Hu
-Author-email: 
-License: BSD 3-Clause License
-Keywords: patchview
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
-===============
-PatchView
-===============
-.. image:: https://img.shields.io/pypi/v/patchview.svg 
-        :target: https://pypi.python.org/pypi/patchview
-      
-.. image:: https://img.shields.io/badge/python-3.8%2B-blue
-        :target: https://www.python.org/downloads/release/python
-        :alt: Python3.8
-
-.. image:: https://readthedocs.org/projects/patchview/badge/?version=latest
-        :target: https://patchview.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-
-.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-        :target: https://opensource.org/licenses/BSD-3-Clause
-        :alt: BSD-3-Clause    
-
-.. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
-   :target: https://doi.org/10.21105/joss.04706
-.. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
-           
-PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
-synaptic connection detection, morphological analysis and more.
-
-* Free software: BSD 3-Clause license
-* Documentation: https://patchview.readthedocs.io.
-
-
-Features
---------
-PatchView integrates multiple open-source tools (see credit page) and wrap them using an intuitive graphic user interface (GUI).
-Thus users can perform most analysis quickly for the data collected in a typical patch-clamp experiment without installing Python and 
-these tools or writing any Python scripts.
-
-* Importing both Heka data and Axon Instruments data. Exporting to Python pickle file or NWB (Neurodata Without Borders) file format.
-* Visualizing single and multiple traces with zoom, pan operations.
-* Automatically sorting experiments data according to predefined labels.
-* Performing analysis on intrinsic membrane properties, action potential detection, firing pattern analysis.
-* Synaptic connection analysis.
-* Visualizing and quantification of neuron's morphological reconstruction from Neurolucida
-
-
-Citation
----------
-If you find our work useful for your research, please cite:
-
-    Hu et al., (2022). PatchView: A Python Package for Patch-clamp Data Analysis and Visualization. Journal of Open Source Software, 7(78), 4706, https://doi.org/10.21105/joss.04706
+Metadata-Version: 2.1
+Name: Patchview
+Version: 0.3.0
+Summary: data analysis and visualization on whole-cell data
+Home-page: https://github.com/zeitgeberH/patchview
+Author: Ming Hu
+Author-email: hi@gmail.com
+License: BSD-3-Clause
+Keywords: patch-clamp,data analysis
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
+===============
+PatchView
+===============
+.. image:: https://img.shields.io/pypi/v/patchview.svg 
+        :target: https://pypi.python.org/pypi/patchview
+      
+.. image:: https://img.shields.io/badge/python-3.8%2B-blue
+        :target: https://www.python.org/downloads/release/python
+        :alt: Python3.8
+
+.. image:: https://readthedocs.org/projects/patchview/badge/?version=latest
+        :target: https://patchview.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+        :target: https://opensource.org/licenses/BSD-3-Clause
+        :alt: BSD-3-Clause    
+
+.. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
+   :target: https://doi.org/10.21105/joss.04706
+.. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
+           
+
+.. image:: docs/resources/images/patchview_ads.png
+    :width: 800
+
+PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
+synaptic connection detection, morphological analysis and more.
+
+* Free software: BSD 3-Clause license
+* Documentation: https://patchview.readthedocs.io.
+
+
+Features
+--------
+PatchView integrates multiple open-source tools (see credit page) and wrap them using an intuitive graphic user interface (GUI).
+Thus users can perform most analysis quickly for the data collected in a typical patch-clamp experiment without installing Python and 
+these tools or writing any Python scripts.
+
+* Importing both Heka data and Axon Instruments data. Exporting to Python pickle file or NWB (Neurodata Without Borders) file format.
+* Visualizing single and multiple traces with zoom, pan operations.
+* Automatically sorting experiments data according to predefined labels.
+* Performing analysis on intrinsic membrane properties, action potential detection, firing pattern analysis.
+* Synaptic connection analysis.
+* Visualizing and quantification of neuron's morphological reconstruction from Neurolucida
+
+
+Citation
+---------
+If you find our work useful for your research, please cite:
+
+    Hu et al., (2022). PatchView: A Python Package for Patch-clamp Data Analysis and Visualization. Journal of Open Source Software, 7(78), 4706, https://doi.org/10.21105/joss.04706
```

### Comparing `Patchview-0.2.9/Patchview.egg-info/PKG-INFO` & `Patchview-0.3.0/Patchview.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,70 @@
-Metadata-Version: 2.1
-Name: Patchview
-Version: 0.2.9
-Summary: GUI software for data analysis and visualization on whole-cell recording data
-Home-page: https://github.com/zeitgeberH/patchview
-Author: Ming Hu
-Author-email: 
-License: BSD 3-Clause License
-Keywords: patchview
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
-===============
-PatchView
-===============
-.. image:: https://img.shields.io/pypi/v/patchview.svg 
-        :target: https://pypi.python.org/pypi/patchview
-      
-.. image:: https://img.shields.io/badge/python-3.8%2B-blue
-        :target: https://www.python.org/downloads/release/python
-        :alt: Python3.8
-
-.. image:: https://readthedocs.org/projects/patchview/badge/?version=latest
-        :target: https://patchview.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-
-.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-        :target: https://opensource.org/licenses/BSD-3-Clause
-        :alt: BSD-3-Clause    
-
-.. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
-   :target: https://doi.org/10.21105/joss.04706
-.. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
-           
-PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
-synaptic connection detection, morphological analysis and more.
-
-* Free software: BSD 3-Clause license
-* Documentation: https://patchview.readthedocs.io.
-
-
-Features
---------
-PatchView integrates multiple open-source tools (see credit page) and wrap them using an intuitive graphic user interface (GUI).
-Thus users can perform most analysis quickly for the data collected in a typical patch-clamp experiment without installing Python and 
-these tools or writing any Python scripts.
-
-* Importing both Heka data and Axon Instruments data. Exporting to Python pickle file or NWB (Neurodata Without Borders) file format.
-* Visualizing single and multiple traces with zoom, pan operations.
-* Automatically sorting experiments data according to predefined labels.
-* Performing analysis on intrinsic membrane properties, action potential detection, firing pattern analysis.
-* Synaptic connection analysis.
-* Visualizing and quantification of neuron's morphological reconstruction from Neurolucida
-
-
-Citation
----------
-If you find our work useful for your research, please cite:
-
-    Hu et al., (2022). PatchView: A Python Package for Patch-clamp Data Analysis and Visualization. Journal of Open Source Software, 7(78), 4706, https://doi.org/10.21105/joss.04706
+Metadata-Version: 2.1
+Name: Patchview
+Version: 0.3.0
+Summary: data analysis and visualization on whole-cell data
+Home-page: https://github.com/zeitgeberH/patchview
+Author: Ming Hu
+Author-email: hi@gmail.com
+License: BSD-3-Clause
+Keywords: patch-clamp,data analysis
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
+===============
+PatchView
+===============
+.. image:: https://img.shields.io/pypi/v/patchview.svg 
+        :target: https://pypi.python.org/pypi/patchview
+      
+.. image:: https://img.shields.io/badge/python-3.8%2B-blue
+        :target: https://www.python.org/downloads/release/python
+        :alt: Python3.8
+
+.. image:: https://readthedocs.org/projects/patchview/badge/?version=latest
+        :target: https://patchview.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+        :target: https://opensource.org/licenses/BSD-3-Clause
+        :alt: BSD-3-Clause    
+
+.. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
+   :target: https://doi.org/10.21105/joss.04706
+.. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
+           
+
+.. image:: docs/resources/images/patchview_ads.png
+    :width: 800
+
+PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
+synaptic connection detection, morphological analysis and more.
+
+* Free software: BSD 3-Clause license
+* Documentation: https://patchview.readthedocs.io.
+
+
+Features
+--------
+PatchView integrates multiple open-source tools (see credit page) and wrap them using an intuitive graphic user interface (GUI).
+Thus users can perform most analysis quickly for the data collected in a typical patch-clamp experiment without installing Python and 
+these tools or writing any Python scripts.
+
+* Importing both Heka data and Axon Instruments data. Exporting to Python pickle file or NWB (Neurodata Without Borders) file format.
+* Visualizing single and multiple traces with zoom, pan operations.
+* Automatically sorting experiments data according to predefined labels.
+* Performing analysis on intrinsic membrane properties, action potential detection, firing pattern analysis.
+* Synaptic connection analysis.
+* Visualizing and quantification of neuron's morphological reconstruction from Neurolucida
+
+
+Citation
+---------
+If you find our work useful for your research, please cite:
+
+    Hu et al., (2022). PatchView: A Python Package for Patch-clamp Data Analysis and Visualization. Journal of Open Source Software, 7(78), 4706, https://doi.org/10.21105/joss.04706
```

### Comparing `Patchview-0.2.9/README.rst` & `Patchview-0.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         :target: https://opensource.org/licenses/BSD-3-Clause
         :alt: BSD-3-Clause    
 
 .. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
    :target: https://doi.org/10.21105/joss.04706
 .. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
            
+
+.. image:: docs/resources/images/patchview_ads.png
+    :width: 800
+
 PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
 synaptic connection detection, morphological analysis and more.
 
 * Free software: BSD 3-Clause license
 * Documentation: https://patchview.readthedocs.io.
```

### Comparing `Patchview-0.2.9/docs/APIs.rst` & `Patchview-0.3.0/docs/APIs.rst`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/Makefile` & `Patchview-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/conf.py` & `Patchview-0.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
 sys.path.insert(0, os.path.abspath('..'))
-import patchview.__version__
+# import patchview.__version__
 
 from typing import Any, Dict
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
@@ -45,29 +45,29 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'PatchView'
-copyright = u"2022, Ming Hu"
+copyright = u"2022-, Ming Hu"
 author = u"Ming Hu"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # # The short X.Y version.
 # version =  patchview.__version__
 # # The full version, including alpha/beta/rc tags.
 # release =  patchview.__version__
 
-version =  "0.2.9"
+version =  "0.3.0"
 # The full version, including alpha/beta/rc tags.
-release =  "0.2.9"
+release =  "0.3.0"
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
@@ -86,15 +86,15 @@
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'furo' #'alabaster'
+html_theme = "furo" #'alabaster'
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
```

### Comparing `Patchview-0.2.9/docs/installation.rst` & `Patchview-0.3.0/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,20 @@
 If this does not resolve the issue, please open a PatchView's github issue.
 
 **Note 2**
 Tested platforms: Windows 10, Ubuntu 18.04 LTS, Mac Catalina. 
 Due to Qt requriment, it won't work under WSL2 in Windows 10. 
 With enhanced GUI support on WSL2 in Windows 11, it may work (but not tested yet)
 
+MacOS user: Please make sure you have `cairo` installed. You can install it via `brew`:
+
+.. code-block:: console
+    
+    $ brew install cairo 
+
 From sources
 ------------
 
 The sources for PatchView can be downloadeded from the `Github repo`_.
 
 You can either clone the public repository:
 
@@ -119,20 +125,30 @@
 
 then activate the environment and run:
 
 .. code-block:: console
 
     $ conda activate patchviewPy3
     
-    $ pip install -r requirement.txt ## install requirement
+The following three packages should be installed from their github repo:
+
+.. code-block:: console
+
+    $ pip install git+https://github.com/ZeitgeberH/NeuroM@patchview#egg=NeuroM
+
+    $ pip install git+https://github.com/ZeitgeberH/dictdiffer#egg=dictdiffer
+
+    $ pip install git+https://github.com/jeremysanders/pyemf3#egg=pyemf3
 
 Finally, 
 
 .. code-block:: console
-    
+
+    $ pip install -r requirement.txt ## install requirement
+
     $ pip install -e .
     
 .. _Pyinstaller: https://pyinstaller.org/en/stable/   
 .. _Github repo: https://github.com/zeitgeberH/patchview
 .. _tarball: https://github.com/zeitgeberH/patchview/tarball/master
```

### Comparing `Patchview-0.2.9/docs/introduction.rst` & `Patchview-0.3.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/make.bat` & `Patchview-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/icons/GP1.png` & `Patchview-0.3.0/docs/resources/icons/GP1.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/icons/GPcorr.png` & `Patchview-0.3.0/docs/resources/icons/GPcorr.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/icons/neuron.png` & `Patchview-0.3.0/docs/resources/icons/neuron.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/icons/rectangle.png` & `Patchview-0.3.0/docs/resources/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/FP_stats.png` & `Patchview-0.3.0/docs/resources/images/FP_stats.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/FP_trace.png` & `Patchview-0.3.0/docs/resources/images/FP_trace.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/PatchViewer.png` & `Patchview-0.3.0/docs/resources/images/PatchViewer.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/connectionTraces_loaded2.png` & `Patchview-0.3.0/docs/resources/images/connectionTraces_loaded2.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/connections.png` & `Patchview-0.3.0/docs/resources/images/connections.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/couplingRatio.png` & `Patchview-0.3.0/docs/resources/images/couplingRatio.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/density.png` & `Patchview-0.3.0/docs/resources/images/density.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/event_curate.png` & `Patchview-0.3.0/docs/resources/images/event_curate.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/event_detec.png` & `Patchview-0.3.0/docs/resources/images/event_detec.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/event_histExport.png` & `Patchview-0.3.0/docs/resources/images/event_histExport.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/event_sweep.png` & `Patchview-0.3.0/docs/resources/images/event_sweep.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/event_template.png` & `Patchview-0.3.0/docs/resources/images/event_template.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/fp.png` & `Patchview-0.3.0/docs/resources/images/fp.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/measurePiaToSomas.png` & `Patchview-0.3.0/docs/resources/images/measurePiaToSomas.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/morphor_polar.png` & `Patchview-0.3.0/docs/resources/images/morphor_polar.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/morphor_tree.png` & `Patchview-0.3.0/docs/resources/images/morphor_tree.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/pasedavian_001_trace.png` & `Patchview-0.3.0/docs/resources/images/pasedavian_001_trace.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/pasedavian_002_multTraces.png` & `Patchview-0.3.0/docs/resources/images/pasedavian_002_multTraces.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/pasedavian_003_series.png` & `Patchview-0.3.0/docs/resources/images/pasedavian_003_series.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/pasedavian_004_morphology.png` & `Patchview-0.3.0/docs/resources/images/pasedavian_004_morphology.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/pasedavian_004_morphology_soma.png` & `Patchview-0.3.0/docs/resources/images/pasedavian_004_morphology_soma.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/shollAna1.png` & `Patchview-0.3.0/docs/resources/images/shollAna1.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources/images/test_CR.png` & `Patchview-0.3.0/docs/resources/images/test_CR.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/resources.rst` & `Patchview-0.3.0/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/docs/tutorials.rst` & `Patchview-0.3.0/docs/tutorials.rst`

 * *Files 4% similar despite different names*

```diff
@@ -133,30 +133,32 @@
 Patchview currently only support neurolucida ASC files. These files should be listed in the file browser panel.
 Double clicking the file would load the file. Visualization and further analysis results are shown in the `Morphology` tab.
 
 Dependent on the content of the file, Patchview can perform:
 
 * **pairwise distance of multiple somas**: this is automatically done if the reconstruction has multiple somas in it (check the test file: `test_multiSoma.ASC`)
 
-*  **Update cell names**: this can be done for a multi-soma file. The `Name` column in the `Summary` table can be edited. After the editing, clicking `Update cell names` will update the Pair names in the  pairwise distance table  in `Distance (um)` tab. 
+*  **Update cell names**: this can be done for a multi-soma file. The `Name` column in the `Summary` table can be edited. After the editing, clicking `Update cell names` will update the Pair names in the  pairwise distance table  in `Distance (um)` tab.
   
 * **Sholl analysis**: if the reconstruction has at least one neurite, this will perform Sholl analysis (counting neurite numbers in a ring from certain soma distance). A line plot (count vs distance) is shown in the `Figures` tab. Try `test.ASC`.
 
 .. image:: resources/images/morphor_tree.png
     :width: 800
     :alt: Alternative text
 
-* **Density analysis**: in either cartesian or polar coordinates
+* **Density analysis**: Visualizing neurites density in either Cartesian or polar coordinates.
+  
 .. image:: resources/images/density.png
     :width: 800
-    :alt: Alternative text
+    :alt: Alternative tex
     
 .. image:: resources/images/morphor_polar.png
     :width: 400
     :alt: Alternative text
+
 *  **Distance to Pia**: if the reconstruction contains a entry labeled "Pia" (check the test file: `test_multiSoma.ASC`), this will measure Euclidean distance from the center of a soma to the Pia. Measured results are shown in the `Distance to Pia` column in `Summary` table.
 
 .. image:: resources/images/measurePiaToSomas.png
     :width: 800
     :alt: Alternative text
 
 **Note**: the figure sometimes (more so under Ubuntu) does not automatically refresh. If it happens, drag the border between upper and lower panels to manually refresh.
```

### Comparing `Patchview-0.2.9/patchview/Data/LICENSE.txt` & `Patchview-0.3.0/patchview/Data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/GP1.png` & `Patchview-0.3.0/patchview/Data/icons/GP1.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/GP2.png` & `Patchview-0.3.0/patchview/Data/icons/GP2.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/GPcorr.png` & `Patchview-0.3.0/patchview/Data/icons/GPcorr.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/PatchViewer.ico` & `Patchview-0.3.0/docs/resources/images/PatchViewer.ico`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/connection.png` & `Patchview-0.3.0/patchview/Data/icons/connection.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/connection2.png` & `Patchview-0.3.0/patchview/Data/icons/connection2.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/neuron.png` & `Patchview-0.3.0/patchview/Data/icons/neuron.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/rectangle.png` & `Patchview-0.3.0/patchview/Data/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/settings.png` & `Patchview-0.3.0/patchview/Data/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/spikes.png` & `Patchview-0.3.0/patchview/Data/icons/spikes.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/icons/tree.png` & `Patchview-0.3.0/patchview/Data/icons/tree.png`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/Data/patchview.yaml` & `Patchview-0.3.0/patchview/Data/patchview.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-RootDir: ''
+RootDir: 'D:\'
 Filters: ## filter cut off frequency for  Bessel or Butterworth filter. unit of Hz.
     Option: 0 ## default Bessel, 1 for Butterworth
     High cutoff: 10000.0
 CleanUp: ## data clean-up criterias
     minimalSweeps: 3 ## at least three sweeps to use!
 Protocols:  ## existing patch protocols and alias
-    Firing pattern: ['FP', 'fp', 'Firing Pattern', 'firing pattern','AllCurrentClamp','ap','ramp']
+    Firing pattern: ['FP', 'fp', 'Firing Pattern', 'firing pattern','AllCurrentClamp','ap','ramp',
+    'LongSquareWave']
     Connection: ['STI', 'Sti', 'Cc', 'cc']  ## check connections
     Retina: ['Light_stimulation', 'light stimulation']  ## check light response
-    Spontaneous: ['EPSP', 'EPSPs','EPSC', 'EPSCs', 'sEPSP','sEPSPs','sEPSC','sEPSCs', \
+    Spontaneous: ['EPSP', 'EPSPs','EPSC', 'EPSCs', 'sEPSP','sEPSPs','sEPSC','sEPSCs',
     'SP','SP_VC', 'SP_CC','Spontaneous Inputs','Spontaneous','sAP']  
-      
 Visulization:
     Plot stim: 1  ## if stim is used, plot it along the raw traces
     Downsampling: 1.0  ## plot less points to speed up
+    Default figure DPI: 100 ## matplotlib figure dot per inch
+    SpikeColor: 'r'
```

### Comparing `Patchview-0.2.9/patchview/HekaIO/HEKA_Reader_MAIN.py` & `Patchview-0.3.0/patchview/HekaIO/HEKA_Reader_MAIN.py`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/HekaIO/HekaHelpers.py` & `Patchview-0.3.0/patchview/HekaIO/HekaHelpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 
 @author: MHu
 """
 from patchview.HekaIO import HEKA_Reader_MAIN as HEKA
 import os
 import numpy as np
 
-
+RECORDMODE = [
+    "In out",
+    "On Cell",
+    "Out Out",
+    "Whole cell",
+    "C-Clamp",
+    "------",
+    "------",
+]
 class HekaBundleInfo(object):
     """
     A helpr class wrap aound HEKA reader
     """
 
     def __init__(self, filePath):
         self.bundle = None
@@ -151,14 +159,22 @@
         ):  ## it happens that experimenter label is not consistent with actual trace count
             print(
                 f"single trace series. Sweep label is not consistent with trace index {idx[-1]}"
             )
             idx[-1] = 0
         return self.bundle.data[idx]
 
+    def getTraceRecordingMode(self, idx:list[int, int, int, int]):
+        assert len(idx) == 4, "trace index need to be a list of 4 integers"
+        trace = self.bundle.pul[idx[0]][idx[1]][idx[2]][idx[3]]
+        modeIdx = int.from_bytes(
+            trace.RecordingMode, byteorder=self.bundle.endian
+        ) 
+        return RECORDMODE[modeIdx]
+
     def getTraceUnit(self, idx):
         print("Not implemented!")
 
     def getNumberOfSamplesPerSweep(self, idx):
         # assert isinstance(idx, list) and len(idx) == 4 , 'series index need to be a list with length of 4'
         return self.bundle.data[idx].shape[0]
```

### Comparing `Patchview-0.2.9/patchview/PatchViewer.ico` & `Patchview-0.3.0/patchview/Data/icons/PatchViewer.ico`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/ephys/ephys_extractor.py` & `Patchview-0.3.0/patchview/ephys/ephys_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         dv_cutoff=20.0,
         max_interval=0.005,
         min_height=2.0,
         min_peak=-30.0,
         thresh_frac=0.05,
         baseline_interval=0.1,
         baseline_detect_thresh=0.3,
+        start_latency = 0.001, ## minimal latency for threshold crossing
         id=None,
     ):
         """Initialize SweepFeatures object.
 
         Parameters
         ----------
         t : ndarray of times (seconds)
@@ -101,15 +102,15 @@
         self.max_interval = max_interval
         self.min_height = min_height
         self.min_peak = min_peak
         self.thresh_frac = thresh_frac
         self.baseline_interval = baseline_interval
         self.baseline_detect_thresh = baseline_detect_thresh
         self.stimulus_amplitude_calculator = None
-
+        self.start_latency = start_latency
         self._sweep_features = {}
         self._affected_by_clipping = []
 
     def process_spikes(self):
         """Perform spike-related feature analysis"""
         self._process_individual_spikes()
         self._process_spike_related_features()
@@ -140,16 +141,21 @@
             # Save time if no spikes detected
             self._spikes_df = DataFrame()
             return
 
         upstrokes = ft.find_upstroke_indexes(
             v, t, putative_spikes, peaks, self.filter, dvdt
         )
-        thresholds = ft.refine_threshold_indexes(
-            v, t, upstrokes, thresh_frac=self.thresh_frac, filter=self.filter, dvdt=dvdt
+        # thresholds = ft.refine_threshold_indexes(
+        #     v, t, upstrokes, thresh_frac=self.thresh_frac, filter=self.filter, dvdt=dvdt
+        # )
+        if self.start is None:
+            self.start = 0
+        thresholds = ft.refine_threshold_indexes_updated(
+            v, t, upstrokes, start = self.start+self.start_latency, thresh_frac=self.thresh_frac, filter=self.filter, dvdt=dvdt
         )
         thresholds, peaks, upstrokes, clipped = ft.check_thresholds_and_peaks(
             v,
             t,
             thresholds,
             peaks,
             upstrokes,
```

### Comparing `Patchview-0.2.9/patchview/ephys/ephys_features.py` & `Patchview-0.3.0/patchview/ephys/ephys_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
     now too.
 
     Parameters
     ----------
     v : numpy array of voltage time series in mV
     t : numpy array of times in seconds
     upstroke_indexes : numpy array of indexes of spike upstrokes (for threshold target calculation)
+    start : start time for threshold calculation (optional, default 0)
     thresh_frac : fraction of average upstroke for threshold calculation (optional, default 0.05)
     filter : cutoff frequency for 4-pole low-pass Bessel filter in kHz (optional, default 10)
     dvdt : pre-calculated time-derivative of voltage (optional)
 
     Returns
     -------
     threshold_indexes : numpy array of threshold indexes
@@ -279,21 +280,25 @@
 
     upstrokes_and_start = np.append(np.array([start_index]), upstroke_indexes)
     threshold_indexes = []
     for upstk, upstk_prev in zip(upstrokes_and_start[1:], upstrokes_and_start[:-1]):
         if upstk_prev == start_index and not upstk_prev == find_time_index(
             t, 0.1
         ):  # Too steep depolarisations
-            threshold_indexes.append(upstk - np.argmin(dvdt[upstk:upstk_prev:-1]))
+            try:
+                threshold_indexes.append(upstk - np.argmin(dvdt[upstk:upstk_prev:-1]))
+            except:
+                threshold_indexes.append(upstk_prev)
             continue
         potential_indexes = np.flatnonzero(dvdt[upstk:upstk_prev:-1] <= target)
         if not potential_indexes.size:
             # couldn't find a matching value for threshold,
             # so just going to the start of the search interval
             threshold_indexes.append(upstk_prev)
+            print('Too steep depolarisation')
         else:
             threshold_indexes.append(upstk - potential_indexes[0])
 
     return np.array(threshold_indexes)
 
 
 def refine_threshold_indexes(
@@ -776,15 +781,14 @@
         - t[width_starts[~missing_widths].astype(int)]
     )
     if any(missing_widths):
         widths[missing_widths] = np.nan
 
     return widths
 
-
 def analyze_trough_details(
     v,
     t,
     spike_indexes,
     peak_indexes,
     clipped=None,
     end=None,
```

### Comparing `Patchview-0.2.9/patchview/ephys/extraEhpys_PV.py` & `Patchview-0.3.0/patchview/ephys/extraEhpys_PV.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,31 +41,32 @@
         dv_cutoff=20.0,
         max_interval=0.005,
         min_height=2.0,
         min_peak=-30.0,
         thresh_frac=0.05,
         baseline_interval=0.1,
         baseline_detect_thresh=0.3,
+        start_latency=0.005,
     ):
         self.time = time  ## time in second
         self.data = data * 1000  ## memebrane voltage in unit of mV
+        self.start_latency = start_latency  ## start latency in second
         self.stim_start = (
             stimInfo[0][1]["start"] * stimInfo[0][1]["sampleInteval"]
         )  ## stimuli start
         self.stim_end = (
             stimInfo[0][1]["end"] * stimInfo[0][1]["sampleInteval"]
         )  ## stimuli end
         self.title = title  ## contain the file name + lable of current node
         current_amp = []  ## stimuli amplitude
         for x in stimInfo:
             current_amp.append(
                 x[1]["amplitude"]
             )  ## we are using the relative current. As the ephys_extrator assume baseline current is zero pA)  ## pA
         self.current = current_amp
-        print(current_amp)
         self.current0_index = np.argsort(np.abs(current_amp))[0]
         self.current_step = np.diff(current_amp)[0]  ## assume constant step
         self.Vholding = x[1]["Vholding"]  ## holding current
         self.sampleRate = 1 / stimInfo[0][1]["sampleInteval"]
         if filterHighCutFreq == None:
             if self.sampleRate > 2.1e4:  ## sampling rate larger than 20K hz
                 self.filterHighCutFreq = 10  ## 10 KHz
@@ -87,14 +88,15 @@
             dv_cutoff=dv_cutoff,
             max_interval=max_interval,
             min_height=min_height,
             min_peak=min_peak,
             thresh_frac=thresh_frac,
             baseline_interval=baseline_interval,
             baseline_detect_thresh=baseline_detect_thresh,
+            start_latency = start_latency,
         )
         self.Cell_Features = self.get_cell_features()
 
     def data_preparation_pickle(pickleObject):
         """data_preparation_pickled object import the data exported from patchviewer and returns the voltage
         traces, stimulus current magnitudes for all traces and the time trace.
 
@@ -149,14 +151,15 @@
         dv_cutoff=20.0,
         max_interval=0.005,
         min_height=2.0,
         min_peak=-30.0,
         thresh_frac=0.05,
         baseline_interval=0.1,
         baseline_detect_thresh=0.3,
+        start_latency = 0.001,
     ):
         """Analyse the voltage traces and extract information for every spike (returned in df), and information for all the spikes
         per current stimulus magnitude.
         Returns
         -------
         df : DataFrame with information for every detected spike (peak_v, peak_index, threshold_v, ...)
         df_related_features : DataFrame with information for every possible used current stimulation magnitude
@@ -194,14 +197,15 @@
                     dv_cutoff=dv_cutoff,
                     max_interval=max_interval,
                     min_height=min_height,
                     min_peak=min_peak,
                     thresh_frac=thresh_frac,
                     baseline_interval=baseline_interval,
                     baseline_detect_thresh=baseline_detect_thresh,
+                    start_latency=start_latency,
                 )
                 EphysObject.process_spikes()
 
                 # Adding peak_height (mV) + code for maximum frequency determination (see further)
                 spike_count = 0
                 if EphysObject._spikes_df.size:
                     EphysObject._spikes_df["peak_height"] = (
```

### Comparing `Patchview-0.2.9/patchview/patchview.py` & `Patchview-0.3.0/patchview/patchview.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,88 +1,112 @@
 """
 Patchviewer by M.H.
 """
 from PyQt5 import QtGui, QtWidgets, QtCore
 from PyQt5.QtWidgets import QMessageBox, QTableWidgetItem
+from PyQt5.QtWidgets import QSplitter
 import pyqtgraph as pg
 import pyqtgraph.opengl as gl
 from pyqtgraph.parametertree import Parameter, ParameterTree
 from patchview.utilitis import AllMyParsHere as AllMyPars
+from patchview.utilitis.pyqtgraph_helpers import * # helper functions for pyqtgraph
 import sys
 import os
 import numpy as np
 import pandas as pd
 from patchview.HekaIO import HEKA_Reader_MAIN as HEKA
 from patchview.HekaIO.HekaHelpers import HekaBundleInfo
 from scipy import signal
 import scipy.stats as stats
 from scipy.optimize import curve_fit
 import seaborn as sns
 sns.despine()
+sns.set_style("whitegrid")
+import yaml
+import dictdiffer
+from sklearn.metrics import _pairwise_distances_reduction
+from sklearn.metrics._pairwise_distances_reduction import (_datasets_pair, _middle_term_computer)
 from patchview.ephys import ephys_features as ephys_ft
 from patchview.ephys import ephys_extractor as efex
 from patchview.ephys import extraEhpys_PV
 from patchview.ephys.extraEhpys_PV import extract_sweep_feature
 from scipy.stats import pearsonr
 import itertools
 import time as sysTime
 from copy import deepcopy
 import glob
+import pickle
+from patchview.utilitis.linecollection_update import FigureUpdater
 from patchview.utilitis.debugHelpers import debugInfo
 from patchview.utilitis.AnalysisMethods import (
     loadYAML,
     filterDatSeries,
     calculateConnectionTraces,
     cleanASCfile,
     smooth, smooth2D, padding_
 )
+import shapely._geos
+import neurom
+from morphopy.computation.feature_presentation import compute_morphometric_statistics
 from neurom.geom.transform import (translate, rotate)
 from patchview.utilitis import fitFuncs
 from patchview.utilitis.morphorFeatureExtrator import (
-    getSomaStats, extractMorphFeatures, sholl_analysis,
-     sholl_single_axis,sholl_2D_density, sholl_polar)
+    getSomaStats, extractMorphFeatures, sholl_analysis,resampleNeurite,
+     sholl_single_axis,sholl_2D_density, sholl_polar,resamplingPathPoints,
+     saveLinearProjectionDensity, save2DPlaneDensity, save2DPolarDensity,
+     getMorphopyFeatures,getPersistanceBarcode,getApicalDendriteTortuosity,
+     longestPathLeafNode,termPathLength,getApicalDendriteDirectionConsistency)
+from neurom.view.matplotlib_impl import plot_dendrogram
+from patchview.utilitis.emfDraw import draw_morphorlogy_emf
 from patchview.utilitis.patchviewObjects import *
 import networkx as nx
-
 ## reading neuroluscida file
+import morphio
 from morphio import SomaType
 import neurom as morphor_nm
 from neurom import viewer as morphor_viewer
 from neurom.io.multiSomas import MultiSoma
-# from neurom.features.utilities import (getSomaStats, extractMorhporFeatures, sholl_analysis)
 from neurom.core.morphology import Morphology
 from neurom.core.types import NeuriteType
 import neo
 from neo.io import AxonIO
 import warnings
+import matplotlib
+matplotlib.use("QtCairo") ## for svg export
+matplotlib.use("svg") ## for svg export
+matplotlib.use("pdf") ## for pdf export
 import matplotlib.pyplot as MATPLT
 from matplotlib.ticker import FormatStrFormatter
-from matplotlib.collections import LineCollection
+from matplotlib  import colors as MATPLTcolors
+from matplotlib.collections import LineCollection, PatchCollection
 from sklearn import linear_model
 from matplotlib import image as ReadImage
-from patchview.utilitis.PVdat2NWB import dat2NWB
-import pynwb
-from hdmf.spec import NamespaceCatalog
+from hdmf.spec import NamespaceCatalog ## pyinstaller need hooks
 from hdmf.utils import docval, getargs, popargs, call_docval_func, get_docval
 from hdmf.backends.io import HDMFIO
 from hdmf.backends.hdf5 import HDF5IO as _HDF5IO
 from hdmf.validate import ValidatorMap
 from hdmf.build import BuildManager, TypeMap
 import hdmf.common
 from hdmf.spec import NamespaceCatalog  # noqa: E402
 from hdmf.utils import docval, getargs, call_docval_func, get_docval, fmt_docval_args  # noqa: E402
 from hdmf.build import BuildManager, TypeMap  # noqa: E402
+import pynwb
+from patchview.utilitis.PVdat2NWB import dat2NWB
+from patchview.utilitis.pvEphy import *
+from patchview.utilitis.dandi2pvNWB import dandiNWB
+from patchview.utilitis.pvNDX_class import PatchviewSweepGroup, PatchviewSweep
 warnings.filterwarnings("ignore")
+import gc as GCollector
 from appdirs import *
+
 patchview_dir, this_filename = os.path.split(__file__)
 appname = "Patchview"
-__version__ = "0.2.6.0"
-NeutriteColors = {NeuriteType.apical_dendrite:'m',
-NeuriteType.basal_dendrite: 'b',
-NeuriteType.axon:'r'}
+__version__ = "0.3.0.0"
+
 class MainWindow(QtWidgets.QMainWindow):
     """
     Main frame.
     """
 
     def __init__(self, app, parent=None):
         super(MainWindow, self).__init__(parent)
@@ -94,14 +118,15 @@
         self.setWindowTitle("PatchView")
         self.setWindowIcon(
             pg.QtGui.QIcon(os.path.join(patchview_dir, "Data", "icons", "PatchViewer.ico"))
              
         )
         #        self.resize(1200, 800)
         self.showMaximized()
+        # self.app.aboutToQuit.connect(self.reset)
         
 
 
     def create_mainWindow(self):
         """Configure Qt GUI:
         Main window + splitters to let user resize panes
         """
@@ -111,19 +136,27 @@
         self.add_menubar()
         self.add_toolbar()
 
         if not self.showSpikePanelsFlag:
             self.hideSpikePanels()
         self.statusBar = QtWidgets.QStatusBar()
         self.setStatusBar(self.statusBar)
-        self.MouseMode = pg.ViewBox.RectMode
+        self.MouseMode = pg.ViewBox.PanMode
         self.setCentralWidget(self.mainFrame)
         self.plotItemList = []  ## collect all plot handles
         self.currentAnMorphView= []
         self.mainFrame.show()
+        self.morphor2D_cid = None
+        self.morphorFig_updater = None
+        self.NeutriteColors = {NeuriteType.apical_dendrite:'m',
+            NeuriteType.basal_dendrite: 'b',
+            NeuriteType.axon:'r',
+            NeuriteType.soma:'k',
+            NeuriteType.all:'gray', ## for all neurites
+            'All dendrite': 'c'} ## for all dendrites
 
     def add_selectedDatFile(self, filePath):
         """adding file to the file list if not exist already"""
         i1 = QtGui.QTreeWidgetItem([filePath])
         self.fileList.addTopLevelItem(i1)
 
     def make_layout(self):
@@ -423,30 +456,39 @@
         self.event_BottomSplitter.setStretchFactor(1, 1)
         ## Done with bottom half. Add it to the frame
         self.event_Vsplitter.addWidget(self.event_BottomSplitter)
         self.event_Vsplitter.setStretchFactor(0, 1)
         self.event_Vsplitter.setStretchFactor(1, 3)
 
         splitViewTab_morph = SplitView("Morphology", "Trees")
-        splitViewTab_morph.addMatPlotviewAtTop(["2D"], size=(100, 100), dpi=1000)
+        splitViewTab_morph.addMatPlotviewAtTop(["2D"], size=(15, 10), dpi=100)
 
         splitViewTab_morph.addTablesAtBottomRight(
             ["Summary", "Distance (um)"],
             editable=True,
             sortable=False,
         )
 
-        self.morphAnaFigs_matplotView = MatplotView() ## host for morph analysis figures
-        splitViewTab_morph.bottomRight_tabview.addTab(self.morphAnaFigs_matplotView,"Figures")
+        # self.morphAnaFigs_matplotView = MatplotView() ## host for morph analysis figures
+        # splitViewTab_morph.bottomRight_tabview.addTab(self.morphAnaFigs_matplotView,"Figures")
 
         splitViewTab_morph.addParameterToLeftTab(
-            "Analysis", AllMyPars.Morphor_analysis, self.morph_analysis_event
+            "Parameters", AllMyPars.Morphor_parameters, self.morph_analysis_event
+        )
+        splitViewTab_morph.addParameterToLeftTab(
+            "Measurments", AllMyPars.Morphor_measurments, self.morph_measure_event
+        )
+        splitViewTab_morph.addParameterToLeftTab(
+            "Export", AllMyPars.Morphor_export, self.morph_export_event
+        )
+        splitViewTab_morph.addTablesAtBottomRight(
+            ["Morphopy features"],
+            editable=False,
+            sortable=False,
         )
-        splitViewTab_morph.addParameterToLeftTab("Legend", AllMyPars.Morphor_legend)
-
         self.splitViewTab_morph = splitViewTab_morph
         self.visulization_view.addTab(splitViewTab_morph, splitViewTab_morph.title)
 
 
         ## add a right tool bar!
         self.frame_splitter.addWidget(self.tree_splitter)
         self.frame_splitter.addWidget(self.visulization_view)
@@ -652,35 +694,40 @@
 
     def addTextlabel(self, label, pos):
         TextLabel = pg.TextItem(text=label, color=(255, 255, 255), anchor=(0, 0))
         TextLabel.setFont(QtGui.QFont("serif", 14))
         TextLabel.setPos(pos[0], pos[1] - 10)
         return TextLabel
 
-    def updateTreeMorphView(self, fname):
+    def updateTreeMorphView(self, fname, redraw=False,morphorOnly=True, showTitle=False):
         # try:
-        pv = self.splitViewTab_morph.getParTreePars("Analysis")
-        if pv["Options"][1]["Draw contour"][0]:
+        pv = self.splitViewTab_morph.getParTreePars("Parameters")
+        neutriteColors = pv['Figure options'][1]['Neutrites color'][1]
+        colors = self.getNeutriteColors(neutriteColors, hex=False)
+        for idx, k in enumerate(self.NeutriteColors):
+            if idx == len(colors):
+                break
+            self.NeutriteColors[k] = colors[idx]
+        if pv["Figure options"][1]["Draw contour"][0]:
             drawContour = True
         else:
             drawContour = False
-        if pv["Options"][1]["Ignore diameters"][0]:
-            realDia = True
-        else:
-            realDia= False
         self.neuronMorph =  None 
-        neurons = morphor_nm.load_morphology(fname, somaType = SomaType.SOMA_CYLINDERS)
+        if fname.endswith('.swc'):
+            somaType = SomaType.SOMA_SINGLE_POINT
+        else:
+            somaType = SomaType.SOMA_CYLINDERS
+        neurons = morphor_nm.load_morphology(fname, somaType = somaType)
         fig2D = self.splitViewTab_morph.matplotViews["2D"].getFigure()
-        fig2D.set_size_inches(
-            5, 5, forward=False)
+        fig2D.set_dpi(self.parameters["defaultDPI"])
         fig2D.clf()
-        ax2D = fig2D.add_subplot(111)
-        ax2D.cla()
         if isinstance(neurons, MultiSoma):
             print('Multi soma detected!')
+            ax2D = fig2D.add_subplot(111)
+            ax2D.cla()
             ## population of neurons with soma only
             centers = {
                 "Name": [],
                 "X": [],
                 "Y": [],
                 "Z": [],
                 "average radius": [],
@@ -703,15 +750,15 @@
                 centers["maximal diameter"].append(maxDia)
                 centers["intercell distance"].append(neurons.getDistMatrix(centers))
                 centers["Name"].append(str(idx + 1))
 
             morphor_viewer.draw(
                 neurons, mode="2d", fig=fig2D, ax=ax2D,
                 contour_on=drawContour, contour_color='g', contour_linewidth=0.2,
-                 labels=None
+                 labels=None, enhanceBifurcationPlotting = True
             )
             self.splitViewTab_morph.matplotViews["2D"].draw()
             xlim1 = ax2D.xaxis.get_data_interval().copy()
             ylim1 = ax2D.yaxis.get_data_interval().copy()
 
             if len(neurons.custom_data) > 0:
                 for datablock in neurons.custom_data:
@@ -738,109 +785,259 @@
             self.splitViewTab_morph.tables["Summary"].clear()
             self.splitViewTab_morph.tables["Summary"].appendData(df)
             self.splitViewTab_morph.tables["Summary"].show()
     
             self.updateInterCellDistance()
             self.neuronMorph =  None ## no dendrites for further analysis
         else:  ## single neuron with dendtrite and/or axons
-            fig2D = self.splitViewTab_morph.matplotViews["2D"].getFigure()
-            fig2D.clf()
+            if self.morphor2D_cid  is not None:
+                fig2D.canvas.mpl_disconnect(self.morphor2D_cid)
+                self.morphor2D_cid = None
+                self.morphorFig_updater = None
+            self.morphorFig_updater = FigureUpdater()
+            self.morphor2D_cid = fig2D.canvas.mpl_connect('button_release_event', self.on_Morph_lims_change)
             widths = [3,1]
             # heights = [5,1]
-            gs0 = fig2D.add_gridspec(1, 2, width_ratios = widths)
-            ax2D = fig2D.add_subplot(gs0[0,0])
+            if not (morphorOnly):
+                gs0 = fig2D.add_gridspec(1, 2, width_ratios = widths)
+                ax2D = fig2D.add_subplot(gs0[0,0])
+            else:
+                ax2D = fig2D.add_subplot(111)
             ax2D.cla()
-            pv = self.splitViewTab_morph.getParTreePars("Analysis")
-            rotateAngle = pv["Options"][1]["Rotate tree (degree)"][0]
-            step_size=pv['Options'][1]['Bin size (um)'][0]
-            smoothBins=pv['Options'][1]['Gaussian window size (num. bins)'][0]
-            smoothStandardDeviation=pv['Options'][1]['Std of Gaussian kernel (num. bins)'][0]
+            pv = self.splitViewTab_morph.getParTreePars("Parameters")
+            rotateAngle = pv["Parameters"][1]["Rotate tree (degree)"][0]
+            step_size=pv['Parameters'][1]['Bin size (um)'][0]
+            smoothBins=pv['Parameters'][1]['Gaussian window size (num. bins)'][0]
+            smoothStandardDeviation=pv['Parameters'][1]['Std of Gaussian kernel (num. bins)'][0]
+            DiameterScaling = pv["Parameters"][1]["Diameter scaling"][0]
             if rotateAngle!=0:
                 neurons = rotate(neurons, [0,0,1], rotateAngle*np.pi/180)
             self.neuronMorph = neurons
             morphor_viewer.draw(
-                neurons, mode="2d", realistic_diameters=realDia, fig=fig2D, ax=ax2D,
-                contour_on=drawContour, contour_color='g', contour_linewidth=0.2,rotationContour=rotateAngle
+                neurons, mode="2d", realistic_diameters=True, fig=fig2D, ax=ax2D, alpha=1.0,
+                contour_on=drawContour, contour_color='g', contour_linewidth=0.2,rotationContour=rotateAngle,
+                neutriteColors = self.NeutriteColors, DiameterScaling = DiameterScaling
             )
             ax2D.axis("equal")  ## only works for 2D
-            # ax2D.view_init(azim=0, elev=90)
-            ax2D.set_title("{0}".format(fname), fontsize=12, color="k")
+            if showTitle:
+                ax2D.set_title("{0}".format(fname), fontsize=6, color="k")
+            else:
+                ax2D.set_title("")
+            # ax2D.autoscale()
+            self.morphorFig_updater.add_ax(ax2D, ['linewidth'])
+            if not (morphorOnly):
+                ax_densityX = fig2D.add_subplot(gs0[0,1], sharey = ax2D)
+                ax_densityX.cla()
+                self.update_density(axis='y', step_size=step_size, ax = ax_densityX,
+                flipAxes=True, addTitle=False,smoothBins=smoothBins,smoothStandardDeviation=smoothStandardDeviation)
+                ax_densityX.xaxis.set_ticks_position('top')
+                ax_densityX.xaxis.set_label_position('top') 
+                ax_densityX.tick_params(labelbottom=False,labeltop=True)
+                ax_densityX.spines["right"].set_visible(False)
+                ax_densityX.spines["bottom"].set_visible(False)
+                fig2D.subplots_adjust(top=0.904, bottom=0.04, left=0.0, right=0.90, hspace=0.0, wspace=0.254)
 
-            # ax3D.set_zlim(zmin=max_scaling[0], zmax=max_scaling[1])
-            print("Neuron morphology loaded!")
+        ax2D.axis("off")
+        self.splitViewTab_morph.matplotViews['2D'].draw()
+        self.splitViewTab_morph.matplotViews["2D"].canvas.draw()
+        fig2D.tight_layout()
+        self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(0)
+        # self.splitViewTab_morph.matplotViews['3D'].draw()
+        self.splitViewTab_morph.show()
+
+        ## turn this on to show the summary table
+        if not (morphorOnly) and not redraw:
             df_summary = {}
             df_summary["ASC file"] = [fname]
             df_summary = extractMorphFeatures(neurons, df_summary)
             df_summary = {k:[df_summary[k]] for k in df_summary} ## weird requr. of pandas
             df_summary  = pd.DataFrame.from_dict(df_summary, orient="index").transpose()
             df_summary  = np.array(
                 df_summary.to_records(index=False)
             )  ## format dataframe for using in QtTable widget
             self.splitViewTab_morph.tables["Summary"].clear()
             self.splitViewTab_morph.tables["Summary"].appendData(df_summary)
             self.splitViewTab_morph.tables["Summary"].show()
-            ax_densityX = fig2D.add_subplot(gs0[0,1], sharey = ax2D)
-            ax_densityX.cla()
-            self.update_density(axis='y', step_size=step_size, ax = ax_densityX,
-             flipAxes=True, addTitle=False,smoothBins=smoothBins,smoothStandardDeviation=smoothStandardDeviation)
-            ax_densityX.xaxis.set_ticks_position('top')
-            ax_densityX.xaxis.set_label_position('top') 
-            ax_densityX.tick_params(labelbottom=False,labeltop=True)
-            ax_densityX.spines["right"].set_visible(False)
-            ax_densityX.spines["bottom"].set_visible(False)
-            fig2D.subplots_adjust(top=0.904, bottom=0.04, left=0.0, right=0.90, hspace=0.0, wspace=0.254)
+            self.update_mpfeatures(True)
+        # self.draw_apical_dendrite_rs(ax2D)
 
-        ax2D.axis("off")
-        self.splitViewTab_morph.matplotViews['2D'].draw()
-        self.splitViewTab_morph.matplotViews["2D"].canvas.draw()
-        fig2D.tight_layout()
-        self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(0)
-        self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(2)
-        # self.splitViewTab_morph.matplotViews['3D'].draw()
+    def draw_apical_dendrite_rs(self,ax):
+        maxPathLeaf, _ = longestPathLeafNode(self.neuronMorph, NeuriteType.apical_dendrite, verbose=True)
+        ms  = 1
+        sectionList = []
+        for n in maxPathLeaf.iupstream():
+            # ps = n.points
+            # ms +=0.5
+            # ax.plot(ps[:,0],ps[:,1], marker='o', markersize=ms, alpha=0.5)
+            sectionList.append(n)
+        ps, borders = resampleNeurite(sectionList, min_length_filter=5, max_length_filter=150, pathStep = 10)
+        markers = ['o','x','s','d']
+        c = 0
+        for p, b in zip(ps, borders):
+            m = markers[c%2]
+            ms = 1 + b*0.5
+            ax.plot(p[0],p[1], marker=m, markersize=ms)
+            c+=1
+
+    def update_mpfeatures(self, stats=False):
+        try:
+            df_mpfeatures, N = getMorphopyFeatures(self.neuronMorph, stats=stats)
+            self.morphPy_N = N
+            if stats:
+                df_mpfeatures.insert(loc=0, column="fileNmae", value=self.currentMorphTreeFile)
+                df_mpfeatures  = np.array(
+                        df_mpfeatures.to_records(index=False)
+                    )  ## 
+                self.splitViewTab_morph.tables["Morphopy features"].clear()
+                self.splitViewTab_morph.tables["Morphopy features"].appendData(df_mpfeatures)
+                self.splitViewTab_morph.tables["Morphopy features"].show()
+            else:
+                self.splitViewTab_morph.tables["Morphopy features"].clear()
+
+        except Exception as e:
+            print(f'loading morphorlogy {self.currentMorphTreeFile} failed')
+            print(e)
+
+    def update_featureHistogram(self, feature):
+        '''https://github.com/berenslab/MorphoPy/blob/master/notebooks/MORPHOPY%20Tutorial.ipynb'''
+        if (not hasattr(self, "morphPy_N")) or  self.morphPy_N is None:
+            self.update_mpfeatures(False)
+
+        statistics = [feature]
+        features = ['branch_order', 'strahler_order', 
+                    'branch_angle', 'path_angle', 'root_angle', 
+                    'thickness', 'segment_length', 'path_length', 'radial_dist']
+        hist_widths = [2,.2, 10, 10, 10, .05, 20, 80, 30]
+        limits = [35, 5, 180, 180, 180, 0.5, 600, 2500, 900]
+        w = hist_widths[features.index(feature)]
+        lim = limits[features.index(feature)]
+        N = self.morphPy_N
+        Axon = N.get_axonal_tree()
+        Dendrites = N.get_dendritic_tree()
+        A = Axon.get_topological_minor()
+        D = Dendrites.get_topological_minor()
+        fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " " + feature+"  historgram",
+        size=(15,10)).getFigure()
+        fig.clf()
+        ax = fig.add_subplot(111)
+        for Trees, c in [[(Axon, A), 'darkgreen'], [(Dendrites, D), 'darkgrey']]:
+            if feature in ['segment_length', 'path_length', 'radial_dist']:
+                bins = np.linspace(0,lim, 20)
+            else:
+                bins= np.linspace(0,lim, 10)
+            if feature in ['branch_order', 'strahler_order', 'root_angle']:
+                dist, edges = Trees[1].get_histogram(feature, bins=bins)
+            else:    
+                dist, edges = Trees[0].get_histogram(feature, bins=bins) # you can pass options to the histogram method
+
+            ax.bar(edges[1:], dist, width=w, color=c, alpha=.7)
+            sns.despine()
+            xlabel = feature.replace("_", " ").capitalize()
+            if xlabel.find('length') > -1 or xlabel.find('dist') > -1 or xlabel == 'Thickness':
+                xlabel += ' (um)'
+            elif xlabel.find('angle') > -1:
+                xlabel += ' (deg)'
+            ax.set_xlabel(xlabel)
+            ax.set_ylabel('Frequency')
+
+        ax.legend(['Axon', 'Dendrites'])
+        MATPLT.suptitle('1-D morphometric distributions', weight='bold')
+        fig.tight_layout()
+        fig.canvas.draw()
+    
+    def on_Morph_lims_change(self, events):
+        '''update figure when resized
+        '''
+        self.morphorFig_updater.update_axes()
 
-        self.splitViewTab_morph.show()
 
     def minmaxDist(self, ps):
         """calculate minmial and maximal diameter
         ps: 2-D numpy array
         """
         nPoints = len(ps)
         maxDia = 0
         for j in range(nPoints - 1):
             for k in range(j + 1, nPoints):
                 diameter = np.sqrt(np.sum((ps[j] - ps[k]) ** 2))
                 if diameter > maxDia:
                     maxDia = diameter
         return maxDia
 
-    def update_2D_polar_density(self, ax=None, addTitle =True, angle_step=np.pi/15, neurite_type = NeuriteType.all, step_size=5):
+    def update_ad_stem_directionality_histogram(self, verbose=False):
+        if self.neuronMorph is not None:
+            fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " apical dendrite directionality").getFigure()
+            fig.clf()
+            ax = fig.add_subplot(111)
+            ax.cla()
+            ad = getApicalDendriteDirectionConsistency(self.neuronMorph)
+            if verbose:
+                print('dendrite directionalityL mean=', np.mean(ad), np.max(ad), ' len:', len(ad))
+            ax.hist(ad, bins=25, alpha=0.7, color=self.NeutriteColors[NeuriteType.apical_dendrite])     
+
+    def update_pathLengthHistogram(self):
+        binwidth = 10
+        print("update_pathLengthHistogram", binwidth)
+        if self.neuronMorph is not None:
+            fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " path length historgram").getFigure()
+            fig.clf()
+            c = 1
+            axes = []
+            for nt in [NeuriteType.axon, NeuriteType.basal_dendrite, NeuriteType.apical_dendrite]:
+                _, pLs = termPathLength(self.neuronMorph, neuriteType=nt)
+                if len(pLs) == 0:
+                    continue
+                ax = fig.add_subplot(3,1,c)
+                ax.cla()
+                bins = np.arange(min(pLs), max(pLs) + binwidth, binwidth)
+                ax.hist(pLs,  bins=bins, alpha=0.7, color=self.NeutriteColors[nt], label=nt.name)
+                c+=1
+                axes.append(ax)
+                ax.set_ylabel("Frequency")
+                ax.legend()
+            axes[-1].set_xlabel("Path length (um)")
+            fig.canvas.draw()
+
+    def update_2D_polar_density(self, ax=None, addTitle =True, angle_step=np.pi/15, 
+    neurite_type = NeuriteType.all, step_size=5, axiOps=None, showgrid=True, cmap="rocket"):
             if self.neuronMorph is not None:
                 if ax is None:
-                    fig = self.morphAnaFigs_matplotView.getFigure()
+                    fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " 2D Polar density").getFigure()
                     fig.clf()
                     ax = fig.add_subplot(111,projection="polar")
-                    ax.cla()                       
-                hist, A, R = sholl_polar(self.neuronMorph, step_size=step_size, angle_step=angle_step)
-                pc = ax.pcolormesh(A, R, hist.T, cmap="magma_r")
+                    ax.cla()
+                rmax = None      
+                if axiOps is not None:
+                    if axiOps[0]:
+                        rmax = axiOps[1]            
+                hist, A, R = sholl_polar(self.neuronMorph, step_size=step_size, angle_step=angle_step,rmax=rmax)
+                MATPLT.style.use('ggplot')
+                MATPLT.rcParams["axes.axisbelow"] = False
+                pc = ax.pcolormesh(A, R, hist.T, cmap=cmap)
+                if showgrid:
+                    ax.grid(True, color='gray', lw=0.5)
+                else:
+                    ax.grid(False)
                 fig.colorbar(pc, orientation='vertical')
                 if addTitle:
                     ax.set(title= "XY plane density")
-                self.morphAnaFigs_matplotView.figure.subplots_adjust(top=0.861,bottom=0.02,left=0.0,right=0.7,hspace=0.2,wspace=0.0)
-                self.morphAnaFigs_matplotView.draw()
-                self.morphAnaFigs_matplotView.canvas.draw()
+                # self.morphAnaFigs_matplotView.figure.subplots_adjust(top=0.861,bottom=0.02,left=0.0,right=0.7,hspace=0.2,wspace=0.0)
+                # self.morphAnaFigs_matplotView.draw()
+                # self.morphAnaFigs_matplotView.canvas.draw()
+                fig.tight_layout()
             else:
                 print('Not a morphological object for sholl analysis')
-            self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(2)
+
             
     def update_2D_density(self, ax=None, addTitle =True, neurite_type = NeuriteType.all,
      step_size=5,  useFullRange=True, showColorbar=False, showAxisValues=False,smoothBins=11,
-                smoothStandardDeviation=2):
+                smoothStandardDeviation=2, cmap="rocket"):
             if self.neuronMorph is not None:
                 if ax is None:
-                    fig = self.morphAnaFigs_matplotView.getFigure()
+                    fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " 2D density").getFigure()
                     fig.clf()
                 axes = []
                 images = []
                 for ntype in [NeuriteType.all, NeuriteType.axon, NeuriteType.basal_dendrite, NeuriteType.apical_dendrite, 'All dendrite']:
                     if ntype == NeuriteType.all:
                         ax = fig.add_subplot(151, aspect='equal')
                         ntypeName = "All neurites"
@@ -866,15 +1063,15 @@
                     ax.cla() 
 
                     if len(d2d) > 0 :
                         d2d = smooth2D(d2d, smoothBins, smoothStandardDeviation)
                         xedges -=centerH
                         yedges -=centerV
                         im = ax.imshow(np.transpose(d2d), extent=[xedges[0], xedges[-1], yedges[0], yedges[-1]],interpolation='bilinear', 
-                        origin='lower')
+                        origin='lower', cmap=cmap)
                         images.append(im)
                         soma = MATPLT.Circle((0, 0), 5, color='r')
                         ax.add_patch(soma)
                         if addTitle:
                             ax.set(title= f"{ntypeName} density")
                         if showColorbar:
                             fig.colorbar(im, ax=ax, orientation='vertical', fraction=0.046, pad=0.04)
@@ -883,100 +1080,106 @@
                     if not showAxisValues:
                         ax.axis('off')
                 if showAxisValues:
                     axes[0].set_xlabel('X (um)')
                     axes[0].set_ylabel('Y (um)')
 
                 fig.tight_layout()
-                self.morphAnaFigs_matplotView.draw()
-                self.morphAnaFigs_matplotView.canvas.draw()
+                # self.morphAnaFigs_matplotView.draw()
+                # self.morphAnaFigs_matplotView.canvas.draw()
 
             else:
                 print('Not a morphological object for sholl analysis')
-            self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(2)
+            # self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(2)
 
     def update_density(self, axis='y', ax=None,step_size=1,
      flipAxes=False, addTitle =True, neurite_type = NeuriteType.all,
-     smoothBins=11,smoothStandardDeviation=2):
+     smoothBins=11,smoothStandardDeviation=2, addAllNeuritesPlot=True):
         if self.neuronMorph is not None:
             if ax is None:
-                fig = self.morphAnaFigs_matplotView.getFigure()
+                fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " y axis density").getFigure()
                 fig.clf()
                 ax = fig.add_subplot(111)
                 ax.cla()
             else:
                 fig = ''
 
             if neurite_type == NeuriteType.all:
-                neurite_type  = [NeuriteType.apical_dendrite, NeuriteType.basal_dendrite, NeuriteType.axon]
+                neurite_type  = [NeuriteType.apical_dendrite, NeuriteType.basal_dendrite, NeuriteType.axon, "All dendrite"]
+                if addAllNeuritesPlot:
+                    neurite_type.insert(0, NeuriteType.all)
             else:
                 neurite_type  = [neurite_type]
-            for neurite_type in neurite_type :
-                c = NeutriteColors[neurite_type]
+            
+            for ntype in neurite_type :
+                c = self.NeutriteColors[ntype]
+                if ntype == NeuriteType.all:
+                    alpha = 0.5
+                elif ntype == "All dendrite":
+                    ntype = [NeuriteType.apical_dendrite, NeuriteType.basal_dendrite]
+                else:
+                    alpha = 0.7
                 density, bin_edges, centerVal, _ = sholl_single_axis(self.neuronMorph, step_size=step_size, axis=axis,
-                 neurite_type=neurite_type)
+                 neurite_type=ntype)
                 if density==[]:
                     continue
                 density = smooth(density, window_len=smoothBins, std=smoothStandardDeviation,
                 window='gaussian')
                 ndiff = len(bin_edges) - len(density)
                 if ndiff > 0:
                     bin_edges = bin_edges[ndiff:]
                 else:
                     density = density[-ndiff:]
                 if flipAxes:
-                    ax.plot(density, bin_edges-centerVal, color=c)
+                    ax.plot(density, bin_edges-centerVal, color=c, alpha=alpha)
                     xlabel = "um per bin"
                     ylabel = 'Distance from soma (um)'
                 else:
-                    ax.plot(bin_edges, density-centerVal, color=c)
+                    ax.plot(bin_edges, density-centerVal, color=c, alpha=alpha)
                     ylabel = "um per bin"
                     xlabel = 'Distance from soma (um)'
 
             ax.set(xlabel=xlabel, ylabel=ylabel)
             if addTitle:
                 ax.set(title= axis+" density")
-            self.morphAnaFigs_matplotView.draw()
-            self.morphAnaFigs_matplotView.canvas.draw()  
+            # self.morphAnaFigs_matplotView.draw()
+            # self.morphAnaFigs_matplotView.canvas.draw()  
             if fig != '':
                 fig.tight_layout()
         else:
             print('Not a morphological object for sholl analysis')
-        self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(2)
-
 
     def update_sholl(self, step_size=1, smoothBins=11,smoothStandardDeviation=2):
         if self.neuronMorph is not None:        
-            fig = self.morphAnaFigs_matplotView.getFigure()
+            fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " Sholl intercetions").getFigure()
             fig.clf()
             ax = fig.add_subplot(111)
             ax.cla()
-            sns.set_style("whitegrid")
             for neurite in self.neuronMorph.neurites:
                 sholl_dist, sholl_bins = sholl_analysis(self.neuronMorph, step_size=step_size, neurite_type=neurite.type)
-                c = NeutriteColors[neurite.type]
+                c = self.NeutriteColors[neurite.type]
                 sholl_bins = smooth(sholl_bins, window_len=smoothBins, std=smoothStandardDeviation,
                 window='gaussian')
                 ndiff = len(sholl_bins) - len(sholl_dist)
                 if ndiff > 0:
                     sholl_bins = sholl_bins[ndiff:]
                 else:
                     sholl_dist = sholl_dist[-ndiff:]
                 ax = sns.lineplot(x=sholl_bins, y=sholl_dist, ax=ax, color=c)
             ax.set(xlabel='Distance from soma (um)', ylabel="Num. points",\
             title="Sholl frequency")
             ax.spines["right"].set_visible(False)
             ax.spines["top"].set_visible(False)
             fig.tight_layout()
-            self.morphAnaFigs_matplotView.draw()
-            self.morphAnaFigs_matplotView.canvas.draw()
+            # self.morphAnaFigs_matplotView.draw()
+            # self.morphAnaFigs_matplotView.canvas.draw()
 
         else:
             print('Not a morphological object for sholl analysis')
-        self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(2)
+        # self.splitViewTab_morph.bottomRight_tabview.setCurrentIndex(2)
 
     def updateSliceView(self):
         if hasattr(self, "slice_viewROIs"):
             for roi in self.slice_viewROIs:
                 roi.remove()
 
         self.currentROI_label = ""
@@ -1092,30 +1295,14 @@
             pg.QtGui.QIcon(rect_icon), "Mouse Mode"
         )
         self.toogleMouseModePanAction.setShortcut("Ctrl+m")
         self.toogleMouseModePanAction.setStatusTip("switch between pan and rect mode")
         self.toogleMouseModePanAction.triggered.connect(self.MouseMode_clicked)
         self.toolbar.addAction(self.toogleMouseModePanAction)
 
-        # self.toogleDetectSpikeAction = pg.QtGui.QAction(
-        #     pg.QtGui.QIcon(spk_icon), "Firing pattern"
-        # )
-        # self.toogleDetectSpikeAction.setShortcut("Alt+a")
-        # self.toogleDetectSpikeAction.setStatusTip("Firing pattern")
-        # self.toogleDetectSpikeAction.triggered.connect(self.detectSpikes_clicked)
-        # self.toolbar.addAction(self.toogleDetectSpikeAction)
-
-        # self.exportAction = pg.QtGui.QAction(
-        #     pg.QtGui.QIcon(connection2_icon), "Connectivtiy"
-        # )
-        # self.exportAction.setShortcut("Alt+e")
-        # self.exportAction.setStatusTip("Connectivtiy")
-        # self.exportAction.triggered.connect(self.exportConnectionFig_clicked)
-        # self.toolbar.addAction(self.exportAction)
-
         self.importSlicetAction = pg.QtGui.QAction(
             pg.QtGui.QIcon(neuron_icon), "Import slice image"
         )
         # self.exportAction.setShortcut("Alt+e")
         self.importSlicetAction.setStatusTip("import slice image")
         self.importSlicetAction.triggered.connect(self.importSlice_clicked)
         self.toolbar.addAction(self.importSlicetAction)
@@ -1133,41 +1320,42 @@
         self.gpAction2.setStatusTip("Analysis gap junction")
         self.gpAction2.triggered.connect(self.gpc_clicked)
         self.toolbar.addAction(self.gpAction2)
 
     def importTree_clicked(self):        
         dialog = QtWidgets.QFileDialog(self)
         dialog.setWindowTitle("Import Slice image")
-        dialog.setNameFilter("Image files (*.asc *.ASC)")
+        dialog.setNameFilter("Image files (*.asc *.ASC *.swc)")
         if hasattr(self, "cwd"):
             dialog.setDirectory(self.cwd)
         else:
             dialog.setDirectory(QtCore.QDir.currentPath())
         dialog.setFileMode(QtWidgets.QFileDialog.ExistingFile)
         if dialog.exec_() == QtWidgets.QDialog.Accepted:
             fname = str(dialog.selectedFiles()[0])
             self.cwd = os.path.dirname(os.path.abspath(fname))
         else:
             return
         self.prepareTree(fname)
         self.currentAnMorphView = ''
 
     def prepareTree(self, fname):
+        '''prepare tree for visualization'''
         self.visulization_view.setCurrentIndex(5)
         self.currentMorphTreeFile = fname
-        if glob.glob(fname[:-4] + "_mod.ASC") == []:
-            fname = cleanASCfile(fname)  ## to clean not-want sections
+        if fname[-3:] in ["asc","ASC"] and glob.glob(fname[:-4] + "_mod.ASC") == []:
+            fname = cleanASCfile(fname)  ## to clean unwant sections
         self.splitViewTab_morph.matplotViews["2D"].getFigure().clf()
-        self.morphAnaFigs_matplotView.getFigure().clf()
-        self.updateTreeMorphView(fname)
-        print('morphfile', fname, fname[-8:])
+        pv = self.splitViewTab_morph.getParTreePars("Parameters")        
+        morphorOnly = pv['Figure options'][1]['Morphology only'][0]
+        showTitle = pv['Figure options'][1]['Show title'][0]
+        self.updateTreeMorphView(fname, redraw=False, morphorOnly=morphorOnly, showTitle=showTitle)
         if fname[-8:] == "_mod.ASC":
             os.remove(fname)
 
-
     def importSlice_clicked(self):
         self.updateSliceView()
 
     def MouseMode_clicked(self):
         rect_icon = os.path.join(patchview_dir, "Data", "icons", "rectangle.png")
         nav_icon = os.path.join(patchview_dir, "Data", "icons", "navigation.png")
         if self.MouseMode == pg.ViewBox.RectMode:
@@ -1575,15 +1763,15 @@
                     df = pd.DataFrame(events_waveforms)
                     df.columns = header
                     df.insert(0, "Time", T)
                     with open(fileName, "w") as f:
                         df.to_csv(f, header=True, line_terminator="\n")
 
     def exportFile(self, title=None, defaultName=None, extension="all files (*.*)"):
-        fileName = QtGui.QFileDialog.getSaveFileName(
+        fileName = QtWidgets.QFileDialog.getSaveFileName(
             None, title, defaultName, extension
         )
         if isinstance(fileName, tuple):
             return fileName[0]
         else:
             return []
 
@@ -2374,15 +2562,15 @@
         dt["session"] = ss.split("\\")[-1]
         dt["series"] = self.events.seriesName
         funcPars = {}
         for k in dtKeys:
             funcPars[k] = dt[k]
         df = pd.DataFrame.from_dict(funcPars, orient="index").transpose()
         df = np.array(
-            df.to_records(index=False)
+            df.to_records(index=True)
         )  ## format dataframe for using in QtTable wiget
         self.templateFit.clear()  ## clear table for new template
         self.templateFit.appendData(df.copy())  ## update QtTable widget
         self.templateFit.show()
 
     def event_showTemplate(self, toFit):
         plotHandle = self.event_traceView2.getItem(0, 0)
@@ -3231,53 +3419,97 @@
             "This program is under BSD-3 license.\nCopyright (c) 2020-2022, Ming Hu. All rights reserved.",
             BSD_3b,
         )
     def link2Doc_clicked(self):
          self.showdialog(
             "For source code & documentation, see details below: ",
             "Source code & issue reporting:\n https://github.com/ZeitgeberH/patchview \n\nDocumentation:\n https://patchview.readthedocs.io/en/latest/index.html",
-        )       
-    def makeNWBobject(self):
+        )
+
+    def makeNWBobject(self, dataSourceFormat):
         selected = self.currentPulseTree.selectedItems()
-        sel = selected[0]
-        selIdx = sel.index
-        if len(selIdx) < 2:
-            return
-        nwbObj = dat2NWB(self.currentPulseTree.dat_file, [selIdx[0], selIdx[1]])
-        return nwbObj
+        traceIdex_selected = sorted(self.currentPulseTree.selectedTraceIndex)
+        sweepIdx = [] # list of sweep numbers. 
+        if dataSourceFormat in [".dat",".abf"]: # for now. would switch to NWB very soon!
+            for sel in selected: ## selection may be complicated (cross-level etc.)
+                selIdx = sel.index
+                if len(selIdx) == 2: # series level
+                    seriesNode = getAllChildIndexFromItem(sel)
+                    for c in seriesNode: # sweep level
+                        sweepIdx.append(c.index) #
+                elif len(selIdx) == 3: # sweep level
+                    sweepIdx.append(selIdx)
+            pv_ephy = dat2NWB(self.currentPulseTree.dat_file) # a pvEphy object
+            pv_ephy.loadProtocols('patchview') 
+            pv_ephy.AddSweeps(sweepIndex = sweepIdx, traceIndex=traceIdex_selected)
+            print(dataSourceFormat, 'selected', traceIdex_selected)
+        else: # save a portion of sweeps from current NWB file
+            pv_ephy = pvNWB() # a pvEphy object.
+            src = self.currentPulseTree.pvEphy.nwbfile
+            for sel in selected:
+                selIdx = sel.index
+                if len(selIdx) == 2: # series level
+                    seriesNode = getAllChildIndexFromItem(sel)
+                    for c in seriesNode: # sweep level
+                        sweepIdx.append(c.index[2]) #
+                elif len(selIdx) == 3: # sweep level
+                    sweepIdx.append(selIdx[2])
+            pv_ephy.nwbfile = pv_ephy.copy_sweeps(src = src, sweep_table_index=sorted(sweepIdx))
+        return pv_ephy
 
     def getSaveFileNameNWB(self):
         """save file dialog. Return the path and filename for saving user selected data"""
         fileName = QtWidgets.QFileDialog.getSaveFileName(
             self,
             "Save File",
-            self.root + self.QtFileNameLabel.text()[:-4],
+            self.root + self.currentPulseTree.dat_file+'_',
             "NWB (*.nwb)",
         )
         return fileName[0]
 
     def saveNWB_clicked(self):
+        ''' save NWB file
+        temporary solution before unified data structure
+        '''
         fileName = self.getSaveFileNameNWB()
+        pvNWB = None
+
         if fileName !='':
-            self.nwbObj = self.makeNWBobject()
-            if self.nwbObj !=None:
-                self.statusBar.showMessage(" " + fileName, 3000)
-                self.nwbObj.saveNBF(fileName)
+            ext = self.currentPulseTree.fileSourceFormat
+            pvNWB = self.makeNWBobject(ext)
+
+        if pvNWB is not None:
+            self.statusBar.showMessage(" " + fileName, 3000)
+            pvNWB.saveNWB(fileName)
+            # self.currentPulseTree.pvEphy = pvNWB
+
+        # if hasattr(self.currentPulseTree, 'pvEphy'):
+        #     if hasattr(self.currentPulseTree.pvEphy, 'io'): # has io handle
+        #         self.currentPulseTree.pvEphy.io.close() ## close the file before saving
+        #     self.currentPulseTree.pvEphy = None # reset the handle
+        #     GCollector.collect() # force garbage collection
+
 
     def exit_clicked(self):
+        self.reset() ## this should destroy all handles
+        self.close()
+        
+    def closeEvent(self, event):
         self.reset()
         self.close()
 
-    #        self.app.closeAllWindows()
-
     def reset(self):
         """this wipe out every thing. Be careful"""
         self.currentSelectedIndex = []
-        self.trace_view.clear()  ## refresh the layout
-        self.trees_view.setCurrentIndex(0)
+        try:
+            self.trace_view.clear()  ## refresh the layout
+            self.trees_view.setCurrentIndex(0)
+        except Exception as e:
+            print('trace_view clear error \n')
+            print(e)
         self.cellFeatures_view.clear()
         self.sweepFeatures_view.clear()
         self.spikeTable_view.clear()
         self.sliceView.tables["ROI list"].clear()
         self.splitViewTab_connection.reset()
         self.splitViewTab_FP.reset()
         self.spikes_view.clf()
@@ -3293,14 +3525,22 @@
         self.EphyFeaturesObj = []  ## clear ephy object
         if self.showSpikePanelsFlag == 1:
             self.hideSpikePanels()
         self.pia = None
         self.neuronsData = None
         self.neuronMorph =  None 
         self.spikeTableSavePath = ""
+        self.morphor2D_cid = None
+        self.morphorFig_updater = None
+        self.morphPy_N = None
+        if hasattr(self, "MatPlotWindows"):
+            for m in self.MatPlotWindows:
+                m.close()
+            self.MatPlotWindows = []
+        GCollector.collect()  ## force garbage collection
 
     def resetAll_clicked(self):
         self.reset()
 
     def gatherParameters(self, ext=".dat"):
         self.parameters = {}
         self.setUserProfile([])
@@ -3320,33 +3560,47 @@
         else:
             self.user = user
         self.useConfigDir = user_config_dir(appname)
         self.loadUserParamters(user)
 
     def loadUserParamters(self, user):
         confilePath  = os.path.join(self.useConfigDir,"patchview.yaml")
-        if not os.path.exists(self.useConfigDir):
+        if not os.path.exists(self.useConfigDir): ## create the config directory if not exist
             import shutil 
             os.makedirs(self.useConfigDir)
             DATA_PATH = os.path.join(patchview_dir, "Data", "patchview.yaml")    
             shutil.copy(DATA_PATH, confilePath)
+        else: ## compare differnce between the default config file and the user config file
+            print('Detect user config file. Compare with default config file.')
+
+            DATA_PATH = os.path.join(patchview_dir, "Data", "patchview.yaml")
+            with open(DATA_PATH, "r") as f:
+                default_pars = yaml.load(f, Loader=yaml.FullLoader)
+            with open(confilePath, "r") as f:
+                user_pars = yaml.load(f, Loader=yaml.FullLoader)
+            results = dictdiffer.diff(user_pars,default_pars)
+            patched = dictdiffer.patch(results, user_pars, action_flags='a')
+            with open(confilePath, "w") as f:
+                yaml.dump(patched, f,sort_keys=False)
+            print('User config file updated.')
 
         pars = loadYAML(confilePath)
         parameters = {}
         # parameters['HF'] = pars['Filters']['High cutoff']
         parameters["filter_option"] = pars["Filters"]["Option"]
         parameters["HF"] = pars["Filters"]["High cutoff"]
         parameters["CleanUp"] = pars["CleanUp"]
         parameters["Protocols"] = pars["Protocols"]
         parameters["Protocols"]["This serie"] = {"Type": [], "StimChanID": []}
         parameters["plotStim"] = pars["Visulization"][
             "Plot stim"
         ]  ## plot stimulation current
         parameters["Downsampling"] = pars["Visulization"]["Downsampling"]
         parameters["RootDir"] = pars["RootDir"]
+        parameters["defaultDPI"] = pars["Visulization"]["Default figure DPI"]
         self.root = pars["RootDir"]
         self.parameters = parameters
         # self.getEphySpikePars()
         return parameters
 
     def updateUserParamters(self):
         ## this is the parameters changed by the user in the global paramter tree box
@@ -3356,14 +3610,15 @@
             "Notch filter frequency"
         ][0]
 
         self.parameters["HF"] = pv["data preprocessing"][1]["High frequency cutoff"][0]
         self.parameters["CleanUp"]["minimalSweeps"] = pv["data preprocessing"][1][
             "minimal number of sweeps"
         ][0]
+        self.parameters["defaultDPI"] = pv["Basic parameters"][1]["Default figure DPI"][0]
 
     def switchBackground_clicked(self):
         if self.trace_view._background == "k":
             self.trace_view.setBackground("w")
         else:
             self.trace_view.setBackground("k")
 
@@ -3433,16 +3688,16 @@
             self.showSpikePanels()
 
     def getSaveFileName(self):
         """save file dialog. Return the path and filename for saving user selected data"""
         fileName = QtWidgets.QFileDialog.getSaveFileName(
             self,
             "Save File",
-            self.root + self.QtFileNameLabel.text()[:-4] + "_PV",
-            "pickle (*.dat)",
+            self.root + self.currentPulseTree.dat_file+'_' #self.QtFileNameLabel.text()[:-4] + "_PV",
+            "NWB (*nwb); pickle (*.dat)",
         )
         return fileName[0]
 
     def save_clicked(self):
         selected = self.currentPulseTree.selectedItems()
         if len(selected) < 1:
             return
@@ -3461,15 +3716,15 @@
             if treeLevel == 4:  ##  series level: all sweeps, all channels
                 self.saveSingleTrace(
                     sel.node, sel.index
                 )  ## third arugument is for pen. if empty use default pen
 
     def saveSingleSeries(self, sel):
         fileName = self.getSaveFileName()
-        import pickle
+        
 
         if fileName != "":
             self.statusBar.showMessage("Saving " + fileName[:-4], 3000)
             (
                 time,
                 data,
                 stimTime,
@@ -3828,26 +4083,25 @@
         mplWidget.figure.subplots_adjust(
             left=0.08, bottom=0.1, top=0.95, right=0.95, wspace=0.35, hspace=0.35
         )
         self.showSpikePanelsFlag = 1
         self.spikes_view.draw()
 
     def getEphyFeatures(self):
-
         selected = self.currentPulseTree.selectedItems()
         self.visulization_view.setCurrentIndex(1)
         if not len(selected):
             self.showdialog("Load a pulse tree first!")
             return 0
         sel = selected[0]
 
         if len(sel.index) != 2:
             self.showdialog("To extract spike fetures, please select a series!")
             return 0
-        if self.currentPulseTree.filetype == ".dat":
+        if self.currentPulseTree.fileSourceFormat == ".dat":
             title = (
                 self.sliceName[:-4]
                 + " "
                 + "Series"
                 + str(sel.index[1] + 1)
                 + " "
                 + sel.node.Label
@@ -3856,53 +4110,80 @@
                 time,
                 data,
                 stimTime,
                 stimData,
                 stimInfo,
                 serieInfo,
             ) = self.extractSingleSeries(sel)
-        elif self.currentPulseTree.filetype == ".abf":
+        elif self.currentPulseTree.fileSourceFormat == ".abf":
             title = (
                 self.currentPulseTree.dat_file[:-4].split("\\")[-1]
                 + " "
                 + "Block"
                 + str(sel.index[0] + 1)
                 + " Sweep"
                 + str(sel.index[1] + 1)
             )
             time, data = self.extractSingleSeries_ABF(sel.index)
             stimInfo = self.currentPulseTree.abf_stimInfo
-
+        elif self.currentPulseTree.fileSourceFormat  == ".nwb":
+            time, stim, data, metaInfo = self.prepareVoltageNDarray_NWB(sel)
+            # swGps = self.currentPulseTree.pvEphy.getSweepGroups()
+            sweepGroupKey = self.currentPulseTree.pvEphy.sweepGroupNames[sel.index[1]] # which sweep group
+            nSweeps = len(self.currentPulseTree.pvEphy.sweepGroups[sweepGroupKey])
+            self.currentPulseTree.selectedTraceIndex
+            if len(self.currentPulseTree.selectedTraceIndex) > 0:
+                fpChanIdx = self.currentPulseTree.selectedTraceIndex[0] # need a generic way to address this
+            else:
+                fpChanIdx = 0
+            data = np.squeeze(data[:,:,fpChanIdx])
+            print('data shape:', data.shape)
+            srate = metaInfo['recording_rate']
+            stimInfo = []
+            for i in range(nSweeps):
+                swpMetaInfo = self.currentPulseTree.pvEphy.getMetaInfoFromSweepGroups(sweepGroupKey, i, False)
+                stimInfo.append([{},{}])
+                stimInfo[i][1]["start"] = swpMetaInfo['stimulus_onset'] *srate
+                stimInfo[i][1]["end"] = swpMetaInfo['stimulus_offset']*srate
+                stimInfo[i][1]["sampleInteval"] = 1/srate
+                stimInfo[i][1]["amplitude"] = swpMetaInfo['stimulus_amplitude']
+                stimInfo[i][1]["Vholding"] = swpMetaInfo['stimulus_holding_amplitude']
+            
+            title = self.currentPulseTree.pvEphy.nwbfile.identifier + "_" + sweepGroupKey
         (
             dv_cutoff1,
             min_height1,
             min_peak1,
             thresh_frac1,
             baseline_interval1,
             baseline_detect_thresh1,
             max_interval1,
             filterHighCutFreq_spike,
+            start_latency,
         ) = self.getEphySpikePars()
         ## Here we plug in all the available parameters
+        ##
         self.EphyFeaturesObj = extraEhpys_PV.extraEphys(
             time,
             data,
             datIndex=sel.index,
             stimInfo=stimInfo,
             title=title,
             filterHighCutFreq=filterHighCutFreq_spike / 1000,
             dv_cutoff=dv_cutoff1,
             max_interval=max_interval1,
             min_height=min_height1,
             min_peak=min_peak1,
             thresh_frac=thresh_frac1,
             baseline_interval=baseline_interval1,
             baseline_detect_thresh=baseline_detect_thresh1,
+            start_latency=start_latency,
         )
-
+        self.ephyFpObjectList = {}
+        self.ephyFpObjectList[self.currentPulseTree.dat_file[:-4]] = self.EphyFeaturesObj
         # fileName = self.currentPulseTree.dat_file[:-4]+'_Series' + str(sel.index[1]+1) + '_'+ sel.node.Label+'_PvSpikeFeatures.pdf'
         self.plot_splitter.setStretchFactor(1, 3)
         self.topPlot_splitter.setStretchFactor(1, 1)
         self.trace_view2.clear()
         self.showSpikePanels()
         self.EphyFeaturesObj.plot_w_style(
             mplWidget=self.spikeSummary_view
@@ -3915,26 +4196,46 @@
         sw = self.EphyFeaturesObj.df_related_features.copy()
         sw = sw[sw.spike_count>0]
         cellFeature = self.EphyFeaturesObj.Cell_Features
         for n in ['current','spike_count']:
             cellFeature[n]  = 0
             cellFeature[n]  = cellFeature[n].astype('object')
             cellFeature.at[0,n] = list(sw[n].values)
+        # Extract Vholding for the first entry
+        vholding = stimInfo[0][1]['Vholding']
+        # Extract amplitude for all entries
+        amplitudes = [entry[1]['amplitude'] for entry in stimInfo]
+        cellFeature['Vholding'] = vholding
+        cellFeature['Input step'] = np.mean(np.diff(amplitudes))
+        cellFeature['Initial ampltitude'] = amplitudes[0]
+        try:
+            self.updateEphyTable(
+                cellFeature,
+                self.splitViewTab_FP.tables["Cell features"],
+            )
+        except Exception as e:
+            print('cell feature erro', e)
+            return
 
-        self.updateEphyTable(
-            cellFeature,
-            self.splitViewTab_FP.tables["Cell features"],
-        )
         spike_df = self.moveSweepCountFront(self.EphyFeaturesObj.df, "sweepCurrent")
         spike_df = self.moveSweepCountFront(spike_df, "sweepCount")
-        self.updateEphyTable(spike_df, self.splitViewTab_FP.tables["Spike features"])
+
+        try:
+            self.updateEphyTable(spike_df, self.splitViewTab_FP.tables["Spike features"])
+        except Exception as e:
+            print('spike feature erro', e)
+            return
         sw = self.EphyFeaturesObj.df_related_features.copy()
         sw = self.moveSweepCountFront(sw, "current")
         sw.insert(loc=0, column="sweepCount", value=np.arange(1, len(sw) + 1))
-        self.updateEphyTable(sw, self.splitViewTab_FP.tables["Sweep features"])
+        try:
+            self.updateEphyTable(sw, self.splitViewTab_FP.tables["Sweep features"])
+        except Exception as e:
+            print('sweep feature erro', e)
+            return
         self.splitViewTab_FP.bottomLeft_tabview.setCurrentIndex(1)
         return 1
 
     @staticmethod
     def moveSweepCountFront(df, feature):
         """feature: such as 'sweepCount'"""
         if feature in df.columns:
@@ -4017,15 +4318,15 @@
                 print("data not found! line 3241")
                 return
             nSweep = bundleClass.countSweeps(series_index)
         elif self.currentPulseTree.filetype == ".abf":
             datName, series_index = self.checkNodeIndex()
             time, data = self.extractSingleSeries_ABF(series_index)
             avg = np.mean(data, 1)
-            pdb.set_trace()
+
 
     def gpAna(self, option):
         ''' Custom module for cross correlation between voltage of pair of channels in a multi-patch experiment
         '''
         selected = self.currentSelectedIndex
         sel = selected[0]
         if len(sel.index) != 2:
@@ -4242,14 +4543,15 @@
 
     def checkEvent_action_clicked(self):
         self.makeNewEventWindow(True)
         self.visulization_view.setCurrentIndex(4)
 
     def checkFP_action_clicked(self):
         # debugInfo('', True)
+        self.ephyFpObjectList = {}
         self.visulization_view.setCurrentIndex(1)
         (
             bundleFiles,
             stimChanLabels,
             serieIndex,
             treeChildrenIdx,
         ) = self.getDatFilesFromTreeWiget("Firing pattern")
@@ -4269,15 +4571,15 @@
         self.splitViewTab_FP.matplotViews["Firing pattern"].clf()
         axes = self.splitViewTab_FP.matplotViews["Firing pattern"].setPlotGrid(
             nRow, nCol
         )
         pars = self.splitViewTab_FP.getParTreePars(
             "Data selection"
         )  # self.fpParTree_data_view.p
-
+        
         for file_idx, bundle in enumerate(bundleFiles):
             sel = serieIndex[file_idx]
             stimChanIndex = stimChanLabels[file_idx]
             irow, icol = file_idx // nCol, file_idx % nCol
             fs = bundle.getSeriesSamplingRate(sel)
             nSweeps = bundle.countSweeps(sel)
             time = bundle.getSweepTimeStamps(sel)
@@ -4344,19 +4646,17 @@
                 cellFeature.at[0,n] = list(sw[n].values)
             # pdb.set_trace()
             self.updateEphyTable(
                 cellFeature,
                 self.splitViewTab_FP.tables["Cell features"],
                 ephObj.title,
             )
-
-
-        
+   
             self.updateEphyTable(sw, self.splitViewTab_FP.tables["Sweep features"], ephObj.title)
-
+            self.ephyFpObjectList[cellName] = ephObj
             print(cellName, "done!")
                 # except:
                 #     print(cellName, 'failed!')
         if self.batchFPana:
             self.splitViewTab_FP.matplotViews["Firing pattern"].adjustSubplot(
                 left=0.06, right=0.98, top=0.95, bottom=0.06, wspace=0.2, hspace=0.6
             )
@@ -5418,44 +5718,81 @@
             "Connection",
         ]:
             self.selTrees.stimChannelID[dat_file].append(
                 self.parameters["Protocols"]["This serie"]["StimChanID"] - 1
             )  ## ID for stimulation channel
         self.selTrees.update_tree_recursive(self.selTrees.invisibleRootItem(), [])
 
+    def update_treeWidget(self, n):
+        '''n: neuorM object'''
+        self.currentMorphoTree.clear()
+        self.currentMorphoTree = None # clean up the tree widget for reusing
+
     def update_pul(self, dat_file, dat_index=None, ext=".dat"):
         """
         Makes call to update pul view.
         :param dat_file:
         :return:
         """
         if dat_file == "":
             return
-        self.hideSpikePanels()
+        self.updateCurrentPulseTree()
         self.currentPulseTree.clear()
         self.currentPulseTree.sweepCount = 0
         self.currentPulseTree.traceCount = 0
+        self.currentPulseTree.selectedTraceIndex = []
         self.currentPulseTree.dat_file = dat_file  ## data file
+        self.currentPulseTree.fileSourceFormat = ext
         if ext == ".dat":
             self.currentPulseTree.bundle = HEKA.Bundle(dat_file)
             self.currentPulseTree.update_tree_recursive(
                 self.currentPulseTree.invisibleRootItem(), [], dat_index
             )
         elif ext == ".abf":
             self.currentPulseTree.abf = AxonIO(filename=dat_file)
 
             self.currentPulseTree.update_ABFtree(
                 self.currentPulseTree.invisibleRootItem()
             )
             self.parameters["fs"] = self.currentPulseTree.abf.get_signal_sampling_rate()
             self.currentPulseTree.abf_stimInfo = self.extractStimData_ABF()
+        elif ext == '.nwb':
+            # self.currentPulseTree.pvEphy = dandiNWB(dat_file) # how to make this more general?
+            self.currentPulseTree.pvEphy = self.createPVEphyInstance(dat_file, self.getNWBClass()) # how to make this more general?
+            self.currentPulseTree.update_withNWB_sweepTable(
+                self.currentPulseTree.invisibleRootItem()
+            )
+            self.addNWB_metaIinfo()
         # self.currentPulseTree.expandAll()
         self.gatherParameters(ext)
         self.updateStatusBar_fileName()
 
+    def getNWBClass(self):
+        pv = self.globalSettings.p.getValues()
+        nwbClassName = pv["data preprocessing"][1]["NWB sweep table grouping"][0]
+        try:
+            nwbClass = eval(nwbClassName)
+        except:
+            nwbClass = pvNWB
+            print('getNWBClass: ', nwbClassName, ' not found, use pvNWB')
+        return nwbClass
+
+    def createPVEphyInstance(self, dat_file, nwbClasss=None):
+        ''' create a pvEphy instance for the current file according to the user-defined class
+            userDefinedClass: a class object
+            return a pvEphy instance according to user defined class
+        '''
+        if nwbClasss is None:
+            nwbClasss = pvNWB # base class
+        else:
+            assert issubclass(nwbClasss, pvNWB), 'nwbClasss must be a subclass of pvNWB'
+        print('createPVEphyInstance: ', nwbClasss, dat_file)
+        return nwbClasss(dat_file)
+        
+        
     def updateStatusBar_fileName(self):
         if self.currentPulseTree.dat_file != None:
             if hasattr(self, "QtFileNameLabel"):
                 self.statusBar.removeWidget(self.QtFileNameLabel)
             self.QtFileNameLabel = QtWidgets.QLabel()
             self.QtFileNameLabel.setText(self.currentPulseTree.dat_file)
             self.statusBar.addWidget(self.QtFileNameLabel)
@@ -5528,30 +5865,52 @@
                     plt = self.trace_view.addPlot()
                 self.plotSingleTrace(
                     plt, sel.node, sel.index, [], True, True
                 )  ## third arugument is for pen. if empty use default pen
         if self.plotItemList:  ## update mouse mode if not empty
             self.setViewboxMouseMode()
 
+    def update_selected_index(self):
+        ''' Seperate plotting widget selection tree with Exporting tree.
+        '''        
+        selected = self.currentPulseTree.selectedItems()
+        # self.currentPulseTree.current_selected_nodes = selected
+        # self.currentPulseTree.current_selected_sweep_indies = []
+        # if not selected:
+        #     return  # non-selected
+        # sel_levels = [] # check consistency of selection levels
+        # for sel in selected:
+        #     if len(sel.index) == 
+        #     self.currentPulseTree.current_selected_sweep_indies.append(sel.index)
+
+        # selected = [selected[i] for i, l in enumerate(sel_levels) if l==use_level]
+
     def update_trace_plot(self, selected=None):
         """Show data associated with the selected tree node.
         For all nodes, the meta-data is updated in the bottom tree.
         For trace nodes, the data is plotted.
         """
-        self.plt = []  ## plot handles
-        self.plotItemList = []  ## collect all plot handles
-        ### BUILD A plot!
-        # pdb.set_trace()
-        self.trace_view.clear()  ## refresh the layout
-        #        self.trace3DView.clear()
-        # self.trace3DView.hide()
-        self.updateUserParamters()
         selected = self.currentPulseTree.selectedItems()
         if not selected:
             return
+        sel_levels = [] # check consistency of selection levels
+        # if multi-levels are selected (a trace and a sweep for example)
+        # opt to highest level
+        for sel in selected:
+            sel_levels.append(len(sel.index))
+        use_level = min(sel_levels)
+        # filtered all levels below
+        selected = [selected[i] for i, l in enumerate(sel_levels) if l==use_level]
+        self.plt = []  ## plot handles
+        self.plotItemList = []  ## collect all plot handles
+        try:
+            self.trace_view.clear()  ## refresh the layout
+        except Exception as e:
+            print('trace_view clear error')
+        self.updateUserParamters()
         self.currentSelectedIndex = selected
         self.visulization_view.setCurrentIndex(0)
         # update data tree
         sel = selected[0]
         serieIndex = sel.index
         if (
             self.EphyFeaturesObj
@@ -5575,14 +5934,19 @@
             selected.sort(key=lambda x: x.index[2])  ## sorted
             multiSweeps = True
         else:
             getSpikeFeature = True  ## Default not to show spike features
             multiSweeps = False
         for kkk, sel in enumerate(selected):
             treeLevel = len(sel.index)  ## group 1; series, 2; sweep: 3; trace: 4
+            # if treeLevel !=use_level:
+            #     print(f'sel level {treeLevel}, max level {use_level}')
+            #     continue
+            if treeLevel==4 and kkk==0: # init a new selection buffer
+                self.currentPulseTree.selectedTraceIndex = [] # temporally hold trace index that user wants to show at sweep level and above
             self.checkSeriesType(sel)
             if treeLevel < 1:
                 return  ## do nothing at group level
             if treeLevel == 2:  ##  series level: all sweeps, all channels
                 # self.checkSeriesType(sel)  ## check protocol type for this selection
                 if self.currentPulseTree.filetype == ".dat":
                     if (
@@ -5591,22 +5955,32 @@
                     ):
                         if self.showSpikePanelsFlag != 1:
                             self.showSpikePanels()
                         self.plotSingleSeries(sel)
                         # self.plotSingleSeries3D(sel)
                         self.parameter_Tab.clear()
                         self.plotAveragedTraces(sel)
+                        
                 elif self.currentPulseTree.filetype == ".abf":
                     self.plotSingleSeries_ABF(sel)
+                    
+                elif self.currentPulseTree.filetype == ".nwb":
+                    children = getAllSiblings(sel)
+                    sel.setExpanded(True)
+                    for c in children: # shrink all siblings
+                        c.setExpanded(False)
+                    sweepTableIndies  = [c.index[2] for c in getAllChildIndexFromItem(sel)]
+                    self.plotSeletedSweeps_NWB(sweepTableIndies, newAxis=True,chanIdx = self.currentPulseTree.selectedTraceIndex)
+                break
 
             if treeLevel == 3:  ##  sweep level: all channels at this sweep
                 if self.currentPulseTree.filetype == ".dat":
                     self.plotSingleSweep(sel, kkk, Nsel, getSpikeFeature, multiSweeps)
                     self.parameter_Tab.clear()
-                else:
+                elif self.currentPulseTree.filetype == ".abf":
                     if kkk == 0:
                         plotHandle = self.trace_view.addPlot(row=0, col=0)
                         self.plotItemList.append(plotHandle)
                     segmentIdx = [sel.index[1], sel.index[2]]
                     trace = (
                         self.currentPulseTree.abfBlocks[segmentIdx[0]]
                         .segments[segmentIdx[1]]
@@ -5617,16 +5991,48 @@
                         plotHandle,
                         segmentIdx,
                         trace,
                         None,
                         highCutOff=None,
                         analaysisSpike=True,
                     )
-
-            if treeLevel == 4:  ##  trace level: all sweeps, all channels
+                elif self.currentPulseTree.filetype == ".nwb": # sweep level
+                    if len(selected) == 1: # if one sweep is slected.
+                        sel  =selected[0]
+                        children = getAllSiblings(sel)
+                        # sel.setExpanded(True)
+                        for c in children: # shrink all siblings
+                            c.setExpanded(False)
+                    self.currentPulseTree.selectedTraceIndex = sorted(list(set(self.currentPulseTree.selectedTraceIndex)))
+                    # self.get_patchview_sweep(self.sweepNames[sweep_index])
+                    # swGps = self.currentPulseTree.pvEphy.get_sweepgroup() # all sweep groups
+                    # sweepTableIndies = []
+                    # for sel in selected:
+                    #     swG = swGps[swGps.sweepGroupNames[sel.index[1]]] # sweep group
+                    sweepTableIndies = [sel.index[2] for sel in selected]
+                    metaInfos, stims, resps = self.plotSeletedSweeps_NWB(sweepTableIndies, chanIdx = self.currentPulseTree.selectedTraceIndex,
+                    newAxis=True, allSweeps=True) # return list of metaInfo for selected sweeps
+                    metaInfo = metaInfos[-1] ## just show the last one
+                    self.addNWB_metaIinfo(metaInfo) ## we will need to reset the metaInfo before adding new
+                    if getSpikeFeature:
+                        print('to be implemented in  plot_alignedSpikes_SingleTrace_NWB')
+                        ## in  plot_alignedSpikes_SingleTrace_NWB
+                        # self.plot_splitter.setStretchFactor(0, 1)
+                        # self.plot_splitter.setStretchFactor(1, 1)
+                        # self.trace_view2.show()
+                        # self.plot_alignedSpikes_SingleTrace(
+                        #     sel.index[2], mplWidget=self.spikes_view, plotWidget2=self.trace_view2
+                        # )
+                    break
+                else:
+                    print("File type not supported yet!")
+                    break
+            if treeLevel == 4:  ##  trace level:  all channels
+                if not (sel.index[3] in self.currentPulseTree.selectedTraceIndex): # avoid duplicated
+                    self.currentPulseTree.selectedTraceIndex.append(sel.index[3])
                 if self.currentPulseTree.filetype == ".dat":
                     self.vds = 0  ## no downsampling
                     if kkk == 0:
                         # self.checkSeriesType(self, sel)
                         plt = self.trace_view.addPlot(row=0, col=0)
                         # self.plotSingleTrace(plt, sel.node, sel.index, [], True, True, False) ## third arugument is for pen. if empty use default pen
                         if self.parameters["Protocols"]["This serie"]["Type"] in [
@@ -5654,18 +6060,53 @@
 
                     else:
                         self.plotSingleTrace(
                             plt, sel.node, sel.index, [], True, True, False
                         )
                 elif self.currentPulseTree.filetype == ".abf":
                     print("Need to figure out if there are multichannels")
-
+                else:
+                    sweepIdx = [sel.index[2]] # a single sweep
+                    if kkk==0:
+                        newAxis=True
+                    else:
+                        newAxis=False
+                    metaInfos, stims, resps = self.plotSeletedSweeps_NWB(sweepIdx, chanIdx=[sel.index[3]], newAxis=newAxis) # return list of metaInfo for selected sweeps
+                    metaInfo = metaInfos[-1] ## just show the last one
+                    # set parameters
+                    # add sweep level data on top of the file level data
+                    self.addNWB_metaIinfo() ## we will need to reset the metaInfo before adding new
+                    meta_data = np.array([(k, metaInfo[k]) for k in metaInfo],dtype=[("Parameter", object), ("Value", object)])
+                    self.parameter_Tab.appendData(meta_data)
+                    if getSpikeFeature:
+                        print('to be implemented in plot_alignedSpikes_SingleTrace_NWB')
+                        # self.plot_splitter.setStretchFactor(0, 1)
+                        # self.plot_splitter.setStretchFactor(1, 1)
+                        # self.trace_view2.show()
+                        # self.plot_alignedSpikes_SingleTrace(
+                        #     sel.index[3], mplWidget=self.spikes_view, plotWidget2=self.trace_view2
+                        # )
+        selTip = self.currentPulseTree.dat_file+'. Selected trace index: '
+        selTip +=', #'.join([str(x+1) for x in self.currentPulseTree.selectedTraceIndex])
+        self.QtFileNameLabel.setText(selTip)
         if self.plotItemList:  ## update mouse mode if not empty
             self.setViewboxMouseMode()
 
+    def addNWB_metaIinfo(self, metaInfo=None):
+        '''add file level metainformation to the parameter table
+        metainfo is a dictionary from pvEphy class'''
+        try:
+            if metaInfo is None:
+                metaInfo = self.currentPulseTree.pvEphy.metaInfo._asdict() # tree level metaInfo   
+            data = np.array([(k, metaInfo[k]) for k in metaInfo],dtype=[("Parameter", object), ("Value", object)])
+            self.parameter_Tab.clear()
+            self.parameter_Tab.setData(data)
+        except Exception as e:
+            print(e)
+
     def plotSingleStimTrace(self, plt, index, myPen):
         """only at series level!"""
         time, stim, stimInfo = self.currentPulseTree.bundle.stim(
             index
         )  ## assume only 1 channel is stimulating
         #        tr = self.currentPulseTree.bundle.pgf
 
@@ -5786,15 +6227,15 @@
         if len(sel.index) < 2:  ## not a series
             return
         elif len(sel.index) == 3:
             sel = sel.parent()
         elif len(sel.index) == 4:
             sel = sel.parent()
             sel = sel.parent()  ## to reach series level!
-        if self.currentPulseTree.filetype == ".dat":
+        if self.currentPulseTree.fileSourceFormat == ".dat":
             protocolType = self.querySessionProtocolByLabel(sel.node.Label)
             stimChanID = self.searchForStimchan(sel.node.Label)
             # print('stimchanID 5913', stimChanID)
             self.parameters["Protocols"]["This serie"] = {
                 "Type": protocolType,
                 "StimChanID": stimChanID,
             }
@@ -5945,14 +6386,186 @@
                 left=(f"Current ({self.currentPulseTree.abf_stimUnit })")
             )
             plt_stim.setXLink(plotHandle)  ## link x axis for all subplots
             self.trace_view.ci.layout.setRowStretchFactor(0, 3)
             self.trace_view.ci.layout.setRowStretchFactor(1, 1)
             plotHandle.setLabel("bottom", "", units="")
 
+    def plotSingleSweep_NWB(self,
+        plotHandle,
+        sweepIdx,
+        myPen,
+        highCutOff=None,
+        title=True,
+        scaleBar=True,
+        analaysisSpike=True,
+        plotStim=True,
+        stim=None,
+        data=None,
+        metaInfo = None, 
+        chanIdx: list=[]):
+        ''' Plot single sweep.
+
+        Parameters
+        -----------
+        chanIdx: list of channels to be plot. default: all channels
+        '''
+        ## check plotSingleTrace. Unify all the plotSingleTrace functions!
+        plotHandle.showGrid(x=True, y=True)
+        if stim is None or data is None or metaInfo is not None:
+            stim, data, metaInfo = self.currentPulseTree.pvEphy.getSweepData(sweepIdx)
+        data_fs = metaInfo['recording_rate']
+        plotHandle.setLabels(
+            bottom=("Time", metaInfo['recording_time_unit']),
+            left=(metaInfo['recording_unit']),
+        )
+        for d in data:
+            if len(d.shape) > 1:  # multi channels
+                if len(chanIdx)==0:
+                    chanIdx = range(d.shape[1])
+                for c in chanIdx:
+                    d[:,c] = self.bandPass_signal(d[:,c], highCutOff, fs=data_fs)
+                    time = np.arange(d.shape[0]) / data_fs
+                    if len(chanIdx)>1: # multi channel, use channel color. Otherwise, use myPen from input
+                        myPen = pg.mkPen(
+                            color=pg.intColor(c, hues = d.shape[1])
+                        )  ## the pen to draw this
+                    g = plotHandle.plot(time, d[:,c], pen=myPen)
+            else: # single channel``
+                d = self.bandPass_signal(d, highCutOff, fs=data_fs)
+                time = np.arange(len(d)) / data_fs
+                myPen = pg.mkPen('r')
+                g = plotHandle.plot(time, d,  pen=myPen)
+                plotHandle.autoRange()
+        if scaleBar:
+            scale = pg.ScaleBar(size=0.02, suffix="s")
+            scale.setParentItem(plotHandle.getViewBox())
+            scale.anchor((1, 1), (1, 1), offset=(-20, -20))
+        if title:
+            title_ = (
+                self.currentPulseTree.dat_file[:-4].split("\\")[-1]
+            )
+            plotHandle.setTitle(title_)
+        if plotStim:
+            self.trace_view.nextRow()  ## for stimulation
+            plt_stim = self.trace_view.addPlot(col=0, colspan=4)
+            # myPen = pg.mkPen('w')  ## the pen to draw this
+            stim_time = np.arange(len(stim)) / metaInfo['stim_rate']
+            plt_stim.plot(stim_time, stim, pen="w")
+            plt_stim.showGrid(x=True, y=True)
+
+            plt_stim.setLabels(bottom=(f"Time ({metaInfo['stim_time_unit']})"))
+            plt_stim.setLabels(
+                left=(f"Current ({metaInfo['stim_unit']})")
+            )
+            plt_stim.setXLink(plotHandle)  ## link x axis for all subplots
+            self.trace_view.ci.layout.setRowStretchFactor(0, 3)
+            self.trace_view.ci.layout.setRowStretchFactor(1, 1)
+            plotHandle.setLabel("bottom", "", units="")
+        return data, time, metaInfo
+
+    def getSpikeLineColor(self):
+        spkLine =self.splitViewTab_FP.getParTreePars("Spike detection")['Visual aesthetics']
+        spkLine_lw = spkLine[1]['line width'][0]
+        spkLine_col = spkLine[1]['line color'][0]
+        spkLine_col = MATPLTcolors.to_rgb(spkLine_col.name()) ## rgb color
+        spkLine_col = MATPLTcolors.rgb_to_hsv(spkLine_col)
+        return spkLine_lw, spkLine_col
+
+    def plotSeletedSweeps_NWB(self, sweepIdx: list[int], chanIdx:list=[], plotStim=True, newAxis=False, allSweeps=False):
+        ''' Control how to plot selected sweeps
+
+        Parameters
+        -----------
+        sweepIdx: `List` of `int`: sweep index. 
+
+        chanIdx: `List` of `int`: channel index to plot. Default [], all channels avaiable.
+        plotStim: `Bool`. Show stimulus or not.
+        newAxis: `Bool`. create a new subplot axis if True.
+        allSweeps: `Bool`. Plot all sweeps or not. For peformance purpose, we plot 8 sweeps of a series. Set True if desires to draw
+        all sweeps (for example, use selected more than 8 sweeps)
+        ''' 
+        if newAxis:
+            plotHandle = self.trace_view.addPlot(
+                col=0, colspan=4
+            )  ## add a subplot on the graphic layout
+            self.plotItemList.append(plotHandle)
+        else:
+            plotHandle = self.plotItemList[0]
+        ## loops through all the sweeps.
+        # nSweep = sel.childCount()
+        # sweepIdx = [sel.child(c).index[2] for c in range(nSweep)]
+        nSweep = len(sweepIdx)
+        drawN = 8
+        if allSweeps or nSweep <= drawN:
+            drawN = nSweep
+        else:      
+            # spkLine_lw, spkLine_col = self.getSpikeLineColor()        
+            sIdx = np.linspace(0, nSweep, drawN).astype(int)
+            sweepIdx = [sweepIdx[i] for i in sIdx if i < nSweep]
+
+        stims = []
+        resps = []
+        metaInfos = []
+        # selIdx = sel.index.copy()
+        allPens = []
+        idx = 0
+        for idx, sweepIdx_ in enumerate(sweepIdx):  # enumerate(block.segments):
+            myPen = pg.mkPen(
+                    color=pg.intColor(drawN - idx - 1, hues=drawN)
+                )  ## the pen to draw this
+            # qcol = pg.hsvColor(spkLine_col[0], 1.0-idx/drawN , 1.0, 1.0)
+            # myPen = pg.mkPen(color=qcol)
+            allPens.append(myPen)
+            stim, resp, metaInfo = self.currentPulseTree.pvEphy.getSweepData(sweepIdx_)
+            stims.append(stim)
+            resps.append(resp)
+            metaInfos.append(metaInfo)
+            self.plotSingleSweep_NWB(
+                plotHandle,
+                sweepIdx_,
+                myPen,
+                title=False,
+                scaleBar=False,
+                analaysisSpike=False,
+                plotStim=False,
+                stim = stim,
+                data = resp,
+                metaInfo = metaInfo,
+                chanIdx =chanIdx
+            )
+        
+        scale = pg.ScaleBar(size=0.02, suffix="s")
+        scale.setParentItem(plotHandle.getViewBox())
+        scale.anchor((1, 1), (1, 1), offset=(-20, -20))
+        plotHandle.setTitle(
+            self.currentPulseTree.dat_file[:-4].split("\\")[-1]
+        )
+
+        if plotStim:
+            if newAxis:
+                self.trace_view.nextRow()  ## for stimulation
+                plt_stim = self.trace_view.addPlot(col=0, colspan=4)
+                self.plotItemList.append(plt_stim)
+            else:
+                plt_stim = self.plotItemList[-1]
+            for idx, stim in enumerate(stims):
+                stim_time = np.arange(len(stim)) / metaInfo['stim_rate']
+                plt_stim.plot(stim_time, stim, pen=allPens[idx])
+            plt_stim.showGrid(x=True, y=True)
+            plt_stim.setLabels(bottom=("Time (s)"))
+            plt_stim.setLabels(
+                left=(f"Current ({metaInfos[0]['stim_unit']})")
+            )
+            plt_stim.setXLink(plotHandle)  ## link x axis for all subplots
+            self.trace_view.ci.layout.setRowStretchFactor(0, 3)
+            self.trace_view.ci.layout.setRowStretchFactor(1, 1)
+            plotHandle.setLabel("bottom", "", units="")
+        return metaInfos,stims,resps
+
     def plotSingleTrace_ABF(
         self,
         plotHandle,
         segmentIdx,
         trace,
         myPen,
         highCutOff=None,
@@ -6224,14 +6837,15 @@
             plt_stim.setTitle(title)
             self.trace_view.ci.layout.setRowStretchFactor(0, 3)
             self.trace_view.ci.layout.setRowStretchFactor(1, 1)
         else:
             for p in plt[:-1]:
                 p.setXLink(plt[-1])  ## link x axis for all subplots
 
+
     def getEphySpikePars(self):
         pv = self.splitViewTab_FP.getParTreePars("Spike detection")
         # This is just to get spikes peaks. Need to use higher cutoff for dvdt-v phase plot
         HF = pv["Spike detection parameters"][1]["High frequency cutoff"][
             0
         ]  # this may different than general filter options
         dv_cutoff = pv["Spike detection parameters"][1][
@@ -6251,24 +6865,27 @@
         ][0]
         baseline_interval = pv["Spike detection parameters"][1][
             "baseline_interval (min=0.05;max=0.15)"
         ][0]
         baseline_detect_thresh = pv["Spike detection parameters"][1][
             "baseline_detect_thresh (min=-30;max=150)"
         ][0]
-
+        start_latency = pv["Spike detection parameters"][1][
+            "start_latency (min=0.001;max=0.005)"
+        ][0]
         return (
             dv_cutoff,
             min_height,
             min_peak,
             thresh_frac,
             baseline_interval,
             baseline_detect_thresh,
             max_interval,
             HF,
+            start_latency,
         )
 
     def getSingleTraceFeature_ABF(self, v, t, seriesIdx):
         self.updateUserParamters()
         v = np.array(v)
         stimInfo = self.currentPulseTree.abf_stimInfo
         sweepIdx = seriesIdx[1]
@@ -6406,14 +7023,15 @@
             min_height1,
             min_peak1,
             thresh_frac1,
             baseline_interval1,
             baseline_detect_thresh1,
             max_interval1,
             filterHighCutFreq_spike,
+            start_latency
         ) = self.getEphySpikePars()
 
         ## this is to get spike peak.
         if filterHighCutFreq_spike >= sampleRate / 2:
             filterHighCutFreq_signal = np.floor((sampleRate - 100.0)) / 2  ## KHz
 
         EphysObject = efex.EphysSweepFeatureExtractor(
@@ -6426,22 +7044,24 @@
             dv_cutoff=dv_cutoff1,
             max_interval=max_interval1,
             min_height=min_height1,
             min_peak=min_peak1,
             thresh_frac=thresh_frac1,
             baseline_interval=baseline_interval1,
             baseline_detect_thresh=baseline_detect_thresh1,
+            start_latency = start_latency,
         )
         EphysObject.process_spikes()
         spike_df, sweep_df = extract_sweep_feature(t, v, curr, start, end, EphysObject)
         v_filtered = ephys_ft.calculate_v_filter(v, t, filterHighCutFreq_signal / 1000)
         dvdt = ephys_ft.calculate_dvdt(v, t, filterHighCutFreq_signal / 1000)
         dvdt1 = np.insert(dvdt, 0, 0)
         if EphysObject._spikes_df.size:
             peaks = spike_df["peak_index"].to_list()  ## lis tof peak index
+            threhold_index = spike_df["threshold_index"].to_list()
             try:
                 maxSPwidth = int(spike_df["width"].max(skipna=True) * sampleRate * 2.5)
             except:
                 maxSPwidth = int(
                     (spike_df["peak_index"] - spike_df["threshold_index"]).max() * 5
                 )
                 print("exception happens")
@@ -6466,30 +7086,152 @@
                 start_index = p - before_
                 end_index = p + after_
                 # print(start_index, end_index, sweepCount)
                 waves[:, j] = v_filtered[start_index:end_index]
                 waves_dvdt[:, j] = dvdt1[start_index:end_index]
         else:
             peaks = []
+            threhold_index = []
             waves = []
             waves_dvdt = []
             waveTime = []
         return (
             t,
             v_filtered,
             dvdt1,
             peaks,
             waveTime,
             waves,
             waves_dvdt,
             spike_df,
             end - start,
             dv_cutoff1,
+            threhold_index
         )
 
+    def prepareVoltageNDarray_NWB(self, sel):
+        children = getAllChildIndexFromItem(sel)
+        sweepIdx = [c.index[2] for c in children] ## sweep table index
+        minSample = 1e10
+        resps = []
+        for sidx in sweepIdx:
+            stim, response, metaInfo = self.currentPulseTree.pvEphy.getSweepData(sidx)
+            # response are list of np array. 1 for single channel; n for multiple channel
+            if len(response[0]) < minSample:
+                minSample = len(response[0])
+            resps.append(response) ##
+        nChan = len(response)
+        t = np.linspace(0, minSample/metaInfo["recording_rate"], minSample)
+        data = np.array(resps)
+        if len(data.shape) == 4:
+            data = data [:,0,:,:] # squeeze. sweep, np.newaxis, time, channel
+        else:
+            data = data[:,0,:,np.newaxis] # squeeze. sweep, np.newaxis, time, channel
+        data = np.swapaxes(data, 0, 1)[:minSample]  # time, sweep, channel
+        return t, stim, data, metaInfo
+
+    def getSingleTraceFeature_NWB(self, sweepTableIndex, sweepIdx):
+        self.updateUserParamters()
+        stim, v, metaInfo = self.currentPulseTree.pvEphy.getSweepData(sweepTableIndex)
+        t = np.linspace(0, len(v) / metaInfo["recording_rate"], len(v))
+        v = v *1000.0
+        sampleRate = metaInfo["recording_rate"]
+        start = 1.0
+        end = 2.0
+        curr = -110.0+ sweepIdx*20.0
+        if self.parameters["HF"] < sampleRate / 2:
+            filterHighCutFreq_signal = self.parameters["HF"]  ## 10 KHz
+        else:
+            filterHighCutFreq_signal = np.floor((sampleRate - 100.0)) / 2  ## KHz
+        (
+            dv_cutoff1,
+            min_height1,
+            min_peak1,
+            thresh_frac1,
+            baseline_interval1,
+            baseline_detect_thresh1,
+            max_interval1,
+            filterHighCutFreq_spike,
+        ) = self.getEphySpikePars()
+
+        ## this is to get spike peak.
+        if filterHighCutFreq_spike >= sampleRate / 2:
+            filterHighCutFreq_signal = np.floor((sampleRate - 100.0)) / 2  ## KHz
+
+        EphysObject = efex.EphysSweepFeatureExtractor(
+            t=t,
+            v=v,
+            i=stim,
+            start=start,
+            end=end,
+            filter=filterHighCutFreq_spike / 1000,
+            dv_cutoff=dv_cutoff1,
+            max_interval=max_interval1,
+            min_height=min_height1,
+            min_peak=min_peak1,
+            thresh_frac=thresh_frac1,
+            baseline_interval=baseline_interval1,
+            baseline_detect_thresh=baseline_detect_thresh1,
+        )
+        EphysObject.process_spikes()
+        spike_df, sweep_df = extract_sweep_feature(t, v, curr, start, end, EphysObject)
+        v_filtered = ephys_ft.calculate_v_filter(v, t, filterHighCutFreq_signal / 1000)
+        dvdt = ephys_ft.calculate_dvdt(v, t, filterHighCutFreq_signal / 1000)
+        dvdt1 = np.insert(dvdt, 0, 0)
+        if EphysObject._spikes_df.size:
+            peaks = spike_df["peak_index"].to_list()  ## lis tof peak index
+            try:
+                maxSPwidth = int(spike_df["width"].max(skipna=True) * sampleRate * 2.5)
+            except:
+                maxSPwidth = int(
+                    (spike_df["peak_index"] - spike_df["threshold_index"]).max() * 5
+                )
+                print("exception happens")
+            try:
+                before_ = (
+                    int((spike_df["peak_index"] - spike_df["threshold_index"]).max())
+                    + 100
+                )
+            except:
+                maxSPwidth = int(maxSPwidth // 2)
+            try:
+                after_ = int((spike_df["trough_index"] - spike_df["peak_index"]).max())
+                if after_ > 3 * before_:
+                    after_ = 3 * before_
+            except:
+                after_ = int(maxSPwidth - maxSPwidth // 20)
+
+            waves = np.zeros((after_ + before_, len(peaks)))
+            waves_dvdt = np.zeros((after_ + before_, len(peaks)))
+            waveTime = np.arange(-before_, after_) / sampleRate * 1e3
+            for j, p in enumerate(peaks):
+                start_index = p - before_
+                end_index = p + after_
+                # print(start_index, end_index, sweepCount)
+                waves[:, j] = v_filtered[start_index:end_index]
+                waves_dvdt[:, j] = dvdt1[start_index:end_index]
+        else:
+            peaks = []
+            waves = []
+            waves_dvdt = []
+            waveTime = []
+        return (
+            t,
+            v_filtered,
+            dvdt1,
+            peaks,
+            waveTime,
+            waves,
+            waves_dvdt,
+            spike_df,
+            end - start,
+            dv_cutoff1,
+        )
+
+
     def plot_dvdt_v_phasePlot(self, v_spike, dvdt_spike, sweepNumber, plotWidget):
         plotWidget.clear()  ## refresh the layout
         plt = plotWidget.addPlot()
         plt.showGrid(x=True, y=True)
         if not isinstance(v_spike, list):
             for j in range(v_spike.shape[1]):
                 myPen = pg.mkPen(
@@ -6519,26 +7261,31 @@
             plt.setTitle(
                 "Sweep "
                 + str(sweepNumber + 1)
                 + " Spike count:"
                 + str(v_spike.shape[1])
             )
         return plt
+    
+    def plot_alignedSpikes_SingleTrace_NWB(self, stim, data):
+        ## TODO: make use of cached analysis data
+        pass
 
     def plot_alignedSpikes_SingleTrace(
         self,
         traceIdx,
         axis=None,
         mplWidget=None,
         plotWidget2=None,
         isABF=False,
         trace=None,
         time=None,
     ):
-        if isABF:
+        threhold_index = []
+        if self.currentPulseTree.fileSourceFormat  == ".abf":
             (
                 t,
                 v,
                 dvdt,
                 peaks,
                 waveTime,
                 waves,
@@ -6552,38 +7299,69 @@
                 + " "
                 + "Block"
                 + str(traceIdx[0] + 1)
                 + " Sweep"
                 + str(traceIdx[1] + 1)
             )
             sweepNumber = traceIdx[1]
-        else:
+        elif self.currentPulseTree.fileSourceFormat  == ".dat":
             (
                 t,
                 v,
                 dvdt,
                 peaks,
                 waveTime,
                 waves,
                 waves_dvdt,
                 spike_df,
                 dur,
                 dv_cutoff,
+                threhold_index,
             ) = self.getSingleTraceFeature(traceIdx)
             title = (
                 self.sliceName[:-4]
                 + " "
                 + "Series"
                 + str(traceIdx[1] + 1)
                 + " sweep"
                 + str(traceIdx[2] + 1)
             )
             sweepNumber = traceIdx[2]
-
-        print(title)
+        elif self.currentPulseTree.fileSourceFormat  == ".nwb":
+            sel = self.currentPulseTree.selectedItems()[0]
+            # grpIndex = sel.index[0]
+            # swGpIndex = sel.index[1]
+            sweepTableIndex= sel.index[2] # absolute sweep number in sweep table
+            # sweepNumber = sweepTableIndex
+            # swpList = list(self.currentPulseTree.pvEphy.sweepGroups[swGpIndex].patchview_sweeps.keys())
+            # numberOfSweep = len(swpList) # sweep group
+            # relativeSweepIndex = swpList.index(f'{sweepTableIndex:03}') # sweep index in sweep group
+            try:
+                (t,v,dvdt,
+                    peaks,
+                    waveTime,
+                    waves,
+                    waves_dvdt,
+                    spike_df,
+                    dur,
+                    dv_cutoff,
+                ) = self.getSingleTraceFeature_NWB(sweepTableIndex, relativeSweepIndex)
+            except:
+                mplWidget.figure.clear()
+                mplWidget.clf()
+                plotWidget2.clear()
+                print('error get spikes for nwb')
+                return
+            title = 'sweep ' + str(sweepNumber)
+        if len(peaks) == 0:
+            # print('No spike detected')
+            mplWidget.figure.clear()
+            mplWidget.clf()
+            plotWidget2.clear()
+            return
         if mplWidget == None:  ## pure matplotlib
             fig = MATPLT.figure(figsize=(10, 10))
             fig.canvas.set_window_title(title)
             MATPLT.subplot(2, 1, 1)
             MATPLT.plot(t, v)
             MATPLT.plot(t, dvdt)
             for p in peaks:
@@ -6613,56 +7391,65 @@
                 "Spike detection"
             )["Spike detection parameters"][1]["peak voltage (min=-30;max=150)"][0]
             axes[0].axhline(y=peakHeight_threhold, color="r", linestyle="--")
 
             axes[0].title.set_text(title)
             axes[0].set_xlabel("Time (S)")
             axes[0].set_ylabel("Voltage (mV)")
+            xlim_range = axes[0].get_xlim()
+
             if len(peaks) > 0:
+                peakTime = [t[p] for p in peaks]
+                if xlim_range[-1] > peakTime[-1]+1.0:
+                    xextent = peakTime[-1]+1.0
+                else:
+                    xextent = xlim_range[-1]
+                axes[0].set_xlim([xlim_range[0], xextent])
                 for p in peaks:
                     axes[0].plot(t[p], v[p], "og", zorder=1)
-                # axes[0].legend(['dv/dt','v', 'peak'])
-
+                for p in threhold_index:
+                    axes[0].plot(t[p], v[p], "bx", zorder=1)
+                
                 plt1 = mplWidget.figure.add_subplot(gs[0, 1])
                 axes.append(plt1)
                 for j in range(len(peaks)):
                     axes[1].plot(waveTime, waves[:, j])
                 axes[1].title.set_text(
                     f"N={len(peaks)}, avg.rate: {len(peaks)/dur:.1f} Hz"
                 )
                 axes[1].set_xlabel("Time (mS)")
                 axes[1].set_ylabel("Voltage (mV)")
                 axes[1].grid("on")
-
                 plt2 = mplWidget.figure.add_subplot(gs[1, 0])
                 axes.append(plt2)
-                peakTime = [t[p] for p in peaks]
+                
                 axes[2].plot(peakTime, spike_df["width"] * 1e3, "k", linewidth=1.0)
                 axes[2].plot(peakTime, spike_df["width"] * 1e3, "g.")
                 axes[2].set_xlabel("Time (S)")
                 axes[2].set_ylabel("Spike width (mS)")
-                xlim_range = axes[0].get_xlim()
+                
                 axes[2].grid("on")
-                axes[2].set_xlim([xlim_range[0], xlim_range[-1]])
+                xlim_range = axes[0].get_xlim()
+                axes[2].set_xlim([xlim_range[0], xextent])
 
                 plt3 = mplWidget.figure.add_subplot(gs[1, 1])
                 axes.append(plt3)
                 peakTime = [t[p] for p in peaks]
                 peakV = [v[p] for p in peaks]
                 axes[3].plot(peakTime, peakV, "k", linewidth=1.0)
                 axes[3].plot(peakTime, peakV, "g.")
                 axes[3].grid("on")
                 axes[3].set_xlabel("Time (S)")
                 axes[3].set_ylabel("Peak voltage (mv)")
-                axes[3].set_xlim([xlim_range[0], xlim_range[-1]])
+                xlim_range = axes[0].get_xlim()
+                axes[3].set_xlim([xlim_range[0], xextent])
             else:
                 axes[0].legend(["dv/dt", "v"])
 
             mplWidget.draw()
-            #                    print(c)
             mplWidget.figure.tight_layout()
 
         if plotWidget2 != None:
             self.plot_dvdt_v_phasePlot(waves, waves_dvdt, sweepNumber, plotWidget2)
 
     def getCurrentIdx(self):
         #        if hasattr(self, 'currentPulseTree'):
@@ -6818,28 +7605,28 @@
         modeIdx = int.from_bytes(
             trace.RecordingMode, byteorder=self.currentPulseTree.bundle.endian
         )
         #        print('Mode Idx: %g' % modeIdx)
         traceInfo = {"Recording mode": RECORDMODE[modeIdx]}
         return traceInfo
 
-    def bandPass_signal(self, data, highCutOff=None, lowCutOff=None, useButter=False):
+    def bandPass_signal(self, data, highCutOff=None, lowCutOff=None, useButter=False, fs=None):
         if self.globalSettings.p.getValues()["data preprocessing"][1][
             "Apply Notch filter"
         ][0]:
             w0 = self.parameters["Notch"]
             # print('notch filter', w0, self.parameters['fs'])
             b, a = signal.iirnotch(w0, 1000.0, self.parameters["fs"])
             f = signal.filtfilt(b, a, data)
         else:
             f = data
         if (
             self.parameters["filter_option"] == 0 and useButter == False
         ):  ## default fourth order Bessel-Thomson filter
-            self.Bessel_lowpass(highCutOff, None, lowCutOff)
+            self.Bessel_lowpass(highCutOff, fs, lowCutOff)
             f = signal.sosfiltfilt(self.parameters["bessel_filter_sos"], f)
         else:  ## Butter
             self.butter_bandpass(highCutOff, lowCutOff, order=2)
             # print("second order Butter bandpass")
             f = signal.sosfiltfilt(self.parameters["butter_sos"], f)
 
         return f
@@ -6954,15 +7741,15 @@
     def interceptPerpendecularLine(self, a, b, x0, y0):
         x = (x0 + a * y0 - a * b) / (1 + a**2)
         y = a * x + b
         D = np.sqrt((x - x0) ** 2 + (y - y0) ** 2)
         return x, y, D
 
     def measureDist2Pia(self):
-        if self.pia is not None:
+        if hasattr(self, 'pia') and self.pia is not None:
             df = pd.DataFrame(self.pia[:, :2], columns=["x", "y"]).sort_values(
                 by="x", inplace=False
             )
             ransac = linear_model.RANSACRegressor()
             ransac.fit(df["x"].values.reshape(-1, 1), df["y"].values.reshape(-1, 1))
             slope = ransac.estimator_.coef_[0][0]
             intercept = ransac.estimator_.intercept_[0]
@@ -6985,95 +7772,280 @@
             self.splitViewTab_morph.matplotViews["2D"].draw()
             self.splitViewTab_morph.tables["Summary"].clear()
             df = np.array(
                 df.to_records(index=False)
             )  ## format dataframe for using in QtTable wiget
             self.splitViewTab_morph.tables["Summary"].appendData(df)
             self.splitViewTab_morph.tables["Summary"].show()
-
-    def morph_analysis_event(self, param, changes):
-        pv = self.splitViewTab_morph.getParTreePars("Analysis")
-        step_size=pv['Options'][1]['Bin size (um)'][0]
-        anlge_step_size=pv['Options'][1]['Angle bin (degree)'][0]*np.pi/180
-        useFullRange=pv['Options'][1]['Use full range for density plot'][0]
-        showColorBar=pv['Options'][1]['Show color bar for density plot'][0]
-        showAxisVal=pv['Options'][1]['Show axis for density plot'][0]
-        smoothBins= pv['Options'][1]['Gaussian window size (num. bins)'][0]
-        smoothStandardDeviation = pv['Options'][1]['Std of Gaussian kernel (num. bins)'][0]
+    
+    def getNeutriteColors(self, neutriteColors, hex=False):
+        ''' from Qcolor to rgb or hex color
+        rgb: True: rgb color, False: hex color
+        '''
+        bdColors = neutriteColors['Basal dendrite'][0]
+        apColors = neutriteColors['Apical dendrite'][0]
+        axonColors = neutriteColors['Axon'][0]
+        somaColors = neutriteColors['Soma'][0]
+        bdColors = [bdColors.red(), bdColors.green(), bdColors.blue()]
+        apColors = [apColors.red(), apColors.green(), apColors.blue()]
+        axonColors = [axonColors.red(), axonColors.green(), axonColors.blue()]
+        somaColors = [somaColors.red(), somaColors.green(), somaColors.blue()]
+        colors = [apColors,bdColors, axonColors, somaColors]
+        if hex:
+            for c in range(len(colors)):
+                colors[c] = '#%02x%02x%02x' % tuple(colors[c])
+        else:
+            colors = np.array([apColors,bdColors, axonColors, somaColors])/255 ## [0,1]
+        return colors
+
+    def update_dendrogram(self):
+        fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " Dendrogram").getFigure()
+        fig.clf()
+        ax = fig.add_subplot(111)
+        ax.cla()
+        plot_dendrogram(self.neuronMorph, ax= ax, show_diameters=True)
+
+    def morph_measure_event(self, param, changes):
+        pv = self.splitViewTab_morph.getParTreePars("Parameters")
+        step_size=pv['Parameters'][1]['Bin size (um)'][0]
+        anlge_step_size=pv['Parameters'][1]['Angle bin (degree)'][0]*np.pi/180
+        smoothBins= pv['Parameters'][1]['Gaussian window size (num. bins)'][0]
+        smoothStandardDeviation = pv['Parameters'][1]['Std of Gaussian kernel (num. bins)'][0]
+        useFullRange=pv['Figure options'][1]['Use full range for density plot'][0]
+        showColorBar=pv['Figure options'][1]['Show color bar for density plot'][0]
+        showAxisVal=pv['Figure options'][1]['Show axis for density plot'][0]
+        customAxiRange=pv['Figure options'][1]["Custom axis range"][1]
+        customRange_plane_activate = customAxiRange['plane density'][1]['activate'][0]
+        plOps = customAxiRange['plane density'][1]
+        customRange_planeAxisOptions = [customRange_plane_activate, plOps['X min'][0], 
+        plOps['X max'][0],plOps['Y min'][0],plOps['Y max'][0]]
+        customRange_polar_activate = customAxiRange['polar density'][1]['activate'][0]
+        customRange_polarAxisOptions = [customRange_polar_activate, customAxiRange['polar density'][1]['R max'][0]]
+        showgrid = pv['Figure options'][1]['Show grid'][0]
+        cmap = pv['Figure options'][1]['Color map'][0]
+        pvm = self.splitViewTab_morph.getParTreePars("Measurments")
         for param, change, data in changes:
             childName = param.name()
-            if childName in [ "Rotate tree (degree)", "Draw contour", "Ignore diameters", "Scale bar length"]:
-                fname = cleanASCfile(
-                    self.currentMorphTreeFile
-                )  ## to clean not-wanted sections
-                self.updateTreeMorphView(fname)
-                if fname[-8:] == "_mod.ASC":
-                    os.remove(fname)
-            if childName in ["Rotate tree (degree)", "Bin size (um)", "Gaussian window size (num. bins)",
-             "Std of Gaussian kernel (num. bins)", "Angle bin (degree)", "Use full range for density plot",
-             "Show color bar for density plot", "Show axis for density plot"]:
-                if self.currentAnMorphView!="":
-                    childName = self.currentAnMorphView
-            if childName == "Sholl analysis":
+            if childName in ["Sholl analysis"]:
                 self.update_sholl(step_size=step_size,smoothBins=smoothBins,
                 smoothStandardDeviation=smoothStandardDeviation)
-                self.currentAnMorphView = childName
-            if childName in ["X axis density"]:
+                # self.currentAnMorphView = childName
+            elif childName == "Dendrogram":
+                self.update_dendrogram()
+            elif childName in ["X axis density"]:
                 self.update_density('x',step_size=step_size,smoothBins=smoothBins,
                 smoothStandardDeviation=smoothStandardDeviation)
-                self.currentAnMorphView = childName
-            if childName in ["Y axis density"]:
+                # self.currentAnMorphView = childName
+            elif childName in ["Y axis density"]:
                 self.update_density('y',step_size=step_size,smoothBins=smoothBins,
                 smoothStandardDeviation=smoothStandardDeviation)
-                self.currentAnMorphView = childName
-            if childName in ["XY plane density"]:
+                # self.currentAnMorphView = childName
+            elif childName in ["XY plane density"]:
                 self.update_2D_density(step_size=step_size, useFullRange=useFullRange,
                 showColorbar=showColorBar, showAxisValues=showAxisVal,smoothBins=smoothBins,
-                smoothStandardDeviation=smoothStandardDeviation)
-                self.currentAnMorphView = childName
-            if childName in ["XY polar density"]:
-                self.update_2D_polar_density(step_size=step_size, angle_step = anlge_step_size)
-                self.currentAnMorphView = childName
-            if childName == "Update cell names":
+                smoothStandardDeviation=smoothStandardDeviation, cmap=cmap)
+                # self.currentAnMorphView = childName
+            elif childName in ["XY polar density", "R max"]:
+                self.update_2D_polar_density(step_size=step_size, angle_step = anlge_step_size,
+                 axiOps = customRange_polarAxisOptions, showgrid=showgrid, cmap = cmap)
+                # self.currentAnMorphView = childName
+            elif childName in ["Features",'Make histogram']:
+                feature = pvm['Measurement'][1]["Feature histograms"][1]['Features'][0]
+                self.update_featureHistogram(feature)
+            elif childName == "Update cell names":
                 self.updateInterCellDistance()
+            elif childName in ['Distance function', "Compute barcode"]:
+                distFunc = pvm['Measurement'][1]["Persistent barcode"][1]['Distance function'][0]
+                self.drawBarcode(distFunc)
             elif childName == "Distance to Pia":
                 self.measureDist2Pia()
-            elif childName == "Export High resolution figure":
-                dpi = pv["Save options"][1]["DPI"][0]
-                format = pv["Save options"][1]["Format"][0]
-                figsize = pv["Save options"][1]["Size"][0]
-                fig = self.splitViewTab_morph.matplotViews["2D"].getFigure()
-                self.saveHighResFigure(fig, dpi, figsize, format)
-
-    def saveHighResFigure(self, fig, dpi, figsize, format):
-        fig.set_size_inches(figsize, figsize, forward=True)
-        fig.savefig(
-            self.currentMorphTreeFile[:-4] + "." + format,
-            dpi=dpi,
-            format=format,
-            metadata=None,
-            bbox_inches=None,
-            pad_inches=0.1,
-            facecolor="auto",
-            edgecolor="auto",
-            transparent=True,
-            backend=None,
-        )
-        self.showdialog(f"{self.currentMorphTreeFile[:-4]} saved!")
+            elif childName == "Path length histogram":
+                self.update_pathLengthHistogram()
+            elif childName == "Apical dendrite stem directionality histogram":
+                self.update_ad_stem_directionality_histogram()
+            elif childName == "Close all floating windows":
+                self.MatPlotWindows = []
+                GCollector.collect()
+
+    def morph_export_event(self, param, changes):
+        pve = self.splitViewTab_morph.getParTreePars("Export")
+        pv = self.splitViewTab_morph.getParTreePars("Parameters")
+        step_size=pv['Parameters'][1]['Bin size (um)'][0]
+        anlge_step_size=pv['Parameters'][1]['Angle bin (degree)'][0]*np.pi/180
+        smoothBins= pv['Parameters'][1]['Gaussian window size (num. bins)'][0]
+        smoothStandardDeviation = pv['Parameters'][1]['Std of Gaussian kernel (num. bins)'][0]
+        useFullRange=pv['Figure options'][1]['Use full range for density plot'][0]
+        for param, change, data in changes:
+            childName = param.name()
+            if childName == "Export High resolution figure":
+                dpi = pve["Export Morphology"][1]["DPI"][0]
+                format = pve["Export Morphology"][1]["Format"][0]
+                self.saveHighResFigure(dpi, format)
+            elif childName == 'Save to disk':
+                linearProjection = pve['Export Morphology density'][1]['linear projections'][0]
+                xyPlane = pve['Export Morphology density'][1]['xy cartesian'][0]
+                xyPoloar = pve['Export Morphology density'][1]['xy polar'][0]
+                savedResults = ""
+                if linearProjection:
+                    saveLinearProjectionDensity(self.neuronMorph, step_size=step_size,smoothBins=smoothBins,
+                smoothStandardDeviation=smoothStandardDeviation, neuronName=self.currentMorphTreeFile[:-4])
+                    ## message box to notifiy the user that the file is saved
+                    savedResults+="linear projection (x axis, yaxis)\n "
+                if xyPlane:
+                    save2DPlaneDensity(self.neuronMorph, step_size,  useFullRange, smoothBins,
+                smoothStandardDeviation,  neuronName=self.currentMorphTreeFile[:-4])
+                    savedResults+="2D plane density\n "
+                if xyPoloar:
+                    save2DPolarDensity()
+                    savedResults+="2D polar density\n "
+                self.showdialog(f"{self.currentMorphTreeFile[:-4]} saved!", savedResults)
+
+    def morph_analysis_event(self, param, changes):
+        pv = self.splitViewTab_morph.getParTreePars("Parameters")
+        step_size=pv['Parameters'][1]['Bin size (um)'][0]
+        anlge_step_size=pv['Parameters'][1]['Angle bin (degree)'][0]*np.pi/180
+        smoothBins= pv['Parameters'][1]['Gaussian window size (num. bins)'][0]
+        smoothStandardDeviation = pv['Parameters'][1]['Std of Gaussian kernel (num. bins)'][0]
+        useFullRange=pv['Figure options'][1]['Use full range for density plot'][0]
+        showColorBar=pv['Figure options'][1]['Show color bar for density plot'][0]
+        showAxisVal=pv['Figure options'][1]['Show axis for density plot'][0]
+        customAxiRange=pv['Figure options'][1]["Custom axis range"][1]
+        customRange_plane_activate = customAxiRange['plane density'][1]['activate'][0]
+        plOps = customAxiRange['plane density'][1]
+        customRange_planeAxisOptions = [customRange_plane_activate, plOps['X min'][0], 
+        plOps['X max'][0],plOps['Y min'][0],plOps['Y max'][0]]
+        customRange_polar_activate = customAxiRange['polar density'][1]['activate'][0]
+        customRange_polarAxisOptions = [customRange_polar_activate, customAxiRange['polar density'][1]['R max'][0]]
+        seabornStyle  = pv['Figure options'][1]["Figure aesthetics"][0]
+        showgrid = pv['Figure options'][1]['Show grid'][0]
+        cmap = pv['Figure options'][1]['Color map'][0]
+        neutriteColors = pv['Figure options'][1]['Neutrites color'][1]
+        morphorOnly = pv['Figure options'][1]['Morphology only'][0]
+        showTitle = pv['Figure options'][1]['Show title'][0]
+        for param, change, data in changes:
+            childName = param.name()
+            if childName == "Figure aesthetics":
+                sns.set_style(seabornStyle)
+            if childName in [ "Rotate tree (degree)", "Draw contour",  "Scale bar length"]:
+                fname = cleanASCfile(
+                    self.currentMorphTreeFile
+                )  ## to clean not-wanted sections
+                self.updateTreeMorphView(fname, redraw=True,morphorOnly=morphorOnly, showTitle=showTitle)
+                if fname[-8:] == "_mod.ASC":
+                    os.remove(fname)
+            if childName in ["Basal dendrite", "Apical dendrite", "Axon", "Soma","Morphology only", "Show title"]:
+                colors = self.getNeutriteColors(neutriteColors, hex=False)
+                for idx, k in enumerate(self.NeutriteColors):
+                    if idx == len(colors):
+                        break
+                    self.NeutriteColors[k] = colors[idx]
+                self.updateTreeMorphView(self.currentMorphTreeFile, redraw=True,morphorOnly=morphorOnly, showTitle=showTitle)
+
+    def drawBarcode(self, distanceFunc):
+        if (not hasattr(self, "morphPy_N")) or  self.morphPy_N is None:
+            self.update_mpfeatures(False)
+        else:
+            df = getPersistanceBarcode(self.morphPy_N , distanceFunc)
+            fig = self.makeNewMatPlotWindow(title=self.currentMorphTreeFile.split('\\')[-1]+ " persistent diagrams",
+            size=(15,10)).getFigure()
+            fig.clf()
+            ax1 = fig.add_subplot(121)
+            ax1.set_title("Persistent barcode")
+            ax1.set_xlabel("Life time")
+            ax1.set_ylabel("Features")
+            for i in range(len(df)):
+                ax1.plot([df['birth'][i], df['death'][i]], [i, i], color='k', lw=1)
+
+            ax2 = fig.add_subplot(122)
+            ax2.set_title("Persistent diagram")
+            ax2.set_xlabel("Birth "+ distanceFunc)
+            ax2.set_ylabel("Death "+ distanceFunc)
+            ax2.scatter(df['birth'], df['death'], s=10)
+            minDf = min(df['birth'].min(), df['death'].min())
+            maxDf = max(df['birth'].max(), df['death'].max())
+            ax2.plot([minDf, maxDf], [minDf, maxDf], color='k', linestyle='dashed', linewidth=1)
+            fig.tight_layout()
+
+    def makeNewMatPlotWindow(self, title='figure',size=(8,6)):
+        if not hasattr(self, 'MatPlotWindows'):
+            self.MatPlotWindows = []
+        self.MatPlotWindows.append(MatplotView(size=size, title=title))
+        self.MatPlotWindows[-1].show()
+        return self.MatPlotWindows[-1]
+
+    def saveHighResFigure(self,dpi, format):
+        if format =='swc': # save as swc
+            self.neuronMorph.remove_unifurcations()
+            self.neuronMorph.write(self.currentMorphTreeFile[:-4]+".swc")
+            # print("SWC file saved!")
+            self.showdialog(f"{self.currentMorphTreeFile[:-4]} saved!")
+            return
+        fileName = self.currentMorphTreeFile[:-4]
+        # for idx, ax in enumerate(fig.axes):
+        #     if idx >0:
+        #         fig.delaxes(ax)
+        pv = self.splitViewTab_morph.getParTreePars("Parameters")
+        pve = self.splitViewTab_morph.getParTreePars("Export")
+        DiameterScaling = pv["Parameters"][1]["Diameter scaling"][0]
+        rotateAngle = pv["Parameters"][1]["Rotate tree (degree)"][0]
+        step_size=pv['Parameters'][1]['Bin size (um)'][0]
+        smoothBins=pv['Parameters'][1]['Gaussian window size (num. bins)'][0]
+        smoothStandardDeviation=pv['Parameters'][1]['Std of Gaussian kernel (num. bins)'][0]
+        drawContour = pv["Figure options"][1]["Draw contour"][0]
+        axisVisible = pve["Export Morphology"][1]["Axis visible"][0]
+        if format!="emf":
+            ## recreate a new figure
+            matWin = MatplotView(size=(8,6))
+            fig = matWin.getFigure()
+            ax2D = fig.add_subplot(111)
+            fig.set_dpi(dpi)
+            ## Matplotlib figures use Points per inch (ppi) of 72
+            ## so we need to scale the diameter by the dpi
+            morphor_viewer.draw(
+                self.neuronMorph, mode="2d", realistic_diameters=True, fig=fig, ax=ax2D, alpha=1.0,
+                contour_on=drawContour, contour_color='g', contour_linewidth=0.2,rotationContour=rotateAngle,
+                neutriteColors = self.NeutriteColors, DiameterScaling=DiameterScaling*180/dpi
+            ) ##  need to scale the diameter by the dpi?
+            if not axisVisible:
+                ax2D.axis('off') ## turn off axis
+                ax2D.grid(False) ## turn off grid
+            # MATPLT.show()
+            fig.savefig(
+                fileName+ "." + format,
+                dpi=dpi,
+                format=format,
+                metadata=None,
+                bbox_inches='tight',
+                pad_inches=0.01,
+                facecolor="auto",
+                edgecolor="auto",
+                transparent=True,
+                backend=None,
+            )
+        else: 
+            draw_morphorlogy_emf(self.neuronMorph, fileName, unit='mm', rotationContour=rotateAngle,
+            DiameterScaling=DiameterScaling, neuriteColors=self.NeutriteColors, dpi=dpi)
+        self.showdialog(f"{fileName} saved!")
 
     def spike_detection_event(self, param, changes):
         from pathlib import Path
         for param, change, data in changes:
             childName = param.name()
             if childName == "Clear all tables":
                 self.splitViewTab_FP.tables["Sweep features"].clear()
                 self.splitViewTab_FP.tables["Spike features"].clear()
                 self.splitViewTab_FP.tables["Cell features"].clear()
-
-            if childName == "Save all tables":
+            elif childName == "line color":
+                if self.currentPulseTree.filetype == ".nwb":
+                    sel = self.currentPulseTree.selectedItems()[0]
+                    self.plt = []  ## plot handles
+                    self.plotItemList = []  ## collect all plot handles
+                    self.trace_view.clear()  ## refresh the layout
+                    self.plotSingleSeries_NWB(sel)
+            elif childName == "Save all tables":
                 seriesName = (
                     self.splitViewTab_FP.tables["Cell features"].item(0, 0).value
                 )
                 if self.spikeTableSavePath == "":
                     fileName = self.exportFile(
                         title="Save all tables with prefix",
                         defaultName=seriesName,
@@ -7094,15 +8066,32 @@
                         with open(fileName1, "w") as fd:
                             fd.write(
                                 self.splitViewTab_FP.tables[f].serialize(
                                     useSelection=False
                                 )
                             )
                     self.showdialog(f"{seriesName} saved!")
+            elif childName == "Aligned spike list":
+                if hasattr(self, "ephyFpObjectList") and len(self.ephyFpObjectList)>0:
+                    df = {}
+                    for ephyFpObject in self.ephyFpObjectList:
+                        eobj = self.ephyFpObjectList[ephyFpObject]
+                        eobj.alignSpikes()
+                        ## convert a dictionary with key as sweep number and value as a list of spike times
+                        ## to a dataframe with columns as sweep number and rows as spike times
+                        df[ephyFpObject] = eobj.spikeList
 
+                    fileName = self.exportFile(
+                            title="Save spike waveforms",
+                            defaultName="Aligned_spike_list.pickle",
+                            extension="Pickle files (*.pickle)",
+                        )
+                    if fileName != []:
+                        with open(fileName, "wb") as fd:
+                            pickle.dump(df, fd)
 def main(app):
     main = MainWindow(app)
     main.mainFrame.show() 
     sys.exit(app.exec_())
 
 if __name__ == "__main__":
     app = QtWidgets.QApplication(sys.argv)
```

### Comparing `Patchview-0.2.9/patchview/utilitis/AllMyParsHere.py` & `Patchview-0.3.0/patchview/utilitis/AllMyParsHere.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Aug 11 15:42:29 2020
 
 @author: mhu
 """
-
+import pyqtgraph as pg
 ## global setting in the file tab
 params = [
     {
         "name": "data preprocessing",
         "type": "group",
         "children": [
             {
@@ -36,24 +36,38 @@
                 "name": "minimal number of sweeps",
                 "type": "int",
                 "value": 3,
                 "limits": (1, 20),
                 "default": 3,
                 "step": 1,
             },
+            {
+                "name": "NWB sweep table grouping",
+                "type": "list",
+                "values": ["pvNWB", "dandiNWB","Generic"],
+                "value": "pvNWB",
+            },
         ],
     },
     {
         "name": "Basic parameters",
         "type": "group",
         "children": [
             {"name": "Root Directory", "type": "str", "value": "D:\Mhu\Projects"},
-            {"name": "Color map", "type": "colormap"},
+            {
+                "name": "Default figure DPI",
+                "type": "int",
+                "value": 150,
+                "limits": (100, 500),
+                "default": 150,
+                "step": 50,
+            },
         ],
     },
+    
     {
         "name": "Save/Restore parameters",
         "type": "group",
         "children": [
             {"name": "Save State", "type": "action"},
             {
                 "name": "Restore State",
@@ -167,14 +181,24 @@
                 "value": 0.05,
                 "limits": (0.02, 0.08),
                 "step": 0.01,
                 "default": 0.05,
                 "tip": "fraction of average upstroke for threshold calculation",
             },
             {
+    
+                "name": "start_latency (min=0.001;max=0.005)",
+                "type": "float",
+                "value": 0.001,
+                "limits": (0.001, 0.005),
+                "step": 0.001,
+                "default": 0.001,
+                "tip": "Mimimum time between stiumulus onset and trheshold crossing",
+            },
+            {
                 "name": "baseline_interval (min=0.05;max=0.15)",
                 "type": "float",
                 "value": 0.1,
                 "limits": (0.05, 0.15),
                 "step": 0.01,
                 "default": 0.1,
                 "siPrefix": True,
@@ -222,26 +246,36 @@
                 "name": "line width",
                 "type": "float",
                 "value": 1.5,
                 "limits": (0.5, 2.5),
                 "default": 1.5,
                 "step": 0.1,
             },
+            {"name": "line color", "type": "color", "value": "g"},
         ],
     },
     {
         "name": "Tables",
         "type": "group",
         "children": [
             {"name": "Reset table automatically", "type": "bool", "value": True},
             {"name": "Clear all tables", "type": "action"},
             {"name": "Save all tables", "type": "action"},
         ],
     },
+    {
+        "name": "Export",
+        "type": "group",
+        "children": [
+            {"name": "Aligned spike list", "type": "action"},
+
+        ],
+    },
 ]
+#self.ephyFpObjectList
 
 fp_analysis_spikeDetection_help = [
     {
         "name": "Spike detection parameters",
         "type": "group",
         "children": [
             {
@@ -920,28 +954,31 @@
                 "value": "Add more high quality events and try again",
             },
             {"name": "solution2", "type": "str", "value": "Try different parameters"},
         ],
     },
 ]
 
-Morphor_analysis = [
+Morphor_parameters = [
     {
-        "name": "Options",
+        "name": "Parameters",
         "type": "group",
+        "expanded": True,
         "children": [
             {
                 "name": "Scale bar length",
                 "type": "float",
                 "limits": (10, 50),
                 "value": 50,
                 "step": 5,
                 "default": 50,
                 "siPrefix": False,
             },
+            {"name": "Diameter scaling", "type": "float", "value": 2.0,
+                "limits": (0.5, 4.0), "step": 0.5, "default": 2.0, "siPrefix": False},
             {
                 "name": "Rotate tree (degree)",
                 "type": "float",
                 "limits": (-180, 180),
                 "value": 0,
                 "step": 5,
                 "default": 0,
@@ -979,83 +1016,133 @@
                 "type": "float",
                 "limits": (1, 30),
                 "value": 15,
                 "step": 5,
                 "default": 15,
                 "siPrefix": False,
             },
+
+            {"name": "Update cell names", "type": "action"},
+        ],
+    },
+    {
+        "name": "Figure options",
+        "type": "group",
+        "expanded": False,
+        "children": [
+            {"name": "Figure aesthetics", "type": "list",
+                "values": ["whitegrid", "darkgrid", "white", "dark", "ticks"],
+                "value": "whitegrid"},
+            {
+            "name": "Neutrites color",
+            "expanded": False,
+            "type": "group",
+            "children": [
+            {"name": "Basal dendrite", "type": "color", "value": "g"},
+            {"name": "Apical dendrite", "type": "color", "value": "m"},
+            {"name": "All dendrites", "type": "color", "value": "c"},
+            {"name": "Axon", "type": "color", "value": "gray"},
+            {"name": "All neurites", "type": "color", "value": "k"},
+            {"name": "Soma", "type": "color", "value": "r"},
+            ],
+            },
+            {"name": "Morphology only", "type": "bool", "value": True},
+            {"name": "Show title", "type": "bool", "value": False},
             {"name": "Use full range for density plot", "type": "bool", "value": True},
             {"name": "Show color bar for density plot", "type": "bool", "value": True},
+            {"name": "Show grid", "type": "bool", "value": True},
             {"name": "Show axis for density plot", "type": "bool", "value": True},
-            {"name": "Ignore diameters", "type": "bool", "value": False},
             {"name": "Draw contour", "type": "bool", "value": True},
-            {"name": "Update cell names", "type": "action"},
-        ],
-    },
+            {"name": "Color map", "type": "list", "values":["rocket","hot","copper","gnuplot","inferno","magma"], "value": "rocket"},
+            {"name": "Custom axis range", "type": "group", 'expanded':False, "children": 
+            [
+                {"name":'plane density', "type": "group",'expanded':False, "enabled":False, "children":[
+                    {'name': 'activate', 'type': 'bool', "enabled":False,'value': False},
+                    {"name": "X min", "type": "float", "value": -500},
+                    {"name": "X max", "type": "float", "value": 500},
+                    {"name": "Y min", "type": "float", "value": -1000},
+                    {"name": "Y max", "type": "float", "value": 1000},
+                ]},
+                {"name":'polar density', "type": "group",'expanded':False, "children":[
+                    {'name': 'activate', 'type': 'bool', 'value': False},
+                    {"name": "R max", "type": "float", "value": 500},
+                ]
+                },
+            ],
+            },
+        ]
+    }
+]
+
+Morphor_measurments = [
     {
-        "name": "Measurment",
+        "name": "Measurement",
         "type": "group",
+        "expanded": True,
         "children": [
             {"name": "Sholl analysis", "type": "action"},
+            {"name": "Dendrogram", "type": "action"},
             {"name": "X axis density", "type": "action"},
             {"name": "Y axis density", "type": "action"},
             {"name": "XY plane density", "type": "action"},
             {"name": "XY polar density", "type": "action"},
-            {"name": "Distance to Pia", "type": "action"},
-        ],
+            {"name": "Path length histogram", "type": "action"},
+            {"name": "Apical dendrite stem directionality histogram", "type": "action"},
+            {"name": "Persistent barcode", "type": "group",
+             "children": [
+                {"name": "Distance function", "type": "list",
+                 "values": ['radial_distance','height','path_length','branch_order'], 'value': 'radial_distance'},
+                {"name": "Compute barcode", "type": "action"},
+                ]
+            },
+            {"name": "Feature histograms", "type": "group",
+             "children": [
+                {"name": "Features", "type": "list",
+                 "values": ['branch_order', 'strahler_order', 
+                    'branch_angle', 'path_angle', 'root_angle', 
+                    'thickness', 'segment_length', 'path_length', 'radial_dist'],
+                  'value': 'radial_distance'},
+                {"name": "Make histogram", "type": "action"},
+                ]
+             },
+            {"name": "Distance to Pia", "type": "action"},    
+            {"name": "Close all floating windows", "type": "action"},
+        ]
     },
+]
+Morphor_export = [
     {
-        "name": "Save options",
+        "name": "Export Morphology",
         "type": "group",
+        "expanded": True,
         "children": [
             {
                 "name": "DPI",
                 "type": "float",
                 "limits": (100, 1000),
                 "value": 300,
                 "step": 50,
                 "default": 300,
                 "siPrefix": False,
             },
             {
-                "name": "Size",
-                "type": "int",
-                "limits": (10, 100),
-                "value": 60,
-                "step": 5,
-                "default": 60,
-                "siPrefix": False,
-            },
-            {
                 "name": "Format",
                 "type": "list",
-                "values": ["svg", "eps", "png"],
-                "value": "svg",
+                "values": ["emf", "svg","pdf", "eps", "png","swc"],
+                "value": "emf",
             },
+            {"name": "Axis visible", "type": "bool", "value": False},
             {"name": "Export High resolution figure", "type": "action"},
         ],
     },
-]
-
-Morphor_legend = [
-    {
-        "name": "Color scheme",
-        "type": "group",
-        "children": [
-            {"name": "Basal dendtrite", "type": "str", "value": "Purple"},
-            {"name": "Apical dendtrite", "type": "str", "value": "Blue"},
-            {"name": "Axon", "type": "str", "value": "Red"},
-            {"name": "Soma", "type": "str", "value": "Black"},
-        ],
-    },
     {
-        "name": "Help for options",
+        "name": "Export Morphology density",
         "type": "group",
+        "expanded": False,
         "children": [
-            {
-                "name": "ignore diamters",
-                "type": "str",
-                "value": "When set True, will render each section's diamter accordingly",
-            },
+            {"name": "linear projections", "type": "bool", "value": True},
+            {"name": "xy cartesian", "type": "bool", "value": True},
+            {"name": "xy polar", "type": "bool", "value": False, "enabled": False},
+            {"name": "Save to disk", "type": "action"},
         ],
     },
 ]
```

### Comparing `Patchview-0.2.9/patchview/utilitis/AnalysisMethods.py` & `Patchview-0.3.0/patchview/utilitis/AnalysisMethods.py`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/utilitis/fitFuncs.py` & `Patchview-0.3.0/patchview/utilitis/fitFuncs.py`

 * *Files identical despite different names*

### Comparing `Patchview-0.2.9/patchview/utilitis/patchviewObjects.py` & `Patchview-0.3.0/patchview/utilitis/patchviewObjects.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 """
 Created on Mon Dec 13 11:41:59 2021
 
 @author: MHu
 """
 from PyQt5 import QtWidgets, QtCore
 from PyQt5.QtWidgets import *
-# from PyQt5.QtWidgets import QSpinBox, QDoubleSpinBox, QGridLayout, QGroupBox, QFormLayout, QTabWidget, QTableWidget, QHeaderView
-# from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout, QSizePolicy, QScrollArea, QFrame, QSplitter, QToolButton, QMenu, QAction
 import pyqtgraph as pg
 from pyqtgraph import QtGui
 from pyqtgraph import GraphicsLayoutWidget
 from pyqtgraph.parametertree import Parameter, ParameterTree
 import os, glob
 import numpy as np
 import pandas as pd
@@ -30,15 +28,15 @@
 
         # hide system files
         self.setFilter(
             QtCore.QDir.AllDirs | QtCore.QDir.NoDotAndDotDot | QtCore.QDir.AllEntries
         )
 
         # filter out non dats and disable showing
-        self.setNameFilters(["*.dat", "*.abf","*.asc","*.ASC"])
+        self.setNameFilters(["*.dat", "*.abf","*.asc","*.ASC","*.nwb","*.swc"])
         self.setNameFilterDisables(False)
 
         # set root
         self.setRootPath(root_path)
 
 
 class sliceSelectionDialog(pg.QtWidgets.QWidget):
@@ -226,15 +224,15 @@
 
         # get file from index
         file_path = os.path.abspath(self.model.filePath(model_index))
         self.frame.root, f = os.path.split(file_path)
         #        os.chdir(self.frame.root)
         # check extension
         _, ext = os.path.splitext(file_path)
-        if ext in ['.asc','.ASC']:
+        if ext in ['.asc','.ASC','.swc']:
             self.frame.prepareTree(file_path)
         else:
             self.frame.clearAllTrees()
             self.frame.update_pul(file_path, dat_index=None, ext=ext)
 
 
 class SelectionView(pg.QtWidgets.QTreeWidget):
@@ -310,19 +308,19 @@
                 node_type += str(getattr(node, node_type + "Count"))
         except AttributeError:
             pass
 
         # self.setHeaderLabels(['Node', 'Label','dat', 'dat_Index'])
         # self.setHeaderLabels(['Cell label', 'File','Series', 'Index'])
         if len(index) == 1:
-            item = pg.QtGui.QTreeWidgetItem(
+            item = QTreeWidgetItem(
                 [node_type, node_dat, node_label, node_datIndex]
             )
         else:
-            item = pg.QtGui.QTreeWidgetItem(
+            item = QTreeWidgetItem(
                 [node_label, node_dat, node_type, node_datIndex]
             )
 
         item.setCheckState(0, QtCore.Qt.Checked)
         item.node = node
         item.index = index
         root_item.addChild(item)
@@ -597,17 +595,17 @@
             node_label = node.Label
         except AttributeError:
             if node_type[:5] == "Pulse":
                 node_label = self.bundle.header.Version
             else:
                 node_label = ""
         if node_type[:2] == "V9":
-            item = pg.QtGui.QTreeWidgetItem([node_type[3:], node_label])
+            item = QTreeWidgetItem([node_type[3:], node_label])
         else:
-            item = pg.QtGui.QTreeWidgetItem([node_type, node_label])
+            item = QTreeWidgetItem([node_type, node_label])
         if len(index) == 2:
             self.seriesNode.append(node)
 
         if dat_index == None:  ## update all
             root_item.addChild(item)
             item.node = node
             item.index = index
@@ -632,14 +630,76 @@
                 item.node = node
                 item.index = index
                 if len(index) < 2:
                     item.setExpanded(True)
                 for i in range(len(node.children)):
                     self.update_tree_recursive(item, index + [i], dat_index)
 
+    def update_withNWB_sweepTable(self, root_item, sessionIdx=0):
+        r = self.pvEphy # set pvNWB instance as root
+        nwb = r.nwbfile
+        self.filetype = ".nwb"
+        node = r
+        if node == None:
+            return
+        sessionNode = QTreeWidgetItem(['Recordings' , ''])
+        sessionNode.index = [sessionIdx] # We may add more than one session
+        sessionNode.setExpanded(True)
+        root_item.addChild(sessionNode)
+        swGrps = r.getSweepGroups() # dict with sweep name as key
+        for gidx, groupName in enumerate(swGrps): # sweep groups level
+            swGp = swGrps[groupName] # one sweep group
+            stim_type = swGp.get_stimulus_type(0)
+            grpNode = QTreeWidgetItem([groupName , stim_type+'. N='+str(len(swGp))])
+            grpNode.index = [sessionIdx, gidx]
+            grpNode.setExpanded(True)
+            sessionNode.addChild(grpNode)
+            for swp_name in swGp.sweepNames: # sweep level
+                swp = swGp[swp_name]
+                sweep_table_index = swp.sweep_table_index #; sweep group index
+                traceIdx = swp.trace_indexes # this is a list of sweep indices (int), last one is trace index
+                tracelabels = swp.trace_labels # this is a list of sweep indices (int)
+                sweepGrpNode = QTreeWidgetItem([swp.name, ''])
+                sweepGrpNode.index = [sessionIdx, gidx, sweep_table_index]
+                sweepGrpNode.setExpanded(True)
+                grpNode.addChild(sweepGrpNode)
+                for idx, s in enumerate(traceIdx):
+                    sweepNode = QTreeWidgetItem(['trace '+str(s+1), tracelabels[idx]])
+                    sweepNode.index = [sessionIdx, gidx, sweep_table_index, idx] ## the last index is the sweep index in the sweep table
+                    sweepGrpNode.addChild(sweepNode)
+
+    def update_withNWB_sweepTable_namedtuple(self, root_item):
+            """parse pvNWB's sweepGroups (a named tuple) and add items into the GUI tree to allow browsing.
+            """
+            r = self.pvEphy # set pvNWB instance as root
+            nwb = r.nwbfile
+            self.filetype = ".nwb"
+            node = r
+            if node == None:
+                return
+            swGrps = self.pvEphy.sweepGroups._fields # differnt data structure
+            for bidx, g in enumerate(swGrps):
+                g_children = getattr(self.pvEphy.sweepGroups, g) # sweep groups
+                if len(g_children) == 0:
+                    continue
+                grpNode = QTreeWidgetItem([g, str(len(g_children))])
+                grpNode.index = [bidx]
+                grpNode.setExpanded(True)
+                root_item.addChild(grpNode)
+                for swgIdx, swg_g in enumerate(g_children._fields): # sweep level
+                    sweepIdx = g_children[swgIdx] # this is a list of sweep indices (int)
+                    sweepGrpNode = QTreeWidgetItem([swg_g, 'N='+str(len(sweepIdx))])
+                    sweepGrpNode.index = [bidx, swgIdx]
+                    sweepGrpNode.setExpanded(True)
+                    grpNode.addChild(sweepGrpNode)
+                    for s in sweepIdx:
+                        sweepNode = QTreeWidgetItem(['Sweep '+ str(s),''])
+                        sweepNode.index = [bidx, swgIdx, s] ## the last index is the sweep index in the sweep table
+                        sweepGrpNode.addChild(sweepNode)
+ 
     def update_ABFtree(self, root_item):
         """read information from the Axon ABF file using neo.AxonIO interface
         and add items into the GUI tree to allow browsing.
         """
         r = self.abf  ## root
         self.filetype = ".abf"
         self.dat_file = self.frame.currentPulseTree.dat_file
@@ -658,29 +718,29 @@
         ## root level
         node_type = "ABF"
         node_label = (
             metaInfo["fFileSignature"].decode()
             + "_v"
             + str(metaInfo["fFileVersionNumber"])
         )  # abfVersion
-        abfNode = pg.QtGui.QTreeWidgetItem([node_type, node_label])
+        abfNode = QTreeWidgetItem([node_type, node_label])
         root_item.addChild(abfNode)
         root_item.setExpanded(True)
         abfNode.node = r
         abfNode.index = 0
 
         self.abfBlocks = r.read()  # read the entire file > a list of Blocks
         ## block level
         for b in range(nBlock):
-            block = pg.QtGui.QTreeWidgetItem(["Block", str(b + 1)])
+            block = QTreeWidgetItem(["Block", str(b + 1)])
             block.setExpanded(True)
             block.index = [0, b]
             abfNode.addChild(block)
             for seg in range(nSegments[b]):
-                segment = pg.QtGui.QTreeWidgetItem(["Sweep" + str(seg + 1), ""])
+                segment = QTreeWidgetItem(["Sweep" + str(seg + 1), ""])
                 segment.setExpanded(True)
                 segment.index = [0, b, seg]
                 block.addChild(segment)
         rawP = r.read_raw_protocol()
         stimChanIdx = 0  ## channel index where stimuli is applied to
         if len(rawP[0]) > 0:
             self.abf_stimOn = True
```

### Comparing `Patchview-0.2.9/setup.py` & `Patchview-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 #with open('requirements_dev.txt', 'r') as f:
 #    dev_requirements = [l for l in f.read().split('\n') if l.strip()]
 dev_requirements = [] 
 
 setup(
     author="Ming Hu",
-    author_email='',
+    author_email="hi@gmail.com",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Topic :: Scientific/Engineering :: Information Analysis',
@@ -46,25 +46,26 @@
         'Programming Language :: Python :: 3.10',
         "Operating System :: OS Independent",
     ],
     description="Patchview perform data analysis and visualization on whole-cell recording data, including firing pattern analysis, event analysis, synatpic connection detection, morphorlocial analysis and more.",
     install_requires=requirements,
     extras_require={'dev': dev_requirements},
     license="BSD-3-Clause",
-    long_description=readme + '\n\n' + history,
+    long_description_content_type="text/x-rst",
+    long_description=readme,
     include_package_data=True,
     keywords='patchview',
     name='patchview',
     packages=find_packages(include=['patchview','patchview/Data',\
         'patchview/HekaIO','patchview/utilitis']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zeitgeberH/patchview',
-    version = "0.2.9",
+    version = "0.3.0",
     zip_safe=False,
     entry_points={
         'gui_scripts': [
             'patchview=patchview:main'
         ],
     },
 )
```

