# Comparing `tmp/agh_vqis-3.1.0.tar.gz` & `tmp/agh_vqis-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agh_vqis-3.1.0.tar", last modified: Mon Jul 17 00:46:03 2023, max compression
+gzip compressed data, was "agh_vqis-3.2.0.tar", last modified: Mon Jul 24 12:41:01 2023, max compression
```

## Comparing `agh_vqis-3.1.0.tar` & `agh_vqis-3.2.0.tar`

### file list

```diff
@@ -1,147 +1,149 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/
--rw-rw-rw-   0        0        0     2826 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/LICENSE
--rw-rw-rw-   0        0        0    13218 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    12210 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.184081 agh_vqis-3.1.0/agh_vqis.egg-info/
--rw-rw-rw-   0        0        0    13218 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8111 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-17 00:46:03.000000 agh_vqis-3.1.0/agh_vqis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.168754 agh_vqis-3.1.0/python-cpbd/
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.185292 agh_vqis-3.1.0/python-cpbd/cpbd/
--rw-rw-rw-   0        0        0       49 2023-07-16 23:41:56.000000 agh_vqis-3.1.0/python-cpbd/cpbd/__init__.py
--rw-rw-rw-   0        0        0     7670 2023-07-16 23:41:56.000000 agh_vqis-3.1.0/python-cpbd/cpbd/compute.py
--rw-rw-rw-   0        0        0     1540 2023-07-16 23:41:56.000000 agh_vqis-3.1.0/python-cpbd/cpbd/octave.py
--rw-rw-rw-   0        0        0     1329 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.168754 agh_vqis-3.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.191438 agh_vqis-3.1.0/src/agh_vqis/
--rw-rw-rw-   0        0        0      381 2023-07-17 00:45:08.000000 agh_vqis-3.1.0/src/agh_vqis/__init__.py
--rw-rw-rw-   0        0        0    22456 2023-07-17 00:20:36.000000 agh_vqis-3.1.0/src/agh_vqis/__main__.py
--rw-rw-rw-   0        0        0     1349 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.197525 agh_vqis-3.1.0/src/agh_vqis/binaries/
--rw-rw-rw-   0        0        0    97508 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
--rwxrwxrwx   0        0        0   122077 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
--rw-rw-rw-   0        0        0    66424 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
--rw-rw-rw-   0        0        0  2952245 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/binaries/cygwin1.dll
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.168754 agh_vqis-3.1.0/src/agh_vqis/models/
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/
--rw-rw-rw-   0        0        0    21075 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    21723 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    14595 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    15027 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    32379 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    35763 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    34035 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    29643 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
--rw-rw-rw-   0        0        0    33747 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
--rw-rw-rw-   0        0        0    28059 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
--rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
--rw-rw-rw-   0        0        0    33531 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
--rw-rw-rw-   0        0        0    29355 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
--rw-rw-rw-   0        0        0    26691 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
--rw-rw-rw-   0        0        0    31803 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
--rw-rw-rw-   0        0        0    30291 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
--rw-rw-rw-   0        0        0    30795 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
--rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    26907 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    38355 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
--rw-rw-rw-   0        0        0    39075 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
--rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
--rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
--rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38571 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
--rw-rw-rw-   0        0        0    39219 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
--rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
--rw-rw-rw-   0        0        0    37995 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
--rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    38643 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
--rw-rw-rw-   0        0        0    39363 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
--rw-rw-rw-   0        0        0    38067 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
--rw-rw-rw-   0        0        0    38211 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
--rw-rw-rw-   0        0        0    36915 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
--rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
--rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
--rw-rw-rw-   0        0        0    28779 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
--rw-rw-rw-   0        0        0    29715 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
--rw-rw-rw-   0        0        0    30219 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
--rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
--rw-rw-rw-   0        0        0    38283 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
--rw-rw-rw-   0        0        0    37563 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
--rw-rw-rw-   0        0        0    27843 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
--rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
--rw-rw-rw-   0        0        0    27699 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
--rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
--rw-rw-rw-   0        0        0    37275 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
--rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
--rw-rw-rw-   0        0        0    29283 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
--rw-rw-rw-   0        0        0    27483 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
--rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
--rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
--rw-rw-rw-   0        0        0    38139 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
--rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
--rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
--rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
--rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
--rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    17835 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    27411 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
--rw-rw-rw-   0        0        0    25179 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
--rw-rw-rw-   0        0        0    22659 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
--rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    17187 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    25395 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
--rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
--rw-rw-rw-   0        0        0    16827 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    23667 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
--rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
--rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
--rw-rw-rw-   0        0        0    22299 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
--rw-rw-rw-   0        0        0    22155 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
--rw-rw-rw-   0        0        0    19059 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
--rw-rw-rw-   0        0        0    18987 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
--rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
--rw-rw-rw-   0        0        0    23163 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
--rw-rw-rw-   0        0        0    22011 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
--rw-rw-rw-   0        0        0    20283 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
--rw-rw-rw-   0        0        0    18123 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
--rw-rw-rw-   0        0        0    22947 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
--rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
--rw-rw-rw-   0        0        0    22587 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
--rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
--rw-rw-rw-   0        0        0    21435 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
--rw-rw-rw-   0        0        0    18699 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
--rw-rw-rw-   0        0        0     4587 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
--rw-rw-rw-   0        0        0     5739 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
--rw-rw-rw-   0        0        0     6459 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
--rw-rw-rw-   0        0        0     5307 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
--rw-rw-rw-   0        0        0     5811 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
--rw-rw-rw-   0        0        0     4947 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
--rw-rw-rw-   0        0        0     5379 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
--rw-rw-rw-   0        0        0     5163 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
--rw-rw-rw-   0        0        0    40443 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
--rw-rw-rw-   0        0        0    43467 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
--rw-rw-rw-   0        0        0    39435 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
--rw-rw-rw-   0        0        0    42171 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
--rw-rw-rw-   0        0        0    38787 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
--rw-rw-rw-   0        0        0    42747 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
--rw-rw-rw-   0        0        0    39939 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
--rw-rw-rw-   0        0        0    41235 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
--rw-rw-rw-   0        0        0    38931 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
--rw-rw-rw-   0        0        0    40875 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
--rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/src/agh_vqis/models/ugc/
--rw-rw-rw-   0        0        0   594166 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/models/ugc/12k_all_set.json
-drwxrwxrwx   0        0        0        0 2023-07-17 00:46:03.870504 agh_vqis-3.1.0/src/agh_vqis/utils/
--rw-rw-rw-   0        0        0     6043 2023-07-17 00:34:17.000000 agh_vqis-3.1.0/src/agh_vqis/utils/helpers.py
--rw-rw-rw-   0        0        0      754 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/utils/resolution_cast.py
--rw-rw-rw-   0        0        0     5735 2023-07-16 23:33:06.000000 agh_vqis-3.1.0/src/agh_vqis/utils/ugc.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.552589 agh_vqis-3.2.0/
+-rw-rw-rw-   0        0        0     2826 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0    13218 2023-07-24 12:41:01.552589 agh_vqis-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12210 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.333032 agh_vqis-3.2.0/agh_vqis.egg-info/
+-rw-rw-rw-   0        0        0    13218 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8201 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 12:41:01.000000 agh_vqis-3.2.0/agh_vqis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.317397 agh_vqis-3.2.0/python-cpbd/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.333032 agh_vqis-3.2.0/python-cpbd/cpbd/
+-rw-rw-rw-   0        0        0       49 2023-07-16 23:41:56.000000 agh_vqis-3.2.0/python-cpbd/cpbd/__init__.py
+-rw-rw-rw-   0        0        0     7670 2023-07-16 23:41:56.000000 agh_vqis-3.2.0/python-cpbd/cpbd/compute.py
+-rw-rw-rw-   0        0        0     1540 2023-07-16 23:41:56.000000 agh_vqis-3.2.0/python-cpbd/cpbd/octave.py
+-rw-rw-rw-   0        0        0     1329 2023-07-24 12:41:01.552589 agh_vqis-3.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.317397 agh_vqis-3.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.333032 agh_vqis-3.2.0/src/agh_vqis/
+-rw-rw-rw-   0        0        0      381 2023-07-24 12:37:50.000000 agh_vqis-3.2.0/src/agh_vqis/__init__.py
+-rw-rw-rw-   0        0        0    22941 2023-07-24 12:24:21.000000 agh_vqis-3.2.0/src/agh_vqis/__main__.py
+-rw-rw-rw-   0        0        0     1349 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.348658 agh_vqis-3.2.0/src/agh_vqis/binaries/
+-rw-rw-rw-   0        0        0    60648 2023-07-24 11:09:44.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_linux_aarch64_mt
+-rw-rw-rw-   0        0        0    66424 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_linux_x86_64_mt
+-rw-rw-rw-   0        0        0    97508 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_macosx_arm64_mt
+-rw-rw-rw-   0        0        0    88328 2023-07-21 14:04:46.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_macosx_x86_64_mt
+-rwxrwxrwx   0        0        0   122077 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_win64_mt.exe
+-rw-rw-rw-   0        0        0  2952245 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/binaries/cygwin1.dll
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.317397 agh_vqis-3.2.0/src/agh_vqis/models/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.536963 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/
+-rw-rw-rw-   0        0        0    21075 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    21723 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    14595 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    15027 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    32379 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    35763 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    34323 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    34035 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    29643 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb
+-rw-rw-rw-   0        0        0    33747 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb
+-rw-rw-rw-   0        0        0    28059 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb
+-rw-rw-rw-   0        0        0    33531 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb
+-rw-rw-rw-   0        0        0    29355 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb
+-rw-rw-rw-   0        0        0    26691 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb
+-rw-rw-rw-   0        0        0    31803 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    30291 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb
+-rw-rw-rw-   0        0        0    30795 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    26907 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    38355 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb
+-rw-rw-rw-   0        0        0    39075 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    37059 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38571 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb
+-rw-rw-rw-   0        0        0    39219 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    37995 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    27339 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    38643 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb
+-rw-rw-rw-   0        0        0    39363 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb
+-rw-rw-rw-   0        0        0    38067 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb
+-rw-rw-rw-   0        0        0    38211 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    36915 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb
+-rw-rw-rw-   0        0        0    28779 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb
+-rw-rw-rw-   0        0        0    29715 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb
+-rw-rw-rw-   0        0        0    30219 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    38283 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb
+-rw-rw-rw-   0        0        0    37563 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb
+-rw-rw-rw-   0        0        0    27843 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb
+-rw-rw-rw-   0        0        0    27267 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb
+-rw-rw-rw-   0        0        0    27699 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb
+-rw-rw-rw-   0        0        0    37635 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    37275 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    37851 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb
+-rw-rw-rw-   0        0        0    29283 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb
+-rw-rw-rw-   0        0        0    27483 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb
+-rw-rw-rw-   0        0        0    26979 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37347 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    38139 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    37779 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    29787 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb
+-rw-rw-rw-   0        0        0    27195 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    17835 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    27411 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb
+-rw-rw-rw-   0        0        0    25179 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb
+-rw-rw-rw-   0        0        0    22659 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb
+-rw-rw-rw-   0        0        0    17259 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    17187 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    25395 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb
+-rw-rw-rw-   0        0        0    16827 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    23667 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb
+-rw-rw-rw-   0        0        0    19491 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb
+-rw-rw-rw-   0        0        0    22299 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb
+-rw-rw-rw-   0        0        0    22155 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb
+-rw-rw-rw-   0        0        0    19059 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb
+-rw-rw-rw-   0        0        0    18987 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb
+-rw-rw-rw-   0        0        0    20571 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb
+-rw-rw-rw-   0        0        0    23163 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb
+-rw-rw-rw-   0        0        0    22011 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb
+-rw-rw-rw-   0        0        0    20283 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb
+-rw-rw-rw-   0        0        0    18123 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb
+-rw-rw-rw-   0        0        0    22947 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb
+-rw-rw-rw-   0        0        0    22803 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb
+-rw-rw-rw-   0        0        0    22587 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb
+-rw-rw-rw-   0        0        0    23955 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb
+-rw-rw-rw-   0        0        0    21435 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb
+-rw-rw-rw-   0        0        0    18699 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb
+-rw-rw-rw-   0        0        0     4587 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0     5739 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb
+-rw-rw-rw-   0        0        0     6459 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb
+-rw-rw-rw-   0        0        0     5307 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb
+-rw-rw-rw-   0        0        0     5811 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb
+-rw-rw-rw-   0        0        0     4947 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb
+-rw-rw-rw-   0        0        0     5379 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb
+-rw-rw-rw-   0        0        0     5163 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb
+-rw-rw-rw-   0        0        0    40443 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb
+-rw-rw-rw-   0        0        0    43467 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb
+-rw-rw-rw-   0        0        0    39435 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb
+-rw-rw-rw-   0        0        0    42171 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb
+-rw-rw-rw-   0        0        0    38787 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb
+-rw-rw-rw-   0        0        0    42747 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb
+-rw-rw-rw-   0        0        0    39939 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb
+-rw-rw-rw-   0        0        0    41235 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb
+-rw-rw-rw-   0        0        0    38931 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb
+-rw-rw-rw-   0        0        0    40875 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb
+-rw-rw-rw-   0        0        0    37923 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.536963 agh_vqis-3.2.0/src/agh_vqis/models/ugc/
+-rw-rw-rw-   0        0        0   594166 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/models/ugc/12k_all_set.json
+drwxrwxrwx   0        0        0        0 2023-07-24 12:41:01.552589 agh_vqis-3.2.0/src/agh_vqis/utils/
+-rw-rw-rw-   0        0        0     6317 2023-07-24 12:34:08.000000 agh_vqis-3.2.0/src/agh_vqis/utils/helpers.py
+-rw-rw-rw-   0        0        0      754 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/utils/resolution_cast.py
+-rw-rw-rw-   0        0        0     5735 2023-07-16 23:33:06.000000 agh_vqis-3.2.0/src/agh_vqis/utils/ugc.py
```

### Comparing `agh_vqis-3.1.0/LICENSE` & `agh_vqis-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/PKG-INFO` & `agh_vqis-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agh_vqis
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Python wrapper for 18 image quality indicators.
 Home-page: https://qoe.agh.edu.pl/indicators/
 Author: Filip Korus, Jakub Nawała
 Author-email: fkorus@student.agh.edu.pl, jakub.nawala@agh.edu.pl
 License: EVALUATION LICENSE AGREEMENT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `agh_vqis-3.1.0/README.md` & `agh_vqis-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/agh_vqis.egg-info/PKG-INFO` & `agh_vqis-3.2.0/agh_vqis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agh-vqis
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Python wrapper for 18 image quality indicators.
 Home-page: https://qoe.agh.edu.pl/indicators/
 Author: Filip Korus, Jakub Nawała
 Author-email: fkorus@student.agh.edu.pl, jakub.nawala@agh.edu.pl
 License: EVALUATION LICENSE AGREEMENT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `agh_vqis-3.1.0/agh_vqis.egg-info/SOURCES.txt` & `agh_vqis-3.2.0/agh_vqis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 agh_vqis.egg-info/top_level.txt
 python-cpbd/cpbd/__init__.py
 python-cpbd/cpbd/compute.py
 python-cpbd/cpbd/octave.py
 src/agh_vqis/__init__.py
 src/agh_vqis/__main__.py
 src/agh_vqis/_logger.py
-src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
-src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
-src/agh_vqis/binaries/agh_vqis_binary_x86_mt
+src/agh_vqis/binaries/agh_vqis_linux_aarch64_mt
+src/agh_vqis/binaries/agh_vqis_linux_x86_64_mt
+src/agh_vqis/binaries/agh_vqis_macosx_arm64_mt
+src/agh_vqis/binaries/agh_vqis_macosx_x86_64_mt
+src/agh_vqis/binaries/agh_vqis_win64_mt.exe
 src/agh_vqis/binaries/cygwin1.dll
 src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb
 src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb
 src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb
 src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb
 src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb
 src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb
```

### Comparing `agh_vqis-3.1.0/python-cpbd/cpbd/compute.py` & `agh_vqis-3.2.0/python-cpbd/cpbd/compute.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/python-cpbd/cpbd/octave.py` & `agh_vqis-3.2.0/python-cpbd/cpbd/octave.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/setup.cfg` & `agh_vqis-3.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6768 5f76 7169 730d 0a76 6572   = agh_vqis..ver
-00000020: 7369 6f6e 203d 2033 2e31 2e30 0d0a 6175  sion = 3.1.0..au
+00000020: 7369 6f6e 203d 2033 2e32 2e30 0d0a 6175  sion = 3.2.0..au
 00000030: 7468 6f72 203d 2046 696c 6970 204b 6f72  thor = Filip Kor
 00000040: 7573 2c20 4a61 6b75 6220 4e61 7761 c582  us, Jakub Nawa..
 00000050: 610d 0a61 7574 686f 725f 656d 6169 6c20  a..author_email 
 00000060: 3d20 666b 6f72 7573 4073 7475 6465 6e74  = fkorus@student
 00000070: 2e61 6768 2e65 6475 2e70 6c2c 206a 616b  .agh.edu.pl, jak
 00000080: 7562 2e6e 6177 616c 6140 6167 682e 6564  ub.nawala@agh.ed
 00000090: 752e 706c 0d0a 6465 7363 7269 7074 696f  u.pl..descriptio
```

### Comparing `agh_vqis-3.1.0/src/agh_vqis/__main__.py` & `agh_vqis-3.2.0/src/agh_vqis/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Authors: Jakub Nawała <jnawala@agh.edu.pl>, Filip Korus <fkorus@student.agh.edu.pl>
 # Created: June 1, 2021
 
 import argparse
 import logging
+import platform
 
 import numpy as np
 import pims
 from cpbd.compute import compute
 from pims import PyAVVideoReader
 
 from ._logger import setup_console_and_file_logger
@@ -28,19 +29,28 @@
     :param vqis_binary: path to agh_vqis binary file (optional)
     :param selected_vqis: a positive 16-bit integer stating which VQIs to run (all are run by default)
     :return: Pandas DataFrame with VQIs results or -1 if an error occurred
     """
 
     if vqis_binary is None:
         executable_file = get_executable_filename()
+
+        if executable_file is None:
+            logger.error(f'Your platform ({platform.system()} - {platform.machine()}) is not supported. Exiting.')
+            return -1
+
         binary_path = Path(str(get_current_file_location()), 'binaries/', executable_file)
     else:
         binary_path = Path(vqis_binary)
         logger.info(f'Using {binary_path.resolve()} binary file')
 
+    if not binary_path.resolve().exists():
+        logger.error(f'{str(binary_path.resolve())} file does not exist')
+        return -1
+
     if not os.access(binary_path.resolve(), os.X_OK):
         logger.error(f'{str(binary_path.resolve())} file is not executable')
         return -1
 
     logger.debug('Creating working directory')
     random_folder_name = generate_uuid()
     mkdir(random_folder_name)
@@ -324,24 +334,24 @@
     if options is None:
         options = {}
 
     if args is None:
         args = parse_user_input(cli)
 
     if not is_ffmpeg_installed():
-        logger.error(f'ffmpeg is not installed or an executable command')
+        logger.error(f'ffmpeg is not installed or an executable command. Exiting.')
         return -1
 
     if not in_path.exists():
-        logger.error(f'{str(in_path)} file does not exists')
+        logger.error(f'{str(in_path)} file does not exists. Exiting.')
         return -1
 
     mm_file_ext = in_path.suffix
     if mm_file_ext not in allowed_mm_file_extensions:
-        logger.error(f'{mm_file_ext} file extension is not supported')
+        logger.error(f'{mm_file_ext} file extension is not supported. Exiting.')
         return -1
 
     # Read properties of an input multimedia file
     in_mm_file_w, in_mm_file_h, nb_frames, frame_rate = get_mm_file_properties(in_path)
     is_input_video = True  # a flag making further processing logic easier to comprehend
     if nb_frames == 0:
         is_input_video = False
@@ -402,15 +412,15 @@
                            f"{np.abs(len(vqis_res_df) - int(nb_frames))}")
 
     if run_ugc_iqi:
         logger.info(f"Running the UGC IQI on the input ({str(in_path.resolve())})")
 
         ugc_s = get_ugc_vqi(in_path, int(nb_frames), vqis_res_df)
         if ugc_s is None:
-            logger.error(f"Error when running UGC IQI")
+            logger.error(f"Error when running UGC IQI. Skipping.")
         else:
             ugc_s.name = "UGC"
             results.update({Results.UGC: ugc_s})
 
     if vqis_res_df is not None:
         results.update({Results.VQIS: vqis_res_df})
 
@@ -478,15 +488,17 @@
     # TODO Implement user input processing interface that allows to choose individual VQIs from the 15 AGH VQIs in a
     #  user-friendly manner
     args = parse_user_input(True)
 
     in_path = args.path
     in_path = in_path.resolve()
     if not in_path.exists():
-        raise FileNotFoundError(f"The path you specified ({in_path}) does not exist. Exiting.")
+        # raise FileNotFoundError(f"The path you specified ({in_path}) does not exist. Exiting.")
+        logger.error(f'The path you specified ({in_path}) does not exist. Exiting.')
+        return -1
 
     if in_path.is_dir():
         logger.info(f"Processing a folder ({str(in_path)}) potentially containing a set of multimedia materials")
         status = process_folder_w_mm_files(in_path, cli=True, options={}, args=args)
     else:
         in_mm_file_path = in_path  # mm = multimedia
         status = process_single_mm_file(in_mm_file_path, cli=True, options={}, args=args)
```

### Comparing `agh_vqis-3.1.0/src/agh_vqis/_logger.py` & `agh_vqis-3.2.0/src/agh_vqis/_logger.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt` & `agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_macosx_arm64_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe` & `agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_win64_mt.exe`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/binaries/agh_vqis_binary_x86_mt` & `agh_vqis-3.2.0/src/agh_vqis/binaries/agh_vqis_linux_x86_64_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/binaries/cygwin1.dll` & `agh_vqis-3.2.0/src/agh_vqis/binaries/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blockiness_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Blur_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Contrast_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1080p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_1440p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_2160p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_240p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_360p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Exposure(bri)_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Interlace_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1080p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_1080p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_1440p_2160p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_2160p_1440p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_240p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_240p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_360p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_360p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_480p_720p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb` & `agh_vqis-3.2.0/src/agh_vqis/models/resolution_cast/model_Noise_720p_480p.xgb`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/models/ugc/12k_all_set.json` & `agh_vqis-3.2.0/src/agh_vqis/models/ugc/12k_all_set.json`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/utils/helpers.py` & `agh_vqis-3.2.0/src/agh_vqis/utils/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,27 +58,35 @@
     BLUR_AMOUNT = 1
     COLOURFULNESS = 2
     UGC = 3
     VQIS = 4
 
 
 def get_executable_filename():
-    switcher = {
-        'Windows':  'agh_vqis_binary_win64_mt.exe',
-        'Linux':    'agh_vqis_binary_x86_mt',
-        'Darwin':   'agh_vqis_binary_macosx_mt'
+    available_executables = {
+        'Windows AMD64': 'agh_vqis_win64_mt.exe',
+        'Windows x86_64': 'agh_vqis_win64_mt.exe',
+
+        'Linux aarch64': 'agh_vqis_linux_aarch64_mt',
+        'Linux x86_64': 'agh_vqis_linux_x86_64_mt',
+
+        'Darwin arm64': 'agh_vqis_macosx_arm64_mt',
+        'Darwin x86_64': 'agh_vqis_macosx_x86_64_mt'
     }
 
-    os_type = platform.system()
+    os_type, machine = platform.system(), platform.machine()
 
-    return switcher.get(os_type, None)
+    return available_executables \
+        .get(f'{os_type} {machine}', None)
 
 
 def get_current_file_location() -> Path:
-    return Path('/'.join(__file__.split('/')[:-1]) if platform.system() != 'Windows' else '\\'.join(__file__.split('\\')[:-1]), '../')
+    return Path(
+        '/'.join(__file__.split('/')[:-1]) if platform.system() != 'Windows' else '\\'.join(__file__.split('\\')[:-1]),
+        '../')
 
 
 def get_mm_file_properties(video_path: Path):
     """
     Returns multimedia file properties.
 
     :param video_path: path to a video or image file
```

### Comparing `agh_vqis-3.1.0/src/agh_vqis/utils/resolution_cast.py` & `agh_vqis-3.2.0/src/agh_vqis/utils/resolution_cast.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-3.1.0/src/agh_vqis/utils/ugc.py` & `agh_vqis-3.2.0/src/agh_vqis/utils/ugc.py`

 * *Files identical despite different names*

