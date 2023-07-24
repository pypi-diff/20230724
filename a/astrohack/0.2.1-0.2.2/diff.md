# Comparing `tmp/astrohack-0.2.1.tar.gz` & `tmp/astrohack-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.2.1.tar", last modified: Fri Jul 21 19:54:23 2023, max compression
+gzip compressed data, was "astrohack-0.2.2.tar", last modified: Mon Jul 24 21:10:34 2023, max compression
```

## Comparing `astrohack-0.2.1.tar` & `astrohack-0.2.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 19:54:08.000000 astrohack-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:54:08.000000 astrohack-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 19:54:23.466200 astrohack-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-21 19:54:08.000000 astrohack-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:08.000000 astrohack-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-21 19:54:08.000000 astrohack-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:54:23.466200 astrohack-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.454200 astrohack-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.458200 astrohack-0.2.1/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dask_graph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5482 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_panel_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/_utils/_param_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_param_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_param_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_param_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_phase_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/_utils/_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.454200 astrohack-0.2.1/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.462200 astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    28650 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/extract_pointing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    42610 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/mds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.466200 astrohack-0.2.1/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-21 19:54:08.000000 astrohack-0.2.1/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:54:23.458200 astrohack-0.2.1/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 19:54:23.000000 astrohack-0.2.1/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.494420 astrohack-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 21:10:17.000000 astrohack-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:10:17.000000 astrohack-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-24 21:10:34.494420 astrohack-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-24 21:10:17.000000 astrohack-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:17.000000 astrohack-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-24 21:10:17.000000 astrohack-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:10:34.494420 astrohack-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.482419 astrohack-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.486420 astrohack-0.2.2/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_dask_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22280 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5482 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/_utils/_panel_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_panel_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_panel_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_panel_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_panel_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_panel_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/_utils/_param_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_param_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_param_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_param_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_phase_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.482419 astrohack-0.2.2/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.490420 astrohack-0.2.2/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.494420 astrohack-0.2.2/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.494420 astrohack-0.2.2/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.494420 astrohack-0.2.2/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.494420 astrohack-0.2.2/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/extract_pointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42566 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.494420 astrohack-0.2.2/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-24 21:10:17.000000 astrohack-0.2.2/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:34.486420 astrohack-0.2.2/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-24 21:10:34.000000 astrohack-0.2.2/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-24 21:10:34.000000 astrohack-0.2.2/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:10:34.000000 astrohack-0.2.2/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 21:10:34.000000 astrohack-0.2.2/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 21:10:34.000000 astrohack-0.2.2/src/astrohack.egg-info/top_level.txt
```

### Comparing `astrohack-0.2.1/LICENSE` & `astrohack-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/PKG-INFO` & `astrohack-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.2.1
+Version: 0.2.2
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.2.1/README.md` & `astrohack-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/pyproject.toml` & `astrohack-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.2.1"
+version = "0.2.2"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_algorithms.py` & `astrohack-0.2.2/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_combine.py` & `astrohack-0.2.2/src/astrohack/_utils/_combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_constants.py` & `astrohack-0.2.2/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_conversion.py` & `astrohack-0.2.2/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_dask_graph_tools.py` & `astrohack-0.2.2/src/astrohack/_utils/_dask_graph_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.2.2/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.2.2/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_diagnostics.py` & `astrohack-0.2.2/src/astrohack/_utils/_diagnostics.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_dio.py` & `astrohack-0.2.2/src/astrohack/_utils/_dio.py`

 * *Files 4% similar despite different names*

```diff
@@ -319,60 +319,32 @@
         if dask_load:
             return xr.open_zarr(image_path)
         else:
             return _open_no_dask_zarr(image_path)
     else:
         raise FileNotFoundError("Image file: {} not found".format(image_path))
 
-def _read_meta_data(file_name, file_type, origin):
+def _read_meta_data(file_name):
     """Reads dimensional data from holog meta file.
 
     Args:
         file_name (str): astorhack file name.
-        file_type (str): astrohack file type
-        origin (str, list): Astrohack expected origin(s)
 
     Returns:
         dict: dictionary containing dimension data.
     """
     logger = _get_astrohack_logger()
     
     try:
-        with open(f'{file_name}/.{file_type}_attr') as json_file:
+        with open(file_name) as json_file:
             json_dict = json.load(json_file)
 
     except Exception as error:
         logger.error(str(error))
-        raise Exception   
-    
-    # I don't see the use case for this or the origin in general. This means I need to either look at the
-    # meta data of a file I want to open ahead of time or list all possible unctions that could have made it.
-    
-    
-    try:
-        metadataorigin = json_dict['origin']
-    except KeyError:
-        logger.error("[_read_meta_data]: Badly formatted metadata in input file")
-        
-        raise Exception('Bad metadata')
-
-    if isinstance(origin, str):
-        if metadataorigin != origin:
-            logger.error(f"[_read_meta_data]: Input file is not an Astrohack {file_type} file")
-            logger.error(f"Expected origin was {origin} but got {metadataorigin}")
-            
-            raise TypeError('Incorrect file type')
-
-    elif isinstance(origin, (list, tuple)):
-        if metadataorigin not in origin:
-            logger.error(f"[_read_meta_data]: Input file is not an Astrohack {file_type} file")
-            logger.error(f"Expected origin was {origin} but got {metadataorigin}")
-            
-            raise TypeError('Incorrect file type')
-    
+        raise Exception       
 
     return json_dict
 
 
 def _check_mds_origin(file_name, file_type):
     """
```

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.2.2/src/astrohack/_utils/_extract_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_extract_point.py` & `astrohack-0.2.2/src/astrohack/_utils/_extract_point.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_gaussfitter.py` & `astrohack-0.2.2/src/astrohack/_utils/_gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_holog.py` & `astrohack-0.2.2/src/astrohack/_utils/_holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         holog_chunk_params["holog_name"],
         dask_load=False,
         load_pnt_dict=False,
         ant_id=holog_chunk_params["this_ant"],
         ddi_id=holog_chunk_params["this_ddi"]
     )
 
-    meta_data = _read_meta_data(holog_chunk_params["holog_name"], 'holog', 'extract_holog')
+    meta_data = _read_meta_data(holog_chunk_params["holog_name"]+'/.holog_attr')
 
     # Calculate lm coordinates
     l, m = _calc_coords(holog_chunk_params["grid_size"], holog_chunk_params["cell_size"])
     grid_l, grid_m = list(map(np.transpose, np.meshgrid(l, m)))
     
     to_stokes = holog_chunk_params["to_stokes"]
```

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_imaging.py` & `astrohack-0.2.2/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.2.2/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_panel.py` & `astrohack-0.2.2/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/antenna_surface.py` & `astrohack-0.2.2/src/astrohack/_utils/_panel_classes/antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/base_panel.py` & `astrohack-0.2.2/src/astrohack/_utils/_panel_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/polygon_panel.py` & `astrohack-0.2.2/src/astrohack/_utils/_panel_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/ring_panel.py` & `astrohack-0.2.2/src/astrohack/_utils/_panel_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_panel_classes/telescope.py` & `astrohack-0.2.2/src/astrohack/_utils/_panel_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_param_utils/_check_logger_parms.py` & `astrohack-0.2.2/src/astrohack/_utils/_param_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_param_utils/_check_parms.py` & `astrohack-0.2.2/src/astrohack/_utils/_param_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_phase_fitting.py` & `astrohack-0.2.2/src/astrohack/_utils/_phase_fitting.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/_utils/_tools.py` & `astrohack-0.2.2/src/astrohack/_utils/_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/astrohack_client.py` & `astrohack-0.2.2/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/combine.py` & `astrohack-0.2.2/src/astrohack/combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json` & `astrohack-0.2.2/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json` & `astrohack-0.2.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json` & `astrohack-0.2.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.2.2/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.2.2/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.2.2/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.2.2/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.2.2/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.2.2/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.2.2/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.2.2/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.2.2/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.2.2/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.2.2/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.2.2/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/dio.py` & `astrohack-0.2.2/src/astrohack/dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/extract_holog.py` & `astrohack-0.2.2/src/astrohack/extract_holog.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,15 +468,14 @@
 
 def generate_holog_obs_dict(
     ms_name,
     point_name=None,
     ddi='all',
     baseline_average_distance='all',
     baseline_average_nearest='all',
-    data_column="CORRECTED_DATA",
     overwrite=False,
     parallel=False
 ):
     """
     Extract holography and optionally pointing data, from measurement set. Creates holography output file.
 
     :param ms_name: Name of input measurement file name.
@@ -490,17 +489,14 @@
 
     :param baseline_average_nearest: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_nearest is the number of nearest reference antennas to use. The baseline_average_nearest is only used if the holog_obs_dict is not specified.  baseline_average_distance and baseline_average_nearest can not be used together.
     :type holog_obs_dict: int, optional
 
     :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
     :type point_name: str, optional
 
-    :param data_column: Determines the data column to pull from the measurement set. Defaults to "CORRECTED_DATA".
-    :type data_column: str, optional, ex. DATA, CORRECTED_DATA
-
     :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files, defaults to False.
     :type overwrite: bool, optional
 
     :param parallel: Boolean for whether to process in parallel. Defaults to False
     :type parallel: bool, optional
 
     :return: holog observation dictionary
```

### Comparing `astrohack-0.2.1/src/astrohack/extract_pointing.py` & `astrohack-0.2.2/src/astrohack/extract_pointing.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/gdown_utils.py` & `astrohack-0.2.2/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/holog.py` & `astrohack-0.2.2/src/astrohack/holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     _check_if_file_will_be_overwritten(holog_params['image_name'], holog_params['overwrite'])
 
     json_data = "/".join((holog_params['holog_name'], ".holog_json"))
 
     with open(json_data, "r") as json_file:
         holog_json = json.load(json_file)
         
-    meta_data = _read_meta_data(holog_params['holog_name'], 'holog', 'extract_holog')
+    meta_data = _read_meta_data(holog_params['holog_name']+'/.holog_attr')
 
     if holog_params["cell_size"] is None:
         cell_size = np.array([-meta_data["cell_size"], meta_data["cell_size"]])
         holog_params["cell_size"] = cell_size
     
     if holog_params["grid_size"] is None:
         n_pix = int(np.sqrt(meta_data["n_pix"]))
```

### Comparing `astrohack-0.2.1/src/astrohack/mds.py` & `astrohack-0.2.2/src/astrohack/mds.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
             self._file_is_open = True
 
         except Exception as e:
             logger.error("[AstroHackImageFile.open()]: {}".format(e))
             self._file_is_open = False
 
-        self._meta_data = _read_meta_data(file, 'image', ['combine', 'holog'])
+        self._meta_data = _read_meta_data(file+'/.image_attr')
 
         return self._file_is_open
 
     def summary(self):
         """ Prints summary of the AstrohackImageFile object, with available data, attributes and available methods
         """
         _print_summary_header(self.file)
@@ -394,15 +394,15 @@
             _load_holog_file(holog_file=file, dask_load=dask_load, load_pnt_dict=False, holog_dict=self)
             self._file_is_open = True
 
         except Exception as e:
             logger.error("[AstrohackHologFile]: {}".format(e))
             self._file_is_open = False
 
-        self._meta_data = _read_meta_data(file, 'holog', 'extract_holog')
+        self._meta_data = _read_meta_data(file+'/.holog_attr')
 
         return self._file_is_open
 
     def summary(self):
         """ Prints summary of the AstrohackHologFile object, with available data, attributes and available methods
         """
         _print_summary_header(self.file)
@@ -588,15 +588,15 @@
         try:
             _load_panel_file(file, panel_dict=self)
             self._file_is_open = True
         except Exception as e:
             logger.error("[AstroHackPanelFile.open()]: {}".format(e))
             self._file_is_open = False
 
-        self._meta_data = _read_meta_data(file, 'panel', 'panel')
+        self._meta_data = _read_meta_data(file+'/.panel_attr')
 
         return self._file_is_open
 
     def summary(self):
         """ Prints summary of the AstrohackPanelFile object, with available data, attributes and available methods
         """
         _print_summary_header(self.file)
@@ -860,15 +860,15 @@
             _load_point_file(file=file, dask_load=dask_load, pnt_dict=self)
             self._file_is_open = True
 
         except Exception as e:
             logger.error("[AstrohackPointFile]: {}".format(e))
             self._file_is_open = False
 
-        self._meta_data = _read_meta_data(file, 'point', 'extract_pointing')
+        self._meta_data = _read_meta_data(file+'/.point_attr')
 
         return self._file_is_open
 
     def summary(self):
         """ Prints summary of the AstrohackPointFile object, with available data, attributes and available methods
         """
         _print_summary_header(self.file)
```

### Comparing `astrohack-0.2.1/src/astrohack/panel.py` & `astrohack-0.2.2/src/astrohack/panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             panel_mds._open()
             return panel_mds
         else:
             logger.warning(f"[{fname}]: No data to process")
             return None
 
 
-def aips_holog_to_astrohack(amp_image, dev_image, telescope_name, holog_name, overwrite=False):
+def _aips_holog_to_astrohack(amp_image, dev_image, telescope_name, holog_name, overwrite=False):
     """
     Package AIPS HOLOG products in a .image.zarr file compatible with astrohack.panel.panel
 
     This function reads amplitude and deviation FITS files produced by AIPS's HOLOG task and transfers their data onto a
     .image.zarr file that can be read by panel.
     Most of the metadata can be inferred from the FITS headers, but it remains necessary to specify the telescope name
     to be included on the .image.zarr file
```

### Comparing `astrohack-0.2.1/src/astrohack/profiling.py` & `astrohack-0.2.2/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack/visualization/viewer.py` & `astrohack-0.2.2/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.2.1/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.2.2/src/astrohack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.2.1
+Version: 0.2.2
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.2.1/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.2.2/src/astrohack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

