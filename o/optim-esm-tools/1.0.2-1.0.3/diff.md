# Comparing `tmp/optim_esm_tools-1.0.2.tar.gz` & `tmp/optim_esm_tools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-1.0.2.tar", last modified: Thu Jul 20 14:32:53 2023, max compression
+gzip compressed data, was "optim_esm_tools-1.0.3.tar", last modified: Mon Jul 24 17:24:20 2023, max compression
```

## Comparing `optim_esm_tools-1.0.2.tar` & `optim_esm_tools-1.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.081616 optim_esm_tools-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-20 14:32:53.085616 optim_esm_tools-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.069616 optim_esm_tools-1.0.2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/bin/oet_plot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.069616 optim_esm_tools-1.0.2/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.077616 optim_esm_tools-1.0.2/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    27831 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/tipping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/analyze/xarray_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/optim_esm_conf.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.077616 optim_esm_tools-1.0.2/optim_esm_tools/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/plotting/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.077616 optim_esm_tools-1.0.2/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.073616 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-20 14:32:53.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 14:32:52.000000 optim_esm_tools-1.0.2/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-20 14:32:53.085616 optim_esm_tools-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:32:53.081616 optim_esm_tools-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_pangeo_download.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 14:32:47.000000 optim_esm_tools-1.0.2/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.972620 optim_esm_tools-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-07-24 17:24:20.972620 optim_esm_tools-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.964620 optim_esm_tools-1.0.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/bin/oet_plot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.964620 optim_esm_tools-1.0.3/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.968620 optim_esm_tools-1.0.3/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/analyze/xarray_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/optim_esm_conf.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.968620 optim_esm_tools-1.0.3/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.968620 optim_esm_tools-1.0.3/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.968620 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 17:24:20.000000 optim_esm_tools-1.0.3/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 17:24:20.972620 optim_esm_tools-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:24:20.972620 optim_esm_tools-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-24 17:24:14.000000 optim_esm_tools-1.0.3/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-1.0.2/PKG-INFO` & `optim_esm_tools-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim_esm_tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,23 +15,35 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
-        1.0.1 / 2023-07-20
+        1.0.3 / 2023-07-24
+        ------------------
+        * Fix clustering fudge factor by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/91
+        * Preprocessing running mean fix by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/92
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.2...v1.0.3
+        
+        
+        1.0.2 / 2023-07-20
         ------------------
         * fix /0 by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/89
         * Cache region maps by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/90
-        * Clusting bugs by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/88
+        * Clustering bugs by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/88
         
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.0...v1.0.1
         
+        1.0.1 / 2023-07-20
+        ------------------
+        *Dummy release*
         
         1.0.0 / 2023-07-18
         ------------------
         **major change**
         * Harmonize preprocessing with `cdo` by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/81
         
         **minor changes**
@@ -96,22 +108,22 @@
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.1.1...v0.2.1
         
         0.2.0 / 2023-06-21
         ------------------
         ## What's Changed
         * Refactor code - next release by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/46
         * Add new file tools by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/48
-        * Add timeing decorator by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/49
+        * Add timing decorator by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/49
         * Clustering improvements by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/50
         * Add download routine from pangeo store by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/51
         * Add more timed functions by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/52
         * Split `read_ds` by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/53
         * stop double test by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/54
-        * Condition and results as propper classes by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/55
-        * Add config for timeing tool by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/56
+        * Condition and results as proper classes by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/55
+        * Add config for timing tool by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/56
         * Add minimal install test by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/57
         * Add region finder by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/58
         * Fix labels by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/59
         * Fix issue with labelling by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/60
         * Configuration tweaks by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/61
```

### Comparing `optim_esm_tools-1.0.2/README.md` & `optim_esm_tools-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/bin/oet_plot` & `optim_esm_tools-1.0.3/bin/oet_plot`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(err_file, 'a') as f:
         f.write(mm)
     import optim_esm_tools as oet
     oet.config.get_logger().error(message)
 
 
 def parse_args():
-    parser = argparse.ArgumentParser( description='make plots')
+    parser = argparse.ArgumentParser(description='make plots')
     parser.add_argument('--path', type=str,)
     parser.add_argument('--methods', nargs='*', default='Percentiles ProductPercentiles LocalHistory'.split(), type=list,)
     parser.add_argument('--variable', type=str,)
     parser.add_argument('--save_in', type=str,)
     parser.add_argument('--err_file', type=str, default='errors.txt',)
     parser.add_argument('--show', action='store_true')
     parser.add_argument('--profile_memory', action='store_true')
@@ -24,20 +24,22 @@
     parser.add_argument('--read_ds_kw', default='{}', type=json.loads, )
     args = parser.parse_args()
     return args
 
 def make_plot(variable, log, path, save_in, show, read_ds_kw, extra_opt, methods):
     save_kw = dict( save_in = save_in, sub_dir = None, file_types=('png', #'pdf'
                                                                    ), skip= False, )
-    from optim_esm_tools.utils import setup_plt
+    from optim_esm_tools.utils import setup_plt, print_versions
+    print_versions()
+    setup_plt()
     import optim_esm_tools.analyze.region_finding
     from optim_esm_tools.analyze.pre_process import NoDataInTimeRangeError
-    setup_plt()
     constructors = [getattr(optim_esm_tools.analyze.region_finding, meth, 'not found') for meth in methods]
-    if any(c=='not found' for c in constructors): raise ValueError(f'One or more non-existing methods {methods}')
+    if any(c=='not found' for c in constructors):
+        raise ValueError(f'One or more non-existing methods {methods}')
 
     from optim_esm_tools.analyze.cmip_handler import read_ds
 
     log.info('Read path')
     read_ds_kw=read_ds_kw if read_ds_kw is not None else dict()
     ds = read_ds(path, **read_ds_kw)
     kw = dict(data_set=ds, variable=variable, path=None, read_ds_kw=read_ds_kw)
@@ -51,15 +53,15 @@
                 log.warning(f'No results for {result.__class__.__name__} - masks are empty')
                 continue
         except (NoDataInTimeRangeError, NotImplementedError, RuntimeError):
              log.error(f'No match, not making {result.__class__.__name__}')
              continue
         except ValueError as e:
             if 'moving average window' in str(e):
-                log.error(f'ValueError for {result.__class__.__name__} as the dataset is too short. Probably in LocalHistory and unharmfull.')
+                log.error(f'ValueError for {result.__class__.__name__} as the dataset is too short. Probably in LocalHistory and unharmful.')
                 continue
             raise e
         result.show=show
         log.warning(f'{result.__class__.__name__}')
         result.workflow()
 
     log.warning('All done')
@@ -77,15 +79,15 @@
                   path=args.path,
                   save_in=args.save_in,
                   show=args.show,
                   read_ds_kw=args.read_ds_kw,
                   extra_opt=args.extra_opt,
                   methods=args.methods,
                   )
-    except ValueError as e:
+    except Exception as e:
         write_error(args.err_file, f'{args.path} | {e}')
         raise e
 
 if __name__ == '__main__':
     args = parse_args()
     if args.profile_memory:
         from memory_profiler import memory_usage
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/_test_utils.py` & `optim_esm_tools-1.0.3/optim_esm_tools/_test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/analyze/clustering.py` & `optim_esm_tools-1.0.3/optim_esm_tools/analyze/clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import numpy as np
 from optim_esm_tools.utils import tqdm, timed
-from optim_esm_tools.config import get_logger
+from optim_esm_tools.config import get_logger, config
 import typing as ty
-from warnings import warn
 import numba
 from math import sin, cos, sqrt, atan2, radians
 import xarray as xr
 
 
 @timed()
 def build_clusters(
     coordinates_deg: np.ndarray,
     weights: ty.Optional[np.ndarray] = None,
     max_distance_km: ty.Union[float, int] = 750,
     only_core: bool = True,
-    min_samples: int = 10,
+    min_samples: int = int(config['analyze']['clustering_min_neighbors']),
     cluster_opts: ty.Optional[dict] = None,
 ) -> ty.List[np.ndarray]:
-    """Build clusters based on a list of coordinates, use halfsine metric for spherical spatiol data
+    """Build clusters based on a list of coordinates, use halfsine metric for spherical spatial data
 
     Args:
         coordinates_deg (np.ndarray): set of xy coordinates in degrees
         weights (ty.Optional[np.ndarray], optional): weights (in the range [0,1]) corresponding to each coordinate
         max_distance_km (ty.Union[float, int], optional): max distance to other points to consider part of
             cluster (see DBSCAN(eps=<..>)). Defaults to 750.
         only_core (bool, optional): Use only core samples. Defaults to True.
-        min_samples (int): Minimum number of samples in cluster. Defaults to 20.
+        min_samples (int): Minimum number of samples in cluster. Defaults to 8.
         cluster_opts (ty.Optional[dict], optional): Additional options passed to sklearn.cluster.DBSCAN. Defaults to None.
 
     Returns:
         ty.List[np.ndarray]: list of clustered points (in radians)
     """
     cluster_opts = cluster_opts or dict()
     for class_label, v in dict(algorithm='ball_tree', metric='haversine').items():
@@ -83,31 +82,31 @@
     global_mask: np.ndarray,
     lat_coord: np.array,
     lon_coord: np.array,
     show_tqdm: bool = False,
     max_distance_km: ty.Union[str, float, int] = 'infer',
     **kw,
 ) -> ty.Tuple[ty.List[np.ndarray], ty.List[np.ndarray]]:
-    """Build set of clusters and masks based on the global mask, basically a utility wrapper arround build_clusters'
+    """Build set of clusters and masks based on the global mask, basically a utility wrapper around build_clusters'
 
     Args:
         global_mask (np.ndarray): full 2d mask of the data
         lon_coord (np.array): all longitude values
         lat_coord (np.array): all latitude values
-        show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
+        show_tqdm (bool, optional): use verbose progressbar. Defaults to False.
         max_distance_km (ty.Union[str, float, int]): find an appropriate distance
             threshold for build_clusters' max_distance_km argument. If nothing is
             provided, make a guess based on the distance between grid cells.
             Defaults to 'infer'.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
     if max_distance_km == 'infer':
-        max_distance_km = _infer_max_step_size(lat_coord, lon_coord)
+        max_distance_km = infer_max_step_size(lat_coord, lon_coord)
     lat, lon = _check_input(
         global_mask,
         lat_coord,
         lon_coord,
     )
     xy_data = np.array([lat[global_mask], lon[global_mask]])
 
@@ -143,22 +142,22 @@
         weights (np.ndarray): normalized score data (values in [0,1])
         lon_coord (np.array): all longitude values
         lat_coord (np.array): all latitude values
         max_distance_km (ty.Union[str, float, int]): find an appropriate distance
             threshold for build_clusters' max_distance_km argument. If nothing is
             provided, make a guess based on the distance between grid cells.
             Defaults to 'infer'.
-        show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
+        show_tqdm (bool, optional): use verbose progressbar. Defaults to False.
         threshold: float, min value of the passed weights. Defaults to 0.99.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
     if max_distance_km == 'infer':
-        max_distance_km = _infer_max_step_size(lat_coord, lon_coord)
+        max_distance_km = infer_max_step_size(lat_coord, lon_coord)
 
     lat, lon = _check_input(weights, lat_coord, lon_coord)
     xy_data = np.array([lat.flatten(), lon.flatten()])
 
     flat_weights = weights.flatten()
     mask = flat_weights > threshold
     masks, clusters = _build_cluster_with_kw(
@@ -171,15 +170,15 @@
         **kw,
     )
 
     return masks, clusters
 
 
 def _check_input(data, lat_coord, lon_coord):
-    """Check for consistancy and if we need to convert the lon/lat coordinates to a meshgrid"""
+    """Check for consistency and if we need to convert the lon/lat coordinates to a meshgrid"""
     if len(lon_coord.shape) <= 1:
         lon, lat = np.meshgrid(lon_coord, lat_coord)
     else:
         # In an older version, this would have been the default.
         lat, lon = lat_coord, lon_coord
 
     if data.shape != lon.shape or data.shape != lat.shape:
@@ -203,28 +202,54 @@
             mask_x = np.isclose(lon, coord_lon)
             mask_y = np.isclose(lat, coord_lat)
             mask |= mask_x & mask_y
         masks.append(mask)
     return masks, clusters
 
 
-def _infer_max_step_size(lat, lon, off_by_factor=1.1):
+def infer_max_step_size(
+    lat: np.ndarray, lon: np.ndarray, off_by_factor: float = None
+) -> float:
+    """
+    Infer the max. distance between two points to be considered as belonging to the same cluster.
+
+    There are two methods implemented, preferably, the lon, lat values are 1d-arrays, which can be
+    interpreted as a regular grid. If this is the case, calculate the distance for each point to
+    it's neighbors (also diagonally). Then, the max distance for the clustering can be taken as
+    the max. distance to any of the neighboring points.
+
+    Empirically, we found that this distance is not enough, and an additional fudge factor is
+    taken into account from version v1.0.3 onwards, this is taken to be sqrt(2). This is probably
+    not a coincidence, but it's not really clear where it's coming from.
+    """
+    if off_by_factor is None:
+        off_by_factor = float(config['analyze']['clustering_fudge_factor'])
     if len(lat.shape) == 1:
-        return np.max(calculate_distance_map(lat, lon)) * off_by_factor
-    lat = lat[lat > 0]
+        return off_by_factor * np.max(calculate_distance_map(lat, lon))
+
+    get_logger().info(
+        '(Irregular) grid, max_step_size based on first points above equator'
+    )
+    # We have to get two points from the potentially irregular grid and guess the distance from
+    # that. This is not as reliable as calculating this for a regular grid.
+
+    equator_idx = np.argmin(np.abs(np.mean(lat, axis=1)) - 90)
+    lon_0 = lon[0]
     coords = [
-        [[lat[0], lon[0]], [lat[0], lon[1]]],
-        [[lat[0], lon[0]], [lat[1], lon[0]]],
+        [[lat[equator_idx][0], lon_0[0]], [lat[equator_idx][0], lon_0[1]]],
+        [[lat[equator_idx][0], lon_0[0]], [lat[equator_idx + 1][0], lon_0[0]]],
+        [[lat[equator_idx][0], lon_0[0]], [lat[equator_idx + 1][0], lon_0[1]]],
     ]
-    # Return 2x the distance between grid cells
-    return 2 * max(_distance(c) for c in coords)
+    # assert False, coords
+    # Return the distance between grid cells * off_by_factor
+    return off_by_factor * max(_distance(c) for c in coords)
 
 
 def calculate_distance_map(lat, lon):
-    """For each point in a spanned lat lon grid, calculate the distance to the neighbouring points"""
+    """For each point in a spanned lat lon grid, calculate the distance to the neighboring points"""
     if isinstance(lat, xr.DataArray):
         lat = lat.values
         lon = lon.values
     return _calculate_distance_map(lat, lon)
 
 
 @numba.njit
@@ -232,29 +257,29 @@
     n_lat = len(lat)
     n_lon = len(lon)
     distances = np.zeros((n_lat, n_lon))
 
     shift_by_index = np.array(
         [(-1, 0), (1, 0), (0, -1), (0, 1), (-1, -1), (1, 1), (1, -1), (-1, 1)]
     )
-    neighbourgs = np.zeros(len(shift_by_index), dtype=np.float64)
+    neighbors = np.zeros(len(shift_by_index), dtype=np.float64)
     for lon_i in range(n_lon):
         for lat_i in range(n_lat):
-            neighbourgs[:] = 0
+            neighbors[:] = 0
             current = (lat[lat_i], lon[lon_i])
             for i, (x, y) in enumerate(shift_by_index):
                 alt_lon = np.mod(lon_i + x, n_lon)
                 alt_lat = lat_i + y
                 if alt_lat == n_lat or alt_lat < 0:
                     continue
                 alt_coord = (lat[alt_lat], lon[alt_lon])
                 if alt_coord == current:
                     continue
-                neighbourgs[i] = _distance_bf_coord(*current, *alt_coord)
-            distances[lat_i][lon_i] = np.max(neighbourgs)
+                neighbors[i] = _distance_bf_coord(*current, *alt_coord)
+            distances[lat_i][lon_i] = np.max(neighbors)
     return distances
 
 
 def _distance(coords, force_math=False):
     """Wrapper for if geopy is not installed"""
     if not force_math:
         try:
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-1.0.3/optim_esm_tools/analyze/cmip_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import os
 import xarray as xr
 
 import typing as ty
 from warnings import warn
 
-from .globals import _FOLDER_FMT
+from .globals import _FOLDER_FMT, _DEFAULT_MAX_TIME
 import optim_esm_tools as oet
 from optim_esm_tools.analyze import tipping_criteria
 
 
 def add_conditions_to_ds(
     ds: xr.Dataset,
     calculate_conditions: ty.Tuple[tipping_criteria._Condition] = None,
@@ -17,24 +17,26 @@
     variable_of_interest: ty.Tuple[str] = ('tas',),
     _ma_window: int = None,
 ) -> xr.Dataset:
     """Transform the dataset to get it ready for handling in optim_esm_tools
 
     Args:
         ds (xr.Dataset): input dataset
-        calculate_conditions (ty.Tuple[tipping_criteria._Condition], optional): Calculate the results of these tipping conditions. Defaults to None.
-        condition_kwargs (ty.Mapping, optional): kwargs for the tipping conditions. Defaults to None.
+        calculate_conditions (ty.Tuple[tipping_criteria._Condition], optional): Calculate the
+            results of these tipping conditions. Defaults to None.
+        condition_kwargs (ty.Mapping, optional): kwargs for the tipping conditions. Defaults to
+            None.
         variable_of_interest (ty.Tuple[str], optional): Variables to handle. Defaults to ('tas',).
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
 
     Raises:
         ValueError: If there are multiple tipping conditions with the same short_description
 
     Returns:
-        xr.Dataset: The fully initiallized dataset
+        xr.Dataset: The fully initialized dataset
     """
     _ma_window = _ma_window or oet.config.config['analyze']['moving_average_years']
     if calculate_conditions is None:
         calculate_conditions = (
             tipping_criteria.StartEndDifference,
             tipping_criteria.StdDetrended,
             tipping_criteria.MaxJump,
@@ -64,43 +66,48 @@
 
 
 @oet.utils.add_load_kw
 @oet.utils.timed()
 def read_ds(
     base: str,
     variable_of_interest: ty.Tuple[str] = None,
-    max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
+    max_time: ty.Optional[ty.Tuple[int, int, int]] = _DEFAULT_MAX_TIME,
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
     apply_transform: bool = True,
     pre_process: bool = True,
     strict: bool = True,
-    load: bool = False,
+    load: bool = None,
     _ma_window: ty.Optional[int] = None,
     _cache: bool = True,
     _file_name: str = None,
     **kwargs,
 ) -> xr.Dataset:
     """Read a dataset from a folder called "base".
 
     Args:
         base (str): Folder to load the data from
         variable_of_interest (ty.Tuple[str], optional): Variables to handle. Defaults to ('tas',).
-        max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to (2100, 1, 1).
-        min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to None.
-        apply_transform: (bool, optional): Apply analysis specific postprocessing algoritms. Defaults to True.
-        pre_process (bool, optional): Should be true, this pre-processing of the data is required later on. Defaults to True.
-        area_query_kwargs (ty.Mapping, optional): additionall keyword arguments for searching.
+        max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to
+            load data. Defaults to (2100, 12, 31).
+        min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to
+            load data. Defaults to None.
+        apply_transform: (bool, optional): Apply analysis specific postprocessing algorithms.
+            Defaults to True.
+        pre_process (bool, optional): Should be true, this pre-processing of the data is required
+            later on. Defaults to True.
+        area_query_kwargs (ty.Mapping, optional): additionally keyword arguments for searching.
         strict (bool, optional): raise errors on loading, if any. Defaults to True.
         load (bool, optional): apply dataset.load to dataset directly. Defaults to False.
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
-        _cache (bool, optional): cache the dataset with it's extra fields to alow faster (re)loading. Defaults to True.
+        _cache (bool, optional): cache the dataset with it's extra fields to alow faster
+            (re)loading. Defaults to True.
         _file_name (str, optional): name to match. Defaults to configs settings.
 
     kwargs:
-        any kwargs are passed onto transfor_ds.
+        any kwargs are passed onto transform_ds.
 
     Returns:
         xr.Dataset: An xarray dataset with the appropriate variables
     """
     log = oet.config.get_logger()
     _file_name = _file_name or oet.config.config['CMIP_files']['base_name']
     _ma_window = _ma_window or oet.config.config['analyze']['moving_average_years']
@@ -145,16 +152,19 @@
             min_time=min_time,
             save_as=temp_file,
             _ma_window=_ma_window,
             variable_id=variable_of_interest,
         )
     else:
         log.warning(
-            f'Not preprocessing file is dangerous, dimentions may differ wildly!'
+            f'Not preprocessing file is dangerous, dimensions may differ wildly!'
         )
+    # At this point, if load is None, change it to true, we will have to load it anyway to do the
+    # transforms
+    load = load if load is not None else True
     data_set = oet.analyze.io.load_glob(data_path, load=load)
 
     if os.path.exists(temp_file):
         # Maybe we can make this optional, but, for now, let's prevent double caching of
         # res_file and temp_file
         os.remove(temp_file)
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/analyze/find_matches.py` & `optim_esm_tools-1.0.3/optim_esm_tools/analyze/find_matches.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,22 +56,22 @@
         required_file (str, optional): Filename to match. Defaults to 'merged.nc'.
 
     Returns:
         list: of matches corresponding to the query
     """
     if grid is not None:
         get_logger().warning(
-            f'grid argument for find_matches is depricated, use grid_label'
+            f'grid argument for find_matches is deprecated, use grid_label'
         )
         grid_label = grid
     if max_versions is None:
         max_versions = int(9e9)
     if max_members is None:
         max_members = int(9e9)
-    variantes = sorted(
+    variants = sorted(
         glob.glob(
             os.path.join(
                 base,
                 activity_id,
                 institution_id,
                 source_id,
                 experiment_id,
@@ -81,15 +81,15 @@
                 grid_label,
                 version,
             )
         ),
         key=_variant_label_id_and_version,
     )
     seen = dict()
-    for candidate in variantes:
+    for candidate in variants:
         folders = candidate.split(os.sep)
         group = folders[-7]
         member = folders[-5]
         version = folders[-1]
 
         if group not in seen:
             seen[group] = defaultdict(list)
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/analyze/io.py` & `optim_esm_tools-1.0.3/optim_esm_tools/analyze/io.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/analyze/pre_process.py` & `optim_esm_tools-1.0.3/optim_esm_tools/analyze/pre_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from optim_esm_tools.utils import timed
 from optim_esm_tools.config import config, get_logger
 from optim_esm_tools.analyze.xarray_tools import _native_date_fmt
 from optim_esm_tools.analyze.io import load_glob
+from optim_esm_tools.analyze.globals import _DEFAULT_MAX_TIME
+import numpy as np
 import os
 import typing as ty
 
 
 @timed
 def pre_process(
     source: str,
     target_grid: str = None,
-    max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
+    max_time: ty.Optional[ty.Tuple[int, int, int]] = _DEFAULT_MAX_TIME,
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
     save_as: str = None,
     clean_up: bool = True,
     _ma_window: int = None,
     variable_id: str = None,
 ) -> str:
     """Apply several preprocessing steps to the file located at <source>:
@@ -22,17 +24,20 @@
       - regrid to simple grid
       - calculate corresponding area
       - calculate running mean, detrended and not-detrended
       - merge all files into one
 
     Args:
         source (str): path of file to parse
-        target_grid (str, optional): Grid specification (like n64, n90 etc.). Defaults to None and is taken from config.
-        max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to (2100, 1, 1).
-        min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to None.
+        target_grid (str, optional): Grid specification (like n64, n90 etc.). Defaults to None and
+            is taken from config.
+        max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to
+            load data. Defaults to (2100, 12, 30).
+        min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to
+            load data. Defaults to None.
         save_as (str, optional): path where to store the pre-processed folder. Defaults to None.
         clean_up (bool, optional): delete intermediate files. Defaults to True.
         _ma_window (int, optional): moving average window (assumed 10 years). Defaults to None.
         variable_id (str, optional): Name of the variable of interest. Defaults to None.
 
     Raises:
         ValueError: If source and dest are the same, we'll run into problems
@@ -40,15 +45,15 @@
     Returns:
         str: path of the dest file (same provided, if any)
     """
     import cdo
 
     _remove_bad_vars(source)
     variable_id = variable_id or _read_variable_id(source)
-    max_time = max_time or (9999, 1, 1)  # unreasonably far away
+    max_time = max_time or (9999, 12, 30)  # unreasonably far away
     min_time = min_time or (0, 1, 1)  # unreasonably long ago
     target_grid = target_grid or config['analyze']['regrid_to']
     _ma_window = _ma_window or config['analyze']['moving_average_years']
     _check_time_range(source, max_time, min_time, _ma_window)
 
     cdo_int = cdo.Cdo()
     head, _ = os.path.split(source)
@@ -86,16 +91,22 @@
     cdo_int.gridarea(input=f_regrid, output=f_area)
 
     cdo_int.detrend(input=f_regrid, output=f_tmp)
     cdo_int.chname(f'{var},{var_det}', input=f_tmp, output=f_det)
     os.remove(f_tmp)
 
     cdo_int.runmean(_ma_window, input=f_regrid, output=f_tmp)
-
-    cdo_int.chname(f'{var},{var_rm}', input=f_tmp, output=f_rm)
+    _run_mean_patch(
+        f_start=f_regrid,
+        f_rm=f_tmp,
+        f_out=f_rm,
+        ma_window=_ma_window,
+        var_name=var,
+        var_rm_name=var_rm,
+    )
     os.remove(f_tmp)
 
     cdo_int.detrend(input=f_rm, output=f_tmp)
     cdo_int.chname(f'{var_rm},{var_det_rm}', input=f_tmp, output=f_det_rm)
     # remove in cleanup
     cdo_int.merge(
         input=' '.join([f_regrid, f_det, f_det_rm, f_rm, f_area]), output=save_as
@@ -134,14 +145,40 @@
         # CF time does not always support year 0
         time_mask &= times > _native_date_fmt(times, min_time)
     if time_mask.sum() < float(ma_window):
         message = f'Data from {path} has {time_mask.sum()} time stamps in [{min_time}, {max_time}]'
         raise NoDataInTimeRangeError(message)
 
 
+def _run_mean_patch(f_start, f_rm, f_out, ma_window, var_name, var_rm_name):
+    """
+    Patch running mean file, since cdo decreases the length of the file by the ma_window, merging
+    two files of different durations results in bad data.
+
+    As a solution, we take the original file (f_start) and use it's shape (like the number of
+    timestamps) and fill those timestamps where the value of the running mean is defined.
+    Everything else is set to zero.
+    """
+    ds_base = load_glob(f_start)
+    ds_rm = load_glob(f_rm)
+    ds_out = ds_base.copy()
+
+    # Replace timestamps with the CDO computed running mean
+    data = np.zeros(ds_base[var_name].shape, ds_base[var_name].dtype)
+    data[:] = np.nan
+    ma_window = int(ma_window)
+    data[ma_window // 2 : 1 - ma_window // 2] = ds_rm[var_name].values
+    ds_out[var_name].data = data
+
+    # Patch variables and save
+    ds_out = ds_out.rename({var_name: var_rm_name})
+    ds_out.attrs = ds_rm.attrs
+    ds_out.to_netcdf(f_out)
+
+
 class NoDataInTimeRangeError(Exception):
     pass
 
 
 def _fmt_date(date: tuple) -> str:
     assert len(date) == 3
     y, m, d = date
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/analyze/region_finding.py` & `optim_esm_tools-1.0.3/optim_esm_tools/analyze/region_finding.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     func_by_drop = {True: _drop_by_mask, False: _mask_xr_ds}[drop]
     data_set = func_by_drop(data_set, masked_dims, ds_start, da_mask)
     data_set = data_set.assign_attrs(ds_start.attrs)
     return data_set
 
 
 def _drop_by_mask(data_set, masked_dims, ds_start, da_mask):
-    """Drop values with masked_dims dimentions.
+    """Drop values with masked_dims dimensions.
     Unfortunately, data_set.where(da_mask, drop=True) sometimes leads to bad results,
     for example for time_bnds (time, bnds) being dropped by (lon, lat). So we have to do
-    some funny bookkeeping of which datavars we can drop with data_set.where.
+    some funny bookkeeping of which data vars we can drop with data_set.where.
     """
 
     dropped = []
     for k, data_array in data_set.data_vars.items():
         if not all(dim in list(data_array.dims) for dim in masked_dims):
             dropped += [k]
 
@@ -64,15 +64,15 @@
     # Restore ignored variables and attributes
     for k in dropped:
         data_set[k] = ds_start[k]
     return data_set
 
 
 def _mask_xr_ds(data_set, masked_dims, ds_start, da_mask):
-    """Rebuild data_set for each variabled that has all masked_dims"""
+    """Rebuild data_set for each variable that has all masked_dims"""
     for k, data_array in data_set.data_vars.items():
         if all(dim in list(data_array.dims) for dim in masked_dims):
             # First dim is time?
             if (
                 'time' == data_array.dims[0] and data_array.shape[1:] == da_mask.T.shape
             ) or data_array.shape == da_mask.T.shape:
                 raise ValueError(f'Please make "{k}" lat, lon, now "{data_array.dims}"')
@@ -253,15 +253,16 @@
     def store_mask(self, mask, m_i, store_masks=True):
         if not store_masks:
             return
         save_in = self.save_kw['save_in']
         store_in_dir = os.path.join(save_in, 'masks')
         os.makedirs(store_in_dir, exist_ok=True)
         # Mask twice, "mask" is a np.ndarray, whereas ds.where needs a xr.DataArray.
-        # While we could make this more efficient (and only use the second step), the first step does only take ~10 ms
+        # While we could make this more efficient (and only use the second step), the first step
+        # does only take ~10 ms
         ds_masked = mask_xr_ds(self.data_set.copy(), mask)
         ds_masked = mask_xr_ds(ds_masked, ~ds_masked['cell_area'].isnull(), drop=True)
         ds_masked.to_netcdf(
             os.path.join(
                 store_in_dir,
                 f'{self.title_label}_cluster-{m_i}_v{_CMIP_HANDLER_VERSION}.nc',
             )
@@ -276,15 +277,15 @@
             if np.sum(mask) == 0:
                 continue
             self.summarize_mask(mask, m_i)
 
 
 class MaxRegion(RegionExtractor):
     def get_masks(self) -> dict:
-        """Get mask for max of ii and iii and a box arround that"""
+        """Get mask for max of ii and iii and a box around that"""
 
         def _val(label):
             return self.data_set[label].values
 
         def _max(label):
             return _val(label)[~np.isnan(_val(label))].max()
 
@@ -647,16 +648,14 @@
     def find_historical(
         self,
         match_to='piControl',
         look_back_extra=0,
         query_updates=None,
         search_kw=None,
     ):
-        from optim_esm_tools.config import config
-
         base = base_from_path(
             self.data_set.attrs['path'], look_back_extra=look_back_extra
         )
 
         search = oet.analyze.find_matches.folder_to_dict(self.data_set.attrs['path'])
         search['activity_id'] = 'CMIP'
         if search['experiment_id'] == match_to:
@@ -697,15 +696,15 @@
     labels = ('ii', 'iii', 'v')
 
     @oet.utils.check_accepts(
         accepts=immutabledict.immutabledict(cluster_method=('weighted', 'masked'))
     )
     @apply_options
     def get_masks(self, cluster_method='masked') -> dict:
-        """Get mask for max of ii and iii and a box arround that"""
+        """Get mask for max of ii and iii and a box around that"""
         if cluster_method == 'weighted':
             masks, clusters = self._get_masks_weighted()
         else:
             masks, clusters = self._get_masks_masked()
         if len(masks):
             self.check_shape(masks[0])
         return masks, clusters
@@ -729,15 +728,15 @@
         )
         return masks, clusters
 
     @apply_options
     def _get_masks_masked(
         self, product_percentiles=_two_sigma_percent, lon_lat_dim=('lon', 'lat')
     ) -> dict:
-        """Get mask for max of ii and iii and a box arround that"""
+        """Get mask for max of ii and iii and a box around that"""
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         ds = self.data_set.copy()
         combined_score = np.ones_like(ds[labels[0]].values)
         for label in labels:
             combined_score *= rank2d(ds[label].values)
@@ -768,15 +767,15 @@
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         for lab in labels:
             arr = self.data_set[lab].values
             arr_historical = historical_ds[lab].values
 
-            # If arr_historical is 0, the devision is going to get a nan assigned,
+            # If arr_historical is 0, the division is going to get a nan assigned,
             # despite this being the most interesting region (no historical
             # changes, only in the scenario's)!
             mask_no_std = arr_historical == 0
             mask_divide = np.zeros_like(mask_no_std)
             mask_divide[~mask_no_std] = (
                 arr[~mask_no_std] / arr_historical[~mask_no_std] > n_times_historical
             )
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/analyze/tipping_criteria.py` & `optim_esm_tools-1.0.3/optim_esm_tools/analyze/tipping_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,16 @@
         variable (str, optional): . Defaults to 'tas'.
         time_var (str, optional): . Defaults to 'time'.
         naming (str, optional): . Defaults to '{variable}_run_mean_{running_mean}'.
         running_mean (int, optional): . Defaults to 10.
         rename_to (str, optional): . Defaults to 'long_name'.
         unit (str, optional): . Defaults to 'absolute'.
         apply_abs (bool, optional): . Defaults to True.
-        _t_0_date (ty.Optional[tuple], optional): . Defaults to (2015, 1, 1).
-        _t_1_date (ty.Optional[tuple], optional): . Defaults to (2100, 1, 1).
+        _t_0_date (ty.Optional[tuple], optional): . Defaults to None.
+        _t_1_date (ty.Optional[tuple], optional): . Defaults to None.
 
     Raises:
         ValueError: when no timestamps are not none?
 
     Returns:
         xr.Dataset:
     """
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/analyze/xarray_tools.py` & `optim_esm_tools-1.0.3/optim_esm_tools/analyze/xarray_tools.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/config.py` & `optim_esm_tools-1.0.3/optim_esm_tools/config.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/optim_esm_conf.ini` & `optim_esm_tools-1.0.3/optim_esm_tools/optim_esm_conf.ini`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [constants]
 # 365.25 * 24 * 3600
 seconds_to_year = 31557600
 
 
 [versions]
-cmip_handler = 0.4.2
+cmip_handler = 0.4.4
 
 
 [display]
 progress_bar = True
 
 
 [analyze]
@@ -18,14 +18,23 @@
 moving_average_years = 10
 lon_lat_dim = lon,lat
 
 # If any of these names are in the dataset, remove them as they break pre-processing and are calculated for the regridded file anyway
 remove_vars = area cell_area GEOLON GEOLAT
 cartopy_projection = PlateCarree
 
+# In the clustering method, assume points closer than clustering_fudge_factor * max_distance belong
+# to the same cluster. See analyze.clustering._infer_max_step_size for more information
+clustering_fudge_factor = 1.1
+clustering_min_neighbors = 8
+
+# Split data sets on this year for nominal analyses
+max_time=2100 12 30
+
+
 [CMIP_files]
 folder_fmt = activity_id institution_id source_id experiment_id variant_label domain variable_id grid_label version
 base_name = merged.nc
 temp_file_name = temp_pre.nc
 
 excluded =
         ; # This one only has a dataset which is 5 years long, rendering it quite useless for 10yr running means
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/plotting/map_maker.py` & `optim_esm_tools-1.0.3/optim_esm_tools/plotting/map_maker.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/plotting/plot.py` & `optim_esm_tools-1.0.3/optim_esm_tools/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-1.0.3/optim_esm_tools/synda_files/synda_files.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools/utils.py` & `optim_esm_tools-1.0.3/optim_esm_tools/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             res = fn(*args, **kwargs)
             dt = time.time() - t0
             if dt > seconds:
                 hours = '' if dt < 3600 else f' ({dt/3600:{_fmt}} h) '
                 message = (
                     f'{fn.__name__} took {dt:{_fmt}} s{hours} (for '
                     f'{_chopped_string(args, _args_max)}, '
-                    f'{_chopped_string(kwargs,_args_max)})'
+                    f'{_chopped_string(kwargs, _args_max)})'
                 ).replace('\n', ' ')
                 if _report == 'print':
                     print(message)
                 else:
                     from .config import get_logger
 
                     getattr(get_logger(), _report)(message)
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-1.0.3/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim-esm-tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,23 +15,35 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
-        1.0.1 / 2023-07-20
+        1.0.3 / 2023-07-24
+        ------------------
+        * Fix clustering fudge factor by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/91
+        * Preprocessing running mean fix by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/92
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.2...v1.0.3
+        
+        
+        1.0.2 / 2023-07-20
         ------------------
         * fix /0 by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/89
         * Cache region maps by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/90
-        * Clusting bugs by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/88
+        * Clustering bugs by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/88
         
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v1.0.0...v1.0.1
         
+        1.0.1 / 2023-07-20
+        ------------------
+        *Dummy release*
         
         1.0.0 / 2023-07-18
         ------------------
         **major change**
         * Harmonize preprocessing with `cdo` by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/81
         
         **minor changes**
@@ -96,22 +108,22 @@
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.1.1...v0.2.1
         
         0.2.0 / 2023-06-21
         ------------------
         ## What's Changed
         * Refactor code - next release by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/46
         * Add new file tools by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/48
-        * Add timeing decorator by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/49
+        * Add timing decorator by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/49
         * Clustering improvements by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/50
         * Add download routine from pangeo store by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/51
         * Add more timed functions by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/52
         * Split `read_ds` by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/53
         * stop double test by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/54
-        * Condition and results as propper classes by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/55
-        * Add config for timeing tool by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/56
+        * Condition and results as proper classes by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/55
+        * Add config for timing tool by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/56
         * Add minimal install test by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/57
         * Add region finder by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/58
         * Fix labels by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/59
         * Fix issue with labelling by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/60
         * Configuration tweaks by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/61
```

### Comparing `optim_esm_tools-1.0.2/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-1.0.3/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/setup.py` & `optim_esm_tools-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='1.0.2',
+    version='1.0.3',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages(),
     package_dir={
```

### Comparing `optim_esm_tools-1.0.2/test/test_find_matches.py` & `optim_esm_tools-1.0.3/test/test_find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/test/test_region_finding.py` & `optim_esm_tools-1.0.3/test/test_region_finding.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/test/test_utils.py` & `optim_esm_tools-1.0.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/test/test_viewer.py` & `optim_esm_tools-1.0.3/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/test/test_workflow.py` & `optim_esm_tools-1.0.3/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-1.0.2/test/test_xarray_tools.py` & `optim_esm_tools-1.0.3/test/test_xarray_tools.py`

 * *Files identical despite different names*

