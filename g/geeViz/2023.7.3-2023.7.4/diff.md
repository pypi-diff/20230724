# Comparing `tmp/geeViz-2023.7.3.tar.gz` & `tmp/geeViz-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geeViz-2023.7.3.tar", last modified: Mon Jul 24 21:19:47 2023, max compression
+gzip compressed data, was "geeViz-2023.7.4.tar", last modified: Mon Jul 24 21:31:26 2023, max compression
```

## Comparing `geeViz-2023.7.3.tar` & `geeViz-2023.7.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 21:19:47.429401 geeViz-2023.7.3/
--rw-rw-rw-   0        0        0      574 2023-07-24 21:19:20.000000 geeViz-2023.7.3/LICENSE
--rw-rw-rw-   0        0        0     3851 2023-07-24 21:19:47.428402 geeViz-2023.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-07-18 20:28:01.000000 geeViz-2023.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 21:19:47.332657 geeViz-2023.7.3/geeViz/
--rw-rw-rw-   0        0        0      127 2023-07-24 15:39:45.000000 geeViz-2023.7.3/geeViz/__init__.py
--rw-rw-rw-   0        0        0    23538 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/assetManagerLib.py
--rw-rw-rw-   0        0        0    96153 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/changeDetectionLib.py
-drwxrwxrwx   0        0        0        0 2023-07-24 21:19:47.394501 geeViz-2023.7.3/geeViz/examples/
--rw-rw-rw-   0        0        0     5467 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/CCDCViz.py
--rw-rw-rw-   0        0        0    11883 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/CCDCVizNotebook.ipynb
--rw-rw-rw-   0        0        0     8037 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/CCDCWrapper.py
--rw-rw-rw-   0        0        0     4424 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/GFSTimeLapse.py
--rw-rw-rw-   0        0        0     6284 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/LANDTRENDRViz.py
--rw-rw-rw-   0        0        0     9586 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/LANDTRENDRWrapper.py
--rw-rw-rw-   0        0        0    15557 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12631 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/LCMAP_and_LCMS_Viewer.py
--rw-rw-rw-   0        0        0    19522 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
--rw-rw-rw-   0        0        0      127 2023-07-24 15:39:39.000000 geeViz-2023.7.3/geeViz/examples/__init__.py
--rw-rw-rw-   0        0        0     1972 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/foliumViewerExample.py
--rw-rw-rw-   0        0        0   225731 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/gee2PandasExample.ipynb
--rw-rw-rw-   0        0        0     5771 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/geeViewExample.py
--rw-rw-rw-   0        0        0    16613 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/geeViewExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    43661 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0     5779 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/getClimateWrapper.py
--rw-rw-rw-   0        0        0    14302 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
--rw-rw-rw-   0        0        0    11478 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/getLandsatWrapper.py
--rw-rw-rw-   0        0        0    18431 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/getLandsatWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12263 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/getSentinel2Wrapper.py
--rw-rw-rw-   0        0        0     9196 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/harmonicRegressionWrapper.py
--rw-rw-rw-   0        0        0     8218 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/lcmsViewerExample.py
--rw-rw-rw-   0        0        0    18777 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/lcmsViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    13051 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/phEEnoVizWrapper.py
--rw-rw-rw-   0        0        0     1063 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/taskTrackerExample.py
--rw-rw-rw-   0        0        0     6317 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/examples/timeLapseExample.py
--rw-rw-rw-   0        0        0     8783 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/foliumView.py
--rw-rw-rw-   0        0        0     1741 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/gcpLib.py
--rw-rw-rw-   0        0        0    10077 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/gee2Pandas.py
-drwxrwxrwx   0        0        0        0 2023-07-24 21:19:47.400476 geeViz-2023.7.3/geeViz/geeView/
-drwxrwxrwx   0        0        0        0 2023-07-24 21:19:47.401484 geeViz-2023.7.3/geeViz/geeView/css/
--rw-rw-rw-   0        0        0    30585 2023-07-19 17:12:21.000000 geeViz-2023.7.3/geeViz/geeView/css/style.min.css
--rw-rw-rw-   0        0        0    10024 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/foliumView.html
-drwxrwxrwx   0        0        0        0 2023-07-24 21:19:47.420422 geeViz-2023.7.3/geeViz/geeView/images/
--rw-rw-rw-   0        0        0     7295 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/EE-logo-150.png
--rw-rw-rw-   0        0        0    10301 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/GEE.png
--rw-rw-rw-   0        0        0     5692 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/GEE_logo_transparent.png
--rw-rw-rw-   0        0        0     4551 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/RCR-logo.jpg
--rw-rw-rw-   0        0        0     8352 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/cumulative_icon.png
--rw-rw-rw-   0        0        0     1502 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/layer_icon.png
--rw-rw-rw-   0        0        0   232219 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/logos_usda-fs.svg
--rw-rw-rw-   0        0        0   231399 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
--rw-rw-rw-   0        0        0      652 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/menu-hamburger_ffffff.svg
--rw-rw-rw-   0        0        0     1489 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/usdalogo.png
--rw-rw-rw-   0        0        0     8174 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/images/usfslogo.png
--rw-rw-rw-   0        0        0     3455 2023-07-19 17:06:25.000000 geeViz-2023.7.3/geeViz/geeView/index.html
-drwxrwxrwx   0        0        0        0 2023-07-24 21:19:47.425411 geeViz-2023.7.3/geeViz/geeView/js/
--rw-rw-rw-   0        0        0    45351 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/js/gena-gee-palettes.js
--rw-rw-rw-   0        0        0   528516 2023-07-19 17:12:21.000000 geeViz-2023.7.3/geeViz/geeView/js/lcms-viewer.min.js
--rw-rw-rw-   0        0        0     1021 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/geeView/js/load.min.js
--rw-rw-rw-   0        0        0    22679 2023-07-19 18:17:03.000000 geeViz-2023.7.3/geeViz/geeView/js/runGeeViz.js
--rw-rw-rw-   0        0        0    16069 2023-07-19 18:14:04.000000 geeViz-2023.7.3/geeViz/geeView.py
--rw-rw-rw-   0        0        0   175641 2023-07-24 15:31:50.000000 geeViz-2023.7.3/geeViz/getImagesLib.py
--rw-rw-rw-   0        0        0     7467 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/migrateGEEAssets.py
--rw-rw-rw-   0        0        0    20743 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/phEEnoViz.py
--rw-rw-rw-   0        0        0     9885 2023-07-18 20:07:28.000000 geeViz-2023.7.3/geeViz/taskManagerLib.py
-drwxrwxrwx   0        0        0        0 2023-07-24 21:19:47.346619 geeViz-2023.7.3/geeViz.egg-info/
--rw-rw-rw-   0        0        0     3851 2023-07-24 21:19:47.000000 geeViz-2023.7.3/geeViz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2023-07-24 21:19:47.000000 geeViz-2023.7.3/geeViz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 21:19:47.000000 geeViz-2023.7.3/geeViz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-07-24 21:19:47.000000 geeViz-2023.7.3/geeViz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 21:19:47.000000 geeViz-2023.7.3/geeViz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 21:19:47.429401 geeViz-2023.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2173 2023-07-18 20:28:01.000000 geeViz-2023.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.911134 geeViz-2023.7.4/
+-rw-rw-rw-   0        0        0      574 2023-07-24 21:19:20.000000 geeViz-2023.7.4/LICENSE
+-rw-rw-rw-   0        0        0     3851 2023-07-24 21:31:26.910134 geeViz-2023.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-07-18 20:28:01.000000 geeViz-2023.7.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.784470 geeViz-2023.7.4/geeViz/
+-rw-rw-rw-   0        0        0      127 2023-07-24 21:29:30.000000 geeViz-2023.7.4/geeViz/__init__.py
+-rw-rw-rw-   0        0        0    23538 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/assetManagerLib.py
+-rw-rw-rw-   0        0        0    96153 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/changeDetectionLib.py
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.861264 geeViz-2023.7.4/geeViz/examples/
+-rw-rw-rw-   0        0        0     5467 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/CCDCViz.py
+-rw-rw-rw-   0        0        0    11883 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/CCDCVizNotebook.ipynb
+-rw-rw-rw-   0        0        0     8037 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/CCDCWrapper.py
+-rw-rw-rw-   0        0        0     4424 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/GFSTimeLapse.py
+-rw-rw-rw-   0        0        0     6284 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LANDTRENDRViz.py
+-rw-rw-rw-   0        0        0     9586 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LANDTRENDRWrapper.py
+-rw-rw-rw-   0        0        0    15557 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12631 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LCMAP_and_LCMS_Viewer.py
+-rw-rw-rw-   0        0        0    19522 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
+-rw-rw-rw-   0        0        0      127 2023-07-24 21:29:23.000000 geeViz-2023.7.4/geeViz/examples/__init__.py
+-rw-rw-rw-   0        0        0     1972 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/foliumViewerExample.py
+-rw-rw-rw-   0        0        0   225731 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/gee2PandasExample.ipynb
+-rw-rw-rw-   0        0        0     5771 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/geeViewExample.py
+-rw-rw-rw-   0        0        0    16613 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/geeViewExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    43661 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0     5779 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getClimateWrapper.py
+-rw-rw-rw-   0        0        0    14302 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0    11478 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getLandsatWrapper.py
+-rw-rw-rw-   0        0        0    18431 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getLandsatWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12263 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0     9196 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/harmonicRegressionWrapper.py
+-rw-rw-rw-   0        0        0     8218 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/lcmsViewerExample.py
+-rw-rw-rw-   0        0        0    18777 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/lcmsViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    13051 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/phEEnoVizWrapper.py
+-rw-rw-rw-   0        0        0     1063 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/taskTrackerExample.py
+-rw-rw-rw-   0        0        0     6317 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/timeLapseExample.py
+-rw-rw-rw-   0        0        0     8783 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/foliumView.py
+-rw-rw-rw-   0        0        0     1741 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/gcpLib.py
+-rw-rw-rw-   0        0        0    10077 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/gee2Pandas.py
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.864255 geeViz-2023.7.4/geeViz/geeView/
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.866250 geeViz-2023.7.4/geeViz/geeView/css/
+-rw-rw-rw-   0        0        0    30585 2023-07-19 17:12:21.000000 geeViz-2023.7.4/geeViz/geeView/css/style.min.css
+-rw-rw-rw-   0        0        0    10024 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/foliumView.html
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.896171 geeViz-2023.7.4/geeViz/geeView/images/
+-rw-rw-rw-   0        0        0     7295 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/EE-logo-150.png
+-rw-rw-rw-   0        0        0    10301 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/GEE.png
+-rw-rw-rw-   0        0        0     5692 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/GEE_logo_transparent.png
+-rw-rw-rw-   0        0        0     4551 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/RCR-logo.jpg
+-rw-rw-rw-   0        0        0     8352 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/cumulative_icon.png
+-rw-rw-rw-   0        0        0     1502 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/layer_icon.png
+-rw-rw-rw-   0        0        0   232219 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/logos_usda-fs.svg
+-rw-rw-rw-   0        0        0   231399 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
+-rw-rw-rw-   0        0        0      652 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/menu-hamburger_ffffff.svg
+-rw-rw-rw-   0        0        0     1489 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/usdalogo.png
+-rw-rw-rw-   0        0        0     8174 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/usfslogo.png
+-rw-rw-rw-   0        0        0     3455 2023-07-19 17:06:25.000000 geeViz-2023.7.4/geeViz/geeView/index.html
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.904148 geeViz-2023.7.4/geeViz/geeView/js/
+-rw-rw-rw-   0        0        0    45351 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/js/gena-gee-palettes.js
+-rw-rw-rw-   0        0        0   528516 2023-07-19 17:12:21.000000 geeViz-2023.7.4/geeViz/geeView/js/lcms-viewer.min.js
+-rw-rw-rw-   0        0        0     1021 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/js/load.min.js
+-rw-rw-rw-   0        0        0    22679 2023-07-19 18:17:03.000000 geeViz-2023.7.4/geeViz/geeView/js/runGeeViz.js
+-rw-rw-rw-   0        0        0    16069 2023-07-19 18:14:04.000000 geeViz-2023.7.4/geeViz/geeView.py
+-rw-rw-rw-   0        0        0   175797 2023-07-24 21:29:01.000000 geeViz-2023.7.4/geeViz/getImagesLib.py
+-rw-rw-rw-   0        0        0     7467 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/migrateGEEAssets.py
+-rw-rw-rw-   0        0        0    20743 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/phEEnoViz.py
+-rw-rw-rw-   0        0        0     9885 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/taskManagerLib.py
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.807407 geeViz-2023.7.4/geeViz.egg-info/
+-rw-rw-rw-   0        0        0     3851 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 21:31:26.911134 geeViz-2023.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-18 20:28:01.000000 geeViz-2023.7.4/setup.py
```

### Comparing `geeViz-2023.7.3/LICENSE` & `geeViz-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/PKG-INFO` & `geeViz-2023.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geeViz-2023.7.3/README.md` & `geeViz-2023.7.4/README.md`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/assetManagerLib.py` & `geeViz-2023.7.4/geeViz/assetManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/changeDetectionLib.py` & `geeViz-2023.7.4/geeViz/changeDetectionLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/CCDCViz.py` & `geeViz-2023.7.4/geeViz/examples/CCDCViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/CCDCVizNotebook.ipynb` & `geeViz-2023.7.4/geeViz/examples/CCDCVizNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/CCDCWrapper.py` & `geeViz-2023.7.4/geeViz/examples/CCDCWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/GFSTimeLapse.py` & `geeViz-2023.7.4/geeViz/examples/GFSTimeLapse.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/LANDTRENDRViz.py` & `geeViz-2023.7.4/geeViz/examples/LANDTRENDRViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/LANDTRENDRWrapper.py` & `geeViz-2023.7.4/geeViz/examples/LANDTRENDRWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb` & `geeViz-2023.7.4/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/LCMAP_and_LCMS_Viewer.py` & `geeViz-2023.7.4/geeViz/examples/LCMAP_and_LCMS_Viewer.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb` & `geeViz-2023.7.4/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/foliumViewerExample.py` & `geeViz-2023.7.4/geeViz/examples/foliumViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/gee2PandasExample.ipynb` & `geeViz-2023.7.4/geeViz/examples/gee2PandasExample.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/geeViewExample.py` & `geeViz-2023.7.4/geeViz/examples/geeViewExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/geeViewExampleNotebook.ipynb` & `geeViz-2023.7.4/geeViz/examples/geeViewExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb` & `geeViz-2023.7.4/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/getClimateWrapper.py` & `geeViz-2023.7.4/geeViz/examples/getClimateWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py` & `geeViz-2023.7.4/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/getLandsatWrapper.py` & `geeViz-2023.7.4/geeViz/examples/getLandsatWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/getLandsatWrapperNotebook.ipynb` & `geeViz-2023.7.4/geeViz/examples/getLandsatWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/getSentinel2Wrapper.py` & `geeViz-2023.7.4/geeViz/examples/getSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/harmonicRegressionWrapper.py` & `geeViz-2023.7.4/geeViz/examples/harmonicRegressionWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/lcmsViewerExample.py` & `geeViz-2023.7.4/geeViz/examples/lcmsViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/lcmsViewerExampleNotebook.ipynb` & `geeViz-2023.7.4/geeViz/examples/lcmsViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/phEEnoVizWrapper.py` & `geeViz-2023.7.4/geeViz/examples/phEEnoVizWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/taskTrackerExample.py` & `geeViz-2023.7.4/geeViz/examples/taskTrackerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/examples/timeLapseExample.py` & `geeViz-2023.7.4/geeViz/examples/timeLapseExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/foliumView.py` & `geeViz-2023.7.4/geeViz/foliumView.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/gcpLib.py` & `geeViz-2023.7.4/geeViz/gcpLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/gee2Pandas.py` & `geeViz-2023.7.4/geeViz/gee2Pandas.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/css/style.min.css` & `geeViz-2023.7.4/geeViz/geeView/css/style.min.css`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/foliumView.html` & `geeViz-2023.7.4/geeViz/geeView/foliumView.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/EE-logo-150.png` & `geeViz-2023.7.4/geeViz/geeView/images/EE-logo-150.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/GEE.png` & `geeViz-2023.7.4/geeViz/geeView/images/GEE.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/GEE_logo_transparent.png` & `geeViz-2023.7.4/geeViz/geeView/images/GEE_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/RCR-logo.jpg` & `geeViz-2023.7.4/geeViz/geeView/images/RCR-logo.jpg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/cumulative_icon.png` & `geeViz-2023.7.4/geeViz/geeView/images/cumulative_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/layer_icon.png` & `geeViz-2023.7.4/geeViz/geeView/images/layer_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/logos_usda-fs.svg` & `geeViz-2023.7.4/geeViz/geeView/images/logos_usda-fs.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg` & `geeViz-2023.7.4/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/menu-hamburger_ffffff.svg` & `geeViz-2023.7.4/geeViz/geeView/images/menu-hamburger_ffffff.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/usdalogo.png` & `geeViz-2023.7.4/geeViz/geeView/images/usdalogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/images/usfslogo.png` & `geeViz-2023.7.4/geeViz/geeView/images/usfslogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/index.html` & `geeViz-2023.7.4/geeViz/geeView/index.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/js/gena-gee-palettes.js` & `geeViz-2023.7.4/geeViz/geeView/js/gena-gee-palettes.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/js/lcms-viewer.min.js` & `geeViz-2023.7.4/geeViz/geeView/js/lcms-viewer.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/js/load.min.js` & `geeViz-2023.7.4/geeViz/geeView/js/load.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView/js/runGeeViz.js` & `geeViz-2023.7.4/geeViz/geeView/js/runGeeViz.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/geeView.py` & `geeViz-2023.7.4/geeViz/geeView.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/getImagesLib.py` & `geeViz-2023.7.4/geeViz/getImagesLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -7186,3793 +7186,3803 @@
 0001c110: 7075 7465 6454 444f 4d49 5253 7464 4465  putedTDOMIRStdDe
 0001c120: 7620 3d20 4e6f 6e65 2c0d 0a20 2063 6f6d  v = None,..  com
 0001c130: 706f 7369 7469 6e67 5265 6475 6365 7220  positingReducer 
 0001c140: 3d20 4e6f 6e65 2c0d 0a20 2068 6172 6d6f  = None,..  harmo
 0001c150: 6e69 7a65 4f4c 4920 3d20 4661 6c73 652c  nizeOLI = False,
 0001c160: 0d0a 2020 6c61 6e64 7361 7443 6f6c 6c65  ..  landsatColle
 0001c170: 6374 696f 6e56 6572 7369 6f6e 203d 2027  ctionVersion = '
-0001c180: 4332 2729 3a0d 0a0d 0a20 2074 6f61 4f72  C2'):....  toaOr
-0001c190: 5352 203d 2074 6f61 4f72 5352 2e75 7070  SR = toaOrSR.upp
-0001c1a0: 6572 2829 0d0a 2020 6f72 6967 696e 203d  er()..  origin =
-0001c1b0: 2027 4c61 6e64 7361 7427 0d0a 2020 6172   'Landsat'..  ar
-0001c1c0: 6773 203d 2066 6f72 6d61 7441 7267 7328  gs = formatArgs(
-0001c1d0: 6c6f 6361 6c73 2829 290d 0a20 2069 6620  locals())..  if 
-0001c1e0: 2761 7267 7327 2069 6e20 6172 6773 2e6b  'args' in args.k
-0001c1f0: 6579 7328 293a 0d0a 2020 2020 6465 6c20  eys():..    del 
-0001c200: 6172 6773 5b27 6172 6773 275d 0d0a 0d0a  args['args']....
-0001c210: 2020 2350 7265 7061 7265 2064 6174 6573    #Prepare dates
-0001c220: 0d0a 2020 7772 6170 4f66 6673 6574 203d  ..  wrapOffset =
-0001c230: 2030 0d0a 2020 6966 2073 7461 7274 4a75   0..  if startJu
-0001c240: 6c69 616e 203e 2065 6e64 4a75 6c69 616e  lian > endJulian
-0001c250: 3a0d 0a20 2020 2077 7261 704f 6666 7365  :..    wrapOffse
-0001c260: 7420 3d20 3336 350d 0a20 2073 7461 7274  t = 365..  start
-0001c270: 4461 7465 203d 2065 652e 4461 7465 2e66  Date = ee.Date.f
-0001c280: 726f 6d59 4d44 2873 7461 7274 5965 6172  romYMD(startYear
-0001c290: 2c31 2c31 292e 6164 7661 6e63 6528 7374  ,1,1).advance(st
-0001c2a0: 6172 744a 756c 6961 6e2d 312c 2764 6179  artJulian-1,'day
-0001c2b0: 2729 0d0a 2020 656e 6444 6174 6520 3d20  ')..  endDate = 
-0001c2c0: 6565 2e44 6174 652e 6672 6f6d 594d 4428  ee.Date.fromYMD(
-0001c2d0: 656e 6459 6561 722c 312c 3129 2e61 6476  endYear,1,1).adv
-0001c2e0: 616e 6365 2865 6e64 4a75 6c69 616e 2d31  ance(endJulian-1
-0001c2f0: 2b77 7261 704f 6666 7365 742c 2764 6179  +wrapOffset,'day
-0001c300: 2729 0d0a 0d0a 2020 2320 4765 7420 4c61  ')....  # Get La
-0001c310: 6e64 7361 7420 696d 6167 6520 636f 6c6c  ndsat image coll
-0001c320: 6563 7469 6f6e 2061 6e64 2061 7070 6c79  ection and apply
-0001c330: 2063 6c6f 7564 206d 6173 6b69 6e67 0d0a   cloud masking..
-0001c340: 2020 6c73 203d 2067 6574 5072 6f63 6573    ls = getProces
-0001c350: 7365 644c 616e 6473 6174 5363 656e 6573  sedLandsatScenes
-0001c360: 280d 0a20 2020 2073 7475 6479 4172 6561  (..    studyArea
-0001c370: 203d 2073 7475 6479 4172 6561 2c0d 0a20   = studyArea,.. 
-0001c380: 2020 2073 7461 7274 5965 6172 203d 2073     startYear = s
-0001c390: 7461 7274 5965 6172 2c0d 0a20 2020 2065  tartYear,..    e
-0001c3a0: 6e64 5965 6172 203d 2065 6e64 5965 6172  ndYear = endYear
-0001c3b0: 2c0d 0a20 2020 2073 7461 7274 4a75 6c69  ,..    startJuli
-0001c3c0: 616e 203d 2073 7461 7274 4a75 6c69 616e  an = startJulian
-0001c3d0: 2c0d 0a20 2020 2065 6e64 4a75 6c69 616e  ,..    endJulian
-0001c3e0: 203d 2065 6e64 4a75 6c69 616e 2c0d 0a20   = endJulian,.. 
-0001c3f0: 2020 2074 6f61 4f72 5352 203d 2074 6f61     toaOrSR = toa
-0001c400: 4f72 5352 2c0d 0a20 2020 2069 6e63 6c75  OrSR,..    inclu
-0001c410: 6465 534c 434f 6666 4c37 203d 2069 6e63  deSLCOffL7 = inc
-0001c420: 6c75 6465 534c 434f 6666 4c37 2c0d 0a20  ludeSLCOffL7,.. 
-0001c430: 2020 2064 6566 7269 6e67 654c 3520 3d20     defringeL5 = 
-0001c440: 6465 6672 696e 6765 4c35 2c0d 0a20 2020  defringeL5,..   
-0001c450: 2061 7070 6c79 436c 6f75 6453 636f 7265   applyCloudScore
-0001c460: 203d 2061 7070 6c79 436c 6f75 6453 636f   = applyCloudSco
-0001c470: 7265 2c0d 0a20 2020 2061 7070 6c79 466d  re,..    applyFm
-0001c480: 6173 6b43 6c6f 7564 4d61 736b 203d 2061  askCloudMask = a
+0001c180: 4332 272c 0d0a 2020 6f76 6572 7772 6974  C2',..  overwrit
+0001c190: 6520 3d20 4661 6c73 6529 3a0d 0a0d 0a20  e = False):.... 
+0001c1a0: 2074 6f61 4f72 5352 203d 2074 6f61 4f72   toaOrSR = toaOr
+0001c1b0: 5352 2e75 7070 6572 2829 0d0a 2020 6f72  SR.upper()..  or
+0001c1c0: 6967 696e 203d 2027 4c61 6e64 7361 7427  igin = 'Landsat'
+0001c1d0: 0d0a 2020 6172 6773 203d 2066 6f72 6d61  ..  args = forma
+0001c1e0: 7441 7267 7328 6c6f 6361 6c73 2829 290d  tArgs(locals()).
+0001c1f0: 0a20 2069 6620 2761 7267 7327 2069 6e20  .  if 'args' in 
+0001c200: 6172 6773 2e6b 6579 7328 293a 0d0a 2020  args.keys():..  
+0001c210: 2020 6465 6c20 6172 6773 5b27 6172 6773    del args['args
+0001c220: 275d 0d0a 0d0a 2020 2350 7265 7061 7265  ']....  #Prepare
+0001c230: 2064 6174 6573 0d0a 2020 7772 6170 4f66   dates..  wrapOf
+0001c240: 6673 6574 203d 2030 0d0a 2020 6966 2073  fset = 0..  if s
+0001c250: 7461 7274 4a75 6c69 616e 203e 2065 6e64  tartJulian > end
+0001c260: 4a75 6c69 616e 3a0d 0a20 2020 2077 7261  Julian:..    wra
+0001c270: 704f 6666 7365 7420 3d20 3336 350d 0a20  pOffset = 365.. 
+0001c280: 2073 7461 7274 4461 7465 203d 2065 652e   startDate = ee.
+0001c290: 4461 7465 2e66 726f 6d59 4d44 2873 7461  Date.fromYMD(sta
+0001c2a0: 7274 5965 6172 2c31 2c31 292e 6164 7661  rtYear,1,1).adva
+0001c2b0: 6e63 6528 7374 6172 744a 756c 6961 6e2d  nce(startJulian-
+0001c2c0: 312c 2764 6179 2729 0d0a 2020 656e 6444  1,'day')..  endD
+0001c2d0: 6174 6520 3d20 6565 2e44 6174 652e 6672  ate = ee.Date.fr
+0001c2e0: 6f6d 594d 4428 656e 6459 6561 722c 312c  omYMD(endYear,1,
+0001c2f0: 3129 2e61 6476 616e 6365 2865 6e64 4a75  1).advance(endJu
+0001c300: 6c69 616e 2d31 2b77 7261 704f 6666 7365  lian-1+wrapOffse
+0001c310: 742c 2764 6179 2729 0d0a 0d0a 2020 2320  t,'day')....  # 
+0001c320: 4765 7420 4c61 6e64 7361 7420 696d 6167  Get Landsat imag
+0001c330: 6520 636f 6c6c 6563 7469 6f6e 2061 6e64  e collection and
+0001c340: 2061 7070 6c79 2063 6c6f 7564 206d 6173   apply cloud mas
+0001c350: 6b69 6e67 0d0a 2020 6c73 203d 2067 6574  king..  ls = get
+0001c360: 5072 6f63 6573 7365 644c 616e 6473 6174  ProcessedLandsat
+0001c370: 5363 656e 6573 280d 0a20 2020 2073 7475  Scenes(..    stu
+0001c380: 6479 4172 6561 203d 2073 7475 6479 4172  dyArea = studyAr
+0001c390: 6561 2c0d 0a20 2020 2073 7461 7274 5965  ea,..    startYe
+0001c3a0: 6172 203d 2073 7461 7274 5965 6172 2c0d  ar = startYear,.
+0001c3b0: 0a20 2020 2065 6e64 5965 6172 203d 2065  .    endYear = e
+0001c3c0: 6e64 5965 6172 2c0d 0a20 2020 2073 7461  ndYear,..    sta
+0001c3d0: 7274 4a75 6c69 616e 203d 2073 7461 7274  rtJulian = start
+0001c3e0: 4a75 6c69 616e 2c0d 0a20 2020 2065 6e64  Julian,..    end
+0001c3f0: 4a75 6c69 616e 203d 2065 6e64 4a75 6c69  Julian = endJuli
+0001c400: 616e 2c0d 0a20 2020 2074 6f61 4f72 5352  an,..    toaOrSR
+0001c410: 203d 2074 6f61 4f72 5352 2c0d 0a20 2020   = toaOrSR,..   
+0001c420: 2069 6e63 6c75 6465 534c 434f 6666 4c37   includeSLCOffL7
+0001c430: 203d 2069 6e63 6c75 6465 534c 434f 6666   = includeSLCOff
+0001c440: 4c37 2c0d 0a20 2020 2064 6566 7269 6e67  L7,..    defring
+0001c450: 654c 3520 3d20 6465 6672 696e 6765 4c35  eL5 = defringeL5
+0001c460: 2c0d 0a20 2020 2061 7070 6c79 436c 6f75  ,..    applyClou
+0001c470: 6453 636f 7265 203d 2061 7070 6c79 436c  dScore = applyCl
+0001c480: 6f75 6453 636f 7265 2c0d 0a20 2020 2061  oudScore,..    a
 0001c490: 7070 6c79 466d 6173 6b43 6c6f 7564 4d61  pplyFmaskCloudMa
-0001c4a0: 736b 2c0d 0a20 2020 2061 7070 6c79 5444  sk,..    applyTD
-0001c4b0: 4f4d 203d 2061 7070 6c79 5444 4f4d 2c0d  OM = applyTDOM,.
-0001c4c0: 0a20 2020 2061 7070 6c79 466d 6173 6b43  .    applyFmaskC
-0001c4d0: 6c6f 7564 5368 6164 6f77 4d61 736b 203d  loudShadowMask =
-0001c4e0: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
-0001c4f0: 5368 6164 6f77 4d61 736b 2c0d 0a20 2020  ShadowMask,..   
-0001c500: 2061 7070 6c79 466d 6173 6b53 6e6f 774d   applyFmaskSnowM
-0001c510: 6173 6b20 3d20 6170 706c 7946 6d61 736b  ask = applyFmask
-0001c520: 536e 6f77 4d61 736b 2c0d 0a20 2020 2063  SnowMask,..    c
-0001c530: 6c6f 7564 5363 6f72 6554 6872 6573 6820  loudScoreThresh 
-0001c540: 3d20 636c 6f75 6453 636f 7265 5468 7265  = cloudScoreThre
-0001c550: 7368 2c0d 0a20 2020 2070 6572 666f 726d  sh,..    perform
-0001c560: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
-0001c570: 203d 2070 6572 666f 726d 436c 6f75 6453   = performCloudS
-0001c580: 636f 7265 4f66 6673 6574 2c0d 0a20 2020  coreOffset,..   
-0001c590: 2063 6c6f 7564 5363 6f72 6550 6374 6c20   cloudScorePctl 
-0001c5a0: 3d20 636c 6f75 6453 636f 7265 5063 746c  = cloudScorePctl
-0001c5b0: 2c0d 0a20 2020 207a 5363 6f72 6554 6872  ,..    zScoreThr
-0001c5c0: 6573 6820 3d20 7a53 636f 7265 5468 7265  esh = zScoreThre
-0001c5d0: 7368 2c0d 0a20 2020 2073 6861 646f 7753  sh,..    shadowS
-0001c5e0: 756d 5468 7265 7368 203d 2073 6861 646f  umThresh = shado
-0001c5f0: 7753 756d 5468 7265 7368 2c0d 0a20 2020  wSumThresh,..   
-0001c600: 2063 6f6e 7472 6163 7450 6978 656c 7320   contractPixels 
-0001c610: 3d20 636f 6e74 7261 6374 5069 7865 6c73  = contractPixels
-0001c620: 2c0d 0a20 2020 2064 696c 6174 6550 6978  ,..    dilatePix
-0001c630: 656c 7320 3d20 6469 6c61 7465 5069 7865  els = dilatePixe
-0001c640: 6c73 2c0d 0a20 2020 2072 6573 616d 706c  ls,..    resampl
-0001c650: 654d 6574 686f 6420 3d20 7265 7361 6d70  eMethod = resamp
-0001c660: 6c65 4d65 7468 6f64 2c0d 0a20 2020 2068  leMethod,..    h
-0001c670: 6172 6d6f 6e69 7a65 4f4c 4920 3d20 6861  armonizeOLI = ha
-0001c680: 726d 6f6e 697a 654f 4c49 2c0d 0a20 2020  rmonizeOLI,..   
-0001c690: 2070 7265 436f 6d70 7574 6564 436c 6f75   preComputedClou
-0001c6a0: 6453 636f 7265 4f66 6673 6574 203d 2070  dScoreOffset = p
-0001c6b0: 7265 436f 6d70 7574 6564 436c 6f75 6453  reComputedCloudS
-0001c6c0: 636f 7265 4f66 6673 6574 2c0d 0a20 2020  coreOffset,..   
-0001c6d0: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
-0001c6e0: 4952 4d65 616e 203d 2070 7265 436f 6d70  IRMean = preComp
-0001c6f0: 7574 6564 5444 4f4d 4952 4d65 616e 2c0d  utedTDOMIRMean,.
-0001c700: 0a20 2020 2070 7265 436f 6d70 7574 6564  .    preComputed
-0001c710: 5444 4f4d 4952 5374 6444 6576 203d 2070  TDOMIRStdDev = p
-0001c720: 7265 436f 6d70 7574 6564 5444 4f4d 4952  reComputedTDOMIR
-0001c730: 5374 6444 6576 2c0d 0a20 2020 206c 616e  StdDev,..    lan
-0001c740: 6473 6174 436f 6c6c 6563 7469 6f6e 5665  dsatCollectionVe
-0001c750: 7273 696f 6e20 3d20 6c61 6e64 7361 7443  rsion = landsatC
-0001c760: 6f6c 6c65 6374 696f 6e56 6572 7369 6f6e  ollectionVersion
-0001c770: 290d 0a0d 0a20 2023 4164 6420 7a65 6e69  )....  #Add zeni
-0001c780: 7468 2061 6e64 2061 7a69 6d75 7468 0d0a  th and azimuth..
-0001c790: 2020 6966 2063 6f72 7265 6374 496c 6c75    if correctIllu
-0001c7a0: 6d69 6e61 7469 6f6e 3a0d 0a20 2020 2070  mination:..    p
-0001c7b0: 7269 6e74 2827 4164 6469 6e67 207a 656e  rint('Adding zen
-0001c7c0: 6974 6820 616e 6420 617a 696d 7574 6820  ith and azimuth 
-0001c7d0: 666f 7220 7465 7272 6169 6e20 636f 7272  for terrain corr
-0001c7e0: 6563 7469 6f6e 2729 0d0a 2020 2020 6c73  ection')..    ls
-0001c7f0: 203d 206c 732e 6d61 7028 6c61 6d62 6461   = ls.map(lambda
-0001c800: 2069 6d67 3a20 6164 645a 656e 6974 6841   img: addZenithA
-0001c810: 7a69 6d75 7468 2869 6d67 2c20 746f 614f  zimuth(img, toaO
-0001c820: 7253 5229 290d 0a0d 0a20 2023 4372 6561  rSR))....  #Crea
-0001c830: 7465 2063 6f6d 706f 7369 7465 2074 696d  te composite tim
-0001c840: 6520 7365 7269 6573 0d0a 2020 7473 203d  e series..  ts =
-0001c850: 2063 6f6d 706f 7369 7465 5469 6d65 5365   compositeTimeSe
-0001c860: 7269 6573 285c 0d0a 2020 2020 6c73 203d  ries(\..    ls =
-0001c870: 206c 732c 0d0a 2020 2020 7374 6172 7459   ls,..    startY
-0001c880: 6561 7220 3d20 7374 6172 7459 6561 722c  ear = startYear,
-0001c890: 0d0a 2020 2020 656e 6459 6561 7220 3d20  ..    endYear = 
-0001c8a0: 656e 6459 6561 722c 0d0a 2020 2020 7374  endYear,..    st
-0001c8b0: 6172 744a 756c 6961 6e20 3d20 7374 6172  artJulian = star
-0001c8c0: 744a 756c 6961 6e2c 0d0a 2020 2020 656e  tJulian,..    en
-0001c8d0: 644a 756c 6961 6e20 3d20 656e 644a 756c  dJulian = endJul
-0001c8e0: 6961 6e2c 0d0a 2020 2020 7469 6d65 6275  ian,..    timebu
-0001c8f0: 6666 6572 203d 2074 696d 6562 7566 6665  ffer = timebuffe
-0001c900: 722c 0d0a 2020 2020 7765 6967 6874 7320  r,..    weights 
-0001c910: 3d20 7765 6967 6874 732c 0d0a 2020 2020  = weights,..    
-0001c920: 636f 6d70 6f73 6974 696e 674d 6574 686f  compositingMetho
-0001c930: 6420 3d20 636f 6d70 6f73 6974 696e 674d  d = compositingM
-0001c940: 6574 686f 642c 0d0a 2020 2020 636f 6d70  ethod,..    comp
-0001c950: 6f73 6974 696e 6752 6564 7563 6572 203d  ositingReducer =
-0001c960: 2063 6f6d 706f 7369 7469 6e67 5265 6475   compositingRedu
-0001c970: 6365 7229 0d0a 0d0a 2020 2320 436f 7272  cer)....  # Corr
-0001c980: 6563 7420 696c 6c75 6d69 6e61 7469 6f6e  ect illumination
-0001c990: 0d0a 2020 6966 2063 6f72 7265 6374 496c  ..  if correctIl
-0001c9a0: 6c75 6d69 6e61 7469 6f6e 3a0d 0a20 2020  lumination:..   
-0001c9b0: 2070 7269 6e74 2827 436f 7272 6563 7469   print('Correcti
-0001c9c0: 6e67 2069 6c6c 756d 696e 6174 696f 6e27  ng illumination'
-0001c9d0: 293b 0d0a 2020 2020 7473 203d 2074 732e  );..    ts = ts.
-0001c9e0: 6d61 7028 696c 6c75 6d69 6e61 7469 6f6e  map(illumination
-0001c9f0: 436f 6e64 6974 696f 6e29 2e6d 6170 286c  Condition).map(l
-0001ca00: 616d 6264 6120 696d 673a 2069 6c6c 756d  ambda img: illum
-0001ca10: 696e 6174 696f 6e43 6f72 7265 6374 696f  inationCorrectio
-0001ca20: 6e28 696d 672c 2063 6f72 7265 6374 5363  n(img, correctSc
-0001ca30: 616c 652c 2073 7475 6479 4172 6561 2929  ale, studyArea))
-0001ca40: 0d0a 0d0a 2020 2345 7870 6f72 7420 636f  ....  #Export co
-0001ca50: 6d70 6f73 6974 6573 0d0a 2020 6966 2065  mposites..  if e
-0001ca60: 7870 6f72 7443 6f6d 706f 7369 7465 733a  xportComposites:
-0001ca70: 0d0a 2020 2020 6966 2063 6f6d 706f 7369  ..    if composi
-0001ca80: 7469 6e67 4d65 7468 6f64 203d 3d20 276d  tingMethod == 'm
-0001ca90: 6564 6f69 6427 3a0d 0a20 2020 2020 2065  edoid':..      e
-0001caa0: 7870 6f72 7442 616e 6473 203d 205b 2762  xportBands = ['b
-0001cab0: 6c75 6527 2c20 2767 7265 656e 272c 2027  lue', 'green', '
-0001cac0: 7265 6427 2c20 276e 6972 272c 2027 7377  red', 'nir', 'sw
-0001cad0: 6972 3127 2c20 2773 7769 7232 272c 2027  ir1', 'swir2', '
-0001cae0: 7465 6d70 272c 2027 636f 6d70 6f73 6974  temp', 'composit
-0001caf0: 654f 6273 436f 756e 7427 2c20 2773 656e  eObsCount', 'sen
-0001cb00: 736f 7227 2c20 2779 6561 7227 2c20 276a  sor', 'year', 'j
-0001cb10: 756c 6961 6e44 6179 275d 0d0a 2020 2020  ulianDay']..    
-0001cb20: 2020 6e6f 6e44 6976 6964 6542 616e 6473    nonDivideBands
-0001cb30: 203d 205b 2774 656d 7027 2c20 2763 6f6d   = ['temp', 'com
-0001cb40: 706f 7369 7465 4f62 7343 6f75 6e74 272c  positeObsCount',
-0001cb50: 2027 7365 6e73 6f72 272c 2027 7965 6172   'sensor', 'year
-0001cb60: 272c 2027 6a75 6c69 616e 4461 7927 5d0d  ', 'julianDay'].
-0001cb70: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-0001cb80: 2020 6578 706f 7274 4261 6e64 7320 3d20    exportBands = 
-0001cb90: 5b27 626c 7565 272c 2027 6772 6565 6e27  ['blue', 'green'
-0001cba0: 2c20 2772 6564 272c 2027 6e69 7227 2c20  , 'red', 'nir', 
-0001cbb0: 2773 7769 7231 272c 2027 7377 6972 3227  'swir1', 'swir2'
-0001cbc0: 2c20 2774 656d 7027 2c20 2763 6f6d 706f  , 'temp', 'compo
-0001cbd0: 7369 7465 4f62 7343 6f75 6e74 275d 0d0a  siteObsCount']..
-0001cbe0: 2020 2020 2020 6e6f 6e44 6976 6964 6542        nonDivideB
-0001cbf0: 616e 6473 203d 205b 2774 656d 7027 2c20  ands = ['temp', 
-0001cc00: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
-0001cc10: 6e74 275d 0d0a 0d0a 2020 2020 6578 706f  nt']....    expo
-0001cc20: 7274 436f 6d70 6f73 6974 6543 6f6c 6c65  rtCompositeColle
-0001cc30: 6374 696f 6e28 5c0d 0a20 2020 2020 2063  ction(\..      c
-0001cc40: 6f6c 6c65 6374 696f 6e20 3d20 7473 2c0d  ollection = ts,.
-0001cc50: 0a20 2020 2020 2065 7870 6f72 7450 6174  .      exportPat
-0001cc60: 6852 6f6f 7420 3d20 6578 706f 7274 5061  hRoot = exportPa
-0001cc70: 7468 526f 6f74 2c0d 0a20 2020 2020 206f  thRoot,..      o
-0001cc80: 7574 7075 744e 616d 6520 3d20 6f75 7470  utputName = outp
-0001cc90: 7574 4e61 6d65 2c0d 0a20 2020 2020 206f  utName,..      o
-0001cca0: 7269 6769 6e20 3d20 6f72 6967 696e 2c0d  rigin = origin,.
-0001ccb0: 0a20 2020 2020 2073 7475 6479 4172 6561  .      studyArea
-0001ccc0: 203d 2073 7475 6479 4172 6561 2c0d 0a20   = studyArea,.. 
-0001ccd0: 2020 2020 2063 7273 203d 2063 7273 2c0d       crs = crs,.
-0001cce0: 0a20 2020 2020 2074 7261 6e73 666f 726d  .      transform
-0001ccf0: 203d 2074 7261 6e73 666f 726d 2c0d 0a20   = transform,.. 
-0001cd00: 2020 2020 2073 6361 6c65 203d 2073 6361       scale = sca
-0001cd10: 6c65 2c0d 0a20 2020 2020 2073 7461 7274  le,..      start
-0001cd20: 5965 6172 203d 2073 7461 7274 5965 6172  Year = startYear
-0001cd30: 2c0d 0a20 2020 2020 2065 6e64 5965 6172  ,..      endYear
-0001cd40: 203d 2065 6e64 5965 6172 2c0d 0a20 2020   = endYear,..   
-0001cd50: 2020 2073 7461 7274 4a75 6c69 616e 203d     startJulian =
-0001cd60: 2073 7461 7274 4a75 6c69 616e 2c0d 0a20   startJulian,.. 
-0001cd70: 2020 2020 2065 6e64 4a75 6c69 616e 203d       endJulian =
-0001cd80: 2065 6e64 4a75 6c69 616e 2c0d 0a20 2020   endJulian,..   
-0001cd90: 2020 2063 6f6d 706f 7369 7469 6e67 4d65     compositingMe
-0001cda0: 7468 6f64 203d 2063 6f6d 706f 7369 7469  thod = compositi
-0001cdb0: 6e67 4d65 7468 6f64 2c0d 0a20 2020 2020  ngMethod,..     
-0001cdc0: 2074 696d 6562 7566 6665 7220 3d20 7469   timebuffer = ti
-0001cdd0: 6d65 6275 6666 6572 2c0d 0a20 2020 2020  mebuffer,..     
-0001cde0: 2074 6f61 4f72 5352 203d 2074 6f61 4f72   toaOrSR = toaOr
-0001cdf0: 5352 2c0d 0a20 2020 2020 206e 6f6e 4469  SR,..      nonDi
-0001ce00: 7669 6465 4261 6e64 7320 3d20 6e6f 6e44  videBands = nonD
-0001ce10: 6976 6964 6542 616e 6473 2c0d 0a20 2020  ivideBands,..   
-0001ce20: 2020 2065 7870 6f72 7442 616e 6473 203d     exportBands =
-0001ce30: 2065 7870 6f72 7442 616e 6473 2c0d 0a20   exportBands,.. 
-0001ce40: 2020 2020 2023 2077 6569 6768 7473 203d       # weights =
-0001ce50: 2077 6569 6768 7473 2c0d 0a20 2020 2020   weights,..     
-0001ce60: 2023 2064 6566 7269 6e67 654c 3520 3d20   # defringeL5 = 
-0001ce70: 4661 6c73 652c 0d0a 2020 2020 2020 2320  False,..      # 
-0001ce80: 696e 636c 7564 6553 4c43 4f66 664c 3720  includeSLCOffL7 
-0001ce90: 3d20 696e 636c 7564 6553 4c43 4f66 664c  = includeSLCOffL
-0001cea0: 372c 0d0a 2020 2020 2020 2320 636f 6e76  7,..      # conv
-0001ceb0: 6572 7454 6f44 6169 6c79 4d6f 7361 6963  ertToDailyMosaic
-0001cec0: 7320 3d20 274e 4127 2c0d 0a20 2020 2020  s = 'NA',..     
-0001ced0: 2023 2061 7070 6c79 5141 4261 6e64 203d   # applyQABand =
-0001cee0: 2046 616c 7365 2c0d 0a20 2020 2020 2023   False,..      #
-0001cef0: 2061 7070 6c79 436c 6f75 6453 636f 7265   applyCloudScore
-0001cf00: 203d 2061 7070 6c79 436c 6f75 6453 636f   = applyCloudSco
-0001cf10: 7265 2c0d 0a20 2020 2020 2023 2061 7070  re,..      # app
-0001cf20: 6c79 466d 6173 6b43 6c6f 7564 4d61 736b  lyFmaskCloudMask
-0001cf30: 203d 2061 7070 6c79 466d 6173 6b43 6c6f   = applyFmaskClo
-0001cf40: 7564 4d61 736b 2c0d 0a20 2020 2020 2023  udMask,..      #
-0001cf50: 2061 7070 6c79 436c 6f75 6450 726f 6261   applyCloudProba
-0001cf60: 6269 6c69 7479 203d 2027 4e41 272c 0d0a  bility = 'NA',..
-0001cf70: 2020 2020 2020 2320 6170 706c 7954 444f        # applyTDO
-0001cf80: 4d20 3d20 6170 706c 7954 444f 4d2c 0d0a  M = applyTDOM,..
-0001cf90: 2020 2020 2020 2320 6170 706c 7946 6d61        # applyFma
-0001cfa0: 736b 436c 6f75 6453 6861 646f 774d 6173  skCloudShadowMas
-0001cfb0: 6b20 3d20 6170 706c 7946 6d61 736b 436c  k = applyFmaskCl
-0001cfc0: 6f75 6453 6861 646f 774d 6173 6b2c 0d0a  oudShadowMask,..
-0001cfd0: 2020 2020 2020 2320 6170 706c 7946 6d61        # applyFma
-0001cfe0: 736b 536e 6f77 4d61 736b 203d 2061 7070  skSnowMask = app
-0001cff0: 6c79 466d 6173 6b53 6e6f 774d 6173 6b2c  lyFmaskSnowMask,
-0001d000: 0d0a 2020 2020 2020 2320 6170 706c 7953  ..      # applyS
-0001d010: 6861 646f 7753 6869 6674 203d 2027 4e41  hadowShift = 'NA
-0001d020: 272c 0d0a 2020 2020 2020 2320 636c 6f75  ',..      # clou
-0001d030: 6448 6569 6768 7473 203d 2063 6c6f 7564  dHeights = cloud
-0001d040: 4865 6967 6874 732c 0d0a 2020 2020 2020  Heights,..      
-0001d050: 2320 636c 6f75 6453 636f 7265 5468 7265  # cloudScoreThre
-0001d060: 7368 203d 2063 6c6f 7564 5363 6f72 6554  sh = cloudScoreT
-0001d070: 6872 6573 682c 0d0a 2020 2020 2020 2320  hresh,..      # 
-0001d080: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
-0001d090: 654f 6666 7365 7420 3d20 7065 7266 6f72  eOffset = perfor
-0001d0a0: 6d43 6c6f 7564 5363 6f72 654f 6666 7365  mCloudScoreOffse
-0001d0b0: 742c 0d0a 2020 2020 2020 2320 636c 6f75  t,..      # clou
-0001d0c0: 6453 636f 7265 5063 746c 203d 2063 6c6f  dScorePctl = clo
-0001d0d0: 7564 5363 6f72 6550 6374 6c2c 0d0a 2020  udScorePctl,..  
-0001d0e0: 2020 2020 2320 7a53 636f 7265 5468 7265      # zScoreThre
-0001d0f0: 7368 203d 207a 5363 6f72 6554 6872 6573  sh = zScoreThres
-0001d100: 682c 0d0a 2020 2020 2020 2320 7368 6164  h,..      # shad
-0001d110: 6f77 5375 6d54 6872 6573 6820 3d20 7368  owSumThresh = sh
-0001d120: 6164 6f77 5375 6d54 6872 6573 682c 0d0a  adowSumThresh,..
-0001d130: 2020 2020 2020 2320 636f 6e74 7261 6374        # contract
-0001d140: 5069 7865 6c73 203d 2063 6f6e 7472 6163  Pixels = contrac
-0001d150: 7450 6978 656c 732c 0d0a 2020 2020 2020  tPixels,..      
-0001d160: 2320 6469 6c61 7465 5069 7865 6c73 203d  # dilatePixels =
-0001d170: 2064 696c 6174 6550 6978 656c 732c 0d0a   dilatePixels,..
-0001d180: 2020 2020 2020 2320 636f 7272 6563 7449        # correctI
-0001d190: 6c6c 756d 696e 6174 696f 6e20 3d20 636f  llumination = co
+0001c4a0: 736b 203d 2061 7070 6c79 466d 6173 6b43  sk = applyFmaskC
+0001c4b0: 6c6f 7564 4d61 736b 2c0d 0a20 2020 2061  loudMask,..    a
+0001c4c0: 7070 6c79 5444 4f4d 203d 2061 7070 6c79  pplyTDOM = apply
+0001c4d0: 5444 4f4d 2c0d 0a20 2020 2061 7070 6c79  TDOM,..    apply
+0001c4e0: 466d 6173 6b43 6c6f 7564 5368 6164 6f77  FmaskCloudShadow
+0001c4f0: 4d61 736b 203d 2061 7070 6c79 466d 6173  Mask = applyFmas
+0001c500: 6b43 6c6f 7564 5368 6164 6f77 4d61 736b  kCloudShadowMask
+0001c510: 2c0d 0a20 2020 2061 7070 6c79 466d 6173  ,..    applyFmas
+0001c520: 6b53 6e6f 774d 6173 6b20 3d20 6170 706c  kSnowMask = appl
+0001c530: 7946 6d61 736b 536e 6f77 4d61 736b 2c0d  yFmaskSnowMask,.
+0001c540: 0a20 2020 2063 6c6f 7564 5363 6f72 6554  .    cloudScoreT
+0001c550: 6872 6573 6820 3d20 636c 6f75 6453 636f  hresh = cloudSco
+0001c560: 7265 5468 7265 7368 2c0d 0a20 2020 2070  reThresh,..    p
+0001c570: 6572 666f 726d 436c 6f75 6453 636f 7265  erformCloudScore
+0001c580: 4f66 6673 6574 203d 2070 6572 666f 726d  Offset = perform
+0001c590: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
+0001c5a0: 2c0d 0a20 2020 2063 6c6f 7564 5363 6f72  ,..    cloudScor
+0001c5b0: 6550 6374 6c20 3d20 636c 6f75 6453 636f  ePctl = cloudSco
+0001c5c0: 7265 5063 746c 2c0d 0a20 2020 207a 5363  rePctl,..    zSc
+0001c5d0: 6f72 6554 6872 6573 6820 3d20 7a53 636f  oreThresh = zSco
+0001c5e0: 7265 5468 7265 7368 2c0d 0a20 2020 2073  reThresh,..    s
+0001c5f0: 6861 646f 7753 756d 5468 7265 7368 203d  hadowSumThresh =
+0001c600: 2073 6861 646f 7753 756d 5468 7265 7368   shadowSumThresh
+0001c610: 2c0d 0a20 2020 2063 6f6e 7472 6163 7450  ,..    contractP
+0001c620: 6978 656c 7320 3d20 636f 6e74 7261 6374  ixels = contract
+0001c630: 5069 7865 6c73 2c0d 0a20 2020 2064 696c  Pixels,..    dil
+0001c640: 6174 6550 6978 656c 7320 3d20 6469 6c61  atePixels = dila
+0001c650: 7465 5069 7865 6c73 2c0d 0a20 2020 2072  tePixels,..    r
+0001c660: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
+0001c670: 7265 7361 6d70 6c65 4d65 7468 6f64 2c0d  resampleMethod,.
+0001c680: 0a20 2020 2068 6172 6d6f 6e69 7a65 4f4c  .    harmonizeOL
+0001c690: 4920 3d20 6861 726d 6f6e 697a 654f 4c49  I = harmonizeOLI
+0001c6a0: 2c0d 0a20 2020 2070 7265 436f 6d70 7574  ,..    preComput
+0001c6b0: 6564 436c 6f75 6453 636f 7265 4f66 6673  edCloudScoreOffs
+0001c6c0: 6574 203d 2070 7265 436f 6d70 7574 6564  et = preComputed
+0001c6d0: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
+0001c6e0: 2c0d 0a20 2020 2070 7265 436f 6d70 7574  ,..    preComput
+0001c6f0: 6564 5444 4f4d 4952 4d65 616e 203d 2070  edTDOMIRMean = p
+0001c700: 7265 436f 6d70 7574 6564 5444 4f4d 4952  reComputedTDOMIR
+0001c710: 4d65 616e 2c0d 0a20 2020 2070 7265 436f  Mean,..    preCo
+0001c720: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
+0001c730: 6576 203d 2070 7265 436f 6d70 7574 6564  ev = preComputed
+0001c740: 5444 4f4d 4952 5374 6444 6576 2c0d 0a20  TDOMIRStdDev,.. 
+0001c750: 2020 206c 616e 6473 6174 436f 6c6c 6563     landsatCollec
+0001c760: 7469 6f6e 5665 7273 696f 6e20 3d20 6c61  tionVersion = la
+0001c770: 6e64 7361 7443 6f6c 6c65 6374 696f 6e56  ndsatCollectionV
+0001c780: 6572 7369 6f6e 290d 0a0d 0a20 2023 4164  ersion)....  #Ad
+0001c790: 6420 7a65 6e69 7468 2061 6e64 2061 7a69  d zenith and azi
+0001c7a0: 6d75 7468 0d0a 2020 6966 2063 6f72 7265  muth..  if corre
+0001c7b0: 6374 496c 6c75 6d69 6e61 7469 6f6e 3a0d  ctIllumination:.
+0001c7c0: 0a20 2020 2070 7269 6e74 2827 4164 6469  .    print('Addi
+0001c7d0: 6e67 207a 656e 6974 6820 616e 6420 617a  ng zenith and az
+0001c7e0: 696d 7574 6820 666f 7220 7465 7272 6169  imuth for terrai
+0001c7f0: 6e20 636f 7272 6563 7469 6f6e 2729 0d0a  n correction')..
+0001c800: 2020 2020 6c73 203d 206c 732e 6d61 7028      ls = ls.map(
+0001c810: 6c61 6d62 6461 2069 6d67 3a20 6164 645a  lambda img: addZ
+0001c820: 656e 6974 6841 7a69 6d75 7468 2869 6d67  enithAzimuth(img
+0001c830: 2c20 746f 614f 7253 5229 290d 0a0d 0a20  , toaOrSR)).... 
+0001c840: 2023 4372 6561 7465 2063 6f6d 706f 7369   #Create composi
+0001c850: 7465 2074 696d 6520 7365 7269 6573 0d0a  te time series..
+0001c860: 2020 7473 203d 2063 6f6d 706f 7369 7465    ts = composite
+0001c870: 5469 6d65 5365 7269 6573 285c 0d0a 2020  TimeSeries(\..  
+0001c880: 2020 6c73 203d 206c 732c 0d0a 2020 2020    ls = ls,..    
+0001c890: 7374 6172 7459 6561 7220 3d20 7374 6172  startYear = star
+0001c8a0: 7459 6561 722c 0d0a 2020 2020 656e 6459  tYear,..    endY
+0001c8b0: 6561 7220 3d20 656e 6459 6561 722c 0d0a  ear = endYear,..
+0001c8c0: 2020 2020 7374 6172 744a 756c 6961 6e20      startJulian 
+0001c8d0: 3d20 7374 6172 744a 756c 6961 6e2c 0d0a  = startJulian,..
+0001c8e0: 2020 2020 656e 644a 756c 6961 6e20 3d20      endJulian = 
+0001c8f0: 656e 644a 756c 6961 6e2c 0d0a 2020 2020  endJulian,..    
+0001c900: 7469 6d65 6275 6666 6572 203d 2074 696d  timebuffer = tim
+0001c910: 6562 7566 6665 722c 0d0a 2020 2020 7765  ebuffer,..    we
+0001c920: 6967 6874 7320 3d20 7765 6967 6874 732c  ights = weights,
+0001c930: 0d0a 2020 2020 636f 6d70 6f73 6974 696e  ..    compositin
+0001c940: 674d 6574 686f 6420 3d20 636f 6d70 6f73  gMethod = compos
+0001c950: 6974 696e 674d 6574 686f 642c 0d0a 2020  itingMethod,..  
+0001c960: 2020 636f 6d70 6f73 6974 696e 6752 6564    compositingRed
+0001c970: 7563 6572 203d 2063 6f6d 706f 7369 7469  ucer = compositi
+0001c980: 6e67 5265 6475 6365 7229 0d0a 0d0a 2020  ngReducer)....  
+0001c990: 2320 436f 7272 6563 7420 696c 6c75 6d69  # Correct illumi
+0001c9a0: 6e61 7469 6f6e 0d0a 2020 6966 2063 6f72  nation..  if cor
+0001c9b0: 7265 6374 496c 6c75 6d69 6e61 7469 6f6e  rectIllumination
+0001c9c0: 3a0d 0a20 2020 2070 7269 6e74 2827 436f  :..    print('Co
+0001c9d0: 7272 6563 7469 6e67 2069 6c6c 756d 696e  rrecting illumin
+0001c9e0: 6174 696f 6e27 293b 0d0a 2020 2020 7473  ation');..    ts
+0001c9f0: 203d 2074 732e 6d61 7028 696c 6c75 6d69   = ts.map(illumi
+0001ca00: 6e61 7469 6f6e 436f 6e64 6974 696f 6e29  nationCondition)
+0001ca10: 2e6d 6170 286c 616d 6264 6120 696d 673a  .map(lambda img:
+0001ca20: 2069 6c6c 756d 696e 6174 696f 6e43 6f72   illuminationCor
+0001ca30: 7265 6374 696f 6e28 696d 672c 2063 6f72  rection(img, cor
+0001ca40: 7265 6374 5363 616c 652c 2073 7475 6479  rectScale, study
+0001ca50: 4172 6561 2929 0d0a 0d0a 2020 2345 7870  Area))....  #Exp
+0001ca60: 6f72 7420 636f 6d70 6f73 6974 6573 0d0a  ort composites..
+0001ca70: 2020 6966 2065 7870 6f72 7443 6f6d 706f    if exportCompo
+0001ca80: 7369 7465 733a 0d0a 2020 2020 6966 2063  sites:..    if c
+0001ca90: 6f6d 706f 7369 7469 6e67 4d65 7468 6f64  ompositingMethod
+0001caa0: 203d 3d20 276d 6564 6f69 6427 3a0d 0a20   == 'medoid':.. 
+0001cab0: 2020 2020 2065 7870 6f72 7442 616e 6473       exportBands
+0001cac0: 203d 205b 2762 6c75 6527 2c20 2767 7265   = ['blue', 'gre
+0001cad0: 656e 272c 2027 7265 6427 2c20 276e 6972  en', 'red', 'nir
+0001cae0: 272c 2027 7377 6972 3127 2c20 2773 7769  ', 'swir1', 'swi
+0001caf0: 7232 272c 2027 7465 6d70 272c 2027 636f  r2', 'temp', 'co
+0001cb00: 6d70 6f73 6974 654f 6273 436f 756e 7427  mpositeObsCount'
+0001cb10: 2c20 2773 656e 736f 7227 2c20 2779 6561  , 'sensor', 'yea
+0001cb20: 7227 2c20 276a 756c 6961 6e44 6179 275d  r', 'julianDay']
+0001cb30: 0d0a 2020 2020 2020 6e6f 6e44 6976 6964  ..      nonDivid
+0001cb40: 6542 616e 6473 203d 205b 2774 656d 7027  eBands = ['temp'
+0001cb50: 2c20 2763 6f6d 706f 7369 7465 4f62 7343  , 'compositeObsC
+0001cb60: 6f75 6e74 272c 2027 7365 6e73 6f72 272c  ount', 'sensor',
+0001cb70: 2027 7965 6172 272c 2027 6a75 6c69 616e   'year', 'julian
+0001cb80: 4461 7927 5d0d 0a20 2020 2065 6c73 653a  Day']..    else:
+0001cb90: 0d0a 2020 2020 2020 6578 706f 7274 4261  ..      exportBa
+0001cba0: 6e64 7320 3d20 5b27 626c 7565 272c 2027  nds = ['blue', '
+0001cbb0: 6772 6565 6e27 2c20 2772 6564 272c 2027  green', 'red', '
+0001cbc0: 6e69 7227 2c20 2773 7769 7231 272c 2027  nir', 'swir1', '
+0001cbd0: 7377 6972 3227 2c20 2774 656d 7027 2c20  swir2', 'temp', 
+0001cbe0: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
+0001cbf0: 6e74 275d 0d0a 2020 2020 2020 6e6f 6e44  nt']..      nonD
+0001cc00: 6976 6964 6542 616e 6473 203d 205b 2774  ivideBands = ['t
+0001cc10: 656d 7027 2c20 2763 6f6d 706f 7369 7465  emp', 'composite
+0001cc20: 4f62 7343 6f75 6e74 275d 0d0a 0d0a 2020  ObsCount']....  
+0001cc30: 2020 6578 706f 7274 436f 6d70 6f73 6974    exportComposit
+0001cc40: 6543 6f6c 6c65 6374 696f 6e28 5c0d 0a20  eCollection(\.. 
+0001cc50: 2020 2020 2063 6f6c 6c65 6374 696f 6e20       collection 
+0001cc60: 3d20 7473 2c0d 0a20 2020 2020 2065 7870  = ts,..      exp
+0001cc70: 6f72 7450 6174 6852 6f6f 7420 3d20 6578  ortPathRoot = ex
+0001cc80: 706f 7274 5061 7468 526f 6f74 2c0d 0a20  portPathRoot,.. 
+0001cc90: 2020 2020 206f 7574 7075 744e 616d 6520       outputName 
+0001cca0: 3d20 6f75 7470 7574 4e61 6d65 2c0d 0a20  = outputName,.. 
+0001ccb0: 2020 2020 206f 7269 6769 6e20 3d20 6f72       origin = or
+0001ccc0: 6967 696e 2c0d 0a20 2020 2020 2073 7475  igin,..      stu
+0001ccd0: 6479 4172 6561 203d 2073 7475 6479 4172  dyArea = studyAr
+0001cce0: 6561 2c0d 0a20 2020 2020 2063 7273 203d  ea,..      crs =
+0001ccf0: 2063 7273 2c0d 0a20 2020 2020 2074 7261   crs,..      tra
+0001cd00: 6e73 666f 726d 203d 2074 7261 6e73 666f  nsform = transfo
+0001cd10: 726d 2c0d 0a20 2020 2020 2073 6361 6c65  rm,..      scale
+0001cd20: 203d 2073 6361 6c65 2c0d 0a20 2020 2020   = scale,..     
+0001cd30: 2073 7461 7274 5965 6172 203d 2073 7461   startYear = sta
+0001cd40: 7274 5965 6172 2c0d 0a20 2020 2020 2065  rtYear,..      e
+0001cd50: 6e64 5965 6172 203d 2065 6e64 5965 6172  ndYear = endYear
+0001cd60: 2c0d 0a20 2020 2020 2073 7461 7274 4a75  ,..      startJu
+0001cd70: 6c69 616e 203d 2073 7461 7274 4a75 6c69  lian = startJuli
+0001cd80: 616e 2c0d 0a20 2020 2020 2065 6e64 4a75  an,..      endJu
+0001cd90: 6c69 616e 203d 2065 6e64 4a75 6c69 616e  lian = endJulian
+0001cda0: 2c0d 0a20 2020 2020 2063 6f6d 706f 7369  ,..      composi
+0001cdb0: 7469 6e67 4d65 7468 6f64 203d 2063 6f6d  tingMethod = com
+0001cdc0: 706f 7369 7469 6e67 4d65 7468 6f64 2c0d  positingMethod,.
+0001cdd0: 0a20 2020 2020 2074 696d 6562 7566 6665  .      timebuffe
+0001cde0: 7220 3d20 7469 6d65 6275 6666 6572 2c0d  r = timebuffer,.
+0001cdf0: 0a20 2020 2020 2074 6f61 4f72 5352 203d  .      toaOrSR =
+0001ce00: 2074 6f61 4f72 5352 2c0d 0a20 2020 2020   toaOrSR,..     
+0001ce10: 206e 6f6e 4469 7669 6465 4261 6e64 7320   nonDivideBands 
+0001ce20: 3d20 6e6f 6e44 6976 6964 6542 616e 6473  = nonDivideBands
+0001ce30: 2c0d 0a20 2020 2020 2065 7870 6f72 7442  ,..      exportB
+0001ce40: 616e 6473 203d 2065 7870 6f72 7442 616e  ands = exportBan
+0001ce50: 6473 2c0d 0a20 2020 2020 2023 2077 6569  ds,..      # wei
+0001ce60: 6768 7473 203d 2077 6569 6768 7473 2c0d  ghts = weights,.
+0001ce70: 0a20 2020 2020 2023 2064 6566 7269 6e67  .      # defring
+0001ce80: 654c 3520 3d20 4661 6c73 652c 0d0a 2020  eL5 = False,..  
+0001ce90: 2020 2020 2320 696e 636c 7564 6553 4c43      # includeSLC
+0001cea0: 4f66 664c 3720 3d20 696e 636c 7564 6553  OffL7 = includeS
+0001ceb0: 4c43 4f66 664c 372c 0d0a 2020 2020 2020  LCOffL7,..      
+0001cec0: 2320 636f 6e76 6572 7454 6f44 6169 6c79  # convertToDaily
+0001ced0: 4d6f 7361 6963 7320 3d20 274e 4127 2c0d  Mosaics = 'NA',.
+0001cee0: 0a20 2020 2020 2023 2061 7070 6c79 5141  .      # applyQA
+0001cef0: 4261 6e64 203d 2046 616c 7365 2c0d 0a20  Band = False,.. 
+0001cf00: 2020 2020 2023 2061 7070 6c79 436c 6f75       # applyClou
+0001cf10: 6453 636f 7265 203d 2061 7070 6c79 436c  dScore = applyCl
+0001cf20: 6f75 6453 636f 7265 2c0d 0a20 2020 2020  oudScore,..     
+0001cf30: 2023 2061 7070 6c79 466d 6173 6b43 6c6f   # applyFmaskClo
+0001cf40: 7564 4d61 736b 203d 2061 7070 6c79 466d  udMask = applyFm
+0001cf50: 6173 6b43 6c6f 7564 4d61 736b 2c0d 0a20  askCloudMask,.. 
+0001cf60: 2020 2020 2023 2061 7070 6c79 436c 6f75       # applyClou
+0001cf70: 6450 726f 6261 6269 6c69 7479 203d 2027  dProbability = '
+0001cf80: 4e41 272c 0d0a 2020 2020 2020 2320 6170  NA',..      # ap
+0001cf90: 706c 7954 444f 4d20 3d20 6170 706c 7954  plyTDOM = applyT
+0001cfa0: 444f 4d2c 0d0a 2020 2020 2020 2320 6170  DOM,..      # ap
+0001cfb0: 706c 7946 6d61 736b 436c 6f75 6453 6861  plyFmaskCloudSha
+0001cfc0: 646f 774d 6173 6b20 3d20 6170 706c 7946  dowMask = applyF
+0001cfd0: 6d61 736b 436c 6f75 6453 6861 646f 774d  maskCloudShadowM
+0001cfe0: 6173 6b2c 0d0a 2020 2020 2020 2320 6170  ask,..      # ap
+0001cff0: 706c 7946 6d61 736b 536e 6f77 4d61 736b  plyFmaskSnowMask
+0001d000: 203d 2061 7070 6c79 466d 6173 6b53 6e6f   = applyFmaskSno
+0001d010: 774d 6173 6b2c 0d0a 2020 2020 2020 2320  wMask,..      # 
+0001d020: 6170 706c 7953 6861 646f 7753 6869 6674  applyShadowShift
+0001d030: 203d 2027 4e41 272c 0d0a 2020 2020 2020   = 'NA',..      
+0001d040: 2320 636c 6f75 6448 6569 6768 7473 203d  # cloudHeights =
+0001d050: 2063 6c6f 7564 4865 6967 6874 732c 0d0a   cloudHeights,..
+0001d060: 2020 2020 2020 2320 636c 6f75 6453 636f        # cloudSco
+0001d070: 7265 5468 7265 7368 203d 2063 6c6f 7564  reThresh = cloud
+0001d080: 5363 6f72 6554 6872 6573 682c 0d0a 2020  ScoreThresh,..  
+0001d090: 2020 2020 2320 7065 7266 6f72 6d43 6c6f      # performClo
+0001d0a0: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
+0001d0b0: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
+0001d0c0: 654f 6666 7365 742c 0d0a 2020 2020 2020  eOffset,..      
+0001d0d0: 2320 636c 6f75 6453 636f 7265 5063 746c  # cloudScorePctl
+0001d0e0: 203d 2063 6c6f 7564 5363 6f72 6550 6374   = cloudScorePct
+0001d0f0: 6c2c 0d0a 2020 2020 2020 2320 7a53 636f  l,..      # zSco
+0001d100: 7265 5468 7265 7368 203d 207a 5363 6f72  reThresh = zScor
+0001d110: 6554 6872 6573 682c 0d0a 2020 2020 2020  eThresh,..      
+0001d120: 2320 7368 6164 6f77 5375 6d54 6872 6573  # shadowSumThres
+0001d130: 6820 3d20 7368 6164 6f77 5375 6d54 6872  h = shadowSumThr
+0001d140: 6573 682c 0d0a 2020 2020 2020 2320 636f  esh,..      # co
+0001d150: 6e74 7261 6374 5069 7865 6c73 203d 2063  ntractPixels = c
+0001d160: 6f6e 7472 6163 7450 6978 656c 732c 0d0a  ontractPixels,..
+0001d170: 2020 2020 2020 2320 6469 6c61 7465 5069        # dilatePi
+0001d180: 7865 6c73 203d 2064 696c 6174 6550 6978  xels = dilatePix
+0001d190: 656c 732c 0d0a 2020 2020 2020 2320 636f  els,..      # co
 0001d1a0: 7272 6563 7449 6c6c 756d 696e 6174 696f  rrectIlluminatio
-0001d1b0: 6e2c 0d0a 2020 2020 2020 2320 636f 7272  n,..      # corr
-0001d1c0: 6563 7453 6361 6c65 203d 2063 6f72 7265  ectScale = corre
-0001d1d0: 6374 5363 616c 652c 0d0a 2020 2020 2020  ctScale,..      
-0001d1e0: 2320 6e6f 6e44 6976 6964 6542 616e 6473  # nonDivideBands
-0001d1f0: 203d 206e 6f6e 4469 7669 6465 4261 6e64   = nonDivideBand
-0001d200: 732c 0d0a 2020 2020 2020 2320 6578 706f  s,..      # expo
-0001d210: 7274 4261 6e64 7320 3d20 6578 706f 7274  rtBands = export
-0001d220: 4261 6e64 732c 0d0a 2020 2020 2020 2320  Bands,..      # 
-0001d230: 7265 7361 6d70 6c65 4d65 7468 6f64 203d  resampleMethod =
-0001d240: 2072 6573 616d 706c 654d 6574 686f 642c   resampleMethod,
-0001d250: 0d0a 2020 2020 2020 2320 7275 6e43 6861  ..      # runCha
-0001d260: 7374 6169 6e48 6172 6d6f 6e69 7a61 7469  stainHarmonizati
-0001d270: 6f6e 203d 2027 4e41 272c 0d0a 2020 2020  on = 'NA',..    
-0001d280: 2020 6164 6469 7469 6f6e 616c 5072 6f70    additionalProp
-0001d290: 6572 7479 4469 6374 203d 2061 7267 7329  ertyDict = args)
-0001d2a0: 0d0a 0d0a 2020 6172 6773 5b27 7072 6f63  ....  args['proc
-0001d2b0: 6573 7365 6453 6365 6e65 7327 5d20 3d20  essedScenes'] = 
-0001d2c0: 6c73 0d0a 2020 6172 6773 5b27 7072 6f63  ls..  args['proc
-0001d2d0: 6573 7365 6443 6f6d 706f 7369 7465 7327  essedComposites'
-0001d2e0: 5d20 3d20 7473 0d0a 0d0a 2020 7265 7475  ] = ts....  retu
-0001d2f0: 726e 2061 7267 730d 0a0d 0a23 2323 2323  rn args....#####
-0001d300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d1b0: 6e20 3d20 636f 7272 6563 7449 6c6c 756d  n = correctIllum
+0001d1c0: 696e 6174 696f 6e2c 0d0a 2020 2020 2020  ination,..      
+0001d1d0: 2320 636f 7272 6563 7453 6361 6c65 203d  # correctScale =
+0001d1e0: 2063 6f72 7265 6374 5363 616c 652c 0d0a   correctScale,..
+0001d1f0: 2020 2020 2020 2320 6e6f 6e44 6976 6964        # nonDivid
+0001d200: 6542 616e 6473 203d 206e 6f6e 4469 7669  eBands = nonDivi
+0001d210: 6465 4261 6e64 732c 0d0a 2020 2020 2020  deBands,..      
+0001d220: 2320 6578 706f 7274 4261 6e64 7320 3d20  # exportBands = 
+0001d230: 6578 706f 7274 4261 6e64 732c 0d0a 2020  exportBands,..  
+0001d240: 2020 2020 2320 7265 7361 6d70 6c65 4d65      # resampleMe
+0001d250: 7468 6f64 203d 2072 6573 616d 706c 654d  thod = resampleM
+0001d260: 6574 686f 642c 0d0a 2020 2020 2020 2320  ethod,..      # 
+0001d270: 7275 6e43 6861 7374 6169 6e48 6172 6d6f  runChastainHarmo
+0001d280: 6e69 7a61 7469 6f6e 203d 2027 4e41 272c  nization = 'NA',
+0001d290: 0d0a 2020 2020 2020 6164 6469 7469 6f6e  ..      addition
+0001d2a0: 616c 5072 6f70 6572 7479 4469 6374 203d  alPropertyDict =
+0001d2b0: 2061 7267 732c 0d0a 2020 2020 2020 6f76   args,..      ov
+0001d2c0: 6572 7772 6974 6520 3d20 6f76 6572 7772  erwrite = overwr
+0001d2d0: 6974 6529 0d0a 0d0a 2020 6172 6773 5b27  ite)....  args['
+0001d2e0: 7072 6f63 6573 7365 6453 6365 6e65 7327  processedScenes'
+0001d2f0: 5d20 3d20 6c73 0d0a 2020 6172 6773 5b27  ] = ls..  args['
+0001d300: 7072 6f63 6573 7365 6443 6f6d 706f 7369  processedComposi
+0001d310: 7465 7327 5d20 3d20 7473 0d0a 0d0a 2020  tes'] = ts....  
+0001d320: 7265 7475 726e 2061 7267 730d 0a0d 0a23  return args....#
 0001d330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d340: 2323 2323 0d0a 2323 2323 2323 2323 2323  ####..##########
+0001d340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001d350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001d360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d380: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-0001d390: 0a23 5772 6170 7065 7220 6675 6e63 7469  .#Wrapper functi
-0001d3a0: 6f6e 2066 6f72 2067 6574 7469 6e67 204c  on for getting L
-0001d3b0: 616e 6473 6174 2069 6d61 6765 7279 0d0a  andsat imagery..
-0001d3c0: 6465 6620 6765 7450 726f 6365 7373 6564  def getProcessed
-0001d3d0: 4c61 6e64 7361 7453 6365 6e65 7328 0d0a  LandsatScenes(..
-0001d3e0: 2020 7374 7564 7941 7265 612c 0d0a 2020    studyArea,..  
-0001d3f0: 7374 6172 7459 6561 722c 0d0a 2020 656e  startYear,..  en
-0001d400: 6459 6561 722c 0d0a 2020 7374 6172 744a  dYear,..  startJ
-0001d410: 756c 6961 6e2c 0d0a 2020 656e 644a 756c  ulian,..  endJul
-0001d420: 6961 6e2c 0d0a 2020 746f 614f 7253 5220  ian,..  toaOrSR 
-0001d430: 3d20 2753 5227 2c0d 0a20 2069 6e63 6c75  = 'SR',..  inclu
-0001d440: 6465 534c 434f 6666 4c37 203d 2046 616c  deSLCOffL7 = Fal
-0001d450: 7365 2c0d 0a20 2064 6566 7269 6e67 654c  se,..  defringeL
-0001d460: 3520 3d20 4661 6c73 652c 0d0a 2020 6170  5 = False,..  ap
-0001d470: 706c 7943 6c6f 7564 5363 6f72 6520 3d20  plyCloudScore = 
-0001d480: 4661 6c73 652c 0d0a 2020 6170 706c 7946  False,..  applyF
-0001d490: 6d61 736b 436c 6f75 644d 6173 6b20 3d20  maskCloudMask = 
-0001d4a0: 5472 7565 2c0d 0a20 2061 7070 6c79 5444  True,..  applyTD
-0001d4b0: 4f4d 203d 2046 616c 7365 2c0d 0a20 2061  OM = False,..  a
-0001d4c0: 7070 6c79 466d 6173 6b43 6c6f 7564 5368  pplyFmaskCloudSh
-0001d4d0: 6164 6f77 4d61 736b 203d 2054 7275 652c  adowMask = True,
-0001d4e0: 0d0a 2020 6170 706c 7946 6d61 736b 536e  ..  applyFmaskSn
-0001d4f0: 6f77 4d61 736b 203d 2046 616c 7365 2c0d  owMask = False,.
-0001d500: 0a20 2063 6c6f 7564 5363 6f72 6554 6872  .  cloudScoreThr
-0001d510: 6573 6820 3d20 3130 2c0d 0a20 2070 6572  esh = 10,..  per
-0001d520: 666f 726d 436c 6f75 6453 636f 7265 4f66  formCloudScoreOf
-0001d530: 6673 6574 203d 2054 7275 652c 0d0a 2020  fset = True,..  
-0001d540: 636c 6f75 6453 636f 7265 5063 746c 203d  cloudScorePctl =
-0001d550: 2031 302c 0d0a 2020 7a53 636f 7265 5468   10,..  zScoreTh
-0001d560: 7265 7368 203d 202d 312c 0d0a 2020 7368  resh = -1,..  sh
-0001d570: 6164 6f77 5375 6d54 6872 6573 6820 3d20  adowSumThresh = 
-0001d580: 302e 3335 2c0d 0a20 2063 6f6e 7472 6163  0.35,..  contrac
-0001d590: 7450 6978 656c 7320 3d20 312e 352c 0d0a  tPixels = 1.5,..
-0001d5a0: 2020 6469 6c61 7465 5069 7865 6c73 203d    dilatePixels =
-0001d5b0: 2033 2e35 2c0d 0a20 2073 6861 646f 7753   3.5,..  shadowS
-0001d5c0: 756d 4261 6e64 7320 3d20 5b27 6e69 7227  umBands = ['nir'
-0001d5d0: 2c27 7377 6972 3127 5d2c 0d0a 2020 7265  ,'swir1'],..  re
-0001d5e0: 7361 6d70 6c65 4d65 7468 6f64 203d 2027  sampleMethod = '
-0001d5f0: 6e65 6172 272c 0d0a 2020 6861 726d 6f6e  near',..  harmon
-0001d600: 697a 654f 4c49 203d 2046 616c 7365 2c0d  izeOLI = False,.
-0001d610: 0a20 2070 7265 436f 6d70 7574 6564 436c  .  preComputedCl
-0001d620: 6f75 6453 636f 7265 4f66 6673 6574 203d  oudScoreOffset =
-0001d630: 204e 6f6e 652c 0d0a 2020 7072 6543 6f6d   None,..  preCom
-0001d640: 7075 7465 6454 444f 4d49 524d 6561 6e20  putedTDOMIRMean 
-0001d650: 3d20 4e6f 6e65 2c0d 0a20 2070 7265 436f  = None,..  preCo
-0001d660: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
-0001d670: 6576 203d 204e 6f6e 652c 0d0a 2020 6c61  ev = None,..  la
-0001d680: 6e64 7361 7443 6f6c 6c65 6374 696f 6e56  ndsatCollectionV
-0001d690: 6572 7369 6f6e 203d 2027 4332 2729 3a0d  ersion = 'C2'):.
-0001d6a0: 0a0d 0a20 206f 7269 6769 6e20 3d20 274c  ...  origin = 'L
-0001d6b0: 616e 6473 6174 270d 0a20 2074 6f61 4f72  andsat'..  toaOr
-0001d6c0: 5352 203d 2074 6f61 4f72 5352 2e75 7070  SR = toaOrSR.upp
-0001d6d0: 6572 2829 0d0a 2020 6966 2074 6f61 4f72  er()..  if toaOr
-0001d6e0: 5352 2e6c 6f77 6572 2829 203d 3d20 2774  SR.lower() == 't
-0001d6f0: 6f61 2720 616e 6420 6c61 6e64 7361 7443  oa' and landsatC
-0001d700: 6f6c 6c65 6374 696f 6e56 6572 7369 6f6e  ollectionVersion
-0001d710: 2e6c 6f77 6572 2829 203d 3d20 2763 3127  .lower() == 'c1'
-0001d720: 2061 6e64 2028 6170 706c 7946 6d61 736b   and (applyFmask
-0001d730: 436c 6f75 644d 6173 6b20 6f72 2061 7070  CloudMask or app
-0001d740: 6c79 466d 6173 6b43 6c6f 7564 5368 6164  lyFmaskCloudShad
-0001d750: 6f77 4d61 736b 2020 6f72 2061 7070 6c79  owMask  or apply
-0001d760: 466d 6173 6b53 6e6f 774d 6173 6b20 293a  FmaskSnowMask ):
-0001d770: 0d0a 2020 2020 6164 6450 6978 656c 5141  ..    addPixelQA
-0001d780: 203d 2054 7275 650d 0a20 2065 6c73 653a   = True..  else:
-0001d790: 0d0a 2020 2020 6164 6450 6978 656c 5141  ..    addPixelQA
-0001d7a0: 203d 2046 616c 7365 0d0a 0d0a 2020 2350   = False....  #P
-0001d7b0: 7265 7061 7265 2064 6174 6573 0d0a 2020  repare dates..  
-0001d7c0: 2357 7261 7020 7468 6520 6461 7465 7320  #Wrap the dates 
-0001d7d0: 6966 206e 6565 6465 640d 0a20 2077 7261  if needed..  wra
-0001d7e0: 704f 6666 7365 7420 3d20 300d 0a20 2069  pOffset = 0..  i
-0001d7f0: 6620 7374 6172 744a 756c 6961 6e20 3e20  f startJulian > 
-0001d800: 656e 644a 756c 6961 6e3a 0d0a 2020 2020  endJulian:..    
-0001d810: 7772 6170 4f66 6673 6574 203d 2033 3635  wrapOffset = 365
-0001d820: 0d0a 2020 7374 6172 7444 6174 6520 3d20  ..  startDate = 
-0001d830: 6565 2e44 6174 652e 6672 6f6d 594d 4428  ee.Date.fromYMD(
-0001d840: 7374 6172 7459 6561 722c 312c 3129 2e61  startYear,1,1).a
-0001d850: 6476 616e 6365 2873 7461 7274 4a75 6c69  dvance(startJuli
-0001d860: 616e 2d31 2c27 6461 7927 290d 0a20 2065  an-1,'day')..  e
-0001d870: 6e64 4461 7465 203d 2065 652e 4461 7465  ndDate = ee.Date
-0001d880: 2e66 726f 6d59 4d44 2865 6e64 5965 6172  .fromYMD(endYear
-0001d890: 2c31 2c31 292e 6164 7661 6e63 6528 656e  ,1,1).advance(en
-0001d8a0: 644a 756c 6961 6e2d 312b 7772 6170 4f66  dJulian-1+wrapOf
-0001d8b0: 6673 6574 2c27 6461 7927 290d 0a0d 0a20  fset,'day').... 
-0001d8c0: 2061 7267 7320 3d20 666f 726d 6174 4172   args = formatAr
-0001d8d0: 6773 286c 6f63 616c 7328 2929 0d0a 2020  gs(locals())..  
-0001d8e0: 6966 2027 6172 6773 2720 696e 2061 7267  if 'args' in arg
-0001d8f0: 732e 6b65 7973 2829 3a0d 0a20 2020 2064  s.keys():..    d
-0001d900: 656c 2061 7267 735b 2761 7267 7327 5d0d  el args['args'].
-0001d910: 0a0d 0a20 2070 7269 6e74 2827 4765 7420  ...  print('Get 
-0001d920: 5072 6f63 6573 7365 6420 4c61 6e64 7361  Processed Landsa
-0001d930: 743a 2027 290d 0a20 2023 2070 7269 6e74  t: ')..  # print
-0001d940: 2827 5374 6172 7420 6461 7465 3a27 2c20  ('Start date:', 
-0001d950: 7374 6172 7444 6174 652e 666f 726d 6174  startDate.format
-0001d960: 2827 4d4d 4d20 6464 2079 7979 7927 292e  ('MMM dd yyyy').
-0001d970: 6765 7449 6e66 6f28 292c 272c 2045 6e64  getInfo(),', End
-0001d980: 2064 6174 653a 272c 2065 6e64 4461 7465   date:', endDate
-0001d990: 2e66 6f72 6d61 7428 274d 4d4d 2064 6420  .format('MMM dd 
-0001d9a0: 7979 7979 2729 2e67 6574 496e 666f 2829  yyyy').getInfo()
-0001d9b0: 290d 0a20 2023 2066 6f72 2061 7267 2069  )..  # for arg i
-0001d9c0: 6e20 6172 6773 2e6b 6579 7328 293a 0d0a  n args.keys():..
-0001d9d0: 2020 2320 2020 7072 696e 7428 6172 672c    #   print(arg,
-0001d9e0: 2027 3a20 272c 2061 7267 735b 6172 675d   ': ', args[arg]
-0001d9f0: 290d 0a0d 0a20 2023 4765 7420 4c61 6e64  )....  #Get Land
-0001da00: 7361 7420 696d 6167 6520 636f 6c6c 6563  sat image collec
-0001da10: 7469 6f6e 0d0a 2020 6c73 203d 2067 6574  tion..  ls = get
-0001da20: 4c61 6e64 7361 7428 5c0d 0a20 2020 2073  Landsat(\..    s
-0001da30: 7475 6479 4172 6561 203d 2073 7475 6479  tudyArea = study
-0001da40: 4172 6561 2c0d 0a20 2020 2073 7461 7274  Area,..    start
-0001da50: 4461 7465 203d 2073 7461 7274 4461 7465  Date = startDate
-0001da60: 2c0d 0a20 2020 2065 6e64 4461 7465 203d  ,..    endDate =
-0001da70: 2065 6e64 4461 7465 2c0d 0a20 2020 2073   endDate,..    s
-0001da80: 7461 7274 4a75 6c69 616e 203d 2073 7461  tartJulian = sta
-0001da90: 7274 4a75 6c69 616e 2c0d 0a20 2020 2065  rtJulian,..    e
-0001daa0: 6e64 4a75 6c69 616e 203d 2065 6e64 4a75  ndJulian = endJu
-0001dab0: 6c69 616e 2c0d 0a20 2020 2074 6f61 4f72  lian,..    toaOr
-0001dac0: 5352 203d 2074 6f61 4f72 5352 2c0d 0a20  SR = toaOrSR,.. 
-0001dad0: 2020 2069 6e63 6c75 6465 534c 434f 6666     includeSLCOff
-0001dae0: 4c37 203d 2069 6e63 6c75 6465 534c 434f  L7 = includeSLCO
-0001daf0: 6666 4c37 2c0d 0a20 2020 2064 6566 7269  ffL7,..    defri
-0001db00: 6e67 654c 3520 3d20 6465 6672 696e 6765  ngeL5 = defringe
-0001db10: 4c35 2c0d 0a20 2020 2061 6464 5069 7865  L5,..    addPixe
-0001db20: 6c51 4120 3d20 6164 6450 6978 656c 5141  lQA = addPixelQA
-0001db30: 2c0d 0a20 2020 2072 6573 616d 706c 654d  ,..    resampleM
-0001db40: 6574 686f 6420 3d20 7265 7361 6d70 6c65  ethod = resample
-0001db50: 4d65 7468 6f64 2c0d 0a20 2020 206c 616e  Method,..    lan
-0001db60: 6473 6174 436f 6c6c 6563 7469 6f6e 5665  dsatCollectionVe
-0001db70: 7273 696f 6e20 3d20 6c61 6e64 7361 7443  rsion = landsatC
-0001db80: 6f6c 6c65 6374 696f 6e56 6572 7369 6f6e  ollectionVersion
-0001db90: 290d 0a0d 0a20 2023 4170 706c 7920 7265  )....  #Apply re
-0001dba0: 6c65 7661 6e74 2063 6c6f 7564 206d 6173  levant cloud mas
-0001dbb0: 6b69 6e67 206d 6574 686f 6473 0d0a 2020  king methods..  
-0001dbc0: 6966 2061 7070 6c79 436c 6f75 6453 636f  if applyCloudSco
-0001dbd0: 7265 3a0d 0a20 2020 2070 7269 6e74 2827  re:..    print('
-0001dbe0: 4170 706c 7969 6e67 2043 6c6f 7564 2053  Applying Cloud S
-0001dbf0: 636f 7265 2729 0d0a 2020 2020 6c73 203d  core')..    ls =
-0001dc00: 2061 7070 6c79 436c 6f75 6453 636f 7265   applyCloudScore
-0001dc10: 416c 676f 7269 7468 6d28 5c0d 0a20 2020  Algorithm(\..   
-0001dc20: 2020 2063 6f6c 6c65 6374 696f 6e20 3d20     collection = 
-0001dc30: 6c73 2c0d 0a20 2020 2020 2063 6c6f 7564  ls,..      cloud
-0001dc40: 5363 6f72 6546 756e 6374 696f 6e20 3d20  ScoreFunction = 
-0001dc50: 6c61 6e64 7361 7443 6c6f 7564 5363 6f72  landsatCloudScor
-0001dc60: 652c 0d0a 2020 2020 2020 636c 6f75 6453  e,..      cloudS
-0001dc70: 636f 7265 5468 7265 7368 203d 2063 6c6f  coreThresh = clo
-0001dc80: 7564 5363 6f72 6554 6872 6573 682c 0d0a  udScoreThresh,..
-0001dc90: 2020 2020 2020 636c 6f75 6453 636f 7265        cloudScore
-0001dca0: 5063 746c 203d 2063 6c6f 7564 5363 6f72  Pctl = cloudScor
-0001dcb0: 6550 6374 6c2c 0d0a 2020 2020 2020 636f  ePctl,..      co
-0001dcc0: 6e74 7261 6374 5069 7865 6c73 203d 2063  ntractPixels = c
-0001dcd0: 6f6e 7472 6163 7450 6978 656c 732c 0d0a  ontractPixels,..
-0001dce0: 2020 2020 2020 6469 6c61 7465 5069 7865        dilatePixe
-0001dcf0: 6c73 203d 2064 696c 6174 6550 6978 656c  ls = dilatePixel
-0001dd00: 732c 0d0a 2020 2020 2020 7065 7266 6f72  s,..      perfor
-0001dd10: 6d43 6c6f 7564 5363 6f72 654f 6666 7365  mCloudScoreOffse
-0001dd20: 7420 3d20 7065 7266 6f72 6d43 6c6f 7564  t = performCloud
-0001dd30: 5363 6f72 654f 6666 7365 742c 0d0a 2020  ScoreOffset,..  
-0001dd40: 2020 2020 7072 6543 6f6d 7075 7465 6443      preComputedC
-0001dd50: 6c6f 7564 5363 6f72 654f 6666 7365 7420  loudScoreOffset 
-0001dd60: 3d20 7072 6543 6f6d 7075 7465 6443 6c6f  = preComputedClo
-0001dd70: 7564 5363 6f72 654f 6666 7365 7429 0d0a  udScoreOffset)..
-0001dd80: 0d0a 2020 6966 2061 7070 6c79 466d 6173  ..  if applyFmas
-0001dd90: 6b43 6c6f 7564 4d61 736b 3a0d 0a20 2020  kCloudMask:..   
-0001dda0: 2070 7269 6e74 2827 4170 706c 7969 6e67   print('Applying
-0001ddb0: 2046 6d61 736b 2043 6c6f 7564 204d 6173   Fmask Cloud Mas
-0001ddc0: 6b27 290d 0a20 2020 206c 7320 3d20 6c73  k')..    ls = ls
-0001ddd0: 2e6d 6170 286c 616d 6264 6120 696d 673a  .map(lambda img:
-0001dde0: 2061 7070 6c79 4269 744d 6173 6b28 696d   applyBitMask(im
-0001ddf0: 672c 666d 6173 6b42 6974 4469 6374 5b6c  g,fmaskBitDict[l
-0001de00: 616e 6473 6174 436f 6c6c 6563 7469 6f6e  andsatCollection
-0001de10: 5665 7273 696f 6e5d 5b27 636c 6f75 6427  Version]['cloud'
-0001de20: 5d2c 6c61 6e64 7361 7446 6d61 736b 4261  ],landsatFmaskBa
-0001de30: 6e64 4e61 6d65 4469 6374 5b6c 616e 6473  ndNameDict[lands
-0001de40: 6174 436f 6c6c 6563 7469 6f6e 5665 7273  atCollectionVers
-0001de50: 696f 6e5d 2929 0d0a 0d0a 2020 6966 2061  ion]))....  if a
-0001de60: 7070 6c79 5444 4f4d 3a0d 0a20 2020 2070  pplyTDOM:..    p
-0001de70: 7269 6e74 2827 4170 706c 7969 6e67 2054  rint('Applying T
-0001de80: 444f 4d20 5368 6164 6f77 204d 6173 6b27  DOM Shadow Mask'
-0001de90: 290d 0a20 2020 206c 7320 3d20 7369 6d70  )..    ls = simp
-0001dea0: 6c65 5444 4f4d 3228 5c0d 0a20 2020 2020  leTDOM2(\..     
-0001deb0: 2063 6f6c 6c65 6374 696f 6e20 3d20 6c73   collection = ls
-0001dec0: 2c0d 0a20 2020 2020 207a 5363 6f72 6554  ,..      zScoreT
-0001ded0: 6872 6573 6820 3d20 7a53 636f 7265 5468  hresh = zScoreTh
-0001dee0: 7265 7368 2c0d 0a20 2020 2020 2073 6861  resh,..      sha
-0001def0: 646f 7753 756d 5468 7265 7368 203d 2073  dowSumThresh = s
-0001df00: 6861 646f 7753 756d 5468 7265 7368 2c0d  hadowSumThresh,.
-0001df10: 0a20 2020 2020 2063 6f6e 7472 6163 7450  .      contractP
-0001df20: 6978 656c 7320 3d20 636f 6e74 7261 6374  ixels = contract
-0001df30: 5069 7865 6c73 2c0d 0a20 2020 2020 2064  Pixels,..      d
-0001df40: 696c 6174 6550 6978 656c 7320 3d20 6469  ilatePixels = di
-0001df50: 6c61 7465 5069 7865 6c73 2c0d 0a20 2020  latePixels,..   
-0001df60: 2020 2073 6861 646f 7753 756d 4261 6e64     shadowSumBand
-0001df70: 7320 3d20 5b27 6e69 7227 2c27 7377 6972  s = ['nir','swir
-0001df80: 3127 5d2c 0d0a 2020 2020 2020 7072 6543  1'],..      preC
-0001df90: 6f6d 7075 7465 6454 444f 4d49 524d 6561  omputedTDOMIRMea
-0001dfa0: 6e20 3d20 7072 6543 6f6d 7075 7465 6454  n = preComputedT
-0001dfb0: 444f 4d49 524d 6561 6e2c 0d0a 2020 2020  DOMIRMean,..    
-0001dfc0: 2020 7072 6543 6f6d 7075 7465 6454 444f    preComputedTDO
-0001dfd0: 4d49 5253 7464 4465 7620 3d20 7072 6543  MIRStdDev = preC
-0001dfe0: 6f6d 7075 7465 6454 444f 4d49 5253 7464  omputedTDOMIRStd
-0001dff0: 4465 7629 0d0a 0d0a 2020 6966 2061 7070  Dev)....  if app
-0001e000: 6c79 466d 6173 6b43 6c6f 7564 5368 6164  lyFmaskCloudShad
-0001e010: 6f77 4d61 736b 3a0d 0a20 2020 2070 7269  owMask:..    pri
-0001e020: 6e74 2827 4170 706c 7969 6e67 2046 6d61  nt('Applying Fma
-0001e030: 736b 2053 6861 646f 7720 4d61 736b 2729  sk Shadow Mask')
-0001e040: 0d0a 2020 2020 6c73 203d 206c 732e 6d61  ..    ls = ls.ma
-0001e050: 7028 6c61 6d62 6461 2069 6d67 3a20 6170  p(lambda img: ap
-0001e060: 706c 7942 6974 4d61 736b 2869 6d67 2c66  plyBitMask(img,f
-0001e070: 6d61 736b 4269 7444 6963 745b 6c61 6e64  maskBitDict[land
-0001e080: 7361 7443 6f6c 6c65 6374 696f 6e56 6572  satCollectionVer
-0001e090: 7369 6f6e 5d5b 2773 6861 646f 7727 5d2c  sion]['shadow'],
-0001e0a0: 6c61 6e64 7361 7446 6d61 736b 4261 6e64  landsatFmaskBand
-0001e0b0: 4e61 6d65 4469 6374 5b6c 616e 6473 6174  NameDict[landsat
-0001e0c0: 436f 6c6c 6563 7469 6f6e 5665 7273 696f  CollectionVersio
-0001e0d0: 6e5d 2929 0d0a 0d0a 0d0a 2020 6966 2061  n]))......  if a
-0001e0e0: 7070 6c79 466d 6173 6b53 6e6f 774d 6173  pplyFmaskSnowMas
-0001e0f0: 6b3a 0d0a 2020 2020 7072 696e 7428 2741  k:..    print('A
-0001e100: 7070 6c79 696e 6720 466d 6173 6b20 736e  pplying Fmask sn
-0001e110: 6f77 206d 6173 6b27 290d 0a20 2020 206c  ow mask')..    l
-0001e120: 7320 3d20 6c73 2e6d 6170 286c 616d 6264  s = ls.map(lambd
-0001e130: 6120 696d 673a 2061 7070 6c79 4269 744d  a img: applyBitM
-0001e140: 6173 6b28 696d 672c 666d 6173 6b42 6974  ask(img,fmaskBit
-0001e150: 4469 6374 5b6c 616e 6473 6174 436f 6c6c  Dict[landsatColl
-0001e160: 6563 7469 6f6e 5665 7273 696f 6e5d 5b27  ectionVersion]['
-0001e170: 736e 6f77 275d 2c6c 616e 6473 6174 466d  snow'],landsatFm
-0001e180: 6173 6b42 616e 644e 616d 6544 6963 745b  askBandNameDict[
-0001e190: 6c61 6e64 7361 7443 6f6c 6c65 6374 696f  landsatCollectio
-0001e1a0: 6e56 6572 7369 6f6e 5d29 290d 0a0d 0a0d  nVersion])).....
-0001e1b0: 0a20 2023 2041 6464 2063 6f6d 6d6f 6e20  .  # Add common 
-0001e1c0: 696e 6469 6365 730d 0a20 206c 7320 3d20  indices..  ls = 
-0001e1d0: 6c73 2e6d 6170 2873 696d 706c 6541 6464  ls.map(simpleAdd
-0001e1e0: 496e 6469 6365 7329 5c0d 0a20 2020 2020  Indices)\..     
-0001e1f0: 2020 2020 202e 6d61 7028 6765 7454 6173       .map(getTas
-0001e200: 7365 6c65 6443 6170 295c 0d0a 2020 2020  seledCap)\..    
-0001e210: 2020 2020 2020 2e6d 6170 2873 696d 706c        .map(simpl
-0001e220: 6541 6464 5443 416e 676c 6573 290d 0a0d  eAddTCAngles)...
-0001e230: 0a20 2023 2041 6464 2053 656e 736f 7220  .  # Add Sensor 
-0001e240: 4261 6e64 0d0a 2020 6c73 203d 206c 732e  Band..  ls = ls.
-0001e250: 6d61 7028 6c61 6d62 6461 2069 6d67 3a20  map(lambda img: 
-0001e260: 6164 6453 656e 736f 7242 616e 6428 696d  addSensorBand(im
-0001e270: 672c 206c 616e 6473 6174 436f 6c6c 6563  g, landsatCollec
-0001e280: 7469 6f6e 5665 7273 696f 6e2b 275f 6c61  tionVersion+'_la
-0001e290: 6e64 7361 7427 2c20 746f 614f 7253 5229  ndsat', toaOrSR)
-0001e2a0: 290d 0a0d 0a20 2072 6574 7572 6e20 6c73  )....  return ls
-0001e2b0: 2e73 6574 2861 7267 7329 0d0a 0d0a 2323  .set(args)....##
-0001e2c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e2d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e2e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e2f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e300: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
+0001d370: 2323 2323 2323 2323 0d0a 2323 2323 2323  ########..######
+0001d380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d3a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d3b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d3c0: 2323 230d 0a23 5772 6170 7065 7220 6675  ###..#Wrapper fu
+0001d3d0: 6e63 7469 6f6e 2066 6f72 2067 6574 7469  nction for getti
+0001d3e0: 6e67 204c 616e 6473 6174 2069 6d61 6765  ng Landsat image
+0001d3f0: 7279 0d0a 6465 6620 6765 7450 726f 6365  ry..def getProce
+0001d400: 7373 6564 4c61 6e64 7361 7453 6365 6e65  ssedLandsatScene
+0001d410: 7328 0d0a 2020 7374 7564 7941 7265 612c  s(..  studyArea,
+0001d420: 0d0a 2020 7374 6172 7459 6561 722c 0d0a  ..  startYear,..
+0001d430: 2020 656e 6459 6561 722c 0d0a 2020 7374    endYear,..  st
+0001d440: 6172 744a 756c 6961 6e2c 0d0a 2020 656e  artJulian,..  en
+0001d450: 644a 756c 6961 6e2c 0d0a 2020 746f 614f  dJulian,..  toaO
+0001d460: 7253 5220 3d20 2753 5227 2c0d 0a20 2069  rSR = 'SR',..  i
+0001d470: 6e63 6c75 6465 534c 434f 6666 4c37 203d  ncludeSLCOffL7 =
+0001d480: 2046 616c 7365 2c0d 0a20 2064 6566 7269   False,..  defri
+0001d490: 6e67 654c 3520 3d20 4661 6c73 652c 0d0a  ngeL5 = False,..
+0001d4a0: 2020 6170 706c 7943 6c6f 7564 5363 6f72    applyCloudScor
+0001d4b0: 6520 3d20 4661 6c73 652c 0d0a 2020 6170  e = False,..  ap
+0001d4c0: 706c 7946 6d61 736b 436c 6f75 644d 6173  plyFmaskCloudMas
+0001d4d0: 6b20 3d20 5472 7565 2c0d 0a20 2061 7070  k = True,..  app
+0001d4e0: 6c79 5444 4f4d 203d 2046 616c 7365 2c0d  lyTDOM = False,.
+0001d4f0: 0a20 2061 7070 6c79 466d 6173 6b43 6c6f  .  applyFmaskClo
+0001d500: 7564 5368 6164 6f77 4d61 736b 203d 2054  udShadowMask = T
+0001d510: 7275 652c 0d0a 2020 6170 706c 7946 6d61  rue,..  applyFma
+0001d520: 736b 536e 6f77 4d61 736b 203d 2046 616c  skSnowMask = Fal
+0001d530: 7365 2c0d 0a20 2063 6c6f 7564 5363 6f72  se,..  cloudScor
+0001d540: 6554 6872 6573 6820 3d20 3130 2c0d 0a20  eThresh = 10,.. 
+0001d550: 2070 6572 666f 726d 436c 6f75 6453 636f   performCloudSco
+0001d560: 7265 4f66 6673 6574 203d 2054 7275 652c  reOffset = True,
+0001d570: 0d0a 2020 636c 6f75 6453 636f 7265 5063  ..  cloudScorePc
+0001d580: 746c 203d 2031 302c 0d0a 2020 7a53 636f  tl = 10,..  zSco
+0001d590: 7265 5468 7265 7368 203d 202d 312c 0d0a  reThresh = -1,..
+0001d5a0: 2020 7368 6164 6f77 5375 6d54 6872 6573    shadowSumThres
+0001d5b0: 6820 3d20 302e 3335 2c0d 0a20 2063 6f6e  h = 0.35,..  con
+0001d5c0: 7472 6163 7450 6978 656c 7320 3d20 312e  tractPixels = 1.
+0001d5d0: 352c 0d0a 2020 6469 6c61 7465 5069 7865  5,..  dilatePixe
+0001d5e0: 6c73 203d 2033 2e35 2c0d 0a20 2073 6861  ls = 3.5,..  sha
+0001d5f0: 646f 7753 756d 4261 6e64 7320 3d20 5b27  dowSumBands = ['
+0001d600: 6e69 7227 2c27 7377 6972 3127 5d2c 0d0a  nir','swir1'],..
+0001d610: 2020 7265 7361 6d70 6c65 4d65 7468 6f64    resampleMethod
+0001d620: 203d 2027 6e65 6172 272c 0d0a 2020 6861   = 'near',..  ha
+0001d630: 726d 6f6e 697a 654f 4c49 203d 2046 616c  rmonizeOLI = Fal
+0001d640: 7365 2c0d 0a20 2070 7265 436f 6d70 7574  se,..  preComput
+0001d650: 6564 436c 6f75 6453 636f 7265 4f66 6673  edCloudScoreOffs
+0001d660: 6574 203d 204e 6f6e 652c 0d0a 2020 7072  et = None,..  pr
+0001d670: 6543 6f6d 7075 7465 6454 444f 4d49 524d  eComputedTDOMIRM
+0001d680: 6561 6e20 3d20 4e6f 6e65 2c0d 0a20 2070  ean = None,..  p
+0001d690: 7265 436f 6d70 7574 6564 5444 4f4d 4952  reComputedTDOMIR
+0001d6a0: 5374 6444 6576 203d 204e 6f6e 652c 0d0a  StdDev = None,..
+0001d6b0: 2020 6c61 6e64 7361 7443 6f6c 6c65 6374    landsatCollect
+0001d6c0: 696f 6e56 6572 7369 6f6e 203d 2027 4332  ionVersion = 'C2
+0001d6d0: 2729 3a0d 0a0d 0a20 206f 7269 6769 6e20  '):....  origin 
+0001d6e0: 3d20 274c 616e 6473 6174 270d 0a20 2074  = 'Landsat'..  t
+0001d6f0: 6f61 4f72 5352 203d 2074 6f61 4f72 5352  oaOrSR = toaOrSR
+0001d700: 2e75 7070 6572 2829 0d0a 2020 6966 2074  .upper()..  if t
+0001d710: 6f61 4f72 5352 2e6c 6f77 6572 2829 203d  oaOrSR.lower() =
+0001d720: 3d20 2774 6f61 2720 616e 6420 6c61 6e64  = 'toa' and land
+0001d730: 7361 7443 6f6c 6c65 6374 696f 6e56 6572  satCollectionVer
+0001d740: 7369 6f6e 2e6c 6f77 6572 2829 203d 3d20  sion.lower() == 
+0001d750: 2763 3127 2061 6e64 2028 6170 706c 7946  'c1' and (applyF
+0001d760: 6d61 736b 436c 6f75 644d 6173 6b20 6f72  maskCloudMask or
+0001d770: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
+0001d780: 5368 6164 6f77 4d61 736b 2020 6f72 2061  ShadowMask  or a
+0001d790: 7070 6c79 466d 6173 6b53 6e6f 774d 6173  pplyFmaskSnowMas
+0001d7a0: 6b20 293a 0d0a 2020 2020 6164 6450 6978  k ):..    addPix
+0001d7b0: 656c 5141 203d 2054 7275 650d 0a20 2065  elQA = True..  e
+0001d7c0: 6c73 653a 0d0a 2020 2020 6164 6450 6978  lse:..    addPix
+0001d7d0: 656c 5141 203d 2046 616c 7365 0d0a 0d0a  elQA = False....
+0001d7e0: 2020 2350 7265 7061 7265 2064 6174 6573    #Prepare dates
+0001d7f0: 0d0a 2020 2357 7261 7020 7468 6520 6461  ..  #Wrap the da
+0001d800: 7465 7320 6966 206e 6565 6465 640d 0a20  tes if needed.. 
+0001d810: 2077 7261 704f 6666 7365 7420 3d20 300d   wrapOffset = 0.
+0001d820: 0a20 2069 6620 7374 6172 744a 756c 6961  .  if startJulia
+0001d830: 6e20 3e20 656e 644a 756c 6961 6e3a 0d0a  n > endJulian:..
+0001d840: 2020 2020 7772 6170 4f66 6673 6574 203d      wrapOffset =
+0001d850: 2033 3635 0d0a 2020 7374 6172 7444 6174   365..  startDat
+0001d860: 6520 3d20 6565 2e44 6174 652e 6672 6f6d  e = ee.Date.from
+0001d870: 594d 4428 7374 6172 7459 6561 722c 312c  YMD(startYear,1,
+0001d880: 3129 2e61 6476 616e 6365 2873 7461 7274  1).advance(start
+0001d890: 4a75 6c69 616e 2d31 2c27 6461 7927 290d  Julian-1,'day').
+0001d8a0: 0a20 2065 6e64 4461 7465 203d 2065 652e  .  endDate = ee.
+0001d8b0: 4461 7465 2e66 726f 6d59 4d44 2865 6e64  Date.fromYMD(end
+0001d8c0: 5965 6172 2c31 2c31 292e 6164 7661 6e63  Year,1,1).advanc
+0001d8d0: 6528 656e 644a 756c 6961 6e2d 312b 7772  e(endJulian-1+wr
+0001d8e0: 6170 4f66 6673 6574 2c27 6461 7927 290d  apOffset,'day').
+0001d8f0: 0a0d 0a20 2061 7267 7320 3d20 666f 726d  ...  args = form
+0001d900: 6174 4172 6773 286c 6f63 616c 7328 2929  atArgs(locals())
+0001d910: 0d0a 2020 6966 2027 6172 6773 2720 696e  ..  if 'args' in
+0001d920: 2061 7267 732e 6b65 7973 2829 3a0d 0a20   args.keys():.. 
+0001d930: 2020 2064 656c 2061 7267 735b 2761 7267     del args['arg
+0001d940: 7327 5d0d 0a0d 0a20 2070 7269 6e74 2827  s']....  print('
+0001d950: 4765 7420 5072 6f63 6573 7365 6420 4c61  Get Processed La
+0001d960: 6e64 7361 743a 2027 290d 0a20 2023 2070  ndsat: ')..  # p
+0001d970: 7269 6e74 2827 5374 6172 7420 6461 7465  rint('Start date
+0001d980: 3a27 2c20 7374 6172 7444 6174 652e 666f  :', startDate.fo
+0001d990: 726d 6174 2827 4d4d 4d20 6464 2079 7979  rmat('MMM dd yyy
+0001d9a0: 7927 292e 6765 7449 6e66 6f28 292c 272c  y').getInfo(),',
+0001d9b0: 2045 6e64 2064 6174 653a 272c 2065 6e64   End date:', end
+0001d9c0: 4461 7465 2e66 6f72 6d61 7428 274d 4d4d  Date.format('MMM
+0001d9d0: 2064 6420 7979 7979 2729 2e67 6574 496e   dd yyyy').getIn
+0001d9e0: 666f 2829 290d 0a20 2023 2066 6f72 2061  fo())..  # for a
+0001d9f0: 7267 2069 6e20 6172 6773 2e6b 6579 7328  rg in args.keys(
+0001da00: 293a 0d0a 2020 2320 2020 7072 696e 7428  ):..  #   print(
+0001da10: 6172 672c 2027 3a20 272c 2061 7267 735b  arg, ': ', args[
+0001da20: 6172 675d 290d 0a0d 0a20 2023 4765 7420  arg])....  #Get 
+0001da30: 4c61 6e64 7361 7420 696d 6167 6520 636f  Landsat image co
+0001da40: 6c6c 6563 7469 6f6e 0d0a 2020 6c73 203d  llection..  ls =
+0001da50: 2067 6574 4c61 6e64 7361 7428 5c0d 0a20   getLandsat(\.. 
+0001da60: 2020 2073 7475 6479 4172 6561 203d 2073     studyArea = s
+0001da70: 7475 6479 4172 6561 2c0d 0a20 2020 2073  tudyArea,..    s
+0001da80: 7461 7274 4461 7465 203d 2073 7461 7274  tartDate = start
+0001da90: 4461 7465 2c0d 0a20 2020 2065 6e64 4461  Date,..    endDa
+0001daa0: 7465 203d 2065 6e64 4461 7465 2c0d 0a20  te = endDate,.. 
+0001dab0: 2020 2073 7461 7274 4a75 6c69 616e 203d     startJulian =
+0001dac0: 2073 7461 7274 4a75 6c69 616e 2c0d 0a20   startJulian,.. 
+0001dad0: 2020 2065 6e64 4a75 6c69 616e 203d 2065     endJulian = e
+0001dae0: 6e64 4a75 6c69 616e 2c0d 0a20 2020 2074  ndJulian,..    t
+0001daf0: 6f61 4f72 5352 203d 2074 6f61 4f72 5352  oaOrSR = toaOrSR
+0001db00: 2c0d 0a20 2020 2069 6e63 6c75 6465 534c  ,..    includeSL
+0001db10: 434f 6666 4c37 203d 2069 6e63 6c75 6465  COffL7 = include
+0001db20: 534c 434f 6666 4c37 2c0d 0a20 2020 2064  SLCOffL7,..    d
+0001db30: 6566 7269 6e67 654c 3520 3d20 6465 6672  efringeL5 = defr
+0001db40: 696e 6765 4c35 2c0d 0a20 2020 2061 6464  ingeL5,..    add
+0001db50: 5069 7865 6c51 4120 3d20 6164 6450 6978  PixelQA = addPix
+0001db60: 656c 5141 2c0d 0a20 2020 2072 6573 616d  elQA,..    resam
+0001db70: 706c 654d 6574 686f 6420 3d20 7265 7361  pleMethod = resa
+0001db80: 6d70 6c65 4d65 7468 6f64 2c0d 0a20 2020  mpleMethod,..   
+0001db90: 206c 616e 6473 6174 436f 6c6c 6563 7469   landsatCollecti
+0001dba0: 6f6e 5665 7273 696f 6e20 3d20 6c61 6e64  onVersion = land
+0001dbb0: 7361 7443 6f6c 6c65 6374 696f 6e56 6572  satCollectionVer
+0001dbc0: 7369 6f6e 290d 0a0d 0a20 2023 4170 706c  sion)....  #Appl
+0001dbd0: 7920 7265 6c65 7661 6e74 2063 6c6f 7564  y relevant cloud
+0001dbe0: 206d 6173 6b69 6e67 206d 6574 686f 6473   masking methods
+0001dbf0: 0d0a 2020 6966 2061 7070 6c79 436c 6f75  ..  if applyClou
+0001dc00: 6453 636f 7265 3a0d 0a20 2020 2070 7269  dScore:..    pri
+0001dc10: 6e74 2827 4170 706c 7969 6e67 2043 6c6f  nt('Applying Clo
+0001dc20: 7564 2053 636f 7265 2729 0d0a 2020 2020  ud Score')..    
+0001dc30: 6c73 203d 2061 7070 6c79 436c 6f75 6453  ls = applyCloudS
+0001dc40: 636f 7265 416c 676f 7269 7468 6d28 5c0d  coreAlgorithm(\.
+0001dc50: 0a20 2020 2020 2063 6f6c 6c65 6374 696f  .      collectio
+0001dc60: 6e20 3d20 6c73 2c0d 0a20 2020 2020 2063  n = ls,..      c
+0001dc70: 6c6f 7564 5363 6f72 6546 756e 6374 696f  loudScoreFunctio
+0001dc80: 6e20 3d20 6c61 6e64 7361 7443 6c6f 7564  n = landsatCloud
+0001dc90: 5363 6f72 652c 0d0a 2020 2020 2020 636c  Score,..      cl
+0001dca0: 6f75 6453 636f 7265 5468 7265 7368 203d  oudScoreThresh =
+0001dcb0: 2063 6c6f 7564 5363 6f72 6554 6872 6573   cloudScoreThres
+0001dcc0: 682c 0d0a 2020 2020 2020 636c 6f75 6453  h,..      cloudS
+0001dcd0: 636f 7265 5063 746c 203d 2063 6c6f 7564  corePctl = cloud
+0001dce0: 5363 6f72 6550 6374 6c2c 0d0a 2020 2020  ScorePctl,..    
+0001dcf0: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
+0001dd00: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
+0001dd10: 732c 0d0a 2020 2020 2020 6469 6c61 7465  s,..      dilate
+0001dd20: 5069 7865 6c73 203d 2064 696c 6174 6550  Pixels = dilateP
+0001dd30: 6978 656c 732c 0d0a 2020 2020 2020 7065  ixels,..      pe
+0001dd40: 7266 6f72 6d43 6c6f 7564 5363 6f72 654f  rformCloudScoreO
+0001dd50: 6666 7365 7420 3d20 7065 7266 6f72 6d43  ffset = performC
+0001dd60: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
+0001dd70: 0d0a 2020 2020 2020 7072 6543 6f6d 7075  ..      preCompu
+0001dd80: 7465 6443 6c6f 7564 5363 6f72 654f 6666  tedCloudScoreOff
+0001dd90: 7365 7420 3d20 7072 6543 6f6d 7075 7465  set = preCompute
+0001dda0: 6443 6c6f 7564 5363 6f72 654f 6666 7365  dCloudScoreOffse
+0001ddb0: 7429 0d0a 0d0a 2020 6966 2061 7070 6c79  t)....  if apply
+0001ddc0: 466d 6173 6b43 6c6f 7564 4d61 736b 3a0d  FmaskCloudMask:.
+0001ddd0: 0a20 2020 2070 7269 6e74 2827 4170 706c  .    print('Appl
+0001dde0: 7969 6e67 2046 6d61 736b 2043 6c6f 7564  ying Fmask Cloud
+0001ddf0: 204d 6173 6b27 290d 0a20 2020 206c 7320   Mask')..    ls 
+0001de00: 3d20 6c73 2e6d 6170 286c 616d 6264 6120  = ls.map(lambda 
+0001de10: 696d 673a 2061 7070 6c79 4269 744d 6173  img: applyBitMas
+0001de20: 6b28 696d 672c 666d 6173 6b42 6974 4469  k(img,fmaskBitDi
+0001de30: 6374 5b6c 616e 6473 6174 436f 6c6c 6563  ct[landsatCollec
+0001de40: 7469 6f6e 5665 7273 696f 6e5d 5b27 636c  tionVersion]['cl
+0001de50: 6f75 6427 5d2c 6c61 6e64 7361 7446 6d61  oud'],landsatFma
+0001de60: 736b 4261 6e64 4e61 6d65 4469 6374 5b6c  skBandNameDict[l
+0001de70: 616e 6473 6174 436f 6c6c 6563 7469 6f6e  andsatCollection
+0001de80: 5665 7273 696f 6e5d 2929 0d0a 0d0a 2020  Version]))....  
+0001de90: 6966 2061 7070 6c79 5444 4f4d 3a0d 0a20  if applyTDOM:.. 
+0001dea0: 2020 2070 7269 6e74 2827 4170 706c 7969     print('Applyi
+0001deb0: 6e67 2054 444f 4d20 5368 6164 6f77 204d  ng TDOM Shadow M
+0001dec0: 6173 6b27 290d 0a20 2020 206c 7320 3d20  ask')..    ls = 
+0001ded0: 7369 6d70 6c65 5444 4f4d 3228 5c0d 0a20  simpleTDOM2(\.. 
+0001dee0: 2020 2020 2063 6f6c 6c65 6374 696f 6e20       collection 
+0001def0: 3d20 6c73 2c0d 0a20 2020 2020 207a 5363  = ls,..      zSc
+0001df00: 6f72 6554 6872 6573 6820 3d20 7a53 636f  oreThresh = zSco
+0001df10: 7265 5468 7265 7368 2c0d 0a20 2020 2020  reThresh,..     
+0001df20: 2073 6861 646f 7753 756d 5468 7265 7368   shadowSumThresh
+0001df30: 203d 2073 6861 646f 7753 756d 5468 7265   = shadowSumThre
+0001df40: 7368 2c0d 0a20 2020 2020 2063 6f6e 7472  sh,..      contr
+0001df50: 6163 7450 6978 656c 7320 3d20 636f 6e74  actPixels = cont
+0001df60: 7261 6374 5069 7865 6c73 2c0d 0a20 2020  ractPixels,..   
+0001df70: 2020 2064 696c 6174 6550 6978 656c 7320     dilatePixels 
+0001df80: 3d20 6469 6c61 7465 5069 7865 6c73 2c0d  = dilatePixels,.
+0001df90: 0a20 2020 2020 2073 6861 646f 7753 756d  .      shadowSum
+0001dfa0: 4261 6e64 7320 3d20 5b27 6e69 7227 2c27  Bands = ['nir','
+0001dfb0: 7377 6972 3127 5d2c 0d0a 2020 2020 2020  swir1'],..      
+0001dfc0: 7072 6543 6f6d 7075 7465 6454 444f 4d49  preComputedTDOMI
+0001dfd0: 524d 6561 6e20 3d20 7072 6543 6f6d 7075  RMean = preCompu
+0001dfe0: 7465 6454 444f 4d49 524d 6561 6e2c 0d0a  tedTDOMIRMean,..
+0001dff0: 2020 2020 2020 7072 6543 6f6d 7075 7465        preCompute
+0001e000: 6454 444f 4d49 5253 7464 4465 7620 3d20  dTDOMIRStdDev = 
+0001e010: 7072 6543 6f6d 7075 7465 6454 444f 4d49  preComputedTDOMI
+0001e020: 5253 7464 4465 7629 0d0a 0d0a 2020 6966  RStdDev)....  if
+0001e030: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
+0001e040: 5368 6164 6f77 4d61 736b 3a0d 0a20 2020  ShadowMask:..   
+0001e050: 2070 7269 6e74 2827 4170 706c 7969 6e67   print('Applying
+0001e060: 2046 6d61 736b 2053 6861 646f 7720 4d61   Fmask Shadow Ma
+0001e070: 736b 2729 0d0a 2020 2020 6c73 203d 206c  sk')..    ls = l
+0001e080: 732e 6d61 7028 6c61 6d62 6461 2069 6d67  s.map(lambda img
+0001e090: 3a20 6170 706c 7942 6974 4d61 736b 2869  : applyBitMask(i
+0001e0a0: 6d67 2c66 6d61 736b 4269 7444 6963 745b  mg,fmaskBitDict[
+0001e0b0: 6c61 6e64 7361 7443 6f6c 6c65 6374 696f  landsatCollectio
+0001e0c0: 6e56 6572 7369 6f6e 5d5b 2773 6861 646f  nVersion]['shado
+0001e0d0: 7727 5d2c 6c61 6e64 7361 7446 6d61 736b  w'],landsatFmask
+0001e0e0: 4261 6e64 4e61 6d65 4469 6374 5b6c 616e  BandNameDict[lan
+0001e0f0: 6473 6174 436f 6c6c 6563 7469 6f6e 5665  dsatCollectionVe
+0001e100: 7273 696f 6e5d 2929 0d0a 0d0a 0d0a 2020  rsion]))......  
+0001e110: 6966 2061 7070 6c79 466d 6173 6b53 6e6f  if applyFmaskSno
+0001e120: 774d 6173 6b3a 0d0a 2020 2020 7072 696e  wMask:..    prin
+0001e130: 7428 2741 7070 6c79 696e 6720 466d 6173  t('Applying Fmas
+0001e140: 6b20 736e 6f77 206d 6173 6b27 290d 0a20  k snow mask').. 
+0001e150: 2020 206c 7320 3d20 6c73 2e6d 6170 286c     ls = ls.map(l
+0001e160: 616d 6264 6120 696d 673a 2061 7070 6c79  ambda img: apply
+0001e170: 4269 744d 6173 6b28 696d 672c 666d 6173  BitMask(img,fmas
+0001e180: 6b42 6974 4469 6374 5b6c 616e 6473 6174  kBitDict[landsat
+0001e190: 436f 6c6c 6563 7469 6f6e 5665 7273 696f  CollectionVersio
+0001e1a0: 6e5d 5b27 736e 6f77 275d 2c6c 616e 6473  n]['snow'],lands
+0001e1b0: 6174 466d 6173 6b42 616e 644e 616d 6544  atFmaskBandNameD
+0001e1c0: 6963 745b 6c61 6e64 7361 7443 6f6c 6c65  ict[landsatColle
+0001e1d0: 6374 696f 6e56 6572 7369 6f6e 5d29 290d  ctionVersion])).
+0001e1e0: 0a0d 0a0d 0a20 2023 2041 6464 2063 6f6d  .....  # Add com
+0001e1f0: 6d6f 6e20 696e 6469 6365 730d 0a20 206c  mon indices..  l
+0001e200: 7320 3d20 6c73 2e6d 6170 2873 696d 706c  s = ls.map(simpl
+0001e210: 6541 6464 496e 6469 6365 7329 5c0d 0a20  eAddIndices)\.. 
+0001e220: 2020 2020 2020 2020 202e 6d61 7028 6765           .map(ge
+0001e230: 7454 6173 7365 6c65 6443 6170 295c 0d0a  tTasseledCap)\..
+0001e240: 2020 2020 2020 2020 2020 2e6d 6170 2873            .map(s
+0001e250: 696d 706c 6541 6464 5443 416e 676c 6573  impleAddTCAngles
+0001e260: 290d 0a0d 0a20 2023 2041 6464 2053 656e  )....  # Add Sen
+0001e270: 736f 7220 4261 6e64 0d0a 2020 6c73 203d  sor Band..  ls =
+0001e280: 206c 732e 6d61 7028 6c61 6d62 6461 2069   ls.map(lambda i
+0001e290: 6d67 3a20 6164 6453 656e 736f 7242 616e  mg: addSensorBan
+0001e2a0: 6428 696d 672c 206c 616e 6473 6174 436f  d(img, landsatCo
+0001e2b0: 6c6c 6563 7469 6f6e 5665 7273 696f 6e2b  llectionVersion+
+0001e2c0: 275f 6c61 6e64 7361 7427 2c20 746f 614f  '_landsat', toaO
+0001e2d0: 7253 5229 290d 0a0d 0a20 2072 6574 7572  rSR))....  retur
+0001e2e0: 6e20 6c73 2e73 6574 2861 7267 7329 0d0a  n ls.set(args)..
+0001e2f0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+0001e300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001e310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001e320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e330: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
 0001e340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e350: 2323 0d0a 2357 7261 7070 6572 2066 756e  ##..#Wrapper fun
-0001e360: 6374 696f 6e20 666f 7220 6765 7474 696e  ction for gettin
-0001e370: 6720 5365 6e74 696e 656c 3220 696d 6167  g Sentinel2 imag
-0001e380: 6572 790d 0a64 6566 2067 6574 5072 6f63  ery..def getProc
-0001e390: 6573 7365 6453 656e 7469 6e65 6c32 5363  essedSentinel2Sc
-0001e3a0: 656e 6573 285c 0d0a 2020 7374 7564 7941  enes(\..  studyA
-0001e3b0: 7265 612c 0d0a 2020 7374 6172 7459 6561  rea,..  startYea
-0001e3c0: 722c 0d0a 2020 656e 6459 6561 722c 0d0a  r,..  endYear,..
-0001e3d0: 2020 7374 6172 744a 756c 6961 6e2c 0d0a    startJulian,..
-0001e3e0: 2020 656e 644a 756c 6961 6e2c 0d0a 2020    endJulian,..  
-0001e3f0: 6170 706c 7951 4142 616e 6420 3d20 4661  applyQABand = Fa
-0001e400: 6c73 652c 0d0a 2020 6170 706c 7943 6c6f  lse,..  applyClo
-0001e410: 7564 5363 6f72 6520 3d20 4661 6c73 652c  udScore = False,
-0001e420: 0d0a 2020 6170 706c 7953 6861 646f 7753  ..  applyShadowS
-0001e430: 6869 6674 203d 2046 616c 7365 2c0d 0a20  hift = False,.. 
-0001e440: 2061 7070 6c79 5444 4f4d 203d 2054 7275   applyTDOM = Tru
-0001e450: 652c 0d0a 2020 636c 6f75 6453 636f 7265  e,..  cloudScore
-0001e460: 5468 7265 7368 203d 2032 302c 0d0a 2020  Thresh = 20,..  
-0001e470: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
-0001e480: 654f 6666 7365 7420 3d20 5472 7565 2c0d  eOffset = True,.
-0001e490: 0a20 2063 6c6f 7564 5363 6f72 6550 6374  .  cloudScorePct
-0001e4a0: 6c20 3d20 3130 2c0d 0a20 2063 6c6f 7564  l = 10,..  cloud
-0001e4b0: 4865 6967 6874 7320 3d20 6565 2e4c 6973  Heights = ee.Lis
-0001e4c0: 742e 7365 7175 656e 6365 2835 3030 2c31  t.sequence(500,1
-0001e4d0: 3030 3030 2c35 3030 292c 0d0a 2020 7a53  0000,500),..  zS
-0001e4e0: 636f 7265 5468 7265 7368 203d 202d 312c  coreThresh = -1,
-0001e4f0: 0d0a 2020 7368 6164 6f77 5375 6d54 6872  ..  shadowSumThr
-0001e500: 6573 6820 3d20 302e 3335 2c0d 0a20 2063  esh = 0.35,..  c
-0001e510: 6f6e 7472 6163 7450 6978 656c 7320 3d20  ontractPixels = 
-0001e520: 312e 352c 0d0a 2020 6469 6c61 7465 5069  1.5,..  dilatePi
-0001e530: 7865 6c73 203d 2033 2e35 2c0d 0a20 2073  xels = 3.5,..  s
-0001e540: 6861 646f 7753 756d 4261 6e64 7320 3d20  hadowSumBands = 
-0001e550: 5b27 6e69 7227 2c27 7377 6972 3127 5d2c  ['nir','swir1'],
-0001e560: 0d0a 2020 7265 7361 6d70 6c65 4d65 7468  ..  resampleMeth
-0001e570: 6f64 203d 2027 6167 6772 6567 6174 6527  od = 'aggregate'
-0001e580: 2c0d 0a20 2074 6f61 4f72 5352 203d 2027  ,..  toaOrSR = '
-0001e590: 544f 4127 2c0d 0a20 2063 6f6e 7665 7274  TOA',..  convert
-0001e5a0: 546f 4461 696c 794d 6f73 6169 6373 203d  ToDailyMosaics =
-0001e5b0: 2054 7275 652c 0d0a 2020 6170 706c 7943   True,..  applyC
-0001e5c0: 6c6f 7564 5072 6f62 6162 696c 6974 7920  loudProbability 
-0001e5d0: 3d20 5472 7565 2c0d 0a20 2070 7265 436f  = True,..  preCo
-0001e5e0: 6d70 7574 6564 436c 6f75 6453 636f 7265  mputedCloudScore
-0001e5f0: 4f66 6673 6574 203d 204e 6f6e 652c 0d0a  Offset = None,..
-0001e600: 2020 7072 6543 6f6d 7075 7465 6454 444f    preComputedTDO
-0001e610: 4d49 524d 6561 6e20 3d20 4e6f 6e65 2c0d  MIRMean = None,.
-0001e620: 0a20 2070 7265 436f 6d70 7574 6564 5444  .  preComputedTD
-0001e630: 4f4d 4952 5374 6444 6576 203d 204e 6f6e  OMIRStdDev = Non
-0001e640: 652c 0d0a 2020 636c 6f75 6450 726f 6254  e,..  cloudProbT
-0001e650: 6872 6573 6820 3d20 3430 293a 0d0a 0d0a  hresh = 40):....
-0001e660: 2020 6f72 6967 696e 203d 2027 5365 6e74    origin = 'Sent
-0001e670: 696e 656c 3227 0d0a 2020 746f 614f 7253  inel2'..  toaOrS
-0001e680: 5220 3d20 746f 614f 7253 522e 7570 7065  R = toaOrSR.uppe
-0001e690: 7228 290d 0a0d 0a20 2023 5072 6570 6172  r()....  #Prepar
-0001e6a0: 6520 6461 7465 730d 0a20 2023 5772 6170  e dates..  #Wrap
-0001e6b0: 2074 6865 2064 6174 6573 2069 6620 6e65   the dates if ne
-0001e6c0: 6564 6564 0d0a 2020 7772 6170 4f66 6673  eded..  wrapOffs
-0001e6d0: 6574 203d 2030 0d0a 2020 6966 2073 7461  et = 0..  if sta
-0001e6e0: 7274 4a75 6c69 616e 203e 2065 6e64 4a75  rtJulian > endJu
-0001e6f0: 6c69 616e 3a0d 0a20 2020 2077 7261 704f  lian:..    wrapO
-0001e700: 6666 7365 7420 3d20 3336 350d 0a20 2073  ffset = 365..  s
-0001e710: 7461 7274 4461 7465 203d 2065 652e 4461  tartDate = ee.Da
-0001e720: 7465 2e66 726f 6d59 4d44 2873 7461 7274  te.fromYMD(start
-0001e730: 5965 6172 2c31 2c31 292e 6164 7661 6e63  Year,1,1).advanc
-0001e740: 6528 7374 6172 744a 756c 6961 6e2d 312c  e(startJulian-1,
-0001e750: 2764 6179 2729 0d0a 2020 656e 6444 6174  'day')..  endDat
-0001e760: 6520 3d20 6565 2e44 6174 652e 6672 6f6d  e = ee.Date.from
-0001e770: 594d 4428 656e 6459 6561 722c 312c 3129  YMD(endYear,1,1)
-0001e780: 2e61 6476 616e 6365 2865 6e64 4a75 6c69  .advance(endJuli
-0001e790: 616e 2d31 2b77 7261 704f 6666 7365 742c  an-1+wrapOffset,
-0001e7a0: 2764 6179 2729 0d0a 0d0a 2020 6172 6773  'day')....  args
-0001e7b0: 203d 2066 6f72 6d61 7441 7267 7328 6c6f   = formatArgs(lo
-0001e7c0: 6361 6c73 2829 290d 0a20 2069 6620 2761  cals())..  if 'a
-0001e7d0: 7267 7327 2069 6e20 6172 6773 2e6b 6579  rgs' in args.key
-0001e7e0: 7328 293a 0d0a 2020 2020 6465 6c20 6172  s():..    del ar
-0001e7f0: 6773 5b27 6172 6773 275d 0d0a 0d0a 2020  gs['args']....  
-0001e800: 7072 696e 7428 2747 6574 2050 726f 6365  print('Get Proce
-0001e810: 7373 6564 2053 656e 7469 6e65 6c32 3a20  ssed Sentinel2: 
-0001e820: 2729 0d0a 2020 7072 696e 7428 2753 7461  ')..  print('Sta
-0001e830: 7274 2064 6174 653a 272c 2073 7461 7274  rt date:', start
-0001e840: 4461 7465 2e66 6f72 6d61 7428 274d 4d4d  Date.format('MMM
-0001e850: 2064 6420 7979 7979 2729 2e67 6574 496e   dd yyyy').getIn
-0001e860: 666f 2829 2c27 2c20 456e 6420 6461 7465  fo(),', End date
-0001e870: 3a27 2c20 656e 6444 6174 652e 666f 726d  :', endDate.form
-0001e880: 6174 2827 4d4d 4d20 6464 2079 7979 7927  at('MMM dd yyyy'
-0001e890: 292e 6765 7449 6e66 6f28 2929 0d0a 2020  ).getInfo())..  
-0001e8a0: 666f 7220 6172 6720 696e 2061 7267 732e  for arg in args.
-0001e8b0: 6b65 7973 2829 3a0d 0a20 2020 2070 7269  keys():..    pri
-0001e8c0: 6e74 2861 7267 2c20 273a 2027 2c20 6172  nt(arg, ': ', ar
-0001e8d0: 6773 5b61 7267 5d29 0d0a 0d0a 2020 2347  gs[arg])....  #G
-0001e8e0: 6574 2053 656e 7469 6e65 6c32 2069 6d61  et Sentinel2 ima
-0001e8f0: 6765 2063 6f6c 6c65 6374 696f 6e0d 0a20  ge collection.. 
-0001e900: 2073 3273 203d 2067 6574 5332 285c 0d0a   s2s = getS2(\..
-0001e910: 2020 2020 7374 7564 7941 7265 6120 3d20      studyArea = 
-0001e920: 7374 7564 7941 7265 612c 0d0a 2020 2020  studyArea,..    
-0001e930: 7374 6172 7444 6174 6520 3d20 7374 6172  startDate = star
-0001e940: 7444 6174 652c 0d0a 2020 2020 656e 6444  tDate,..    endD
-0001e950: 6174 6520 3d20 656e 6444 6174 652c 0d0a  ate = endDate,..
-0001e960: 2020 2020 7374 6172 744a 756c 6961 6e20      startJulian 
-0001e970: 3d20 7374 6172 744a 756c 6961 6e2c 0d0a  = startJulian,..
-0001e980: 2020 2020 656e 644a 756c 6961 6e20 3d20      endJulian = 
-0001e990: 656e 644a 756c 6961 6e2c 0d0a 2020 2020  endJulian,..    
-0001e9a0: 7265 7361 6d70 6c65 4d65 7468 6f64 203d  resampleMethod =
-0001e9b0: 2072 6573 616d 706c 654d 6574 686f 642c   resampleMethod,
-0001e9c0: 0d0a 2020 2020 746f 614f 7253 5220 3d20  ..    toaOrSR = 
-0001e9d0: 746f 614f 7253 522c 0d0a 2020 2020 636f  toaOrSR,..    co
-0001e9e0: 6e76 6572 7454 6f44 6169 6c79 4d6f 7361  nvertToDailyMosa
-0001e9f0: 6963 7320 3d20 636f 6e76 6572 7454 6f44  ics = convertToD
-0001ea00: 6169 6c79 4d6f 7361 6963 732c 0d0a 2020  ailyMosaics,..  
-0001ea10: 2020 6164 6443 6c6f 7564 5072 6f62 6162    addCloudProbab
-0001ea20: 696c 6974 7920 3d20 6170 706c 7943 6c6f  ility = applyClo
-0001ea30: 7564 5072 6f62 6162 696c 6974 7929 0d0a  udProbability)..
-0001ea40: 0d0a 2020 6966 2061 7070 6c79 5141 4261  ..  if applyQABa
-0001ea50: 6e64 3a0d 0a20 2020 2070 7269 6e74 2827  nd:..    print('
-0001ea60: 4170 706c 7969 6e67 2051 4120 4261 6e64  Applying QA Band
-0001ea70: 2043 6c6f 7564 204d 6173 6b27 290d 0a20   Cloud Mask').. 
-0001ea80: 2020 2073 3273 203d 2073 3273 2e6d 6170     s2s = s2s.map
-0001ea90: 286d 6173 6b53 3263 6c6f 7564 7329 0d0a  (maskS2clouds)..
-0001eaa0: 0d0a 2020 6966 2061 7070 6c79 436c 6f75  ..  if applyClou
-0001eab0: 6453 636f 7265 3a0d 0a20 2020 2070 7269  dScore:..    pri
-0001eac0: 6e74 2827 4170 706c 7969 6e67 2043 6c6f  nt('Applying Clo
-0001ead0: 7564 2053 636f 7265 2729 0d0a 2020 2020  ud Score')..    
-0001eae0: 7332 7320 3d20 6170 706c 7943 6c6f 7564  s2s = applyCloud
-0001eaf0: 5363 6f72 6541 6c67 6f72 6974 686d 285c  ScoreAlgorithm(\
-0001eb00: 0d0a 2020 2020 2020 636f 6c6c 6563 7469  ..      collecti
-0001eb10: 6f6e 203d 2073 3273 2c0d 0a20 2020 2020  on = s2s,..     
-0001eb20: 2063 6c6f 7564 5363 6f72 6546 756e 6374   cloudScoreFunct
-0001eb30: 696f 6e20 3d20 7365 6e74 696e 656c 3243  ion = sentinel2C
-0001eb40: 6c6f 7564 5363 6f72 652c 0d0a 2020 2020  loudScore,..    
-0001eb50: 2020 636c 6f75 6453 636f 7265 5468 7265    cloudScoreThre
-0001eb60: 7368 203d 2063 6c6f 7564 5363 6f72 6554  sh = cloudScoreT
-0001eb70: 6872 6573 682c 0d0a 2020 2020 2020 636c  hresh,..      cl
-0001eb80: 6f75 6453 636f 7265 5063 746c 203d 2063  oudScorePctl = c
-0001eb90: 6c6f 7564 5363 6f72 6550 6374 6c2c 0d0a  loudScorePctl,..
-0001eba0: 2020 2020 2020 636f 6e74 7261 6374 5069        contractPi
-0001ebb0: 7865 6c73 203d 2063 6f6e 7472 6163 7450  xels = contractP
-0001ebc0: 6978 656c 732c 0d0a 2020 2020 2020 6469  ixels,..      di
-0001ebd0: 6c61 7465 5069 7865 6c73 203d 2064 696c  latePixels = dil
-0001ebe0: 6174 6550 6978 656c 732c 0d0a 2020 2020  atePixels,..    
-0001ebf0: 2020 7065 7266 6f72 6d43 6c6f 7564 5363    performCloudSc
-0001ec00: 6f72 654f 6666 7365 7420 3d20 7065 7266  oreOffset = perf
-0001ec10: 6f72 6d43 6c6f 7564 5363 6f72 654f 6666  ormCloudScoreOff
-0001ec20: 7365 742c 0d0a 2020 2020 2020 7072 6543  set,..      preC
-0001ec30: 6f6d 7075 7465 6443 6c6f 7564 5363 6f72  omputedCloudScor
-0001ec40: 654f 6666 7365 7420 3d20 7072 6543 6f6d  eOffset = preCom
-0001ec50: 7075 7465 6443 6c6f 7564 5363 6f72 654f  putedCloudScoreO
-0001ec60: 6666 7365 7429 0d0a 0d0a 2020 6966 2061  ffset)....  if a
-0001ec70: 7070 6c79 436c 6f75 6450 726f 6261 6269  pplyCloudProbabi
-0001ec80: 6c69 7479 3a0d 0a20 2020 2070 7269 6e74  lity:..    print
-0001ec90: 2827 4170 706c 7920 436c 6f75 6420 5072  ('Apply Cloud Pr
-0001eca0: 6f62 6162 696c 6974 7927 290d 0a20 2020  obability')..   
-0001ecb0: 2073 3273 203d 2073 3273 2e6d 6170 286c   s2s = s2s.map(l
-0001ecc0: 616d 6264 6120 696d 673a 2069 6d67 2e75  ambda img: img.u
-0001ecd0: 7064 6174 654d 6173 6b28 696d 672e 7365  pdateMask(img.se
-0001ece0: 6c65 6374 285b 2763 6c6f 7564 5f70 726f  lect(['cloud_pro
-0001ecf0: 6261 6269 6c69 7479 275d 292e 6c74 6528  bability']).lte(
-0001ed00: 636c 6f75 6450 726f 6254 6872 6573 6829  cloudProbThresh)
-0001ed10: 2929 0d0a 0d0a 2020 6966 2061 7070 6c79  ))....  if apply
-0001ed20: 5368 6164 6f77 5368 6966 743a 0d0a 2020  ShadowShift:..  
-0001ed30: 2020 7072 696e 7428 2741 7070 6c79 696e    print('Applyin
-0001ed40: 6720 5368 6164 6f77 2053 6869 6674 2729  g Shadow Shift')
-0001ed50: 0d0a 2020 2020 7332 7320 3d20 7332 732e  ..    s2s = s2s.
-0001ed60: 6d61 7028 6c61 6d62 6461 2069 6d67 3a20  map(lambda img: 
-0001ed70: 7072 6f6a 6563 7453 6861 646f 7773 5772  projectShadowsWr
-0001ed80: 6170 7065 7228 5c0d 0a20 2020 2020 2069  apper(\..      i
-0001ed90: 6d67 203d 2069 6d67 2c0d 0a20 2020 2020  mg = img,..     
-0001eda0: 2063 6c6f 7564 5468 7265 7368 203d 2063   cloudThresh = c
-0001edb0: 6c6f 7564 5363 6f72 6554 6872 6573 682c  loudScoreThresh,
-0001edc0: 0d0a 2020 2020 2020 6972 5375 6d54 6872  ..      irSumThr
-0001edd0: 6573 6820 3d20 7368 6164 6f77 5375 6d54  esh = shadowSumT
-0001ede0: 6872 6573 682c 0d0a 2020 2020 2020 636f  hresh,..      co
-0001edf0: 6e74 7261 6374 5069 7865 6c73 203d 2063  ntractPixels = c
-0001ee00: 6f6e 7472 6163 7450 6978 656c 732c 0d0a  ontractPixels,..
-0001ee10: 2020 2020 2020 6469 6c61 7465 5069 7865        dilatePixe
-0001ee20: 6c73 203d 2064 696c 6174 6550 6978 656c  ls = dilatePixel
-0001ee30: 732c 0d0a 2020 2020 2020 636c 6f75 6448  s,..      cloudH
-0001ee40: 6569 6768 7473 203d 2063 6c6f 7564 4865  eights = cloudHe
-0001ee50: 6967 6874 7329 290d 0a0d 0a20 2069 6620  ights))....  if 
-0001ee60: 6170 706c 7954 444f 4d3a 0d0a 2020 2020  applyTDOM:..    
-0001ee70: 7072 696e 7428 2741 7070 6c79 696e 6720  print('Applying 
-0001ee80: 5444 4f4d 2729 0d0a 2020 2020 7332 7320  TDOM')..    s2s 
-0001ee90: 3d20 7369 6d70 6c65 5444 4f4d 3228 5c0d  = simpleTDOM2(\.
-0001eea0: 0a20 2020 2020 2063 6f6c 6c65 6374 696f  .      collectio
-0001eeb0: 6e20 3d20 7332 732c 0d0a 2020 2020 2020  n = s2s,..      
-0001eec0: 7a53 636f 7265 5468 7265 7368 203d 207a  zScoreThresh = z
-0001eed0: 5363 6f72 6554 6872 6573 682c 0d0a 2020  ScoreThresh,..  
-0001eee0: 2020 2020 7368 6164 6f77 5375 6d54 6872      shadowSumThr
-0001eef0: 6573 6820 3d20 7368 6164 6f77 5375 6d54  esh = shadowSumT
-0001ef00: 6872 6573 682c 0d0a 2020 2020 2020 636f  hresh,..      co
-0001ef10: 6e74 7261 6374 5069 7865 6c73 203d 2063  ntractPixels = c
-0001ef20: 6f6e 7472 6163 7450 6978 656c 732c 0d0a  ontractPixels,..
-0001ef30: 2020 2020 2020 6469 6c61 7465 5069 7865        dilatePixe
-0001ef40: 6c73 203d 2064 696c 6174 6550 6978 656c  ls = dilatePixel
-0001ef50: 732c 0d0a 2020 2020 2020 7368 6164 6f77  s,..      shadow
-0001ef60: 5375 6d42 616e 6473 203d 205b 276e 6972  SumBands = ['nir
-0001ef70: 272c 2773 7769 7231 275d 2c0d 0a20 2020  ','swir1'],..   
-0001ef80: 2020 2070 7265 436f 6d70 7574 6564 5444     preComputedTD
-0001ef90: 4f4d 4952 4d65 616e 203d 2070 7265 436f  OMIRMean = preCo
-0001efa0: 6d70 7574 6564 5444 4f4d 4952 4d65 616e  mputedTDOMIRMean
-0001efb0: 2c0d 0a20 2020 2020 2070 7265 436f 6d70  ,..      preComp
-0001efc0: 7574 6564 5444 4f4d 4952 5374 6444 6576  utedTDOMIRStdDev
-0001efd0: 203d 2070 7265 436f 6d70 7574 6564 5444   = preComputedTD
-0001efe0: 4f4d 4952 5374 6444 6576 290d 0a0d 0a20  OMIRStdDev).... 
-0001eff0: 2023 2041 6464 2063 6f6d 6d6f 6e20 696e   # Add common in
-0001f000: 6469 6365 730d 0a20 2073 3273 203d 2073  dices..  s2s = s
-0001f010: 3273 2e6d 6170 2873 696d 706c 6541 6464  2s.map(simpleAdd
-0001f020: 496e 6469 6365 7329 5c0d 0a20 2020 2020  Indices)\..     
-0001f030: 2020 2020 2020 2e6d 6170 2867 6574 5461        .map(getTa
-0001f040: 7373 656c 6564 4361 7029 5c0d 0a20 2020  sseledCap)\..   
-0001f050: 2020 2020 2020 2020 2e6d 6170 2873 696d          .map(sim
-0001f060: 706c 6541 6464 5443 416e 676c 6573 295c  pleAddTCAngles)\
-0001f070: 0d0a 2020 2020 2020 2020 2020 202e 6d61  ..           .ma
-0001f080: 7028 6c61 6d62 6461 2069 6d67 3a20 696d  p(lambda img: im
-0001f090: 672e 6164 6442 616e 6473 2869 6d67 2e6e  g.addBands(img.n
-0001f0a0: 6f72 6d61 6c69 7a65 6444 6966 6665 7265  ormalizedDiffere
-0001f0b0: 6e63 6528 5b27 7265 3127 2c20 2772 6564  nce(['re1', 'red
-0001f0c0: 275d 292e 7365 6c65 6374 285b 305d 2c5b  ']).select([0],[
-0001f0d0: 274e 4443 4927 5d29 2929 0d0a 2020 2320  'NDCI'])))..  # 
-0001f0e0: 4164 6420 5365 6e73 6f72 2042 616e 640d  Add Sensor Band.
-0001f0f0: 0a20 2073 3273 203d 2073 3273 2e6d 6170  .  s2s = s2s.map
-0001f100: 286c 616d 6264 6120 696d 673a 2061 6464  (lambda img: add
-0001f110: 5365 6e73 6f72 4261 6e64 2869 6d67 2c20  SensorBand(img, 
-0001f120: 2773 656e 7469 6e65 6c32 272c 2074 6f61  'sentinel2', toa
-0001f130: 4f72 5352 2929 0d0a 0d0a 200d 0a20 2072  OrSR)).... ..  r
-0001f140: 6574 7572 6e20 7332 732e 7365 7428 6172  eturn s2s.set(ar
-0001f150: 6773 290d 0a0d 0a0d 0a23 2323 2323 2323  gs)......#######
-0001f160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e380: 2323 2323 2323 0d0a 2357 7261 7070 6572  ######..#Wrapper
+0001e390: 2066 756e 6374 696f 6e20 666f 7220 6765   function for ge
+0001e3a0: 7474 696e 6720 5365 6e74 696e 656c 3220  tting Sentinel2 
+0001e3b0: 696d 6167 6572 790d 0a64 6566 2067 6574  imagery..def get
+0001e3c0: 5072 6f63 6573 7365 6453 656e 7469 6e65  ProcessedSentine
+0001e3d0: 6c32 5363 656e 6573 285c 0d0a 2020 7374  l2Scenes(\..  st
+0001e3e0: 7564 7941 7265 612c 0d0a 2020 7374 6172  udyArea,..  star
+0001e3f0: 7459 6561 722c 0d0a 2020 656e 6459 6561  tYear,..  endYea
+0001e400: 722c 0d0a 2020 7374 6172 744a 756c 6961  r,..  startJulia
+0001e410: 6e2c 0d0a 2020 656e 644a 756c 6961 6e2c  n,..  endJulian,
+0001e420: 0d0a 2020 6170 706c 7951 4142 616e 6420  ..  applyQABand 
+0001e430: 3d20 4661 6c73 652c 0d0a 2020 6170 706c  = False,..  appl
+0001e440: 7943 6c6f 7564 5363 6f72 6520 3d20 4661  yCloudScore = Fa
+0001e450: 6c73 652c 0d0a 2020 6170 706c 7953 6861  lse,..  applySha
+0001e460: 646f 7753 6869 6674 203d 2046 616c 7365  dowShift = False
+0001e470: 2c0d 0a20 2061 7070 6c79 5444 4f4d 203d  ,..  applyTDOM =
+0001e480: 2054 7275 652c 0d0a 2020 636c 6f75 6453   True,..  cloudS
+0001e490: 636f 7265 5468 7265 7368 203d 2032 302c  coreThresh = 20,
+0001e4a0: 0d0a 2020 7065 7266 6f72 6d43 6c6f 7564  ..  performCloud
+0001e4b0: 5363 6f72 654f 6666 7365 7420 3d20 5472  ScoreOffset = Tr
+0001e4c0: 7565 2c0d 0a20 2063 6c6f 7564 5363 6f72  ue,..  cloudScor
+0001e4d0: 6550 6374 6c20 3d20 3130 2c0d 0a20 2063  ePctl = 10,..  c
+0001e4e0: 6c6f 7564 4865 6967 6874 7320 3d20 6565  loudHeights = ee
+0001e4f0: 2e4c 6973 742e 7365 7175 656e 6365 2835  .List.sequence(5
+0001e500: 3030 2c31 3030 3030 2c35 3030 292c 0d0a  00,10000,500),..
+0001e510: 2020 7a53 636f 7265 5468 7265 7368 203d    zScoreThresh =
+0001e520: 202d 312c 0d0a 2020 7368 6164 6f77 5375   -1,..  shadowSu
+0001e530: 6d54 6872 6573 6820 3d20 302e 3335 2c0d  mThresh = 0.35,.
+0001e540: 0a20 2063 6f6e 7472 6163 7450 6978 656c  .  contractPixel
+0001e550: 7320 3d20 312e 352c 0d0a 2020 6469 6c61  s = 1.5,..  dila
+0001e560: 7465 5069 7865 6c73 203d 2033 2e35 2c0d  tePixels = 3.5,.
+0001e570: 0a20 2073 6861 646f 7753 756d 4261 6e64  .  shadowSumBand
+0001e580: 7320 3d20 5b27 6e69 7227 2c27 7377 6972  s = ['nir','swir
+0001e590: 3127 5d2c 0d0a 2020 7265 7361 6d70 6c65  1'],..  resample
+0001e5a0: 4d65 7468 6f64 203d 2027 6167 6772 6567  Method = 'aggreg
+0001e5b0: 6174 6527 2c0d 0a20 2074 6f61 4f72 5352  ate',..  toaOrSR
+0001e5c0: 203d 2027 544f 4127 2c0d 0a20 2063 6f6e   = 'TOA',..  con
+0001e5d0: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
+0001e5e0: 6373 203d 2054 7275 652c 0d0a 2020 6170  cs = True,..  ap
+0001e5f0: 706c 7943 6c6f 7564 5072 6f62 6162 696c  plyCloudProbabil
+0001e600: 6974 7920 3d20 5472 7565 2c0d 0a20 2070  ity = True,..  p
+0001e610: 7265 436f 6d70 7574 6564 436c 6f75 6453  reComputedCloudS
+0001e620: 636f 7265 4f66 6673 6574 203d 204e 6f6e  coreOffset = Non
+0001e630: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
+0001e640: 6454 444f 4d49 524d 6561 6e20 3d20 4e6f  dTDOMIRMean = No
+0001e650: 6e65 2c0d 0a20 2070 7265 436f 6d70 7574  ne,..  preComput
+0001e660: 6564 5444 4f4d 4952 5374 6444 6576 203d  edTDOMIRStdDev =
+0001e670: 204e 6f6e 652c 0d0a 2020 636c 6f75 6450   None,..  cloudP
+0001e680: 726f 6254 6872 6573 6820 3d20 3430 293a  robThresh = 40):
+0001e690: 0d0a 0d0a 2020 6f72 6967 696e 203d 2027  ....  origin = '
+0001e6a0: 5365 6e74 696e 656c 3227 0d0a 2020 746f  Sentinel2'..  to
+0001e6b0: 614f 7253 5220 3d20 746f 614f 7253 522e  aOrSR = toaOrSR.
+0001e6c0: 7570 7065 7228 290d 0a0d 0a20 2023 5072  upper()....  #Pr
+0001e6d0: 6570 6172 6520 6461 7465 730d 0a20 2023  epare dates..  #
+0001e6e0: 5772 6170 2074 6865 2064 6174 6573 2069  Wrap the dates i
+0001e6f0: 6620 6e65 6564 6564 0d0a 2020 7772 6170  f needed..  wrap
+0001e700: 4f66 6673 6574 203d 2030 0d0a 2020 6966  Offset = 0..  if
+0001e710: 2073 7461 7274 4a75 6c69 616e 203e 2065   startJulian > e
+0001e720: 6e64 4a75 6c69 616e 3a0d 0a20 2020 2077  ndJulian:..    w
+0001e730: 7261 704f 6666 7365 7420 3d20 3336 350d  rapOffset = 365.
+0001e740: 0a20 2073 7461 7274 4461 7465 203d 2065  .  startDate = e
+0001e750: 652e 4461 7465 2e66 726f 6d59 4d44 2873  e.Date.fromYMD(s
+0001e760: 7461 7274 5965 6172 2c31 2c31 292e 6164  tartYear,1,1).ad
+0001e770: 7661 6e63 6528 7374 6172 744a 756c 6961  vance(startJulia
+0001e780: 6e2d 312c 2764 6179 2729 0d0a 2020 656e  n-1,'day')..  en
+0001e790: 6444 6174 6520 3d20 6565 2e44 6174 652e  dDate = ee.Date.
+0001e7a0: 6672 6f6d 594d 4428 656e 6459 6561 722c  fromYMD(endYear,
+0001e7b0: 312c 3129 2e61 6476 616e 6365 2865 6e64  1,1).advance(end
+0001e7c0: 4a75 6c69 616e 2d31 2b77 7261 704f 6666  Julian-1+wrapOff
+0001e7d0: 7365 742c 2764 6179 2729 0d0a 0d0a 2020  set,'day')....  
+0001e7e0: 6172 6773 203d 2066 6f72 6d61 7441 7267  args = formatArg
+0001e7f0: 7328 6c6f 6361 6c73 2829 290d 0a20 2069  s(locals())..  i
+0001e800: 6620 2761 7267 7327 2069 6e20 6172 6773  f 'args' in args
+0001e810: 2e6b 6579 7328 293a 0d0a 2020 2020 6465  .keys():..    de
+0001e820: 6c20 6172 6773 5b27 6172 6773 275d 0d0a  l args['args']..
+0001e830: 0d0a 2020 7072 696e 7428 2747 6574 2050  ..  print('Get P
+0001e840: 726f 6365 7373 6564 2053 656e 7469 6e65  rocessed Sentine
+0001e850: 6c32 3a20 2729 0d0a 2020 7072 696e 7428  l2: ')..  print(
+0001e860: 2753 7461 7274 2064 6174 653a 272c 2073  'Start date:', s
+0001e870: 7461 7274 4461 7465 2e66 6f72 6d61 7428  tartDate.format(
+0001e880: 274d 4d4d 2064 6420 7979 7979 2729 2e67  'MMM dd yyyy').g
+0001e890: 6574 496e 666f 2829 2c27 2c20 456e 6420  etInfo(),', End 
+0001e8a0: 6461 7465 3a27 2c20 656e 6444 6174 652e  date:', endDate.
+0001e8b0: 666f 726d 6174 2827 4d4d 4d20 6464 2079  format('MMM dd y
+0001e8c0: 7979 7927 292e 6765 7449 6e66 6f28 2929  yyy').getInfo())
+0001e8d0: 0d0a 2020 666f 7220 6172 6720 696e 2061  ..  for arg in a
+0001e8e0: 7267 732e 6b65 7973 2829 3a0d 0a20 2020  rgs.keys():..   
+0001e8f0: 2070 7269 6e74 2861 7267 2c20 273a 2027   print(arg, ': '
+0001e900: 2c20 6172 6773 5b61 7267 5d29 0d0a 0d0a  , args[arg])....
+0001e910: 2020 2347 6574 2053 656e 7469 6e65 6c32    #Get Sentinel2
+0001e920: 2069 6d61 6765 2063 6f6c 6c65 6374 696f   image collectio
+0001e930: 6e0d 0a20 2073 3273 203d 2067 6574 5332  n..  s2s = getS2
+0001e940: 285c 0d0a 2020 2020 7374 7564 7941 7265  (\..    studyAre
+0001e950: 6120 3d20 7374 7564 7941 7265 612c 0d0a  a = studyArea,..
+0001e960: 2020 2020 7374 6172 7444 6174 6520 3d20      startDate = 
+0001e970: 7374 6172 7444 6174 652c 0d0a 2020 2020  startDate,..    
+0001e980: 656e 6444 6174 6520 3d20 656e 6444 6174  endDate = endDat
+0001e990: 652c 0d0a 2020 2020 7374 6172 744a 756c  e,..    startJul
+0001e9a0: 6961 6e20 3d20 7374 6172 744a 756c 6961  ian = startJulia
+0001e9b0: 6e2c 0d0a 2020 2020 656e 644a 756c 6961  n,..    endJulia
+0001e9c0: 6e20 3d20 656e 644a 756c 6961 6e2c 0d0a  n = endJulian,..
+0001e9d0: 2020 2020 7265 7361 6d70 6c65 4d65 7468      resampleMeth
+0001e9e0: 6f64 203d 2072 6573 616d 706c 654d 6574  od = resampleMet
+0001e9f0: 686f 642c 0d0a 2020 2020 746f 614f 7253  hod,..    toaOrS
+0001ea00: 5220 3d20 746f 614f 7253 522c 0d0a 2020  R = toaOrSR,..  
+0001ea10: 2020 636f 6e76 6572 7454 6f44 6169 6c79    convertToDaily
+0001ea20: 4d6f 7361 6963 7320 3d20 636f 6e76 6572  Mosaics = conver
+0001ea30: 7454 6f44 6169 6c79 4d6f 7361 6963 732c  tToDailyMosaics,
+0001ea40: 0d0a 2020 2020 6164 6443 6c6f 7564 5072  ..    addCloudPr
+0001ea50: 6f62 6162 696c 6974 7920 3d20 6170 706c  obability = appl
+0001ea60: 7943 6c6f 7564 5072 6f62 6162 696c 6974  yCloudProbabilit
+0001ea70: 7929 0d0a 0d0a 2020 6966 2061 7070 6c79  y)....  if apply
+0001ea80: 5141 4261 6e64 3a0d 0a20 2020 2070 7269  QABand:..    pri
+0001ea90: 6e74 2827 4170 706c 7969 6e67 2051 4120  nt('Applying QA 
+0001eaa0: 4261 6e64 2043 6c6f 7564 204d 6173 6b27  Band Cloud Mask'
+0001eab0: 290d 0a20 2020 2073 3273 203d 2073 3273  )..    s2s = s2s
+0001eac0: 2e6d 6170 286d 6173 6b53 3263 6c6f 7564  .map(maskS2cloud
+0001ead0: 7329 0d0a 0d0a 2020 6966 2061 7070 6c79  s)....  if apply
+0001eae0: 436c 6f75 6453 636f 7265 3a0d 0a20 2020  CloudScore:..   
+0001eaf0: 2070 7269 6e74 2827 4170 706c 7969 6e67   print('Applying
+0001eb00: 2043 6c6f 7564 2053 636f 7265 2729 0d0a   Cloud Score')..
+0001eb10: 2020 2020 7332 7320 3d20 6170 706c 7943      s2s = applyC
+0001eb20: 6c6f 7564 5363 6f72 6541 6c67 6f72 6974  loudScoreAlgorit
+0001eb30: 686d 285c 0d0a 2020 2020 2020 636f 6c6c  hm(\..      coll
+0001eb40: 6563 7469 6f6e 203d 2073 3273 2c0d 0a20  ection = s2s,.. 
+0001eb50: 2020 2020 2063 6c6f 7564 5363 6f72 6546       cloudScoreF
+0001eb60: 756e 6374 696f 6e20 3d20 7365 6e74 696e  unction = sentin
+0001eb70: 656c 3243 6c6f 7564 5363 6f72 652c 0d0a  el2CloudScore,..
+0001eb80: 2020 2020 2020 636c 6f75 6453 636f 7265        cloudScore
+0001eb90: 5468 7265 7368 203d 2063 6c6f 7564 5363  Thresh = cloudSc
+0001eba0: 6f72 6554 6872 6573 682c 0d0a 2020 2020  oreThresh,..    
+0001ebb0: 2020 636c 6f75 6453 636f 7265 5063 746c    cloudScorePctl
+0001ebc0: 203d 2063 6c6f 7564 5363 6f72 6550 6374   = cloudScorePct
+0001ebd0: 6c2c 0d0a 2020 2020 2020 636f 6e74 7261  l,..      contra
+0001ebe0: 6374 5069 7865 6c73 203d 2063 6f6e 7472  ctPixels = contr
+0001ebf0: 6163 7450 6978 656c 732c 0d0a 2020 2020  actPixels,..    
+0001ec00: 2020 6469 6c61 7465 5069 7865 6c73 203d    dilatePixels =
+0001ec10: 2064 696c 6174 6550 6978 656c 732c 0d0a   dilatePixels,..
+0001ec20: 2020 2020 2020 7065 7266 6f72 6d43 6c6f        performClo
+0001ec30: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
+0001ec40: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
+0001ec50: 654f 6666 7365 742c 0d0a 2020 2020 2020  eOffset,..      
+0001ec60: 7072 6543 6f6d 7075 7465 6443 6c6f 7564  preComputedCloud
+0001ec70: 5363 6f72 654f 6666 7365 7420 3d20 7072  ScoreOffset = pr
+0001ec80: 6543 6f6d 7075 7465 6443 6c6f 7564 5363  eComputedCloudSc
+0001ec90: 6f72 654f 6666 7365 7429 0d0a 0d0a 2020  oreOffset)....  
+0001eca0: 6966 2061 7070 6c79 436c 6f75 6450 726f  if applyCloudPro
+0001ecb0: 6261 6269 6c69 7479 3a0d 0a20 2020 2070  bability:..    p
+0001ecc0: 7269 6e74 2827 4170 706c 7920 436c 6f75  rint('Apply Clou
+0001ecd0: 6420 5072 6f62 6162 696c 6974 7927 290d  d Probability').
+0001ece0: 0a20 2020 2073 3273 203d 2073 3273 2e6d  .    s2s = s2s.m
+0001ecf0: 6170 286c 616d 6264 6120 696d 673a 2069  ap(lambda img: i
+0001ed00: 6d67 2e75 7064 6174 654d 6173 6b28 696d  mg.updateMask(im
+0001ed10: 672e 7365 6c65 6374 285b 2763 6c6f 7564  g.select(['cloud
+0001ed20: 5f70 726f 6261 6269 6c69 7479 275d 292e  _probability']).
+0001ed30: 6c74 6528 636c 6f75 6450 726f 6254 6872  lte(cloudProbThr
+0001ed40: 6573 6829 2929 0d0a 0d0a 2020 6966 2061  esh)))....  if a
+0001ed50: 7070 6c79 5368 6164 6f77 5368 6966 743a  pplyShadowShift:
+0001ed60: 0d0a 2020 2020 7072 696e 7428 2741 7070  ..    print('App
+0001ed70: 6c79 696e 6720 5368 6164 6f77 2053 6869  lying Shadow Shi
+0001ed80: 6674 2729 0d0a 2020 2020 7332 7320 3d20  ft')..    s2s = 
+0001ed90: 7332 732e 6d61 7028 6c61 6d62 6461 2069  s2s.map(lambda i
+0001eda0: 6d67 3a20 7072 6f6a 6563 7453 6861 646f  mg: projectShado
+0001edb0: 7773 5772 6170 7065 7228 5c0d 0a20 2020  wsWrapper(\..   
+0001edc0: 2020 2069 6d67 203d 2069 6d67 2c0d 0a20     img = img,.. 
+0001edd0: 2020 2020 2063 6c6f 7564 5468 7265 7368       cloudThresh
+0001ede0: 203d 2063 6c6f 7564 5363 6f72 6554 6872   = cloudScoreThr
+0001edf0: 6573 682c 0d0a 2020 2020 2020 6972 5375  esh,..      irSu
+0001ee00: 6d54 6872 6573 6820 3d20 7368 6164 6f77  mThresh = shadow
+0001ee10: 5375 6d54 6872 6573 682c 0d0a 2020 2020  SumThresh,..    
+0001ee20: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
+0001ee30: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
+0001ee40: 732c 0d0a 2020 2020 2020 6469 6c61 7465  s,..      dilate
+0001ee50: 5069 7865 6c73 203d 2064 696c 6174 6550  Pixels = dilateP
+0001ee60: 6978 656c 732c 0d0a 2020 2020 2020 636c  ixels,..      cl
+0001ee70: 6f75 6448 6569 6768 7473 203d 2063 6c6f  oudHeights = clo
+0001ee80: 7564 4865 6967 6874 7329 290d 0a0d 0a20  udHeights)).... 
+0001ee90: 2069 6620 6170 706c 7954 444f 4d3a 0d0a   if applyTDOM:..
+0001eea0: 2020 2020 7072 696e 7428 2741 7070 6c79      print('Apply
+0001eeb0: 696e 6720 5444 4f4d 2729 0d0a 2020 2020  ing TDOM')..    
+0001eec0: 7332 7320 3d20 7369 6d70 6c65 5444 4f4d  s2s = simpleTDOM
+0001eed0: 3228 5c0d 0a20 2020 2020 2063 6f6c 6c65  2(\..      colle
+0001eee0: 6374 696f 6e20 3d20 7332 732c 0d0a 2020  ction = s2s,..  
+0001eef0: 2020 2020 7a53 636f 7265 5468 7265 7368      zScoreThresh
+0001ef00: 203d 207a 5363 6f72 6554 6872 6573 682c   = zScoreThresh,
+0001ef10: 0d0a 2020 2020 2020 7368 6164 6f77 5375  ..      shadowSu
+0001ef20: 6d54 6872 6573 6820 3d20 7368 6164 6f77  mThresh = shadow
+0001ef30: 5375 6d54 6872 6573 682c 0d0a 2020 2020  SumThresh,..    
+0001ef40: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
+0001ef50: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
+0001ef60: 732c 0d0a 2020 2020 2020 6469 6c61 7465  s,..      dilate
+0001ef70: 5069 7865 6c73 203d 2064 696c 6174 6550  Pixels = dilateP
+0001ef80: 6978 656c 732c 0d0a 2020 2020 2020 7368  ixels,..      sh
+0001ef90: 6164 6f77 5375 6d42 616e 6473 203d 205b  adowSumBands = [
+0001efa0: 276e 6972 272c 2773 7769 7231 275d 2c0d  'nir','swir1'],.
+0001efb0: 0a20 2020 2020 2070 7265 436f 6d70 7574  .      preComput
+0001efc0: 6564 5444 4f4d 4952 4d65 616e 203d 2070  edTDOMIRMean = p
+0001efd0: 7265 436f 6d70 7574 6564 5444 4f4d 4952  reComputedTDOMIR
+0001efe0: 4d65 616e 2c0d 0a20 2020 2020 2070 7265  Mean,..      pre
+0001eff0: 436f 6d70 7574 6564 5444 4f4d 4952 5374  ComputedTDOMIRSt
+0001f000: 6444 6576 203d 2070 7265 436f 6d70 7574  dDev = preComput
+0001f010: 6564 5444 4f4d 4952 5374 6444 6576 290d  edTDOMIRStdDev).
+0001f020: 0a0d 0a20 2023 2041 6464 2063 6f6d 6d6f  ...  # Add commo
+0001f030: 6e20 696e 6469 6365 730d 0a20 2073 3273  n indices..  s2s
+0001f040: 203d 2073 3273 2e6d 6170 2873 696d 706c   = s2s.map(simpl
+0001f050: 6541 6464 496e 6469 6365 7329 5c0d 0a20  eAddIndices)\.. 
+0001f060: 2020 2020 2020 2020 2020 2e6d 6170 2867            .map(g
+0001f070: 6574 5461 7373 656c 6564 4361 7029 5c0d  etTasseledCap)\.
+0001f080: 0a20 2020 2020 2020 2020 2020 2e6d 6170  .           .map
+0001f090: 2873 696d 706c 6541 6464 5443 416e 676c  (simpleAddTCAngl
+0001f0a0: 6573 295c 0d0a 2020 2020 2020 2020 2020  es)\..          
+0001f0b0: 202e 6d61 7028 6c61 6d62 6461 2069 6d67   .map(lambda img
+0001f0c0: 3a20 696d 672e 6164 6442 616e 6473 2869  : img.addBands(i
+0001f0d0: 6d67 2e6e 6f72 6d61 6c69 7a65 6444 6966  mg.normalizedDif
+0001f0e0: 6665 7265 6e63 6528 5b27 7265 3127 2c20  ference(['re1', 
+0001f0f0: 2772 6564 275d 292e 7365 6c65 6374 285b  'red']).select([
+0001f100: 305d 2c5b 274e 4443 4927 5d29 2929 0d0a  0],['NDCI'])))..
+0001f110: 2020 2320 4164 6420 5365 6e73 6f72 2042    # Add Sensor B
+0001f120: 616e 640d 0a20 2073 3273 203d 2073 3273  and..  s2s = s2s
+0001f130: 2e6d 6170 286c 616d 6264 6120 696d 673a  .map(lambda img:
+0001f140: 2061 6464 5365 6e73 6f72 4261 6e64 2869   addSensorBand(i
+0001f150: 6d67 2c20 2773 656e 7469 6e65 6c32 272c  mg, 'sentinel2',
+0001f160: 2074 6f61 4f72 5352 2929 0d0a 0d0a 200d   toaOrSR)).... .
+0001f170: 0a20 2072 6574 7572 6e20 7332 732e 7365  .  return s2s.se
+0001f180: 7428 6172 6773 290d 0a0d 0a0d 0a23 2323  t(args)......###
 0001f190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1a0: 2323 0d0a 2323 2323 2323 2323 2323 2323  ##..############
+0001f1a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001f1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001f1c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1e0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-0001f1f0: 2057 7261 7070 6572 2066 756e 6374 696f   Wrapper functio
-0001f200: 6e20 666f 7220 6765 7474 696e 6720 5365  n for getting Se
-0001f210: 6e74 696e 656c 2032 2069 6d61 6765 7279  ntinel 2 imagery
-0001f220: 0d0a 6465 6620 6765 7453 656e 7469 6e65  ..def getSentine
-0001f230: 6c32 5772 6170 7065 7228 5c0d 0a20 2073  l2Wrapper(\..  s
-0001f240: 7475 6479 4172 6561 2c0d 0a20 2073 7461  tudyArea,..  sta
-0001f250: 7274 5965 6172 2c0d 0a20 2065 6e64 5965  rtYear,..  endYe
-0001f260: 6172 2c0d 0a20 2073 7461 7274 4a75 6c69  ar,..  startJuli
-0001f270: 616e 2c0d 0a20 2065 6e64 4a75 6c69 616e  an,..  endJulian
-0001f280: 2c0d 0a20 2074 696d 6562 7566 6665 7220  ,..  timebuffer 
-0001f290: 3d20 302c 0d0a 2020 7765 6967 6874 7320  = 0,..  weights 
-0001f2a0: 3d20 5b31 5d2c 0d0a 2020 636f 6d70 6f73  = [1],..  compos
-0001f2b0: 6974 696e 674d 6574 686f 6420 3d20 276d  itingMethod = 'm
-0001f2c0: 6564 6f69 6427 2c0d 0a20 2061 7070 6c79  edoid',..  apply
-0001f2d0: 5141 4261 6e64 203d 2046 616c 7365 2c0d  QABand = False,.
-0001f2e0: 0a20 2061 7070 6c79 436c 6f75 6453 636f  .  applyCloudSco
-0001f2f0: 7265 203d 2046 616c 7365 2c0d 0a20 2061  re = False,..  a
-0001f300: 7070 6c79 5368 6164 6f77 5368 6966 7420  pplyShadowShift 
-0001f310: 3d20 4661 6c73 652c 0d0a 2020 6170 706c  = False,..  appl
-0001f320: 7954 444f 4d20 3d20 5472 7565 2c0d 0a20  yTDOM = True,.. 
-0001f330: 2063 6c6f 7564 5363 6f72 6554 6872 6573   cloudScoreThres
-0001f340: 6820 3d20 3230 2c0d 0a20 2070 6572 666f  h = 20,..  perfo
-0001f350: 726d 436c 6f75 6453 636f 7265 4f66 6673  rmCloudScoreOffs
-0001f360: 6574 203d 2054 7275 652c 0d0a 2020 636c  et = True,..  cl
-0001f370: 6f75 6453 636f 7265 5063 746c 203d 2031  oudScorePctl = 1
-0001f380: 302c 0d0a 2020 636c 6f75 6448 6569 6768  0,..  cloudHeigh
-0001f390: 7473 203d 6565 2e4c 6973 742e 7365 7175  ts =ee.List.sequ
-0001f3a0: 656e 6365 2835 3030 2c31 3030 3030 2c35  ence(500,10000,5
-0001f3b0: 3030 292c 0d0a 2020 7a53 636f 7265 5468  00),..  zScoreTh
-0001f3c0: 7265 7368 203d 202d 312c 0d0a 2020 7368  resh = -1,..  sh
-0001f3d0: 6164 6f77 5375 6d54 6872 6573 6820 3d20  adowSumThresh = 
-0001f3e0: 302e 3335 2c0d 0a20 2063 6f6e 7472 6163  0.35,..  contrac
-0001f3f0: 7450 6978 656c 7320 3d20 312e 352c 0d0a  tPixels = 1.5,..
-0001f400: 2020 6469 6c61 7465 5069 7865 6c73 203d    dilatePixels =
-0001f410: 2033 2e35 2c0d 0a20 2073 6861 646f 7753   3.5,..  shadowS
-0001f420: 756d 4261 6e64 7320 3d20 5b27 6e69 7227  umBands = ['nir'
-0001f430: 2c27 7377 6972 3127 5d2c 0d0a 2020 636f  ,'swir1'],..  co
-0001f440: 7272 6563 7449 6c6c 756d 696e 6174 696f  rrectIlluminatio
-0001f450: 6e20 3d20 4661 6c73 652c 0d0a 2020 636f  n = False,..  co
-0001f460: 7272 6563 7453 6361 6c65 203d 2032 3530  rrectScale = 250
-0001f470: 2c0d 0a20 2065 7870 6f72 7443 6f6d 706f  ,..  exportCompo
-0001f480: 7369 7465 7320 3d20 4661 6c73 652c 0d0a  sites = False,..
-0001f490: 2020 6f75 7470 7574 4e61 6d65 203d 2027    outputName = '
-0001f4a0: 5365 6e74 696e 656c 322d 436f 6d70 6f73  Sentinel2-Compos
-0001f4b0: 6974 6527 2c0d 0a20 2065 7870 6f72 7450  ite',..  exportP
-0001f4c0: 6174 6852 6f6f 7420 3d20 2775 7365 7273  athRoot = 'users
-0001f4d0: 2f69 616e 686f 7573 6d61 6e2f 7465 7374  /ianhousman/test
-0001f4e0: 272c 0d0a 2020 6372 7320 3d20 2745 5053  ',..  crs = 'EPS
-0001f4f0: 473a 3530 3730 272c 0d0a 2020 7472 616e  G:5070',..  tran
-0001f500: 7366 6f72 6d20 3d20 5b31 302c 302c 2d32  sform = [10,0,-2
-0001f510: 3336 3139 3135 2e30 2c30 2c2d 3130 2c33  361915.0,0,-10,3
-0001f520: 3137 3737 3335 2e30 5d2c 0d0a 2020 7363  177735.0],..  sc
-0001f530: 616c 6520 3d20 4e6f 6e65 2c0d 0a20 2072  ale = None,..  r
-0001f540: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
-0001f550: 2761 6767 7265 6761 7465 272c 0d0a 2020  'aggregate',..  
-0001f560: 746f 614f 7253 5220 3d20 2754 4f41 272c  toaOrSR = 'TOA',
-0001f570: 0d0a 2020 636f 6e76 6572 7454 6f44 6169  ..  convertToDai
-0001f580: 6c79 4d6f 7361 6963 7320 3d20 5472 7565  lyMosaics = True
-0001f590: 2c0d 0a20 2061 7070 6c79 436c 6f75 6450  ,..  applyCloudP
-0001f5a0: 726f 6261 6269 6c69 7479 203d 2054 7275  robability = Tru
-0001f5b0: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
-0001f5c0: 6443 6c6f 7564 5363 6f72 654f 6666 7365  dCloudScoreOffse
-0001f5d0: 7420 3d20 4e6f 6e65 2c0d 0a20 2070 7265  t = None,..  pre
-0001f5e0: 436f 6d70 7574 6564 5444 4f4d 4952 4d65  ComputedTDOMIRMe
-0001f5f0: 616e 203d 204e 6f6e 652c 0d0a 2020 7072  an = None,..  pr
-0001f600: 6543 6f6d 7075 7465 6454 444f 4d49 5253  eComputedTDOMIRS
-0001f610: 7464 4465 7620 3d20 4e6f 6e65 2c0d 0a20  tdDev = None,.. 
-0001f620: 2063 6c6f 7564 5072 6f62 5468 7265 7368   cloudProbThresh
-0001f630: 203d 2034 3029 3a0d 0a0d 0a20 206f 7269   = 40):....  ori
-0001f640: 6769 6e20 3d20 2753 656e 7469 6e65 6c32  gin = 'Sentinel2
-0001f650: 270d 0a20 2074 6f61 4f72 5352 203d 2074  '..  toaOrSR = t
-0001f660: 6f61 4f72 5352 2e75 7070 6572 2829 0d0a  oaOrSR.upper()..
-0001f670: 0d0a 2020 6172 6773 203d 2066 6f72 6d61  ..  args = forma
-0001f680: 7441 7267 7328 6c6f 6361 6c73 2829 290d  tArgs(locals()).
-0001f690: 0a20 2069 6620 2761 7267 7327 2069 6e20  .  if 'args' in 
-0001f6a0: 6172 6773 2e6b 6579 7328 293a 0d0a 2020  args.keys():..  
-0001f6b0: 2020 6465 6c20 6172 6773 5b27 6172 6773    del args['args
-0001f6c0: 275d 0d0a 0d0a 2020 7332 7320 3d20 6765  ']....  s2s = ge
-0001f6d0: 7450 726f 6365 7373 6564 5365 6e74 696e  tProcessedSentin
-0001f6e0: 656c 3253 6365 6e65 7328 5c0d 0a20 2020  el2Scenes(\..   
-0001f6f0: 2073 7475 6479 4172 6561 203d 2073 7475   studyArea = stu
-0001f700: 6479 4172 6561 2c0d 0a20 2020 2073 7461  dyArea,..    sta
-0001f710: 7274 5965 6172 203d 2073 7461 7274 5965  rtYear = startYe
-0001f720: 6172 2c0d 0a20 2020 2065 6e64 5965 6172  ar,..    endYear
-0001f730: 203d 2065 6e64 5965 6172 2c0d 0a20 2020   = endYear,..   
-0001f740: 2073 7461 7274 4a75 6c69 616e 203d 2073   startJulian = s
-0001f750: 7461 7274 4a75 6c69 616e 2c0d 0a20 2020  tartJulian,..   
-0001f760: 2065 6e64 4a75 6c69 616e 203d 2065 6e64   endJulian = end
-0001f770: 4a75 6c69 616e 2c0d 0a20 2020 2061 7070  Julian,..    app
-0001f780: 6c79 5141 4261 6e64 203d 2061 7070 6c79  lyQABand = apply
-0001f790: 5141 4261 6e64 2c0d 0a20 2020 2061 7070  QABand,..    app
-0001f7a0: 6c79 436c 6f75 6453 636f 7265 203d 2061  lyCloudScore = a
-0001f7b0: 7070 6c79 436c 6f75 6453 636f 7265 2c0d  pplyCloudScore,.
-0001f7c0: 0a20 2020 2061 7070 6c79 5368 6164 6f77  .    applyShadow
-0001f7d0: 5368 6966 7420 3d20 6170 706c 7953 6861  Shift = applySha
-0001f7e0: 646f 7753 6869 6674 2c0d 0a20 2020 2061  dowShift,..    a
-0001f7f0: 7070 6c79 5444 4f4d 203d 2061 7070 6c79  pplyTDOM = apply
-0001f800: 5444 4f4d 2c0d 0a20 2020 2063 6c6f 7564  TDOM,..    cloud
-0001f810: 5363 6f72 6554 6872 6573 6820 3d20 636c  ScoreThresh = cl
-0001f820: 6f75 6453 636f 7265 5468 7265 7368 2c0d  oudScoreThresh,.
-0001f830: 0a20 2020 2070 6572 666f 726d 436c 6f75  .    performClou
-0001f840: 6453 636f 7265 4f66 6673 6574 203d 2070  dScoreOffset = p
-0001f850: 6572 666f 726d 436c 6f75 6453 636f 7265  erformCloudScore
-0001f860: 4f66 6673 6574 2c0d 0a20 2020 2063 6c6f  Offset,..    clo
-0001f870: 7564 5363 6f72 6550 6374 6c20 3d20 636c  udScorePctl = cl
-0001f880: 6f75 6453 636f 7265 5063 746c 2c0d 0a20  oudScorePctl,.. 
-0001f890: 2020 2063 6c6f 7564 4865 6967 6874 7320     cloudHeights 
-0001f8a0: 3d20 636c 6f75 6448 6569 6768 7473 2c0d  = cloudHeights,.
-0001f8b0: 0a20 2020 207a 5363 6f72 6554 6872 6573  .    zScoreThres
-0001f8c0: 6820 3d20 7a53 636f 7265 5468 7265 7368  h = zScoreThresh
-0001f8d0: 2c0d 0a20 2020 2073 6861 646f 7753 756d  ,..    shadowSum
-0001f8e0: 5468 7265 7368 203d 2073 6861 646f 7753  Thresh = shadowS
-0001f8f0: 756d 5468 7265 7368 2c0d 0a20 2020 2063  umThresh,..    c
-0001f900: 6f6e 7472 6163 7450 6978 656c 7320 3d20  ontractPixels = 
-0001f910: 636f 6e74 7261 6374 5069 7865 6c73 2c0d  contractPixels,.
-0001f920: 0a20 2020 2064 696c 6174 6550 6978 656c  .    dilatePixel
-0001f930: 7320 3d20 6469 6c61 7465 5069 7865 6c73  s = dilatePixels
-0001f940: 2c0d 0a20 2020 2073 6861 646f 7753 756d  ,..    shadowSum
-0001f950: 4261 6e64 7320 3d20 7368 6164 6f77 5375  Bands = shadowSu
-0001f960: 6d42 616e 6473 2c0d 0a20 2020 2072 6573  mBands,..    res
-0001f970: 616d 706c 654d 6574 686f 6420 3d20 7265  ampleMethod = re
-0001f980: 7361 6d70 6c65 4d65 7468 6f64 2c0d 0a20  sampleMethod,.. 
-0001f990: 2020 2074 6f61 4f72 5352 203d 2074 6f61     toaOrSR = toa
-0001f9a0: 4f72 5352 2c0d 0a20 2020 2063 6f6e 7665  OrSR,..    conve
-0001f9b0: 7274 546f 4461 696c 794d 6f73 6169 6373  rtToDailyMosaics
-0001f9c0: 203d 2063 6f6e 7665 7274 546f 4461 696c   = convertToDail
-0001f9d0: 794d 6f73 6169 6373 2c0d 0a20 2020 2061  yMosaics,..    a
-0001f9e0: 7070 6c79 436c 6f75 6450 726f 6261 6269  pplyCloudProbabi
-0001f9f0: 6c69 7479 203d 2061 7070 6c79 436c 6f75  lity = applyClou
-0001fa00: 6450 726f 6261 6269 6c69 7479 2c0d 0a20  dProbability,.. 
-0001fa10: 2020 2070 7265 436f 6d70 7574 6564 436c     preComputedCl
-0001fa20: 6f75 6453 636f 7265 4f66 6673 6574 203d  oudScoreOffset =
-0001fa30: 2070 7265 436f 6d70 7574 6564 436c 6f75   preComputedClou
-0001fa40: 6453 636f 7265 4f66 6673 6574 2c0d 0a20  dScoreOffset,.. 
-0001fa50: 2020 2070 7265 436f 6d70 7574 6564 5444     preComputedTD
-0001fa60: 4f4d 4952 4d65 616e 203d 2070 7265 436f  OMIRMean = preCo
-0001fa70: 6d70 7574 6564 5444 4f4d 4952 4d65 616e  mputedTDOMIRMean
-0001fa80: 2c0d 0a20 2020 2070 7265 436f 6d70 7574  ,..    preComput
-0001fa90: 6564 5444 4f4d 4952 5374 6444 6576 203d  edTDOMIRStdDev =
-0001faa0: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
-0001fab0: 4952 5374 6444 6576 2c0d 0a20 2020 2063  IRStdDev,..    c
-0001fac0: 6c6f 7564 5072 6f62 5468 7265 7368 203d  loudProbThresh =
-0001fad0: 2063 6c6f 7564 5072 6f62 5468 7265 7368   cloudProbThresh
-0001fae0: 290d 0a0d 0a20 2023 4164 6420 7a65 6e69  )....  #Add zeni
-0001faf0: 7468 2061 6e64 2061 7a69 6d75 7468 0d0a  th and azimuth..
-0001fb00: 2020 2369 6620 636f 7272 6563 7449 6c6c    #if correctIll
-0001fb10: 756d 696e 6174 696f 6e3a 0d0a 2020 2320  umination:..  # 
-0001fb20: 2073 3273 203d 2073 3273 2e6d 6170 2866   s2s = s2s.map(f
-0001fb30: 756e 6374 696f 6e28 696d 6729 7b0d 0a20  unction(img){.. 
-0001fb40: 2023 2020 2020 7265 7475 726e 2061 6464   #    return add
-0001fb50: 5a65 6e69 7468 417a 696d 7574 6828 696d  ZenithAzimuth(im
-0001fb60: 672c 2754 4f41 272c 7b27 544f 4127 3a27  g,'TOA',{'TOA':'
-0001fb70: 4d45 414e 5f53 4f4c 4152 5f5a 454e 4954  MEAN_SOLAR_ZENIT
-0001fb80: 485f 414e 474c 4527 7d2c 7b27 544f 4127  H_ANGLE'},{'TOA'
-0001fb90: 3a27 4d45 414e 5f53 4f4c 4152 5f41 5a49  :'MEAN_SOLAR_AZI
-0001fba0: 4d55 5448 5f41 4e47 4c45 277d 293b 0d0a  MUTH_ANGLE'});..
-0001fbb0: 2020 2320 207d 293b 0d0a 2020 237d 0d0a    #  });..  #}..
-0001fbc0: 0d0a 2020 2343 7265 6174 6520 636f 6d70  ..  #Create comp
-0001fbd0: 6f73 6974 6520 7469 6d65 2073 6572 6965  osite time serie
-0001fbe0: 730d 0a20 2074 7320 3d20 636f 6d70 6f73  s..  ts = compos
-0001fbf0: 6974 6554 696d 6553 6572 6965 7328 5c0d  iteTimeSeries(\.
-0001fc00: 0a20 2020 206c 7320 3d20 7332 732c 0d0a  .    ls = s2s,..
-0001fc10: 2020 2020 7374 6172 7459 6561 7220 3d20      startYear = 
-0001fc20: 7374 6172 7459 6561 722c 0d0a 2020 2020  startYear,..    
-0001fc30: 656e 6459 6561 7220 3d20 656e 6459 6561  endYear = endYea
-0001fc40: 722c 0d0a 2020 2020 7374 6172 744a 756c  r,..    startJul
-0001fc50: 6961 6e20 3d20 7374 6172 744a 756c 6961  ian = startJulia
-0001fc60: 6e2c 0d0a 2020 2020 656e 644a 756c 6961  n,..    endJulia
-0001fc70: 6e20 3d20 656e 644a 756c 6961 6e2c 0d0a  n = endJulian,..
-0001fc80: 2020 2020 7469 6d65 6275 6666 6572 203d      timebuffer =
-0001fc90: 2074 696d 6562 7566 6665 722c 0d0a 2020   timebuffer,..  
-0001fca0: 2020 7765 6967 6874 7320 3d20 7765 6967    weights = weig
-0001fcb0: 6874 732c 0d0a 2020 2020 636f 6d70 6f73  hts,..    compos
-0001fcc0: 6974 696e 674d 6574 686f 6420 3d20 636f  itingMethod = co
-0001fcd0: 6d70 6f73 6974 696e 674d 6574 686f 6429  mpositingMethod)
-0001fce0: 0d0a 0d0a 2020 2343 6f72 7265 6374 2069  ....  #Correct i
-0001fcf0: 6c6c 756d 696e 6174 696f 6e0d 0a20 2023  llumination..  #
-0001fd00: 2069 6620 2863 6f72 7265 6374 496c 6c75   if (correctIllu
-0001fd10: 6d69 6e61 7469 6f6e 297b 0d0a 2020 2320  mination){..  # 
-0001fd20: 2020 6620 3d20 6565 2e49 6d61 6765 2874    f = ee.Image(t
-0001fd30: 732e 6669 7273 7428 2929 3b0d 0a20 2023  s.first());..  #
-0001fd40: 2020 204d 6170 2e61 6464 4c61 7965 7228     Map.addLayer(
-0001fd50: 662c 7669 7a50 6172 616d 7346 616c 7365  f,vizParamsFalse
-0001fd60: 2c27 4669 7273 742d 6e6f 6e2d 696c 6c75  ,'First-non-illu
-0001fd70: 6d69 6e61 7465 6427 2c66 616c 7365 293b  minated',false);
-0001fd80: 0d0a 0d0a 2020 2320 2020 7072 696e 7428  ....  #   print(
-0001fd90: 2743 6f72 7265 6374 696e 6720 696c 6c75  'Correcting illu
-0001fda0: 6d69 6e61 7469 6f6e 2729 3b0d 0a20 2023  mination');..  #
-0001fdb0: 2020 2074 7320 3d20 7473 2e6d 6170 2869     ts = ts.map(i
-0001fdc0: 6c6c 756d 696e 6174 696f 6e43 6f6e 6469  lluminationCondi
-0001fdd0: 7469 6f6e 290d 0a20 2023 2020 2020 202e  tion)..  #     .
-0001fde0: 6d61 7028 6675 6e63 7469 6f6e 2869 6d67  map(function(img
-0001fdf0: 297b 0d0a 2020 2320 2020 2020 2020 7265  ){..  #       re
-0001fe00: 7475 726e 2069 6c6c 756d 696e 6174 696f  turn illuminatio
-0001fe10: 6e43 6f72 7265 6374 696f 6e28 696d 672c  nCorrection(img,
-0001fe20: 2063 6f72 7265 6374 5363 616c 652c 7374   correctScale,st
-0001fe30: 7564 7941 7265 612c 5b20 2762 6c75 6527  udyArea,[ 'blue'
-0001fe40: 2c20 2767 7265 656e 272c 2027 7265 6427  , 'green', 'red'
-0001fe50: 2c27 6e69 7227 2c27 7377 6972 3127 2c20  ,'nir','swir1', 
-0001fe60: 2773 7769 7232 275d 293b 0d0a 2020 2320  'swir2']);..  # 
-0001fe70: 2020 2020 7d29 3b0d 0a20 2023 2020 2066      });..  #   f
-0001fe80: 203d 2065 652e 496d 6167 6528 7473 2e66   = ee.Image(ts.f
-0001fe90: 6972 7374 2829 293b 0d0a 2020 2320 2020  irst());..  #   
-0001fea0: 4d61 702e 6164 644c 6179 6572 2866 2c76  Map.addLayer(f,v
-0001feb0: 697a 5061 7261 6d73 4661 6c73 652c 2746  izParamsFalse,'F
-0001fec0: 6972 7374 2d69 6c6c 756d 696e 6174 6564  irst-illuminated
-0001fed0: 272c 6661 6c73 6529 3b0d 0a0d 0a20 2023  ',false);....  #
-0001fee0: 2045 7870 6f72 7420 636f 6d70 6f73 6974   Export composit
-0001fef0: 6573 0d0a 2020 6966 2065 7870 6f72 7443  es..  if exportC
-0001ff00: 6f6d 706f 7369 7465 733a 0d0a 2020 2020  omposites:..    
-0001ff10: 6578 706f 7274 4261 6e64 4469 6374 203d  exportBandDict =
-0001ff20: 207b 5c0d 0a20 2020 2020 2027 5352 5f6d   {\..      'SR_m
-0001ff30: 6564 6f69 6427 3a5b 2763 6227 2c20 2762  edoid':['cb', 'b
-0001ff40: 6c75 6527 2c20 2767 7265 656e 272c 2027  lue', 'green', '
-0001ff50: 7265 6427 2c20 2772 6531 272c 2772 6532  red', 're1','re2
-0001ff60: 272c 2772 6533 272c 276e 6972 272c 2027  ','re3','nir', '
-0001ff70: 6e69 7232 272c 2027 7761 7465 7256 6170  nir2', 'waterVap
-0001ff80: 6f72 272c 2027 7377 6972 3127 2c20 2773  or', 'swir1', 's
-0001ff90: 7769 7232 272c 2763 6f6d 706f 7369 7465  wir2','composite
-0001ffa0: 4f62 7343 6f75 6e74 272c 2773 656e 736f  ObsCount','senso
-0001ffb0: 7227 2c27 7965 6172 272c 276a 756c 6961  r','year','julia
-0001ffc0: 6e44 6179 275d 2c0d 0a20 2020 2020 2027  nDay'],..      '
-0001ffd0: 5352 5f6d 6564 6961 6e27 3a5b 2763 6227  SR_median':['cb'
-0001ffe0: 2c20 2762 6c75 6527 2c20 2767 7265 656e  , 'blue', 'green
-0001fff0: 272c 2027 7265 6427 2c20 2772 6531 272c  ', 'red', 're1',
-00020000: 2772 6532 272c 2772 6533 272c 276e 6972  're2','re3','nir
-00020010: 272c 2027 6e69 7232 272c 2027 7761 7465  ', 'nir2', 'wate
-00020020: 7256 6170 6f72 272c 2027 7377 6972 3127  rVapor', 'swir1'
-00020030: 2c20 2773 7769 7232 272c 2763 6f6d 706f  , 'swir2','compo
-00020040: 7369 7465 4f62 7343 6f75 6e74 275d 2c0d  siteObsCount'],.
-00020050: 0a20 2020 2020 2027 544f 415f 6d65 646f  .      'TOA_medo
-00020060: 6964 273a 5b27 6362 272c 2027 626c 7565  id':['cb', 'blue
-00020070: 272c 2027 6772 6565 6e27 2c20 2772 6564  ', 'green', 'red
-00020080: 272c 2027 7265 3127 2c27 7265 3227 2c27  ', 're1','re2','
-00020090: 7265 3327 2c27 6e69 7227 2c20 276e 6972  re3','nir', 'nir
-000200a0: 3227 2c20 2777 6174 6572 5661 706f 7227  2', 'waterVapor'
-000200b0: 2c20 2763 6972 7275 7327 2c20 2773 7769  , 'cirrus', 'swi
-000200c0: 7231 272c 2027 7377 6972 3227 2c27 636f  r1', 'swir2','co
-000200d0: 6d70 6f73 6974 654f 6273 436f 756e 7427  mpositeObsCount'
-000200e0: 2c27 7365 6e73 6f72 272c 2779 6561 7227  ,'sensor','year'
-000200f0: 2c27 6a75 6c69 616e 4461 7927 5d2c 0d0a  ,'julianDay'],..
-00020100: 2020 2020 2020 2754 4f41 5f6d 6564 6961        'TOA_media
-00020110: 6e27 3a5b 2763 6227 2c20 2762 6c75 6527  n':['cb', 'blue'
-00020120: 2c20 2767 7265 656e 272c 2027 7265 6427  , 'green', 'red'
-00020130: 2c20 2772 6531 272c 2772 6532 272c 2772  , 're1','re2','r
-00020140: 6533 272c 276e 6972 272c 2027 6e69 7232  e3','nir', 'nir2
-00020150: 272c 2027 7761 7465 7256 6170 6f72 272c  ', 'waterVapor',
-00020160: 2027 6369 7272 7573 272c 2027 7377 6972   'cirrus', 'swir
-00020170: 3127 2c20 2773 7769 7232 272c 2763 6f6d  1', 'swir2','com
-00020180: 706f 7369 7465 4f62 7343 6f75 6e74 275d  positeObsCount']
-00020190: 5c0d 0a20 2020 207d 0d0a 2020 2020 6e6f  \..    }..    no
-000201a0: 6e44 6976 6964 6542 616e 6444 6963 7420  nDivideBandDict 
-000201b0: 3d20 7b5c 0d0a 2020 2020 2020 276d 6564  = {\..      'med
-000201c0: 6f69 6427 3a5b 2763 6f6d 706f 7369 7465  oid':['composite
-000201d0: 4f62 7343 6f75 6e74 272c 2773 656e 736f  ObsCount','senso
-000201e0: 7227 2c27 7965 6172 272c 276a 756c 6961  r','year','julia
-000201f0: 6e44 6179 275d 2c0d 0a20 2020 2020 2027  nDay'],..      '
-00020200: 6d65 6469 616e 273a 5b27 636f 6d70 6f73  median':['compos
-00020210: 6974 654f 6273 436f 756e 7427 5d5c 0d0a  iteObsCount']\..
-00020220: 2020 2020 7d0d 0a20 2020 2065 7870 6f72      }..    expor
-00020230: 7442 616e 6473 203d 2065 7870 6f72 7442  tBands = exportB
-00020240: 616e 6444 6963 745b 746f 614f 7253 5220  andDict[toaOrSR 
-00020250: 2b20 275f 2720 2b20 636f 6d70 6f73 6974  + '_' + composit
-00020260: 696e 674d 6574 686f 645d 0d0a 2020 2020  ingMethod]..    
-00020270: 6e6f 6e44 6976 6964 6542 616e 6473 203d  nonDivideBands =
-00020280: 206e 6f6e 4469 7669 6465 4261 6e64 4469   nonDivideBandDi
-00020290: 6374 5b63 6f6d 706f 7369 7469 6e67 4d65  ct[compositingMe
-000202a0: 7468 6f64 5d0d 0a0d 0a20 2020 2065 7870  thod]....    exp
-000202b0: 6f72 7443 6f6d 706f 7369 7465 436f 6c6c  ortCompositeColl
-000202c0: 6563 7469 6f6e 285c 0d0a 2020 2020 2020  ection(\..      
-000202d0: 636f 6c6c 6563 7469 6f6e 203d 2074 732c  collection = ts,
-000202e0: 0d0a 2020 2020 2020 6578 706f 7274 5061  ..      exportPa
-000202f0: 7468 526f 6f74 203d 2065 7870 6f72 7450  thRoot = exportP
-00020300: 6174 6852 6f6f 742c 0d0a 2020 2020 2020  athRoot,..      
-00020310: 6f75 7470 7574 4e61 6d65 203d 206f 7574  outputName = out
-00020320: 7075 744e 616d 652c 0d0a 2020 2020 2020  putName,..      
-00020330: 6f72 6967 696e 203d 206f 7269 6769 6e2c  origin = origin,
-00020340: 0d0a 2020 2020 2020 7374 7564 7941 7265  ..      studyAre
-00020350: 6120 3d20 7374 7564 7941 7265 612c 0d0a  a = studyArea,..
-00020360: 2020 2020 2020 6372 7320 3d20 6372 732c        crs = crs,
-00020370: 0d0a 2020 2020 2020 7472 616e 7366 6f72  ..      transfor
-00020380: 6d20 3d20 7472 616e 7366 6f72 6d2c 0d0a  m = transform,..
-00020390: 2020 2020 2020 7363 616c 6520 3d20 7363        scale = sc
-000203a0: 616c 652c 0d0a 2020 2020 2020 7374 6172  ale,..      star
-000203b0: 7459 6561 7220 3d20 7374 6172 7459 6561  tYear = startYea
-000203c0: 722c 0d0a 2020 2020 2020 656e 6459 6561  r,..      endYea
-000203d0: 7220 3d20 656e 6459 6561 722c 0d0a 2020  r = endYear,..  
-000203e0: 2020 2020 7374 6172 744a 756c 6961 6e20      startJulian 
-000203f0: 3d20 7374 6172 744a 756c 6961 6e2c 0d0a  = startJulian,..
-00020400: 2020 2020 2020 656e 644a 756c 6961 6e20        endJulian 
-00020410: 3d20 656e 644a 756c 6961 6e2c 0d0a 2020  = endJulian,..  
-00020420: 2020 2020 636f 6d70 6f73 6974 696e 674d      compositingM
-00020430: 6574 686f 6420 3d20 636f 6d70 6f73 6974  ethod = composit
-00020440: 696e 674d 6574 686f 642c 0d0a 2020 2020  ingMethod,..    
-00020450: 2020 7469 6d65 6275 6666 6572 203d 2074    timebuffer = t
-00020460: 696d 6562 7566 6665 722c 0d0a 2020 2020  imebuffer,..    
-00020470: 2020 746f 614f 7253 5220 3d20 746f 614f    toaOrSR = toaO
-00020480: 7253 522c 0d0a 2020 2020 2020 6e6f 6e44  rSR,..      nonD
-00020490: 6976 6964 6542 616e 6473 203d 206e 6f6e  ivideBands = non
-000204a0: 4469 7669 6465 4261 6e64 732c 0d0a 2020  DivideBands,..  
-000204b0: 2020 2020 6578 706f 7274 4261 6e64 7320      exportBands 
-000204c0: 3d20 6578 706f 7274 4261 6e64 732c 0d0a  = exportBands,..
-000204d0: 2020 2020 2020 6164 6469 7469 6f6e 616c        additional
-000204e0: 5072 6f70 6572 7479 4469 6374 203d 2061  PropertyDict = a
-000204f0: 7267 7329 0d0a 0d0a 2020 6172 6773 5b27  rgs)....  args['
-00020500: 7072 6f63 6573 7365 6453 6365 6e65 7327  processedScenes'
-00020510: 5d20 3d20 7332 730d 0a20 2061 7267 735b  ] = s2s..  args[
-00020520: 2770 726f 6365 7373 6564 436f 6d70 6f73  'processedCompos
-00020530: 6974 6573 275d 203d 2074 730d 0a0d 0a20  ites'] = ts.... 
-00020540: 2072 6574 7572 6e20 6172 6773 0d0a 0d0a   return args....
-00020550: 2320 4879 6272 6964 2067 6574 204c 616e  # Hybrid get Lan
-00020560: 6473 6174 2061 6e64 2053 656e 7469 6e65  dsat and Sentine
-00020570: 6c20 3220 7072 6f63 6573 7365 6420 7363  l 2 processed sc
-00020580: 656e 6573 0d0a 2320 4861 6e64 6c65 7320  enes..# Handles 
-00020590: 6765 7474 696e 6720 7072 6f63 6573 7365  getting processe
-000205a0: 6420 7363 656e 6573 2020 7769 7468 204c  d scenes  with L
-000205b0: 616e 6473 6174 2061 6e64 2053 656e 7469  andsat and Senti
-000205c0: 6e65 6c20 320d 0a64 6566 2067 6574 5072  nel 2..def getPr
-000205d0: 6f63 6573 7365 644c 616e 6473 6174 416e  ocessedLandsatAn
-000205e0: 6453 656e 7469 6e65 6c32 5363 656e 6573  dSentinel2Scenes
-000205f0: 280d 0a20 2020 2020 2073 7475 6479 4172  (..      studyAr
-00020600: 6561 2c0d 0a20 2020 2020 2073 7461 7274  ea,..      start
-00020610: 5965 6172 2c0d 0a20 2020 2020 2065 6e64  Year,..      end
-00020620: 5965 6172 2c0d 0a20 2020 2020 2073 7461  Year,..      sta
-00020630: 7274 4a75 6c69 616e 2c0d 0a20 2020 2020  rtJulian,..     
-00020640: 2065 6e64 4a75 6c69 616e 2c0d 0a20 2020   endJulian,..   
-00020650: 2020 2074 6f61 4f72 5352 203d 2027 544f     toaOrSR = 'TO
-00020660: 4127 2c0d 0a20 2020 2020 2069 6e63 6c75  A',..      inclu
-00020670: 6465 534c 434f 6666 4c37 203d 2046 616c  deSLCOffL7 = Fal
-00020680: 7365 2c0d 0a20 2020 2020 2064 6566 7269  se,..      defri
-00020690: 6e67 654c 3520 3d20 4661 6c73 652c 0d0a  ngeL5 = False,..
-000206a0: 2020 2020 2020 6170 706c 7951 4142 616e        applyQABan
-000206b0: 6420 3d20 4661 6c73 652c 0d0a 2020 2020  d = False,..    
-000206c0: 2020 6170 706c 7943 6c6f 7564 5072 6f62    applyCloudProb
-000206d0: 6162 696c 6974 7920 3d20 5472 7565 2c0d  ability = True,.
-000206e0: 0a20 2020 2020 2061 7070 6c79 5368 6164  .      applyShad
-000206f0: 6f77 5368 6966 7420 3d20 4661 6c73 652c  owShift = False,
-00020700: 0d0a 2020 2020 2020 6170 706c 7943 6c6f  ..      applyClo
-00020710: 7564 5363 6f72 654c 616e 6473 6174 203d  udScoreLandsat =
-00020720: 2046 616c 7365 2c0d 0a20 2020 2020 2061   False,..      a
-00020730: 7070 6c79 436c 6f75 6453 636f 7265 5365  pplyCloudScoreSe
-00020740: 6e74 696e 656c 3220 3d20 4661 6c73 652c  ntinel2 = False,
-00020750: 0d0a 2020 2020 2020 6170 706c 7954 444f  ..      applyTDO
-00020760: 4d4c 616e 6473 6174 203d 2054 7275 652c  MLandsat = True,
-00020770: 0d0a 2020 2020 2020 6170 706c 7954 444f  ..      applyTDO
-00020780: 4d53 656e 7469 6e65 6c32 203d 2054 7275  MSentinel2 = Tru
-00020790: 652c 0d0a 2020 2020 2020 6170 706c 7946  e,..      applyF
-000207a0: 6d61 736b 436c 6f75 644d 6173 6b20 3d20  maskCloudMask = 
-000207b0: 5472 7565 2c0d 0a20 2020 2020 2061 7070  True,..      app
-000207c0: 6c79 466d 6173 6b43 6c6f 7564 5368 6164  lyFmaskCloudShad
-000207d0: 6f77 4d61 736b 203d 2054 7275 652c 0d0a  owMask = True,..
-000207e0: 2020 2020 2020 6170 706c 7946 6d61 736b        applyFmask
-000207f0: 536e 6f77 4d61 736b 203d 2046 616c 7365  SnowMask = False
-00020800: 2c0d 0a20 2020 2020 2063 6c6f 7564 4865  ,..      cloudHe
-00020810: 6967 6874 7320 3d20 6565 2e4c 6973 742e  ights = ee.List.
-00020820: 7365 7175 656e 6365 2835 3030 2c31 3030  sequence(500,100
-00020830: 3030 2c35 3030 292c 0d0a 2020 2020 2020  00,500),..      
-00020840: 636c 6f75 6453 636f 7265 5468 7265 7368  cloudScoreThresh
-00020850: 203d 2032 302c 0d0a 2020 2020 2020 7065   = 20,..      pe
-00020860: 7266 6f72 6d43 6c6f 7564 5363 6f72 654f  rformCloudScoreO
-00020870: 6666 7365 7420 3d20 5472 7565 2c0d 0a20  ffset = True,.. 
-00020880: 2020 2020 2063 6c6f 7564 5363 6f72 6550       cloudScoreP
-00020890: 6374 6c20 3d20 3130 2c0d 0a20 2020 2020  ctl = 10,..     
-000208a0: 207a 5363 6f72 6554 6872 6573 6820 3d20   zScoreThresh = 
-000208b0: 2d31 2c0d 0a20 2020 2020 2073 6861 646f  -1,..      shado
-000208c0: 7753 756d 5468 7265 7368 203d 2030 2e33  wSumThresh = 0.3
-000208d0: 352c 0d0a 2020 2020 2020 636f 6e74 7261  5,..      contra
-000208e0: 6374 5069 7865 6c73 203d 2031 2e35 2c0d  ctPixels = 1.5,.
-000208f0: 0a20 2020 2020 2064 696c 6174 6550 6978  .      dilatePix
-00020900: 656c 7320 3d20 332e 352c 0d0a 2020 2020  els = 3.5,..    
-00020910: 2020 7368 6164 6f77 5375 6d42 616e 6473    shadowSumBands
-00020920: 203d 205b 276e 6972 272c 2773 7769 7231   = ['nir','swir1
-00020930: 275d 2c0d 0a20 2020 2020 206c 616e 6473  '],..      lands
-00020940: 6174 5265 7361 6d70 6c65 4d65 7468 6f64  atResampleMethod
-00020950: 203d 2027 6e65 6172 272c 0d0a 2020 2020   = 'near',..    
-00020960: 2020 7365 6e74 696e 656c 3252 6573 616d    sentinel2Resam
-00020970: 706c 654d 6574 686f 6420 3d20 2761 6767  pleMethod = 'agg
-00020980: 7265 6761 7465 272c 0d0a 2020 2020 2020  regate',..      
-00020990: 636f 6e76 6572 7454 6f44 6169 6c79 4d6f  convertToDailyMo
-000209a0: 7361 6963 7320 3d20 5472 7565 2c0d 0a20  saics = True,.. 
-000209b0: 2020 2020 2072 756e 4368 6173 7461 696e       runChastain
-000209c0: 4861 726d 6f6e 697a 6174 696f 6e20 3d20  Harmonization = 
-000209d0: 5472 7565 2c0d 0a20 2020 2020 2063 6f72  True,..      cor
-000209e0: 7265 6374 496c 6c75 6d69 6e61 7469 6f6e  rectIllumination
-000209f0: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-00020a00: 2063 6f72 7265 6374 5363 616c 6520 3d20   correctScale = 
-00020a10: 3235 302c 0d0a 2020 2020 2020 7072 6543  250,..      preC
-00020a20: 6f6d 7075 7465 644c 616e 6473 6174 436c  omputedLandsatCl
-00020a30: 6f75 6453 636f 7265 4f66 6673 6574 203d  oudScoreOffset =
-00020a40: 204e 6f6e 652c 0d0a 2020 2020 2020 7072   None,..      pr
-00020a50: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
-00020a60: 5444 4f4d 4952 4d65 616e 203d 204e 6f6e  TDOMIRMean = Non
-00020a70: 652c 0d0a 2020 2020 2020 7072 6543 6f6d  e,..      preCom
-00020a80: 7075 7465 644c 616e 6473 6174 5444 4f4d  putedLandsatTDOM
-00020a90: 4952 5374 6444 6576 203d 204e 6f6e 652c  IRStdDev = None,
-00020aa0: 0d0a 2020 2020 2020 7072 6543 6f6d 7075  ..      preCompu
-00020ab0: 7465 6453 656e 7469 6e65 6c32 436c 6f75  tedSentinel2Clou
-00020ac0: 6453 636f 7265 4f66 6673 6574 203d 204e  dScoreOffset = N
-00020ad0: 6f6e 652c 0d0a 2020 2020 2020 7072 6543  one,..      preC
-00020ae0: 6f6d 7075 7465 6453 656e 7469 6e65 6c32  omputedSentinel2
-00020af0: 5444 4f4d 4952 4d65 616e 203d 204e 6f6e  TDOMIRMean = Non
-00020b00: 652c 0d0a 2020 2020 2020 7072 6543 6f6d  e,..      preCom
-00020b10: 7075 7465 6453 656e 7469 6e65 6c32 5444  putedSentinel2TD
-00020b20: 4f4d 4952 5374 6444 6576 203d 204e 6f6e  OMIRStdDev = Non
-00020b30: 652c 0d0a 2020 2020 2020 636c 6f75 6450  e,..      cloudP
-00020b40: 726f 6254 6872 6573 6820 3d20 3430 2c0d  robThresh = 40,.
-00020b50: 0a20 2020 2020 206c 616e 6473 6174 436f  .      landsatCo
-00020b60: 6c6c 6563 7469 6f6e 5665 7273 696f 6e20  llectionVersion 
-00020b70: 3d20 2743 3227 293a 0d0a 0d0a 2020 6966  = 'C2'):....  if
-00020b80: 2074 6f61 4f72 5352 203d 3d20 2753 5227   toaOrSR == 'SR'
-00020b90: 3a0d 0a20 2020 2072 756e 4368 6173 7461  :..    runChasta
-00020ba0: 696e 4861 726d 6f6e 697a 6174 696f 6e20  inHarmonization 
-00020bb0: 3d20 4661 6c73 650d 0a0d 0a20 206f 7269  = False....  ori
-00020bc0: 6769 6e20 3d20 274c 616e 6473 6174 2d53  gin = 'Landsat-S
-00020bd0: 656e 7469 6e65 6c32 2d48 7962 7269 6427  entinel2-Hybrid'
-00020be0: 0d0a 2020 746f 614f 7253 5220 3d20 746f  ..  toaOrSR = to
-00020bf0: 614f 7253 522e 7570 7065 7228 290d 0a0d  aOrSR.upper()...
-00020c00: 0a20 2023 5072 6570 6172 6520 6461 7465  .  #Prepare date
-00020c10: 730d 0a20 2023 5772 6170 2074 6865 2064  s..  #Wrap the d
-00020c20: 6174 6573 2069 6620 6e65 6564 6564 0d0a  ates if needed..
-00020c30: 2020 7772 6170 4f66 6673 6574 203d 2030    wrapOffset = 0
-00020c40: 0d0a 2020 6966 2073 7461 7274 4a75 6c69  ..  if startJuli
-00020c50: 616e 203e 2065 6e64 4a75 6c69 616e 3a0d  an > endJulian:.
-00020c60: 0a20 2020 2077 7261 704f 6666 7365 7420  .    wrapOffset 
-00020c70: 3d20 3336 350d 0a20 2073 7461 7274 4461  = 365..  startDa
-00020c80: 7465 203d 2065 652e 4461 7465 2e66 726f  te = ee.Date.fro
-00020c90: 6d59 4d44 2873 7461 7274 5965 6172 2c31  mYMD(startYear,1
-00020ca0: 2c31 292e 6164 7661 6e63 6528 7374 6172  ,1).advance(star
-00020cb0: 744a 756c 6961 6e2d 312c 2764 6179 2729  tJulian-1,'day')
-00020cc0: 0d0a 2020 656e 6444 6174 6520 3d20 6565  ..  endDate = ee
-00020cd0: 2e44 6174 652e 6672 6f6d 594d 4428 656e  .Date.fromYMD(en
-00020ce0: 6459 6561 722c 312c 3129 2e61 6476 616e  dYear,1,1).advan
-00020cf0: 6365 2865 6e64 4a75 6c69 616e 2d31 2b77  ce(endJulian-1+w
-00020d00: 7261 704f 6666 7365 742c 2764 6179 2729  rapOffset,'day')
-00020d10: 0d0a 0d0a 2020 6172 6773 203d 2066 6f72  ....  args = for
-00020d20: 6d61 7441 7267 7328 6c6f 6361 6c73 2829  matArgs(locals()
-00020d30: 290d 0a20 2069 6620 2761 7267 7327 2069  )..  if 'args' i
-00020d40: 6e20 6172 6773 2e6b 6579 7328 293a 0d0a  n args.keys():..
-00020d50: 2020 2020 6465 6c20 6172 6773 5b27 6172      del args['ar
-00020d60: 6773 275d 0d0a 0d0a 2020 7072 696e 7428  gs']....  print(
-00020d70: 2747 6574 2050 726f 6365 7373 6564 204c  'Get Processed L
-00020d80: 616e 6473 6174 2061 6e64 2053 656e 7469  andsat and Senti
-00020d90: 6e65 6c32 2053 6365 6e65 733a 2027 290d  nel2 Scenes: ').
-00020da0: 0a20 2070 7269 6e74 2827 5374 6172 7420  .  print('Start 
-00020db0: 6461 7465 3a27 2c20 7374 6172 7444 6174  date:', startDat
-00020dc0: 652e 666f 726d 6174 2827 4d4d 4d20 6464  e.format('MMM dd
-00020dd0: 2079 7979 7927 292e 6765 7449 6e66 6f28   yyyy').getInfo(
-00020de0: 292c 272c 2045 6e64 2064 6174 653a 272c  ),', End date:',
-00020df0: 2065 6e64 4461 7465 2e66 6f72 6d61 7428   endDate.format(
-00020e00: 274d 4d4d 2064 6420 7979 7979 2729 2e67  'MMM dd yyyy').g
-00020e10: 6574 496e 666f 2829 290d 0a20 2066 6f72  etInfo())..  for
-00020e20: 2061 7267 2069 6e20 6172 6773 2e6b 6579   arg in args.key
-00020e30: 7328 293a 0d0a 2020 2020 7072 696e 7428  s():..    print(
-00020e40: 6172 672c 2027 3a20 272c 2061 7267 735b  arg, ': ', args[
-00020e50: 6172 675d 290d 0a0d 0a20 2023 4765 7420  arg])....  #Get 
-00020e60: 4c61 6e64 7361 740d 0a20 206c 7320 3d20  Landsat..  ls = 
-00020e70: 6765 7450 726f 6365 7373 6564 4c61 6e64  getProcessedLand
-00020e80: 7361 7453 6365 6e65 7328 5c0d 0a20 2020  satScenes(\..   
-00020e90: 2073 7475 6479 4172 6561 203d 2073 7475   studyArea = stu
-00020ea0: 6479 4172 6561 2c0d 0a20 2020 2073 7461  dyArea,..    sta
-00020eb0: 7274 5965 6172 203d 2073 7461 7274 5965  rtYear = startYe
-00020ec0: 6172 2c0d 0a20 2020 2065 6e64 5965 6172  ar,..    endYear
-00020ed0: 203d 2065 6e64 5965 6172 2c0d 0a20 2020   = endYear,..   
-00020ee0: 2073 7461 7274 4a75 6c69 616e 203d 2073   startJulian = s
-00020ef0: 7461 7274 4a75 6c69 616e 2c0d 0a20 2020  tartJulian,..   
-00020f00: 2065 6e64 4a75 6c69 616e 203d 2065 6e64   endJulian = end
-00020f10: 4a75 6c69 616e 2c0d 0a20 2020 2074 6f61  Julian,..    toa
-00020f20: 4f72 5352 203d 2074 6f61 4f72 5352 2c0d  OrSR = toaOrSR,.
-00020f30: 0a20 2020 2069 6e63 6c75 6465 534c 434f  .    includeSLCO
-00020f40: 6666 4c37 203d 2069 6e63 6c75 6465 534c  ffL7 = includeSL
-00020f50: 434f 6666 4c37 2c0d 0a20 2020 2064 6566  COffL7,..    def
-00020f60: 7269 6e67 654c 3520 3d20 6465 6672 696e  ringeL5 = defrin
-00020f70: 6765 4c35 2c0d 0a20 2020 2061 7070 6c79  geL5,..    apply
-00020f80: 436c 6f75 6453 636f 7265 203d 2061 7070  CloudScore = app
-00020f90: 6c79 436c 6f75 6453 636f 7265 4c61 6e64  lyCloudScoreLand
-00020fa0: 7361 742c 0d0a 2020 2020 6170 706c 7946  sat,..    applyF
-00020fb0: 6d61 736b 436c 6f75 644d 6173 6b20 3d20  maskCloudMask = 
-00020fc0: 6170 706c 7946 6d61 736b 436c 6f75 644d  applyFmaskCloudM
-00020fd0: 6173 6b2c 0d0a 2020 2020 6170 706c 7954  ask,..    applyT
-00020fe0: 444f 4d20 3d20 6170 706c 7954 444f 4d4c  DOM = applyTDOML
-00020ff0: 616e 6473 6174 2c0d 0a20 2020 2061 7070  andsat,..    app
-00021000: 6c79 466d 6173 6b43 6c6f 7564 5368 6164  lyFmaskCloudShad
-00021010: 6f77 4d61 736b 203d 2061 7070 6c79 466d  owMask = applyFm
-00021020: 6173 6b43 6c6f 7564 5368 6164 6f77 4d61  askCloudShadowMa
-00021030: 736b 2c0d 0a20 2020 2061 7070 6c79 466d  sk,..    applyFm
-00021040: 6173 6b53 6e6f 774d 6173 6b20 3d20 6170  askSnowMask = ap
-00021050: 706c 7946 6d61 736b 536e 6f77 4d61 736b  plyFmaskSnowMask
-00021060: 2c0d 0a20 2020 2063 6c6f 7564 5363 6f72  ,..    cloudScor
-00021070: 6554 6872 6573 6820 3d20 636c 6f75 6453  eThresh = cloudS
-00021080: 636f 7265 5468 7265 7368 2c0d 0a20 2020  coreThresh,..   
-00021090: 2070 6572 666f 726d 436c 6f75 6453 636f   performCloudSco
-000210a0: 7265 4f66 6673 6574 203d 2070 6572 666f  reOffset = perfo
-000210b0: 726d 436c 6f75 6453 636f 7265 4f66 6673  rmCloudScoreOffs
-000210c0: 6574 2c0d 0a20 2020 2063 6c6f 7564 5363  et,..    cloudSc
-000210d0: 6f72 6550 6374 6c20 3d20 636c 6f75 6453  orePctl = cloudS
-000210e0: 636f 7265 5063 746c 2c0d 0a20 2020 207a  corePctl,..    z
-000210f0: 5363 6f72 6554 6872 6573 6820 3d20 7a53  ScoreThresh = zS
-00021100: 636f 7265 5468 7265 7368 2c0d 0a20 2020  coreThresh,..   
-00021110: 2073 6861 646f 7753 756d 5468 7265 7368   shadowSumThresh
-00021120: 203d 2073 6861 646f 7753 756d 5468 7265   = shadowSumThre
-00021130: 7368 2c0d 0a20 2020 2063 6f6e 7472 6163  sh,..    contrac
-00021140: 7450 6978 656c 7320 3d20 636f 6e74 7261  tPixels = contra
-00021150: 6374 5069 7865 6c73 2c0d 0a20 2020 2064  ctPixels,..    d
-00021160: 696c 6174 6550 6978 656c 7320 3d20 6469  ilatePixels = di
-00021170: 6c61 7465 5069 7865 6c73 2c0d 0a20 2020  latePixels,..   
-00021180: 2073 6861 646f 7753 756d 4261 6e64 7320   shadowSumBands 
-00021190: 3d20 7368 6164 6f77 5375 6d42 616e 6473  = shadowSumBands
-000211a0: 2c0d 0a20 2020 2072 6573 616d 706c 654d  ,..    resampleM
-000211b0: 6574 686f 6420 3d20 6c61 6e64 7361 7452  ethod = landsatR
-000211c0: 6573 616d 706c 654d 6574 686f 642c 0d0a  esampleMethod,..
-000211d0: 2020 2020 2368 6172 6d6f 6e69 7a65 4f4c      #harmonizeOL
-000211e0: 4920 3d20 6861 726d 6f6e 697a 654f 4c49  I = harmonizeOLI
-000211f0: 2c0d 0a20 2020 2070 7265 436f 6d70 7574  ,..    preComput
-00021200: 6564 436c 6f75 6453 636f 7265 4f66 6673  edCloudScoreOffs
-00021210: 6574 203d 2070 7265 436f 6d70 7574 6564  et = preComputed
-00021220: 4c61 6e64 7361 7443 6c6f 7564 5363 6f72  LandsatCloudScor
-00021230: 654f 6666 7365 742c 0d0a 2020 2020 7072  eOffset,..    pr
-00021240: 6543 6f6d 7075 7465 6454 444f 4d49 524d  eComputedTDOMIRM
-00021250: 6561 6e20 3d20 7072 6543 6f6d 7075 7465  ean = preCompute
-00021260: 644c 616e 6473 6174 5444 4f4d 4952 4d65  dLandsatTDOMIRMe
-00021270: 616e 2c0d 0a20 2020 2070 7265 436f 6d70  an,..    preComp
-00021280: 7574 6564 5444 4f4d 4952 5374 6444 6576  utedTDOMIRStdDev
-00021290: 203d 2070 7265 436f 6d70 7574 6564 5365   = preComputedSe
-000212a0: 6e74 696e 656c 3254 444f 4d49 5253 7464  ntinel2TDOMIRStd
-000212b0: 4465 762c 0d0a 2020 2020 6c61 6e64 7361  Dev,..    landsa
-000212c0: 7443 6f6c 6c65 6374 696f 6e56 6572 7369  tCollectionVersi
-000212d0: 6f6e 203d 206c 616e 6473 6174 436f 6c6c  on = landsatColl
-000212e0: 6563 7469 6f6e 5665 7273 696f 6e29 0d0a  ectionVersion)..
-000212f0: 0d0a 2020 2347 6574 2053 656e 7469 6e65  ..  #Get Sentine
-00021300: 6c20 320d 0a20 2073 3273 203d 2067 6574  l 2..  s2s = get
-00021310: 5072 6f63 6573 7365 6453 656e 7469 6e65  ProcessedSentine
-00021320: 6c32 5363 656e 6573 285c 0d0a 2020 2020  l2Scenes(\..    
-00021330: 7374 7564 7941 7265 6120 3d20 7374 7564  studyArea = stud
-00021340: 7941 7265 612c 0d0a 2020 2020 7374 6172  yArea,..    star
-00021350: 7459 6561 7220 3d20 7374 6172 7459 6561  tYear = startYea
-00021360: 722c 0d0a 2020 2020 656e 6459 6561 7220  r,..    endYear 
-00021370: 3d20 656e 6459 6561 722c 0d0a 2020 2020  = endYear,..    
-00021380: 7374 6172 744a 756c 6961 6e20 3d20 7374  startJulian = st
-00021390: 6172 744a 756c 6961 6e2c 0d0a 2020 2020  artJulian,..    
-000213a0: 656e 644a 756c 6961 6e20 3d20 656e 644a  endJulian = endJ
-000213b0: 756c 6961 6e2c 0d0a 2020 2020 6170 706c  ulian,..    appl
-000213c0: 7951 4142 616e 6420 3d20 6170 706c 7951  yQABand = applyQ
-000213d0: 4142 616e 642c 0d0a 2020 2020 6170 706c  ABand,..    appl
-000213e0: 7943 6c6f 7564 5363 6f72 6520 3d20 6170  yCloudScore = ap
-000213f0: 706c 7943 6c6f 7564 5363 6f72 6553 656e  plyCloudScoreSen
-00021400: 7469 6e65 6c32 2c0d 0a20 2020 2061 7070  tinel2,..    app
-00021410: 6c79 5368 6164 6f77 5368 6966 7420 3d20  lyShadowShift = 
-00021420: 6170 706c 7953 6861 646f 7753 6869 6674  applyShadowShift
-00021430: 2c0d 0a20 2020 2061 7070 6c79 5444 4f4d  ,..    applyTDOM
-00021440: 203d 2061 7070 6c79 5444 4f4d 5365 6e74   = applyTDOMSent
-00021450: 696e 656c 322c 0d0a 2020 2020 636c 6f75  inel2,..    clou
-00021460: 6453 636f 7265 5468 7265 7368 203d 2063  dScoreThresh = c
-00021470: 6c6f 7564 5363 6f72 6554 6872 6573 682c  loudScoreThresh,
-00021480: 0d0a 2020 2020 7065 7266 6f72 6d43 6c6f  ..    performClo
-00021490: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
-000214a0: 7065 7266 6f72 6d43 6c6f 7564 5363 6f72  performCloudScor
-000214b0: 654f 6666 7365 742c 0d0a 2020 2020 636c  eOffset,..    cl
-000214c0: 6f75 6453 636f 7265 5063 746c 203d 2063  oudScorePctl = c
-000214d0: 6c6f 7564 5363 6f72 6550 6374 6c2c 0d0a  loudScorePctl,..
-000214e0: 2020 2020 636c 6f75 6448 6569 6768 7473      cloudHeights
-000214f0: 203d 2063 6c6f 7564 4865 6967 6874 732c   = cloudHeights,
-00021500: 0d0a 2020 2020 7a53 636f 7265 5468 7265  ..    zScoreThre
-00021510: 7368 203d 207a 5363 6f72 6554 6872 6573  sh = zScoreThres
-00021520: 682c 0d0a 2020 2020 7368 6164 6f77 5375  h,..    shadowSu
-00021530: 6d54 6872 6573 6820 3d20 7368 6164 6f77  mThresh = shadow
-00021540: 5375 6d54 6872 6573 682c 0d0a 2020 2020  SumThresh,..    
-00021550: 636f 6e74 7261 6374 5069 7865 6c73 203d  contractPixels =
-00021560: 2063 6f6e 7472 6163 7450 6978 656c 732c   contractPixels,
-00021570: 0d0a 2020 2020 6469 6c61 7465 5069 7865  ..    dilatePixe
-00021580: 6c73 203d 2064 696c 6174 6550 6978 656c  ls = dilatePixel
-00021590: 732c 0d0a 2020 2020 7368 6164 6f77 5375  s,..    shadowSu
-000215a0: 6d42 616e 6473 203d 2073 6861 646f 7753  mBands = shadowS
-000215b0: 756d 4261 6e64 732c 0d0a 2020 2020 7265  umBands,..    re
-000215c0: 7361 6d70 6c65 4d65 7468 6f64 203d 2073  sampleMethod = s
-000215d0: 656e 7469 6e65 6c32 5265 7361 6d70 6c65  entinel2Resample
-000215e0: 4d65 7468 6f64 2c0d 0a20 2020 2074 6f61  Method,..    toa
-000215f0: 4f72 5352 203d 2074 6f61 4f72 5352 2c0d  OrSR = toaOrSR,.
-00021600: 0a20 2020 2063 6f6e 7665 7274 546f 4461  .    convertToDa
-00021610: 696c 794d 6f73 6169 6373 203d 2063 6f6e  ilyMosaics = con
-00021620: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
-00021630: 6373 2c0d 0a20 2020 2061 7070 6c79 436c  cs,..    applyCl
-00021640: 6f75 6450 726f 6261 6269 6c69 7479 203d  oudProbability =
-00021650: 2061 7070 6c79 436c 6f75 6450 726f 6261   applyCloudProba
-00021660: 6269 6c69 7479 2c0d 0a20 2020 2070 7265  bility,..    pre
-00021670: 436f 6d70 7574 6564 436c 6f75 6453 636f  ComputedCloudSco
-00021680: 7265 4f66 6673 6574 203d 2070 7265 436f  reOffset = preCo
-00021690: 6d70 7574 6564 5365 6e74 696e 656c 3243  mputedSentinel2C
-000216a0: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
-000216b0: 0d0a 2020 2020 7072 6543 6f6d 7075 7465  ..    preCompute
-000216c0: 6454 444f 4d49 524d 6561 6e20 3d20 7072  dTDOMIRMean = pr
-000216d0: 6543 6f6d 7075 7465 6453 656e 7469 6e65  eComputedSentine
-000216e0: 6c32 5444 4f4d 4952 4d65 616e 2c0d 0a20  l2TDOMIRMean,.. 
-000216f0: 2020 2070 7265 436f 6d70 7574 6564 5444     preComputedTD
-00021700: 4f4d 4952 5374 6444 6576 203d 2070 7265  OMIRStdDev = pre
-00021710: 436f 6d70 7574 6564 5365 6e74 696e 656c  ComputedSentinel
-00021720: 3254 444f 4d49 5253 7464 4465 762c 0d0a  2TDOMIRStdDev,..
-00021730: 2020 2020 636c 6f75 6450 726f 6254 6872      cloudProbThr
-00021740: 6573 6820 3d20 636c 6f75 6450 726f 6254  esh = cloudProbT
-00021750: 6872 6573 6829 0d0a 0d0a 0d0a 2020 2353  hresh)......  #S
-00021760: 656c 6563 7420 6f66 6620 636f 6d6d 6f6e  elect off common
-00021770: 2062 616e 6473 2062 6574 7765 656e 204c   bands between L
-00021780: 616e 6473 6174 2061 6e64 2053 656e 7469  andsat and Senti
-00021790: 6e65 6c20 320d 0a20 2063 6f6d 6d6f 6e42  nel 2..  commonB
-000217a0: 616e 6473 203d 2020 5b27 626c 7565 272c  ands =  ['blue',
-000217b0: 2027 6772 6565 6e27 2c20 2772 6564 272c   'green', 'red',
-000217c0: 2027 6e69 7227 2c20 2773 7769 7231 272c   'nir', 'swir1',
-000217d0: 2027 7377 6972 3227 2c20 2773 656e 736f   'swir2', 'senso
-000217e0: 7227 5d0d 0a20 206c 7320 3d20 6c73 2e73  r']..  ls = ls.s
-000217f0: 656c 6563 7428 636f 6d6d 6f6e 4261 6e64  elect(commonBand
-00021800: 7329 0d0a 2020 7332 7320 3d20 7332 732e  s)..  s2s = s2s.
-00021810: 7365 6c65 6374 2863 6f6d 6d6f 6e42 616e  select(commonBan
-00021820: 6473 290d 0a20 2023 4669 6c6c 2069 6e20  ds)..  #Fill in 
-00021830: 616e 7920 656d 7074 7920 636f 6c6c 6563  any empty collec
-00021840: 7469 6f6e 730d 0a20 2023 4966 2074 6865  tions..  #If the
-00021850: 7927 7265 2062 6f74 6820 656d 7074 792c  y're both empty,
-00021860: 2074 6869 7320 7769 6c6c 206e 6f74 2077   this will not w
-00021870: 6f72 6b0d 0a20 2064 756d 6d79 496d 6167  ork..  dummyImag
-00021880: 6520 3d65 652e 496d 6167 6528 6565 2e49  e =ee.Image(ee.I
-00021890: 6d61 6765 436f 6c6c 6563 7469 6f6e 2865  mageCollection(e
-000218a0: 652e 416c 676f 7269 7468 6d73 2e49 6628  e.Algorithms.If(
-000218b0: 6c73 2e74 6f4c 6973 7428 3129 2e6c 656e  ls.toList(1).len
-000218c0: 6774 6828 292e 6774 2830 292c 6c73 2c73  gth().gt(0),ls,s
-000218d0: 3273 2929 2e66 6972 7374 2829 290d 0a20  2s)).first()).. 
-000218e0: 206c 7320 3d20 6669 6c6c 456d 7074 7943   ls = fillEmptyC
-000218f0: 6f6c 6c65 6374 696f 6e73 286c 732c 6475  ollections(ls,du
-00021900: 6d6d 7949 6d61 6765 290d 0a20 2073 3273  mmyImage)..  s2s
-00021910: 203d 2066 696c 6c45 6d70 7479 436f 6c6c   = fillEmptyColl
-00021920: 6563 7469 6f6e 7328 7332 732c 6475 6d6d  ections(s2s,dumm
-00021930: 7949 6d61 6765 290d 0a0d 0a0d 0a20 2069  yImage)......  i
-00021940: 6620 7275 6e43 6861 7374 6169 6e48 6172  f runChastainHar
-00021950: 6d6f 6e69 7a61 7469 6f6e 2061 6e64 2074  monization and t
-00021960: 6f61 4f72 5352 203d 3d20 2754 4f41 273a  oaOrSR == 'TOA':
-00021970: 0d0a 0d0a 2020 2020 2320 5365 7061 7261  ....    # Separa
-00021980: 7465 2065 6163 6820 7365 6e73 6f72 0d0a  te each sensor..
-00021990: 0d0a 2020 2020 746d 203d 206c 732e 6669  ..    tm = ls.fi
-000219a0: 6c74 6572 2865 652e 4669 6c74 6572 2e69  lter(ee.Filter.i
-000219b0: 6e4c 6973 7428 2753 454e 534f 525f 4944  nList('SENSOR_ID
-000219c0: 272c 5b27 544d 272c 2745 544d 275d 2929  ',['TM','ETM']))
-000219d0: 0d0a 2020 2020 6f6c 6920 3d20 6c73 2e66  ..    oli = ls.f
-000219e0: 696c 7465 7228 6565 2e46 696c 7465 722e  ilter(ee.Filter.
-000219f0: 6571 2827 5345 4e53 4f52 5f49 4427 2c27  eq('SENSOR_ID','
-00021a00: 4f4c 495f 5449 5253 2729 290d 0a20 2020  OLI_TIRS'))..   
-00021a10: 2023 2065 6c73 653a 0d0a 2020 2020 2320   # else:..    # 
-00021a20: 2020 746d 203d 206c 732e 6669 6c74 6572    tm = ls.filter
-00021a30: 2865 652e 4669 6c74 6572 2e69 6e4c 6973  (ee.Filter.inLis
-00021a40: 7428 2773 656e 736f 7227 2c5b 274c 414e  t('sensor',['LAN
-00021a50: 4453 4154 5f34 272c 274c 414e 4453 4154  DSAT_4','LANDSAT
-00021a60: 5f35 272c 274c 414e 4453 4154 5f37 275d  _5','LANDSAT_7']
-00021a70: 2929 0d0a 2020 2020 2320 2020 6f6c 6920  ))..    #   oli 
-00021a80: 3d20 6c73 2e66 696c 7465 7228 6565 2e46  = ls.filter(ee.F
-00021a90: 696c 7465 722e 6571 2827 7365 6e73 6f72  ilter.eq('sensor
-00021aa0: 272c 274c 414e 4453 4154 5f38 2729 290d  ','LANDSAT_8')).
-00021ab0: 0a20 2020 206d 7369 203d 2073 3273 0d0a  .    msi = s2s..
-00021ac0: 0d0a 2020 2020 2320 4669 6c6c 2069 6620  ..    # Fill if 
-00021ad0: 6e6f 2069 6d61 6765 7320 6578 6973 7420  no images exist 
-00021ae0: 666f 7220 7061 7274 6963 756c 6172 204c  for particular L
-00021af0: 616e 6473 6174 2073 656e 736f 720d 0a20  andsat sensor.. 
-00021b00: 2020 2023 2041 6c6c 6f77 2069 7420 746f     # Allow it to
-00021b10: 2066 6169 6c20 6f66 206e 6f20 696d 6167   fail of no imag
-00021b20: 6573 2065 7869 7374 2066 6f72 2053 656e  es exist for Sen
-00021b30: 7469 6e65 6c20 3220 7369 6e63 6520 7468  tinel 2 since th
-00021b40: 6520 706f 696e 740d 0a20 2020 2023 206f  e point..    # o
-00021b50: 6620 7468 6973 206d 6574 686f 6420 6973  f this method is
-00021b60: 2074 6f20 696e 636c 7564 6520 5332 0d0a   to include S2..
-00021b70: 2020 2020 746d 203d 2066 696c 6c45 6d70      tm = fillEmp
-00021b80: 7479 436f 6c6c 6563 7469 6f6e 7328 746d  tyCollections(tm
-00021b90: 2c20 6565 2e49 6d61 6765 286c 732e 6669  , ee.Image(ls.fi
-00021ba0: 7273 7428 2929 290d 0a20 2020 206f 6c69  rst()))..    oli
-00021bb0: 203d 2066 696c 6c45 6d70 7479 436f 6c6c   = fillEmptyColl
-00021bc0: 6563 7469 6f6e 7328 6f6c 692c 2065 652e  ections(oli, ee.
-00021bd0: 496d 6167 6528 6c73 2e66 6972 7374 2829  Image(ls.first()
-00021be0: 2929 0d0a 0d0a 2020 2020 7072 696e 7428  ))....    print(
-00021bf0: 2752 756e 6e69 6e67 2043 6861 7374 6169  'Running Chastai
-00021c00: 6e20 6574 2061 6c20 3230 3139 2068 6172  n et al 2019 har
-00021c10: 6d6f 6e69 7a61 7469 6f6e 2729 0d0a 0d0a  monization')....
-00021c20: 2020 2020 2341 7070 6c79 2063 6f72 7265      #Apply corre
-00021c30: 6374 696f 6e0d 0a20 2020 2023 4375 7272  ction..    #Curr
-00021c40: 656e 746c 7920 636f 6465 6420 746f 2067  ently coded to g
-00021c50: 6f20 746f 2045 544d 2b0d 0a0d 0a20 2020  o to ETM+....   
-00021c60: 2023 4e6f 206e 6565 6420 746f 2063 6f72   #No need to cor
-00021c70: 7265 6374 2045 544d 2074 6f20 4554 4d0d  rect ETM to ETM.
-00021c80: 0a20 2020 2023 2074 6d20 3d20 746d 2e6d  .    # tm = tm.m
-00021c90: 6170 2866 756e 6374 696f 6e28 696d 6729  ap(function(img)
-00021ca0: 7b72 6574 7572 6e20 6765 7449 6d61 6765  {return getImage
-00021cb0: 734c 6962 2e68 6172 6d6f 6e69 7a61 7469  sLib.harmonizati
-00021cc0: 6f6e 4368 6173 7461 696e 2869 6d67 2c20  onChastain(img, 
-00021cd0: 2745 544d 272c 2745 544d 2729 7d29 0d0a  'ETM','ETM')})..
-00021ce0: 2020 2020 2320 6574 6d20 3d20 6574 6d2e      # etm = etm.
-00021cf0: 6d61 7028 6675 6e63 7469 6f6e 2869 6d67  map(function(img
-00021d00: 297b 7265 7475 726e 2067 6574 496d 6167  ){return getImag
-00021d10: 6573 4c69 622e 6861 726d 6f6e 697a 6174  esLib.harmonizat
-00021d20: 696f 6e43 6861 7374 6169 6e28 696d 672c  ionChastain(img,
-00021d30: 2027 4554 4d27 2c27 4554 4d27 297d 290d   'ETM','ETM')}).
-00021d40: 0a0d 0a20 2020 2023 4861 726d 6f6e 697a  ...    #Harmoniz
-00021d50: 6520 7468 6520 6f74 6865 7220 7477 6f0d  e the other two.
-00021d60: 0a20 2020 206f 6c69 203d 206f 6c69 2e6d  .    oli = oli.m
-00021d70: 6170 286c 616d 6264 6120 696d 673a 2068  ap(lambda img: h
-00021d80: 6172 6d6f 6e69 7a61 7469 6f6e 4368 6173  armonizationChas
-00021d90: 7461 696e 2869 6d67 2c20 274f 4c49 272c  tain(img, 'OLI',
-00021da0: 2745 544d 2729 290d 0a20 2020 206d 7369  'ETM'))..    msi
-00021db0: 203d 206d 7369 2e6d 6170 286c 616d 6264   = msi.map(lambd
-00021dc0: 6120 696d 673a 2068 6172 6d6f 6e69 7a61  a img: harmoniza
-00021dd0: 7469 6f6e 4368 6173 7461 696e 2869 6d67  tionChastain(img
-00021de0: 2c20 274d 5349 272c 2745 544d 2729 290d  , 'MSI','ETM')).
-00021df0: 0a0d 0a20 2020 2073 3273 203d 206d 7369  ...    s2s = msi
-00021e00: 0d0a 0d0a 2020 2020 234d 6572 6765 204c  ....    #Merge L
-00021e10: 616e 6473 6174 2062 6163 6b20 746f 6765  andsat back toge
-00021e20: 7468 6572 0d0a 2020 2020 6c73 203d 2065  ther..    ls = e
-00021e30: 652e 496d 6167 6543 6f6c 6c65 6374 696f  e.ImageCollectio
-00021e40: 6e28 746d 2e6d 6572 6765 286f 6c69 2929  n(tm.merge(oli))
-00021e50: 0d0a 0d0a 0d0a 2020 2320 4d65 7267 6520  ......  # Merge 
-00021e60: 4c61 6e64 7361 7420 616e 6420 5332 0d0a  Landsat and S2..
-00021e70: 2020 6d65 7267 6564 203d 2065 652e 496d    merged = ee.Im
-00021e80: 6167 6543 6f6c 6c65 6374 696f 6e28 6c73  ageCollection(ls
-00021e90: 2e6d 6572 6765 2873 3273 2929 0d0a 2020  .merge(s2s))..  
-00021ea0: 6d65 7267 6564 203d 206d 6572 6765 642e  merged = merged.
-00021eb0: 6d61 7028 7369 6d70 6c65 4164 6449 6e64  map(simpleAddInd
-00021ec0: 6963 6573 295c 0d0a 2020 2020 2020 2020  ices)\..        
-00021ed0: 2020 2020 2e6d 6170 2867 6574 5461 7373      .map(getTass
-00021ee0: 656c 6564 4361 7029 5c0d 0a20 2020 2020  eledCap)\..     
-00021ef0: 2020 2020 2020 202e 6d61 7028 7369 6d70         .map(simp
-00021f00: 6c65 4164 6454 4341 6e67 6c65 7329 0d0a  leAddTCAngles)..
-00021f10: 0d0a 2020 6d65 7267 6564 203d 206d 6572  ..  merged = mer
-00021f20: 6765 642e 7365 7428 6172 6773 290d 0a0d  ged.set(args)...
-00021f30: 0a0d 0a20 2072 6574 7572 6e20 6d65 7267  ...  return merg
-00021f40: 6564 0d0a 2323 2323 2323 2323 2323 2323  ed..############
-00021f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021f70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021f80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021f90: 2323 2323 230d 0a23 4675 6e63 7469 6f6e  #####..#Function
-00021fa0: 2074 6f20 7265 6769 7374 6572 2061 6e20   to register an 
-00021fb0: 696d 6167 6543 6f6c 6c65 6374 696f 6e20  imageCollection 
-00021fc0: 746f 2069 6d61 6765 7320 7769 7468 696e  to images within
-00021fd0: 2069 740d 0a23 416c 7761 7973 2075 7365   it..#Always use
-00021fe0: 7320 7468 6520 6669 7273 7420 696d 6167  s the first imag
-00021ff0: 6520 6173 2074 6865 2072 6566 6572 656e  e as the referen
-00022000: 6365 2069 6d61 6765 0d0a 6465 6620 636f  ce image..def co
-00022010: 5265 6769 7374 6572 436f 6c6c 6563 7469  RegisterCollecti
-00022020: 6f6e 2869 6d61 6765 732c 7265 6665 7265  on(images,refere
-00022030: 6e63 6542 616e 6473 203d 205b 276e 6972  nceBands = ['nir
-00022040: 275d 293a 0d0a 2020 2020 7265 6665 7265  ']):..    refere
-00022050: 6e63 6549 6d61 6765 496e 6465 7820 3d20  nceImageIndex = 
-00022060: 300d 0a20 2020 2072 6566 6572 656e 6365  0..    reference
-00022070: 496d 6167 6520 3d20 6565 2e49 6d61 6765  Image = ee.Image
-00022080: 2869 6d61 6765 732e 746f 4c69 7374 2872  (images.toList(r
-00022090: 6566 6572 656e 6365 496d 6167 6549 6e64  eferenceImageInd
-000220a0: 6578 2b31 292e 6765 7428 7265 6665 7265  ex+1).get(refere
-000220b0: 6e63 6549 6d61 6765 496e 6465 7829 292e  nceImageIndex)).
-000220c0: 7365 6c65 6374 2872 6566 6572 656e 6365  select(reference
-000220d0: 4261 6e64 7329 0d0a 0d0a 2020 2020 6465  Bands)....    de
-000220e0: 6620 7265 6769 7374 6572 496d 6167 6528  f registerImage(
-000220f0: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
-00022100: 2023 4465 7465 726d 696e 6520 7468 6520   #Determine the 
-00022110: 6469 7370 6c61 6365 6d65 6e74 2062 7920  displacement by 
-00022120: 6d61 7463 6869 6e67 206f 6e6c 7920 7468  matching only th
-00022130: 6520 7265 6665 7265 6e63 6542 616e 6420  e referenceBand 
-00022140: 6261 6e64 732e 0d0a 2020 2020 2020 2020  bands...        
-00022150: 6469 7370 6c61 6365 6d65 6e74 5f70 6172  displacement_par
-00022160: 616d 7320 3d20 7b0d 0a20 2020 2020 2020  ams = {..       
-00022170: 2020 2020 2027 7265 6665 7265 6e63 6549       'referenceI
-00022180: 6d61 6765 273a 2072 6566 6572 656e 6365  mage': reference
-00022190: 496d 6167 652c 0d0a 2020 2020 2020 2020  Image,..        
-000221a0: 2020 2020 276d 6178 4f66 6673 6574 273a      'maxOffset':
-000221b0: 2032 302e 302c 0d0a 2020 2020 2020 2020   20.0,..        
-000221c0: 2020 2020 2770 726f 6a65 6374 696f 6e27      'projection'
-000221d0: 3a20 4e6f 6e65 2c0d 0a20 2020 2020 2020  : None,..       
-000221e0: 2020 2020 2027 7061 7463 6857 6964 7468       'patchWidth
-000221f0: 273a 2032 302e 302c 0d0a 2020 2020 2020  ': 20.0,..      
-00022200: 2020 2020 2020 2773 7469 6666 6e65 7373        'stiffness
-00022210: 273a 2035 0d0a 2020 2020 2020 2020 2020  ': 5..          
-00022220: 2020 7d0d 0a20 2020 2020 2020 2064 6973    }..        dis
-00022230: 706c 6163 656d 656e 7420 3d20 696d 6167  placement = imag
-00022240: 652e 7365 6c65 6374 2872 6566 6572 656e  e.select(referen
-00022250: 6365 4261 6e64 7329 2e64 6973 706c 6163  ceBands).displac
-00022260: 656d 656e 7428 2a2a 6469 7370 6c61 6365  ement(**displace
-00022270: 6d65 6e74 5f70 6172 616d 7329 0d0a 2020  ment_params)..  
-00022280: 2020 2020 2020 7265 7475 726e 2069 6d61        return ima
-00022290: 6765 2e64 6973 706c 6163 6528 6469 7370  ge.displace(disp
-000222a0: 6c61 6365 6d65 6e74 290d 0a0d 0a20 2020  lacement)....   
-000222b0: 206f 7574 203d 2065 652e 496d 6167 6543   out = ee.ImageC
-000222c0: 6f6c 6c65 6374 696f 6e28 6565 2e49 6d61  ollection(ee.Ima
-000222d0: 6765 436f 6c6c 6563 7469 6f6e 2869 6d61  geCollection(ima
-000222e0: 6765 732e 746f 4c69 7374 2831 3030 3030  ges.toList(10000
-000222f0: 2c31 2929 2e6d 6170 2872 6567 6973 7465  ,1)).map(registe
-00022300: 7249 6d61 6765 2929 2328 6565 2e49 6d61  rImage))#(ee.Ima
-00022310: 6765 2869 6d61 6765 732e 746f 4c69 7374  ge(images.toList
-00022320: 2831 3030 3030 2c30 292e 6765 7428 3129  (10000,0).get(1)
-00022330: 292c 7265 6665 7265 6e63 6549 6d61 6765  ),referenceImage
-00022340: 290d 0a20 2020 206f 7574 203d 2065 652e  )..    out = ee.
-00022350: 496d 6167 6543 6f6c 6c65 6374 696f 6e28  ImageCollection(
-00022360: 696d 6167 6573 2e6c 696d 6974 2831 292e  images.limit(1).
-00022370: 6d65 7267 6528 6f75 7429 290d 0a0d 0a20  merge(out)).... 
-00022380: 2020 2072 6574 7572 6e20 6f75 740d 0a23     return out..#
-00022390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000223a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000223b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000223c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000223d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000223e0: 0d0a 2346 756e 6374 696f 6e20 746f 2066  ..#Function to f
-000223f0: 696e 6420 6120 7375 6273 6574 206f 6620  ind a subset of 
-00022400: 6120 636f 6c6c 6563 7469 6f6e 0d0a 2346  a collection..#F
-00022410: 6f72 2065 6163 6820 6772 6f75 7020 2865  or each group (e
-00022420: 2e67 2e20 7469 6c65 206f 7220 6f72 6269  .g. tile or orbi
-00022430: 7420 6f72 2070 6174 6829 2c20 616c 6c20  t or path), all 
-00022440: 696d 6167 6573 2077 6974 6869 6e20 7468  images within th
-00022450: 6174 2067 726f 7570 2077 696c 6c20 6265  at group will be
-00022460: 2072 6567 6973 7465 7265 640d 0a23 4173   registered..#As
-00022470: 2073 696e 676c 6520 636f 6c6c 6563 7469   single collecti
-00022480: 6f6e 2069 7320 7265 7475 726e 6564 0d0a  on is returned..
-00022490: 6465 6620 636f 5265 6769 7374 6572 4772  def coRegisterGr
-000224a0: 6f75 7073 2869 6d67 732c 6669 656c 644e  oups(imgs,fieldN
-000224b0: 616d 6520 3d20 2753 454e 5349 4e47 5f4f  ame = 'SENSING_O
-000224c0: 5242 4954 5f4e 554d 4245 5227 2c66 6965  RBIT_NUMBER',fie
-000224d0: 6c64 4973 4e75 6d65 7269 6320 3d20 5472  ldIsNumeric = Tr
-000224e0: 7565 293a 0d0a 2020 2020 6772 6f75 7073  ue):..    groups
-000224f0: 203d 2065 652e 4469 6374 696f 6e61 7279   = ee.Dictionary
-00022500: 2869 6d67 732e 6167 6772 6567 6174 655f  (imgs.aggregate_
-00022510: 6869 7374 6f67 7261 6d28 6669 656c 644e  histogram(fieldN
-00022520: 616d 6529 292e 6b65 7973 2829 0d0a 2020  ame)).keys()..  
-00022530: 2020 6966 2066 6965 6c64 4973 4e75 6d65    if fieldIsNume
-00022540: 7269 633a 0d0a 2020 2020 2020 2020 6772  ric:..        gr
-00022550: 6f75 7073 203d 2067 726f 7570 732e 6d61  oups = groups.ma
-00022560: 7028 6c61 6d62 6461 206e 3a20 6565 2e4e  p(lambda n: ee.N
-00022570: 756d 6265 722e 7061 7273 6528 6e29 290d  umber.parse(n)).
-00022580: 0a0d 0a20 2020 206f 7574 203d 6565 2e49  ...    out =ee.I
-00022590: 6d61 6765 436f 6c6c 6563 7469 6f6e 2865  mageCollection(e
-000225a0: 652e 4665 6174 7572 6543 6f6c 6c65 6374  e.FeatureCollect
-000225b0: 696f 6e28 6772 6f75 7073 2e6d 6170 286c  ion(groups.map(l
-000225c0: 616d 6264 6120 6772 6f75 703a 636f 5265  ambda group:coRe
-000225d0: 6769 7374 6572 436f 6c6c 6563 7469 6f6e  gisterCollection
-000225e0: 2869 6d67 732e 6669 6c74 6572 2865 652e  (imgs.filter(ee.
-000225f0: 4669 6c74 6572 2e65 7128 6669 656c 644e  Filter.eq(fieldN
-00022600: 616d 652c 6772 6f75 7029 2929 2929 2e66  ame,group))))).f
-00022610: 6c61 7474 656e 2829 290d 0a0d 0a20 2020  latten())....   
-00022620: 2072 6574 7572 6e20 6f75 740d 0a23 2323   return out..###
-00022630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022670: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-00022680: 6465 6620 6765 744c 616e 6473 6174 416e  def getLandsatAn
-00022690: 6453 656e 7469 6e65 6c32 4879 6272 6964  dSentinel2Hybrid
-000226a0: 5772 6170 7065 7228 5c0d 0a20 2073 7475  Wrapper(\..  stu
-000226b0: 6479 4172 6561 2c0d 0a20 2073 7461 7274  dyArea,..  start
-000226c0: 5965 6172 2c0d 0a20 2065 6e64 5965 6172  Year,..  endYear
-000226d0: 2c0d 0a20 2073 7461 7274 4a75 6c69 616e  ,..  startJulian
-000226e0: 2c0d 0a20 2065 6e64 4a75 6c69 616e 2c0d  ,..  endJulian,.
-000226f0: 0a20 2074 696d 6562 7566 6665 7220 3d20  .  timebuffer = 
-00022700: 2030 2c0d 0a20 2077 6569 6768 7473 203d   0,..  weights =
-00022710: 2020 5b31 5d2c 0d0a 2020 636f 6d70 6f73    [1],..  compos
-00022720: 6974 696e 674d 6574 686f 6420 3d20 276d  itingMethod = 'm
-00022730: 6564 6f69 6427 2c0d 0a20 2074 6f61 4f72  edoid',..  toaOr
-00022740: 5352 203d 2027 544f 4127 2c0d 0a20 2069  SR = 'TOA',..  i
-00022750: 6e63 6c75 6465 534c 434f 6666 4c37 203d  ncludeSLCOffL7 =
-00022760: 2046 616c 7365 2c0d 0a20 2064 6566 7269   False,..  defri
-00022770: 6e67 654c 3520 3d20 4661 6c73 652c 0d0a  ngeL5 = False,..
-00022780: 2020 6170 706c 7951 4142 616e 6420 3d20    applyQABand = 
-00022790: 4661 6c73 652c 0d0a 2020 6170 706c 7943  False,..  applyC
-000227a0: 6c6f 7564 5072 6f62 6162 696c 6974 7920  loudProbability 
-000227b0: 3d20 5472 7565 2c0d 0a20 2061 7070 6c79  = True,..  apply
-000227c0: 5368 6164 6f77 5368 6966 7420 3d20 4661  ShadowShift = Fa
-000227d0: 6c73 652c 0d0a 2020 6170 706c 7943 6c6f  lse,..  applyClo
-000227e0: 7564 5363 6f72 654c 616e 6473 6174 203d  udScoreLandsat =
-000227f0: 2046 616c 7365 2c0d 0a20 2061 7070 6c79   False,..  apply
-00022800: 436c 6f75 6453 636f 7265 5365 6e74 696e  CloudScoreSentin
-00022810: 656c 3220 3d20 4661 6c73 652c 0d0a 2020  el2 = False,..  
-00022820: 6170 706c 7954 444f 4d4c 616e 6473 6174  applyTDOMLandsat
-00022830: 203d 2054 7275 652c 0d0a 2020 6170 706c   = True,..  appl
-00022840: 7954 444f 4d53 656e 7469 6e65 6c32 203d  yTDOMSentinel2 =
-00022850: 2054 7275 652c 0d0a 2020 6170 706c 7946   True,..  applyF
-00022860: 6d61 736b 436c 6f75 644d 6173 6b20 3d20  maskCloudMask = 
-00022870: 5472 7565 2c0d 0a20 2061 7070 6c79 466d  True,..  applyFm
-00022880: 6173 6b43 6c6f 7564 5368 6164 6f77 4d61  askCloudShadowMa
-00022890: 736b 203d 2054 7275 652c 0d0a 2020 6170  sk = True,..  ap
-000228a0: 706c 7946 6d61 736b 536e 6f77 4d61 736b  plyFmaskSnowMask
-000228b0: 203d 2046 616c 7365 2c0d 0a20 2063 6c6f   = False,..  clo
-000228c0: 7564 4865 6967 6874 7320 3d20 6565 2e4c  udHeights = ee.L
-000228d0: 6973 742e 7365 7175 656e 6365 2835 3030  ist.sequence(500
-000228e0: 2c31 3030 3030 2c35 3030 292c 0d0a 2020  ,10000,500),..  
-000228f0: 636c 6f75 6453 636f 7265 5468 7265 7368  cloudScoreThresh
-00022900: 203d 2032 302c 0d0a 2020 7065 7266 6f72   = 20,..  perfor
-00022910: 6d43 6c6f 7564 5363 6f72 654f 6666 7365  mCloudScoreOffse
-00022920: 7420 3d20 5472 7565 2c0d 0a20 2063 6c6f  t = True,..  clo
-00022930: 7564 5363 6f72 6550 6374 6c20 3d20 3130  udScorePctl = 10
-00022940: 2c0d 0a20 207a 5363 6f72 6554 6872 6573  ,..  zScoreThres
-00022950: 6820 3d20 2d31 2c0d 0a20 2073 6861 646f  h = -1,..  shado
-00022960: 7753 756d 5468 7265 7368 203d 2030 2e33  wSumThresh = 0.3
-00022970: 352c 0d0a 2020 636f 6e74 7261 6374 5069  5,..  contractPi
-00022980: 7865 6c73 203d 2031 2e35 2c0d 0a20 2064  xels = 1.5,..  d
-00022990: 696c 6174 6550 6978 656c 7320 3d20 332e  ilatePixels = 3.
-000229a0: 352c 0d0a 2020 7368 6164 6f77 5375 6d42  5,..  shadowSumB
-000229b0: 616e 6473 203d 205b 276e 6972 272c 2773  ands = ['nir','s
-000229c0: 7769 7231 275d 2c0d 0a20 206c 616e 6473  wir1'],..  lands
-000229d0: 6174 5265 7361 6d70 6c65 4d65 7468 6f64  atResampleMethod
-000229e0: 203d 2027 6e65 6172 272c 0d0a 2020 7365   = 'near',..  se
-000229f0: 6e74 696e 656c 3252 6573 616d 706c 654d  ntinel2ResampleM
-00022a00: 6574 686f 6420 3d20 2761 6767 7265 6761  ethod = 'aggrega
-00022a10: 7465 272c 0d0a 2020 636f 6e76 6572 7454  te',..  convertT
-00022a20: 6f44 6169 6c79 4d6f 7361 6963 7320 3d20  oDailyMosaics = 
-00022a30: 5472 7565 2c0d 0a20 2072 756e 4368 6173  True,..  runChas
-00022a40: 7461 696e 4861 726d 6f6e 697a 6174 696f  tainHarmonizatio
-00022a50: 6e20 3d20 5472 7565 2c0d 0a20 2063 6f72  n = True,..  cor
-00022a60: 7265 6374 496c 6c75 6d69 6e61 7469 6f6e  rectIllumination
-00022a70: 203d 2046 616c 7365 2c0d 0a20 2063 6f72   = False,..  cor
-00022a80: 7265 6374 5363 616c 6520 3d20 3235 302c  rectScale = 250,
-00022a90: 0d0a 2020 6578 706f 7274 436f 6d70 6f73  ..  exportCompos
-00022aa0: 6974 6573 203d 2046 616c 7365 2c0d 0a20  ites = False,.. 
-00022ab0: 206f 7574 7075 744e 616d 6520 3d20 274c   outputName = 'L
-00022ac0: 616e 6473 6174 2d53 656e 7469 6e65 6c32  andsat-Sentinel2
-00022ad0: 2d48 7962 7269 6427 2c0d 0a20 2065 7870  -Hybrid',..  exp
-00022ae0: 6f72 7450 6174 6852 6f6f 7420 3d20 4e6f  ortPathRoot = No
-00022af0: 6e65 2c0d 0a20 2063 7273 203d 2027 4550  ne,..  crs = 'EP
-00022b00: 5347 3a35 3037 3027 2c0d 0a20 2074 7261  SG:5070',..  tra
-00022b10: 6e73 666f 726d 203d 205b 3330 2c30 2c2d  nsform = [30,0,-
-00022b20: 3233 3631 3931 352e 302c 302c 2d33 302c  2361915.0,0,-30,
-00022b30: 3331 3737 3733 352e 305d 2c0d 0a20 2073  3177735.0],..  s
-00022b40: 6361 6c65 203d 204e 6f6e 652c 0d0a 2020  cale = None,..  
-00022b50: 7072 6543 6f6d 7075 7465 644c 616e 6473  preComputedLands
-00022b60: 6174 436c 6f75 6453 636f 7265 4f66 6673  atCloudScoreOffs
-00022b70: 6574 203d 204e 6f6e 652c 0d0a 2020 7072  et = None,..  pr
-00022b80: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
-00022b90: 5444 4f4d 4952 4d65 616e 203d 204e 6f6e  TDOMIRMean = Non
-00022ba0: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
-00022bb0: 644c 616e 6473 6174 5444 4f4d 4952 5374  dLandsatTDOMIRSt
-00022bc0: 6444 6576 203d 204e 6f6e 652c 0d0a 2020  dDev = None,..  
-00022bd0: 7072 6543 6f6d 7075 7465 6453 656e 7469  preComputedSenti
-00022be0: 6e65 6c32 436c 6f75 6453 636f 7265 4f66  nel2CloudScoreOf
-00022bf0: 6673 6574 203d 204e 6f6e 652c 0d0a 2020  fset = None,..  
-00022c00: 7072 6543 6f6d 7075 7465 6453 656e 7469  preComputedSenti
-00022c10: 6e65 6c32 5444 4f4d 4952 4d65 616e 203d  nel2TDOMIRMean =
-00022c20: 204e 6f6e 652c 0d0a 2020 7072 6543 6f6d   None,..  preCom
-00022c30: 7075 7465 6453 656e 7469 6e65 6c32 5444  putedSentinel2TD
-00022c40: 4f4d 4952 5374 6444 6576 203d 204e 6f6e  OMIRStdDev = Non
-00022c50: 652c 0d0a 2020 636c 6f75 6450 726f 6254  e,..  cloudProbT
-00022c60: 6872 6573 6820 3d20 3430 2c0d 0a20 206c  hresh = 40,..  l
-00022c70: 616e 6473 6174 436f 6c6c 6563 7469 6f6e  andsatCollection
-00022c80: 5665 7273 696f 6e20 3d20 2743 3227 293a  Version = 'C2'):
-00022c90: 0d0a 0d0a 2020 6f72 6967 696e 203d 2027  ....  origin = '
-00022ca0: 4c61 6e64 7361 742d 5365 6e74 696e 656c  Landsat-Sentinel
-00022cb0: 322d 4879 6272 6964 270d 0a20 2074 6f61  2-Hybrid'..  toa
-00022cc0: 4f72 5352 203d 2074 6f61 4f72 5352 2e75  OrSR = toaOrSR.u
-00022cd0: 7070 6572 2829 0d0a 0d0a 2020 6172 6773  pper()....  args
-00022ce0: 203d 2066 6f72 6d61 7441 7267 7328 6c6f   = formatArgs(lo
-00022cf0: 6361 6c73 2829 290d 0a20 2069 6620 2761  cals())..  if 'a
-00022d00: 7267 7327 2069 6e20 6172 6773 2e6b 6579  rgs' in args.key
-00022d10: 7328 293a 0d0a 2020 2020 6465 6c20 6172  s():..    del ar
-00022d20: 6773 5b27 6172 6773 275d 0d0a 0d0a 2020  gs['args']....  
-00022d30: 6d65 7267 6564 203d 2067 6574 5072 6f63  merged = getProc
-00022d40: 6573 7365 644c 616e 6473 6174 416e 6453  essedLandsatAndS
-00022d50: 656e 7469 6e65 6c32 5363 656e 6573 285c  entinel2Scenes(\
-00022d60: 0d0a 2020 2020 7374 7564 7941 7265 6120  ..    studyArea 
-00022d70: 3d20 7374 7564 7941 7265 612c 0d0a 2020  = studyArea,..  
-00022d80: 2020 7374 6172 7459 6561 7220 3d20 7374    startYear = st
-00022d90: 6172 7459 6561 722c 0d0a 2020 2020 656e  artYear,..    en
-00022da0: 6459 6561 7220 3d20 656e 6459 6561 722c  dYear = endYear,
-00022db0: 0d0a 2020 2020 7374 6172 744a 756c 6961  ..    startJulia
-00022dc0: 6e20 3d20 7374 6172 744a 756c 6961 6e2c  n = startJulian,
-00022dd0: 0d0a 2020 2020 656e 644a 756c 6961 6e20  ..    endJulian 
-00022de0: 3d20 656e 644a 756c 6961 6e2c 0d0a 2020  = endJulian,..  
-00022df0: 2020 746f 614f 7253 5220 3d20 746f 614f    toaOrSR = toaO
-00022e00: 7253 522c 0d0a 2020 2020 696e 636c 7564  rSR,..    includ
-00022e10: 6553 4c43 4f66 664c 3720 3d20 696e 636c  eSLCOffL7 = incl
-00022e20: 7564 6553 4c43 4f66 664c 372c 0d0a 2020  udeSLCOffL7,..  
-00022e30: 2020 6465 6672 696e 6765 4c35 203d 2064    defringeL5 = d
-00022e40: 6566 7269 6e67 654c 352c 0d0a 2020 2020  efringeL5,..    
-00022e50: 6170 706c 7951 4142 616e 6420 3d20 6170  applyQABand = ap
-00022e60: 706c 7951 4142 616e 642c 0d0a 2020 2020  plyQABand,..    
-00022e70: 6170 706c 7943 6c6f 7564 5072 6f62 6162  applyCloudProbab
-00022e80: 696c 6974 7920 3d20 6170 706c 7943 6c6f  ility = applyClo
-00022e90: 7564 5072 6f62 6162 696c 6974 792c 0d0a  udProbability,..
-00022ea0: 2020 2020 6170 706c 7953 6861 646f 7753      applyShadowS
-00022eb0: 6869 6674 203d 2061 7070 6c79 5368 6164  hift = applyShad
-00022ec0: 6f77 5368 6966 742c 0d0a 2020 2020 6170  owShift,..    ap
-00022ed0: 706c 7943 6c6f 7564 5363 6f72 654c 616e  plyCloudScoreLan
-00022ee0: 6473 6174 203d 2061 7070 6c79 436c 6f75  dsat = applyClou
-00022ef0: 6453 636f 7265 4c61 6e64 7361 742c 0d0a  dScoreLandsat,..
-00022f00: 2020 2020 6170 706c 7943 6c6f 7564 5363      applyCloudSc
-00022f10: 6f72 6553 656e 7469 6e65 6c32 203d 2061  oreSentinel2 = a
-00022f20: 7070 6c79 436c 6f75 6453 636f 7265 5365  pplyCloudScoreSe
-00022f30: 6e74 696e 656c 322c 0d0a 2020 2020 6170  ntinel2,..    ap
-00022f40: 706c 7954 444f 4d4c 616e 6473 6174 203d  plyTDOMLandsat =
-00022f50: 2061 7070 6c79 5444 4f4d 4c61 6e64 7361   applyTDOMLandsa
-00022f60: 742c 0d0a 2020 2020 6170 706c 7954 444f  t,..    applyTDO
-00022f70: 4d53 656e 7469 6e65 6c32 203d 2061 7070  MSentinel2 = app
-00022f80: 6c79 5444 4f4d 5365 6e74 696e 656c 322c  lyTDOMSentinel2,
-00022f90: 0d0a 2020 2020 6170 706c 7946 6d61 736b  ..    applyFmask
-00022fa0: 436c 6f75 644d 6173 6b20 3d20 6170 706c  CloudMask = appl
-00022fb0: 7946 6d61 736b 436c 6f75 644d 6173 6b2c  yFmaskCloudMask,
-00022fc0: 0d0a 2020 2020 6170 706c 7946 6d61 736b  ..    applyFmask
-00022fd0: 436c 6f75 6453 6861 646f 774d 6173 6b20  CloudShadowMask 
-00022fe0: 3d20 6170 706c 7946 6d61 736b 436c 6f75  = applyFmaskClou
-00022ff0: 6453 6861 646f 774d 6173 6b2c 0d0a 2020  dShadowMask,..  
-00023000: 2020 6170 706c 7946 6d61 736b 536e 6f77    applyFmaskSnow
-00023010: 4d61 736b 203d 2061 7070 6c79 466d 6173  Mask = applyFmas
-00023020: 6b53 6e6f 774d 6173 6b2c 0d0a 2020 2020  kSnowMask,..    
-00023030: 636c 6f75 6448 6569 6768 7473 203d 2063  cloudHeights = c
-00023040: 6c6f 7564 4865 6967 6874 732c 0d0a 2020  loudHeights,..  
-00023050: 2020 636c 6f75 6453 636f 7265 5468 7265    cloudScoreThre
-00023060: 7368 203d 2063 6c6f 7564 5363 6f72 6554  sh = cloudScoreT
-00023070: 6872 6573 682c 0d0a 2020 2020 7065 7266  hresh,..    perf
-00023080: 6f72 6d43 6c6f 7564 5363 6f72 654f 6666  ormCloudScoreOff
-00023090: 7365 7420 3d20 7065 7266 6f72 6d43 6c6f  set = performClo
-000230a0: 7564 5363 6f72 654f 6666 7365 742c 0d0a  udScoreOffset,..
-000230b0: 2020 2020 636c 6f75 6453 636f 7265 5063      cloudScorePc
-000230c0: 746c 203d 2063 6c6f 7564 5363 6f72 6550  tl = cloudScoreP
-000230d0: 6374 6c2c 0d0a 2020 2020 7a53 636f 7265  ctl,..    zScore
-000230e0: 5468 7265 7368 203d 207a 5363 6f72 6554  Thresh = zScoreT
-000230f0: 6872 6573 682c 0d0a 2020 2020 7368 6164  hresh,..    shad
-00023100: 6f77 5375 6d54 6872 6573 6820 3d20 7368  owSumThresh = sh
-00023110: 6164 6f77 5375 6d54 6872 6573 682c 0d0a  adowSumThresh,..
-00023120: 2020 2020 636f 6e74 7261 6374 5069 7865      contractPixe
-00023130: 6c73 203d 2063 6f6e 7472 6163 7450 6978  ls = contractPix
-00023140: 656c 732c 0d0a 2020 2020 6469 6c61 7465  els,..    dilate
-00023150: 5069 7865 6c73 203d 2064 696c 6174 6550  Pixels = dilateP
-00023160: 6978 656c 732c 0d0a 2020 2020 7368 6164  ixels,..    shad
-00023170: 6f77 5375 6d42 616e 6473 203d 2073 6861  owSumBands = sha
-00023180: 646f 7753 756d 4261 6e64 732c 0d0a 2020  dowSumBands,..  
-00023190: 2020 6c61 6e64 7361 7452 6573 616d 706c    landsatResampl
-000231a0: 654d 6574 686f 6420 3d20 6c61 6e64 7361  eMethod = landsa
-000231b0: 7452 6573 616d 706c 654d 6574 686f 642c  tResampleMethod,
-000231c0: 0d0a 2020 2020 7365 6e74 696e 656c 3252  ..    sentinel2R
-000231d0: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
-000231e0: 7365 6e74 696e 656c 3252 6573 616d 706c  sentinel2Resampl
-000231f0: 654d 6574 686f 642c 0d0a 2020 2020 636f  eMethod,..    co
-00023200: 6e76 6572 7454 6f44 6169 6c79 4d6f 7361  nvertToDailyMosa
-00023210: 6963 7320 3d20 636f 6e76 6572 7454 6f44  ics = convertToD
-00023220: 6169 6c79 4d6f 7361 6963 732c 0d0a 2020  ailyMosaics,..  
-00023230: 2020 7275 6e43 6861 7374 6169 6e48 6172    runChastainHar
-00023240: 6d6f 6e69 7a61 7469 6f6e 203d 2072 756e  monization = run
-00023250: 4368 6173 7461 696e 4861 726d 6f6e 697a  ChastainHarmoniz
-00023260: 6174 696f 6e2c 0d0a 2020 2020 636f 7272  ation,..    corr
-00023270: 6563 7449 6c6c 756d 696e 6174 696f 6e20  ectIllumination 
-00023280: 3d20 636f 7272 6563 7449 6c6c 756d 696e  = correctIllumin
-00023290: 6174 696f 6e2c 0d0a 2020 2020 636f 7272  ation,..    corr
-000232a0: 6563 7453 6361 6c65 203d 2063 6f72 7265  ectScale = corre
-000232b0: 6374 5363 616c 652c 0d0a 2020 2020 7072  ctScale,..    pr
-000232c0: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
-000232d0: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
-000232e0: 203d 2070 7265 436f 6d70 7574 6564 4c61   = preComputedLa
-000232f0: 6e64 7361 7443 6c6f 7564 5363 6f72 654f  ndsatCloudScoreO
-00023300: 6666 7365 742c 0d0a 2020 2020 7072 6543  ffset,..    preC
-00023310: 6f6d 7075 7465 644c 616e 6473 6174 5444  omputedLandsatTD
-00023320: 4f4d 4952 4d65 616e 203d 2070 7265 436f  OMIRMean = preCo
-00023330: 6d70 7574 6564 4c61 6e64 7361 7454 444f  mputedLandsatTDO
-00023340: 4d49 524d 6561 6e2c 0d0a 2020 2020 7072  MIRMean,..    pr
-00023350: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
-00023360: 5444 4f4d 4952 5374 6444 6576 203d 2070  TDOMIRStdDev = p
-00023370: 7265 436f 6d70 7574 6564 4c61 6e64 7361  reComputedLandsa
-00023380: 7454 444f 4d49 5253 7464 4465 762c 0d0a  tTDOMIRStdDev,..
-00023390: 2020 2020 7072 6543 6f6d 7075 7465 6453      preComputedS
-000233a0: 656e 7469 6e65 6c32 436c 6f75 6453 636f  entinel2CloudSco
-000233b0: 7265 4f66 6673 6574 203d 2070 7265 436f  reOffset = preCo
-000233c0: 6d70 7574 6564 5365 6e74 696e 656c 3243  mputedSentinel2C
-000233d0: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
-000233e0: 0d0a 2020 2020 7072 6543 6f6d 7075 7465  ..    preCompute
-000233f0: 6453 656e 7469 6e65 6c32 5444 4f4d 4952  dSentinel2TDOMIR
-00023400: 4d65 616e 203d 2070 7265 436f 6d70 7574  Mean = preComput
-00023410: 6564 5365 6e74 696e 656c 3254 444f 4d49  edSentinel2TDOMI
-00023420: 524d 6561 6e2c 0d0a 2020 2020 7072 6543  RMean,..    preC
-00023430: 6f6d 7075 7465 6453 656e 7469 6e65 6c32  omputedSentinel2
-00023440: 5444 4f4d 4952 5374 6444 6576 203d 2070  TDOMIRStdDev = p
-00023450: 7265 436f 6d70 7574 6564 5365 6e74 696e  reComputedSentin
-00023460: 656c 3254 444f 4d49 5253 7464 4465 762c  el2TDOMIRStdDev,
-00023470: 0d0a 2020 2020 636c 6f75 6450 726f 6254  ..    cloudProbT
-00023480: 6872 6573 6820 3d20 636c 6f75 6450 726f  hresh = cloudPro
-00023490: 6254 6872 6573 682c 0d0a 2020 2020 6c61  bThresh,..    la
-000234a0: 6e64 7361 7443 6f6c 6c65 6374 696f 6e56  ndsatCollectionV
-000234b0: 6572 7369 6f6e 203d 206c 616e 6473 6174  ersion = landsat
-000234c0: 436f 6c6c 6563 7469 6f6e 5665 7273 696f  CollectionVersio
-000234d0: 6e29 0d0a 0d0a 2020 2343 7265 6174 6520  n)....  #Create 
-000234e0: 6879 6272 6964 2063 6f6d 706f 7369 7465  hybrid composite
-000234f0: 730d 0a20 2063 6f6d 706f 7369 7465 7320  s..  composites 
-00023500: 3d20 636f 6d70 6f73 6974 6554 696d 6553  = compositeTimeS
-00023510: 6572 6965 7328 5c0d 0a20 2020 206c 7320  eries(\..    ls 
-00023520: 3d20 6d65 7267 6564 2c0d 0a20 2020 2073  = merged,..    s
-00023530: 7461 7274 5965 6172 203d 2073 7461 7274  tartYear = start
-00023540: 5965 6172 2c0d 0a20 2020 2065 6e64 5965  Year,..    endYe
-00023550: 6172 203d 2065 6e64 5965 6172 2c0d 0a20  ar = endYear,.. 
-00023560: 2020 2073 7461 7274 4a75 6c69 616e 203d     startJulian =
-00023570: 2073 7461 7274 4a75 6c69 616e 2c0d 0a20   startJulian,.. 
-00023580: 2020 2065 6e64 4a75 6c69 616e 203d 2065     endJulian = e
-00023590: 6e64 4a75 6c69 616e 2c0d 0a20 2020 2074  ndJulian,..    t
-000235a0: 696d 6562 7566 6665 7220 3d20 7469 6d65  imebuffer = time
-000235b0: 6275 6666 6572 2c0d 0a20 2020 2077 6569  buffer,..    wei
-000235c0: 6768 7473 203d 2077 6569 6768 7473 2c0d  ghts = weights,.
-000235d0: 0a20 2020 2063 6f6d 706f 7369 7469 6e67  .    compositing
-000235e0: 4d65 7468 6f64 203d 2063 6f6d 706f 7369  Method = composi
-000235f0: 7469 6e67 4d65 7468 6f64 290d 0a0d 0a20  tingMethod).... 
-00023600: 2023 2045 7870 6f72 7420 636f 6d70 6f73   # Export compos
-00023610: 6974 6520 636f 6c6c 6563 7469 6f6e 0d0a  ite collection..
-00023620: 2020 6966 2065 7870 6f72 7443 6f6d 706f    if exportCompo
-00023630: 7369 7465 733a 0d0a 0d0a 2020 2020 6578  sites:....    ex
-00023640: 706f 7274 4261 6e64 4469 6374 203d 207b  portBandDict = {
-00023650: 5c0d 0a20 2020 2020 2027 6d65 646f 6964  \..      'medoid
-00023660: 273a 5b27 626c 7565 272c 2027 6772 6565  ':['blue', 'gree
-00023670: 6e27 2c20 2772 6564 272c 276e 6972 272c  n', 'red','nir',
-00023680: 2773 7769 7231 272c 2027 7377 6972 3227  'swir1', 'swir2'
-00023690: 2c27 636f 6d70 6f73 6974 654f 6273 436f  ,'compositeObsCo
-000236a0: 756e 7427 2c27 7365 6e73 6f72 272c 2779  unt','sensor','y
-000236b0: 6561 7227 2c27 6a75 6c69 616e 4461 7927  ear','julianDay'
-000236c0: 5d2c 0d0a 2020 2020 2020 276d 6564 6961  ],..      'media
-000236d0: 6e27 3a5b 2762 6c75 6527 2c20 2767 7265  n':['blue', 'gre
-000236e0: 656e 272c 2027 7265 6427 2c27 6e69 7227  en', 'red','nir'
-000236f0: 2c27 7377 6972 3127 2c20 2773 7769 7232  ,'swir1', 'swir2
-00023700: 272c 2763 6f6d 706f 7369 7465 4f62 7343  ','compositeObsC
-00023710: 6f75 6e74 275d 5c0d 0a20 2020 207d 3b0d  ount']\..    };.
-00023720: 0a20 2020 206e 6f6e 4469 7669 6465 4261  .    nonDivideBa
-00023730: 6e64 4469 6374 203d 207b 5c0d 0a20 2020  ndDict = {\..   
-00023740: 2020 2027 6d65 646f 6964 273a 5b27 636f     'medoid':['co
-00023750: 6d70 6f73 6974 654f 6273 436f 756e 7427  mpositeObsCount'
-00023760: 2c27 7365 6e73 6f72 272c 2779 6561 7227  ,'sensor','year'
-00023770: 2c27 6a75 6c69 616e 4461 7927 5d2c 0d0a  ,'julianDay'],..
-00023780: 2020 2020 2020 276d 6564 6961 6e27 3a5b        'median':[
-00023790: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
-000237a0: 6e74 275d 5c0d 0a20 2020 207d 3b0d 0a20  nt']\..    };.. 
-000237b0: 2020 2065 7870 6f72 7442 616e 6473 203d     exportBands =
-000237c0: 2065 7870 6f72 7442 616e 6444 6963 745b   exportBandDict[
-000237d0: 636f 6d70 6f73 6974 696e 674d 6574 686f  compositingMetho
-000237e0: 645d 0d0a 2020 2020 6e6f 6e44 6976 6964  d]..    nonDivid
-000237f0: 6542 616e 6473 203d 206e 6f6e 4469 7669  eBands = nonDivi
-00023800: 6465 4261 6e64 4469 6374 5b63 6f6d 706f  deBandDict[compo
-00023810: 7369 7469 6e67 4d65 7468 6f64 5d0d 0a0d  sitingMethod]...
-00023820: 0a20 2020 2065 7870 6f72 7443 6f6d 706f  .    exportCompo
-00023830: 7369 7465 436f 6c6c 6563 7469 6f6e 285c  siteCollection(\
-00023840: 0d0a 2020 2020 2020 636f 6c6c 6563 7469  ..      collecti
-00023850: 6f6e 203d 2063 6f6d 706f 7369 7465 732c  on = composites,
-00023860: 0d0a 2020 2020 2020 6578 706f 7274 5061  ..      exportPa
-00023870: 7468 526f 6f74 203d 2065 7870 6f72 7450  thRoot = exportP
-00023880: 6174 6852 6f6f 742c 0d0a 2020 2020 2020  athRoot,..      
-00023890: 6f75 7470 7574 4e61 6d65 203d 206f 7574  outputName = out
-000238a0: 7075 744e 616d 652c 0d0a 2020 2020 2020  putName,..      
-000238b0: 6f72 6967 696e 203d 206f 7269 6769 6e2c  origin = origin,
-000238c0: 0d0a 2020 2020 2020 7374 7564 7941 7265  ..      studyAre
-000238d0: 6120 3d20 7374 7564 7941 7265 612c 0d0a  a = studyArea,..
-000238e0: 2020 2020 2020 6372 7320 3d20 6372 732c        crs = crs,
-000238f0: 0d0a 2020 2020 2020 7472 616e 7366 6f72  ..      transfor
-00023900: 6d20 3d20 7472 616e 7366 6f72 6d2c 0d0a  m = transform,..
-00023910: 2020 2020 2020 7363 616c 6520 3d20 7363        scale = sc
-00023920: 616c 652c 0d0a 2020 2020 2020 7374 6172  ale,..      star
-00023930: 7459 6561 7220 3d20 7374 6172 7459 6561  tYear = startYea
-00023940: 722c 0d0a 2020 2020 2020 656e 6459 6561  r,..      endYea
-00023950: 7220 3d20 656e 6459 6561 722c 0d0a 2020  r = endYear,..  
-00023960: 2020 2020 7374 6172 744a 756c 6961 6e20      startJulian 
-00023970: 3d20 7374 6172 744a 756c 6961 6e2c 0d0a  = startJulian,..
-00023980: 2020 2020 2020 656e 644a 756c 6961 6e20        endJulian 
-00023990: 3d20 656e 644a 756c 6961 6e2c 0d0a 2020  = endJulian,..  
-000239a0: 2020 2020 636f 6d70 6f73 6974 696e 674d      compositingM
-000239b0: 6574 686f 6420 3d20 636f 6d70 6f73 6974  ethod = composit
-000239c0: 696e 674d 6574 686f 642c 0d0a 2020 2020  ingMethod,..    
-000239d0: 2020 7469 6d65 6275 6666 6572 203d 2074    timebuffer = t
-000239e0: 696d 6562 7566 6665 722c 0d0a 2020 2020  imebuffer,..    
-000239f0: 2020 746f 614f 7253 5220 3d20 746f 614f    toaOrSR = toaO
-00023a00: 7253 522c 0d0a 2020 2020 2020 6e6f 6e44  rSR,..      nonD
-00023a10: 6976 6964 6542 616e 6473 203d 206e 6f6e  ivideBands = non
-00023a20: 4469 7669 6465 4261 6e64 732c 0d0a 2020  DivideBands,..  
-00023a30: 2020 2020 6578 706f 7274 4261 6e64 7320      exportBands 
-00023a40: 3d20 6578 706f 7274 4261 6e64 732c 0d0a  = exportBands,..
-00023a50: 2020 2020 2020 6164 6469 7469 6f6e 616c        additional
-00023a60: 5072 6f70 6572 7479 4469 6374 203d 2061  PropertyDict = a
-00023a70: 7267 7329 0d0a 0d0a 2020 6172 6773 5b27  rgs)....  args['
-00023a80: 7072 6f63 6573 7365 6453 6365 6e65 7327  processedScenes'
-00023a90: 5d20 3d20 6d65 7267 6564 0d0a 2020 6172  ] = merged..  ar
-00023aa0: 6773 5b27 7072 6f63 6573 7365 6443 6f6d  gs['processedCom
-00023ab0: 706f 7369 7465 7327 5d20 3d20 636f 6d70  posites'] = comp
-00023ac0: 6f73 6974 6573 0d0a 0d0a 2020 7265 7475  osites....  retu
-00023ad0: 726e 2061 7267 730d 0a0d 0a23 2323 2323  rn args....#####
-00023ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023b20: 2323 2323 0d0a 2323 2323 2323 2323 2323  ####..##########
-00023b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023b50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023b60: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-00023b70: 0a23 4861 726d 6f6e 6963 2072 6567 7265  .#Harmonic regre
-00023b80: 7373 696f 6e0d 0a23 2323 2323 2323 2323  ssion..#########
+0001f1d0: 2323 2323 2323 0d0a 2323 2323 2323 2323  ######..########
+0001f1e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f1f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f220: 230d 0a23 2057 7261 7070 6572 2066 756e  #..# Wrapper fun
+0001f230: 6374 696f 6e20 666f 7220 6765 7474 696e  ction for gettin
+0001f240: 6720 5365 6e74 696e 656c 2032 2069 6d61  g Sentinel 2 ima
+0001f250: 6765 7279 0d0a 6465 6620 6765 7453 656e  gery..def getSen
+0001f260: 7469 6e65 6c32 5772 6170 7065 7228 5c0d  tinel2Wrapper(\.
+0001f270: 0a20 2073 7475 6479 4172 6561 2c0d 0a20  .  studyArea,.. 
+0001f280: 2073 7461 7274 5965 6172 2c0d 0a20 2065   startYear,..  e
+0001f290: 6e64 5965 6172 2c0d 0a20 2073 7461 7274  ndYear,..  start
+0001f2a0: 4a75 6c69 616e 2c0d 0a20 2065 6e64 4a75  Julian,..  endJu
+0001f2b0: 6c69 616e 2c0d 0a20 2074 696d 6562 7566  lian,..  timebuf
+0001f2c0: 6665 7220 3d20 302c 0d0a 2020 7765 6967  fer = 0,..  weig
+0001f2d0: 6874 7320 3d20 5b31 5d2c 0d0a 2020 636f  hts = [1],..  co
+0001f2e0: 6d70 6f73 6974 696e 674d 6574 686f 6420  mpositingMethod 
+0001f2f0: 3d20 276d 6564 6f69 6427 2c0d 0a20 2061  = 'medoid',..  a
+0001f300: 7070 6c79 5141 4261 6e64 203d 2046 616c  pplyQABand = Fal
+0001f310: 7365 2c0d 0a20 2061 7070 6c79 436c 6f75  se,..  applyClou
+0001f320: 6453 636f 7265 203d 2046 616c 7365 2c0d  dScore = False,.
+0001f330: 0a20 2061 7070 6c79 5368 6164 6f77 5368  .  applyShadowSh
+0001f340: 6966 7420 3d20 4661 6c73 652c 0d0a 2020  ift = False,..  
+0001f350: 6170 706c 7954 444f 4d20 3d20 5472 7565  applyTDOM = True
+0001f360: 2c0d 0a20 2063 6c6f 7564 5363 6f72 6554  ,..  cloudScoreT
+0001f370: 6872 6573 6820 3d20 3230 2c0d 0a20 2070  hresh = 20,..  p
+0001f380: 6572 666f 726d 436c 6f75 6453 636f 7265  erformCloudScore
+0001f390: 4f66 6673 6574 203d 2054 7275 652c 0d0a  Offset = True,..
+0001f3a0: 2020 636c 6f75 6453 636f 7265 5063 746c    cloudScorePctl
+0001f3b0: 203d 2031 302c 0d0a 2020 636c 6f75 6448   = 10,..  cloudH
+0001f3c0: 6569 6768 7473 203d 6565 2e4c 6973 742e  eights =ee.List.
+0001f3d0: 7365 7175 656e 6365 2835 3030 2c31 3030  sequence(500,100
+0001f3e0: 3030 2c35 3030 292c 0d0a 2020 7a53 636f  00,500),..  zSco
+0001f3f0: 7265 5468 7265 7368 203d 202d 312c 0d0a  reThresh = -1,..
+0001f400: 2020 7368 6164 6f77 5375 6d54 6872 6573    shadowSumThres
+0001f410: 6820 3d20 302e 3335 2c0d 0a20 2063 6f6e  h = 0.35,..  con
+0001f420: 7472 6163 7450 6978 656c 7320 3d20 312e  tractPixels = 1.
+0001f430: 352c 0d0a 2020 6469 6c61 7465 5069 7865  5,..  dilatePixe
+0001f440: 6c73 203d 2033 2e35 2c0d 0a20 2073 6861  ls = 3.5,..  sha
+0001f450: 646f 7753 756d 4261 6e64 7320 3d20 5b27  dowSumBands = ['
+0001f460: 6e69 7227 2c27 7377 6972 3127 5d2c 0d0a  nir','swir1'],..
+0001f470: 2020 636f 7272 6563 7449 6c6c 756d 696e    correctIllumin
+0001f480: 6174 696f 6e20 3d20 4661 6c73 652c 0d0a  ation = False,..
+0001f490: 2020 636f 7272 6563 7453 6361 6c65 203d    correctScale =
+0001f4a0: 2032 3530 2c0d 0a20 2065 7870 6f72 7443   250,..  exportC
+0001f4b0: 6f6d 706f 7369 7465 7320 3d20 4661 6c73  omposites = Fals
+0001f4c0: 652c 0d0a 2020 6f75 7470 7574 4e61 6d65  e,..  outputName
+0001f4d0: 203d 2027 5365 6e74 696e 656c 322d 436f   = 'Sentinel2-Co
+0001f4e0: 6d70 6f73 6974 6527 2c0d 0a20 2065 7870  mposite',..  exp
+0001f4f0: 6f72 7450 6174 6852 6f6f 7420 3d20 2775  ortPathRoot = 'u
+0001f500: 7365 7273 2f69 616e 686f 7573 6d61 6e2f  sers/ianhousman/
+0001f510: 7465 7374 272c 0d0a 2020 6372 7320 3d20  test',..  crs = 
+0001f520: 2745 5053 473a 3530 3730 272c 0d0a 2020  'EPSG:5070',..  
+0001f530: 7472 616e 7366 6f72 6d20 3d20 5b31 302c  transform = [10,
+0001f540: 302c 2d32 3336 3139 3135 2e30 2c30 2c2d  0,-2361915.0,0,-
+0001f550: 3130 2c33 3137 3737 3335 2e30 5d2c 0d0a  10,3177735.0],..
+0001f560: 2020 7363 616c 6520 3d20 4e6f 6e65 2c0d    scale = None,.
+0001f570: 0a20 2072 6573 616d 706c 654d 6574 686f  .  resampleMetho
+0001f580: 6420 3d20 2761 6767 7265 6761 7465 272c  d = 'aggregate',
+0001f590: 0d0a 2020 746f 614f 7253 5220 3d20 2754  ..  toaOrSR = 'T
+0001f5a0: 4f41 272c 0d0a 2020 636f 6e76 6572 7454  OA',..  convertT
+0001f5b0: 6f44 6169 6c79 4d6f 7361 6963 7320 3d20  oDailyMosaics = 
+0001f5c0: 5472 7565 2c0d 0a20 2061 7070 6c79 436c  True,..  applyCl
+0001f5d0: 6f75 6450 726f 6261 6269 6c69 7479 203d  oudProbability =
+0001f5e0: 2054 7275 652c 0d0a 2020 7072 6543 6f6d   True,..  preCom
+0001f5f0: 7075 7465 6443 6c6f 7564 5363 6f72 654f  putedCloudScoreO
+0001f600: 6666 7365 7420 3d20 4e6f 6e65 2c0d 0a20  ffset = None,.. 
+0001f610: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
+0001f620: 4952 4d65 616e 203d 204e 6f6e 652c 0d0a  IRMean = None,..
+0001f630: 2020 7072 6543 6f6d 7075 7465 6454 444f    preComputedTDO
+0001f640: 4d49 5253 7464 4465 7620 3d20 4e6f 6e65  MIRStdDev = None
+0001f650: 2c0d 0a20 2063 6c6f 7564 5072 6f62 5468  ,..  cloudProbTh
+0001f660: 7265 7368 203d 2034 302c 0d0a 2020 6f76  resh = 40,..  ov
+0001f670: 6572 7772 6974 6520 3d20 4661 6c73 6529  erwrite = False)
+0001f680: 3a0d 0a0d 0a20 206f 7269 6769 6e20 3d20  :....  origin = 
+0001f690: 2753 656e 7469 6e65 6c32 270d 0a20 2074  'Sentinel2'..  t
+0001f6a0: 6f61 4f72 5352 203d 2074 6f61 4f72 5352  oaOrSR = toaOrSR
+0001f6b0: 2e75 7070 6572 2829 0d0a 0d0a 2020 6172  .upper()....  ar
+0001f6c0: 6773 203d 2066 6f72 6d61 7441 7267 7328  gs = formatArgs(
+0001f6d0: 6c6f 6361 6c73 2829 290d 0a20 2069 6620  locals())..  if 
+0001f6e0: 2761 7267 7327 2069 6e20 6172 6773 2e6b  'args' in args.k
+0001f6f0: 6579 7328 293a 0d0a 2020 2020 6465 6c20  eys():..    del 
+0001f700: 6172 6773 5b27 6172 6773 275d 0d0a 0d0a  args['args']....
+0001f710: 2020 7332 7320 3d20 6765 7450 726f 6365    s2s = getProce
+0001f720: 7373 6564 5365 6e74 696e 656c 3253 6365  ssedSentinel2Sce
+0001f730: 6e65 7328 5c0d 0a20 2020 2073 7475 6479  nes(\..    study
+0001f740: 4172 6561 203d 2073 7475 6479 4172 6561  Area = studyArea
+0001f750: 2c0d 0a20 2020 2073 7461 7274 5965 6172  ,..    startYear
+0001f760: 203d 2073 7461 7274 5965 6172 2c0d 0a20   = startYear,.. 
+0001f770: 2020 2065 6e64 5965 6172 203d 2065 6e64     endYear = end
+0001f780: 5965 6172 2c0d 0a20 2020 2073 7461 7274  Year,..    start
+0001f790: 4a75 6c69 616e 203d 2073 7461 7274 4a75  Julian = startJu
+0001f7a0: 6c69 616e 2c0d 0a20 2020 2065 6e64 4a75  lian,..    endJu
+0001f7b0: 6c69 616e 203d 2065 6e64 4a75 6c69 616e  lian = endJulian
+0001f7c0: 2c0d 0a20 2020 2061 7070 6c79 5141 4261  ,..    applyQABa
+0001f7d0: 6e64 203d 2061 7070 6c79 5141 4261 6e64  nd = applyQABand
+0001f7e0: 2c0d 0a20 2020 2061 7070 6c79 436c 6f75  ,..    applyClou
+0001f7f0: 6453 636f 7265 203d 2061 7070 6c79 436c  dScore = applyCl
+0001f800: 6f75 6453 636f 7265 2c0d 0a20 2020 2061  oudScore,..    a
+0001f810: 7070 6c79 5368 6164 6f77 5368 6966 7420  pplyShadowShift 
+0001f820: 3d20 6170 706c 7953 6861 646f 7753 6869  = applyShadowShi
+0001f830: 6674 2c0d 0a20 2020 2061 7070 6c79 5444  ft,..    applyTD
+0001f840: 4f4d 203d 2061 7070 6c79 5444 4f4d 2c0d  OM = applyTDOM,.
+0001f850: 0a20 2020 2063 6c6f 7564 5363 6f72 6554  .    cloudScoreT
+0001f860: 6872 6573 6820 3d20 636c 6f75 6453 636f  hresh = cloudSco
+0001f870: 7265 5468 7265 7368 2c0d 0a20 2020 2070  reThresh,..    p
+0001f880: 6572 666f 726d 436c 6f75 6453 636f 7265  erformCloudScore
+0001f890: 4f66 6673 6574 203d 2070 6572 666f 726d  Offset = perform
+0001f8a0: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
+0001f8b0: 2c0d 0a20 2020 2063 6c6f 7564 5363 6f72  ,..    cloudScor
+0001f8c0: 6550 6374 6c20 3d20 636c 6f75 6453 636f  ePctl = cloudSco
+0001f8d0: 7265 5063 746c 2c0d 0a20 2020 2063 6c6f  rePctl,..    clo
+0001f8e0: 7564 4865 6967 6874 7320 3d20 636c 6f75  udHeights = clou
+0001f8f0: 6448 6569 6768 7473 2c0d 0a20 2020 207a  dHeights,..    z
+0001f900: 5363 6f72 6554 6872 6573 6820 3d20 7a53  ScoreThresh = zS
+0001f910: 636f 7265 5468 7265 7368 2c0d 0a20 2020  coreThresh,..   
+0001f920: 2073 6861 646f 7753 756d 5468 7265 7368   shadowSumThresh
+0001f930: 203d 2073 6861 646f 7753 756d 5468 7265   = shadowSumThre
+0001f940: 7368 2c0d 0a20 2020 2063 6f6e 7472 6163  sh,..    contrac
+0001f950: 7450 6978 656c 7320 3d20 636f 6e74 7261  tPixels = contra
+0001f960: 6374 5069 7865 6c73 2c0d 0a20 2020 2064  ctPixels,..    d
+0001f970: 696c 6174 6550 6978 656c 7320 3d20 6469  ilatePixels = di
+0001f980: 6c61 7465 5069 7865 6c73 2c0d 0a20 2020  latePixels,..   
+0001f990: 2073 6861 646f 7753 756d 4261 6e64 7320   shadowSumBands 
+0001f9a0: 3d20 7368 6164 6f77 5375 6d42 616e 6473  = shadowSumBands
+0001f9b0: 2c0d 0a20 2020 2072 6573 616d 706c 654d  ,..    resampleM
+0001f9c0: 6574 686f 6420 3d20 7265 7361 6d70 6c65  ethod = resample
+0001f9d0: 4d65 7468 6f64 2c0d 0a20 2020 2074 6f61  Method,..    toa
+0001f9e0: 4f72 5352 203d 2074 6f61 4f72 5352 2c0d  OrSR = toaOrSR,.
+0001f9f0: 0a20 2020 2063 6f6e 7665 7274 546f 4461  .    convertToDa
+0001fa00: 696c 794d 6f73 6169 6373 203d 2063 6f6e  ilyMosaics = con
+0001fa10: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
+0001fa20: 6373 2c0d 0a20 2020 2061 7070 6c79 436c  cs,..    applyCl
+0001fa30: 6f75 6450 726f 6261 6269 6c69 7479 203d  oudProbability =
+0001fa40: 2061 7070 6c79 436c 6f75 6450 726f 6261   applyCloudProba
+0001fa50: 6269 6c69 7479 2c0d 0a20 2020 2070 7265  bility,..    pre
+0001fa60: 436f 6d70 7574 6564 436c 6f75 6453 636f  ComputedCloudSco
+0001fa70: 7265 4f66 6673 6574 203d 2070 7265 436f  reOffset = preCo
+0001fa80: 6d70 7574 6564 436c 6f75 6453 636f 7265  mputedCloudScore
+0001fa90: 4f66 6673 6574 2c0d 0a20 2020 2070 7265  Offset,..    pre
+0001faa0: 436f 6d70 7574 6564 5444 4f4d 4952 4d65  ComputedTDOMIRMe
+0001fab0: 616e 203d 2070 7265 436f 6d70 7574 6564  an = preComputed
+0001fac0: 5444 4f4d 4952 4d65 616e 2c0d 0a20 2020  TDOMIRMean,..   
+0001fad0: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
+0001fae0: 4952 5374 6444 6576 203d 2070 7265 436f  IRStdDev = preCo
+0001faf0: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
+0001fb00: 6576 2c0d 0a20 2020 2063 6c6f 7564 5072  ev,..    cloudPr
+0001fb10: 6f62 5468 7265 7368 203d 2063 6c6f 7564  obThresh = cloud
+0001fb20: 5072 6f62 5468 7265 7368 290d 0a0d 0a20  ProbThresh).... 
+0001fb30: 2023 4164 6420 7a65 6e69 7468 2061 6e64   #Add zenith and
+0001fb40: 2061 7a69 6d75 7468 0d0a 2020 2369 6620   azimuth..  #if 
+0001fb50: 636f 7272 6563 7449 6c6c 756d 696e 6174  correctIlluminat
+0001fb60: 696f 6e3a 0d0a 2020 2320 2073 3273 203d  ion:..  #  s2s =
+0001fb70: 2073 3273 2e6d 6170 2866 756e 6374 696f   s2s.map(functio
+0001fb80: 6e28 696d 6729 7b0d 0a20 2023 2020 2020  n(img){..  #    
+0001fb90: 7265 7475 726e 2061 6464 5a65 6e69 7468  return addZenith
+0001fba0: 417a 696d 7574 6828 696d 672c 2754 4f41  Azimuth(img,'TOA
+0001fbb0: 272c 7b27 544f 4127 3a27 4d45 414e 5f53  ',{'TOA':'MEAN_S
+0001fbc0: 4f4c 4152 5f5a 454e 4954 485f 414e 474c  OLAR_ZENITH_ANGL
+0001fbd0: 4527 7d2c 7b27 544f 4127 3a27 4d45 414e  E'},{'TOA':'MEAN
+0001fbe0: 5f53 4f4c 4152 5f41 5a49 4d55 5448 5f41  _SOLAR_AZIMUTH_A
+0001fbf0: 4e47 4c45 277d 293b 0d0a 2020 2320 207d  NGLE'});..  #  }
+0001fc00: 293b 0d0a 2020 237d 0d0a 0d0a 2020 2343  );..  #}....  #C
+0001fc10: 7265 6174 6520 636f 6d70 6f73 6974 6520  reate composite 
+0001fc20: 7469 6d65 2073 6572 6965 730d 0a20 2074  time series..  t
+0001fc30: 7320 3d20 636f 6d70 6f73 6974 6554 696d  s = compositeTim
+0001fc40: 6553 6572 6965 7328 5c0d 0a20 2020 206c  eSeries(\..    l
+0001fc50: 7320 3d20 7332 732c 0d0a 2020 2020 7374  s = s2s,..    st
+0001fc60: 6172 7459 6561 7220 3d20 7374 6172 7459  artYear = startY
+0001fc70: 6561 722c 0d0a 2020 2020 656e 6459 6561  ear,..    endYea
+0001fc80: 7220 3d20 656e 6459 6561 722c 0d0a 2020  r = endYear,..  
+0001fc90: 2020 7374 6172 744a 756c 6961 6e20 3d20    startJulian = 
+0001fca0: 7374 6172 744a 756c 6961 6e2c 0d0a 2020  startJulian,..  
+0001fcb0: 2020 656e 644a 756c 6961 6e20 3d20 656e    endJulian = en
+0001fcc0: 644a 756c 6961 6e2c 0d0a 2020 2020 7469  dJulian,..    ti
+0001fcd0: 6d65 6275 6666 6572 203d 2074 696d 6562  mebuffer = timeb
+0001fce0: 7566 6665 722c 0d0a 2020 2020 7765 6967  uffer,..    weig
+0001fcf0: 6874 7320 3d20 7765 6967 6874 732c 0d0a  hts = weights,..
+0001fd00: 2020 2020 636f 6d70 6f73 6974 696e 674d      compositingM
+0001fd10: 6574 686f 6420 3d20 636f 6d70 6f73 6974  ethod = composit
+0001fd20: 696e 674d 6574 686f 6429 0d0a 0d0a 2020  ingMethod)....  
+0001fd30: 2343 6f72 7265 6374 2069 6c6c 756d 696e  #Correct illumin
+0001fd40: 6174 696f 6e0d 0a20 2023 2069 6620 2863  ation..  # if (c
+0001fd50: 6f72 7265 6374 496c 6c75 6d69 6e61 7469  orrectIlluminati
+0001fd60: 6f6e 297b 0d0a 2020 2320 2020 6620 3d20  on){..  #   f = 
+0001fd70: 6565 2e49 6d61 6765 2874 732e 6669 7273  ee.Image(ts.firs
+0001fd80: 7428 2929 3b0d 0a20 2023 2020 204d 6170  t());..  #   Map
+0001fd90: 2e61 6464 4c61 7965 7228 662c 7669 7a50  .addLayer(f,vizP
+0001fda0: 6172 616d 7346 616c 7365 2c27 4669 7273  aramsFalse,'Firs
+0001fdb0: 742d 6e6f 6e2d 696c 6c75 6d69 6e61 7465  t-non-illuminate
+0001fdc0: 6427 2c66 616c 7365 293b 0d0a 0d0a 2020  d',false);....  
+0001fdd0: 2320 2020 7072 696e 7428 2743 6f72 7265  #   print('Corre
+0001fde0: 6374 696e 6720 696c 6c75 6d69 6e61 7469  cting illuminati
+0001fdf0: 6f6e 2729 3b0d 0a20 2023 2020 2074 7320  on');..  #   ts 
+0001fe00: 3d20 7473 2e6d 6170 2869 6c6c 756d 696e  = ts.map(illumin
+0001fe10: 6174 696f 6e43 6f6e 6469 7469 6f6e 290d  ationCondition).
+0001fe20: 0a20 2023 2020 2020 202e 6d61 7028 6675  .  #     .map(fu
+0001fe30: 6e63 7469 6f6e 2869 6d67 297b 0d0a 2020  nction(img){..  
+0001fe40: 2320 2020 2020 2020 7265 7475 726e 2069  #       return i
+0001fe50: 6c6c 756d 696e 6174 696f 6e43 6f72 7265  lluminationCorre
+0001fe60: 6374 696f 6e28 696d 672c 2063 6f72 7265  ction(img, corre
+0001fe70: 6374 5363 616c 652c 7374 7564 7941 7265  ctScale,studyAre
+0001fe80: 612c 5b20 2762 6c75 6527 2c20 2767 7265  a,[ 'blue', 'gre
+0001fe90: 656e 272c 2027 7265 6427 2c27 6e69 7227  en', 'red','nir'
+0001fea0: 2c27 7377 6972 3127 2c20 2773 7769 7232  ,'swir1', 'swir2
+0001feb0: 275d 293b 0d0a 2020 2320 2020 2020 7d29  ']);..  #     })
+0001fec0: 3b0d 0a20 2023 2020 2066 203d 2065 652e  ;..  #   f = ee.
+0001fed0: 496d 6167 6528 7473 2e66 6972 7374 2829  Image(ts.first()
+0001fee0: 293b 0d0a 2020 2320 2020 4d61 702e 6164  );..  #   Map.ad
+0001fef0: 644c 6179 6572 2866 2c76 697a 5061 7261  dLayer(f,vizPara
+0001ff00: 6d73 4661 6c73 652c 2746 6972 7374 2d69  msFalse,'First-i
+0001ff10: 6c6c 756d 696e 6174 6564 272c 6661 6c73  lluminated',fals
+0001ff20: 6529 3b0d 0a0d 0a20 2023 2045 7870 6f72  e);....  # Expor
+0001ff30: 7420 636f 6d70 6f73 6974 6573 0d0a 2020  t composites..  
+0001ff40: 6966 2065 7870 6f72 7443 6f6d 706f 7369  if exportComposi
+0001ff50: 7465 733a 0d0a 2020 2020 6578 706f 7274  tes:..    export
+0001ff60: 4261 6e64 4469 6374 203d 207b 5c0d 0a20  BandDict = {\.. 
+0001ff70: 2020 2020 2027 5352 5f6d 6564 6f69 6427       'SR_medoid'
+0001ff80: 3a5b 2763 6227 2c20 2762 6c75 6527 2c20  :['cb', 'blue', 
+0001ff90: 2767 7265 656e 272c 2027 7265 6427 2c20  'green', 'red', 
+0001ffa0: 2772 6531 272c 2772 6532 272c 2772 6533  're1','re2','re3
+0001ffb0: 272c 276e 6972 272c 2027 6e69 7232 272c  ','nir', 'nir2',
+0001ffc0: 2027 7761 7465 7256 6170 6f72 272c 2027   'waterVapor', '
+0001ffd0: 7377 6972 3127 2c20 2773 7769 7232 272c  swir1', 'swir2',
+0001ffe0: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
+0001fff0: 6e74 272c 2773 656e 736f 7227 2c27 7965  nt','sensor','ye
+00020000: 6172 272c 276a 756c 6961 6e44 6179 275d  ar','julianDay']
+00020010: 2c0d 0a20 2020 2020 2027 5352 5f6d 6564  ,..      'SR_med
+00020020: 6961 6e27 3a5b 2763 6227 2c20 2762 6c75  ian':['cb', 'blu
+00020030: 6527 2c20 2767 7265 656e 272c 2027 7265  e', 'green', 're
+00020040: 6427 2c20 2772 6531 272c 2772 6532 272c  d', 're1','re2',
+00020050: 2772 6533 272c 276e 6972 272c 2027 6e69  're3','nir', 'ni
+00020060: 7232 272c 2027 7761 7465 7256 6170 6f72  r2', 'waterVapor
+00020070: 272c 2027 7377 6972 3127 2c20 2773 7769  ', 'swir1', 'swi
+00020080: 7232 272c 2763 6f6d 706f 7369 7465 4f62  r2','compositeOb
+00020090: 7343 6f75 6e74 275d 2c0d 0a20 2020 2020  sCount'],..     
+000200a0: 2027 544f 415f 6d65 646f 6964 273a 5b27   'TOA_medoid':['
+000200b0: 6362 272c 2027 626c 7565 272c 2027 6772  cb', 'blue', 'gr
+000200c0: 6565 6e27 2c20 2772 6564 272c 2027 7265  een', 'red', 're
+000200d0: 3127 2c27 7265 3227 2c27 7265 3327 2c27  1','re2','re3','
+000200e0: 6e69 7227 2c20 276e 6972 3227 2c20 2777  nir', 'nir2', 'w
+000200f0: 6174 6572 5661 706f 7227 2c20 2763 6972  aterVapor', 'cir
+00020100: 7275 7327 2c20 2773 7769 7231 272c 2027  rus', 'swir1', '
+00020110: 7377 6972 3227 2c27 636f 6d70 6f73 6974  swir2','composit
+00020120: 654f 6273 436f 756e 7427 2c27 7365 6e73  eObsCount','sens
+00020130: 6f72 272c 2779 6561 7227 2c27 6a75 6c69  or','year','juli
+00020140: 616e 4461 7927 5d2c 0d0a 2020 2020 2020  anDay'],..      
+00020150: 2754 4f41 5f6d 6564 6961 6e27 3a5b 2763  'TOA_median':['c
+00020160: 6227 2c20 2762 6c75 6527 2c20 2767 7265  b', 'blue', 'gre
+00020170: 656e 272c 2027 7265 6427 2c20 2772 6531  en', 'red', 're1
+00020180: 272c 2772 6532 272c 2772 6533 272c 276e  ','re2','re3','n
+00020190: 6972 272c 2027 6e69 7232 272c 2027 7761  ir', 'nir2', 'wa
+000201a0: 7465 7256 6170 6f72 272c 2027 6369 7272  terVapor', 'cirr
+000201b0: 7573 272c 2027 7377 6972 3127 2c20 2773  us', 'swir1', 's
+000201c0: 7769 7232 272c 2763 6f6d 706f 7369 7465  wir2','composite
+000201d0: 4f62 7343 6f75 6e74 275d 5c0d 0a20 2020  ObsCount']\..   
+000201e0: 207d 0d0a 2020 2020 6e6f 6e44 6976 6964   }..    nonDivid
+000201f0: 6542 616e 6444 6963 7420 3d20 7b5c 0d0a  eBandDict = {\..
+00020200: 2020 2020 2020 276d 6564 6f69 6427 3a5b        'medoid':[
+00020210: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
+00020220: 6e74 272c 2773 656e 736f 7227 2c27 7965  nt','sensor','ye
+00020230: 6172 272c 276a 756c 6961 6e44 6179 275d  ar','julianDay']
+00020240: 2c0d 0a20 2020 2020 2027 6d65 6469 616e  ,..      'median
+00020250: 273a 5b27 636f 6d70 6f73 6974 654f 6273  ':['compositeObs
+00020260: 436f 756e 7427 5d5c 0d0a 2020 2020 7d0d  Count']\..    }.
+00020270: 0a20 2020 2065 7870 6f72 7442 616e 6473  .    exportBands
+00020280: 203d 2065 7870 6f72 7442 616e 6444 6963   = exportBandDic
+00020290: 745b 746f 614f 7253 5220 2b20 275f 2720  t[toaOrSR + '_' 
+000202a0: 2b20 636f 6d70 6f73 6974 696e 674d 6574  + compositingMet
+000202b0: 686f 645d 0d0a 2020 2020 6e6f 6e44 6976  hod]..    nonDiv
+000202c0: 6964 6542 616e 6473 203d 206e 6f6e 4469  ideBands = nonDi
+000202d0: 7669 6465 4261 6e64 4469 6374 5b63 6f6d  videBandDict[com
+000202e0: 706f 7369 7469 6e67 4d65 7468 6f64 5d0d  positingMethod].
+000202f0: 0a0d 0a20 2020 2065 7870 6f72 7443 6f6d  ...    exportCom
+00020300: 706f 7369 7465 436f 6c6c 6563 7469 6f6e  positeCollection
+00020310: 285c 0d0a 2020 2020 2020 636f 6c6c 6563  (\..      collec
+00020320: 7469 6f6e 203d 2074 732c 0d0a 2020 2020  tion = ts,..    
+00020330: 2020 6578 706f 7274 5061 7468 526f 6f74    exportPathRoot
+00020340: 203d 2065 7870 6f72 7450 6174 6852 6f6f   = exportPathRoo
+00020350: 742c 0d0a 2020 2020 2020 6f75 7470 7574  t,..      output
+00020360: 4e61 6d65 203d 206f 7574 7075 744e 616d  Name = outputNam
+00020370: 652c 0d0a 2020 2020 2020 6f72 6967 696e  e,..      origin
+00020380: 203d 206f 7269 6769 6e2c 0d0a 2020 2020   = origin,..    
+00020390: 2020 7374 7564 7941 7265 6120 3d20 7374    studyArea = st
+000203a0: 7564 7941 7265 612c 0d0a 2020 2020 2020  udyArea,..      
+000203b0: 6372 7320 3d20 6372 732c 0d0a 2020 2020  crs = crs,..    
+000203c0: 2020 7472 616e 7366 6f72 6d20 3d20 7472    transform = tr
+000203d0: 616e 7366 6f72 6d2c 0d0a 2020 2020 2020  ansform,..      
+000203e0: 7363 616c 6520 3d20 7363 616c 652c 0d0a  scale = scale,..
+000203f0: 2020 2020 2020 7374 6172 7459 6561 7220        startYear 
+00020400: 3d20 7374 6172 7459 6561 722c 0d0a 2020  = startYear,..  
+00020410: 2020 2020 656e 6459 6561 7220 3d20 656e      endYear = en
+00020420: 6459 6561 722c 0d0a 2020 2020 2020 7374  dYear,..      st
+00020430: 6172 744a 756c 6961 6e20 3d20 7374 6172  artJulian = star
+00020440: 744a 756c 6961 6e2c 0d0a 2020 2020 2020  tJulian,..      
+00020450: 656e 644a 756c 6961 6e20 3d20 656e 644a  endJulian = endJ
+00020460: 756c 6961 6e2c 0d0a 2020 2020 2020 636f  ulian,..      co
+00020470: 6d70 6f73 6974 696e 674d 6574 686f 6420  mpositingMethod 
+00020480: 3d20 636f 6d70 6f73 6974 696e 674d 6574  = compositingMet
+00020490: 686f 642c 0d0a 2020 2020 2020 7469 6d65  hod,..      time
+000204a0: 6275 6666 6572 203d 2074 696d 6562 7566  buffer = timebuf
+000204b0: 6665 722c 0d0a 2020 2020 2020 746f 614f  fer,..      toaO
+000204c0: 7253 5220 3d20 746f 614f 7253 522c 0d0a  rSR = toaOrSR,..
+000204d0: 2020 2020 2020 6e6f 6e44 6976 6964 6542        nonDivideB
+000204e0: 616e 6473 203d 206e 6f6e 4469 7669 6465  ands = nonDivide
+000204f0: 4261 6e64 732c 0d0a 2020 2020 2020 6578  Bands,..      ex
+00020500: 706f 7274 4261 6e64 7320 3d20 6578 706f  portBands = expo
+00020510: 7274 4261 6e64 732c 0d0a 2020 2020 2020  rtBands,..      
+00020520: 6164 6469 7469 6f6e 616c 5072 6f70 6572  additionalProper
+00020530: 7479 4469 6374 203d 2061 7267 732c 0d0a  tyDict = args,..
+00020540: 2020 2020 2020 6f76 6572 7772 6974 6520        overwrite 
+00020550: 3d20 6f76 6572 7772 6974 6529 0d0a 0d0a  = overwrite)....
+00020560: 2020 6172 6773 5b27 7072 6f63 6573 7365    args['processe
+00020570: 6453 6365 6e65 7327 5d20 3d20 7332 730d  dScenes'] = s2s.
+00020580: 0a20 2061 7267 735b 2770 726f 6365 7373  .  args['process
+00020590: 6564 436f 6d70 6f73 6974 6573 275d 203d  edComposites'] =
+000205a0: 2074 730d 0a0d 0a20 2072 6574 7572 6e20   ts....  return 
+000205b0: 6172 6773 0d0a 0d0a 2320 4879 6272 6964  args....# Hybrid
+000205c0: 2067 6574 204c 616e 6473 6174 2061 6e64   get Landsat and
+000205d0: 2053 656e 7469 6e65 6c20 3220 7072 6f63   Sentinel 2 proc
+000205e0: 6573 7365 6420 7363 656e 6573 0d0a 2320  essed scenes..# 
+000205f0: 4861 6e64 6c65 7320 6765 7474 696e 6720  Handles getting 
+00020600: 7072 6f63 6573 7365 6420 7363 656e 6573  processed scenes
+00020610: 2020 7769 7468 204c 616e 6473 6174 2061    with Landsat a
+00020620: 6e64 2053 656e 7469 6e65 6c20 320d 0a64  nd Sentinel 2..d
+00020630: 6566 2067 6574 5072 6f63 6573 7365 644c  ef getProcessedL
+00020640: 616e 6473 6174 416e 6453 656e 7469 6e65  andsatAndSentine
+00020650: 6c32 5363 656e 6573 280d 0a20 2020 2020  l2Scenes(..     
+00020660: 2073 7475 6479 4172 6561 2c0d 0a20 2020   studyArea,..   
+00020670: 2020 2073 7461 7274 5965 6172 2c0d 0a20     startYear,.. 
+00020680: 2020 2020 2065 6e64 5965 6172 2c0d 0a20       endYear,.. 
+00020690: 2020 2020 2073 7461 7274 4a75 6c69 616e       startJulian
+000206a0: 2c0d 0a20 2020 2020 2065 6e64 4a75 6c69  ,..      endJuli
+000206b0: 616e 2c0d 0a20 2020 2020 2074 6f61 4f72  an,..      toaOr
+000206c0: 5352 203d 2027 544f 4127 2c0d 0a20 2020  SR = 'TOA',..   
+000206d0: 2020 2069 6e63 6c75 6465 534c 434f 6666     includeSLCOff
+000206e0: 4c37 203d 2046 616c 7365 2c0d 0a20 2020  L7 = False,..   
+000206f0: 2020 2064 6566 7269 6e67 654c 3520 3d20     defringeL5 = 
+00020700: 4661 6c73 652c 0d0a 2020 2020 2020 6170  False,..      ap
+00020710: 706c 7951 4142 616e 6420 3d20 4661 6c73  plyQABand = Fals
+00020720: 652c 0d0a 2020 2020 2020 6170 706c 7943  e,..      applyC
+00020730: 6c6f 7564 5072 6f62 6162 696c 6974 7920  loudProbability 
+00020740: 3d20 5472 7565 2c0d 0a20 2020 2020 2061  = True,..      a
+00020750: 7070 6c79 5368 6164 6f77 5368 6966 7420  pplyShadowShift 
+00020760: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00020770: 6170 706c 7943 6c6f 7564 5363 6f72 654c  applyCloudScoreL
+00020780: 616e 6473 6174 203d 2046 616c 7365 2c0d  andsat = False,.
+00020790: 0a20 2020 2020 2061 7070 6c79 436c 6f75  .      applyClou
+000207a0: 6453 636f 7265 5365 6e74 696e 656c 3220  dScoreSentinel2 
+000207b0: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+000207c0: 6170 706c 7954 444f 4d4c 616e 6473 6174  applyTDOMLandsat
+000207d0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
+000207e0: 6170 706c 7954 444f 4d53 656e 7469 6e65  applyTDOMSentine
+000207f0: 6c32 203d 2054 7275 652c 0d0a 2020 2020  l2 = True,..    
+00020800: 2020 6170 706c 7946 6d61 736b 436c 6f75    applyFmaskClou
+00020810: 644d 6173 6b20 3d20 5472 7565 2c0d 0a20  dMask = True,.. 
+00020820: 2020 2020 2061 7070 6c79 466d 6173 6b43       applyFmaskC
+00020830: 6c6f 7564 5368 6164 6f77 4d61 736b 203d  loudShadowMask =
+00020840: 2054 7275 652c 0d0a 2020 2020 2020 6170   True,..      ap
+00020850: 706c 7946 6d61 736b 536e 6f77 4d61 736b  plyFmaskSnowMask
+00020860: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+00020870: 2063 6c6f 7564 4865 6967 6874 7320 3d20   cloudHeights = 
+00020880: 6565 2e4c 6973 742e 7365 7175 656e 6365  ee.List.sequence
+00020890: 2835 3030 2c31 3030 3030 2c35 3030 292c  (500,10000,500),
+000208a0: 0d0a 2020 2020 2020 636c 6f75 6453 636f  ..      cloudSco
+000208b0: 7265 5468 7265 7368 203d 2032 302c 0d0a  reThresh = 20,..
+000208c0: 2020 2020 2020 7065 7266 6f72 6d43 6c6f        performClo
+000208d0: 7564 5363 6f72 654f 6666 7365 7420 3d20  udScoreOffset = 
+000208e0: 5472 7565 2c0d 0a20 2020 2020 2063 6c6f  True,..      clo
+000208f0: 7564 5363 6f72 6550 6374 6c20 3d20 3130  udScorePctl = 10
+00020900: 2c0d 0a20 2020 2020 207a 5363 6f72 6554  ,..      zScoreT
+00020910: 6872 6573 6820 3d20 2d31 2c0d 0a20 2020  hresh = -1,..   
+00020920: 2020 2073 6861 646f 7753 756d 5468 7265     shadowSumThre
+00020930: 7368 203d 2030 2e33 352c 0d0a 2020 2020  sh = 0.35,..    
+00020940: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
+00020950: 203d 2031 2e35 2c0d 0a20 2020 2020 2064   = 1.5,..      d
+00020960: 696c 6174 6550 6978 656c 7320 3d20 332e  ilatePixels = 3.
+00020970: 352c 0d0a 2020 2020 2020 7368 6164 6f77  5,..      shadow
+00020980: 5375 6d42 616e 6473 203d 205b 276e 6972  SumBands = ['nir
+00020990: 272c 2773 7769 7231 275d 2c0d 0a20 2020  ','swir1'],..   
+000209a0: 2020 206c 616e 6473 6174 5265 7361 6d70     landsatResamp
+000209b0: 6c65 4d65 7468 6f64 203d 2027 6e65 6172  leMethod = 'near
+000209c0: 272c 0d0a 2020 2020 2020 7365 6e74 696e  ',..      sentin
+000209d0: 656c 3252 6573 616d 706c 654d 6574 686f  el2ResampleMetho
+000209e0: 6420 3d20 2761 6767 7265 6761 7465 272c  d = 'aggregate',
+000209f0: 0d0a 2020 2020 2020 636f 6e76 6572 7454  ..      convertT
+00020a00: 6f44 6169 6c79 4d6f 7361 6963 7320 3d20  oDailyMosaics = 
+00020a10: 5472 7565 2c0d 0a20 2020 2020 2072 756e  True,..      run
+00020a20: 4368 6173 7461 696e 4861 726d 6f6e 697a  ChastainHarmoniz
+00020a30: 6174 696f 6e20 3d20 5472 7565 2c0d 0a20  ation = True,.. 
+00020a40: 2020 2020 2063 6f72 7265 6374 496c 6c75       correctIllu
+00020a50: 6d69 6e61 7469 6f6e 203d 2046 616c 7365  mination = False
+00020a60: 2c0d 0a20 2020 2020 2063 6f72 7265 6374  ,..      correct
+00020a70: 5363 616c 6520 3d20 3235 302c 0d0a 2020  Scale = 250,..  
+00020a80: 2020 2020 7072 6543 6f6d 7075 7465 644c      preComputedL
+00020a90: 616e 6473 6174 436c 6f75 6453 636f 7265  andsatCloudScore
+00020aa0: 4f66 6673 6574 203d 204e 6f6e 652c 0d0a  Offset = None,..
+00020ab0: 2020 2020 2020 7072 6543 6f6d 7075 7465        preCompute
+00020ac0: 644c 616e 6473 6174 5444 4f4d 4952 4d65  dLandsatTDOMIRMe
+00020ad0: 616e 203d 204e 6f6e 652c 0d0a 2020 2020  an = None,..    
+00020ae0: 2020 7072 6543 6f6d 7075 7465 644c 616e    preComputedLan
+00020af0: 6473 6174 5444 4f4d 4952 5374 6444 6576  dsatTDOMIRStdDev
+00020b00: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+00020b10: 7072 6543 6f6d 7075 7465 6453 656e 7469  preComputedSenti
+00020b20: 6e65 6c32 436c 6f75 6453 636f 7265 4f66  nel2CloudScoreOf
+00020b30: 6673 6574 203d 204e 6f6e 652c 0d0a 2020  fset = None,..  
+00020b40: 2020 2020 7072 6543 6f6d 7075 7465 6453      preComputedS
+00020b50: 656e 7469 6e65 6c32 5444 4f4d 4952 4d65  entinel2TDOMIRMe
+00020b60: 616e 203d 204e 6f6e 652c 0d0a 2020 2020  an = None,..    
+00020b70: 2020 7072 6543 6f6d 7075 7465 6453 656e    preComputedSen
+00020b80: 7469 6e65 6c32 5444 4f4d 4952 5374 6444  tinel2TDOMIRStdD
+00020b90: 6576 203d 204e 6f6e 652c 0d0a 2020 2020  ev = None,..    
+00020ba0: 2020 636c 6f75 6450 726f 6254 6872 6573    cloudProbThres
+00020bb0: 6820 3d20 3430 2c0d 0a20 2020 2020 206c  h = 40,..      l
+00020bc0: 616e 6473 6174 436f 6c6c 6563 7469 6f6e  andsatCollection
+00020bd0: 5665 7273 696f 6e20 3d20 2743 3227 293a  Version = 'C2'):
+00020be0: 0d0a 0d0a 2020 6966 2074 6f61 4f72 5352  ....  if toaOrSR
+00020bf0: 203d 3d20 2753 5227 3a0d 0a20 2020 2072   == 'SR':..    r
+00020c00: 756e 4368 6173 7461 696e 4861 726d 6f6e  unChastainHarmon
+00020c10: 697a 6174 696f 6e20 3d20 4661 6c73 650d  ization = False.
+00020c20: 0a0d 0a20 206f 7269 6769 6e20 3d20 274c  ...  origin = 'L
+00020c30: 616e 6473 6174 2d53 656e 7469 6e65 6c32  andsat-Sentinel2
+00020c40: 2d48 7962 7269 6427 0d0a 2020 746f 614f  -Hybrid'..  toaO
+00020c50: 7253 5220 3d20 746f 614f 7253 522e 7570  rSR = toaOrSR.up
+00020c60: 7065 7228 290d 0a0d 0a20 2023 5072 6570  per()....  #Prep
+00020c70: 6172 6520 6461 7465 730d 0a20 2023 5772  are dates..  #Wr
+00020c80: 6170 2074 6865 2064 6174 6573 2069 6620  ap the dates if 
+00020c90: 6e65 6564 6564 0d0a 2020 7772 6170 4f66  needed..  wrapOf
+00020ca0: 6673 6574 203d 2030 0d0a 2020 6966 2073  fset = 0..  if s
+00020cb0: 7461 7274 4a75 6c69 616e 203e 2065 6e64  tartJulian > end
+00020cc0: 4a75 6c69 616e 3a0d 0a20 2020 2077 7261  Julian:..    wra
+00020cd0: 704f 6666 7365 7420 3d20 3336 350d 0a20  pOffset = 365.. 
+00020ce0: 2073 7461 7274 4461 7465 203d 2065 652e   startDate = ee.
+00020cf0: 4461 7465 2e66 726f 6d59 4d44 2873 7461  Date.fromYMD(sta
+00020d00: 7274 5965 6172 2c31 2c31 292e 6164 7661  rtYear,1,1).adva
+00020d10: 6e63 6528 7374 6172 744a 756c 6961 6e2d  nce(startJulian-
+00020d20: 312c 2764 6179 2729 0d0a 2020 656e 6444  1,'day')..  endD
+00020d30: 6174 6520 3d20 6565 2e44 6174 652e 6672  ate = ee.Date.fr
+00020d40: 6f6d 594d 4428 656e 6459 6561 722c 312c  omYMD(endYear,1,
+00020d50: 3129 2e61 6476 616e 6365 2865 6e64 4a75  1).advance(endJu
+00020d60: 6c69 616e 2d31 2b77 7261 704f 6666 7365  lian-1+wrapOffse
+00020d70: 742c 2764 6179 2729 0d0a 0d0a 2020 6172  t,'day')....  ar
+00020d80: 6773 203d 2066 6f72 6d61 7441 7267 7328  gs = formatArgs(
+00020d90: 6c6f 6361 6c73 2829 290d 0a20 2069 6620  locals())..  if 
+00020da0: 2761 7267 7327 2069 6e20 6172 6773 2e6b  'args' in args.k
+00020db0: 6579 7328 293a 0d0a 2020 2020 6465 6c20  eys():..    del 
+00020dc0: 6172 6773 5b27 6172 6773 275d 0d0a 0d0a  args['args']....
+00020dd0: 2020 7072 696e 7428 2747 6574 2050 726f    print('Get Pro
+00020de0: 6365 7373 6564 204c 616e 6473 6174 2061  cessed Landsat a
+00020df0: 6e64 2053 656e 7469 6e65 6c32 2053 6365  nd Sentinel2 Sce
+00020e00: 6e65 733a 2027 290d 0a20 2070 7269 6e74  nes: ')..  print
+00020e10: 2827 5374 6172 7420 6461 7465 3a27 2c20  ('Start date:', 
+00020e20: 7374 6172 7444 6174 652e 666f 726d 6174  startDate.format
+00020e30: 2827 4d4d 4d20 6464 2079 7979 7927 292e  ('MMM dd yyyy').
+00020e40: 6765 7449 6e66 6f28 292c 272c 2045 6e64  getInfo(),', End
+00020e50: 2064 6174 653a 272c 2065 6e64 4461 7465   date:', endDate
+00020e60: 2e66 6f72 6d61 7428 274d 4d4d 2064 6420  .format('MMM dd 
+00020e70: 7979 7979 2729 2e67 6574 496e 666f 2829  yyyy').getInfo()
+00020e80: 290d 0a20 2066 6f72 2061 7267 2069 6e20  )..  for arg in 
+00020e90: 6172 6773 2e6b 6579 7328 293a 0d0a 2020  args.keys():..  
+00020ea0: 2020 7072 696e 7428 6172 672c 2027 3a20    print(arg, ': 
+00020eb0: 272c 2061 7267 735b 6172 675d 290d 0a0d  ', args[arg])...
+00020ec0: 0a20 2023 4765 7420 4c61 6e64 7361 740d  .  #Get Landsat.
+00020ed0: 0a20 206c 7320 3d20 6765 7450 726f 6365  .  ls = getProce
+00020ee0: 7373 6564 4c61 6e64 7361 7453 6365 6e65  ssedLandsatScene
+00020ef0: 7328 5c0d 0a20 2020 2073 7475 6479 4172  s(\..    studyAr
+00020f00: 6561 203d 2073 7475 6479 4172 6561 2c0d  ea = studyArea,.
+00020f10: 0a20 2020 2073 7461 7274 5965 6172 203d  .    startYear =
+00020f20: 2073 7461 7274 5965 6172 2c0d 0a20 2020   startYear,..   
+00020f30: 2065 6e64 5965 6172 203d 2065 6e64 5965   endYear = endYe
+00020f40: 6172 2c0d 0a20 2020 2073 7461 7274 4a75  ar,..    startJu
+00020f50: 6c69 616e 203d 2073 7461 7274 4a75 6c69  lian = startJuli
+00020f60: 616e 2c0d 0a20 2020 2065 6e64 4a75 6c69  an,..    endJuli
+00020f70: 616e 203d 2065 6e64 4a75 6c69 616e 2c0d  an = endJulian,.
+00020f80: 0a20 2020 2074 6f61 4f72 5352 203d 2074  .    toaOrSR = t
+00020f90: 6f61 4f72 5352 2c0d 0a20 2020 2069 6e63  oaOrSR,..    inc
+00020fa0: 6c75 6465 534c 434f 6666 4c37 203d 2069  ludeSLCOffL7 = i
+00020fb0: 6e63 6c75 6465 534c 434f 6666 4c37 2c0d  ncludeSLCOffL7,.
+00020fc0: 0a20 2020 2064 6566 7269 6e67 654c 3520  .    defringeL5 
+00020fd0: 3d20 6465 6672 696e 6765 4c35 2c0d 0a20  = defringeL5,.. 
+00020fe0: 2020 2061 7070 6c79 436c 6f75 6453 636f     applyCloudSco
+00020ff0: 7265 203d 2061 7070 6c79 436c 6f75 6453  re = applyCloudS
+00021000: 636f 7265 4c61 6e64 7361 742c 0d0a 2020  coreLandsat,..  
+00021010: 2020 6170 706c 7946 6d61 736b 436c 6f75    applyFmaskClou
+00021020: 644d 6173 6b20 3d20 6170 706c 7946 6d61  dMask = applyFma
+00021030: 736b 436c 6f75 644d 6173 6b2c 0d0a 2020  skCloudMask,..  
+00021040: 2020 6170 706c 7954 444f 4d20 3d20 6170    applyTDOM = ap
+00021050: 706c 7954 444f 4d4c 616e 6473 6174 2c0d  plyTDOMLandsat,.
+00021060: 0a20 2020 2061 7070 6c79 466d 6173 6b43  .    applyFmaskC
+00021070: 6c6f 7564 5368 6164 6f77 4d61 736b 203d  loudShadowMask =
+00021080: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
+00021090: 5368 6164 6f77 4d61 736b 2c0d 0a20 2020  ShadowMask,..   
+000210a0: 2061 7070 6c79 466d 6173 6b53 6e6f 774d   applyFmaskSnowM
+000210b0: 6173 6b20 3d20 6170 706c 7946 6d61 736b  ask = applyFmask
+000210c0: 536e 6f77 4d61 736b 2c0d 0a20 2020 2063  SnowMask,..    c
+000210d0: 6c6f 7564 5363 6f72 6554 6872 6573 6820  loudScoreThresh 
+000210e0: 3d20 636c 6f75 6453 636f 7265 5468 7265  = cloudScoreThre
+000210f0: 7368 2c0d 0a20 2020 2070 6572 666f 726d  sh,..    perform
+00021100: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
+00021110: 203d 2070 6572 666f 726d 436c 6f75 6453   = performCloudS
+00021120: 636f 7265 4f66 6673 6574 2c0d 0a20 2020  coreOffset,..   
+00021130: 2063 6c6f 7564 5363 6f72 6550 6374 6c20   cloudScorePctl 
+00021140: 3d20 636c 6f75 6453 636f 7265 5063 746c  = cloudScorePctl
+00021150: 2c0d 0a20 2020 207a 5363 6f72 6554 6872  ,..    zScoreThr
+00021160: 6573 6820 3d20 7a53 636f 7265 5468 7265  esh = zScoreThre
+00021170: 7368 2c0d 0a20 2020 2073 6861 646f 7753  sh,..    shadowS
+00021180: 756d 5468 7265 7368 203d 2073 6861 646f  umThresh = shado
+00021190: 7753 756d 5468 7265 7368 2c0d 0a20 2020  wSumThresh,..   
+000211a0: 2063 6f6e 7472 6163 7450 6978 656c 7320   contractPixels 
+000211b0: 3d20 636f 6e74 7261 6374 5069 7865 6c73  = contractPixels
+000211c0: 2c0d 0a20 2020 2064 696c 6174 6550 6978  ,..    dilatePix
+000211d0: 656c 7320 3d20 6469 6c61 7465 5069 7865  els = dilatePixe
+000211e0: 6c73 2c0d 0a20 2020 2073 6861 646f 7753  ls,..    shadowS
+000211f0: 756d 4261 6e64 7320 3d20 7368 6164 6f77  umBands = shadow
+00021200: 5375 6d42 616e 6473 2c0d 0a20 2020 2072  SumBands,..    r
+00021210: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
+00021220: 6c61 6e64 7361 7452 6573 616d 706c 654d  landsatResampleM
+00021230: 6574 686f 642c 0d0a 2020 2020 2368 6172  ethod,..    #har
+00021240: 6d6f 6e69 7a65 4f4c 4920 3d20 6861 726d  monizeOLI = harm
+00021250: 6f6e 697a 654f 4c49 2c0d 0a20 2020 2070  onizeOLI,..    p
+00021260: 7265 436f 6d70 7574 6564 436c 6f75 6453  reComputedCloudS
+00021270: 636f 7265 4f66 6673 6574 203d 2070 7265  coreOffset = pre
+00021280: 436f 6d70 7574 6564 4c61 6e64 7361 7443  ComputedLandsatC
+00021290: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
+000212a0: 0d0a 2020 2020 7072 6543 6f6d 7075 7465  ..    preCompute
+000212b0: 6454 444f 4d49 524d 6561 6e20 3d20 7072  dTDOMIRMean = pr
+000212c0: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
+000212d0: 5444 4f4d 4952 4d65 616e 2c0d 0a20 2020  TDOMIRMean,..   
+000212e0: 2070 7265 436f 6d70 7574 6564 5444 4f4d   preComputedTDOM
+000212f0: 4952 5374 6444 6576 203d 2070 7265 436f  IRStdDev = preCo
+00021300: 6d70 7574 6564 5365 6e74 696e 656c 3254  mputedSentinel2T
+00021310: 444f 4d49 5253 7464 4465 762c 0d0a 2020  DOMIRStdDev,..  
+00021320: 2020 6c61 6e64 7361 7443 6f6c 6c65 6374    landsatCollect
+00021330: 696f 6e56 6572 7369 6f6e 203d 206c 616e  ionVersion = lan
+00021340: 6473 6174 436f 6c6c 6563 7469 6f6e 5665  dsatCollectionVe
+00021350: 7273 696f 6e29 0d0a 0d0a 2020 2347 6574  rsion)....  #Get
+00021360: 2053 656e 7469 6e65 6c20 320d 0a20 2073   Sentinel 2..  s
+00021370: 3273 203d 2067 6574 5072 6f63 6573 7365  2s = getProcesse
+00021380: 6453 656e 7469 6e65 6c32 5363 656e 6573  dSentinel2Scenes
+00021390: 285c 0d0a 2020 2020 7374 7564 7941 7265  (\..    studyAre
+000213a0: 6120 3d20 7374 7564 7941 7265 612c 0d0a  a = studyArea,..
+000213b0: 2020 2020 7374 6172 7459 6561 7220 3d20      startYear = 
+000213c0: 7374 6172 7459 6561 722c 0d0a 2020 2020  startYear,..    
+000213d0: 656e 6459 6561 7220 3d20 656e 6459 6561  endYear = endYea
+000213e0: 722c 0d0a 2020 2020 7374 6172 744a 756c  r,..    startJul
+000213f0: 6961 6e20 3d20 7374 6172 744a 756c 6961  ian = startJulia
+00021400: 6e2c 0d0a 2020 2020 656e 644a 756c 6961  n,..    endJulia
+00021410: 6e20 3d20 656e 644a 756c 6961 6e2c 0d0a  n = endJulian,..
+00021420: 2020 2020 6170 706c 7951 4142 616e 6420      applyQABand 
+00021430: 3d20 6170 706c 7951 4142 616e 642c 0d0a  = applyQABand,..
+00021440: 2020 2020 6170 706c 7943 6c6f 7564 5363      applyCloudSc
+00021450: 6f72 6520 3d20 6170 706c 7943 6c6f 7564  ore = applyCloud
+00021460: 5363 6f72 6553 656e 7469 6e65 6c32 2c0d  ScoreSentinel2,.
+00021470: 0a20 2020 2061 7070 6c79 5368 6164 6f77  .    applyShadow
+00021480: 5368 6966 7420 3d20 6170 706c 7953 6861  Shift = applySha
+00021490: 646f 7753 6869 6674 2c0d 0a20 2020 2061  dowShift,..    a
+000214a0: 7070 6c79 5444 4f4d 203d 2061 7070 6c79  pplyTDOM = apply
+000214b0: 5444 4f4d 5365 6e74 696e 656c 322c 0d0a  TDOMSentinel2,..
+000214c0: 2020 2020 636c 6f75 6453 636f 7265 5468      cloudScoreTh
+000214d0: 7265 7368 203d 2063 6c6f 7564 5363 6f72  resh = cloudScor
+000214e0: 6554 6872 6573 682c 0d0a 2020 2020 7065  eThresh,..    pe
+000214f0: 7266 6f72 6d43 6c6f 7564 5363 6f72 654f  rformCloudScoreO
+00021500: 6666 7365 7420 3d20 7065 7266 6f72 6d43  ffset = performC
+00021510: 6c6f 7564 5363 6f72 654f 6666 7365 742c  loudScoreOffset,
+00021520: 0d0a 2020 2020 636c 6f75 6453 636f 7265  ..    cloudScore
+00021530: 5063 746c 203d 2063 6c6f 7564 5363 6f72  Pctl = cloudScor
+00021540: 6550 6374 6c2c 0d0a 2020 2020 636c 6f75  ePctl,..    clou
+00021550: 6448 6569 6768 7473 203d 2063 6c6f 7564  dHeights = cloud
+00021560: 4865 6967 6874 732c 0d0a 2020 2020 7a53  Heights,..    zS
+00021570: 636f 7265 5468 7265 7368 203d 207a 5363  coreThresh = zSc
+00021580: 6f72 6554 6872 6573 682c 0d0a 2020 2020  oreThresh,..    
+00021590: 7368 6164 6f77 5375 6d54 6872 6573 6820  shadowSumThresh 
+000215a0: 3d20 7368 6164 6f77 5375 6d54 6872 6573  = shadowSumThres
+000215b0: 682c 0d0a 2020 2020 636f 6e74 7261 6374  h,..    contract
+000215c0: 5069 7865 6c73 203d 2063 6f6e 7472 6163  Pixels = contrac
+000215d0: 7450 6978 656c 732c 0d0a 2020 2020 6469  tPixels,..    di
+000215e0: 6c61 7465 5069 7865 6c73 203d 2064 696c  latePixels = dil
+000215f0: 6174 6550 6978 656c 732c 0d0a 2020 2020  atePixels,..    
+00021600: 7368 6164 6f77 5375 6d42 616e 6473 203d  shadowSumBands =
+00021610: 2073 6861 646f 7753 756d 4261 6e64 732c   shadowSumBands,
+00021620: 0d0a 2020 2020 7265 7361 6d70 6c65 4d65  ..    resampleMe
+00021630: 7468 6f64 203d 2073 656e 7469 6e65 6c32  thod = sentinel2
+00021640: 5265 7361 6d70 6c65 4d65 7468 6f64 2c0d  ResampleMethod,.
+00021650: 0a20 2020 2074 6f61 4f72 5352 203d 2074  .    toaOrSR = t
+00021660: 6f61 4f72 5352 2c0d 0a20 2020 2063 6f6e  oaOrSR,..    con
+00021670: 7665 7274 546f 4461 696c 794d 6f73 6169  vertToDailyMosai
+00021680: 6373 203d 2063 6f6e 7665 7274 546f 4461  cs = convertToDa
+00021690: 696c 794d 6f73 6169 6373 2c0d 0a20 2020  ilyMosaics,..   
+000216a0: 2061 7070 6c79 436c 6f75 6450 726f 6261   applyCloudProba
+000216b0: 6269 6c69 7479 203d 2061 7070 6c79 436c  bility = applyCl
+000216c0: 6f75 6450 726f 6261 6269 6c69 7479 2c0d  oudProbability,.
+000216d0: 0a20 2020 2070 7265 436f 6d70 7574 6564  .    preComputed
+000216e0: 436c 6f75 6453 636f 7265 4f66 6673 6574  CloudScoreOffset
+000216f0: 203d 2070 7265 436f 6d70 7574 6564 5365   = preComputedSe
+00021700: 6e74 696e 656c 3243 6c6f 7564 5363 6f72  ntinel2CloudScor
+00021710: 654f 6666 7365 742c 0d0a 2020 2020 7072  eOffset,..    pr
+00021720: 6543 6f6d 7075 7465 6454 444f 4d49 524d  eComputedTDOMIRM
+00021730: 6561 6e20 3d20 7072 6543 6f6d 7075 7465  ean = preCompute
+00021740: 6453 656e 7469 6e65 6c32 5444 4f4d 4952  dSentinel2TDOMIR
+00021750: 4d65 616e 2c0d 0a20 2020 2070 7265 436f  Mean,..    preCo
+00021760: 6d70 7574 6564 5444 4f4d 4952 5374 6444  mputedTDOMIRStdD
+00021770: 6576 203d 2070 7265 436f 6d70 7574 6564  ev = preComputed
+00021780: 5365 6e74 696e 656c 3254 444f 4d49 5253  Sentinel2TDOMIRS
+00021790: 7464 4465 762c 0d0a 2020 2020 636c 6f75  tdDev,..    clou
+000217a0: 6450 726f 6254 6872 6573 6820 3d20 636c  dProbThresh = cl
+000217b0: 6f75 6450 726f 6254 6872 6573 6829 0d0a  oudProbThresh)..
+000217c0: 0d0a 0d0a 2020 2353 656c 6563 7420 6f66  ....  #Select of
+000217d0: 6620 636f 6d6d 6f6e 2062 616e 6473 2062  f common bands b
+000217e0: 6574 7765 656e 204c 616e 6473 6174 2061  etween Landsat a
+000217f0: 6e64 2053 656e 7469 6e65 6c20 320d 0a20  nd Sentinel 2.. 
+00021800: 2063 6f6d 6d6f 6e42 616e 6473 203d 2020   commonBands =  
+00021810: 5b27 626c 7565 272c 2027 6772 6565 6e27  ['blue', 'green'
+00021820: 2c20 2772 6564 272c 2027 6e69 7227 2c20  , 'red', 'nir', 
+00021830: 2773 7769 7231 272c 2027 7377 6972 3227  'swir1', 'swir2'
+00021840: 2c20 2773 656e 736f 7227 5d0d 0a20 206c  , 'sensor']..  l
+00021850: 7320 3d20 6c73 2e73 656c 6563 7428 636f  s = ls.select(co
+00021860: 6d6d 6f6e 4261 6e64 7329 0d0a 2020 7332  mmonBands)..  s2
+00021870: 7320 3d20 7332 732e 7365 6c65 6374 2863  s = s2s.select(c
+00021880: 6f6d 6d6f 6e42 616e 6473 290d 0a20 2023  ommonBands)..  #
+00021890: 4669 6c6c 2069 6e20 616e 7920 656d 7074  Fill in any empt
+000218a0: 7920 636f 6c6c 6563 7469 6f6e 730d 0a20  y collections.. 
+000218b0: 2023 4966 2074 6865 7927 7265 2062 6f74   #If they're bot
+000218c0: 6820 656d 7074 792c 2074 6869 7320 7769  h empty, this wi
+000218d0: 6c6c 206e 6f74 2077 6f72 6b0d 0a20 2064  ll not work..  d
+000218e0: 756d 6d79 496d 6167 6520 3d65 652e 496d  ummyImage =ee.Im
+000218f0: 6167 6528 6565 2e49 6d61 6765 436f 6c6c  age(ee.ImageColl
+00021900: 6563 7469 6f6e 2865 652e 416c 676f 7269  ection(ee.Algori
+00021910: 7468 6d73 2e49 6628 6c73 2e74 6f4c 6973  thms.If(ls.toLis
+00021920: 7428 3129 2e6c 656e 6774 6828 292e 6774  t(1).length().gt
+00021930: 2830 292c 6c73 2c73 3273 2929 2e66 6972  (0),ls,s2s)).fir
+00021940: 7374 2829 290d 0a20 206c 7320 3d20 6669  st())..  ls = fi
+00021950: 6c6c 456d 7074 7943 6f6c 6c65 6374 696f  llEmptyCollectio
+00021960: 6e73 286c 732c 6475 6d6d 7949 6d61 6765  ns(ls,dummyImage
+00021970: 290d 0a20 2073 3273 203d 2066 696c 6c45  )..  s2s = fillE
+00021980: 6d70 7479 436f 6c6c 6563 7469 6f6e 7328  mptyCollections(
+00021990: 7332 732c 6475 6d6d 7949 6d61 6765 290d  s2s,dummyImage).
+000219a0: 0a0d 0a0d 0a20 2069 6620 7275 6e43 6861  .....  if runCha
+000219b0: 7374 6169 6e48 6172 6d6f 6e69 7a61 7469  stainHarmonizati
+000219c0: 6f6e 2061 6e64 2074 6f61 4f72 5352 203d  on and toaOrSR =
+000219d0: 3d20 2754 4f41 273a 0d0a 0d0a 2020 2020  = 'TOA':....    
+000219e0: 2320 5365 7061 7261 7465 2065 6163 6820  # Separate each 
+000219f0: 7365 6e73 6f72 0d0a 0d0a 2020 2020 746d  sensor....    tm
+00021a00: 203d 206c 732e 6669 6c74 6572 2865 652e   = ls.filter(ee.
+00021a10: 4669 6c74 6572 2e69 6e4c 6973 7428 2753  Filter.inList('S
+00021a20: 454e 534f 525f 4944 272c 5b27 544d 272c  ENSOR_ID',['TM',
+00021a30: 2745 544d 275d 2929 0d0a 2020 2020 6f6c  'ETM']))..    ol
+00021a40: 6920 3d20 6c73 2e66 696c 7465 7228 6565  i = ls.filter(ee
+00021a50: 2e46 696c 7465 722e 6571 2827 5345 4e53  .Filter.eq('SENS
+00021a60: 4f52 5f49 4427 2c27 4f4c 495f 5449 5253  OR_ID','OLI_TIRS
+00021a70: 2729 290d 0a20 2020 2023 2065 6c73 653a  '))..    # else:
+00021a80: 0d0a 2020 2020 2320 2020 746d 203d 206c  ..    #   tm = l
+00021a90: 732e 6669 6c74 6572 2865 652e 4669 6c74  s.filter(ee.Filt
+00021aa0: 6572 2e69 6e4c 6973 7428 2773 656e 736f  er.inList('senso
+00021ab0: 7227 2c5b 274c 414e 4453 4154 5f34 272c  r',['LANDSAT_4',
+00021ac0: 274c 414e 4453 4154 5f35 272c 274c 414e  'LANDSAT_5','LAN
+00021ad0: 4453 4154 5f37 275d 2929 0d0a 2020 2020  DSAT_7']))..    
+00021ae0: 2320 2020 6f6c 6920 3d20 6c73 2e66 696c  #   oli = ls.fil
+00021af0: 7465 7228 6565 2e46 696c 7465 722e 6571  ter(ee.Filter.eq
+00021b00: 2827 7365 6e73 6f72 272c 274c 414e 4453  ('sensor','LANDS
+00021b10: 4154 5f38 2729 290d 0a20 2020 206d 7369  AT_8'))..    msi
+00021b20: 203d 2073 3273 0d0a 0d0a 2020 2020 2320   = s2s....    # 
+00021b30: 4669 6c6c 2069 6620 6e6f 2069 6d61 6765  Fill if no image
+00021b40: 7320 6578 6973 7420 666f 7220 7061 7274  s exist for part
+00021b50: 6963 756c 6172 204c 616e 6473 6174 2073  icular Landsat s
+00021b60: 656e 736f 720d 0a20 2020 2023 2041 6c6c  ensor..    # All
+00021b70: 6f77 2069 7420 746f 2066 6169 6c20 6f66  ow it to fail of
+00021b80: 206e 6f20 696d 6167 6573 2065 7869 7374   no images exist
+00021b90: 2066 6f72 2053 656e 7469 6e65 6c20 3220   for Sentinel 2 
+00021ba0: 7369 6e63 6520 7468 6520 706f 696e 740d  since the point.
+00021bb0: 0a20 2020 2023 206f 6620 7468 6973 206d  .    # of this m
+00021bc0: 6574 686f 6420 6973 2074 6f20 696e 636c  ethod is to incl
+00021bd0: 7564 6520 5332 0d0a 2020 2020 746d 203d  ude S2..    tm =
+00021be0: 2066 696c 6c45 6d70 7479 436f 6c6c 6563   fillEmptyCollec
+00021bf0: 7469 6f6e 7328 746d 2c20 6565 2e49 6d61  tions(tm, ee.Ima
+00021c00: 6765 286c 732e 6669 7273 7428 2929 290d  ge(ls.first())).
+00021c10: 0a20 2020 206f 6c69 203d 2066 696c 6c45  .    oli = fillE
+00021c20: 6d70 7479 436f 6c6c 6563 7469 6f6e 7328  mptyCollections(
+00021c30: 6f6c 692c 2065 652e 496d 6167 6528 6c73  oli, ee.Image(ls
+00021c40: 2e66 6972 7374 2829 2929 0d0a 0d0a 2020  .first()))....  
+00021c50: 2020 7072 696e 7428 2752 756e 6e69 6e67    print('Running
+00021c60: 2043 6861 7374 6169 6e20 6574 2061 6c20   Chastain et al 
+00021c70: 3230 3139 2068 6172 6d6f 6e69 7a61 7469  2019 harmonizati
+00021c80: 6f6e 2729 0d0a 0d0a 2020 2020 2341 7070  on')....    #App
+00021c90: 6c79 2063 6f72 7265 6374 696f 6e0d 0a20  ly correction.. 
+00021ca0: 2020 2023 4375 7272 656e 746c 7920 636f     #Currently co
+00021cb0: 6465 6420 746f 2067 6f20 746f 2045 544d  ded to go to ETM
+00021cc0: 2b0d 0a0d 0a20 2020 2023 4e6f 206e 6565  +....    #No nee
+00021cd0: 6420 746f 2063 6f72 7265 6374 2045 544d  d to correct ETM
+00021ce0: 2074 6f20 4554 4d0d 0a20 2020 2023 2074   to ETM..    # t
+00021cf0: 6d20 3d20 746d 2e6d 6170 2866 756e 6374  m = tm.map(funct
+00021d00: 696f 6e28 696d 6729 7b72 6574 7572 6e20  ion(img){return 
+00021d10: 6765 7449 6d61 6765 734c 6962 2e68 6172  getImagesLib.har
+00021d20: 6d6f 6e69 7a61 7469 6f6e 4368 6173 7461  monizationChasta
+00021d30: 696e 2869 6d67 2c20 2745 544d 272c 2745  in(img, 'ETM','E
+00021d40: 544d 2729 7d29 0d0a 2020 2020 2320 6574  TM')})..    # et
+00021d50: 6d20 3d20 6574 6d2e 6d61 7028 6675 6e63  m = etm.map(func
+00021d60: 7469 6f6e 2869 6d67 297b 7265 7475 726e  tion(img){return
+00021d70: 2067 6574 496d 6167 6573 4c69 622e 6861   getImagesLib.ha
+00021d80: 726d 6f6e 697a 6174 696f 6e43 6861 7374  rmonizationChast
+00021d90: 6169 6e28 696d 672c 2027 4554 4d27 2c27  ain(img, 'ETM','
+00021da0: 4554 4d27 297d 290d 0a0d 0a20 2020 2023  ETM')})....    #
+00021db0: 4861 726d 6f6e 697a 6520 7468 6520 6f74  Harmonize the ot
+00021dc0: 6865 7220 7477 6f0d 0a20 2020 206f 6c69  her two..    oli
+00021dd0: 203d 206f 6c69 2e6d 6170 286c 616d 6264   = oli.map(lambd
+00021de0: 6120 696d 673a 2068 6172 6d6f 6e69 7a61  a img: harmoniza
+00021df0: 7469 6f6e 4368 6173 7461 696e 2869 6d67  tionChastain(img
+00021e00: 2c20 274f 4c49 272c 2745 544d 2729 290d  , 'OLI','ETM')).
+00021e10: 0a20 2020 206d 7369 203d 206d 7369 2e6d  .    msi = msi.m
+00021e20: 6170 286c 616d 6264 6120 696d 673a 2068  ap(lambda img: h
+00021e30: 6172 6d6f 6e69 7a61 7469 6f6e 4368 6173  armonizationChas
+00021e40: 7461 696e 2869 6d67 2c20 274d 5349 272c  tain(img, 'MSI',
+00021e50: 2745 544d 2729 290d 0a0d 0a20 2020 2073  'ETM'))....    s
+00021e60: 3273 203d 206d 7369 0d0a 0d0a 2020 2020  2s = msi....    
+00021e70: 234d 6572 6765 204c 616e 6473 6174 2062  #Merge Landsat b
+00021e80: 6163 6b20 746f 6765 7468 6572 0d0a 2020  ack together..  
+00021e90: 2020 6c73 203d 2065 652e 496d 6167 6543    ls = ee.ImageC
+00021ea0: 6f6c 6c65 6374 696f 6e28 746d 2e6d 6572  ollection(tm.mer
+00021eb0: 6765 286f 6c69 2929 0d0a 0d0a 0d0a 2020  ge(oli))......  
+00021ec0: 2320 4d65 7267 6520 4c61 6e64 7361 7420  # Merge Landsat 
+00021ed0: 616e 6420 5332 0d0a 2020 6d65 7267 6564  and S2..  merged
+00021ee0: 203d 2065 652e 496d 6167 6543 6f6c 6c65   = ee.ImageColle
+00021ef0: 6374 696f 6e28 6c73 2e6d 6572 6765 2873  ction(ls.merge(s
+00021f00: 3273 2929 0d0a 2020 6d65 7267 6564 203d  2s))..  merged =
+00021f10: 206d 6572 6765 642e 6d61 7028 7369 6d70   merged.map(simp
+00021f20: 6c65 4164 6449 6e64 6963 6573 295c 0d0a  leAddIndices)\..
+00021f30: 2020 2020 2020 2020 2020 2020 2e6d 6170              .map
+00021f40: 2867 6574 5461 7373 656c 6564 4361 7029  (getTasseledCap)
+00021f50: 5c0d 0a20 2020 2020 2020 2020 2020 202e  \..            .
+00021f60: 6d61 7028 7369 6d70 6c65 4164 6454 4341  map(simpleAddTCA
+00021f70: 6e67 6c65 7329 0d0a 0d0a 2020 6d65 7267  ngles)....  merg
+00021f80: 6564 203d 206d 6572 6765 642e 7365 7428  ed = merged.set(
+00021f90: 6172 6773 290d 0a0d 0a0d 0a20 2072 6574  args)......  ret
+00021fa0: 7572 6e20 6d65 7267 6564 0d0a 2323 2323  urn merged..####
+00021fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021fe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021ff0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
+00022000: 4675 6e63 7469 6f6e 2074 6f20 7265 6769  Function to regi
+00022010: 7374 6572 2061 6e20 696d 6167 6543 6f6c  ster an imageCol
+00022020: 6c65 6374 696f 6e20 746f 2069 6d61 6765  lection to image
+00022030: 7320 7769 7468 696e 2069 740d 0a23 416c  s within it..#Al
+00022040: 7761 7973 2075 7365 7320 7468 6520 6669  ways uses the fi
+00022050: 7273 7420 696d 6167 6520 6173 2074 6865  rst image as the
+00022060: 2072 6566 6572 656e 6365 2069 6d61 6765   reference image
+00022070: 0d0a 6465 6620 636f 5265 6769 7374 6572  ..def coRegister
+00022080: 436f 6c6c 6563 7469 6f6e 2869 6d61 6765  Collection(image
+00022090: 732c 7265 6665 7265 6e63 6542 616e 6473  s,referenceBands
+000220a0: 203d 205b 276e 6972 275d 293a 0d0a 2020   = ['nir']):..  
+000220b0: 2020 7265 6665 7265 6e63 6549 6d61 6765    referenceImage
+000220c0: 496e 6465 7820 3d20 300d 0a20 2020 2072  Index = 0..    r
+000220d0: 6566 6572 656e 6365 496d 6167 6520 3d20  eferenceImage = 
+000220e0: 6565 2e49 6d61 6765 2869 6d61 6765 732e  ee.Image(images.
+000220f0: 746f 4c69 7374 2872 6566 6572 656e 6365  toList(reference
+00022100: 496d 6167 6549 6e64 6578 2b31 292e 6765  ImageIndex+1).ge
+00022110: 7428 7265 6665 7265 6e63 6549 6d61 6765  t(referenceImage
+00022120: 496e 6465 7829 292e 7365 6c65 6374 2872  Index)).select(r
+00022130: 6566 6572 656e 6365 4261 6e64 7329 0d0a  eferenceBands)..
+00022140: 0d0a 2020 2020 6465 6620 7265 6769 7374  ..    def regist
+00022150: 6572 496d 6167 6528 696d 6167 6529 3a0d  erImage(image):.
+00022160: 0a20 2020 2020 2020 2023 4465 7465 726d  .        #Determ
+00022170: 696e 6520 7468 6520 6469 7370 6c61 6365  ine the displace
+00022180: 6d65 6e74 2062 7920 6d61 7463 6869 6e67  ment by matching
+00022190: 206f 6e6c 7920 7468 6520 7265 6665 7265   only the refere
+000221a0: 6e63 6542 616e 6420 6261 6e64 732e 0d0a  nceBand bands...
+000221b0: 2020 2020 2020 2020 6469 7370 6c61 6365          displace
+000221c0: 6d65 6e74 5f70 6172 616d 7320 3d20 7b0d  ment_params = {.
+000221d0: 0a20 2020 2020 2020 2020 2020 2027 7265  .            're
+000221e0: 6665 7265 6e63 6549 6d61 6765 273a 2072  ferenceImage': r
+000221f0: 6566 6572 656e 6365 496d 6167 652c 0d0a  eferenceImage,..
+00022200: 2020 2020 2020 2020 2020 2020 276d 6178              'max
+00022210: 4f66 6673 6574 273a 2032 302e 302c 0d0a  Offset': 20.0,..
+00022220: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
+00022230: 6a65 6374 696f 6e27 3a20 4e6f 6e65 2c0d  jection': None,.
+00022240: 0a20 2020 2020 2020 2020 2020 2027 7061  .            'pa
+00022250: 7463 6857 6964 7468 273a 2032 302e 302c  tchWidth': 20.0,
+00022260: 0d0a 2020 2020 2020 2020 2020 2020 2773  ..            's
+00022270: 7469 6666 6e65 7373 273a 2035 0d0a 2020  tiffness': 5..  
+00022280: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+00022290: 2020 2020 2064 6973 706c 6163 656d 656e       displacemen
+000222a0: 7420 3d20 696d 6167 652e 7365 6c65 6374  t = image.select
+000222b0: 2872 6566 6572 656e 6365 4261 6e64 7329  (referenceBands)
+000222c0: 2e64 6973 706c 6163 656d 656e 7428 2a2a  .displacement(**
+000222d0: 6469 7370 6c61 6365 6d65 6e74 5f70 6172  displacement_par
+000222e0: 616d 7329 0d0a 2020 2020 2020 2020 7265  ams)..        re
+000222f0: 7475 726e 2069 6d61 6765 2e64 6973 706c  turn image.displ
+00022300: 6163 6528 6469 7370 6c61 6365 6d65 6e74  ace(displacement
+00022310: 290d 0a0d 0a20 2020 206f 7574 203d 2065  )....    out = e
+00022320: 652e 496d 6167 6543 6f6c 6c65 6374 696f  e.ImageCollectio
+00022330: 6e28 6565 2e49 6d61 6765 436f 6c6c 6563  n(ee.ImageCollec
+00022340: 7469 6f6e 2869 6d61 6765 732e 746f 4c69  tion(images.toLi
+00022350: 7374 2831 3030 3030 2c31 2929 2e6d 6170  st(10000,1)).map
+00022360: 2872 6567 6973 7465 7249 6d61 6765 2929  (registerImage))
+00022370: 2328 6565 2e49 6d61 6765 2869 6d61 6765  #(ee.Image(image
+00022380: 732e 746f 4c69 7374 2831 3030 3030 2c30  s.toList(10000,0
+00022390: 292e 6765 7428 3129 292c 7265 6665 7265  ).get(1)),refere
+000223a0: 6e63 6549 6d61 6765 290d 0a20 2020 206f  nceImage)..    o
+000223b0: 7574 203d 2065 652e 496d 6167 6543 6f6c  ut = ee.ImageCol
+000223c0: 6c65 6374 696f 6e28 696d 6167 6573 2e6c  lection(images.l
+000223d0: 696d 6974 2831 292e 6d65 7267 6528 6f75  imit(1).merge(ou
+000223e0: 7429 290d 0a0d 0a20 2020 2072 6574 7572  t))....    retur
+000223f0: 6e20 6f75 740d 0a23 2323 2323 2323 2323  n out..#########
+00022400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022440: 2323 2323 2323 2323 0d0a 2346 756e 6374  ########..#Funct
+00022450: 696f 6e20 746f 2066 696e 6420 6120 7375  ion to find a su
+00022460: 6273 6574 206f 6620 6120 636f 6c6c 6563  bset of a collec
+00022470: 7469 6f6e 0d0a 2346 6f72 2065 6163 6820  tion..#For each 
+00022480: 6772 6f75 7020 2865 2e67 2e20 7469 6c65  group (e.g. tile
+00022490: 206f 7220 6f72 6269 7420 6f72 2070 6174   or orbit or pat
+000224a0: 6829 2c20 616c 6c20 696d 6167 6573 2077  h), all images w
+000224b0: 6974 6869 6e20 7468 6174 2067 726f 7570  ithin that group
+000224c0: 2077 696c 6c20 6265 2072 6567 6973 7465   will be registe
+000224d0: 7265 640d 0a23 4173 2073 696e 676c 6520  red..#As single 
+000224e0: 636f 6c6c 6563 7469 6f6e 2069 7320 7265  collection is re
+000224f0: 7475 726e 6564 0d0a 6465 6620 636f 5265  turned..def coRe
+00022500: 6769 7374 6572 4772 6f75 7073 2869 6d67  gisterGroups(img
+00022510: 732c 6669 656c 644e 616d 6520 3d20 2753  s,fieldName = 'S
+00022520: 454e 5349 4e47 5f4f 5242 4954 5f4e 554d  ENSING_ORBIT_NUM
+00022530: 4245 5227 2c66 6965 6c64 4973 4e75 6d65  BER',fieldIsNume
+00022540: 7269 6320 3d20 5472 7565 293a 0d0a 2020  ric = True):..  
+00022550: 2020 6772 6f75 7073 203d 2065 652e 4469    groups = ee.Di
+00022560: 6374 696f 6e61 7279 2869 6d67 732e 6167  ctionary(imgs.ag
+00022570: 6772 6567 6174 655f 6869 7374 6f67 7261  gregate_histogra
+00022580: 6d28 6669 656c 644e 616d 6529 292e 6b65  m(fieldName)).ke
+00022590: 7973 2829 0d0a 2020 2020 6966 2066 6965  ys()..    if fie
+000225a0: 6c64 4973 4e75 6d65 7269 633a 0d0a 2020  ldIsNumeric:..  
+000225b0: 2020 2020 2020 6772 6f75 7073 203d 2067        groups = g
+000225c0: 726f 7570 732e 6d61 7028 6c61 6d62 6461  roups.map(lambda
+000225d0: 206e 3a20 6565 2e4e 756d 6265 722e 7061   n: ee.Number.pa
+000225e0: 7273 6528 6e29 290d 0a0d 0a20 2020 206f  rse(n))....    o
+000225f0: 7574 203d 6565 2e49 6d61 6765 436f 6c6c  ut =ee.ImageColl
+00022600: 6563 7469 6f6e 2865 652e 4665 6174 7572  ection(ee.Featur
+00022610: 6543 6f6c 6c65 6374 696f 6e28 6772 6f75  eCollection(grou
+00022620: 7073 2e6d 6170 286c 616d 6264 6120 6772  ps.map(lambda gr
+00022630: 6f75 703a 636f 5265 6769 7374 6572 436f  oup:coRegisterCo
+00022640: 6c6c 6563 7469 6f6e 2869 6d67 732e 6669  llection(imgs.fi
+00022650: 6c74 6572 2865 652e 4669 6c74 6572 2e65  lter(ee.Filter.e
+00022660: 7128 6669 656c 644e 616d 652c 6772 6f75  q(fieldName,grou
+00022670: 7029 2929 2929 2e66 6c61 7474 656e 2829  p))))).flatten()
+00022680: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
+00022690: 6f75 740d 0a23 2323 2323 2323 2323 2323  out..###########
+000226a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000226b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000226c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000226d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000226e0: 2323 2323 2323 0d0a 6465 6620 6765 744c  ######..def getL
+000226f0: 616e 6473 6174 416e 6453 656e 7469 6e65  andsatAndSentine
+00022700: 6c32 4879 6272 6964 5772 6170 7065 7228  l2HybridWrapper(
+00022710: 5c0d 0a20 2073 7475 6479 4172 6561 2c0d  \..  studyArea,.
+00022720: 0a20 2073 7461 7274 5965 6172 2c0d 0a20  .  startYear,.. 
+00022730: 2065 6e64 5965 6172 2c0d 0a20 2073 7461   endYear,..  sta
+00022740: 7274 4a75 6c69 616e 2c0d 0a20 2065 6e64  rtJulian,..  end
+00022750: 4a75 6c69 616e 2c0d 0a20 2074 696d 6562  Julian,..  timeb
+00022760: 7566 6665 7220 3d20 2030 2c0d 0a20 2077  uffer =  0,..  w
+00022770: 6569 6768 7473 203d 2020 5b31 5d2c 0d0a  eights =  [1],..
+00022780: 2020 636f 6d70 6f73 6974 696e 674d 6574    compositingMet
+00022790: 686f 6420 3d20 276d 6564 6f69 6427 2c0d  hod = 'medoid',.
+000227a0: 0a20 2074 6f61 4f72 5352 203d 2027 544f  .  toaOrSR = 'TO
+000227b0: 4127 2c0d 0a20 2069 6e63 6c75 6465 534c  A',..  includeSL
+000227c0: 434f 6666 4c37 203d 2046 616c 7365 2c0d  COffL7 = False,.
+000227d0: 0a20 2064 6566 7269 6e67 654c 3520 3d20  .  defringeL5 = 
+000227e0: 4661 6c73 652c 0d0a 2020 6170 706c 7951  False,..  applyQ
+000227f0: 4142 616e 6420 3d20 4661 6c73 652c 0d0a  ABand = False,..
+00022800: 2020 6170 706c 7943 6c6f 7564 5072 6f62    applyCloudProb
+00022810: 6162 696c 6974 7920 3d20 5472 7565 2c0d  ability = True,.
+00022820: 0a20 2061 7070 6c79 5368 6164 6f77 5368  .  applyShadowSh
+00022830: 6966 7420 3d20 4661 6c73 652c 0d0a 2020  ift = False,..  
+00022840: 6170 706c 7943 6c6f 7564 5363 6f72 654c  applyCloudScoreL
+00022850: 616e 6473 6174 203d 2046 616c 7365 2c0d  andsat = False,.
+00022860: 0a20 2061 7070 6c79 436c 6f75 6453 636f  .  applyCloudSco
+00022870: 7265 5365 6e74 696e 656c 3220 3d20 4661  reSentinel2 = Fa
+00022880: 6c73 652c 0d0a 2020 6170 706c 7954 444f  lse,..  applyTDO
+00022890: 4d4c 616e 6473 6174 203d 2054 7275 652c  MLandsat = True,
+000228a0: 0d0a 2020 6170 706c 7954 444f 4d53 656e  ..  applyTDOMSen
+000228b0: 7469 6e65 6c32 203d 2054 7275 652c 0d0a  tinel2 = True,..
+000228c0: 2020 6170 706c 7946 6d61 736b 436c 6f75    applyFmaskClou
+000228d0: 644d 6173 6b20 3d20 5472 7565 2c0d 0a20  dMask = True,.. 
+000228e0: 2061 7070 6c79 466d 6173 6b43 6c6f 7564   applyFmaskCloud
+000228f0: 5368 6164 6f77 4d61 736b 203d 2054 7275  ShadowMask = Tru
+00022900: 652c 0d0a 2020 6170 706c 7946 6d61 736b  e,..  applyFmask
+00022910: 536e 6f77 4d61 736b 203d 2046 616c 7365  SnowMask = False
+00022920: 2c0d 0a20 2063 6c6f 7564 4865 6967 6874  ,..  cloudHeight
+00022930: 7320 3d20 6565 2e4c 6973 742e 7365 7175  s = ee.List.sequ
+00022940: 656e 6365 2835 3030 2c31 3030 3030 2c35  ence(500,10000,5
+00022950: 3030 292c 0d0a 2020 636c 6f75 6453 636f  00),..  cloudSco
+00022960: 7265 5468 7265 7368 203d 2032 302c 0d0a  reThresh = 20,..
+00022970: 2020 7065 7266 6f72 6d43 6c6f 7564 5363    performCloudSc
+00022980: 6f72 654f 6666 7365 7420 3d20 5472 7565  oreOffset = True
+00022990: 2c0d 0a20 2063 6c6f 7564 5363 6f72 6550  ,..  cloudScoreP
+000229a0: 6374 6c20 3d20 3130 2c0d 0a20 207a 5363  ctl = 10,..  zSc
+000229b0: 6f72 6554 6872 6573 6820 3d20 2d31 2c0d  oreThresh = -1,.
+000229c0: 0a20 2073 6861 646f 7753 756d 5468 7265  .  shadowSumThre
+000229d0: 7368 203d 2030 2e33 352c 0d0a 2020 636f  sh = 0.35,..  co
+000229e0: 6e74 7261 6374 5069 7865 6c73 203d 2031  ntractPixels = 1
+000229f0: 2e35 2c0d 0a20 2064 696c 6174 6550 6978  .5,..  dilatePix
+00022a00: 656c 7320 3d20 332e 352c 0d0a 2020 7368  els = 3.5,..  sh
+00022a10: 6164 6f77 5375 6d42 616e 6473 203d 205b  adowSumBands = [
+00022a20: 276e 6972 272c 2773 7769 7231 275d 2c0d  'nir','swir1'],.
+00022a30: 0a20 206c 616e 6473 6174 5265 7361 6d70  .  landsatResamp
+00022a40: 6c65 4d65 7468 6f64 203d 2027 6e65 6172  leMethod = 'near
+00022a50: 272c 0d0a 2020 7365 6e74 696e 656c 3252  ',..  sentinel2R
+00022a60: 6573 616d 706c 654d 6574 686f 6420 3d20  esampleMethod = 
+00022a70: 2761 6767 7265 6761 7465 272c 0d0a 2020  'aggregate',..  
+00022a80: 636f 6e76 6572 7454 6f44 6169 6c79 4d6f  convertToDailyMo
+00022a90: 7361 6963 7320 3d20 5472 7565 2c0d 0a20  saics = True,.. 
+00022aa0: 2072 756e 4368 6173 7461 696e 4861 726d   runChastainHarm
+00022ab0: 6f6e 697a 6174 696f 6e20 3d20 5472 7565  onization = True
+00022ac0: 2c0d 0a20 2063 6f72 7265 6374 496c 6c75  ,..  correctIllu
+00022ad0: 6d69 6e61 7469 6f6e 203d 2046 616c 7365  mination = False
+00022ae0: 2c0d 0a20 2063 6f72 7265 6374 5363 616c  ,..  correctScal
+00022af0: 6520 3d20 3235 302c 0d0a 2020 6578 706f  e = 250,..  expo
+00022b00: 7274 436f 6d70 6f73 6974 6573 203d 2046  rtComposites = F
+00022b10: 616c 7365 2c0d 0a20 206f 7574 7075 744e  alse,..  outputN
+00022b20: 616d 6520 3d20 274c 616e 6473 6174 2d53  ame = 'Landsat-S
+00022b30: 656e 7469 6e65 6c32 2d48 7962 7269 6427  entinel2-Hybrid'
+00022b40: 2c0d 0a20 2065 7870 6f72 7450 6174 6852  ,..  exportPathR
+00022b50: 6f6f 7420 3d20 4e6f 6e65 2c0d 0a20 2063  oot = None,..  c
+00022b60: 7273 203d 2027 4550 5347 3a35 3037 3027  rs = 'EPSG:5070'
+00022b70: 2c0d 0a20 2074 7261 6e73 666f 726d 203d  ,..  transform =
+00022b80: 205b 3330 2c30 2c2d 3233 3631 3931 352e   [30,0,-2361915.
+00022b90: 302c 302c 2d33 302c 3331 3737 3733 352e  0,0,-30,3177735.
+00022ba0: 305d 2c0d 0a20 2073 6361 6c65 203d 204e  0],..  scale = N
+00022bb0: 6f6e 652c 0d0a 2020 7072 6543 6f6d 7075  one,..  preCompu
+00022bc0: 7465 644c 616e 6473 6174 436c 6f75 6453  tedLandsatCloudS
+00022bd0: 636f 7265 4f66 6673 6574 203d 204e 6f6e  coreOffset = Non
+00022be0: 652c 0d0a 2020 7072 6543 6f6d 7075 7465  e,..  preCompute
+00022bf0: 644c 616e 6473 6174 5444 4f4d 4952 4d65  dLandsatTDOMIRMe
+00022c00: 616e 203d 204e 6f6e 652c 0d0a 2020 7072  an = None,..  pr
+00022c10: 6543 6f6d 7075 7465 644c 616e 6473 6174  eComputedLandsat
+00022c20: 5444 4f4d 4952 5374 6444 6576 203d 204e  TDOMIRStdDev = N
+00022c30: 6f6e 652c 0d0a 2020 7072 6543 6f6d 7075  one,..  preCompu
+00022c40: 7465 6453 656e 7469 6e65 6c32 436c 6f75  tedSentinel2Clou
+00022c50: 6453 636f 7265 4f66 6673 6574 203d 204e  dScoreOffset = N
+00022c60: 6f6e 652c 0d0a 2020 7072 6543 6f6d 7075  one,..  preCompu
+00022c70: 7465 6453 656e 7469 6e65 6c32 5444 4f4d  tedSentinel2TDOM
+00022c80: 4952 4d65 616e 203d 204e 6f6e 652c 0d0a  IRMean = None,..
+00022c90: 2020 7072 6543 6f6d 7075 7465 6453 656e    preComputedSen
+00022ca0: 7469 6e65 6c32 5444 4f4d 4952 5374 6444  tinel2TDOMIRStdD
+00022cb0: 6576 203d 204e 6f6e 652c 0d0a 2020 636c  ev = None,..  cl
+00022cc0: 6f75 6450 726f 6254 6872 6573 6820 3d20  oudProbThresh = 
+00022cd0: 3430 2c0d 0a20 206c 616e 6473 6174 436f  40,..  landsatCo
+00022ce0: 6c6c 6563 7469 6f6e 5665 7273 696f 6e20  llectionVersion 
+00022cf0: 3d20 2743 3227 2c0d 0a20 206f 7665 7277  = 'C2',..  overw
+00022d00: 7269 7465 203d 2046 616c 7365 293a 0d0a  rite = False):..
+00022d10: 0d0a 2020 6f72 6967 696e 203d 2027 4c61  ..  origin = 'La
+00022d20: 6e64 7361 742d 5365 6e74 696e 656c 322d  ndsat-Sentinel2-
+00022d30: 4879 6272 6964 270d 0a20 2074 6f61 4f72  Hybrid'..  toaOr
+00022d40: 5352 203d 2074 6f61 4f72 5352 2e75 7070  SR = toaOrSR.upp
+00022d50: 6572 2829 0d0a 0d0a 2020 6172 6773 203d  er()....  args =
+00022d60: 2066 6f72 6d61 7441 7267 7328 6c6f 6361   formatArgs(loca
+00022d70: 6c73 2829 290d 0a20 2069 6620 2761 7267  ls())..  if 'arg
+00022d80: 7327 2069 6e20 6172 6773 2e6b 6579 7328  s' in args.keys(
+00022d90: 293a 0d0a 2020 2020 6465 6c20 6172 6773  ):..    del args
+00022da0: 5b27 6172 6773 275d 0d0a 0d0a 2020 6d65  ['args']....  me
+00022db0: 7267 6564 203d 2067 6574 5072 6f63 6573  rged = getProces
+00022dc0: 7365 644c 616e 6473 6174 416e 6453 656e  sedLandsatAndSen
+00022dd0: 7469 6e65 6c32 5363 656e 6573 285c 0d0a  tinel2Scenes(\..
+00022de0: 2020 2020 7374 7564 7941 7265 6120 3d20      studyArea = 
+00022df0: 7374 7564 7941 7265 612c 0d0a 2020 2020  studyArea,..    
+00022e00: 7374 6172 7459 6561 7220 3d20 7374 6172  startYear = star
+00022e10: 7459 6561 722c 0d0a 2020 2020 656e 6459  tYear,..    endY
+00022e20: 6561 7220 3d20 656e 6459 6561 722c 0d0a  ear = endYear,..
+00022e30: 2020 2020 7374 6172 744a 756c 6961 6e20      startJulian 
+00022e40: 3d20 7374 6172 744a 756c 6961 6e2c 0d0a  = startJulian,..
+00022e50: 2020 2020 656e 644a 756c 6961 6e20 3d20      endJulian = 
+00022e60: 656e 644a 756c 6961 6e2c 0d0a 2020 2020  endJulian,..    
+00022e70: 746f 614f 7253 5220 3d20 746f 614f 7253  toaOrSR = toaOrS
+00022e80: 522c 0d0a 2020 2020 696e 636c 7564 6553  R,..    includeS
+00022e90: 4c43 4f66 664c 3720 3d20 696e 636c 7564  LCOffL7 = includ
+00022ea0: 6553 4c43 4f66 664c 372c 0d0a 2020 2020  eSLCOffL7,..    
+00022eb0: 6465 6672 696e 6765 4c35 203d 2064 6566  defringeL5 = def
+00022ec0: 7269 6e67 654c 352c 0d0a 2020 2020 6170  ringeL5,..    ap
+00022ed0: 706c 7951 4142 616e 6420 3d20 6170 706c  plyQABand = appl
+00022ee0: 7951 4142 616e 642c 0d0a 2020 2020 6170  yQABand,..    ap
+00022ef0: 706c 7943 6c6f 7564 5072 6f62 6162 696c  plyCloudProbabil
+00022f00: 6974 7920 3d20 6170 706c 7943 6c6f 7564  ity = applyCloud
+00022f10: 5072 6f62 6162 696c 6974 792c 0d0a 2020  Probability,..  
+00022f20: 2020 6170 706c 7953 6861 646f 7753 6869    applyShadowShi
+00022f30: 6674 203d 2061 7070 6c79 5368 6164 6f77  ft = applyShadow
+00022f40: 5368 6966 742c 0d0a 2020 2020 6170 706c  Shift,..    appl
+00022f50: 7943 6c6f 7564 5363 6f72 654c 616e 6473  yCloudScoreLands
+00022f60: 6174 203d 2061 7070 6c79 436c 6f75 6453  at = applyCloudS
+00022f70: 636f 7265 4c61 6e64 7361 742c 0d0a 2020  coreLandsat,..  
+00022f80: 2020 6170 706c 7943 6c6f 7564 5363 6f72    applyCloudScor
+00022f90: 6553 656e 7469 6e65 6c32 203d 2061 7070  eSentinel2 = app
+00022fa0: 6c79 436c 6f75 6453 636f 7265 5365 6e74  lyCloudScoreSent
+00022fb0: 696e 656c 322c 0d0a 2020 2020 6170 706c  inel2,..    appl
+00022fc0: 7954 444f 4d4c 616e 6473 6174 203d 2061  yTDOMLandsat = a
+00022fd0: 7070 6c79 5444 4f4d 4c61 6e64 7361 742c  pplyTDOMLandsat,
+00022fe0: 0d0a 2020 2020 6170 706c 7954 444f 4d53  ..    applyTDOMS
+00022ff0: 656e 7469 6e65 6c32 203d 2061 7070 6c79  entinel2 = apply
+00023000: 5444 4f4d 5365 6e74 696e 656c 322c 0d0a  TDOMSentinel2,..
+00023010: 2020 2020 6170 706c 7946 6d61 736b 436c      applyFmaskCl
+00023020: 6f75 644d 6173 6b20 3d20 6170 706c 7946  oudMask = applyF
+00023030: 6d61 736b 436c 6f75 644d 6173 6b2c 0d0a  maskCloudMask,..
+00023040: 2020 2020 6170 706c 7946 6d61 736b 436c      applyFmaskCl
+00023050: 6f75 6453 6861 646f 774d 6173 6b20 3d20  oudShadowMask = 
+00023060: 6170 706c 7946 6d61 736b 436c 6f75 6453  applyFmaskCloudS
+00023070: 6861 646f 774d 6173 6b2c 0d0a 2020 2020  hadowMask,..    
+00023080: 6170 706c 7946 6d61 736b 536e 6f77 4d61  applyFmaskSnowMa
+00023090: 736b 203d 2061 7070 6c79 466d 6173 6b53  sk = applyFmaskS
+000230a0: 6e6f 774d 6173 6b2c 0d0a 2020 2020 636c  nowMask,..    cl
+000230b0: 6f75 6448 6569 6768 7473 203d 2063 6c6f  oudHeights = clo
+000230c0: 7564 4865 6967 6874 732c 0d0a 2020 2020  udHeights,..    
+000230d0: 636c 6f75 6453 636f 7265 5468 7265 7368  cloudScoreThresh
+000230e0: 203d 2063 6c6f 7564 5363 6f72 6554 6872   = cloudScoreThr
+000230f0: 6573 682c 0d0a 2020 2020 7065 7266 6f72  esh,..    perfor
+00023100: 6d43 6c6f 7564 5363 6f72 654f 6666 7365  mCloudScoreOffse
+00023110: 7420 3d20 7065 7266 6f72 6d43 6c6f 7564  t = performCloud
+00023120: 5363 6f72 654f 6666 7365 742c 0d0a 2020  ScoreOffset,..  
+00023130: 2020 636c 6f75 6453 636f 7265 5063 746c    cloudScorePctl
+00023140: 203d 2063 6c6f 7564 5363 6f72 6550 6374   = cloudScorePct
+00023150: 6c2c 0d0a 2020 2020 7a53 636f 7265 5468  l,..    zScoreTh
+00023160: 7265 7368 203d 207a 5363 6f72 6554 6872  resh = zScoreThr
+00023170: 6573 682c 0d0a 2020 2020 7368 6164 6f77  esh,..    shadow
+00023180: 5375 6d54 6872 6573 6820 3d20 7368 6164  SumThresh = shad
+00023190: 6f77 5375 6d54 6872 6573 682c 0d0a 2020  owSumThresh,..  
+000231a0: 2020 636f 6e74 7261 6374 5069 7865 6c73    contractPixels
+000231b0: 203d 2063 6f6e 7472 6163 7450 6978 656c   = contractPixel
+000231c0: 732c 0d0a 2020 2020 6469 6c61 7465 5069  s,..    dilatePi
+000231d0: 7865 6c73 203d 2064 696c 6174 6550 6978  xels = dilatePix
+000231e0: 656c 732c 0d0a 2020 2020 7368 6164 6f77  els,..    shadow
+000231f0: 5375 6d42 616e 6473 203d 2073 6861 646f  SumBands = shado
+00023200: 7753 756d 4261 6e64 732c 0d0a 2020 2020  wSumBands,..    
+00023210: 6c61 6e64 7361 7452 6573 616d 706c 654d  landsatResampleM
+00023220: 6574 686f 6420 3d20 6c61 6e64 7361 7452  ethod = landsatR
+00023230: 6573 616d 706c 654d 6574 686f 642c 0d0a  esampleMethod,..
+00023240: 2020 2020 7365 6e74 696e 656c 3252 6573      sentinel2Res
+00023250: 616d 706c 654d 6574 686f 6420 3d20 7365  ampleMethod = se
+00023260: 6e74 696e 656c 3252 6573 616d 706c 654d  ntinel2ResampleM
+00023270: 6574 686f 642c 0d0a 2020 2020 636f 6e76  ethod,..    conv
+00023280: 6572 7454 6f44 6169 6c79 4d6f 7361 6963  ertToDailyMosaic
+00023290: 7320 3d20 636f 6e76 6572 7454 6f44 6169  s = convertToDai
+000232a0: 6c79 4d6f 7361 6963 732c 0d0a 2020 2020  lyMosaics,..    
+000232b0: 7275 6e43 6861 7374 6169 6e48 6172 6d6f  runChastainHarmo
+000232c0: 6e69 7a61 7469 6f6e 203d 2072 756e 4368  nization = runCh
+000232d0: 6173 7461 696e 4861 726d 6f6e 697a 6174  astainHarmonizat
+000232e0: 696f 6e2c 0d0a 2020 2020 636f 7272 6563  ion,..    correc
+000232f0: 7449 6c6c 756d 696e 6174 696f 6e20 3d20  tIllumination = 
+00023300: 636f 7272 6563 7449 6c6c 756d 696e 6174  correctIlluminat
+00023310: 696f 6e2c 0d0a 2020 2020 636f 7272 6563  ion,..    correc
+00023320: 7453 6361 6c65 203d 2063 6f72 7265 6374  tScale = correct
+00023330: 5363 616c 652c 0d0a 2020 2020 7072 6543  Scale,..    preC
+00023340: 6f6d 7075 7465 644c 616e 6473 6174 436c  omputedLandsatCl
+00023350: 6f75 6453 636f 7265 4f66 6673 6574 203d  oudScoreOffset =
+00023360: 2070 7265 436f 6d70 7574 6564 4c61 6e64   preComputedLand
+00023370: 7361 7443 6c6f 7564 5363 6f72 654f 6666  satCloudScoreOff
+00023380: 7365 742c 0d0a 2020 2020 7072 6543 6f6d  set,..    preCom
+00023390: 7075 7465 644c 616e 6473 6174 5444 4f4d  putedLandsatTDOM
+000233a0: 4952 4d65 616e 203d 2070 7265 436f 6d70  IRMean = preComp
+000233b0: 7574 6564 4c61 6e64 7361 7454 444f 4d49  utedLandsatTDOMI
+000233c0: 524d 6561 6e2c 0d0a 2020 2020 7072 6543  RMean,..    preC
+000233d0: 6f6d 7075 7465 644c 616e 6473 6174 5444  omputedLandsatTD
+000233e0: 4f4d 4952 5374 6444 6576 203d 2070 7265  OMIRStdDev = pre
+000233f0: 436f 6d70 7574 6564 4c61 6e64 7361 7454  ComputedLandsatT
+00023400: 444f 4d49 5253 7464 4465 762c 0d0a 2020  DOMIRStdDev,..  
+00023410: 2020 7072 6543 6f6d 7075 7465 6453 656e    preComputedSen
+00023420: 7469 6e65 6c32 436c 6f75 6453 636f 7265  tinel2CloudScore
+00023430: 4f66 6673 6574 203d 2070 7265 436f 6d70  Offset = preComp
+00023440: 7574 6564 5365 6e74 696e 656c 3243 6c6f  utedSentinel2Clo
+00023450: 7564 5363 6f72 654f 6666 7365 742c 0d0a  udScoreOffset,..
+00023460: 2020 2020 7072 6543 6f6d 7075 7465 6453      preComputedS
+00023470: 656e 7469 6e65 6c32 5444 4f4d 4952 4d65  entinel2TDOMIRMe
+00023480: 616e 203d 2070 7265 436f 6d70 7574 6564  an = preComputed
+00023490: 5365 6e74 696e 656c 3254 444f 4d49 524d  Sentinel2TDOMIRM
+000234a0: 6561 6e2c 0d0a 2020 2020 7072 6543 6f6d  ean,..    preCom
+000234b0: 7075 7465 6453 656e 7469 6e65 6c32 5444  putedSentinel2TD
+000234c0: 4f4d 4952 5374 6444 6576 203d 2070 7265  OMIRStdDev = pre
+000234d0: 436f 6d70 7574 6564 5365 6e74 696e 656c  ComputedSentinel
+000234e0: 3254 444f 4d49 5253 7464 4465 762c 0d0a  2TDOMIRStdDev,..
+000234f0: 2020 2020 636c 6f75 6450 726f 6254 6872      cloudProbThr
+00023500: 6573 6820 3d20 636c 6f75 6450 726f 6254  esh = cloudProbT
+00023510: 6872 6573 682c 0d0a 2020 2020 6c61 6e64  hresh,..    land
+00023520: 7361 7443 6f6c 6c65 6374 696f 6e56 6572  satCollectionVer
+00023530: 7369 6f6e 203d 206c 616e 6473 6174 436f  sion = landsatCo
+00023540: 6c6c 6563 7469 6f6e 5665 7273 696f 6e29  llectionVersion)
+00023550: 0d0a 0d0a 2020 2343 7265 6174 6520 6879  ....  #Create hy
+00023560: 6272 6964 2063 6f6d 706f 7369 7465 730d  brid composites.
+00023570: 0a20 2063 6f6d 706f 7369 7465 7320 3d20  .  composites = 
+00023580: 636f 6d70 6f73 6974 6554 696d 6553 6572  compositeTimeSer
+00023590: 6965 7328 5c0d 0a20 2020 206c 7320 3d20  ies(\..    ls = 
+000235a0: 6d65 7267 6564 2c0d 0a20 2020 2073 7461  merged,..    sta
+000235b0: 7274 5965 6172 203d 2073 7461 7274 5965  rtYear = startYe
+000235c0: 6172 2c0d 0a20 2020 2065 6e64 5965 6172  ar,..    endYear
+000235d0: 203d 2065 6e64 5965 6172 2c0d 0a20 2020   = endYear,..   
+000235e0: 2073 7461 7274 4a75 6c69 616e 203d 2073   startJulian = s
+000235f0: 7461 7274 4a75 6c69 616e 2c0d 0a20 2020  tartJulian,..   
+00023600: 2065 6e64 4a75 6c69 616e 203d 2065 6e64   endJulian = end
+00023610: 4a75 6c69 616e 2c0d 0a20 2020 2074 696d  Julian,..    tim
+00023620: 6562 7566 6665 7220 3d20 7469 6d65 6275  ebuffer = timebu
+00023630: 6666 6572 2c0d 0a20 2020 2077 6569 6768  ffer,..    weigh
+00023640: 7473 203d 2077 6569 6768 7473 2c0d 0a20  ts = weights,.. 
+00023650: 2020 2063 6f6d 706f 7369 7469 6e67 4d65     compositingMe
+00023660: 7468 6f64 203d 2063 6f6d 706f 7369 7469  thod = compositi
+00023670: 6e67 4d65 7468 6f64 290d 0a0d 0a20 2023  ngMethod)....  #
+00023680: 2045 7870 6f72 7420 636f 6d70 6f73 6974   Export composit
+00023690: 6520 636f 6c6c 6563 7469 6f6e 0d0a 2020  e collection..  
+000236a0: 6966 2065 7870 6f72 7443 6f6d 706f 7369  if exportComposi
+000236b0: 7465 733a 0d0a 0d0a 2020 2020 6578 706f  tes:....    expo
+000236c0: 7274 4261 6e64 4469 6374 203d 207b 5c0d  rtBandDict = {\.
+000236d0: 0a20 2020 2020 2027 6d65 646f 6964 273a  .      'medoid':
+000236e0: 5b27 626c 7565 272c 2027 6772 6565 6e27  ['blue', 'green'
+000236f0: 2c20 2772 6564 272c 276e 6972 272c 2773  , 'red','nir','s
+00023700: 7769 7231 272c 2027 7377 6972 3227 2c27  wir1', 'swir2','
+00023710: 636f 6d70 6f73 6974 654f 6273 436f 756e  compositeObsCoun
+00023720: 7427 2c27 7365 6e73 6f72 272c 2779 6561  t','sensor','yea
+00023730: 7227 2c27 6a75 6c69 616e 4461 7927 5d2c  r','julianDay'],
+00023740: 0d0a 2020 2020 2020 276d 6564 6961 6e27  ..      'median'
+00023750: 3a5b 2762 6c75 6527 2c20 2767 7265 656e  :['blue', 'green
+00023760: 272c 2027 7265 6427 2c27 6e69 7227 2c27  ', 'red','nir','
+00023770: 7377 6972 3127 2c20 2773 7769 7232 272c  swir1', 'swir2',
+00023780: 2763 6f6d 706f 7369 7465 4f62 7343 6f75  'compositeObsCou
+00023790: 6e74 275d 5c0d 0a20 2020 207d 3b0d 0a20  nt']\..    };.. 
+000237a0: 2020 206e 6f6e 4469 7669 6465 4261 6e64     nonDivideBand
+000237b0: 4469 6374 203d 207b 5c0d 0a20 2020 2020  Dict = {\..     
+000237c0: 2027 6d65 646f 6964 273a 5b27 636f 6d70   'medoid':['comp
+000237d0: 6f73 6974 654f 6273 436f 756e 7427 2c27  ositeObsCount','
+000237e0: 7365 6e73 6f72 272c 2779 6561 7227 2c27  sensor','year','
+000237f0: 6a75 6c69 616e 4461 7927 5d2c 0d0a 2020  julianDay'],..  
+00023800: 2020 2020 276d 6564 6961 6e27 3a5b 2763      'median':['c
+00023810: 6f6d 706f 7369 7465 4f62 7343 6f75 6e74  ompositeObsCount
+00023820: 275d 5c0d 0a20 2020 207d 3b0d 0a20 2020  ']\..    };..   
+00023830: 2065 7870 6f72 7442 616e 6473 203d 2065   exportBands = e
+00023840: 7870 6f72 7442 616e 6444 6963 745b 636f  xportBandDict[co
+00023850: 6d70 6f73 6974 696e 674d 6574 686f 645d  mpositingMethod]
+00023860: 0d0a 2020 2020 6e6f 6e44 6976 6964 6542  ..    nonDivideB
+00023870: 616e 6473 203d 206e 6f6e 4469 7669 6465  ands = nonDivide
+00023880: 4261 6e64 4469 6374 5b63 6f6d 706f 7369  BandDict[composi
+00023890: 7469 6e67 4d65 7468 6f64 5d0d 0a0d 0a20  tingMethod].... 
+000238a0: 2020 2065 7870 6f72 7443 6f6d 706f 7369     exportComposi
+000238b0: 7465 436f 6c6c 6563 7469 6f6e 285c 0d0a  teCollection(\..
+000238c0: 2020 2020 2020 636f 6c6c 6563 7469 6f6e        collection
+000238d0: 203d 2063 6f6d 706f 7369 7465 732c 0d0a   = composites,..
+000238e0: 2020 2020 2020 6578 706f 7274 5061 7468        exportPath
+000238f0: 526f 6f74 203d 2065 7870 6f72 7450 6174  Root = exportPat
+00023900: 6852 6f6f 742c 0d0a 2020 2020 2020 6f75  hRoot,..      ou
+00023910: 7470 7574 4e61 6d65 203d 206f 7574 7075  tputName = outpu
+00023920: 744e 616d 652c 0d0a 2020 2020 2020 6f72  tName,..      or
+00023930: 6967 696e 203d 206f 7269 6769 6e2c 0d0a  igin = origin,..
+00023940: 2020 2020 2020 7374 7564 7941 7265 6120        studyArea 
+00023950: 3d20 7374 7564 7941 7265 612c 0d0a 2020  = studyArea,..  
+00023960: 2020 2020 6372 7320 3d20 6372 732c 0d0a      crs = crs,..
+00023970: 2020 2020 2020 7472 616e 7366 6f72 6d20        transform 
+00023980: 3d20 7472 616e 7366 6f72 6d2c 0d0a 2020  = transform,..  
+00023990: 2020 2020 7363 616c 6520 3d20 7363 616c      scale = scal
+000239a0: 652c 0d0a 2020 2020 2020 7374 6172 7459  e,..      startY
+000239b0: 6561 7220 3d20 7374 6172 7459 6561 722c  ear = startYear,
+000239c0: 0d0a 2020 2020 2020 656e 6459 6561 7220  ..      endYear 
+000239d0: 3d20 656e 6459 6561 722c 0d0a 2020 2020  = endYear,..    
+000239e0: 2020 7374 6172 744a 756c 6961 6e20 3d20    startJulian = 
+000239f0: 7374 6172 744a 756c 6961 6e2c 0d0a 2020  startJulian,..  
+00023a00: 2020 2020 656e 644a 756c 6961 6e20 3d20      endJulian = 
+00023a10: 656e 644a 756c 6961 6e2c 0d0a 2020 2020  endJulian,..    
+00023a20: 2020 636f 6d70 6f73 6974 696e 674d 6574    compositingMet
+00023a30: 686f 6420 3d20 636f 6d70 6f73 6974 696e  hod = compositin
+00023a40: 674d 6574 686f 642c 0d0a 2020 2020 2020  gMethod,..      
+00023a50: 7469 6d65 6275 6666 6572 203d 2074 696d  timebuffer = tim
+00023a60: 6562 7566 6665 722c 0d0a 2020 2020 2020  ebuffer,..      
+00023a70: 746f 614f 7253 5220 3d20 746f 614f 7253  toaOrSR = toaOrS
+00023a80: 522c 0d0a 2020 2020 2020 6e6f 6e44 6976  R,..      nonDiv
+00023a90: 6964 6542 616e 6473 203d 206e 6f6e 4469  ideBands = nonDi
+00023aa0: 7669 6465 4261 6e64 732c 0d0a 2020 2020  videBands,..    
+00023ab0: 2020 6578 706f 7274 4261 6e64 7320 3d20    exportBands = 
+00023ac0: 6578 706f 7274 4261 6e64 732c 0d0a 2020  exportBands,..  
+00023ad0: 2020 2020 6164 6469 7469 6f6e 616c 5072      additionalPr
+00023ae0: 6f70 6572 7479 4469 6374 203d 2061 7267  opertyDict = arg
+00023af0: 732c 0d0a 2020 2020 2020 6f76 6572 7772  s,..      overwr
+00023b00: 6974 6520 3d20 6f76 6572 7772 6974 6529  ite = overwrite)
+00023b10: 0d0a 0d0a 2020 6172 6773 5b27 7072 6f63  ....  args['proc
+00023b20: 6573 7365 6453 6365 6e65 7327 5d20 3d20  essedScenes'] = 
+00023b30: 6d65 7267 6564 0d0a 2020 6172 6773 5b27  merged..  args['
+00023b40: 7072 6f63 6573 7365 6443 6f6d 706f 7369  processedComposi
+00023b50: 7465 7327 5d20 3d20 636f 6d70 6f73 6974  tes'] = composit
+00023b60: 6573 0d0a 0d0a 2020 7265 7475 726e 2061  es....  return a
+00023b70: 7267 730d 0a0d 0a23 2323 2323 2323 2323  rgs....#########
+00023b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00023b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00023ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00023bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023bc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023bd0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00023bc0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00023bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00023be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00023bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c10: 2323 2323 2323 2323 2323 230d 0a23 4675  ###########..#Fu
-00023c20: 6e63 7469 6f6e 2074 6f20 6769 7665 2079  nction to give y
-00023c30: 6561 722e 6464 2069 6d61 6765 2061 6e64  ear.dd image and
-00023c40: 2068 6172 6d6f 6e69 6373 206c 6973 7420   harmonics list 
-00023c50: 2865 2e67 2e20 5b31 2c32 2c33 2c2e 2e2e  (e.g. [1,2,3,...
-00023c60: 5d29 0d0a 6465 6620 6765 7448 6172 6d6f  ])..def getHarmo
-00023c70: 6e69 634c 6973 7428 7965 6172 4461 7465  nicList(yearDate
-00023c80: 496d 672c 7472 616e 7366 6f72 6d42 616e  Img,transformBan
-00023c90: 644e 616d 652c 6861 726d 6f6e 6963 4c69  dName,harmonicLi
-00023ca0: 7374 293a 0d0a 2020 743d 2079 6561 7244  st):..  t= yearD
-00023cb0: 6174 6549 6d67 2e73 656c 6563 7428 5b74  ateImg.select([t
-00023cc0: 7261 6e73 666f 726d 4261 6e64 4e61 6d65  ransformBandName
-00023cd0: 5d29 0d0a 2020 7365 6c65 6374 4261 6e64  ])..  selectBand
-00023ce0: 7320 3d20 6565 2e4c 6973 742e 7365 7175  s = ee.List.sequ
-00023cf0: 656e 6365 2830 2c6c 656e 2868 6172 6d6f  ence(0,len(harmo
-00023d00: 6e69 634c 6973 7429 2d31 290d 0a0d 0a20  nicList)-1).... 
-00023d10: 2064 6566 2073 696e 4361 7428 6829 3a0d   def sinCat(h):.
-00023d20: 0a20 2020 2068 7420 3d20 682a 3130 300d  .    ht = h*100.
-00023d30: 0a20 2020 2072 6574 7572 6e20 6565 2e53  .    return ee.S
-00023d40: 7472 696e 6728 2773 696e 5f27 292e 6361  tring('sin_').ca
-00023d50: 7428 7374 7228 6874 2929 2e63 6174 2827  t(str(ht)).cat('
-00023d60: 5f27 292e 6361 7428 7472 616e 7366 6f72  _').cat(transfor
-00023d70: 6d42 616e 644e 616d 6529 0d0a 2020 7369  mBandName)..  si
-00023d80: 6e4e 616d 6573 203d 206c 6973 7428 6d61  nNames = list(ma
-00023d90: 7028 6c61 6d62 6461 2069 3a73 696e 4361  p(lambda i:sinCa
-00023da0: 7428 6929 2c68 6172 6d6f 6e69 634c 6973  t(i),harmonicLis
-00023db0: 7429 290d 0a0d 0a20 2064 6566 2063 6f73  t))....  def cos
-00023dc0: 4361 7428 6829 3a0d 0a20 2020 2068 7420  Cat(h):..    ht 
-00023dd0: 3d68 2a31 3030 3b0d 0a20 2020 2072 6574  =h*100;..    ret
-00023de0: 7572 6e20 6565 2e53 7472 696e 6728 2763  urn ee.String('c
-00023df0: 6f73 5f27 292e 6361 7428 7374 7228 6874  os_').cat(str(ht
-00023e00: 2929 2e63 6174 2827 5f27 292e 6361 7428  )).cat('_').cat(
-00023e10: 7472 616e 7366 6f72 6d42 616e 644e 616d  transformBandNam
-00023e20: 6529 0d0a 0d0a 2020 636f 734e 616d 6573  e)....  cosNames
-00023e30: 203d 206c 6973 7428 6d61 7028 6c61 6d62   = list(map(lamb
-00023e40: 6461 2069 203a 2063 6f73 4361 7428 6929  da i : cosCat(i)
-00023e50: 2c68 6172 6d6f 6e69 634c 6973 7429 290d  ,harmonicList)).
-00023e60: 0a0d 0a0d 0a0d 0a20 206d 756c 7469 706c  .......  multipl
-00023e70: 6965 7273 203d 2065 652e 496d 6167 6528  iers = ee.Image(
-00023e80: 6861 726d 6f6e 6963 4c69 7374 292e 6d75  harmonicList).mu
-00023e90: 6c74 6970 6c79 2865 652e 4e75 6d62 6572  ltiply(ee.Number
-00023ea0: 286d 6174 682e 7069 292e 666c 6f61 7428  (math.pi).float(
-00023eb0: 2929 0d0a 2020 7369 6e49 6e64 203d 2028  ))..  sinInd = (
-00023ec0: 742e 6d75 6c74 6970 6c79 2865 652e 496d  t.multiply(ee.Im
-00023ed0: 6167 6528 6d75 6c74 6970 6c69 6572 7329  age(multipliers)
-00023ee0: 2929 2e73 696e 2829 2e73 656c 6563 7428  )).sin().select(
-00023ef0: 7365 6c65 6374 4261 6e64 732c 7369 6e4e  selectBands,sinN
-00023f00: 616d 6573 292e 666c 6f61 7428 290d 0a20  ames).float().. 
-00023f10: 2063 6f73 496e 6420 3d20 2874 2e6d 756c   cosInd = (t.mul
-00023f20: 7469 706c 7928 6565 2e49 6d61 6765 286d  tiply(ee.Image(m
-00023f30: 756c 7469 706c 6965 7273 2929 292e 636f  ultipliers))).co
-00023f40: 7328 292e 7365 6c65 6374 2873 656c 6563  s().select(selec
-00023f50: 7442 616e 6473 2c63 6f73 4e61 6d65 7329  tBands,cosNames)
-00023f60: 2e66 6c6f 6174 2829 0d0a 0d0a 2020 7265  .float()....  re
-00023f70: 7475 726e 2079 6561 7244 6174 6549 6d67  turn yearDateImg
-00023f80: 2e61 6464 4261 6e64 7328 7369 6e49 6e64  .addBands(sinInd
-00023f90: 2e61 6464 4261 6e64 7328 636f 7349 6e64  .addBands(cosInd
-00023fa0: 2929 0d0a 0d0a 2323 2323 2323 2323 2323  ))....##########
-00023fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023fe0: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-00023ff0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-00024000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024030: 2323 2323 2323 2323 2323 0d0a 2354 616b  ##########..#Tak
-00024040: 6573 2061 2064 6570 656e 6465 6e74 2061  es a dependent a
-00024050: 6e64 2069 6e64 6570 656e 6465 6e74 2076  nd independent v
-00024060: 6172 6961 626c 6520 616e 6420 7265 7475  ariable and retu
-00024070: 726e 7320 7468 6520 6465 7065 6e64 656e  rns the dependen
-00024080: 742c 0d0a 2320 7369 6e20 6f66 2069 6e64  t,..# sin of ind
-00024090: 2c20 616e 6420 636f 7320 6f66 2069 6e64  , and cos of ind
-000240a0: 0d0a 2349 6e74 656e 6465 6420 666f 7220  ..#Intended for 
-000240b0: 6861 726d 6f6e 6963 2072 6567 7265 7373  harmonic regress
-000240c0: 696f 6e0d 0a64 6566 2067 6574 4861 726d  ion..def getHarm
-000240d0: 6f6e 6963 7332 2863 6f6c 6c65 6374 696f  onics2(collectio
-000240e0: 6e2c 7472 616e 7366 6f72 6d42 616e 644e  n,transformBandN
-000240f0: 616d 652c 6861 726d 6f6e 6963 4c69 7374  ame,harmonicList
-00024100: 2c64 6574 7265 6e64 203d 2046 616c 7365  ,detrend = False
-00024110: 293a 0d0a 0d0a 2020 6465 7042 616e 644e  ):....  depBandN
-00024120: 616d 6573 203d 2065 652e 496d 6167 6528  ames = ee.Image(
-00024130: 636f 6c6c 6563 7469 6f6e 2e66 6972 7374  collection.first
-00024140: 2829 292e 6261 6e64 4e61 6d65 7328 292e  ()).bandNames().
-00024150: 7265 6d6f 7665 2874 7261 6e73 666f 726d  remove(transform
-00024160: 4261 6e64 4e61 6d65 290d 0a20 2064 6570  BandName)..  dep
-00024170: 4261 6e64 4e75 6d62 6572 7320 3d20 6465  BandNumbers = de
-00024180: 7042 616e 644e 616d 6573 2e6d 6170 286c  pBandNames.map(l
-00024190: 616d 6264 6120 6462 6e3a 6465 7042 616e  ambda dbn:depBan
-000241a0: 644e 616d 6573 2e69 6e64 6578 4f66 2864  dNames.indexOf(d
-000241b0: 626e 2929 0d0a 0d0a 2020 6465 6620 6861  bn))....  def ha
-000241c0: 726d 5772 6170 2869 6d67 293a 0d0a 2020  rmWrap(img):..  
-000241d0: 2020 6f75 7454 203d 2067 6574 4861 726d    outT = getHarm
-000241e0: 6f6e 6963 4c69 7374 2869 6d67 2c74 7261  onicList(img,tra
-000241f0: 6e73 666f 726d 4261 6e64 4e61 6d65 2c68  nsformBandName,h
-00024200: 6172 6d6f 6e69 634c 6973 7429 5c0d 0a20  armonicList)\.. 
-00024210: 2020 202e 636f 7079 5072 6f70 6572 7469     .copyProperti
-00024220: 6573 2869 6d67 2c5b 2773 7973 7465 6d3a  es(img,['system:
-00024230: 7469 6d65 5f73 7461 7274 272c 2773 7973  time_start','sys
-00024240: 7465 6d3a 7469 6d65 5f65 6e64 275d 290d  tem:time_end']).
-00024250: 0a20 2020 2072 6574 7572 6e20 6f75 7454  .    return outT
-00024260: 0d0a 2020 6f75 7420 3d20 636f 6c6c 6563  ..  out = collec
-00024270: 7469 6f6e 2e6d 6170 2868 6172 6d57 7261  tion.map(harmWra
-00024280: 7029 0d0a 0d0a 2020 6966 206e 6f74 2064  p)....  if not d
-00024290: 6574 7265 6e64 3a0d 0a20 2020 206f 7574  etrend:..    out
-000242a0: 4261 6e64 4e61 6d65 7320 3d20 6565 2e49  BandNames = ee.I
-000242b0: 6d61 6765 286f 7574 2e66 6972 7374 2829  mage(out.first()
-000242c0: 292e 6261 6e64 4e61 6d65 7328 292e 7265  ).bandNames().re
-000242d0: 6d6f 7665 416c 6c28 5b27 7965 6172 275d  moveAll(['year']
-000242e0: 290d 0a20 2020 206f 7574 203d 206f 7574  )..    out = out
-000242f0: 2e73 656c 6563 7428 6f75 7442 616e 644e  .select(outBandN
-00024300: 616d 6573 290d 0a0d 0a0d 0a20 2069 6e64  ames)......  ind
-00024310: 4261 6e64 4e61 6d65 7320 3d20 6565 2e49  BandNames = ee.I
-00024320: 6d61 6765 286f 7574 2e66 6972 7374 2829  mage(out.first()
-00024330: 292e 6261 6e64 4e61 6d65 7328 292e 7265  ).bandNames().re
-00024340: 6d6f 7665 416c 6c28 6465 7042 616e 644e  moveAll(depBandN
-00024350: 616d 6573 290d 0a20 2069 6e64 4261 6e64  ames)..  indBand
-00024360: 4e75 6d62 6572 7320 3d20 696e 6442 616e  Numbers = indBan
-00024370: 644e 616d 6573 2e6d 6170 286c 616d 6264  dNames.map(lambd
-00024380: 6120 696e 643a 2065 652e 496d 6167 6528  a ind: ee.Image(
-00024390: 6f75 742e 6669 7273 7428 2929 2e62 616e  out.first()).ban
-000243a0: 644e 616d 6573 2829 2e69 6e64 6578 4f66  dNames().indexOf
-000243b0: 2869 6e64 2929 0d0a 0d0a 0d0a 2020 6f75  (ind))......  ou
-000243c0: 7420 3d20 6f75 742e 7365 7428 7b27 696e  t = out.set({'in
-000243d0: 6442 616e 644e 616d 6573 273a 696e 6442  dBandNames':indB
-000243e0: 616e 644e 616d 6573 2c27 6465 7042 616e  andNames,'depBan
-000243f0: 644e 616d 6573 273a 6465 7042 616e 644e  dNames':depBandN
-00024400: 616d 6573 2c5c 0d0a 2020 2020 2020 2020  ames,\..        
-00024410: 2020 2020 2020 2020 2769 6e64 4261 6e64          'indBand
-00024420: 4e75 6d62 6572 7327 3a69 6e64 4261 6e64  Numbers':indBand
-00024430: 4e75 6d62 6572 732c 2764 6570 4261 6e64  Numbers,'depBand
-00024440: 4e75 6d62 6572 7327 3a64 6570 4261 6e64  Numbers':depBand
-00024450: 4e75 6d62 6572 737d 290d 0a0d 0a20 2072  Numbers})....  r
-00024460: 6574 7572 6e20 6f75 740d 0a0d 0a23 2323  eturn out....###
-00024470: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024480: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024490: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000244a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000244b0: 2323 2323 2323 0d0a 2323 2323 2323 2323  ######..########
-000244c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000244d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000244e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000244f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024500: 230d 0a23 5369 6d70 6c69 6669 6573 2074  #..#Simplifies t
-00024510: 6865 2075 7365 206f 6620 7468 6520 726f  he use of the ro
-00024520: 6275 7374 206c 696e 6561 7220 7265 6772  bust linear regr
-00024530: 6573 7369 6f6e 2072 6564 7563 6572 0d0a  ession reducer..
-00024540: 2341 7373 756d 6573 2074 6865 2064 6570  #Assumes the dep
-00024550: 656e 6465 6e74 2069 7320 7468 6520 6669  endent is the fi
-00024560: 7273 7420 6261 6e64 2061 6e64 2061 6c6c  rst band and all
-00024570: 2073 7562 7365 7175 656e 7420 6261 6e64   subsequent band
-00024580: 7320 6172 6520 696e 6465 7065 6e64 656e  s are independen
-00024590: 7473 0d0a 6465 6620 6e65 7752 6f62 7573  ts..def newRobus
-000245a0: 744d 756c 7469 706c 654c 696e 6561 7232  tMultipleLinear2
-000245b0: 2864 6570 656e 6465 6e74 7349 6e64 6570  (dependentsIndep
-000245c0: 656e 6465 6e74 7329 3a0d 0a20 2023 5365  endents):..  #Se
-000245d0: 7420 7570 2074 6865 2062 616e 6420 6e61  t up the band na
-000245e0: 6d65 730d 0a0d 0a20 2064 6570 656e 6465  mes....  depende
-000245f0: 6e74 4261 6e64 7320 3d20 6565 2e4c 6973  ntBands = ee.Lis
-00024600: 7428 6465 7065 6e64 656e 7473 496e 6465  t(dependentsInde
-00024610: 7065 6e64 656e 7473 2e67 6574 2827 6465  pendents.get('de
-00024620: 7042 616e 644e 756d 6265 7273 2729 290d  pBandNumbers')).
-00024630: 0a20 2069 6e64 6570 656e 6465 6e74 4261  .  independentBa
-00024640: 6e64 7320 3d20 6565 2e4c 6973 7428 6465  nds = ee.List(de
-00024650: 7065 6e64 656e 7473 496e 6465 7065 6e64  pendentsIndepend
-00024660: 656e 7473 2e67 6574 2827 696e 6442 616e  ents.get('indBan
-00024670: 644e 756d 6265 7273 2729 290d 0a20 2062  dNumbers'))..  b
-00024680: 6e73 203d 2065 652e 496d 6167 6528 6465  ns = ee.Image(de
-00024690: 7065 6e64 656e 7473 496e 6465 7065 6e64  pendentsIndepend
-000246a0: 656e 7473 2e66 6972 7374 2829 292e 6261  ents.first()).ba
-000246b0: 6e64 4e61 6d65 7328 290d 0a20 2064 6570  ndNames()..  dep
-000246c0: 656e 6465 6e74 7320 3d20 6565 2e4c 6973  endents = ee.Lis
-000246d0: 7428 6465 7065 6e64 656e 7473 496e 6465  t(dependentsInde
-000246e0: 7065 6e64 656e 7473 2e67 6574 2827 6465  pendents.get('de
-000246f0: 7042 616e 644e 616d 6573 2729 290d 0a20  pBandNames')).. 
-00024700: 2069 6e64 6570 656e 6465 6e74 7320 3d20   independents = 
-00024710: 6565 2e4c 6973 7428 6465 7065 6e64 656e  ee.List(dependen
-00024720: 7473 496e 6465 7065 6e64 656e 7473 2e67  tsIndependents.g
-00024730: 6574 2827 696e 6442 616e 644e 616d 6573  et('indBandNames
-00024740: 2729 290d 0a0d 0a20 2023 6465 7065 6e64  '))....  #depend
-00024750: 656e 7420 3d20 626e 732e 736c 6963 6528  ent = bns.slice(
-00024760: 302c 3129 0d0a 2020 2369 6e64 6570 656e  0,1)..  #indepen
-00024770: 6465 6e74 7320 3d20 626e 732e 736c 6963  dents = bns.slic
-00024780: 6528 312c 6e75 6c6c 290d 0a20 206e 6f49  e(1,null)..  noI
-00024790: 6e64 6570 656e 6465 6e74 7320 3d20 696e  ndependents = in
-000247a0: 6465 7065 6e64 656e 7473 2e6c 656e 6774  dependents.lengt
-000247b0: 6828 292e 6164 6428 3129 0d0a 2020 6e6f  h().add(1)..  no
-000247c0: 4465 7065 6e64 656e 7473 203d 2064 6570  Dependents = dep
-000247d0: 656e 6465 6e74 732e 6c65 6e67 7468 2829  endents.length()
-000247e0: 0d0a 0d0a 2020 6f75 744e 616d 6573 203d  ....  outNames =
-000247f0: 2065 652e 4c69 7374 285b 2769 6e74 6572   ee.List(['inter
-00024800: 6365 7074 275d 292e 6361 7428 696e 6465  cept']).cat(inde
-00024810: 7065 6e64 656e 7473 290d 0a0d 0a20 2023  pendents)....  #
-00024820: 4164 6420 636f 6e73 7461 6e74 2062 616e  Add constant ban
-00024830: 6420 666f 7220 696e 7465 7263 6570 7420  d for intercept 
-00024840: 616e 6420 7265 6f72 6465 7220 666f 720d  and reorder for.
-00024850: 0a20 2023 7379 6e74 6178 3a20 636f 6e73  .  #syntax: cons
-00024860: 7461 6e74 2c20 696e 6431 2c69 6e64 322c  tant, ind1,ind2,
-00024870: 696e 6433 2c69 6e64 6e2c 6465 7065 6e64  ind3,indn,depend
-00024880: 656e 740d 0a20 2064 6566 2066 6f72 4669  ent..  def forFi
-00024890: 7446 756e 2869 6d67 293a 0d0a 2020 2020  tFun(img):..    
-000248a0: 6f75 7420 3d20 696d 672e 6164 6442 616e  out = img.addBan
-000248b0: 6473 2865 652e 496d 6167 6528 3129 2e73  ds(ee.Image(1).s
-000248c0: 656c 6563 7428 5b30 5d2c 5b27 636f 6e73  elect([0],['cons
-000248d0: 7461 6e74 275d 2929 0d0a 2020 2020 6f75  tant']))..    ou
-000248e0: 7420 3d20 6f75 742e 7365 6c65 6374 2865  t = out.select(e
-000248f0: 652e 4c69 7374 285b 2763 6f6e 7374 616e  e.List(['constan
-00024900: 7427 2c69 6e64 6570 656e 6465 6e74 735d  t',independents]
-00024910: 292e 666c 6174 7465 6e28 2929 0d0a 2020  ).flatten())..  
-00024920: 2020 7265 7475 726e 206f 7574 2e61 6464    return out.add
-00024930: 4261 6e64 7328 696d 672e 7365 6c65 6374  Bands(img.select
-00024940: 2864 6570 656e 6465 6e74 7329 290d 0a0d  (dependents))...
-00024950: 0a0d 0a20 2066 6f72 4669 7420 3d20 6465  ...  forFit = de
-00024960: 7065 6e64 656e 7473 496e 6465 7065 6e64  pendentsIndepend
-00024970: 656e 7473 2e6d 6170 2866 6f72 4669 7446  ents.map(forFitF
-00024980: 756e 290d 0a0d 0a20 2023 4170 706c 7920  un)....  #Apply 
-00024990: 7265 6475 6365 722c 2061 6e64 2063 6f6e  reducer, and con
-000249a0: 7665 7274 2062 6163 6b20 746f 2069 6d61  vert back to ima
-000249b0: 6765 2077 6974 6820 7265 7370 6563 7469  ge with respecti
-000249c0: 7665 2062 616e 644e 616d 6573 0d0a 2020  ve bandNames..  
-000249d0: 7265 6475 6365 724f 7574 203d 2066 6f72  reducerOut = for
-000249e0: 4669 742e 7265 6475 6365 2865 652e 5265  Fit.reduce(ee.Re
-000249f0: 6475 6365 722e 6c69 6e65 6172 5265 6772  ducer.linearRegr
-00024a00: 6573 7369 6f6e 286e 6f49 6e64 6570 656e  ession(noIndepen
-00024a10: 6465 6e74 732c 6e6f 4465 7065 6e64 656e  dents,noDependen
-00024a20: 7473 2929 0d0a 2020 2320 2f2f 2074 6573  ts))..  # // tes
-00024a30: 7420 3d20 666f 7246 6974 2e72 6564 7563  t = forFit.reduc
-00024a40: 6528 6565 2e52 6564 7563 6572 2e72 6f62  e(ee.Reducer.rob
-00024a50: 7573 744c 696e 6561 7252 6567 7265 7373  ustLinearRegress
-00024a60: 696f 6e28 6e6f 496e 6465 7065 6e64 656e  ion(noIndependen
-00024a70: 7473 2c6e 6f44 6570 656e 6465 6e74 732c  ts,noDependents,
-00024a80: 302e 3229 290d 0a20 2023 202f 2f20 7265  0.2))..  # // re
-00024a90: 7369 6473 203d 2074 6573 740d 0a20 2023  sids = test..  #
-00024aa0: 202f 2f20 2e73 656c 6563 7428 5b31 5d2c   // .select([1],
-00024ab0: 5b27 7265 7369 6475 616c 7327 5d29 2e61  ['residuals']).a
-00024ac0: 7272 6179 466c 6174 7465 6e28 5b64 6570  rrayFlatten([dep
-00024ad0: 656e 6465 6e74 735d 293b 0d0a 2020 2320  endents]);..  # 
-00024ae0: 2f2f 204d 6170 2e61 6464 4c61 7965 7228  // Map.addLayer(
-00024af0: 7265 7369 6473 2c7b 7d2c 2772 6573 6964  resids,{},'resid
-00024b00: 7349 6d61 6765 2729 3b0d 0a20 2023 202f  sImage');..  # /
-00024b10: 2f20 4d61 702e 6164 644c 6179 6572 2872  / Map.addLayer(r
-00024b20: 6564 7563 6572 4f75 742e 7365 6c65 6374  educerOut.select
-00024b30: 285b 305d 292c 7b7d 2c27 636f 6566 6669  ([0]),{},'coeffi
-00024b40: 6369 656e 7473 2729 3b0d 0a20 2023 202f  cients');..  # /
-00024b50: 2f20 4d61 702e 6164 644c 6179 6572 2874  / Map.addLayer(t
-00024b60: 6573 742e 7365 6c65 6374 285b 315d 292c  est.select([1]),
-00024b70: 7b7d 2c27 7472 6573 6964 7561 6c73 2729  {},'tresiduals')
-00024b80: 3b0d 0a20 2023 202f 2f20 4d61 702e 6164  ;..  # // Map.ad
-00024b90: 644c 6179 6572 2872 6564 7563 6572 4f75  dLayer(reducerOu
-00024ba0: 742e 7365 6c65 6374 285b 315d 292c 7b7d  t.select([1]),{}
-00024bb0: 2c27 726f 7265 7369 6475 616c 7327 293b  ,'roresiduals');
-00024bc0: 0d0a 2020 7265 6475 6365 724f 7574 203d  ..  reducerOut =
-00024bd0: 2072 6564 7563 6572 4f75 742e 7365 6c65   reducerOut.sele
-00024be0: 6374 285b 305d 2c5b 2763 6f65 6666 6963  ct([0],['coeffic
-00024bf0: 6965 6e74 7327 5d29 2e61 7272 6179 5472  ients']).arrayTr
-00024c00: 616e 7370 6f73 6528 292e 6172 7261 7946  anspose().arrayF
-00024c10: 6c61 7474 656e 285b 6465 7065 6e64 656e  latten([dependen
-00024c20: 7473 2c6f 7574 4e61 6d65 735d 290d 0a20  ts,outNames]).. 
-00024c30: 2072 6564 7563 6572 4f75 7420 3d20 7265   reducerOut = re
-00024c40: 6475 6365 724f 7574 2e73 6574 287b 276e  ducerOut.set({'n
-00024c50: 6f44 6570 656e 6465 6e74 7327 3a65 652e  oDependents':ee.
-00024c60: 4e75 6d62 6572 286e 6f44 6570 656e 6465  Number(noDepende
-00024c70: 6e74 7329 2c5c 0d0a 2020 276d 6f64 656c  nts),\..  'model
-00024c80: 4c65 6e67 7468 273a 6565 2e4e 756d 6265  Length':ee.Numbe
-00024c90: 7228 6e6f 496e 6465 7065 6e64 656e 7473  r(noIndependents
-00024ca0: 295c 0d0a 2020 7d29 0d0a 0d0a 2020 7265  )\..  })....  re
-00024cb0: 7475 726e 2072 6564 7563 6572 4f75 740d  turn reducerOut.
-00024cc0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-00024cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024d00: 2323 2323 2323 2323 2323 0d0a 2323 2323  ##########..####
-00024d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024d40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024d50: 2323 2323 230d 0a23 436f 6465 2066 6f72  #####..#Code for
-00024d60: 2066 696e 6469 6e67 2074 6865 2064 6174   finding the dat
-00024d70: 6520 6f66 2070 6561 6b20 6f66 2067 7265  e of peak of gre
-00024d80: 656e 0d0a 2320 416c 736f 2063 6f6e 7665  en..# Also conve
-00024d90: 7274 7320 6974 2074 6f20 4a75 6c69 616e  rts it to Julian
-00024da0: 2064 6179 2c20 6d6f 6e74 682c 2061 6e64   day, month, and
-00024db0: 2064 6179 206f 6620 6d6f 6e74 680d 0a6d   day of month..m
-00024dc0: 6f6e 7468 5265 6d61 7020 3d5b 312c 2031  onthRemap =[1, 1
-00024dd0: 2c20 312c 2031 2c20 312c 2031 2c20 312c  , 1, 1, 1, 1, 1,
-00024de0: 2031 2c20 312c 2031 2c20 312c 2031 2c20   1, 1, 1, 1, 1, 
-00024df0: 312c 2031 2c20 312c 2031 2c20 312c 2031  1, 1, 1, 1, 1, 1
-00024e00: 2c20 312c 2031 2c20 312c 2031 2c20 312c  , 1, 1, 1, 1, 1,
-00024e10: 2031 2c20 312c 2031 2c20 312c 2031 2c20   1, 1, 1, 1, 1, 
-00024e20: 312c 2031 2c20 312c 2032 2c20 322c 2032  1, 1, 1, 2, 2, 2
-00024e30: 2c20 322c 2032 2c20 322c 2032 2c20 322c  , 2, 2, 2, 2, 2,
-00024e40: 2032 2c20 322c 2032 2c20 322c 2032 2c20   2, 2, 2, 2, 2, 
-00024e50: 322c 2032 2c20 322c 2032 2c20 322c 2032  2, 2, 2, 2, 2, 2
-00024e60: 2c20 322c 2032 2c20 322c 2032 2c20 322c  , 2, 2, 2, 2, 2,
-00024e70: 2032 2c20 322c 2032 2c20 322c 2033 2c20   2, 2, 2, 2, 3, 
-00024e80: 332c 2033 2c20 332c 2033 2c20 332c 2033  3, 3, 3, 3, 3, 3
-00024e90: 2c20 332c 2033 2c20 332c 2033 2c20 332c  , 3, 3, 3, 3, 3,
-00024ea0: 2033 2c20 332c 2033 2c20 332c 2033 2c20   3, 3, 3, 3, 3, 
-00024eb0: 332c 2033 2c20 332c 2033 2c20 332c 2033  3, 3, 3, 3, 3, 3
-00024ec0: 2c20 332c 2033 2c20 332c 2033 2c20 332c  , 3, 3, 3, 3, 3,
-00024ed0: 2033 2c20 332c 2033 2c20 342c 2034 2c20   3, 3, 3, 4, 4, 
-00024ee0: 342c 2034 2c20 342c 2034 2c20 342c 2034  4, 4, 4, 4, 4, 4
-00024ef0: 2c20 342c 2034 2c20 342c 2034 2c20 342c  , 4, 4, 4, 4, 4,
-00024f00: 2034 2c20 342c 2034 2c20 342c 2034 2c20   4, 4, 4, 4, 4, 
-00024f10: 342c 2034 2c20 342c 2034 2c20 342c 2034  4, 4, 4, 4, 4, 4
-00024f20: 2c20 342c 2034 2c20 342c 2034 2c20 342c  , 4, 4, 4, 4, 4,
-00024f30: 2034 2c20 352c 2035 2c20 352c 2035 2c20   4, 5, 5, 5, 5, 
-00024f40: 352c 2035 2c20 352c 2035 2c20 352c 2035  5, 5, 5, 5, 5, 5
-00024f50: 2c20 352c 2035 2c20 352c 2035 2c20 352c  , 5, 5, 5, 5, 5,
-00024f60: 2035 2c20 352c 2035 2c20 352c 2035 2c20   5, 5, 5, 5, 5, 
-00024f70: 352c 2035 2c20 352c 2035 2c20 352c 2035  5, 5, 5, 5, 5, 5
-00024f80: 2c20 352c 2035 2c20 352c 2035 2c20 352c  , 5, 5, 5, 5, 5,
-00024f90: 2036 2c20 362c 2036 2c20 362c 2036 2c20   6, 6, 6, 6, 6, 
-00024fa0: 362c 2036 2c20 362c 2036 2c20 362c 2036  6, 6, 6, 6, 6, 6
-00024fb0: 2c20 362c 2036 2c20 362c 2036 2c20 362c  , 6, 6, 6, 6, 6,
-00024fc0: 2036 2c20 362c 2036 2c20 362c 2036 2c20   6, 6, 6, 6, 6, 
-00024fd0: 362c 2036 2c20 362c 2036 2c20 362c 2036  6, 6, 6, 6, 6, 6
-00024fe0: 2c20 362c 2036 2c20 362c 2037 2c20 372c  , 6, 6, 6, 7, 7,
-00024ff0: 2037 2c20 372c 2037 2c20 372c 2037 2c20   7, 7, 7, 7, 7, 
-00025000: 372c 2037 2c20 372c 2037 2c20 372c 2037  7, 7, 7, 7, 7, 7
-00025010: 2c20 372c 2037 2c20 372c 2037 2c20 372c  , 7, 7, 7, 7, 7,
-00025020: 2037 2c20 372c 2037 2c20 372c 2037 2c20   7, 7, 7, 7, 7, 
-00025030: 372c 2037 2c20 372c 2037 2c20 372c 2037  7, 7, 7, 7, 7, 7
-00025040: 2c20 372c 2037 2c20 382c 2038 2c20 382c  , 7, 7, 8, 8, 8,
-00025050: 2038 2c20 382c 2038 2c20 382c 2038 2c20   8, 8, 8, 8, 8, 
-00025060: 382c 2038 2c20 382c 2038 2c20 382c 2038  8, 8, 8, 8, 8, 8
-00025070: 2c20 382c 2038 2c20 382c 2038 2c20 382c  , 8, 8, 8, 8, 8,
-00025080: 2038 2c20 382c 2038 2c20 382c 2038 2c20   8, 8, 8, 8, 8, 
-00025090: 382c 2038 2c20 382c 2038 2c20 382c 2038  8, 8, 8, 8, 8, 8
-000250a0: 2c20 382c 2039 2c20 392c 2039 2c20 392c  , 8, 9, 9, 9, 9,
-000250b0: 2039 2c20 392c 2039 2c20 392c 2039 2c20   9, 9, 9, 9, 9, 
-000250c0: 392c 2039 2c20 392c 2039 2c20 392c 2039  9, 9, 9, 9, 9, 9
-000250d0: 2c20 392c 2039 2c20 392c 2039 2c20 392c  , 9, 9, 9, 9, 9,
-000250e0: 2039 2c20 392c 2039 2c20 392c 2039 2c20   9, 9, 9, 9, 9, 
-000250f0: 392c 2039 2c20 392c 2039 2c20 392c 2031  9, 9, 9, 9, 9, 1
-00025100: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025110: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025120: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025130: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025140: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025150: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025160: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
-00025170: 302c 2031 302c 2031 302c 2031 312c 2031  0, 10, 10, 11, 1
-00025180: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-00025190: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-000251a0: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-000251b0: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-000251c0: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-000251d0: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-000251e0: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
-000251f0: 312c 2031 322c 2031 322c 2031 322c 2031  1, 12, 12, 12, 1
-00025200: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-00025210: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-00025220: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-00025230: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-00025240: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-00025250: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
-00025260: 322c 2031 322c 2031 322c 2031 3220 5d0d  2, 12, 12, 12 ].
-00025270: 0a6d 6f6e 7468 4461 7952 656d 6170 203d  .monthDayRemap =
-00025280: 205b 312c 2032 2c20 332c 2034 2c20 352c   [1, 2, 3, 4, 5,
-00025290: 2036 2c20 372c 2038 2c20 392c 2031 302c   6, 7, 8, 9, 10,
-000252a0: 2031 312c 2031 322c 2031 332c 2031 342c   11, 12, 13, 14,
-000252b0: 2031 352c 2031 362c 2031 372c 2031 382c   15, 16, 17, 18,
-000252c0: 2031 392c 2032 302c 2032 312c 2032 322c   19, 20, 21, 22,
-000252d0: 2032 332c 2032 342c 2032 352c 2032 362c   23, 24, 25, 26,
-000252e0: 2032 372c 2032 382c 2032 392c 2033 302c   27, 28, 29, 30,
-000252f0: 2033 312c 2031 2c20 322c 2033 2c20 342c   31, 1, 2, 3, 4,
-00025300: 2035 2c20 362c 2037 2c20 382c 2039 2c20   5, 6, 7, 8, 9, 
-00025310: 3130 2c20 3131 2c20 3132 2c20 3133 2c20  10, 11, 12, 13, 
-00025320: 3134 2c20 3135 2c20 3136 2c20 3137 2c20  14, 15, 16, 17, 
-00025330: 3138 2c20 3139 2c20 3230 2c20 3231 2c20  18, 19, 20, 21, 
-00025340: 3232 2c20 3233 2c20 3234 2c20 3235 2c20  22, 23, 24, 25, 
-00025350: 3236 2c20 3237 2c20 3238 2c20 312c 2032  26, 27, 28, 1, 2
-00025360: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
-00025370: 2038 2c20 392c 2031 302c 2031 312c 2031   8, 9, 10, 11, 1
-00025380: 322c 2031 332c 2031 342c 2031 352c 2031  2, 13, 14, 15, 1
-00025390: 362c 2031 372c 2031 382c 2031 392c 2032  6, 17, 18, 19, 2
-000253a0: 302c 2032 312c 2032 322c 2032 332c 2032  0, 21, 22, 23, 2
-000253b0: 342c 2032 352c 2032 362c 2032 372c 2032  4, 25, 26, 27, 2
-000253c0: 382c 2032 392c 2033 302c 2033 312c 2031  8, 29, 30, 31, 1
-000253d0: 2c20 322c 2033 2c20 342c 2035 2c20 362c  , 2, 3, 4, 5, 6,
-000253e0: 2037 2c20 382c 2039 2c20 3130 2c20 3131   7, 8, 9, 10, 11
-000253f0: 2c20 3132 2c20 3133 2c20 3134 2c20 3135  , 12, 13, 14, 15
-00025400: 2c20 3136 2c20 3137 2c20 3138 2c20 3139  , 16, 17, 18, 19
-00025410: 2c20 3230 2c20 3231 2c20 3232 2c20 3233  , 20, 21, 22, 23
-00025420: 2c20 3234 2c20 3235 2c20 3236 2c20 3237  , 24, 25, 26, 27
-00025430: 2c20 3238 2c20 3239 2c20 3330 2c20 312c  , 28, 29, 30, 1,
-00025440: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
-00025450: 372c 2038 2c20 392c 2031 302c 2031 312c  7, 8, 9, 10, 11,
-00025460: 2031 322c 2031 332c 2031 342c 2031 352c   12, 13, 14, 15,
-00025470: 2031 362c 2031 372c 2031 382c 2031 392c   16, 17, 18, 19,
-00025480: 2032 302c 2032 312c 2032 322c 2032 332c   20, 21, 22, 23,
-00025490: 2032 342c 2032 352c 2032 362c 2032 372c   24, 25, 26, 27,
-000254a0: 2032 382c 2032 392c 2033 302c 2033 312c   28, 29, 30, 31,
-000254b0: 2031 2c20 322c 2033 2c20 342c 2035 2c20   1, 2, 3, 4, 5, 
-000254c0: 362c 2037 2c20 382c 2039 2c20 3130 2c20  6, 7, 8, 9, 10, 
-000254d0: 3131 2c20 3132 2c20 3133 2c20 3134 2c20  11, 12, 13, 14, 
-000254e0: 3135 2c20 3136 2c20 3137 2c20 3138 2c20  15, 16, 17, 18, 
-000254f0: 3139 2c20 3230 2c20 3231 2c20 3232 2c20  19, 20, 21, 22, 
-00025500: 3233 2c20 3234 2c20 3235 2c20 3236 2c20  23, 24, 25, 26, 
-00025510: 3237 2c20 3238 2c20 3239 2c20 3330 2c20  27, 28, 29, 30, 
-00025520: 312c 2032 2c20 332c 2034 2c20 352c 2036  1, 2, 3, 4, 5, 6
-00025530: 2c20 372c 2038 2c20 392c 2031 302c 2031  , 7, 8, 9, 10, 1
-00025540: 312c 2031 322c 2031 332c 2031 342c 2031  1, 12, 13, 14, 1
-00025550: 352c 2031 362c 2031 372c 2031 382c 2031  5, 16, 17, 18, 1
-00025560: 392c 2032 302c 2032 312c 2032 322c 2032  9, 20, 21, 22, 2
-00025570: 332c 2032 342c 2032 352c 2032 362c 2032  3, 24, 25, 26, 2
-00025580: 372c 2032 382c 2032 392c 2033 302c 2033  7, 28, 29, 30, 3
-00025590: 312c 2031 2c20 322c 2033 2c20 342c 2035  1, 1, 2, 3, 4, 5
-000255a0: 2c20 362c 2037 2c20 382c 2039 2c20 3130  , 6, 7, 8, 9, 10
-000255b0: 2c20 3131 2c20 3132 2c20 3133 2c20 3134  , 11, 12, 13, 14
-000255c0: 2c20 3135 2c20 3136 2c20 3137 2c20 3138  , 15, 16, 17, 18
-000255d0: 2c20 3139 2c20 3230 2c20 3231 2c20 3232  , 19, 20, 21, 22
-000255e0: 2c20 3233 2c20 3234 2c20 3235 2c20 3236  , 23, 24, 25, 26
-000255f0: 2c20 3237 2c20 3238 2c20 3239 2c20 3330  , 27, 28, 29, 30
-00025600: 2c20 3331 2c20 312c 2032 2c20 332c 2034  , 31, 1, 2, 3, 4
-00025610: 2c20 352c 2036 2c20 372c 2038 2c20 392c  , 5, 6, 7, 8, 9,
-00025620: 2031 302c 2031 312c 2031 322c 2031 332c   10, 11, 12, 13,
-00025630: 2031 342c 2031 352c 2031 362c 2031 372c   14, 15, 16, 17,
-00025640: 2031 382c 2031 392c 2032 302c 2032 312c   18, 19, 20, 21,
-00025650: 2032 322c 2032 332c 2032 342c 2032 352c   22, 23, 24, 25,
-00025660: 2032 362c 2032 372c 2032 382c 2032 392c   26, 27, 28, 29,
-00025670: 2033 302c 2031 2c20 322c 2033 2c20 342c   30, 1, 2, 3, 4,
-00025680: 2035 2c20 362c 2037 2c20 382c 2039 2c20   5, 6, 7, 8, 9, 
-00025690: 3130 2c20 3131 2c20 3132 2c20 3133 2c20  10, 11, 12, 13, 
-000256a0: 3134 2c20 3135 2c20 3136 2c20 3137 2c20  14, 15, 16, 17, 
-000256b0: 3138 2c20 3139 2c20 3230 2c20 3231 2c20  18, 19, 20, 21, 
-000256c0: 3232 2c20 3233 2c20 3234 2c20 3235 2c20  22, 23, 24, 25, 
-000256d0: 3236 2c20 3237 2c20 3238 2c20 3239 2c20  26, 27, 28, 29, 
-000256e0: 3330 2c20 3331 2c20 312c 2032 2c20 332c  30, 31, 1, 2, 3,
-000256f0: 2034 2c20 352c 2036 2c20 372c 2038 2c20   4, 5, 6, 7, 8, 
-00025700: 392c 2031 302c 2031 312c 2031 322c 2031  9, 10, 11, 12, 1
-00025710: 332c 2031 342c 2031 352c 2031 362c 2031  3, 14, 15, 16, 1
-00025720: 372c 2031 382c 2031 392c 2032 302c 2032  7, 18, 19, 20, 2
-00025730: 312c 2032 322c 2032 332c 2032 342c 2032  1, 22, 23, 24, 2
-00025740: 352c 2032 362c 2032 372c 2032 382c 2032  5, 26, 27, 28, 2
-00025750: 392c 2033 302c 2031 2c20 322c 2033 2c20  9, 30, 1, 2, 3, 
-00025760: 342c 2035 2c20 362c 2037 2c20 382c 2039  4, 5, 6, 7, 8, 9
-00025770: 2c20 3130 2c20 3131 2c20 3132 2c20 3133  , 10, 11, 12, 13
-00025780: 2c20 3134 2c20 3135 2c20 3136 2c20 3137  , 14, 15, 16, 17
-00025790: 2c20 3138 2c20 3139 2c20 3230 2c20 3231  , 18, 19, 20, 21
-000257a0: 2c20 3232 2c20 3233 2c20 3234 2c20 3235  , 22, 23, 24, 25
-000257b0: 2c20 3236 2c20 3237 2c20 3238 2c20 3239  , 26, 27, 28, 29
-000257c0: 2c20 3330 2c20 3331 205d 0d0a 6a75 6c69  , 30, 31 ]..juli
-000257d0: 616e 4461 7920 3d20 5b31 2c20 322c 2033  anDay = [1, 2, 3
-000257e0: 2c20 342c 2035 2c20 362c 2037 2c20 382c  , 4, 5, 6, 7, 8,
-000257f0: 2039 2c20 3130 2c20 3131 2c20 3132 2c20   9, 10, 11, 12, 
-00025800: 3133 2c20 3134 2c20 3135 2c20 3136 2c20  13, 14, 15, 16, 
-00025810: 3137 2c20 3138 2c20 3139 2c20 3230 2c20  17, 18, 19, 20, 
-00025820: 3231 2c20 3232 2c20 3233 2c20 3234 2c20  21, 22, 23, 24, 
-00025830: 3235 2c20 3236 2c20 3237 2c20 3238 2c20  25, 26, 27, 28, 
-00025840: 3239 2c20 3330 2c20 3331 2c20 3332 2c20  29, 30, 31, 32, 
-00025850: 3333 2c20 3334 2c20 3335 2c20 3336 2c20  33, 34, 35, 36, 
-00025860: 3337 2c20 3338 2c20 3339 2c20 3430 2c20  37, 38, 39, 40, 
-00025870: 3431 2c20 3432 2c20 3433 2c20 3434 2c20  41, 42, 43, 44, 
-00025880: 3435 2c20 3436 2c20 3437 2c20 3438 2c20  45, 46, 47, 48, 
-00025890: 3439 2c20 3530 2c20 3531 2c20 3532 2c20  49, 50, 51, 52, 
-000258a0: 3533 2c20 3534 2c20 3535 2c20 3536 2c20  53, 54, 55, 56, 
-000258b0: 3537 2c20 3538 2c20 3539 2c20 3630 2c20  57, 58, 59, 60, 
-000258c0: 3631 2c20 3632 2c20 3633 2c20 3634 2c20  61, 62, 63, 64, 
-000258d0: 3635 2c20 3636 2c20 3637 2c20 3638 2c20  65, 66, 67, 68, 
-000258e0: 3639 2c20 3730 2c20 3731 2c20 3732 2c20  69, 70, 71, 72, 
-000258f0: 3733 2c20 3734 2c20 3735 2c20 3736 2c20  73, 74, 75, 76, 
-00025900: 3737 2c20 3738 2c20 3739 2c20 3830 2c20  77, 78, 79, 80, 
-00025910: 3831 2c20 3832 2c20 3833 2c20 3834 2c20  81, 82, 83, 84, 
-00025920: 3835 2c20 3836 2c20 3837 2c20 3838 2c20  85, 86, 87, 88, 
-00025930: 3839 2c20 3930 2c20 3931 2c20 3932 2c20  89, 90, 91, 92, 
-00025940: 3933 2c20 3934 2c20 3935 2c20 3936 2c20  93, 94, 95, 96, 
-00025950: 3937 2c20 3938 2c20 3939 2c20 3130 302c  97, 98, 99, 100,
-00025960: 2031 3031 2c20 3130 322c 2031 3033 2c20   101, 102, 103, 
-00025970: 3130 342c 2031 3035 2c20 3130 362c 2031  104, 105, 106, 1
-00025980: 3037 2c20 3130 382c 2031 3039 2c20 3131  07, 108, 109, 11
-00025990: 302c 2031 3131 2c20 3131 322c 2031 3133  0, 111, 112, 113
-000259a0: 2c20 3131 342c 2031 3135 2c20 3131 362c  , 114, 115, 116,
-000259b0: 2031 3137 2c20 3131 382c 2031 3139 2c20   117, 118, 119, 
-000259c0: 3132 302c 2031 3231 2c20 3132 322c 2031  120, 121, 122, 1
-000259d0: 3233 2c20 3132 342c 2031 3235 2c20 3132  23, 124, 125, 12
-000259e0: 362c 2031 3237 2c20 3132 382c 2031 3239  6, 127, 128, 129
-000259f0: 2c20 3133 302c 2031 3331 2c20 3133 322c  , 130, 131, 132,
-00025a00: 2031 3333 2c20 3133 342c 2031 3335 2c20   133, 134, 135, 
-00025a10: 3133 362c 2031 3337 2c20 3133 382c 2031  136, 137, 138, 1
-00025a20: 3339 2c20 3134 302c 2031 3431 2c20 3134  39, 140, 141, 14
-00025a30: 322c 2031 3433 2c20 3134 342c 2031 3435  2, 143, 144, 145
-00025a40: 2c20 3134 362c 2031 3437 2c20 3134 382c  , 146, 147, 148,
-00025a50: 2031 3439 2c20 3135 302c 2031 3531 2c20   149, 150, 151, 
-00025a60: 3135 322c 2031 3533 2c20 3135 342c 2031  152, 153, 154, 1
-00025a70: 3535 2c20 3135 362c 2031 3537 2c20 3135  55, 156, 157, 15
-00025a80: 382c 2031 3539 2c20 3136 302c 2031 3631  8, 159, 160, 161
-00025a90: 2c20 3136 322c 2031 3633 2c20 3136 342c  , 162, 163, 164,
-00025aa0: 2031 3635 2c20 3136 362c 2031 3637 2c20   165, 166, 167, 
-00025ab0: 3136 382c 2031 3639 2c20 3137 302c 2031  168, 169, 170, 1
-00025ac0: 3731 2c20 3137 322c 2031 3733 2c20 3137  71, 172, 173, 17
-00025ad0: 342c 2031 3735 2c20 3137 362c 2031 3737  4, 175, 176, 177
-00025ae0: 2c20 3137 382c 2031 3739 2c20 3138 302c  , 178, 179, 180,
-00025af0: 2031 3831 2c20 3138 322c 2031 3833 2c20   181, 182, 183, 
-00025b00: 3138 342c 2031 3835 2c20 3138 362c 2031  184, 185, 186, 1
-00025b10: 3837 2c20 3138 382c 2031 3839 2c20 3139  87, 188, 189, 19
-00025b20: 302c 2031 3931 2c20 3139 322c 2031 3933  0, 191, 192, 193
-00025b30: 2c20 3139 342c 2031 3935 2c20 3139 362c  , 194, 195, 196,
-00025b40: 2031 3937 2c20 3139 382c 2031 3939 2c20   197, 198, 199, 
-00025b50: 3230 302c 2032 3031 2c20 3230 322c 2032  200, 201, 202, 2
-00025b60: 3033 2c20 3230 342c 2032 3035 2c20 3230  03, 204, 205, 20
-00025b70: 362c 2032 3037 2c20 3230 382c 2032 3039  6, 207, 208, 209
-00025b80: 2c20 3231 302c 2032 3131 2c20 3231 322c  , 210, 211, 212,
-00025b90: 2032 3133 2c20 3231 342c 2032 3135 2c20   213, 214, 215, 
-00025ba0: 3231 362c 2032 3137 2c20 3231 382c 2032  216, 217, 218, 2
-00025bb0: 3139 2c20 3232 302c 2032 3231 2c20 3232  19, 220, 221, 22
-00025bc0: 322c 2032 3233 2c20 3232 342c 2032 3235  2, 223, 224, 225
-00025bd0: 2c20 3232 362c 2032 3237 2c20 3232 382c  , 226, 227, 228,
-00025be0: 2032 3239 2c20 3233 302c 2032 3331 2c20   229, 230, 231, 
-00025bf0: 3233 322c 2032 3333 2c20 3233 342c 2032  232, 233, 234, 2
-00025c00: 3335 2c20 3233 362c 2032 3337 2c20 3233  35, 236, 237, 23
-00025c10: 382c 2032 3339 2c20 3234 302c 2032 3431  8, 239, 240, 241
-00025c20: 2c20 3234 322c 2032 3433 2c20 3234 342c  , 242, 243, 244,
-00025c30: 2032 3435 2c20 3234 362c 2032 3437 2c20   245, 246, 247, 
-00025c40: 3234 382c 2032 3439 2c20 3235 302c 2032  248, 249, 250, 2
-00025c50: 3531 2c20 3235 322c 2032 3533 2c20 3235  51, 252, 253, 25
-00025c60: 342c 2032 3535 2c20 3235 362c 2032 3537  4, 255, 256, 257
-00025c70: 2c20 3235 382c 2032 3539 2c20 3236 302c  , 258, 259, 260,
-00025c80: 2032 3631 2c20 3236 322c 2032 3633 2c20   261, 262, 263, 
-00025c90: 3236 342c 2032 3635 2c20 3236 362c 2032  264, 265, 266, 2
-00025ca0: 3637 2c20 3236 382c 2032 3639 2c20 3237  67, 268, 269, 27
-00025cb0: 302c 2032 3731 2c20 3237 322c 2032 3733  0, 271, 272, 273
-00025cc0: 2c20 3237 342c 2032 3735 2c20 3237 362c  , 274, 275, 276,
-00025cd0: 2032 3737 2c20 3237 382c 2032 3739 2c20   277, 278, 279, 
-00025ce0: 3238 302c 2032 3831 2c20 3238 322c 2032  280, 281, 282, 2
-00025cf0: 3833 2c20 3238 342c 2032 3835 2c20 3238  83, 284, 285, 28
-00025d00: 362c 2032 3837 2c20 3238 382c 2032 3839  6, 287, 288, 289
-00025d10: 2c20 3239 302c 2032 3931 2c20 3239 322c  , 290, 291, 292,
-00025d20: 2032 3933 2c20 3239 342c 2032 3935 2c20   293, 294, 295, 
-00025d30: 3239 362c 2032 3937 2c20 3239 382c 2032  296, 297, 298, 2
-00025d40: 3939 2c20 3330 302c 2033 3031 2c20 3330  99, 300, 301, 30
-00025d50: 322c 2033 3033 2c20 3330 342c 2033 3035  2, 303, 304, 305
-00025d60: 2c20 3330 362c 2033 3037 2c20 3330 382c  , 306, 307, 308,
-00025d70: 2033 3039 2c20 3331 302c 2033 3131 2c20   309, 310, 311, 
-00025d80: 3331 322c 2033 3133 2c20 3331 342c 2033  312, 313, 314, 3
-00025d90: 3135 2c20 3331 362c 2033 3137 2c20 3331  15, 316, 317, 31
-00025da0: 382c 2033 3139 2c20 3332 302c 2033 3231  8, 319, 320, 321
-00025db0: 2c20 3332 322c 2033 3233 2c20 3332 342c  , 322, 323, 324,
-00025dc0: 2033 3235 2c20 3332 362c 2033 3237 2c20   325, 326, 327, 
-00025dd0: 3332 382c 2033 3239 2c20 3333 302c 2033  328, 329, 330, 3
-00025de0: 3331 2c20 3333 322c 2033 3333 2c20 3333  31, 332, 333, 33
-00025df0: 342c 2033 3335 2c20 3333 362c 2033 3337  4, 335, 336, 337
-00025e00: 2c20 3333 382c 2033 3339 2c20 3334 302c  , 338, 339, 340,
-00025e10: 2033 3431 2c20 3334 322c 2033 3433 2c20   341, 342, 343, 
-00025e20: 3334 342c 2033 3435 2c20 3334 362c 2033  344, 345, 346, 3
-00025e30: 3437 2c20 3334 382c 2033 3439 2c20 3335  47, 348, 349, 35
-00025e40: 302c 2033 3531 2c20 3335 322c 2033 3533  0, 351, 352, 353
-00025e50: 2c20 3335 342c 2033 3535 2c20 3335 362c  , 354, 355, 356,
-00025e60: 2033 3537 2c20 3335 382c 2033 3539 2c20   357, 358, 359, 
-00025e70: 3336 302c 2033 3631 2c20 3336 322c 2033  360, 361, 362, 3
-00025e80: 3633 2c20 3336 342c 2033 3635 205d 0d0a  63, 364, 365 ]..
-00025e90: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-00025ea0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025eb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025ed0: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
-00025ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025f10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025f20: 2323 2323 2323 0d0a 2346 756e 6374 696f  ######..#Functio
-00025f30: 6e20 666f 7220 6765 7474 696e 6720 7468  n for getting th
-00025f40: 6520 6461 7465 206f 6620 7468 6520 7065  e date of the pe
-00025f50: 616b 206f 6620 7665 6720 7669 676f 722d  ak of veg vigor-
-00025f60: 2063 616e 2068 616e 646c 6520 6261 6e64   can handle band
-00025f70: 7320 6e65 6761 7469 7665 6c79 2063 6f72  s negatively cor
-00025f80: 7265 6c61 7465 6420 746f 2076 6567 2069  related to veg i
-00025f90: 6e0d 0a23 6368 616e 6765 4469 7244 6963  n..#changeDirDic
-00025fa0: 7420 6469 6374 696f 6e61 7279 2061 626f  t dictionary abo
-00025fb0: 7665 0d0a 6465 6620 6765 7450 6561 6b44  ve..def getPeakD
-00025fc0: 6174 6528 636f 6566 6673 2c70 6561 6b44  ate(coeffs,peakD
-00025fd0: 6972 6563 7469 6f6e 203d 2031 293a 0d0a  irection = 1):..
-00025fe0: 0d0a 2020 7369 6e20 3d20 636f 6566 6673  ..  sin = coeffs
-00025ff0: 2e73 656c 6563 7428 5b30 5d29 0d0a 2020  .select([0])..  
-00026000: 636f 7320 3d20 636f 6566 6673 2e73 656c  cos = coeffs.sel
-00026010: 6563 7428 5b31 5d29 0d0a 0d0a 2020 2346  ect([1])....  #F
-00026020: 696e 6420 7768 6572 6520 696e 2063 7963  ind where in cyc
-00026030: 6c65 2073 6c6f 7065 2069 7320 7a65 726f  le slope is zero
-00026040: 0d0a 2020 6772 6565 6e44 6174 6520 3d20  ..  greenDate = 
-00026050: 2828 7369 6e2e 6469 7669 6465 2863 6f73  ((sin.divide(cos
-00026060: 2929 2e61 7461 6e28 2929 2e64 6976 6964  )).atan()).divid
-00026070: 6528 322a 6d61 7468 2e70 6929 2e72 656e  e(2*math.pi).ren
-00026080: 616d 6528 5b27 7065 616b 4461 7465 275d  ame(['peakDate']
-00026090: 290d 0a20 2067 7265 656e 4461 7465 4c61  )..  greenDateLa
-000260a0: 7465 7220 3d20 6772 6565 6e44 6174 652e  ter = greenDate.
-000260b0: 6164 6428 302e 3529 0d0a 2020 2343 6865  add(0.5)..  #Che
-000260c0: 636b 2077 6869 6368 2064 3120 736c 6f70  ck which d1 slop
-000260d0: 6520 3d20 3020 6973 2074 6865 206d 6178  e = 0 is the max
-000260e0: 2062 7920 7072 6564 6963 7469 6e67 206f   by predicting o
-000260f0: 7574 2074 6865 2076 616c 7565 0d0a 2020  ut the value..  
-00026100: 7072 6564 6963 7465 6431 203d 2063 6f65  predicted1 = coe
-00026110: 6666 732e 7365 6c65 6374 285b 305d 295c  ffs.select([0])\
-00026120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00026130: 2e61 6464 2873 696e 2e6d 756c 7469 706c  .add(sin.multipl
-00026140: 7928 6772 6565 6e44 6174 652e 6d75 6c74  y(greenDate.mult
-00026150: 6970 6c79 2832 2a6d 6174 682e 7069 292e  iply(2*math.pi).
-00026160: 7369 6e28 2929 295c 0d0a 2020 2020 2020  sin()))\..      
-00026170: 2020 2020 2020 2020 2e61 6464 2863 6f73          .add(cos
-00026180: 2e6d 756c 7469 706c 7928 6772 6565 6e44  .multiply(greenD
-00026190: 6174 652e 6d75 6c74 6970 6c79 2832 2a6d  ate.multiply(2*m
-000261a0: 6174 682e 7069 292e 636f 7328 2929 295c  ath.pi).cos()))\
-000261b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000261c0: 2e72 656e 616d 6528 5b27 7072 6564 6963  .rename(['predic
-000261d0: 7465 6427 5d29 5c0d 0a20 2020 2020 2020  ted'])\..       
-000261e0: 2020 2020 2020 202e 6d75 6c74 6970 6c79         .multiply
-000261f0: 2865 652e 496d 6167 652e 636f 6e73 7461  (ee.Image.consta
-00026200: 6e74 2870 6561 6b44 6972 6563 7469 6f6e  nt(peakDirection
-00026210: 2929 5c0d 0a20 2020 2020 2020 2020 2020  ))\..           
-00026220: 2020 202e 6164 6442 616e 6473 2867 7265     .addBands(gre
-00026230: 656e 4461 7465 290d 0a20 2070 7265 6469  enDate)..  predi
-00026240: 6374 6564 3220 3d20 636f 6566 6673 2e73  cted2 = coeffs.s
-00026250: 656c 6563 7428 5b30 5d29 5c0d 0a20 2020  elect([0])\..   
-00026260: 2020 2020 2020 2020 2020 202e 6164 6428             .add(
-00026270: 7369 6e2e 6d75 6c74 6970 6c79 2867 7265  sin.multiply(gre
-00026280: 656e 4461 7465 4c61 7465 722e 6d75 6c74  enDateLater.mult
-00026290: 6970 6c79 2832 2a6d 6174 682e 7069 292e  iply(2*math.pi).
-000262a0: 7369 6e28 2929 295c 0d0a 2020 2020 2020  sin()))\..      
-000262b0: 2020 2020 2020 2020 2e61 6464 2863 6f73          .add(cos
-000262c0: 2e6d 756c 7469 706c 7928 6772 6565 6e44  .multiply(greenD
-000262d0: 6174 654c 6174 6572 2e6d 756c 7469 706c  ateLater.multipl
-000262e0: 7928 322a 6d61 7468 2e70 6929 2e63 6f73  y(2*math.pi).cos
-000262f0: 2829 2929 5c0d 0a20 2020 2020 2020 2020  ()))\..         
-00026300: 2020 2020 202e 7265 6e61 6d65 285b 2770       .rename(['p
-00026310: 7265 6469 6374 6564 275d 295c 0d0a 2020  redicted'])\..  
-00026320: 2020 2020 2020 2020 2020 2020 2e6d 756c              .mul
-00026330: 7469 706c 7928 6565 2e49 6d61 6765 2e63  tiply(ee.Image.c
-00026340: 6f6e 7374 616e 7428 7065 616b 4469 7265  onstant(peakDire
-00026350: 6374 696f 6e29 295c 0d0a 2020 2020 2020  ction))\..      
-00026360: 2020 2020 2020 2020 2e61 6464 4261 6e64          .addBand
-00026370: 7328 6772 6565 6e44 6174 654c 6174 6572  s(greenDateLater
-00026380: 290d 0a20 2066 696e 616c 4772 6565 6e44  )..  finalGreenD
-00026390: 6174 6520 3d20 6565 2e49 6d61 6765 436f  ate = ee.ImageCo
-000263a0: 6c6c 6563 7469 6f6e 285b 7072 6564 6963  llection([predic
-000263b0: 7465 6431 2c70 7265 6469 6374 6564 325d  ted1,predicted2]
-000263c0: 292e 7175 616c 6974 794d 6f73 6169 6328  ).qualityMosaic(
-000263d0: 2770 7265 6469 6374 6564 2729 2e73 656c  'predicted').sel
-000263e0: 6563 7428 5b27 7065 616b 4461 7465 275d  ect(['peakDate']
-000263f0: 292e 7265 6e61 6d65 285b 2770 6561 6b4a  ).rename(['peakJ
-00026400: 756c 6961 6e44 6179 275d 290d 0a0d 0a20  ulianDay']).... 
-00026410: 2066 696e 616c 4772 6565 6e44 6174 6520   finalGreenDate 
-00026420: 3d20 6669 6e61 6c47 7265 656e 4461 7465  = finalGreenDate
-00026430: 2e77 6865 7265 2866 696e 616c 4772 6565  .where(finalGree
-00026440: 6e44 6174 652e 6c74 2830 292c 2067 7265  nDate.lt(0), gre
-00026450: 656e 4461 7465 2e61 6464 2831 2929 2e6d  enDate.add(1)).m
-00026460: 756c 7469 706c 7928 3336 3529 2e69 6e74  ultiply(365).int
-00026470: 3136 2829 3b0d 0a0d 0a20 2023 436f 6e76  16();....  #Conv
-00026480: 6572 7420 746f 206d 6f6e 7468 2061 6e64  ert to month and
-00026490: 2064 6179 206f 6620 6d6f 6e74 680d 0a20   day of month.. 
-000264a0: 2067 7265 656e 4d6f 6e74 6820 3d20 6669   greenMonth = fi
-000264b0: 6e61 6c47 7265 656e 4461 7465 2e72 656d  nalGreenDate.rem
-000264c0: 6170 286a 756c 6961 6e44 6179 2c6d 6f6e  ap(julianDay,mon
-000264d0: 7468 5265 6d61 7029 2e72 656e 616d 6528  thRemap).rename(
-000264e0: 5b27 7065 616b 4d6f 6e74 6827 5d29 0d0a  ['peakMonth'])..
-000264f0: 2020 6772 6565 6e4d 6f6e 7468 4461 7920    greenMonthDay 
-00026500: 3d20 6669 6e61 6c47 7265 656e 4461 7465  = finalGreenDate
-00026510: 2e72 656d 6170 286a 756c 6961 6e44 6179  .remap(julianDay
-00026520: 2c6d 6f6e 7468 4461 7952 656d 6170 292e  ,monthDayRemap).
-00026530: 7265 6e61 6d65 285b 2770 6561 6b44 6179  rename(['peakDay
-00026540: 4f66 4d6f 6e74 6827 5d29 0d0a 2020 6772  OfMonth'])..  gr
-00026550: 6565 6e53 7461 636b 203d 2066 696e 616c  eenStack = final
-00026560: 4772 6565 6e44 6174 652e 6164 6442 616e  GreenDate.addBan
-00026570: 6473 2867 7265 656e 4d6f 6e74 6829 2e61  ds(greenMonth).a
-00026580: 6464 4261 6e64 7328 6772 6565 6e4d 6f6e  ddBands(greenMon
-00026590: 7468 4461 7929 0d0a 2020 7265 7475 726e  thDay)..  return
-000265a0: 2067 7265 656e 5374 6163 6b0d 0a20 2023   greenStack..  #
-000265b0: 4d61 702e 6164 644c 6179 6572 2867 7265  Map.addLayer(gre
-000265c0: 656e 5374 6163 6b2c 7b27 6d69 6e27 3a31  enStack,{'min':1
-000265d0: 2c27 6d61 7827 3a31 327d 2c27 6772 6565  ,'max':12},'gree
-000265e0: 6e4d 6f6e 7468 272c 4661 6c73 6529 0d0a  nMonth',False)..
-000265f0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-00026600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026630: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
-00026640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026680: 2323 2323 2323 0d0a 2346 756e 6374 696f  ######..#Functio
-00026690: 6e20 666f 7220 6765 7474 696e 6720 6c65  n for getting le
-000266a0: 6674 2073 756d 2075 6e64 6572 2074 6865  ft sum under the
-000266b0: 2063 7572 7665 2066 6f72 2061 2073 696e   curve for a sin
-000266c0: 676c 6520 6772 6f77 696e 6720 7365 6173  gle growing seas
-000266d0: 6f6e 0d0a 2354 616b 6573 2063 6172 6520  on..#Takes care 
-000266e0: 6f66 206e 6f72 6d61 6c69 7a61 7469 6f6e  of normalization
-000266f0: 2062 7920 666f 7263 696e 6720 7468 6520   by forcing the 
-00026700: 6d69 6e20 7661 6c75 6520 616c 6f6e 6720  min value along 
-00026710: 7468 6520 6375 7276 6520 300d 0a23 6279  the curve 0..#by
-00026720: 2074 616b 696e 6720 7468 6520 616d 706c   taking the ampl
-00026730: 6974 7564 6520 6173 2074 6865 2069 6e74  itude as the int
-00026740: 6572 6365 7074 0d0a 2341 7373 756d 6573  ercept..#Assumes
-00026750: 2074 6865 2073 696e 2061 6e64 2063 6f73   the sin and cos
-00026760: 2063 6f65 6666 7320 6172 6520 7468 6520   coeffs are the 
-00026770: 6861 726d 436f 6566 6673 0d0a 2374 3020  harmCoeffs..#t0 
-00026780: 6973 2074 6865 2073 7461 7274 2074 696d  is the start tim
-00026790: 6520 2864 6566 6175 6c74 7320 746f 2030  e (defaults to 0
-000267a0: 2928 6d69 6e20 7661 6c75 6520 7368 6f75  )(min value shou
-000267b0: 6c64 2062 6520 6275 7420 646f 6573 6e27  ld be but doesn'
-000267c0: 7420 6861 7665 2074 6f20 6265 2030 290d  t have to be 0).
-000267d0: 0a23 7431 2069 7320 7468 6520 656e 6420  .#t1 is the end 
-000267e0: 7469 6d65 2028 6465 6661 756c 7473 2074  time (defaults t
-000267f0: 6f20 3129 286d 6178 2076 616c 7565 2073  o 1)(max value s
-00026800: 686f 756c 6420 6265 2062 7574 2064 6f65  hould be but doe
-00026810: 736e 2774 2068 6176 6520 746f 2062 6520  sn't have to be 
-00026820: 3129 0d0a 0d0a 2345 7861 6d70 6c65 206f  1)....#Example o
-00026830: 6620 7768 6174 2074 6869 7320 636f 6465  f what this code
-00026840: 2069 7320 646f 696e 6720 6361 6e20 6265   is doing can be
-00026850: 2066 6f75 6e64 2068 6572 653a 0d0a 2320   found here:..# 
-00026860: 2068 7474 703a 2f2f 7777 772e 776f 6c66   http://www.wolf
-00026870: 7261 6d61 6c70 6861 2e63 6f6d 2f69 6e70  ramalpha.com/inp
-00026880: 7574 2f3f 693d 696e 7465 6772 6174 652b  ut/?i=integrate+
-00026890: 302e 3135 3934 3930 3734 3932 3339 3932  0.15949074923992
-000268a0: 3135 372b 2532 422b 2d30 2e30 3832 3837  157+%2B+-0.08287
-000268b0: 3539 392a 7369 6e28 322b 5049 2b54 292b  599*sin(2+PI+T)+
-000268c0: 2532 422b 2d30 2e31 3132 3532 3031 3036  %2B+-0.112520106
-000268d0: 3133 2a63 6f73 2832 2b50 492b 5429 2b2b  13*cos(2+PI+T)++
-000268e0: 6672 6f6d 2b30 2b74 6f2b 310d 0a64 6566  from+0+to+1..def
-000268f0: 2067 6574 4172 6561 556e 6465 7243 7572   getAreaUnderCur
-00026900: 7665 2868 6172 6d43 6f65 6666 732c 7430  ve(harmCoeffs,t0
-00026910: 3d20 302c 7431 203d 2031 293a 0d0a 0d0a  = 0,t1 = 1):....
-00026920: 2020 2350 756c 6c20 6170 6172 7420 7468    #Pull apart th
-00026930: 6520 6d6f 6465 6c0d 0a20 2061 6d70 6c69  e model..  ampli
-00026940: 7475 6465 203d 2068 6172 6d43 6f65 6666  tude = harmCoeff
-00026950: 732e 7365 6c65 6374 285b 315d 292e 6879  s.select([1]).hy
-00026960: 706f 7428 6861 726d 436f 6566 6673 2e73  pot(harmCoeffs.s
-00026970: 656c 6563 7428 5b30 5d29 290d 0a20 2069  elect([0]))..  i
-00026980: 6e74 6572 6563 6570 744e 6f72 6d61 6c69  ntereceptNormali
-00026990: 7a65 6420 3d20 616d 706c 6974 7564 6523  zed = amplitude#
-000269a0: 5768 656e 206d 616b 696e 6720 7468 6520  When making the 
-000269b0: 6d69 6e20 302c 2074 6865 2069 6e74 6572  min 0, the inter
-000269c0: 6365 7074 2062 6563 6f6d 6573 2074 6865  cept becomes the
-000269d0: 2061 6d70 6c69 7475 6465 2028 7468 6520   amplitude (the 
-000269e0: 6879 706f 7465 6e75 7365 290d 0a20 2073  hypotenuse)..  s
-000269f0: 696e 203d 2068 6172 6d43 6f65 6666 732e  in = harmCoeffs.
-00026a00: 7365 6c65 6374 285b 305d 290d 0a20 2063  select([0])..  c
-00026a10: 6f73 203d 2068 6172 6d43 6f65 6666 732e  os = harmCoeffs.
-00026a20: 7365 6c65 6374 285b 315d 290d 0a0d 0a20  select([1]).... 
-00026a30: 2023 4669 6e64 2074 6865 2073 756d 2066   #Find the sum f
-00026a40: 726f 6d20 2d20 696e 6669 6e69 7479 2074  rom - infinity t
-00026a50: 6f20 300d 0a20 2073 756d 3020 3d20 696e  o 0..  sum0 = in
-00026a60: 7465 7265 6365 7074 4e6f 726d 616c 697a  tereceptNormaliz
-00026a70: 6564 2e6d 756c 7469 706c 7928 7430 295c  ed.multiply(t0)\
-00026a80: 0d0a 2020 2020 2020 2020 2020 2020 2e73  ..            .s
-00026a90: 7562 7472 6163 7428 7369 6e2e 6469 7669  ubtract(sin.divi
-00026aa0: 6465 2832 2a6d 6174 682e 7069 292e 6d75  de(2*math.pi).mu
-00026ab0: 6c74 6970 6c79 286d 6174 682e 7369 6e28  ltiply(math.sin(
-00026ac0: 322a 6d61 7468 2e70 692a 7430 2929 295c  2*math.pi*t0)))\
-00026ad0: 0d0a 2020 2020 2020 2020 2020 2020 2e61  ..            .a
-00026ae0: 6464 2863 6f73 2e64 6976 6964 6528 322a  dd(cos.divide(2*
-00026af0: 6d61 7468 2e70 6929 2e6d 756c 7469 706c  math.pi).multipl
-00026b00: 7928 6d61 7468 2e63 6f73 2832 2a6d 6174  y(math.cos(2*mat
-00026b10: 682e 7069 2a74 3029 2929 0d0a 2020 2346  h.pi*t0)))..  #F
-00026b20: 696e 6420 7468 6520 7375 6d20 6672 6f6d  ind the sum from
-00026b30: 202d 2069 6e66 696e 6974 7920 746f 2031   - infinity to 1
-00026b40: 0d0a 2020 7375 6d31 203d 2069 6e74 6572  ..  sum1 = inter
-00026b50: 6563 6570 744e 6f72 6d61 6c69 7a65 642e  eceptNormalized.
-00026b60: 6d75 6c74 6970 6c79 2874 3129 5c0d 0a20  multiply(t1)\.. 
-00026b70: 2020 2020 2020 202e 7375 6274 7261 6374         .subtract
-00026b80: 2873 696e 2e64 6976 6964 6528 322a 6d61  (sin.divide(2*ma
-00026b90: 7468 2e70 6929 2e6d 756c 7469 706c 7928  th.pi).multiply(
-00026ba0: 6d61 7468 2e73 696e 2832 2a6d 6174 682e  math.sin(2*math.
-00026bb0: 7069 2a74 3129 2929 5c0d 0a20 2020 2020  pi*t1)))\..     
-00026bc0: 2020 202e 6164 6428 636f 732e 6469 7669     .add(cos.divi
-00026bd0: 6465 2832 2a6d 6174 682e 7069 292e 6d75  de(2*math.pi).mu
-00026be0: 6c74 6970 6c79 286d 6174 682e 636f 7328  ltiply(math.cos(
-00026bf0: 322a 6d61 7468 2e70 692a 7431 2929 290d  2*math.pi*t1))).
-00026c00: 0a20 2023 4669 6e64 2074 6865 2064 6966  .  #Find the dif
-00026c10: 6665 7265 6e63 650d 0a20 206c 6566 7453  ference..  leftS
-00026c20: 756d 203d 2073 756d 312e 7375 6274 7261  um = sum1.subtra
-00026c30: 6374 2873 756d 3029 2e72 656e 616d 6528  ct(sum0).rename(
-00026c40: 5b27 4155 4327 5d29 0d0a 2020 7265 7475  ['AUC'])..  retu
-00026c50: 726e 206c 6566 7453 756d 0d0a 0d0a 2323  rn leftSum....##
-00026c60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026c70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026c80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026c90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026ca0: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
-00026cb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026cc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026cf0: 2323 0d0a 6465 6620 6765 7450 6861 7365  ##..def getPhase
-00026d00: 416d 706c 6974 7564 6550 6561 6b28 636f  AmplitudePeak(co
-00026d10: 6566 6673 2c74 3020 3d20 302c 7431 203d  effs,t0 = 0,t1 =
-00026d20: 2031 293a 0d0a 2020 2350 6172 7365 2074   1):..  #Parse t
-00026d30: 6865 206d 6f64 656c 0d0a 2020 6261 6e64  he model..  band
-00026d40: 4e61 6d65 7320 3d20 636f 6566 6673 2e62  Names = coeffs.b
-00026d50: 616e 644e 616d 6573 2829 0d0a 2020 6261  andNames()..  ba
-00026d60: 6e64 4e75 6d62 6572 203d 2062 616e 644e  ndNumber = bandN
-00026d70: 616d 6573 2e6c 656e 6774 6828 290d 0a20  ames.length().. 
-00026d80: 206e 6f44 6570 656e 6465 6e74 7320 3d20   noDependents = 
-00026d90: 6565 2e4e 756d 6265 7228 636f 6566 6673  ee.Number(coeffs
-00026da0: 2e67 6574 2827 6e6f 4465 7065 6e64 656e  .get('noDependen
-00026db0: 7473 2729 290d 0a20 206d 6f64 656c 4c65  ts'))..  modelLe
-00026dc0: 6e67 7468 203d 2065 652e 4e75 6d62 6572  ngth = ee.Number
-00026dd0: 2863 6f65 6666 732e 6765 7428 276d 6f64  (coeffs.get('mod
-00026de0: 656c 4c65 6e67 7468 2729 290d 0a20 2069  elLength'))..  i
-00026df0: 6e74 6572 6365 7074 4261 6e64 7320 3d20  nterceptBands = 
-00026e00: 6565 2e4c 6973 742e 7365 7175 656e 6365  ee.List.sequence
-00026e10: 2830 2c62 616e 644e 756d 6265 722e 7375  (0,bandNumber.su
-00026e20: 6274 7261 6374 2831 292c 6d6f 6465 6c4c  btract(1),modelL
-00026e30: 656e 6774 6829 0d0a 0d0a 2020 6d6f 6465  ength)....  mode
-00026e40: 6c73 203d 2065 652e 4c69 7374 2e73 6571  ls = ee.List.seq
-00026e50: 7565 6e63 6528 302c 6e6f 4465 7065 6e64  uence(0,noDepend
-00026e60: 656e 7473 2e73 7562 7472 6163 7428 3129  ents.subtract(1)
-00026e70: 290d 0a0d 0a20 2064 6566 206d 6f64 656c  )....  def model
-00026e80: 4765 7474 6572 286d 6e29 3a0d 0a20 2020  Getter(mn):..   
-00026e90: 206d 6e20 3d20 6565 2e4e 756d 6265 7228   mn = ee.Number(
-00026ea0: 6d6e 290d 0a20 2020 2072 6574 7572 6e20  mn)..    return 
-00026eb0: 6261 6e64 4e61 6d65 732e 736c 6963 6528  bandNames.slice(
-00026ec0: 6d6e 2e6d 756c 7469 706c 7928 6d6f 6465  mn.multiply(mode
-00026ed0: 6c4c 656e 6774 6829 2c6d 6e2e 6d75 6c74  lLength),mn.mult
-00026ee0: 6970 6c79 286d 6f64 656c 4c65 6e67 7468  iply(modelLength
-00026ef0: 292e 6164 6428 6d6f 6465 6c4c 656e 6774  ).add(modelLengt
-00026f00: 6829 290d 0a0d 0a20 2070 6172 7365 644d  h))....  parsedM
-00026f10: 6f64 656c 203d 6d6f 6465 6c73 2e6d 6170  odel =models.map
-00026f20: 286d 6f64 656c 4765 7474 6572 290d 0a0d  (modelGetter)...
-00026f30: 0a0d 0a20 2023 7072 696e 7428 2750 6172  ...  #print('Par
-00026f40: 7365 6420 6861 726d 6f6e 6963 2072 6567  sed harmonic reg
-00026f50: 7265 7373 696f 6e20 6d6f 6465 6c27 2c70  ression model',p
-00026f60: 6172 7365 644d 6f64 656c 290d 0a0d 0a20  arsedModel).... 
-00026f70: 2023 4974 6572 6174 6520 6163 726f 7373   #Iterate across
-00026f80: 206d 6f64 656c 7320 746f 2063 6f6e 7665   models to conve
-00026f90: 7274 2074 6f20 7068 6173 652c 2061 6d70  rt to phase, amp
-00026fa0: 6c69 7475 6465 2c20 616e 6420 7065 616b  litude, and peak
-00026fb0: 0d0a 2020 6465 6620 7061 7047 6574 7465  ..  def papGette
-00026fc0: 7228 706d 293a 0d0a 2020 2020 706d 203d  r(pm):..    pm =
-00026fd0: 2065 652e 4c69 7374 2870 6d29 3b0d 0a20   ee.List(pm);.. 
-00026fe0: 2020 206d 6f64 656c 436f 6566 6673 203d     modelCoeffs =
-00026ff0: 2063 6f65 6666 732e 7365 6c65 6374 2870   coeffs.select(p
-00027000: 6d29 0d0a 0d0a 2020 2020 696e 7465 7263  m)....    interc
-00027010: 6570 7420 3d20 6d6f 6465 6c43 6f65 6666  ept = modelCoeff
-00027020: 732e 7365 6c65 6374 2827 2e2a 5f69 6e74  s.select('.*_int
-00027030: 6572 6365 7074 2729 0d0a 2020 2020 6861  ercept')..    ha
-00027040: 726d 436f 6566 6673 203d 206d 6f64 656c  rmCoeffs = model
-00027050: 436f 6566 6673 2e73 656c 6563 7428 272e  Coeffs.select('.
-00027060: 2a5f 3230 305f 7965 6172 2729 0d0a 2020  *_200_year')..  
-00027070: 2020 6f75 744e 616d 6520 3d20 6565 2e53    outName = ee.S
-00027080: 7472 696e 6728 6565 2e53 7472 696e 6728  tring(ee.String(
-00027090: 706d 2e67 6574 2831 2929 2e73 706c 6974  pm.get(1)).split
-000270a0: 2827 5f27 292e 6765 7428 3029 290d 0a20  ('_').get(0)).. 
-000270b0: 2020 2073 6967 6e20 3d20 6565 2e4e 756d     sign = ee.Num
-000270c0: 6265 7228 6565 2e44 6963 7469 6f6e 6172  ber(ee.Dictionar
-000270d0: 7928 6368 616e 6765 4469 7244 6963 7429  y(changeDirDict)
-000270e0: 2e67 6574 286f 7574 4e61 6d65 2929 2e6d  .get(outName)).m
-000270f0: 756c 7469 706c 7928 2d31 290d 0a0d 0a20  ultiply(-1).... 
-00027100: 2020 2061 6d70 6c69 7475 6465 203d 2068     amplitude = h
-00027110: 6172 6d43 6f65 6666 732e 7365 6c65 6374  armCoeffs.select
-00027120: 285b 315d 292e 6879 706f 7428 6861 726d  ([1]).hypot(harm
-00027130: 436f 6566 6673 2e73 656c 6563 7428 5b30  Coeffs.select([0
-00027140: 5d29 295c 0d0a 2020 2020 2020 2020 2020  ]))\..          
-00027150: 2020 2020 2e6d 756c 7469 706c 7928 3229      .multiply(2)
-00027160: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-00027170: 202e 7265 6e61 6d65 285b 6f75 744e 616d   .rename([outNam
-00027180: 652e 6361 7428 275f 616d 706c 6974 7564  e.cat('_amplitud
-00027190: 6527 295d 290d 0a20 2020 2070 6861 7365  e')])..    phase
-000271a0: 203d 2068 6172 6d43 6f65 6666 732e 7365   = harmCoeffs.se
-000271b0: 6c65 6374 285b 305d 292e 6174 616e 3228  lect([0]).atan2(
-000271c0: 6861 726d 436f 6566 6673 2e73 656c 6563  harmCoeffs.selec
-000271d0: 7428 5b31 5d29 295c 0d0a 2020 2020 2020  t([1]))\..      
-000271e0: 2020 2020 2020 2020 2e75 6e69 7453 6361          .unitSca
-000271f0: 6c65 282d 6d61 7468 2e70 692c 206d 6174  le(-math.pi, mat
-00027200: 682e 7069 295c 0d0a 2020 2020 2020 2020  h.pi)\..        
-00027210: 2020 2020 2020 2e72 656e 616d 6528 5b6f        .rename([o
-00027220: 7574 4e61 6d65 2e63 6174 2827 5f70 6861  utName.cat('_pha
-00027230: 7365 2729 5d29 0d0a 0d0a 2020 2020 2347  se')])....    #G
-00027240: 6574 2070 6561 6b20 6461 7465 2069 6e66  et peak date inf
-00027250: 6f0d 0a20 2020 2070 6561 6b44 6174 6520  o..    peakDate 
-00027260: 3d20 6765 7450 6561 6b44 6174 6528 6861  = getPeakDate(ha
-00027270: 726d 436f 6566 6673 2c73 6967 6e29 0d0a  rmCoeffs,sign)..
-00027280: 2020 2020 7065 616b 4461 7465 4261 6e64      peakDateBand
-00027290: 4e61 6d65 7320 3d20 7065 616b 4461 7465  Names = peakDate
-000272a0: 2e62 616e 644e 616d 6573 2829 0d0a 2020  .bandNames()..  
-000272b0: 2020 7065 616b 4461 7465 4261 6e64 4e61    peakDateBandNa
-000272c0: 6d65 7320 3d20 7065 616b 4461 7465 4261  mes = peakDateBa
-000272d0: 6e64 4e61 6d65 732e 6d61 7028 6c61 6d62  ndNames.map(lamb
-000272e0: 6461 2062 6e3a 206f 7574 4e61 6d65 2e63  da bn: outName.c
-000272f0: 6174 2865 652e 5374 7269 6e67 2827 5f27  at(ee.String('_'
-00027300: 292e 6361 7428 6565 2e53 7472 696e 6728  ).cat(ee.String(
-00027310: 626e 2929 2929 0d0a 0d0a 2020 2020 2347  bn))))....    #G
-00027320: 6574 2074 6865 206c 6566 7420 7375 6d0d  et the left sum.
-00027330: 0a20 2020 206c 6566 7453 756d 203d 2067  .    leftSum = g
-00027340: 6574 4172 6561 556e 6465 7243 7572 7665  etAreaUnderCurve
-00027350: 2868 6172 6d43 6f65 6666 732c 7430 2c74  (harmCoeffs,t0,t
-00027360: 3129 0d0a 2020 2020 6c65 6674 5375 6d42  1)..    leftSumB
-00027370: 616e 644e 616d 6573 203d 206c 6566 7453  andNames = leftS
-00027380: 756d 2e62 616e 644e 616d 6573 2829 0d0a  um.bandNames()..
-00027390: 2020 2020 6c65 6674 5375 6d42 616e 644e      leftSumBandN
-000273a0: 616d 6573 203d 206c 6566 7453 756d 4261  ames = leftSumBa
-000273b0: 6e64 4e61 6d65 732e 6d61 7028 6c61 6d62  ndNames.map(lamb
-000273c0: 6461 2062 6e3a 206f 7574 4e61 6d65 2e63  da bn: outName.c
-000273d0: 6174 2865 652e 5374 7269 6e67 2827 5f27  at(ee.String('_'
-000273e0: 292e 6361 7428 6565 2e53 7472 696e 6728  ).cat(ee.String(
-000273f0: 626e 2929 2929 0d0a 0d0a 2020 2020 7265  bn))))....    re
-00027400: 7475 726e 2061 6d70 6c69 7475 6465 5c0d  turn amplitude\.
-00027410: 0a20 2020 2020 2020 2020 2020 202e 6164  .            .ad
-00027420: 6442 616e 6473 2870 6861 7365 295c 0d0a  dBands(phase)\..
-00027430: 2020 2020 2020 2020 2020 2020 2e61 6464              .add
-00027440: 4261 6e64 7328 7065 616b 4461 7465 2e72  Bands(peakDate.r
-00027450: 656e 616d 6528 7065 616b 4461 7465 4261  ename(peakDateBa
-00027460: 6e64 4e61 6d65 7329 295c 0d0a 2020 2020  ndNames))\..    
-00027470: 2020 2020 2020 2020 2e61 6464 4261 6e64          .addBand
-00027480: 7328 6c65 6674 5375 6d2e 7265 6e61 6d65  s(leftSum.rename
-00027490: 286c 6566 7453 756d 4261 6e64 4e61 6d65  (leftSumBandName
-000274a0: 7329 290d 0a0d 0a0d 0a0d 0a20 2023 436f  s))........  #Co
-000274b0: 6e76 6572 7420 746f 2061 6e20 696d 6167  nvert to an imag
-000274c0: 650d 0a20 2070 6861 7365 416d 706c 6974  e..  phaseAmplit
-000274d0: 7564 6520 3d70 6172 7365 644d 6f64 656c  ude =parsedModel
-000274e0: 2e6d 6170 2870 6170 4765 7474 6572 290d  .map(papGetter).
-000274f0: 0a0d 0a20 2070 6861 7365 416d 706c 6974  ...  phaseAmplit
-00027500: 7564 6520 3d20 6565 2e49 6d61 6765 436f  ude = ee.ImageCo
-00027510: 6c6c 6563 7469 6f6e 2e66 726f 6d49 6d61  llection.fromIma
-00027520: 6765 7328 7068 6173 6541 6d70 6c69 7475  ges(phaseAmplitu
-00027530: 6465 290d 0a0d 0a20 2070 6861 7365 416d  de)....  phaseAm
-00027540: 706c 6974 7564 6520 3d20 6565 2e49 6d61  plitude = ee.Ima
-00027550: 6765 2863 6f6c 6c65 6374 696f 6e54 6f49  ge(collectionToI
-00027560: 6d61 6765 2870 6861 7365 416d 706c 6974  mage(phaseAmplit
-00027570: 7564 6529 292e 666c 6f61 7428 295c 0d0a  ude)).float()\..
-00027580: 2020 2020 2020 2020 2e63 6f70 7950 726f          .copyPro
-00027590: 7065 7274 6965 7328 636f 6566 6673 2c5b  perties(coeffs,[
-000275a0: 2773 7973 7465 6d3a 7469 6d65 5f73 7461  'system:time_sta
-000275b0: 7274 275d 290d 0a20 2023 7072 696e 7428  rt'])..  #print(
-000275c0: 2770 6127 2c70 6861 7365 416d 706c 6974  'pa',phaseAmplit
-000275d0: 7564 6529 3b0d 0a20 2072 6574 7572 6e20  ude);..  return 
-000275e0: 7068 6173 6541 6d70 6c69 7475 6465 3b0d  phaseAmplitude;.
-000275f0: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
-00027600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027630: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
-00027640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027680: 2323 2323 2323 230d 0a23 4675 6e63 7469  #######..#Functi
-00027690: 6f6e 2066 6f72 2061 7070 6c79 696e 6720  on for applying 
-000276a0: 6861 726d 6f6e 6963 2072 6567 7265 7373  harmonic regress
-000276b0: 696f 6e20 6d6f 6465 6c20 746f 2073 6574  ion model to set
-000276c0: 206f 6620 7072 6564 6963 746f 7220 7365   of predictor se
-000276d0: 7473 0d0a 6465 6620 6e65 7750 7265 6469  ts..def newPredi
-000276e0: 6374 2863 6f65 6666 732c 6861 726d 6f6e  ct(coeffs,harmon
-000276f0: 6963 7329 3a0d 0a20 2023 5061 7273 6520  ics):..  #Parse 
-00027700: 7468 6520 6d6f 6465 6c0d 0a20 2062 616e  the model..  ban
-00027710: 644e 616d 6573 203d 2063 6f65 6666 732e  dNames = coeffs.
-00027720: 6261 6e64 4e61 6d65 7328 290d 0a20 2062  bandNames()..  b
-00027730: 616e 644e 756d 6265 7220 3d20 6261 6e64  andNumber = band
-00027740: 4e61 6d65 732e 6c65 6e67 7468 2829 0d0a  Names.length()..
-00027750: 2020 6e6f 4465 7065 6e64 656e 7473 203d    noDependents =
-00027760: 2065 652e 4e75 6d62 6572 2863 6f65 6666   ee.Number(coeff
-00027770: 732e 6765 7428 276e 6f44 6570 656e 6465  s.get('noDepende
-00027780: 6e74 7327 2929 0d0a 2020 6d6f 6465 6c4c  nts'))..  modelL
-00027790: 656e 6774 6820 3d20 6565 2e4e 756d 6265  ength = ee.Numbe
-000277a0: 7228 636f 6566 6673 2e67 6574 2827 6d6f  r(coeffs.get('mo
-000277b0: 6465 6c4c 656e 6774 6827 2929 0d0a 2020  delLength'))..  
-000277c0: 696e 7465 7263 6570 7442 616e 6473 203d  interceptBands =
-000277d0: 2065 652e 4c69 7374 2e73 6571 7565 6e63   ee.List.sequenc
-000277e0: 6528 302c 6261 6e64 4e75 6d62 6572 2e73  e(0,bandNumber.s
-000277f0: 7562 7472 6163 7428 3129 2c6d 6f64 656c  ubtract(1),model
-00027800: 4c65 6e67 7468 290d 0a20 2074 696d 6542  Length)..  timeB
-00027810: 616e 6420 3d20 6565 2e4c 6973 7428 6861  and = ee.List(ha
-00027820: 726d 6f6e 6963 732e 6765 7428 2769 6e64  rmonics.get('ind
-00027830: 4261 6e64 4e61 6d65 7327 2929 2e67 6574  BandNames')).get
-00027840: 2830 290d 0a20 2061 6374 7561 6c42 616e  (0)..  actualBan
-00027850: 6473 203d 2068 6172 6d6f 6e69 6373 2e67  ds = harmonics.g
-00027860: 6574 2827 6465 7042 616e 644e 756d 6265  et('depBandNumbe
-00027870: 7273 2729 0d0a 2020 696e 6442 616e 6473  rs')..  indBands
-00027880: 203d 2068 6172 6d6f 6e69 6373 2e67 6574   = harmonics.get
-00027890: 2827 696e 6442 616e 644e 756d 6265 7273  ('indBandNumbers
-000278a0: 2729 0d0a 2020 696e 6442 616e 644e 616d  ')..  indBandNam
-000278b0: 6573 203d 2065 652e 4c69 7374 2868 6172  es = ee.List(har
-000278c0: 6d6f 6e69 6373 2e67 6574 2827 696e 6442  monics.get('indB
-000278d0: 616e 644e 616d 6573 2729 290d 0a20 2064  andNames'))..  d
-000278e0: 6570 4261 6e64 4e61 6d65 7320 3d20 6565  epBandNames = ee
-000278f0: 2e4c 6973 7428 6861 726d 6f6e 6963 732e  .List(harmonics.
-00027900: 6765 7428 2764 6570 4261 6e64 4e61 6d65  get('depBandName
-00027910: 7327 2929 0d0a 2020 7072 6564 6963 7465  s'))..  predicte
-00027920: 6442 616e 644e 616d 6573 203d 2064 6570  dBandNames = dep
-00027930: 4261 6e64 4e61 6d65 732e 6d61 7028 6c61  BandNames.map(la
-00027940: 6d62 6461 2064 6570 626e 6d73 3a65 652e  mbda depbnms:ee.
-00027950: 5374 7269 6e67 2864 6570 626e 6d73 292e  String(depbnms).
-00027960: 6361 7428 275f 7072 6564 6963 7465 6427  cat('_predicted'
-00027970: 2929 0d0a 2020 7072 6564 6963 7465 6442  ))..  predictedB
-00027980: 616e 644e 756d 6265 7273 203d 2065 652e  andNumbers = ee.
-00027990: 4c69 7374 2e73 6571 7565 6e63 6528 302c  List.sequence(0,
-000279a0: 7072 6564 6963 7465 6442 616e 644e 616d  predictedBandNam
-000279b0: 6573 2e6c 656e 6774 6828 292e 7375 6274  es.length().subt
-000279c0: 7261 6374 2831 2929 0d0a 0d0a 2020 6d6f  ract(1))....  mo
-000279d0: 6465 6c73 203d 2065 652e 4c69 7374 2e73  dels = ee.List.s
-000279e0: 6571 7565 6e63 6528 302c 6e6f 4465 7065  equence(0,noDepe
-000279f0: 6e64 656e 7473 2e73 7562 7472 6163 7428  ndents.subtract(
-00027a00: 3129 290d 0a20 2064 6566 206d 6e47 6574  1))..  def mnGet
-00027a10: 7465 7228 6d6e 293a 0d0a 2020 2020 6d6e  ter(mn):..    mn
-00027a20: 203d 2065 652e 4e75 6d62 6572 286d 6e29   = ee.Number(mn)
-00027a30: 0d0a 2020 2020 7265 7475 726e 2062 616e  ..    return ban
-00027a40: 644e 616d 6573 2e73 6c69 6365 286d 6e2e  dNames.slice(mn.
-00027a50: 6d75 6c74 6970 6c79 286d 6f64 656c 4c65  multiply(modelLe
-00027a60: 6e67 7468 292c 6d6e 2e6d 756c 7469 706c  ngth),mn.multipl
-00027a70: 7928 6d6f 6465 6c4c 656e 6774 6829 2e61  y(modelLength).a
-00027a80: 6464 286d 6f64 656c 4c65 6e67 7468 2929  dd(modelLength))
-00027a90: 0d0a 0d0a 2020 7061 7273 6564 4d6f 6465  ....  parsedMode
-00027aa0: 6c20 3d6d 6f64 656c 732e 6d61 7028 6d6e  l =models.map(mn
-00027ab0: 4765 7474 6572 290d 0a0d 0a20 2023 7072  Getter)....  #pr
-00027ac0: 696e 7428 2750 6172 7365 6420 6861 726d  int('Parsed harm
-00027ad0: 6f6e 6963 2072 6567 7265 7373 696f 6e20  onic regression 
-00027ae0: 6d6f 6465 6c27 2c70 6172 7365 644d 6f64  model',parsedMod
-00027af0: 656c 2c70 7265 6469 6374 6564 4261 6e64  el,predictedBand
-00027b00: 4e61 6d65 7329 0d0a 0d0a 2020 2341 7070  Names)....  #App
-00027b10: 6c79 2070 6172 7365 6420 6d6f 6465 6c0d  ly parsed model.
-00027b20: 0a20 2064 6566 2070 7265 6447 6574 7465  .  def predGette
-00027b30: 7228 696d 6729 3a0d 0a20 2020 2074 696d  r(img):..    tim
-00027b40: 6520 3d20 696d 672e 7365 6c65 6374 2874  e = img.select(t
-00027b50: 696d 6542 616e 6429 0d0a 2020 2020 6163  imeBand)..    ac
-00027b60: 7475 616c 203d 2069 6d67 2e73 656c 6563  tual = img.selec
-00027b70: 7428 6163 7475 616c 4261 6e64 7329 2e66  t(actualBands).f
-00027b80: 6c6f 6174 2829 0d0a 2020 2020 7072 6564  loat()..    pred
-00027b90: 6963 746f 7242 616e 6473 203d 2069 6d67  ictorBands = img
-00027ba0: 2e73 656c 6563 7428 696e 6442 616e 644e  .select(indBandN
-00027bb0: 616d 6573 290d 0a0d 0a20 2020 2023 4974  ames)....    #It
-00027bc0: 6572 6174 6520 6163 726f 7373 2065 6163  erate across eac
-00027bd0: 6820 6d6f 6465 6c20 666f 7220 6561 6368  h model for each
-00027be0: 2064 6570 656e 6465 6e74 2076 6172 6961   dependent varia
-00027bf0: 626c 650d 0a20 2020 2064 6566 2070 6d47  ble..    def pmG
-00027c00: 6574 7465 7228 706d 293a 0d0a 2020 2020  etter(pm):..    
-00027c10: 2020 706d 203d 2065 652e 4c69 7374 2870    pm = ee.List(p
-00027c20: 6d29 0d0a 2020 2020 2020 6d6f 6465 6c43  m)..      modelC
-00027c30: 6f65 6666 7320 3d20 636f 6566 6673 2e73  oeffs = coeffs.s
-00027c40: 656c 6563 7428 706d 290d 0a20 2020 2020  elect(pm)..     
-00027c50: 206f 7574 4e61 6d65 203d 2065 652e 5374   outName = ee.St
-00027c60: 7269 6e67 2870 6d2e 6765 7428 3129 292e  ring(pm.get(1)).
-00027c70: 6361 7428 275f 7072 6564 6963 7465 6427  cat('_predicted'
-00027c80: 290d 0a20 2020 2020 2069 6e74 6572 6365  )..      interce
-00027c90: 7074 203d 206d 6f64 656c 436f 6566 6673  pt = modelCoeffs
-00027ca0: 2e73 656c 6563 7428 6d6f 6465 6c43 6f65  .select(modelCoe
-00027cb0: 6666 732e 6261 6e64 4e61 6d65 7328 292e  ffs.bandNames().
-00027cc0: 736c 6963 6528 302c 3129 290d 0a20 2020  slice(0,1))..   
-00027cd0: 2020 206f 7468 6572 7320 3d20 6d6f 6465     others = mode
-00027ce0: 6c43 6f65 6666 732e 7365 6c65 6374 286d  lCoeffs.select(m
-00027cf0: 6f64 656c 436f 6566 6673 2e62 616e 644e  odelCoeffs.bandN
-00027d00: 616d 6573 2829 2e73 6c69 6365 2831 2c4e  ames().slice(1,N
-00027d10: 6f6e 6529 290d 0a0d 0a20 2020 2020 2070  one))....      p
-00027d20: 7265 6469 6374 6564 203d 2070 7265 6469  redicted = predi
-00027d30: 6374 6f72 4261 6e64 732e 6d75 6c74 6970  ctorBands.multip
-00027d40: 6c79 286f 7468 6572 7329 2e72 6564 7563  ly(others).reduc
-00027d50: 6528 6565 2e52 6564 7563 6572 2e73 756d  e(ee.Reducer.sum
-00027d60: 2829 292e 6164 6428 696e 7465 7263 6570  ()).add(intercep
-00027d70: 7429 2e66 6c6f 6174 2829 0d0a 2020 2020  t).float()..    
-00027d80: 2020 7265 7475 726e 2070 7265 6469 6374    return predict
-00027d90: 6564 2e66 6c6f 6174 2829 0d0a 0d0a 0d0a  ed.float()......
-00027da0: 2020 2020 7072 6564 6963 7465 644c 6973      predictedLis
-00027db0: 7420 3d70 6172 7365 644d 6f64 656c 2e6d  t =parsedModel.m
-00027dc0: 6170 2870 6d47 6574 7465 7229 0d0a 0d0a  ap(pmGetter)....
-00027dd0: 2020 2020 2343 6f6e 7665 7274 2074 6f20      #Convert to 
-00027de0: 616e 2069 6d61 6765 0d0a 2020 2020 7072  an image..    pr
-00027df0: 6564 6963 7465 644c 6973 7420 3d20 6565  edictedList = ee
-00027e00: 2e49 6d61 6765 436f 6c6c 6563 7469 6f6e  .ImageCollection
-00027e10: 2e66 726f 6d49 6d61 6765 7328 7072 6564  .fromImages(pred
-00027e20: 6963 7465 644c 6973 7429 0d0a 2020 2020  ictedList)..    
-00027e30: 7072 6564 6963 7465 6449 6d61 6765 203d  predictedImage =
-00027e40: 2063 6f6c 6c65 6374 696f 6e54 6f49 6d61   collectionToIma
-00027e50: 6765 2870 7265 6469 6374 6564 4c69 7374  ge(predictedList
-00027e60: 292e 7365 6c65 6374 2870 7265 6469 6374  ).select(predict
-00027e70: 6564 4261 6e64 4e75 6d62 6572 732c 7072  edBandNumbers,pr
-00027e80: 6564 6963 7465 6442 616e 644e 616d 6573  edictedBandNames
-00027e90: 290d 0a0d 0a20 2020 2023 5365 7420 736f  )....    #Set so
-00027ea0: 6d65 206d 6574 6164 6174 610d 0a20 2020  me metadata..   
-00027eb0: 206f 7574 203d 2061 6374 7561 6c2e 6164   out = actual.ad
-00027ec0: 6442 616e 6473 2870 7265 6469 6374 6564  dBands(predicted
-00027ed0: 496d 6167 652e 666c 6f61 7428 2929 5c0d  Image.float())\.
-00027ee0: 0a20 2020 202e 636f 7079 5072 6f70 6572  .    .copyProper
-00027ef0: 7469 6573 2869 6d67 2c5b 2773 7973 7465  ties(img,['syste
-00027f00: 6d3a 7469 6d65 5f73 7461 7274 272c 2773  m:time_start','s
-00027f10: 7973 7465 6d3a 7469 6d65 5f65 6e64 275d  ystem:time_end']
-00027f20: 290d 0a20 2020 2072 6574 7572 6e20 6f75  )..    return ou
-00027f30: 740d 0a0d 0a20 2070 7265 6469 6374 6564  t....  predicted
-00027f40: 203d 6861 726d 6f6e 6963 732e 6d61 7028   =harmonics.map(
-00027f50: 7072 6564 4765 7474 6572 290d 0a0d 0a20  predGetter).... 
-00027f60: 2070 7265 6469 6374 6564 203d 2065 652e   predicted = ee.
-00027f70: 496d 6167 6543 6f6c 6c65 6374 696f 6e28  ImageCollection(
-00027f80: 7072 6564 6963 7465 6429 0d0a 0d0a 2020  predicted)....  
-00027f90: 234d 6170 2e61 6464 4c61 7965 7228 7072  #Map.addLayer(pr
-00027fa0: 6564 6963 7465 642c 7b7d 2c27 7072 6564  edicted,{},'pred
-00027fb0: 6963 7465 6427 2c46 616c 7365 290d 0a0d  icted',False)...
-00027fc0: 0a20 2072 6574 7572 6e20 7072 6564 6963  .  return predic
-00027fd0: 7465 640d 0a0d 0a23 2323 2323 2323 2323  ted....#########
-00027fe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027ff0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028020: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-00028030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028060: 2323 2323 2323 2323 2323 230d 0a23 4675  ###########..#Fu
-00028070: 6e63 7469 6f6e 2074 6f20 6765 7420 6120  nction to get a 
-00028080: 6475 6d6d 7920 696d 6167 6520 7374 6163  dummy image stac
-00028090: 6b20 666f 7220 7379 6e74 6865 7469 6320  k for synthetic 
-000280a0: 7469 6d65 2073 6572 6965 730d 0a64 6566  time series..def
-000280b0: 2067 6574 4461 7465 5374 6163 6b28 7374   getDateStack(st
-000280c0: 6172 7459 6561 722c 656e 6459 6561 722c  artYear,endYear,
-000280d0: 7374 6172 744a 756c 6961 6e2c 656e 644a  startJulian,endJ
-000280e0: 756c 6961 6e2c 6672 6571 7565 6e63 7929  ulian,frequency)
-000280f0: 3a0d 0a20 2079 6561 7273 203d 2065 652e  :..  years = ee.
-00028100: 4c69 7374 2e73 6571 7565 6e63 6528 7374  List.sequence(st
-00028110: 6172 7459 6561 722c 656e 6459 6561 7229  artYear,endYear)
-00028120: 0d0a 2020 6461 7465 7320 3d20 6565 2e4c  ..  dates = ee.L
-00028130: 6973 742e 7365 7175 656e 6365 2873 7461  ist.sequence(sta
-00028140: 7274 4a75 6c69 616e 2c65 6e64 4a75 6c69  rtJulian,endJuli
-00028150: 616e 2c66 7265 7175 656e 6379 290d 0a0d  an,frequency)...
-00028160: 0a20 2064 6566 2079 7247 6574 7465 7228  .  def yrGetter(
-00028170: 7972 293a 0d0a 2020 2020 6465 6620 6447  yr):..    def dG
-00028180: 6574 7465 7228 6429 3a0d 0a20 2020 2020  etter(d):..     
-00028190: 2072 6574 7572 6e20 6565 2e44 6174 652e   return ee.Date.
-000281a0: 6672 6f6d 594d 4428 7972 2c31 2c31 292e  fromYMD(yr,1,1).
-000281b0: 6164 7661 6e63 6528 642c 2764 6179 2729  advance(d,'day')
-000281c0: 0d0a 2020 2020 6473 203d 2064 6174 6573  ..    ds = dates
-000281d0: 2e6d 6170 2864 4765 7474 6572 290d 0a20  .map(dGetter).. 
-000281e0: 2020 2072 6574 7572 6e20 6473 0d0a 0d0a     return ds....
-000281f0: 2020 6461 7465 5365 7473 203d 2079 6561    dateSets = yea
-00028200: 7273 2e6d 6170 2879 7247 6574 7465 7229  rs.map(yrGetter)
-00028210: 0d0a 0d0a 2020 6c20 3d20 7261 6e67 6528  ....  l = range(
-00028220: 312c 6c65 6e28 696e 6465 784e 616d 6573  1,len(indexNames
-00028230: 292b 3129 0d0a 2020 6c20 3d20 5b69 2569  )+1)..  l = [i%i
-00028240: 2066 6f72 2069 2069 6e20 6c5d 0d0a 2020   for i in l]..  
-00028250: 6320 3d20 6565 2e49 6d61 6765 286c 292e  c = ee.Image(l).
-00028260: 7265 6e61 6d65 2869 6e64 6578 4e61 6d65  rename(indexName
-00028270: 7329 0d0a 2020 6320 3d20 632e 6469 7669  s)..  c = c.divi
-00028280: 6465 2863 290d 0a0d 0a20 2064 6174 6553  de(c)....  dateS
-00028290: 6574 7320 3d20 6461 7465 5365 7473 2e66  ets = dateSets.f
-000282a0: 6c61 7474 656e 2829 0d0a 0d0a 2020 6465  latten()....  de
-000282b0: 6620 6474 4765 7474 6572 2864 7429 3a0d  f dtGetter(dt):.
-000282c0: 0a20 2020 2064 7420 3d20 6565 2e44 6174  .    dt = ee.Dat
-000282d0: 6528 6474 290d 0a20 2020 2079 203d 2064  e(dt)..    y = d
-000282e0: 742e 6765 7428 2779 6561 7227 290d 0a20  t.get('year').. 
-000282f0: 2020 2064 203d 2064 742e 6765 7446 7261     d = dt.getFra
-00028300: 6374 696f 6e28 2779 6561 7227 290d 0a20  ction('year').. 
-00028310: 2020 2069 203d 2065 652e 496d 6167 6528     i = ee.Image(
-00028320: 792e 6164 6428 6429 292e 666c 6f61 7428  y.add(d)).float(
-00028330: 292e 7365 6c65 6374 285b 305d 2c5b 2779  ).select([0],['y
-00028340: 6561 7227 5d29 0d0a 0d0a 2020 2020 6920  ear'])....    i 
-00028350: 3d20 632e 6164 6442 616e 6473 2869 292e  = c.addBands(i).
-00028360: 666c 6f61 7428 295c 0d0a 2020 2020 2020  float()\..      
-00028370: 2e73 6574 2827 7379 7374 656d 3a74 696d  .set('system:tim
-00028380: 655f 7374 6172 7427 2c64 742e 6d69 6c6c  e_start',dt.mill
-00028390: 6973 2829 295c 0d0a 2020 2020 2020 2e73  is())\..      .s
-000283a0: 6574 2827 7379 7374 656d 3a74 696d 655f  et('system:time_
-000283b0: 656e 6427 2c64 742e 6164 7661 6e63 6528  end',dt.advance(
-000283c0: 6672 6571 7565 6e63 792c 2764 6179 2729  frequency,'day')
-000283d0: 2e6d 696c 6c69 7328 2929 0d0a 2020 2020  .millis())..    
-000283e0: 7265 7475 726e 2069 0d0a 2020 7374 6163  return i..  stac
-000283f0: 6b20 3d20 6461 7465 5365 7473 2e6d 6170  k = dateSets.map
-00028400: 2864 7447 6574 7465 7229 0d0a 2020 7374  (dtGetter)..  st
-00028410: 6163 6b20 3d20 6565 2e49 6d61 6765 436f  ack = ee.ImageCo
-00028420: 6c6c 6563 7469 6f6e 2e66 726f 6d49 6d61  llection.fromIma
-00028430: 6765 7328 7374 6163 6b29 0d0a 2020 7265  ges(stack)..  re
-00028440: 7475 726e 2073 7461 636b 0d0a 0d0a 2323  turn stack....##
-00028450: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028460: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028470: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028480: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028490: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
-000284a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000284b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000284c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000284d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000284e0: 2323 0d0a 6465 6620 6765 7448 6172 6d6f  ##..def getHarmo
-000284f0: 6e69 6343 6f65 6666 6963 6965 6e74 7341  nicCoefficientsA
-00028500: 6e64 4669 7428 616c 6c49 6d61 6765 732c  ndFit(allImages,
-00028510: 696e 6465 784e 616d 6573 2c77 6869 6368  indexNames,which
-00028520: 4861 726d 6f6e 6963 7320 3d20 5b32 5d2c  Harmonics = [2],
-00028530: 6465 7472 656e 6420 3d20 4661 6c73 6529  detrend = False)
-00028540: 3a0d 0a0d 0a20 2023 5365 6c65 6374 2064  :....  #Select d
-00028550: 6573 6972 6564 2062 616e 6473 0d0a 2020  esired bands..  
-00028560: 616c 6c49 6e64 6963 6573 203d 2061 6c6c  allIndices = all
-00028570: 496d 6167 6573 2e73 656c 6563 7428 696e  Images.select(in
-00028580: 6465 784e 616d 6573 290d 0a0d 0a20 2023  dexNames)....  #
-00028590: 4164 6420 6461 7465 2062 616e 640d 0a20  Add date band.. 
-000285a0: 2069 6620 6465 7472 656e 643a 0d0a 2020   if detrend:..  
-000285b0: 2020 616c 6c49 6e64 6963 6573 203d 2061    allIndices = a
-000285c0: 6c6c 496e 6469 6365 732e 6d61 7028 6164  llIndices.map(ad
-000285d0: 6444 6174 6542 616e 6429 0d0a 2020 656c  dDateBand)..  el
-000285e0: 7365 3a0d 0a20 2020 2061 6c6c 496e 6469  se:..    allIndi
-000285f0: 6365 7320 3d20 616c 6c49 6e64 6963 6573  ces = allIndices
-00028600: 2e6d 6170 2861 6464 5965 6172 4672 6163  .map(addYearFrac
-00028610: 7469 6f6e 4261 6e64 290d 0a0d 0a0d 0a20  tionBand)...... 
-00028620: 2023 4164 6420 696e 6465 7065 6e64 656e   #Add independen
-00028630: 7420 7072 6564 6963 746f 7273 2028 6861  t predictors (ha
-00028640: 726d 6f6e 6963 7329 0d0a 2020 7769 7468  rmonics)..  with
-00028650: 4861 726d 6f6e 6963 7320 3d20 6765 7448  Harmonics = getH
-00028660: 6172 6d6f 6e69 6373 3228 616c 6c49 6e64  armonics2(allInd
-00028670: 6963 6573 2c27 7965 6172 272c 7768 6963  ices,'year',whic
-00028680: 6848 6172 6d6f 6e69 6373 2c64 6574 7265  hHarmonics,detre
-00028690: 6e64 290d 0a20 2077 6974 6848 6172 6d6f  nd)..  withHarmo
-000286a0: 6e69 6373 426e 7320 3d20 6565 2e49 6d61  nicsBns = ee.Ima
-000286b0: 6765 2877 6974 6848 6172 6d6f 6e69 6373  ge(withHarmonics
-000286c0: 2e66 6972 7374 2829 292e 6261 6e64 4e61  .first()).bandNa
-000286d0: 6d65 7328 292e 736c 6963 6528 6c65 6e28  mes().slice(len(
-000286e0: 696e 6465 784e 616d 6573 292b 312c 4e6f  indexNames)+1,No
-000286f0: 6e65 290d 0a0d 0a20 2023 4f70 7469 6f6e  ne)....  #Option
-00028700: 616c 6c79 2063 6861 7274 2074 6865 2063  ally chart the c
-00028710: 6f6c 6c65 6374 696f 6e20 7769 7468 2068  ollection with h
-00028720: 6172 6d6f 6e69 6373 0d0a 0d0a 2020 2346  armonics....  #F
-00028730: 6974 2061 206c 696e 6561 7220 7265 6772  it a linear regr
-00028740: 6573 7369 6f6e 206d 6f64 656c 0d0a 2020  ession model..  
-00028750: 636f 6566 6673 203d 206e 6577 526f 6275  coeffs = newRobu
-00028760: 7374 4d75 6c74 6970 6c65 4c69 6e65 6172  stMultipleLinear
-00028770: 3228 7769 7468 4861 726d 6f6e 6963 7329  2(withHarmonics)
-00028780: 0d0a 0d0a 2020 2343 616e 2076 6973 7561  ....  #Can visua
-00028790: 6c69 7a65 2074 6865 2070 6861 7365 2061  lize the phase a
-000287a0: 6e64 2061 6d70 6c69 7475 6465 2069 6620  nd amplitude if 
-000287b0: 6f6e 6c79 2074 6865 2066 6972 7374 2028  only the first (
-000287c0: 5b32 5d29 2068 6172 6d6f 6e69 6320 6973  [2]) harmonic is
-000287d0: 2063 686f 7365 6e0d 0a20 2023 2069 6620   chosen..  # if 
-000287e0: 7768 6963 6848 6172 6d6f 6e69 6373 203d  whichHarmonics =
-000287f0: 3d20 327b 0d0a 2020 2320 2020 2070 6120  = 2{..  #    pa 
-00028800: 3d20 6765 7450 6861 7365 416d 706c 6974  = getPhaseAmplit
-00028810: 7564 6528 636f 6566 6673 293b 0d0a 2020  ude(coeffs);..  
-00028820: 2320 202f 2f20 5475 726e 2074 6865 2048  #  // Turn the H
-00028830: 5356 2064 6174 6120 696e 746f 2061 6e20  SV data into an 
-00028840: 5247 4220 696d 6167 6520 616e 6420 6164  RGB image and ad
-00028850: 6420 6974 2074 6f20 7468 6520 6d61 702e  d it to the map.
-00028860: 0d0a 2020 2320 2073 6561 736f 6e61 6c69  ..  #  seasonali
-00028870: 7479 203d 2070 612e 7365 6c65 6374 285b  ty = pa.select([
-00028880: 312c 305d 292e 6164 6442 616e 6473 2861  1,0]).addBands(a
-00028890: 6c6c 496e 6469 6365 732e 7365 6c65 6374  llIndices.select
-000288a0: 285b 696e 6465 784e 616d 6573 5b30 5d5d  ([indexNames[0]]
-000288b0: 292e 6d65 616e 2829 292e 6873 7654 6f52  ).mean()).hsvToR
-000288c0: 6762 2829 3b0d 0a20 2023 2020 2f2f 204d  gb();..  #  // M
-000288d0: 6170 2e61 6464 4c61 7965 7228 7365 6173  ap.addLayer(seas
-000288e0: 6f6e 616c 6974 792c 207b 7d2c 2027 5365  onality, {}, 'Se
-000288f0: 6173 6f6e 616c 6974 7927 293b 0d0a 2020  asonality');..  
-00028900: 2320 207d 0d0a 0d0a 0d0a 0d0a 2020 234d  #  }........  #M
-00028910: 6170 2e61 6464 4c61 7965 7228 636f 6566  ap.addLayer(coef
-00028920: 6673 2c7b 7d2c 2748 6172 6d6f 6e69 6320  fs,{},'Harmonic 
-00028930: 5265 6772 6573 7369 6f6e 2043 6f65 6666  Regression Coeff
-00028940: 6963 6965 6e74 7327 2c46 616c 7365 290d  icients',False).
-00028950: 0a20 2070 7265 6469 6374 6564 203d 206e  .  predicted = n
-00028960: 6577 5072 6564 6963 7428 636f 6566 6673  ewPredict(coeffs
-00028970: 2c77 6974 6848 6172 6d6f 6e69 6373 290d  ,withHarmonics).
-00028980: 0a20 2072 6574 7572 6e20 5b63 6f65 6666  .  return [coeff
-00028990: 732c 7072 6564 6963 7465 645d 0d0a 2323  s,predicted]..##
-000289a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000289b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000289c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000289d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000289e0: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
-000289f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028a10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028a20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028a30: 2323 0d0a 2353 696d 706c 6520 7072 6564  ##..#Simple pred
-00028a40: 6963 7420 6675 6e63 7469 6f6e 2066 6f72  ict function for
-00028a50: 2068 6172 6d6f 6e69 6320 636f 6566 6669   harmonic coeffi
-00028a60: 6369 656e 7473 0d0a 2345 7870 6563 7473  cients..#Expects
-00028a70: 2063 6f65 6666 7320 6672 6f6d 2067 6574   coeffs from get
-00028a80: 4861 726d 6f6e 6963 436f 6566 6669 6369  HarmonicCoeffici
-00028a90: 656e 7473 416e 6446 6974 2066 756e 6374  entsAndFit funct
-00028aa0: 696f 6e0d 0a23 4461 7465 2069 6d61 6765  ion..#Date image
-00028ab0: 2069 7320 6578 7065 6374 6564 2074 6f20   is expected to 
-00028ac0: 6265 2079 7979 792e 6464 2077 6865 7265  be yyyy.dd where
-00028ad0: 2064 6420 6973 2074 6865 2064 6179 206f   dd is the day o
-00028ae0: 6620 7965 6172 202f 2033 3635 2028 7072  f year / 365 (pr
-00028af0: 6f70 6f72 7469 6f6e 206f 6620 7965 6172  oportion of year
-00028b00: 290d 0a23 6578 2e20 7379 6e74 6849 6d61  )..#ex. synthIma
-00028b10: 6765 2863 6f65 6666 732c 6565 2e49 6d61  ge(coeffs,ee.Ima
-00028b20: 6765 285b 3230 3139 2e36 5d29 2c5b 2762  ge([2019.6]),['b
-00028b30: 6c75 6527 2c27 6772 6565 6e27 2c27 7265  lue','green','re
-00028b40: 6427 2c27 6e69 7227 2c27 7377 6972 3127  d','nir','swir1'
-00028b50: 2c27 7377 6972 3227 2c27 4e42 5227 2c27  ,'swir2','NBR','
-00028b60: 4e44 5649 275d 2c5b 322c 345d 2c74 7275  NDVI'],[2,4],tru
-00028b70: 6529 0d0a 6465 6620 7379 6e74 6849 6d61  e)..def synthIma
-00028b80: 6765 2863 6f65 6666 732c 6461 7465 496d  ge(coeffs,dateIm
-00028b90: 6167 652c 696e 6465 784e 616d 6573 2c68  age,indexNames,h
-00028ba0: 6172 6d6f 6e69 6373 2c64 6574 7265 6e64  armonics,detrend
-00028bb0: 293a 0d0a 2020 2353 6574 2075 7020 636f  ):..  #Set up co
-00028bc0: 6e73 7461 6e74 2069 6d61 6765 2074 6f20  nstant image to 
-00028bd0: 6d75 6c74 6970 6c79 2063 6f65 6666 7320  multiply coeffs 
-00028be0: 6279 0d0a 2020 636f 6e73 7449 6d61 6765  by..  constImage
-00028bf0: 203d 2065 652e 496d 6167 6528 3129 0d0a   = ee.Image(1)..
-00028c00: 2020 6966 2064 6574 7265 6e64 3a63 6f6e    if detrend:con
-00028c10: 7374 496d 6167 6520 3d20 636f 6e73 7449  stImage = constI
-00028c20: 6d61 6765 2e61 6464 4261 6e64 7328 6461  mage.addBands(da
-00028c30: 7465 496d 6167 6529 0d0a 2020 666f 7220  teImage)..  for 
-00028c40: 6861 726d 2069 6e20 6861 726d 6f6e 6963  harm in harmonic
-00028c50: 733a 0d0a 2020 2020 636f 6e73 7449 6d61  s:..    constIma
-00028c60: 6765 203d 2063 6f6e 7374 496d 6167 652e  ge = constImage.
-00028c70: 6164 6442 616e 6473 2865 652e 496d 6167  addBands(ee.Imag
-00028c80: 6528 5b64 6174 6549 6d61 6765 2e6d 756c  e([dateImage.mul
-00028c90: 7469 706c 7928 6861 726d 2a6d 6174 682e  tiply(harm*math.
-00028ca0: 7069 292e 7369 6e28 295d 292e 7265 6e61  pi).sin()]).rena
-00028cb0: 6d65 285b 277b 7d5f 7369 6e27 2e66 6f72  me(['{}_sin'.for
-00028cc0: 6d61 7428 6861 726d 2a31 3030 295d 2929  mat(harm*100)]))
-00028cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028ce0: 2020 2020 2020 200d 0a20 2066 6f72 2068         ..  for h
-00028cf0: 6172 6d20 696e 2068 6172 6d6f 6e69 6373  arm in harmonics
-00028d00: 3a0d 0a20 2020 2063 6f6e 7374 496d 6167  :..    constImag
-00028d10: 6520 3d20 636f 6e73 7449 6d61 6765 2e61  e = constImage.a
-00028d20: 6464 4261 6e64 7328 6565 2e49 6d61 6765  ddBands(ee.Image
-00028d30: 285b 6461 7465 496d 6167 652e 6d75 6c74  ([dateImage.mult
-00028d40: 6970 6c79 2868 6172 6d2a 6d61 7468 2e70  iply(harm*math.p
-00028d50: 6929 2e63 6f73 2829 5d29 2e72 656e 616d  i).cos()]).renam
-00028d60: 6528 5b27 7b7d 5f63 6f73 272e 666f 726d  e(['{}_cos'.form
-00028d70: 6174 2868 6172 6d2a 3130 3029 5d29 290d  at(harm*100)])).
-00028d80: 0a20 200d 0a20 2023 2063 6f65 6666 7373  .  ..  # coeffss
-00028d90: 426e 203d 2063 6f65 6666 732e 7365 6c65  Bn = coeffs.sele
-00028da0: 6374 2865 652e 5374 7269 6e67 2869 6e64  ct(ee.String(ind
-00028db0: 6578 4e61 6d65 735b 305d 292e 6361 7428  exNames[0]).cat(
-00028dc0: 275f 2e2a 2729 290d 0a20 2023 2070 7269  '_.*'))..  # pri
-00028dd0: 6e74 2863 6f6e 7374 496d 6167 652e 6261  nt(constImage.ba
-00028de0: 6e64 4e61 6d65 7328 292e 6765 7449 6e66  ndNames().getInf
-00028df0: 6f28 292c 636f 6566 6673 7342 6e2e 6261  o(),coeffssBn.ba
-00028e00: 6e64 4e61 6d65 7328 292e 6765 7449 6e66  ndNames().getInf
-00028e10: 6f28 2929 0d0a 2020 2350 7265 6469 6374  o())..  #Predict
-00028e20: 2076 616c 7565 7320 666f 7220 6561 6368   values for each
-00028e30: 2062 616e 640d 0a20 206f 7574 203d 2065   band..  out = e
-00028e40: 652e 496d 6167 6528 3129 3b0d 0a20 2064  e.Image(1);..  d
-00028e50: 6566 2070 7265 6469 6374 5772 6170 7065  ef predictWrappe
-00028e60: 7228 626e 2c6f 7574 293a 0d0a 2020 2020  r(bn,out):..    
-00028e70: 626e 203d 2065 652e 5374 7269 6e67 2862  bn = ee.String(b
-00028e80: 6e29 0d0a 2020 2020 2353 656c 6563 7420  n)..    #Select 
-00028e90: 636f 6566 6673 2066 6f72 2074 6861 7420  coeffs for that 
-00028ea0: 6261 6e64 0d0a 2020 2020 636f 6566 6673  band..    coeffs
-00028eb0: 7342 6e20 3d20 636f 6566 6673 2e73 656c  sBn = coeffs.sel
-00028ec0: 6563 7428 6565 2e53 7472 696e 6728 626e  ect(ee.String(bn
-00028ed0: 292e 6361 7428 275f 2e2a 2729 290d 0a20  ).cat('_.*')).. 
-00028ee0: 2020 2070 7265 6469 6374 6564 203d 2063     predicted = c
-00028ef0: 6f6e 7374 496d 6167 652e 6d75 6c74 6970  onstImage.multip
-00028f00: 6c79 2863 6f65 6666 7373 426e 292e 7265  ly(coeffssBn).re
-00028f10: 6475 6365 2827 7375 6d27 292e 7265 6e61  duce('sum').rena
-00028f20: 6d65 2862 6e29 0d0a 2020 2020 7265 7475  me(bn)..    retu
-00028f30: 726e 2065 652e 496d 6167 6528 6f75 7429  rn ee.Image(out)
-00028f40: 2e61 6464 4261 6e64 7328 7072 6564 6963  .addBands(predic
-00028f50: 7465 6429 0d0a 0d0a 2020 6f75 7420 3d20  ted)....  out = 
-00028f60: 6565 2e49 6d61 6765 2865 652e 4c69 7374  ee.Image(ee.List
-00028f70: 2869 6e64 6578 4e61 6d65 7329 2e69 7465  (indexNames).ite
-00028f80: 7261 7465 2870 7265 6469 6374 5772 6170  rate(predictWrap
-00028f90: 7065 722c 6f75 7429 293b 0d0a 0d0a 2020  per,out));....  
-00028fa0: 6f75 7420 3d20 6f75 742e 7365 6c65 6374  out = out.select
-00028fb0: 2865 652e 4c69 7374 2e73 6571 7565 6e63  (ee.List.sequenc
-00028fc0: 6528 312c 206f 7574 2e62 616e 644e 616d  e(1, out.bandNam
-00028fd0: 6573 2829 2e73 697a 6528 292e 7375 6274  es().size().subt
-00028fe0: 7261 6374 2831 2929 290d 0a0d 0a20 2072  ract(1)))....  r
-00028ff0: 6574 7572 6e20 6f75 740d 0a23 2323 2323  eturn out..#####
-00029000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029040: 0d0a 2357 7261 7070 6572 2066 756e 6374  ..#Wrapper funct
-00029050: 696f 6e20 746f 2067 6574 2063 6c69 6d61  ion to get clima
-00029060: 7465 2064 6174 610d 0a23 2053 7570 706f  te data..# Suppo
-00029070: 7274 733a 0d0a 2320 4e41 5341 2f4f 524e  rts:..# NASA/ORN
-00029080: 4c2f 4441 594d 4554 5f56 330d 0a23 204e  L/DAYMET_V3..# N
-00029090: 4153 412f 4f52 4e4c 2f44 4159 4d45 545f  ASA/ORNL/DAYMET_
-000290a0: 5634 0d0a 2320 5543 5342 2d43 4847 2f43  V4..# UCSB-CHG/C
-000290b0: 4849 5250 532f 4441 494c 5920 2870 7265  HIRPS/DAILY (pre
-000290c0: 6369 7069 7461 7469 6f6e 206f 6e6c 7929  cipitation only)
-000290d0: 0d0a 2361 6e64 2070 6f73 7369 626c 7920  ..#and possibly 
-000290e0: 6f74 6865 7273 0d0a 6465 6620 6765 7443  others..def getC
-000290f0: 6c69 6d61 7465 5772 6170 7065 7228 636f  limateWrapper(co
-00029100: 6c6c 6563 7469 6f6e 4e61 6d65 2c73 7475  llectionName,stu
-00029110: 6479 4172 6561 2c73 7461 7274 5965 6172  dyArea,startYear
-00029120: 2c65 6e64 5965 6172 2c73 7461 7274 4a75  ,endYear,startJu
-00029130: 6c69 616e 2c65 6e64 4a75 6c69 616e 2c74  lian,endJulian,t
-00029140: 696d 6562 7566 6665 722c 7765 6967 6874  imebuffer,weight
-00029150: 732c 636f 6d70 6f73 6974 696e 6752 6564  s,compositingRed
-00029160: 7563 6572 2c65 7870 6f72 7443 6f6d 706f  ucer,exportCompo
-00029170: 7369 7465 7320 3d20 4661 6c73 652c 6578  sites = False,ex
-00029180: 706f 7274 5061 7468 526f 6f74 203d 204e  portPathRoot = N
-00029190: 6f6e 652c 6372 7320 3d20 4e6f 6e65 2c74  one,crs = None,t
-000291a0: 7261 6e73 666f 726d 203d 204e 6f6e 652c  ransform = None,
-000291b0: 7363 616c 6520 3d20 4e6f 6e65 2c65 7870  scale = None,exp
-000291c0: 6f72 7442 616e 6473 203d 204e 6f6e 6529  ortBands = None)
-000291d0: 3a0d 0a20 2061 7267 7320 3d20 666f 726d  :..  args = form
-000291e0: 6174 4172 6773 286c 6f63 616c 7328 2929  atArgs(locals())
-000291f0: 0d0a 2020 6966 2027 6172 6773 2720 696e  ..  if 'args' in
-00029200: 2061 7267 732e 6b65 7973 2829 3a0d 0a20   args.keys():.. 
-00029210: 2020 2064 656c 2061 7267 735b 2761 7267     del args['arg
-00029220: 7327 5d0d 0a20 2070 7269 6e74 2861 7267  s']..  print(arg
-00029230: 7329 0d0a 0d0a 2020 2350 7265 7061 7265  s)....  #Prepare
-00029240: 2064 6174 6573 0d0a 2020 2357 7261 7020   dates..  #Wrap 
-00029250: 7468 6520 6461 7465 7320 6966 206e 6565  the dates if nee
-00029260: 6465 640d 0a20 2077 7261 704f 6666 7365  ded..  wrapOffse
-00029270: 7420 3d20 300d 0a20 2069 6620 7374 6172  t = 0..  if star
-00029280: 744a 756c 6961 6e20 3e20 656e 644a 756c  tJulian > endJul
-00029290: 6961 6e3a 0d0a 2020 2020 7772 6170 4f66  ian:..    wrapOf
-000292a0: 6673 6574 203d 2033 3635 0d0a 0d0a 2020  fset = 365....  
-000292b0: 7374 6172 7444 6174 6520 3d20 6565 2e44  startDate = ee.D
-000292c0: 6174 652e 6672 6f6d 594d 4428 7374 6172  ate.fromYMD(star
-000292d0: 7459 6561 722c 312c 3129 2e61 6476 616e  tYear,1,1).advan
-000292e0: 6365 2873 7461 7274 4a75 6c69 616e 2d31  ce(startJulian-1
-000292f0: 2c27 6461 7927 290d 0a20 2065 6e64 4461  ,'day')..  endDa
-00029300: 7465 203d 2065 652e 4461 7465 2e66 726f  te = ee.Date.fro
-00029310: 6d59 4d44 2865 6e64 5965 6172 2c31 2c31  mYMD(endYear,1,1
-00029320: 292e 6164 7661 6e63 6528 656e 644a 756c  ).advance(endJul
-00029330: 6961 6e2d 312b 7772 6170 4f66 6673 6574  ian-1+wrapOffset
-00029340: 2c27 6461 7927 290d 0a20 2070 7269 6e74  ,'day')..  print
-00029350: 2827 5374 6172 7420 616e 6420 656e 6420  ('Start and end 
-00029360: 6461 7465 733a 272c 2073 7461 7274 4461  dates:', startDa
-00029370: 7465 2e66 6f72 6d61 7428 2759 5959 592d  te.format('YYYY-
-00029380: 4d4d 2d64 6427 292e 6765 7449 6e66 6f28  MM-dd').getInfo(
-00029390: 292c 2065 6e64 4461 7465 2e66 6f72 6d61  ), endDate.forma
-000293a0: 7428 2759 5959 592d 4d4d 2d64 6427 292e  t('YYYY-MM-dd').
-000293b0: 6765 7449 6e66 6f28 2929 0d0a 2020 7072  getInfo())..  pr
-000293c0: 696e 7428 274a 756c 6961 6e20 6461 7973  int('Julian days
-000293d0: 2061 7265 3a27 2c73 7461 7274 4a75 6c69   are:',startJuli
-000293e0: 616e 2c65 6e64 4a75 6c69 616e 290d 0a0d  an,endJulian)...
-000293f0: 0a20 2023 4765 7420 636c 696d 6174 6520  .  #Get climate 
-00029400: 6461 7461 0d0a 2020 6320 3d20 6565 2e49  data..  c = ee.I
-00029410: 6d61 6765 436f 6c6c 6563 7469 6f6e 2863  mageCollection(c
-00029420: 6f6c 6c65 6374 696f 6e4e 616d 6529 5c0d  ollectionName)\.
-00029430: 0a20 2020 2020 2020 2020 2020 2e66 696c  .           .fil
-00029440: 7465 7242 6f75 6e64 7328 7374 7564 7941  terBounds(studyA
-00029450: 7265 6129 5c0d 0a20 2020 2020 2020 2020  rea)\..         
-00029460: 2020 2e66 696c 7465 7244 6174 6528 7374    .filterDate(st
-00029470: 6172 7444 6174 652c 656e 6444 6174 652e  artDate,endDate.
-00029480: 6164 7661 6e63 6528 312c 2764 6179 2729  advance(1,'day')
-00029490: 295c 0d0a 2020 2020 2020 2020 2020 202e  )\..           .
-000294a0: 6669 6c74 6572 2865 652e 4669 6c74 6572  filter(ee.Filter
-000294b0: 2e63 616c 656e 6461 7252 616e 6765 2873  .calendarRange(s
-000294c0: 7461 7274 4a75 6c69 616e 2c65 6e64 4a75  tartJulian,endJu
-000294d0: 6c69 616e 2929 0d0a 0d0a 2020 2353 6574  lian))....  #Set
-000294e0: 2074 6f20 6170 7072 6f70 7269 6174 6520   to appropriate 
-000294f0: 7265 7361 6d70 6c69 6e67 206d 6574 686f  resampling metho
-00029500: 640d 0a20 2063 203d 2063 2e6d 6170 286c  d..  c = c.map(l
-00029510: 616d 6264 6120 696d 673a 2069 6d67 2e72  ambda img: img.r
-00029520: 6573 616d 706c 6528 2762 6963 7562 6963  esample('bicubic
-00029530: 2729 290d 0a20 204d 6170 2e61 6464 4c61  '))..  Map.addLa
-00029540: 7965 7228 632c 7b7d 2c27 5261 7720 436c  yer(c,{},'Raw Cl
-00029550: 696d 6174 6527 2c46 616c 7365 290d 0a0d  imate',False)...
-00029560: 0a20 2023 4372 6561 7465 2063 6f6d 706f  .  #Create compo
-00029570: 7369 7465 2074 696d 6520 7365 7269 6573  site time series
-00029580: 0d0a 2020 7473 203d 2063 6f6d 706f 7369  ..  ts = composi
-00029590: 7465 5469 6d65 5365 7269 6573 2863 2c73  teTimeSeries(c,s
-000295a0: 7461 7274 5965 6172 2c65 6e64 5965 6172  tartYear,endYear
-000295b0: 2c73 7461 7274 4a75 6c69 616e 2c65 6e64  ,startJulian,end
-000295c0: 4a75 6c69 616e 2c74 696d 6562 7566 6665  Julian,timebuffe
-000295d0: 722c 7765 6967 6874 732c 4e6f 6e65 2c63  r,weights,None,c
-000295e0: 6f6d 706f 7369 7469 6e67 5265 6475 6365  ompositingReduce
-000295f0: 7229 0d0a 2020 7473 203d 2065 652e 496d  r)..  ts = ee.Im
-00029600: 6167 6543 6f6c 6c65 6374 696f 6e28 7473  ageCollection(ts
-00029610: 2e6d 6170 286c 616d 6264 6120 6920 3a20  .map(lambda i : 
-00029620: 692e 666c 6f61 7428 2929 290d 0a0d 0a20  i.float())).... 
-00029630: 2023 4578 706f 7274 2063 6f6d 706f 7369   #Export composi
-00029640: 7465 2063 6f6c 6c65 6374 696f 6e0d 0a20  te collection.. 
-00029650: 2069 6620 6578 706f 7274 436f 6d70 6f73   if exportCompos
-00029660: 6974 6573 3a0d 0a20 2020 2023 5365 7420  ites:..    #Set 
-00029670: 7570 2065 7870 6f72 7420 6261 6e64 7320  up export bands 
-00029680: 6966 206e 6f74 2073 7065 6369 6669 6564  if not specified
-00029690: 0d0a 2020 2020 6966 2065 7870 6f72 7442  ..    if exportB
-000296a0: 616e 6473 203d 3d20 4e6f 6e65 3a0d 0a20  ands == None:.. 
-000296b0: 2020 2020 2065 7870 6f72 7442 616e 6473       exportBands
-000296c0: 203d 2065 652e 4c69 7374 2865 652e 496d   = ee.List(ee.Im
-000296d0: 6167 6528 7473 2e66 6972 7374 2829 292e  age(ts.first()).
-000296e0: 6261 6e64 4e61 6d65 7328 2929 0d0a 0d0a  bandNames())....
-000296f0: 2020 2020 6578 706f 7274 436f 6c6c 6563      exportCollec
-00029700: 7469 6f6e 2865 7870 6f72 7450 6174 6852  tion(exportPathR
-00029710: 6f6f 742c 636f 6c6c 6563 7469 6f6e 4e61  oot,collectionNa
-00029720: 6d65 2e73 706c 6974 2827 2f27 295b 2d31  me.split('/')[-1
-00029730: 5d2c 7374 7564 7941 7265 612c 2063 7273  ],studyArea, crs
-00029740: 2c74 7261 6e73 666f 726d 2c73 6361 6c65  ,transform,scale
-00029750: 2c74 732c 7374 6172 7459 6561 722c 656e  ,ts,startYear,en
-00029760: 6459 6561 722c 7374 6172 744a 756c 6961  dYear,startJulia
-00029770: 6e2c 656e 644a 756c 6961 6e2c 636f 6d70  n,endJulian,comp
-00029780: 6f73 6974 696e 6752 6564 7563 6572 2c74  ositingReducer,t
-00029790: 696d 6562 7566 6665 722c 6578 706f 7274  imebuffer,export
-000297a0: 4261 6e64 7329 0d0a 0d0a 2020 7265 7475  Bands)....  retu
-000297b0: 726e 2074 7323 2323 230d 0a23 2323 2323  rn ts####..#####
-000297c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000297d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000297e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000297f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029800: 0d0a 2341 6464 7320 6162 736f 6c75 7465  ..#Adds absolute
-00029810: 2064 6966 6665 7265 6e63 6520 6672 6f6d   difference from
-00029820: 2061 2073 7065 6369 6669 6564 2062 616e   a specified ban
-00029830: 6420 7375 6d6d 6172 697a 6564 2062 7920  d summarized by 
-00029840: 6120 7072 6f76 6964 6564 2070 6572 6365  a provided perce
-00029850: 6e74 696c 650d 0a23 496e 7465 6e64 6564  ntile..#Intended
-00029860: 2066 6f72 2063 7573 746f 6d20 736f 7274   for custom sort
-00029870: 696e 6720 6163 726f 7373 2063 6f6c 6c65  ing across colle
-00029880: 6374 696f 6e73 0d0a 6465 6620 6164 6441  ctions..def addA
-00029890: 6273 4469 6666 2869 6e43 6f6c 6c65 6374  bsDiff(inCollect
-000298a0: 696f 6e2c 2071 7561 6c69 7479 4261 6e64  ion, qualityBand
-000298b0: 2c20 7065 7263 656e 7469 6c65 2c73 6967  , percentile,sig
-000298c0: 6e29 3a0d 0a20 2062 6573 7451 7561 6c69  n):..  bestQuali
-000298d0: 7479 203d 2069 6e43 6f6c 6c65 6374 696f  ty = inCollectio
-000298e0: 6e2e 7365 6c65 6374 285b 7175 616c 6974  n.select([qualit
-000298f0: 7942 616e 645d 292e 7265 6475 6365 2865  yBand]).reduce(e
-00029900: 652e 5265 6475 6365 722e 7065 7263 656e  e.Reducer.percen
-00029910: 7469 6c65 285b 7065 7263 656e 7469 6c65  tile([percentile
-00029920: 5d29 290d 0a20 2064 6566 2077 2869 6d61  ]))..  def w(ima
-00029930: 6765 293a 0d0a 2020 2020 6465 6c74 6120  ge):..    delta 
-00029940: 3d20 696d 6167 652e 7365 6c65 6374 285b  = image.select([
-00029950: 7175 616c 6974 7942 616e 645d 292e 7375  qualityBand]).su
-00029960: 6274 7261 6374 2862 6573 7451 7561 6c69  btract(bestQuali
-00029970: 7479 292e 6162 7328 292e 6d75 6c74 6970  ty).abs().multip
-00029980: 6c79 2873 6967 6e29 0d0a 2020 2020 7265  ly(sign)..    re
-00029990: 7475 726e 2069 6d61 6765 2e61 6464 4261  turn image.addBa
-000299a0: 6e64 7328 6465 6c74 612e 7365 6c65 6374  nds(delta.select
-000299b0: 285b 305d 2c20 5b27 6465 6c74 6127 5d29  ([0], ['delta'])
-000299c0: 290d 0a20 206f 7574 203d 2069 6e43 6f6c  )..  out = inCol
-000299d0: 6c65 6374 696f 6e2e 6d61 7028 7729 0d0a  lection.map(w)..
-000299e0: 2020 7265 7475 726e 206f 7574 0d0a 0d0a    return out....
-000299f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029a10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029a20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029a30: 2323 2323 230d 0a23 4d65 7468 6f64 2066  #####..#Method f
-00029a40: 6f72 2061 7070 6c79 696e 6720 7468 6520  or applying the 
-00029a50: 7175 616c 6974 794d 6f73 6169 6320 6675  qualityMosaic fu
-00029a60: 6e63 7469 6f6e 2075 7369 6e67 2061 2073  nction using a s
-00029a70: 7065 6369 6669 6564 2070 6572 6365 6e74  pecified percent
-00029a80: 696c 650d 0a23 5573 6566 756c 2077 6865  ile..#Useful whe
-00029a90: 6e20 7468 6520 6d61 7820 6f66 2074 6865  n the max of the
-00029aa0: 2071 7561 6c69 7479 2062 616e 6420 6973   quality band is
-00029ab0: 206e 6f74 2077 6861 7420 6973 2077 616e   not what is wan
-00029ac0: 7465 640d 0a64 6566 2063 7573 746f 6d51  ted..def customQ
-00029ad0: 7561 6c69 7479 4d6f 7361 6963 2869 6e43  ualityMosaic(inC
-00029ae0: 6f6c 6c65 6374 696f 6e2c 7175 616c 6974  ollection,qualit
-00029af0: 7942 616e 642c 7065 7263 656e 7469 6c65  yBand,percentile
-00029b00: 293a 0d0a 2020 2341 6464 2061 6e20 6162  ):..  #Add an ab
-00029b10: 736f 6c75 7465 2064 6966 6665 7265 6e63  solute differenc
-00029b20: 6520 6672 6f6d 2074 6865 2073 7065 6369  e from the speci
-00029b30: 6669 6564 2070 6572 6365 6e74 696c 650d  fied percentile.
-00029b40: 0a20 2023 5468 6973 2069 7320 696e 7665  .  #This is inve
-00029b50: 7274 6564 2066 6f72 2074 6865 2071 7561  rted for the qua
-00029b60: 6c69 7479 4d6f 7361 6963 2066 756e 6374  lityMosaic funct
-00029b70: 696f 6e20 746f 2070 726f 7065 726c 7920  ion to properly 
-00029b80: 7072 696f 7269 7469 7a65 0d0a 2020 696e  prioritize..  in
-00029b90: 436f 6c6c 6563 7469 6f6e 4465 6c74 6120  CollectionDelta 
-00029ba0: 3d20 6164 6441 6273 4469 6666 2869 6e43  = addAbsDiff(inC
-00029bb0: 6f6c 6c65 6374 696f 6e2c 2071 7561 6c69  ollection, quali
-00029bc0: 7479 4261 6e64 2c20 7065 7263 656e 7469  tyBand, percenti
-00029bd0: 6c65 2c2d 3129 0d0a 0d0a 2020 2341 7070  le,-1)....  #App
-00029be0: 6c79 2074 6865 2071 7561 6c69 7479 4d6f  ly the qualityMo
-00029bf0: 7361 6963 2066 756e 6374 696f 6e0d 0a20  saic function.. 
-00029c00: 2072 6574 7572 6e20 696e 436f 6c6c 6563   return inCollec
-00029c10: 7469 6f6e 4465 6c74 612e 7175 616c 6974  tionDelta.qualit
-00029c20: 794d 6f73 6169 6328 2764 656c 7461 2729  yMosaic('delta')
-00029c30: 0d0a 0d0a 2323 2323 2323 2323 2323 2323  ....############
-00029c40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029c50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029c60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029c70: 2323 2323 2323 2323 230d 0a23 4f6e 2d74  #########..#On-t
-00029c80: 6865 2d66 6c79 2062 6173 6963 2077 6174  he-fly basic wat
-00029c90: 6572 206d 6173 6b69 6e67 206d 6574 686f  er masking metho
-00029ca0: 640d 0a23 5468 6973 206d 6574 686f 6420  d..#This method 
-00029cb0: 6973 2075 7365 6420 746f 2070 726f 7669  is used to provi
-00029cc0: 6465 2061 2074 696d 652d 7365 6e73 6974  de a time-sensit
-00029cd0: 6976 6520 7761 7465 7220 6d61 736b 0d0a  ive water mask..
-00029ce0: 2354 6869 7320 6d65 7468 6f64 2074 656e  #This method ten
-00029cf0: 6473 2074 6f20 776f 726b 2077 656c 6c20  ds to work well 
-00029d00: 6966 2074 6865 7265 2069 7320 6e6f 2077  if there is no w
-00029d10: 6574 2073 6e6f 7720 7072 6573 656e 740d  et snow present.
-00029d20: 0a23 5765 7420 736e 6f77 206f 7665 7220  .#Wet snow over 
-00029d30: 666c 6174 2061 7265 6173 2063 616e 2072  flat areas can r
-00029d40: 6573 756c 7420 696e 2066 616c 7365 2070  esult in false p
-00029d50: 6f73 6974 6976 6573 0d0a 2344 6573 6967  ositives..#Desig
-00029d60: 6e65 6420 746f 2077 6f72 6b20 7769 7468  ned to work with
-00029d70: 2054 4f41 2064 6174 612e 2053 5220 6461   TOA data. SR da
-00029d80: 7461 2077 696c 6c20 7265 7375 6c74 2069  ta will result i
-00029d90: 6e20 6661 6c73 6520 6e65 6761 7469 7665  n false negative
-00029da0: 7320 286f 6d69 7373 696f 6e29 0d0a 6465  s (omission)..de
-00029db0: 6620 7369 6d70 6c65 5761 7465 724d 6173  f simpleWaterMas
-00029dc0: 6b28 696d 672c 636f 6e74 7261 6374 5069  k(img,contractPi
-00029dd0: 7865 6c73 203d 2030 2c73 6c6f 7065 5f74  xels = 0,slope_t
-00029de0: 6872 6573 6820 3d20 3130 2c65 6c65 7661  hresh = 10,eleva
-00029df0: 7469 6f6e 496d 6167 6550 6174 6820 3d20  tionImagePath = 
-00029e00: 2255 5347 532f 3344 4550 2f31 306d 222c  "USGS/3DEP/10m",
-00029e10: 656c 6576 6174 696f 6e46 6f63 616c 4d65  elevationFocalMe
-00029e20: 616e 5261 6469 7573 203d 2035 2e35 293a  anRadius = 5.5):
-00029e30: 0d0a 2020 696d 6720 3d20 6164 6454 4341  ..  img = addTCA
-00029e40: 6e67 6c65 7328 696d 6729 0d0a 2020 6e65  ngles(img)..  ne
-00029e50: 6420 3d20 6565 2e49 6d61 6765 2865 6c65  d = ee.Image(ele
-00029e60: 7661 7469 6f6e 496d 6167 6550 6174 6829  vationImagePath)
-00029e70: 2e72 6573 616d 706c 6528 2762 6963 7562  .resample('bicub
-00029e80: 6963 2729 0d0a 2020 736c 6f70 6520 3d20  ic')..  slope = 
-00029e90: 6565 2e54 6572 7261 696e 2e73 6c6f 7065  ee.Terrain.slope
-00029ea0: 286e 6564 2e66 6f63 616c 5f6d 6561 6e28  (ned.focal_mean(
-00029eb0: 656c 6576 6174 696f 6e46 6f63 616c 4d65  elevationFocalMe
-00029ec0: 616e 5261 6469 7573 2929 0d0a 2020 666c  anRadius))..  fl
-00029ed0: 6174 203d 2073 6c6f 7065 2e6c 7465 2873  at = slope.lte(s
-00029ee0: 6c6f 7065 5f74 6872 6573 6829 0d0a 0d0a  lope_thresh)....
-00029ef0: 2020 7761 7465 724d 6173 6b20 3d20 696d    waterMask = im
-00029f00: 672e 7365 6c65 6374 285b 2774 6341 6e67  g.select(['tcAng
-00029f10: 6c65 4257 275d 292e 6774 6528 2d30 2e30  leBW']).gte(-0.0
-00029f20: 3529 5c0d 0a20 2020 202e 416e 6428 696d  5)\..    .And(im
-00029f30: 672e 7365 6c65 6374 285b 2774 6341 6e67  g.select(['tcAng
-00029f40: 6c65 4247 275d 292e 6c74 6528 302e 3035  leBG']).lte(0.05
-00029f50: 2929 5c0d 0a20 2020 202e 416e 6428 696d  ))\..    .And(im
-00029f60: 672e 7365 6c65 6374 285b 2762 7269 6768  g.select(['brigh
-00029f70: 746e 6573 7327 5d29 2e6c 7428 302e 3329  tness']).lt(0.3)
-00029f80: 295c 0d0a 2020 2020 2e41 6e64 2866 6c61  )\..    .And(fla
-00029f90: 7429 2e66 6f63 616c 5f6d 696e 2863 6f6e  t).focal_min(con
-00029fa0: 7472 6163 7450 6978 656c 7329 0d0a 0d0a  tractPixels)....
-00029fb0: 2020 7265 7475 726e 2077 6174 6572 4d61    return waterMa
-00029fc0: 736b 2e72 656e 616d 6528 5b27 7761 7465  sk.rename(['wate
-00029fd0: 724d 6173 6b27 5d29 0d0a 2323 2323 2323  rMask'])..######
-00029fe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029ff0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0002a000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0002a010: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-0002a020: 0a23 4a65 6666 2048 6f20 4d65 7468 6f64  .#Jeff Ho Method
-0002a030: 2066 6f72 2061 6c67 616c 2062 6c6f 6f6d   for algal bloom
-0002a040: 2064 6574 6563 7469 6f6e 0d0a 2368 7474   detection..#htt
-0002a050: 7073 3a2f 2f77 7777 2e6e 6174 7572 652e  ps://www.nature.
-0002a060: 636f 6d2f 6172 7469 636c 6573 2f73 3431  com/articles/s41
-0002a070: 3538 362d 3031 392d 3136 3438 2d37 0d0a  586-019-1648-7..
-0002a080: 0d0a 2320 5369 6d70 6c69 6669 6564 2053  ..# Simplified S
-0002a090: 6372 6970 7420 666f 7220 4c61 6e64 7361  cript for Landsa
-0002a0a0: 7420 5761 7465 7220 5175 616c 6974 790d  t Water Quality.
-0002a0b0: 0a23 2050 726f 6475 6365 7320 6120 6d61  .# Produces a ma
-0002a0c0: 7020 6f66 2061 6e20 616c 6761 6c20 626c  p of an algal bl
-0002a0d0: 6f6f 6d20 696e 204c 616b 6520 4572 6965  oom in Lake Erie
-0002a0e0: 206f 6e20 3230 3131 2f39 2f33 0d0a 2320   on 2011/9/3..# 
-0002a0f0: 4372 6561 7465 6420 6f6e 2031 322f 372f  Created on 12/7/
-0002a100: 3230 3135 2062 7920 4a65 6666 2048 6f0d  2015 by Jeff Ho.
-0002a110: 0a0d 0a23 2053 7065 6369 6669 6573 2061  ...# Specifies a
-0002a120: 2074 6872 6573 686f 6c64 2066 6f72 2068   threshold for h
-0002a130: 7565 2074 6f20 6573 7469 6d61 7465 2022  ue to estimate "
-0002a140: 6772 6565 6e22 2070 6978 656c 730d 0a23  green" pixels..#
-0002a150: 2074 6869 7320 6973 2075 7365 6420 6173   this is used as
-0002a160: 2061 6e20 6164 6469 7469 6f6e 616c 2066   an additional f
-0002a170: 696c 7465 7220 746f 2072 6566 696e 6520  ilter to refine 
-0002a180: 7468 6520 616c 676f 7269 7468 6d20 6162  the algorithm ab
-0002a190: 6f76 650d 0a64 6566 2048 6f43 616c 6347  ove..def HoCalcG
-0002a1a0: 7265 656e 6e65 7373 2869 6d67 293a 0d0a  reenness(img):..
-0002a1b0: 2020 236d 6170 2072 2c20 672c 2061 6e64    #map r, g, and
-0002a1c0: 2062 2066 6f72 206d 6f72 6520 7265 6164   b for more read
-0002a1d0: 6162 6c65 2061 6c67 6562 7261 2062 656c  able algebra bel
-0002a1e0: 6f77 0d0a 2020 7220 3d20 696d 672e 7365  ow..  r = img.se
-0002a1f0: 6c65 6374 285b 2772 6564 275d 290d 0a20  lect(['red']).. 
-0002a200: 2067 203d 2069 6d67 2e73 656c 6563 7428   g = img.select(
-0002a210: 5b27 6772 6565 6e27 5d29 0d0a 2020 6220  ['green'])..  b 
-0002a220: 3d20 696d 672e 7365 6c65 6374 285b 2762  = img.select(['b
-0002a230: 6c75 6527 5d29 0d0a 0d0a 2020 2363 616c  lue'])....  #cal
-0002a240: 6375 6c61 7465 2069 6e74 656e 7369 7479  culate intensity
-0002a250: 2c20 6875 650d 0a20 2049 203d 2072 2e61  , hue..  I = r.a
-0002a260: 6464 2867 292e 6164 6428 6229 2e72 656e  dd(g).add(b).ren
-0002a270: 616d 6528 5b27 4927 5d29 0d0a 2020 6d69  ame(['I'])..  mi
-0002a280: 6e73 203d 2072 2e6d 696e 2867 292e 6d69  ns = r.min(g).mi
-0002a290: 6e28 6229 2e72 656e 616d 6528 5b27 6d69  n(b).rename(['mi
-0002a2a0: 6e73 275d 290d 0a20 2048 203d 206d 696e  ns'])..  H = min
-0002a2b0: 732e 7768 6572 6528 6d69 6e73 2e65 7128  s.where(mins.eq(
-0002a2c0: 7229 2c28 622e 7375 6274 7261 6374 2872  r),(b.subtract(r
-0002a2d0: 2929 2e64 6976 6964 6528 492e 7375 6274  )).divide(I.subt
-0002a2e0: 7261 6374 2872 2e6d 756c 7469 706c 7928  ract(r.multiply(
-0002a2f0: 3329 2929 2e61 6464 2831 2920 290d 0a20  3))).add(1) ).. 
-0002a300: 2048 203d 2048 2e77 6865 7265 286d 696e   H = H.where(min
-0002a310: 732e 6571 2867 292c 2872 2e73 7562 7472  s.eq(g),(r.subtr
-0002a320: 6163 7428 6729 292e 6469 7669 6465 2849  act(g)).divide(I
-0002a330: 2e73 7562 7472 6163 7428 672e 6d75 6c74  .subtract(g.mult
-0002a340: 6970 6c79 2833 2929 292e 6164 6428 3229  iply(3))).add(2)
-0002a350: 2029 0d0a 2020 4820 3d20 482e 7768 6572   )..  H = H.wher
-0002a360: 6528 6d69 6e73 2e65 7128 6229 2c28 672e  e(mins.eq(b),(g.
-0002a370: 7375 6274 7261 6374 2862 2929 2e64 6976  subtract(b)).div
-0002a380: 6964 6528 492e 7375 6274 7261 6374 2862  ide(I.subtract(b
-0002a390: 2e6d 756c 7469 706c 7928 3329 2929 2029  .multiply(3))) )
-0002a3a0: 0d0a 0d0a 2020 2370 6978 656c 7320 7769  ....  #pixels wi
-0002a3b0: 7468 2068 7565 2062 656c 6f77 2031 2e36  th hue below 1.6
-0002a3c0: 206d 6f72 6520 6c69 6b65 6c79 2074 6f20   more likely to 
-0002a3d0: 6265 2062 6c6f 6f6d 2061 6e64 206e 6f74  be bloom and not
-0002a3e0: 2073 7573 7065 6e64 6564 2073 6564 696d   suspended sedim
-0002a3f0: 656e 740d 0a20 2048 7468 7265 7368 203d  ent..  Hthresh =
-0002a400: 2048 2e6c 7465 2831 2e36 290d 0a0d 0a20   H.lte(1.6).... 
-0002a410: 2072 6574 7572 6e20 482e 7265 6e61 6d65   return H.rename
-0002a420: 2827 4827 290d 0a0d 0a0d 0a23 4170 706c  ('H')......#Appl
-0002a430: 7920 626c 6f6f 6d20 6465 7465 6374 696f  y bloom detectio
-0002a440: 6e20 616c 676f 7269 7468 6d0d 0a64 6566  n algorithm..def
-0002a450: 2048 6f43 616c 6341 6c67 6f72 6974 686d   HoCalcAlgorithm
-0002a460: 3128 696d 6167 6529 3a0d 0a20 2074 7275  1(image):..  tru
-0002a470: 6563 6f6c 6f72 203d 2031 2023 7368 6f77  ecolor = 1 #show
-0002a480: 2074 7275 6520 636f 6c6f 7220 696d 6167   true color imag
-0002a490: 6520 6173 2077 656c 6c0d 0a20 2074 6573  e as well..  tes
-0002a4a0: 7454 6872 6573 6820 3d20 4661 6c73 6520  tThresh = False 
-0002a4b0: 2320 6164 6420 6120 6269 6e61 7279 2069  # add a binary i
-0002a4c0: 6d61 6765 2063 6c61 7373 6966 7969 6e67  mage classifying
-0002a4d0: 2069 6e74 6f20 2262 6c6f 6f6d 2261 6e64   into "bloom"and
-0002a4e0: 2022 6e6f 6e2d 626c 6f6f 6d0d 0a20 2062   "non-bloom..  b
-0002a4f0: 6c6f 6f6d 5468 7265 7368 6f6c 6420 3d20  loomThreshold = 
-0002a500: 302e 3032 3334 3620 2374 6872 6573 686f  0.02346 #thresho
-0002a510: 6c64 2066 6f72 2063 6c61 7373 6966 6963  ld for classific
-0002a520: 6174 696f 6e20 6669 7420 6261 7365 6420  ation fit based 
-0002a530: 6f6e 206f 7468 6572 2064 6174 610d 0a20  on other data.. 
-0002a540: 2067 7265 656e 6573 7354 6872 6573 686f   greenessThresho
-0002a550: 6c64 203d 2031 2e36 0d0a 0d0a 2020 2320  ld = 1.6....  # 
-0002a560: 416c 676f 7269 7468 6d20 3120 6261 7365  Algorithm 1 base
-0002a570: 6420 6f6e 3a0d 0a20 2023 2057 616e 672c  d on:..  # Wang,
-0002a580: 204d 2e2c 2026 2053 6869 2c20 572e 2028   M., & Shi, W. (
-0002a590: 3230 3037 292e 2054 6865 204e 4952 2d53  2007). The NIR-S
-0002a5a0: 5749 5220 636f 6d62 696e 6564 2061 746d  WIR combined atm
-0002a5b0: 6f73 7068 6572 6963 0d0a 2020 2320 2063  ospheric..  #  c
-0002a5c0: 6f72 7265 6374 696f 6e20 6170 7072 6f61  orrection approa
-0002a5d0: 6368 2066 6f72 204d 4f44 4953 206f 6365  ch for MODIS oce
-0002a5e0: 616e 2063 6f6c 6f72 2064 6174 6120 7072  an color data pr
-0002a5f0: 6f63 6573 7369 6e67 2e0d 0a20 2023 2020  ocessing...  #  
-0002a600: 4f70 7469 6373 2045 7870 7265 7373 2c20  Optics Express, 
-0002a610: 3135 2832 3429 2c20 3135 3732 32e2 8093  15(24), 15722...
-0002a620: 3135 3733 332e 0d0a 0d0a 2020 2320 4164  15733.....  # Ad
-0002a630: 6420 7365 636f 6e64 6172 7920 6669 6c74  d secondary filt
-0002a640: 6572 2075 7369 6e67 2067 7265 656e 6e65  er using greenne
-0002a650: 7373 2066 756e 6374 696f 6e20 6265 6c6f  ss function belo
-0002a660: 770d 0a20 2069 6d61 6765 203d 2069 6d61  w..  image = ima
-0002a670: 6765 2e61 6464 4261 6e64 7328 486f 4361  ge.addBands(HoCa
-0002a680: 6c63 4772 6565 6e6e 6573 7328 696d 6167  lcGreenness(imag
-0002a690: 6529 290d 0a0d 0a20 2023 2041 7070 6c79  e))....  # Apply
-0002a6a0: 2061 6c67 6f72 6974 686d 2031 3a20 4234   algorithm 1: B4
-0002a6b0: 202d 2031 2e30 332a 4235 0d0a 2020 2362   - 1.03*B5..  #b
-0002a6c0: 6c6f 6f6d 3120 3d20 696d 6167 652e 7365  loom1 = image.se
-0002a6d0: 6c65 6374 2827 6e69 7227 292e 7375 6274  lect('nir').subt
-0002a6e0: 7261 6374 2869 6d61 6765 2e73 656c 6563  ract(image.selec
-0002a6f0: 7428 2773 7769 7231 2729 2e6d 756c 7469  t('swir1').multi
-0002a700: 706c 7928 312e 3033 2929 2e72 656e 616d  ply(1.03)).renam
-0002a710: 6528 2762 6c6f 6f6d 3127 290d 0a0d 0a20  e('bloom1').... 
-0002a720: 2023 2047 6574 2062 696e 6172 7920 696d   # Get binary im
-0002a730: 6167 6520 6279 2061 7070 6c79 696e 6720  age by applying 
-0002a740: 7468 6520 7468 7265 7368 6f6c 640d 0a20  the threshold.. 
-0002a750: 2062 6c6f 6f6d 315f 6d61 736b 203d 2069   bloom1_mask = i
-0002a760: 6d61 6765 2e73 656c 6563 7428 2248 2229  mage.select("H")
-0002a770: 2e6c 7465 2867 7265 656e 6573 7354 6872  .lte(greenessThr
-0002a780: 6573 686f 6c64 292e 7265 6e61 6d65 285b  eshold).rename([
-0002a790: 2262 6c6f 6f6d 315f 6d61 736b 225d 290d  "bloom1_mask"]).
-0002a7a0: 0a0d 0a0d 0a20 2072 6574 7572 6e20 696d  .....  return im
-0002a7b0: 6167 655c 0d0a 2020 2020 2020 2020 2020  age\..          
-0002a7c0: 2e61 6464 4261 6e64 7328 626c 6f6f 6d31  .addBands(bloom1
-0002a7d0: 295c 0d0a 2020 2020 2020 2020 2020 2e61  )\..          .a
-0002a7e0: 6464 4261 6e64 7328 626c 6f6f 6d31 5f6d  ddBands(bloom1_m
-0002a7f0: 6173 6b29 0d0a 0d0a 0d0a 0d0a 0d0a 2320  ask)..........# 
-0002a800: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a810: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a820: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a830: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a840: 2f2f 2f2f 2f2f 2f2f 2f2f 0d0a 2320 2f2f  //////////..# //
-0002a850: 2045 4e44 2046 554e 4354 494f 4e53 0d0a   END FUNCTIONS..
-0002a860: 2320 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  # //////////////
-0002a870: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a880: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a890: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+00023c00: 2323 2323 2323 2323 2323 230d 0a23 4861  ###########..#Ha
+00023c10: 726d 6f6e 6963 2072 6567 7265 7373 696f  rmonic regressio
+00023c20: 6e0d 0a23 2323 2323 2323 2323 2323 2323  n..#############
+00023c30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023c40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023c50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023c60: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
+00023c70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023c80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023c90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023ca0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023cb0: 2323 2323 2323 230d 0a23 4675 6e63 7469  #######..#Functi
+00023cc0: 6f6e 2074 6f20 6769 7665 2079 6561 722e  on to give year.
+00023cd0: 6464 2069 6d61 6765 2061 6e64 2068 6172  dd image and har
+00023ce0: 6d6f 6e69 6373 206c 6973 7420 2865 2e67  monics list (e.g
+00023cf0: 2e20 5b31 2c32 2c33 2c2e 2e2e 5d29 0d0a  . [1,2,3,...])..
+00023d00: 6465 6620 6765 7448 6172 6d6f 6e69 634c  def getHarmonicL
+00023d10: 6973 7428 7965 6172 4461 7465 496d 672c  ist(yearDateImg,
+00023d20: 7472 616e 7366 6f72 6d42 616e 644e 616d  transformBandNam
+00023d30: 652c 6861 726d 6f6e 6963 4c69 7374 293a  e,harmonicList):
+00023d40: 0d0a 2020 743d 2079 6561 7244 6174 6549  ..  t= yearDateI
+00023d50: 6d67 2e73 656c 6563 7428 5b74 7261 6e73  mg.select([trans
+00023d60: 666f 726d 4261 6e64 4e61 6d65 5d29 0d0a  formBandName])..
+00023d70: 2020 7365 6c65 6374 4261 6e64 7320 3d20    selectBands = 
+00023d80: 6565 2e4c 6973 742e 7365 7175 656e 6365  ee.List.sequence
+00023d90: 2830 2c6c 656e 2868 6172 6d6f 6e69 634c  (0,len(harmonicL
+00023da0: 6973 7429 2d31 290d 0a0d 0a20 2064 6566  ist)-1)....  def
+00023db0: 2073 696e 4361 7428 6829 3a0d 0a20 2020   sinCat(h):..   
+00023dc0: 2068 7420 3d20 682a 3130 300d 0a20 2020   ht = h*100..   
+00023dd0: 2072 6574 7572 6e20 6565 2e53 7472 696e   return ee.Strin
+00023de0: 6728 2773 696e 5f27 292e 6361 7428 7374  g('sin_').cat(st
+00023df0: 7228 6874 2929 2e63 6174 2827 5f27 292e  r(ht)).cat('_').
+00023e00: 6361 7428 7472 616e 7366 6f72 6d42 616e  cat(transformBan
+00023e10: 644e 616d 6529 0d0a 2020 7369 6e4e 616d  dName)..  sinNam
+00023e20: 6573 203d 206c 6973 7428 6d61 7028 6c61  es = list(map(la
+00023e30: 6d62 6461 2069 3a73 696e 4361 7428 6929  mbda i:sinCat(i)
+00023e40: 2c68 6172 6d6f 6e69 634c 6973 7429 290d  ,harmonicList)).
+00023e50: 0a0d 0a20 2064 6566 2063 6f73 4361 7428  ...  def cosCat(
+00023e60: 6829 3a0d 0a20 2020 2068 7420 3d68 2a31  h):..    ht =h*1
+00023e70: 3030 3b0d 0a20 2020 2072 6574 7572 6e20  00;..    return 
+00023e80: 6565 2e53 7472 696e 6728 2763 6f73 5f27  ee.String('cos_'
+00023e90: 292e 6361 7428 7374 7228 6874 2929 2e63  ).cat(str(ht)).c
+00023ea0: 6174 2827 5f27 292e 6361 7428 7472 616e  at('_').cat(tran
+00023eb0: 7366 6f72 6d42 616e 644e 616d 6529 0d0a  sformBandName)..
+00023ec0: 0d0a 2020 636f 734e 616d 6573 203d 206c  ..  cosNames = l
+00023ed0: 6973 7428 6d61 7028 6c61 6d62 6461 2069  ist(map(lambda i
+00023ee0: 203a 2063 6f73 4361 7428 6929 2c68 6172   : cosCat(i),har
+00023ef0: 6d6f 6e69 634c 6973 7429 290d 0a0d 0a0d  monicList)).....
+00023f00: 0a0d 0a20 206d 756c 7469 706c 6965 7273  ...  multipliers
+00023f10: 203d 2065 652e 496d 6167 6528 6861 726d   = ee.Image(harm
+00023f20: 6f6e 6963 4c69 7374 292e 6d75 6c74 6970  onicList).multip
+00023f30: 6c79 2865 652e 4e75 6d62 6572 286d 6174  ly(ee.Number(mat
+00023f40: 682e 7069 292e 666c 6f61 7428 2929 0d0a  h.pi).float())..
+00023f50: 2020 7369 6e49 6e64 203d 2028 742e 6d75    sinInd = (t.mu
+00023f60: 6c74 6970 6c79 2865 652e 496d 6167 6528  ltiply(ee.Image(
+00023f70: 6d75 6c74 6970 6c69 6572 7329 2929 2e73  multipliers))).s
+00023f80: 696e 2829 2e73 656c 6563 7428 7365 6c65  in().select(sele
+00023f90: 6374 4261 6e64 732c 7369 6e4e 616d 6573  ctBands,sinNames
+00023fa0: 292e 666c 6f61 7428 290d 0a20 2063 6f73  ).float()..  cos
+00023fb0: 496e 6420 3d20 2874 2e6d 756c 7469 706c  Ind = (t.multipl
+00023fc0: 7928 6565 2e49 6d61 6765 286d 756c 7469  y(ee.Image(multi
+00023fd0: 706c 6965 7273 2929 292e 636f 7328 292e  pliers))).cos().
+00023fe0: 7365 6c65 6374 2873 656c 6563 7442 616e  select(selectBan
+00023ff0: 6473 2c63 6f73 4e61 6d65 7329 2e66 6c6f  ds,cosNames).flo
+00024000: 6174 2829 0d0a 0d0a 2020 7265 7475 726e  at()....  return
+00024010: 2079 6561 7244 6174 6549 6d67 2e61 6464   yearDateImg.add
+00024020: 4261 6e64 7328 7369 6e49 6e64 2e61 6464  Bands(sinInd.add
+00024030: 4261 6e64 7328 636f 7349 6e64 2929 0d0a  Bands(cosInd))..
+00024040: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00024050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024080: 2323 2323 2323 2323 2323 230d 0a23 2323  ###########..###
+00024090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000240a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000240b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000240c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000240d0: 2323 2323 2323 0d0a 2354 616b 6573 2061  ######..#Takes a
+000240e0: 2064 6570 656e 6465 6e74 2061 6e64 2069   dependent and i
+000240f0: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
+00024100: 626c 6520 616e 6420 7265 7475 726e 7320  ble and returns 
+00024110: 7468 6520 6465 7065 6e64 656e 742c 0d0a  the dependent,..
+00024120: 2320 7369 6e20 6f66 2069 6e64 2c20 616e  # sin of ind, an
+00024130: 6420 636f 7320 6f66 2069 6e64 0d0a 2349  d cos of ind..#I
+00024140: 6e74 656e 6465 6420 666f 7220 6861 726d  ntended for harm
+00024150: 6f6e 6963 2072 6567 7265 7373 696f 6e0d  onic regression.
+00024160: 0a64 6566 2067 6574 4861 726d 6f6e 6963  .def getHarmonic
+00024170: 7332 2863 6f6c 6c65 6374 696f 6e2c 7472  s2(collection,tr
+00024180: 616e 7366 6f72 6d42 616e 644e 616d 652c  ansformBandName,
+00024190: 6861 726d 6f6e 6963 4c69 7374 2c64 6574  harmonicList,det
+000241a0: 7265 6e64 203d 2046 616c 7365 293a 0d0a  rend = False):..
+000241b0: 0d0a 2020 6465 7042 616e 644e 616d 6573  ..  depBandNames
+000241c0: 203d 2065 652e 496d 6167 6528 636f 6c6c   = ee.Image(coll
+000241d0: 6563 7469 6f6e 2e66 6972 7374 2829 292e  ection.first()).
+000241e0: 6261 6e64 4e61 6d65 7328 292e 7265 6d6f  bandNames().remo
+000241f0: 7665 2874 7261 6e73 666f 726d 4261 6e64  ve(transformBand
+00024200: 4e61 6d65 290d 0a20 2064 6570 4261 6e64  Name)..  depBand
+00024210: 4e75 6d62 6572 7320 3d20 6465 7042 616e  Numbers = depBan
+00024220: 644e 616d 6573 2e6d 6170 286c 616d 6264  dNames.map(lambd
+00024230: 6120 6462 6e3a 6465 7042 616e 644e 616d  a dbn:depBandNam
+00024240: 6573 2e69 6e64 6578 4f66 2864 626e 2929  es.indexOf(dbn))
+00024250: 0d0a 0d0a 2020 6465 6620 6861 726d 5772  ....  def harmWr
+00024260: 6170 2869 6d67 293a 0d0a 2020 2020 6f75  ap(img):..    ou
+00024270: 7454 203d 2067 6574 4861 726d 6f6e 6963  tT = getHarmonic
+00024280: 4c69 7374 2869 6d67 2c74 7261 6e73 666f  List(img,transfo
+00024290: 726d 4261 6e64 4e61 6d65 2c68 6172 6d6f  rmBandName,harmo
+000242a0: 6e69 634c 6973 7429 5c0d 0a20 2020 202e  nicList)\..    .
+000242b0: 636f 7079 5072 6f70 6572 7469 6573 2869  copyProperties(i
+000242c0: 6d67 2c5b 2773 7973 7465 6d3a 7469 6d65  mg,['system:time
+000242d0: 5f73 7461 7274 272c 2773 7973 7465 6d3a  _start','system:
+000242e0: 7469 6d65 5f65 6e64 275d 290d 0a20 2020  time_end'])..   
+000242f0: 2072 6574 7572 6e20 6f75 7454 0d0a 2020   return outT..  
+00024300: 6f75 7420 3d20 636f 6c6c 6563 7469 6f6e  out = collection
+00024310: 2e6d 6170 2868 6172 6d57 7261 7029 0d0a  .map(harmWrap)..
+00024320: 0d0a 2020 6966 206e 6f74 2064 6574 7265  ..  if not detre
+00024330: 6e64 3a0d 0a20 2020 206f 7574 4261 6e64  nd:..    outBand
+00024340: 4e61 6d65 7320 3d20 6565 2e49 6d61 6765  Names = ee.Image
+00024350: 286f 7574 2e66 6972 7374 2829 292e 6261  (out.first()).ba
+00024360: 6e64 4e61 6d65 7328 292e 7265 6d6f 7665  ndNames().remove
+00024370: 416c 6c28 5b27 7965 6172 275d 290d 0a20  All(['year']).. 
+00024380: 2020 206f 7574 203d 206f 7574 2e73 656c     out = out.sel
+00024390: 6563 7428 6f75 7442 616e 644e 616d 6573  ect(outBandNames
+000243a0: 290d 0a0d 0a0d 0a20 2069 6e64 4261 6e64  )......  indBand
+000243b0: 4e61 6d65 7320 3d20 6565 2e49 6d61 6765  Names = ee.Image
+000243c0: 286f 7574 2e66 6972 7374 2829 292e 6261  (out.first()).ba
+000243d0: 6e64 4e61 6d65 7328 292e 7265 6d6f 7665  ndNames().remove
+000243e0: 416c 6c28 6465 7042 616e 644e 616d 6573  All(depBandNames
+000243f0: 290d 0a20 2069 6e64 4261 6e64 4e75 6d62  )..  indBandNumb
+00024400: 6572 7320 3d20 696e 6442 616e 644e 616d  ers = indBandNam
+00024410: 6573 2e6d 6170 286c 616d 6264 6120 696e  es.map(lambda in
+00024420: 643a 2065 652e 496d 6167 6528 6f75 742e  d: ee.Image(out.
+00024430: 6669 7273 7428 2929 2e62 616e 644e 616d  first()).bandNam
+00024440: 6573 2829 2e69 6e64 6578 4f66 2869 6e64  es().indexOf(ind
+00024450: 2929 0d0a 0d0a 0d0a 2020 6f75 7420 3d20  ))......  out = 
+00024460: 6f75 742e 7365 7428 7b27 696e 6442 616e  out.set({'indBan
+00024470: 644e 616d 6573 273a 696e 6442 616e 644e  dNames':indBandN
+00024480: 616d 6573 2c27 6465 7042 616e 644e 616d  ames,'depBandNam
+00024490: 6573 273a 6465 7042 616e 644e 616d 6573  es':depBandNames
+000244a0: 2c5c 0d0a 2020 2020 2020 2020 2020 2020  ,\..            
+000244b0: 2020 2020 2769 6e64 4261 6e64 4e75 6d62      'indBandNumb
+000244c0: 6572 7327 3a69 6e64 4261 6e64 4e75 6d62  ers':indBandNumb
+000244d0: 6572 732c 2764 6570 4261 6e64 4e75 6d62  ers,'depBandNumb
+000244e0: 6572 7327 3a64 6570 4261 6e64 4e75 6d62  ers':depBandNumb
+000244f0: 6572 737d 290d 0a0d 0a20 2072 6574 7572  ers})....  retur
+00024500: 6e20 6f75 740d 0a0d 0a23 2323 2323 2323  n out....#######
+00024510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024550: 2323 0d0a 2323 2323 2323 2323 2323 2323  ##..############
+00024560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024570: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024580: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024590: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
+000245a0: 5369 6d70 6c69 6669 6573 2074 6865 2075  Simplifies the u
+000245b0: 7365 206f 6620 7468 6520 726f 6275 7374  se of the robust
+000245c0: 206c 696e 6561 7220 7265 6772 6573 7369   linear regressi
+000245d0: 6f6e 2072 6564 7563 6572 0d0a 2341 7373  on reducer..#Ass
+000245e0: 756d 6573 2074 6865 2064 6570 656e 6465  umes the depende
+000245f0: 6e74 2069 7320 7468 6520 6669 7273 7420  nt is the first 
+00024600: 6261 6e64 2061 6e64 2061 6c6c 2073 7562  band and all sub
+00024610: 7365 7175 656e 7420 6261 6e64 7320 6172  sequent bands ar
+00024620: 6520 696e 6465 7065 6e64 656e 7473 0d0a  e independents..
+00024630: 6465 6620 6e65 7752 6f62 7573 744d 756c  def newRobustMul
+00024640: 7469 706c 654c 696e 6561 7232 2864 6570  tipleLinear2(dep
+00024650: 656e 6465 6e74 7349 6e64 6570 656e 6465  endentsIndepende
+00024660: 6e74 7329 3a0d 0a20 2023 5365 7420 7570  nts):..  #Set up
+00024670: 2074 6865 2062 616e 6420 6e61 6d65 730d   the band names.
+00024680: 0a0d 0a20 2064 6570 656e 6465 6e74 4261  ...  dependentBa
+00024690: 6e64 7320 3d20 6565 2e4c 6973 7428 6465  nds = ee.List(de
+000246a0: 7065 6e64 656e 7473 496e 6465 7065 6e64  pendentsIndepend
+000246b0: 656e 7473 2e67 6574 2827 6465 7042 616e  ents.get('depBan
+000246c0: 644e 756d 6265 7273 2729 290d 0a20 2069  dNumbers'))..  i
+000246d0: 6e64 6570 656e 6465 6e74 4261 6e64 7320  ndependentBands 
+000246e0: 3d20 6565 2e4c 6973 7428 6465 7065 6e64  = ee.List(depend
+000246f0: 656e 7473 496e 6465 7065 6e64 656e 7473  entsIndependents
+00024700: 2e67 6574 2827 696e 6442 616e 644e 756d  .get('indBandNum
+00024710: 6265 7273 2729 290d 0a20 2062 6e73 203d  bers'))..  bns =
+00024720: 2065 652e 496d 6167 6528 6465 7065 6e64   ee.Image(depend
+00024730: 656e 7473 496e 6465 7065 6e64 656e 7473  entsIndependents
+00024740: 2e66 6972 7374 2829 292e 6261 6e64 4e61  .first()).bandNa
+00024750: 6d65 7328 290d 0a20 2064 6570 656e 6465  mes()..  depende
+00024760: 6e74 7320 3d20 6565 2e4c 6973 7428 6465  nts = ee.List(de
+00024770: 7065 6e64 656e 7473 496e 6465 7065 6e64  pendentsIndepend
+00024780: 656e 7473 2e67 6574 2827 6465 7042 616e  ents.get('depBan
+00024790: 644e 616d 6573 2729 290d 0a20 2069 6e64  dNames'))..  ind
+000247a0: 6570 656e 6465 6e74 7320 3d20 6565 2e4c  ependents = ee.L
+000247b0: 6973 7428 6465 7065 6e64 656e 7473 496e  ist(dependentsIn
+000247c0: 6465 7065 6e64 656e 7473 2e67 6574 2827  dependents.get('
+000247d0: 696e 6442 616e 644e 616d 6573 2729 290d  indBandNames')).
+000247e0: 0a0d 0a20 2023 6465 7065 6e64 656e 7420  ...  #dependent 
+000247f0: 3d20 626e 732e 736c 6963 6528 302c 3129  = bns.slice(0,1)
+00024800: 0d0a 2020 2369 6e64 6570 656e 6465 6e74  ..  #independent
+00024810: 7320 3d20 626e 732e 736c 6963 6528 312c  s = bns.slice(1,
+00024820: 6e75 6c6c 290d 0a20 206e 6f49 6e64 6570  null)..  noIndep
+00024830: 656e 6465 6e74 7320 3d20 696e 6465 7065  endents = indepe
+00024840: 6e64 656e 7473 2e6c 656e 6774 6828 292e  ndents.length().
+00024850: 6164 6428 3129 0d0a 2020 6e6f 4465 7065  add(1)..  noDepe
+00024860: 6e64 656e 7473 203d 2064 6570 656e 6465  ndents = depende
+00024870: 6e74 732e 6c65 6e67 7468 2829 0d0a 0d0a  nts.length()....
+00024880: 2020 6f75 744e 616d 6573 203d 2065 652e    outNames = ee.
+00024890: 4c69 7374 285b 2769 6e74 6572 6365 7074  List(['intercept
+000248a0: 275d 292e 6361 7428 696e 6465 7065 6e64  ']).cat(independ
+000248b0: 656e 7473 290d 0a0d 0a20 2023 4164 6420  ents)....  #Add 
+000248c0: 636f 6e73 7461 6e74 2062 616e 6420 666f  constant band fo
+000248d0: 7220 696e 7465 7263 6570 7420 616e 6420  r intercept and 
+000248e0: 7265 6f72 6465 7220 666f 720d 0a20 2023  reorder for..  #
+000248f0: 7379 6e74 6178 3a20 636f 6e73 7461 6e74  syntax: constant
+00024900: 2c20 696e 6431 2c69 6e64 322c 696e 6433  , ind1,ind2,ind3
+00024910: 2c69 6e64 6e2c 6465 7065 6e64 656e 740d  ,indn,dependent.
+00024920: 0a20 2064 6566 2066 6f72 4669 7446 756e  .  def forFitFun
+00024930: 2869 6d67 293a 0d0a 2020 2020 6f75 7420  (img):..    out 
+00024940: 3d20 696d 672e 6164 6442 616e 6473 2865  = img.addBands(e
+00024950: 652e 496d 6167 6528 3129 2e73 656c 6563  e.Image(1).selec
+00024960: 7428 5b30 5d2c 5b27 636f 6e73 7461 6e74  t([0],['constant
+00024970: 275d 2929 0d0a 2020 2020 6f75 7420 3d20  ']))..    out = 
+00024980: 6f75 742e 7365 6c65 6374 2865 652e 4c69  out.select(ee.Li
+00024990: 7374 285b 2763 6f6e 7374 616e 7427 2c69  st(['constant',i
+000249a0: 6e64 6570 656e 6465 6e74 735d 292e 666c  ndependents]).fl
+000249b0: 6174 7465 6e28 2929 0d0a 2020 2020 7265  atten())..    re
+000249c0: 7475 726e 206f 7574 2e61 6464 4261 6e64  turn out.addBand
+000249d0: 7328 696d 672e 7365 6c65 6374 2864 6570  s(img.select(dep
+000249e0: 656e 6465 6e74 7329 290d 0a0d 0a0d 0a20  endents))...... 
+000249f0: 2066 6f72 4669 7420 3d20 6465 7065 6e64   forFit = depend
+00024a00: 656e 7473 496e 6465 7065 6e64 656e 7473  entsIndependents
+00024a10: 2e6d 6170 2866 6f72 4669 7446 756e 290d  .map(forFitFun).
+00024a20: 0a0d 0a20 2023 4170 706c 7920 7265 6475  ...  #Apply redu
+00024a30: 6365 722c 2061 6e64 2063 6f6e 7665 7274  cer, and convert
+00024a40: 2062 6163 6b20 746f 2069 6d61 6765 2077   back to image w
+00024a50: 6974 6820 7265 7370 6563 7469 7665 2062  ith respective b
+00024a60: 616e 644e 616d 6573 0d0a 2020 7265 6475  andNames..  redu
+00024a70: 6365 724f 7574 203d 2066 6f72 4669 742e  cerOut = forFit.
+00024a80: 7265 6475 6365 2865 652e 5265 6475 6365  reduce(ee.Reduce
+00024a90: 722e 6c69 6e65 6172 5265 6772 6573 7369  r.linearRegressi
+00024aa0: 6f6e 286e 6f49 6e64 6570 656e 6465 6e74  on(noIndependent
+00024ab0: 732c 6e6f 4465 7065 6e64 656e 7473 2929  s,noDependents))
+00024ac0: 0d0a 2020 2320 2f2f 2074 6573 7420 3d20  ..  # // test = 
+00024ad0: 666f 7246 6974 2e72 6564 7563 6528 6565  forFit.reduce(ee
+00024ae0: 2e52 6564 7563 6572 2e72 6f62 7573 744c  .Reducer.robustL
+00024af0: 696e 6561 7252 6567 7265 7373 696f 6e28  inearRegression(
+00024b00: 6e6f 496e 6465 7065 6e64 656e 7473 2c6e  noIndependents,n
+00024b10: 6f44 6570 656e 6465 6e74 732c 302e 3229  oDependents,0.2)
+00024b20: 290d 0a20 2023 202f 2f20 7265 7369 6473  )..  # // resids
+00024b30: 203d 2074 6573 740d 0a20 2023 202f 2f20   = test..  # // 
+00024b40: 2e73 656c 6563 7428 5b31 5d2c 5b27 7265  .select([1],['re
+00024b50: 7369 6475 616c 7327 5d29 2e61 7272 6179  siduals']).array
+00024b60: 466c 6174 7465 6e28 5b64 6570 656e 6465  Flatten([depende
+00024b70: 6e74 735d 293b 0d0a 2020 2320 2f2f 204d  nts]);..  # // M
+00024b80: 6170 2e61 6464 4c61 7965 7228 7265 7369  ap.addLayer(resi
+00024b90: 6473 2c7b 7d2c 2772 6573 6964 7349 6d61  ds,{},'residsIma
+00024ba0: 6765 2729 3b0d 0a20 2023 202f 2f20 4d61  ge');..  # // Ma
+00024bb0: 702e 6164 644c 6179 6572 2872 6564 7563  p.addLayer(reduc
+00024bc0: 6572 4f75 742e 7365 6c65 6374 285b 305d  erOut.select([0]
+00024bd0: 292c 7b7d 2c27 636f 6566 6669 6369 656e  ),{},'coefficien
+00024be0: 7473 2729 3b0d 0a20 2023 202f 2f20 4d61  ts');..  # // Ma
+00024bf0: 702e 6164 644c 6179 6572 2874 6573 742e  p.addLayer(test.
+00024c00: 7365 6c65 6374 285b 315d 292c 7b7d 2c27  select([1]),{},'
+00024c10: 7472 6573 6964 7561 6c73 2729 3b0d 0a20  tresiduals');.. 
+00024c20: 2023 202f 2f20 4d61 702e 6164 644c 6179   # // Map.addLay
+00024c30: 6572 2872 6564 7563 6572 4f75 742e 7365  er(reducerOut.se
+00024c40: 6c65 6374 285b 315d 292c 7b7d 2c27 726f  lect([1]),{},'ro
+00024c50: 7265 7369 6475 616c 7327 293b 0d0a 2020  residuals');..  
+00024c60: 7265 6475 6365 724f 7574 203d 2072 6564  reducerOut = red
+00024c70: 7563 6572 4f75 742e 7365 6c65 6374 285b  ucerOut.select([
+00024c80: 305d 2c5b 2763 6f65 6666 6963 6965 6e74  0],['coefficient
+00024c90: 7327 5d29 2e61 7272 6179 5472 616e 7370  s']).arrayTransp
+00024ca0: 6f73 6528 292e 6172 7261 7946 6c61 7474  ose().arrayFlatt
+00024cb0: 656e 285b 6465 7065 6e64 656e 7473 2c6f  en([dependents,o
+00024cc0: 7574 4e61 6d65 735d 290d 0a20 2072 6564  utNames])..  red
+00024cd0: 7563 6572 4f75 7420 3d20 7265 6475 6365  ucerOut = reduce
+00024ce0: 724f 7574 2e73 6574 287b 276e 6f44 6570  rOut.set({'noDep
+00024cf0: 656e 6465 6e74 7327 3a65 652e 4e75 6d62  endents':ee.Numb
+00024d00: 6572 286e 6f44 6570 656e 6465 6e74 7329  er(noDependents)
+00024d10: 2c5c 0d0a 2020 276d 6f64 656c 4c65 6e67  ,\..  'modelLeng
+00024d20: 7468 273a 6565 2e4e 756d 6265 7228 6e6f  th':ee.Number(no
+00024d30: 496e 6465 7065 6e64 656e 7473 295c 0d0a  Independents)\..
+00024d40: 2020 7d29 0d0a 0d0a 2020 7265 7475 726e    })....  return
+00024d50: 2072 6564 7563 6572 4f75 740d 0a23 2323   reducerOut..###
+00024d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024d80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024d90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024da0: 2323 2323 2323 0d0a 2323 2323 2323 2323  ######..########
+00024db0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024dc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024dd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024de0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024df0: 230d 0a23 436f 6465 2066 6f72 2066 696e  #..#Code for fin
+00024e00: 6469 6e67 2074 6865 2064 6174 6520 6f66  ding the date of
+00024e10: 2070 6561 6b20 6f66 2067 7265 656e 0d0a   peak of green..
+00024e20: 2320 416c 736f 2063 6f6e 7665 7274 7320  # Also converts 
+00024e30: 6974 2074 6f20 4a75 6c69 616e 2064 6179  it to Julian day
+00024e40: 2c20 6d6f 6e74 682c 2061 6e64 2064 6179  , month, and day
+00024e50: 206f 6620 6d6f 6e74 680d 0a6d 6f6e 7468   of month..month
+00024e60: 5265 6d61 7020 3d5b 312c 2031 2c20 312c  Remap =[1, 1, 1,
+00024e70: 2031 2c20 312c 2031 2c20 312c 2031 2c20   1, 1, 1, 1, 1, 
+00024e80: 312c 2031 2c20 312c 2031 2c20 312c 2031  1, 1, 1, 1, 1, 1
+00024e90: 2c20 312c 2031 2c20 312c 2031 2c20 312c  , 1, 1, 1, 1, 1,
+00024ea0: 2031 2c20 312c 2031 2c20 312c 2031 2c20   1, 1, 1, 1, 1, 
+00024eb0: 312c 2031 2c20 312c 2031 2c20 312c 2031  1, 1, 1, 1, 1, 1
+00024ec0: 2c20 312c 2032 2c20 322c 2032 2c20 322c  , 1, 2, 2, 2, 2,
+00024ed0: 2032 2c20 322c 2032 2c20 322c 2032 2c20   2, 2, 2, 2, 2, 
+00024ee0: 322c 2032 2c20 322c 2032 2c20 322c 2032  2, 2, 2, 2, 2, 2
+00024ef0: 2c20 322c 2032 2c20 322c 2032 2c20 322c  , 2, 2, 2, 2, 2,
+00024f00: 2032 2c20 322c 2032 2c20 322c 2032 2c20   2, 2, 2, 2, 2, 
+00024f10: 322c 2032 2c20 322c 2033 2c20 332c 2033  2, 2, 2, 3, 3, 3
+00024f20: 2c20 332c 2033 2c20 332c 2033 2c20 332c  , 3, 3, 3, 3, 3,
+00024f30: 2033 2c20 332c 2033 2c20 332c 2033 2c20   3, 3, 3, 3, 3, 
+00024f40: 332c 2033 2c20 332c 2033 2c20 332c 2033  3, 3, 3, 3, 3, 3
+00024f50: 2c20 332c 2033 2c20 332c 2033 2c20 332c  , 3, 3, 3, 3, 3,
+00024f60: 2033 2c20 332c 2033 2c20 332c 2033 2c20   3, 3, 3, 3, 3, 
+00024f70: 332c 2033 2c20 342c 2034 2c20 342c 2034  3, 3, 4, 4, 4, 4
+00024f80: 2c20 342c 2034 2c20 342c 2034 2c20 342c  , 4, 4, 4, 4, 4,
+00024f90: 2034 2c20 342c 2034 2c20 342c 2034 2c20   4, 4, 4, 4, 4, 
+00024fa0: 342c 2034 2c20 342c 2034 2c20 342c 2034  4, 4, 4, 4, 4, 4
+00024fb0: 2c20 342c 2034 2c20 342c 2034 2c20 342c  , 4, 4, 4, 4, 4,
+00024fc0: 2034 2c20 342c 2034 2c20 342c 2034 2c20   4, 4, 4, 4, 4, 
+00024fd0: 352c 2035 2c20 352c 2035 2c20 352c 2035  5, 5, 5, 5, 5, 5
+00024fe0: 2c20 352c 2035 2c20 352c 2035 2c20 352c  , 5, 5, 5, 5, 5,
+00024ff0: 2035 2c20 352c 2035 2c20 352c 2035 2c20   5, 5, 5, 5, 5, 
+00025000: 352c 2035 2c20 352c 2035 2c20 352c 2035  5, 5, 5, 5, 5, 5
+00025010: 2c20 352c 2035 2c20 352c 2035 2c20 352c  , 5, 5, 5, 5, 5,
+00025020: 2035 2c20 352c 2035 2c20 352c 2036 2c20   5, 5, 5, 5, 6, 
+00025030: 362c 2036 2c20 362c 2036 2c20 362c 2036  6, 6, 6, 6, 6, 6
+00025040: 2c20 362c 2036 2c20 362c 2036 2c20 362c  , 6, 6, 6, 6, 6,
+00025050: 2036 2c20 362c 2036 2c20 362c 2036 2c20   6, 6, 6, 6, 6, 
+00025060: 362c 2036 2c20 362c 2036 2c20 362c 2036  6, 6, 6, 6, 6, 6
+00025070: 2c20 362c 2036 2c20 362c 2036 2c20 362c  , 6, 6, 6, 6, 6,
+00025080: 2036 2c20 362c 2037 2c20 372c 2037 2c20   6, 6, 7, 7, 7, 
+00025090: 372c 2037 2c20 372c 2037 2c20 372c 2037  7, 7, 7, 7, 7, 7
+000250a0: 2c20 372c 2037 2c20 372c 2037 2c20 372c  , 7, 7, 7, 7, 7,
+000250b0: 2037 2c20 372c 2037 2c20 372c 2037 2c20   7, 7, 7, 7, 7, 
+000250c0: 372c 2037 2c20 372c 2037 2c20 372c 2037  7, 7, 7, 7, 7, 7
+000250d0: 2c20 372c 2037 2c20 372c 2037 2c20 372c  , 7, 7, 7, 7, 7,
+000250e0: 2037 2c20 382c 2038 2c20 382c 2038 2c20   7, 8, 8, 8, 8, 
+000250f0: 382c 2038 2c20 382c 2038 2c20 382c 2038  8, 8, 8, 8, 8, 8
+00025100: 2c20 382c 2038 2c20 382c 2038 2c20 382c  , 8, 8, 8, 8, 8,
+00025110: 2038 2c20 382c 2038 2c20 382c 2038 2c20   8, 8, 8, 8, 8, 
+00025120: 382c 2038 2c20 382c 2038 2c20 382c 2038  8, 8, 8, 8, 8, 8
+00025130: 2c20 382c 2038 2c20 382c 2038 2c20 382c  , 8, 8, 8, 8, 8,
+00025140: 2039 2c20 392c 2039 2c20 392c 2039 2c20   9, 9, 9, 9, 9, 
+00025150: 392c 2039 2c20 392c 2039 2c20 392c 2039  9, 9, 9, 9, 9, 9
+00025160: 2c20 392c 2039 2c20 392c 2039 2c20 392c  , 9, 9, 9, 9, 9,
+00025170: 2039 2c20 392c 2039 2c20 392c 2039 2c20   9, 9, 9, 9, 9, 
+00025180: 392c 2039 2c20 392c 2039 2c20 392c 2039  9, 9, 9, 9, 9, 9
+00025190: 2c20 392c 2039 2c20 392c 2031 302c 2031  , 9, 9, 9, 10, 1
+000251a0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
+000251b0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
+000251c0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
+000251d0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
+000251e0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
+000251f0: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
+00025200: 302c 2031 302c 2031 302c 2031 302c 2031  0, 10, 10, 10, 1
+00025210: 302c 2031 302c 2031 312c 2031 312c 2031  0, 10, 11, 11, 1
+00025220: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
+00025230: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
+00025240: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
+00025250: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
+00025260: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
+00025270: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
+00025280: 312c 2031 312c 2031 312c 2031 312c 2031  1, 11, 11, 11, 1
+00025290: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
+000252a0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
+000252b0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
+000252c0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
+000252d0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
+000252e0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
+000252f0: 322c 2031 322c 2031 322c 2031 322c 2031  2, 12, 12, 12, 1
+00025300: 322c 2031 322c 2031 3220 5d0d 0a6d 6f6e  2, 12, 12 ]..mon
+00025310: 7468 4461 7952 656d 6170 203d 205b 312c  thDayRemap = [1,
+00025320: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
+00025330: 372c 2038 2c20 392c 2031 302c 2031 312c  7, 8, 9, 10, 11,
+00025340: 2031 322c 2031 332c 2031 342c 2031 352c   12, 13, 14, 15,
+00025350: 2031 362c 2031 372c 2031 382c 2031 392c   16, 17, 18, 19,
+00025360: 2032 302c 2032 312c 2032 322c 2032 332c   20, 21, 22, 23,
+00025370: 2032 342c 2032 352c 2032 362c 2032 372c   24, 25, 26, 27,
+00025380: 2032 382c 2032 392c 2033 302c 2033 312c   28, 29, 30, 31,
+00025390: 2031 2c20 322c 2033 2c20 342c 2035 2c20   1, 2, 3, 4, 5, 
+000253a0: 362c 2037 2c20 382c 2039 2c20 3130 2c20  6, 7, 8, 9, 10, 
+000253b0: 3131 2c20 3132 2c20 3133 2c20 3134 2c20  11, 12, 13, 14, 
+000253c0: 3135 2c20 3136 2c20 3137 2c20 3138 2c20  15, 16, 17, 18, 
+000253d0: 3139 2c20 3230 2c20 3231 2c20 3232 2c20  19, 20, 21, 22, 
+000253e0: 3233 2c20 3234 2c20 3235 2c20 3236 2c20  23, 24, 25, 26, 
+000253f0: 3237 2c20 3238 2c20 312c 2032 2c20 332c  27, 28, 1, 2, 3,
+00025400: 2034 2c20 352c 2036 2c20 372c 2038 2c20   4, 5, 6, 7, 8, 
+00025410: 392c 2031 302c 2031 312c 2031 322c 2031  9, 10, 11, 12, 1
+00025420: 332c 2031 342c 2031 352c 2031 362c 2031  3, 14, 15, 16, 1
+00025430: 372c 2031 382c 2031 392c 2032 302c 2032  7, 18, 19, 20, 2
+00025440: 312c 2032 322c 2032 332c 2032 342c 2032  1, 22, 23, 24, 2
+00025450: 352c 2032 362c 2032 372c 2032 382c 2032  5, 26, 27, 28, 2
+00025460: 392c 2033 302c 2033 312c 2031 2c20 322c  9, 30, 31, 1, 2,
+00025470: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
+00025480: 382c 2039 2c20 3130 2c20 3131 2c20 3132  8, 9, 10, 11, 12
+00025490: 2c20 3133 2c20 3134 2c20 3135 2c20 3136  , 13, 14, 15, 16
+000254a0: 2c20 3137 2c20 3138 2c20 3139 2c20 3230  , 17, 18, 19, 20
+000254b0: 2c20 3231 2c20 3232 2c20 3233 2c20 3234  , 21, 22, 23, 24
+000254c0: 2c20 3235 2c20 3236 2c20 3237 2c20 3238  , 25, 26, 27, 28
+000254d0: 2c20 3239 2c20 3330 2c20 312c 2032 2c20  , 29, 30, 1, 2, 
+000254e0: 332c 2034 2c20 352c 2036 2c20 372c 2038  3, 4, 5, 6, 7, 8
+000254f0: 2c20 392c 2031 302c 2031 312c 2031 322c  , 9, 10, 11, 12,
+00025500: 2031 332c 2031 342c 2031 352c 2031 362c   13, 14, 15, 16,
+00025510: 2031 372c 2031 382c 2031 392c 2032 302c   17, 18, 19, 20,
+00025520: 2032 312c 2032 322c 2032 332c 2032 342c   21, 22, 23, 24,
+00025530: 2032 352c 2032 362c 2032 372c 2032 382c   25, 26, 27, 28,
+00025540: 2032 392c 2033 302c 2033 312c 2031 2c20   29, 30, 31, 1, 
+00025550: 322c 2033 2c20 342c 2035 2c20 362c 2037  2, 3, 4, 5, 6, 7
+00025560: 2c20 382c 2039 2c20 3130 2c20 3131 2c20  , 8, 9, 10, 11, 
+00025570: 3132 2c20 3133 2c20 3134 2c20 3135 2c20  12, 13, 14, 15, 
+00025580: 3136 2c20 3137 2c20 3138 2c20 3139 2c20  16, 17, 18, 19, 
+00025590: 3230 2c20 3231 2c20 3232 2c20 3233 2c20  20, 21, 22, 23, 
+000255a0: 3234 2c20 3235 2c20 3236 2c20 3237 2c20  24, 25, 26, 27, 
+000255b0: 3238 2c20 3239 2c20 3330 2c20 312c 2032  28, 29, 30, 1, 2
+000255c0: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
+000255d0: 2038 2c20 392c 2031 302c 2031 312c 2031   8, 9, 10, 11, 1
+000255e0: 322c 2031 332c 2031 342c 2031 352c 2031  2, 13, 14, 15, 1
+000255f0: 362c 2031 372c 2031 382c 2031 392c 2032  6, 17, 18, 19, 2
+00025600: 302c 2032 312c 2032 322c 2032 332c 2032  0, 21, 22, 23, 2
+00025610: 342c 2032 352c 2032 362c 2032 372c 2032  4, 25, 26, 27, 2
+00025620: 382c 2032 392c 2033 302c 2033 312c 2031  8, 29, 30, 31, 1
+00025630: 2c20 322c 2033 2c20 342c 2035 2c20 362c  , 2, 3, 4, 5, 6,
+00025640: 2037 2c20 382c 2039 2c20 3130 2c20 3131   7, 8, 9, 10, 11
+00025650: 2c20 3132 2c20 3133 2c20 3134 2c20 3135  , 12, 13, 14, 15
+00025660: 2c20 3136 2c20 3137 2c20 3138 2c20 3139  , 16, 17, 18, 19
+00025670: 2c20 3230 2c20 3231 2c20 3232 2c20 3233  , 20, 21, 22, 23
+00025680: 2c20 3234 2c20 3235 2c20 3236 2c20 3237  , 24, 25, 26, 27
+00025690: 2c20 3238 2c20 3239 2c20 3330 2c20 3331  , 28, 29, 30, 31
+000256a0: 2c20 312c 2032 2c20 332c 2034 2c20 352c  , 1, 2, 3, 4, 5,
+000256b0: 2036 2c20 372c 2038 2c20 392c 2031 302c   6, 7, 8, 9, 10,
+000256c0: 2031 312c 2031 322c 2031 332c 2031 342c   11, 12, 13, 14,
+000256d0: 2031 352c 2031 362c 2031 372c 2031 382c   15, 16, 17, 18,
+000256e0: 2031 392c 2032 302c 2032 312c 2032 322c   19, 20, 21, 22,
+000256f0: 2032 332c 2032 342c 2032 352c 2032 362c   23, 24, 25, 26,
+00025700: 2032 372c 2032 382c 2032 392c 2033 302c   27, 28, 29, 30,
+00025710: 2031 2c20 322c 2033 2c20 342c 2035 2c20   1, 2, 3, 4, 5, 
+00025720: 362c 2037 2c20 382c 2039 2c20 3130 2c20  6, 7, 8, 9, 10, 
+00025730: 3131 2c20 3132 2c20 3133 2c20 3134 2c20  11, 12, 13, 14, 
+00025740: 3135 2c20 3136 2c20 3137 2c20 3138 2c20  15, 16, 17, 18, 
+00025750: 3139 2c20 3230 2c20 3231 2c20 3232 2c20  19, 20, 21, 22, 
+00025760: 3233 2c20 3234 2c20 3235 2c20 3236 2c20  23, 24, 25, 26, 
+00025770: 3237 2c20 3238 2c20 3239 2c20 3330 2c20  27, 28, 29, 30, 
+00025780: 3331 2c20 312c 2032 2c20 332c 2034 2c20  31, 1, 2, 3, 4, 
+00025790: 352c 2036 2c20 372c 2038 2c20 392c 2031  5, 6, 7, 8, 9, 1
+000257a0: 302c 2031 312c 2031 322c 2031 332c 2031  0, 11, 12, 13, 1
+000257b0: 342c 2031 352c 2031 362c 2031 372c 2031  4, 15, 16, 17, 1
+000257c0: 382c 2031 392c 2032 302c 2032 312c 2032  8, 19, 20, 21, 2
+000257d0: 322c 2032 332c 2032 342c 2032 352c 2032  2, 23, 24, 25, 2
+000257e0: 362c 2032 372c 2032 382c 2032 392c 2033  6, 27, 28, 29, 3
+000257f0: 302c 2031 2c20 322c 2033 2c20 342c 2035  0, 1, 2, 3, 4, 5
+00025800: 2c20 362c 2037 2c20 382c 2039 2c20 3130  , 6, 7, 8, 9, 10
+00025810: 2c20 3131 2c20 3132 2c20 3133 2c20 3134  , 11, 12, 13, 14
+00025820: 2c20 3135 2c20 3136 2c20 3137 2c20 3138  , 15, 16, 17, 18
+00025830: 2c20 3139 2c20 3230 2c20 3231 2c20 3232  , 19, 20, 21, 22
+00025840: 2c20 3233 2c20 3234 2c20 3235 2c20 3236  , 23, 24, 25, 26
+00025850: 2c20 3237 2c20 3238 2c20 3239 2c20 3330  , 27, 28, 29, 30
+00025860: 2c20 3331 205d 0d0a 6a75 6c69 616e 4461  , 31 ]..julianDa
+00025870: 7920 3d20 5b31 2c20 322c 2033 2c20 342c  y = [1, 2, 3, 4,
+00025880: 2035 2c20 362c 2037 2c20 382c 2039 2c20   5, 6, 7, 8, 9, 
+00025890: 3130 2c20 3131 2c20 3132 2c20 3133 2c20  10, 11, 12, 13, 
+000258a0: 3134 2c20 3135 2c20 3136 2c20 3137 2c20  14, 15, 16, 17, 
+000258b0: 3138 2c20 3139 2c20 3230 2c20 3231 2c20  18, 19, 20, 21, 
+000258c0: 3232 2c20 3233 2c20 3234 2c20 3235 2c20  22, 23, 24, 25, 
+000258d0: 3236 2c20 3237 2c20 3238 2c20 3239 2c20  26, 27, 28, 29, 
+000258e0: 3330 2c20 3331 2c20 3332 2c20 3333 2c20  30, 31, 32, 33, 
+000258f0: 3334 2c20 3335 2c20 3336 2c20 3337 2c20  34, 35, 36, 37, 
+00025900: 3338 2c20 3339 2c20 3430 2c20 3431 2c20  38, 39, 40, 41, 
+00025910: 3432 2c20 3433 2c20 3434 2c20 3435 2c20  42, 43, 44, 45, 
+00025920: 3436 2c20 3437 2c20 3438 2c20 3439 2c20  46, 47, 48, 49, 
+00025930: 3530 2c20 3531 2c20 3532 2c20 3533 2c20  50, 51, 52, 53, 
+00025940: 3534 2c20 3535 2c20 3536 2c20 3537 2c20  54, 55, 56, 57, 
+00025950: 3538 2c20 3539 2c20 3630 2c20 3631 2c20  58, 59, 60, 61, 
+00025960: 3632 2c20 3633 2c20 3634 2c20 3635 2c20  62, 63, 64, 65, 
+00025970: 3636 2c20 3637 2c20 3638 2c20 3639 2c20  66, 67, 68, 69, 
+00025980: 3730 2c20 3731 2c20 3732 2c20 3733 2c20  70, 71, 72, 73, 
+00025990: 3734 2c20 3735 2c20 3736 2c20 3737 2c20  74, 75, 76, 77, 
+000259a0: 3738 2c20 3739 2c20 3830 2c20 3831 2c20  78, 79, 80, 81, 
+000259b0: 3832 2c20 3833 2c20 3834 2c20 3835 2c20  82, 83, 84, 85, 
+000259c0: 3836 2c20 3837 2c20 3838 2c20 3839 2c20  86, 87, 88, 89, 
+000259d0: 3930 2c20 3931 2c20 3932 2c20 3933 2c20  90, 91, 92, 93, 
+000259e0: 3934 2c20 3935 2c20 3936 2c20 3937 2c20  94, 95, 96, 97, 
+000259f0: 3938 2c20 3939 2c20 3130 302c 2031 3031  98, 99, 100, 101
+00025a00: 2c20 3130 322c 2031 3033 2c20 3130 342c  , 102, 103, 104,
+00025a10: 2031 3035 2c20 3130 362c 2031 3037 2c20   105, 106, 107, 
+00025a20: 3130 382c 2031 3039 2c20 3131 302c 2031  108, 109, 110, 1
+00025a30: 3131 2c20 3131 322c 2031 3133 2c20 3131  11, 112, 113, 11
+00025a40: 342c 2031 3135 2c20 3131 362c 2031 3137  4, 115, 116, 117
+00025a50: 2c20 3131 382c 2031 3139 2c20 3132 302c  , 118, 119, 120,
+00025a60: 2031 3231 2c20 3132 322c 2031 3233 2c20   121, 122, 123, 
+00025a70: 3132 342c 2031 3235 2c20 3132 362c 2031  124, 125, 126, 1
+00025a80: 3237 2c20 3132 382c 2031 3239 2c20 3133  27, 128, 129, 13
+00025a90: 302c 2031 3331 2c20 3133 322c 2031 3333  0, 131, 132, 133
+00025aa0: 2c20 3133 342c 2031 3335 2c20 3133 362c  , 134, 135, 136,
+00025ab0: 2031 3337 2c20 3133 382c 2031 3339 2c20   137, 138, 139, 
+00025ac0: 3134 302c 2031 3431 2c20 3134 322c 2031  140, 141, 142, 1
+00025ad0: 3433 2c20 3134 342c 2031 3435 2c20 3134  43, 144, 145, 14
+00025ae0: 362c 2031 3437 2c20 3134 382c 2031 3439  6, 147, 148, 149
+00025af0: 2c20 3135 302c 2031 3531 2c20 3135 322c  , 150, 151, 152,
+00025b00: 2031 3533 2c20 3135 342c 2031 3535 2c20   153, 154, 155, 
+00025b10: 3135 362c 2031 3537 2c20 3135 382c 2031  156, 157, 158, 1
+00025b20: 3539 2c20 3136 302c 2031 3631 2c20 3136  59, 160, 161, 16
+00025b30: 322c 2031 3633 2c20 3136 342c 2031 3635  2, 163, 164, 165
+00025b40: 2c20 3136 362c 2031 3637 2c20 3136 382c  , 166, 167, 168,
+00025b50: 2031 3639 2c20 3137 302c 2031 3731 2c20   169, 170, 171, 
+00025b60: 3137 322c 2031 3733 2c20 3137 342c 2031  172, 173, 174, 1
+00025b70: 3735 2c20 3137 362c 2031 3737 2c20 3137  75, 176, 177, 17
+00025b80: 382c 2031 3739 2c20 3138 302c 2031 3831  8, 179, 180, 181
+00025b90: 2c20 3138 322c 2031 3833 2c20 3138 342c  , 182, 183, 184,
+00025ba0: 2031 3835 2c20 3138 362c 2031 3837 2c20   185, 186, 187, 
+00025bb0: 3138 382c 2031 3839 2c20 3139 302c 2031  188, 189, 190, 1
+00025bc0: 3931 2c20 3139 322c 2031 3933 2c20 3139  91, 192, 193, 19
+00025bd0: 342c 2031 3935 2c20 3139 362c 2031 3937  4, 195, 196, 197
+00025be0: 2c20 3139 382c 2031 3939 2c20 3230 302c  , 198, 199, 200,
+00025bf0: 2032 3031 2c20 3230 322c 2032 3033 2c20   201, 202, 203, 
+00025c00: 3230 342c 2032 3035 2c20 3230 362c 2032  204, 205, 206, 2
+00025c10: 3037 2c20 3230 382c 2032 3039 2c20 3231  07, 208, 209, 21
+00025c20: 302c 2032 3131 2c20 3231 322c 2032 3133  0, 211, 212, 213
+00025c30: 2c20 3231 342c 2032 3135 2c20 3231 362c  , 214, 215, 216,
+00025c40: 2032 3137 2c20 3231 382c 2032 3139 2c20   217, 218, 219, 
+00025c50: 3232 302c 2032 3231 2c20 3232 322c 2032  220, 221, 222, 2
+00025c60: 3233 2c20 3232 342c 2032 3235 2c20 3232  23, 224, 225, 22
+00025c70: 362c 2032 3237 2c20 3232 382c 2032 3239  6, 227, 228, 229
+00025c80: 2c20 3233 302c 2032 3331 2c20 3233 322c  , 230, 231, 232,
+00025c90: 2032 3333 2c20 3233 342c 2032 3335 2c20   233, 234, 235, 
+00025ca0: 3233 362c 2032 3337 2c20 3233 382c 2032  236, 237, 238, 2
+00025cb0: 3339 2c20 3234 302c 2032 3431 2c20 3234  39, 240, 241, 24
+00025cc0: 322c 2032 3433 2c20 3234 342c 2032 3435  2, 243, 244, 245
+00025cd0: 2c20 3234 362c 2032 3437 2c20 3234 382c  , 246, 247, 248,
+00025ce0: 2032 3439 2c20 3235 302c 2032 3531 2c20   249, 250, 251, 
+00025cf0: 3235 322c 2032 3533 2c20 3235 342c 2032  252, 253, 254, 2
+00025d00: 3535 2c20 3235 362c 2032 3537 2c20 3235  55, 256, 257, 25
+00025d10: 382c 2032 3539 2c20 3236 302c 2032 3631  8, 259, 260, 261
+00025d20: 2c20 3236 322c 2032 3633 2c20 3236 342c  , 262, 263, 264,
+00025d30: 2032 3635 2c20 3236 362c 2032 3637 2c20   265, 266, 267, 
+00025d40: 3236 382c 2032 3639 2c20 3237 302c 2032  268, 269, 270, 2
+00025d50: 3731 2c20 3237 322c 2032 3733 2c20 3237  71, 272, 273, 27
+00025d60: 342c 2032 3735 2c20 3237 362c 2032 3737  4, 275, 276, 277
+00025d70: 2c20 3237 382c 2032 3739 2c20 3238 302c  , 278, 279, 280,
+00025d80: 2032 3831 2c20 3238 322c 2032 3833 2c20   281, 282, 283, 
+00025d90: 3238 342c 2032 3835 2c20 3238 362c 2032  284, 285, 286, 2
+00025da0: 3837 2c20 3238 382c 2032 3839 2c20 3239  87, 288, 289, 29
+00025db0: 302c 2032 3931 2c20 3239 322c 2032 3933  0, 291, 292, 293
+00025dc0: 2c20 3239 342c 2032 3935 2c20 3239 362c  , 294, 295, 296,
+00025dd0: 2032 3937 2c20 3239 382c 2032 3939 2c20   297, 298, 299, 
+00025de0: 3330 302c 2033 3031 2c20 3330 322c 2033  300, 301, 302, 3
+00025df0: 3033 2c20 3330 342c 2033 3035 2c20 3330  03, 304, 305, 30
+00025e00: 362c 2033 3037 2c20 3330 382c 2033 3039  6, 307, 308, 309
+00025e10: 2c20 3331 302c 2033 3131 2c20 3331 322c  , 310, 311, 312,
+00025e20: 2033 3133 2c20 3331 342c 2033 3135 2c20   313, 314, 315, 
+00025e30: 3331 362c 2033 3137 2c20 3331 382c 2033  316, 317, 318, 3
+00025e40: 3139 2c20 3332 302c 2033 3231 2c20 3332  19, 320, 321, 32
+00025e50: 322c 2033 3233 2c20 3332 342c 2033 3235  2, 323, 324, 325
+00025e60: 2c20 3332 362c 2033 3237 2c20 3332 382c  , 326, 327, 328,
+00025e70: 2033 3239 2c20 3333 302c 2033 3331 2c20   329, 330, 331, 
+00025e80: 3333 322c 2033 3333 2c20 3333 342c 2033  332, 333, 334, 3
+00025e90: 3335 2c20 3333 362c 2033 3337 2c20 3333  35, 336, 337, 33
+00025ea0: 382c 2033 3339 2c20 3334 302c 2033 3431  8, 339, 340, 341
+00025eb0: 2c20 3334 322c 2033 3433 2c20 3334 342c  , 342, 343, 344,
+00025ec0: 2033 3435 2c20 3334 362c 2033 3437 2c20   345, 346, 347, 
+00025ed0: 3334 382c 2033 3439 2c20 3335 302c 2033  348, 349, 350, 3
+00025ee0: 3531 2c20 3335 322c 2033 3533 2c20 3335  51, 352, 353, 35
+00025ef0: 342c 2033 3535 2c20 3335 362c 2033 3537  4, 355, 356, 357
+00025f00: 2c20 3335 382c 2033 3539 2c20 3336 302c  , 358, 359, 360,
+00025f10: 2033 3631 2c20 3336 322c 2033 3633 2c20   361, 362, 363, 
+00025f20: 3336 342c 2033 3635 205d 0d0a 0d0a 2323  364, 365 ]....##
+00025f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025f70: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
+00025f80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025f90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025fa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025fc0: 2323 0d0a 2346 756e 6374 696f 6e20 666f  ##..#Function fo
+00025fd0: 7220 6765 7474 696e 6720 7468 6520 6461  r getting the da
+00025fe0: 7465 206f 6620 7468 6520 7065 616b 206f  te of the peak o
+00025ff0: 6620 7665 6720 7669 676f 722d 2063 616e  f veg vigor- can
+00026000: 2068 616e 646c 6520 6261 6e64 7320 6e65   handle bands ne
+00026010: 6761 7469 7665 6c79 2063 6f72 7265 6c61  gatively correla
+00026020: 7465 6420 746f 2076 6567 2069 6e0d 0a23  ted to veg in..#
+00026030: 6368 616e 6765 4469 7244 6963 7420 6469  changeDirDict di
+00026040: 6374 696f 6e61 7279 2061 626f 7665 0d0a  ctionary above..
+00026050: 6465 6620 6765 7450 6561 6b44 6174 6528  def getPeakDate(
+00026060: 636f 6566 6673 2c70 6561 6b44 6972 6563  coeffs,peakDirec
+00026070: 7469 6f6e 203d 2031 293a 0d0a 0d0a 2020  tion = 1):....  
+00026080: 7369 6e20 3d20 636f 6566 6673 2e73 656c  sin = coeffs.sel
+00026090: 6563 7428 5b30 5d29 0d0a 2020 636f 7320  ect([0])..  cos 
+000260a0: 3d20 636f 6566 6673 2e73 656c 6563 7428  = coeffs.select(
+000260b0: 5b31 5d29 0d0a 0d0a 2020 2346 696e 6420  [1])....  #Find 
+000260c0: 7768 6572 6520 696e 2063 7963 6c65 2073  where in cycle s
+000260d0: 6c6f 7065 2069 7320 7a65 726f 0d0a 2020  lope is zero..  
+000260e0: 6772 6565 6e44 6174 6520 3d20 2828 7369  greenDate = ((si
+000260f0: 6e2e 6469 7669 6465 2863 6f73 2929 2e61  n.divide(cos)).a
+00026100: 7461 6e28 2929 2e64 6976 6964 6528 322a  tan()).divide(2*
+00026110: 6d61 7468 2e70 6929 2e72 656e 616d 6528  math.pi).rename(
+00026120: 5b27 7065 616b 4461 7465 275d 290d 0a20  ['peakDate']).. 
+00026130: 2067 7265 656e 4461 7465 4c61 7465 7220   greenDateLater 
+00026140: 3d20 6772 6565 6e44 6174 652e 6164 6428  = greenDate.add(
+00026150: 302e 3529 0d0a 2020 2343 6865 636b 2077  0.5)..  #Check w
+00026160: 6869 6368 2064 3120 736c 6f70 6520 3d20  hich d1 slope = 
+00026170: 3020 6973 2074 6865 206d 6178 2062 7920  0 is the max by 
+00026180: 7072 6564 6963 7469 6e67 206f 7574 2074  predicting out t
+00026190: 6865 2076 616c 7565 0d0a 2020 7072 6564  he value..  pred
+000261a0: 6963 7465 6431 203d 2063 6f65 6666 732e  icted1 = coeffs.
+000261b0: 7365 6c65 6374 285b 305d 295c 0d0a 2020  select([0])\..  
+000261c0: 2020 2020 2020 2020 2020 2020 2e61 6464              .add
+000261d0: 2873 696e 2e6d 756c 7469 706c 7928 6772  (sin.multiply(gr
+000261e0: 6565 6e44 6174 652e 6d75 6c74 6970 6c79  eenDate.multiply
+000261f0: 2832 2a6d 6174 682e 7069 292e 7369 6e28  (2*math.pi).sin(
+00026200: 2929 295c 0d0a 2020 2020 2020 2020 2020  )))\..          
+00026210: 2020 2020 2e61 6464 2863 6f73 2e6d 756c      .add(cos.mul
+00026220: 7469 706c 7928 6772 6565 6e44 6174 652e  tiply(greenDate.
+00026230: 6d75 6c74 6970 6c79 2832 2a6d 6174 682e  multiply(2*math.
+00026240: 7069 292e 636f 7328 2929 295c 0d0a 2020  pi).cos()))\..  
+00026250: 2020 2020 2020 2020 2020 2020 2e72 656e              .ren
+00026260: 616d 6528 5b27 7072 6564 6963 7465 6427  ame(['predicted'
+00026270: 5d29 5c0d 0a20 2020 2020 2020 2020 2020  ])\..           
+00026280: 2020 202e 6d75 6c74 6970 6c79 2865 652e     .multiply(ee.
+00026290: 496d 6167 652e 636f 6e73 7461 6e74 2870  Image.constant(p
+000262a0: 6561 6b44 6972 6563 7469 6f6e 2929 5c0d  eakDirection))\.
+000262b0: 0a20 2020 2020 2020 2020 2020 2020 202e  .              .
+000262c0: 6164 6442 616e 6473 2867 7265 656e 4461  addBands(greenDa
+000262d0: 7465 290d 0a20 2070 7265 6469 6374 6564  te)..  predicted
+000262e0: 3220 3d20 636f 6566 6673 2e73 656c 6563  2 = coeffs.selec
+000262f0: 7428 5b30 5d29 5c0d 0a20 2020 2020 2020  t([0])\..       
+00026300: 2020 2020 2020 202e 6164 6428 7369 6e2e         .add(sin.
+00026310: 6d75 6c74 6970 6c79 2867 7265 656e 4461  multiply(greenDa
+00026320: 7465 4c61 7465 722e 6d75 6c74 6970 6c79  teLater.multiply
+00026330: 2832 2a6d 6174 682e 7069 292e 7369 6e28  (2*math.pi).sin(
+00026340: 2929 295c 0d0a 2020 2020 2020 2020 2020  )))\..          
+00026350: 2020 2020 2e61 6464 2863 6f73 2e6d 756c      .add(cos.mul
+00026360: 7469 706c 7928 6772 6565 6e44 6174 654c  tiply(greenDateL
+00026370: 6174 6572 2e6d 756c 7469 706c 7928 322a  ater.multiply(2*
+00026380: 6d61 7468 2e70 6929 2e63 6f73 2829 2929  math.pi).cos()))
+00026390: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
+000263a0: 202e 7265 6e61 6d65 285b 2770 7265 6469   .rename(['predi
+000263b0: 6374 6564 275d 295c 0d0a 2020 2020 2020  cted'])\..      
+000263c0: 2020 2020 2020 2020 2e6d 756c 7469 706c          .multipl
+000263d0: 7928 6565 2e49 6d61 6765 2e63 6f6e 7374  y(ee.Image.const
+000263e0: 616e 7428 7065 616b 4469 7265 6374 696f  ant(peakDirectio
+000263f0: 6e29 295c 0d0a 2020 2020 2020 2020 2020  n))\..          
+00026400: 2020 2020 2e61 6464 4261 6e64 7328 6772      .addBands(gr
+00026410: 6565 6e44 6174 654c 6174 6572 290d 0a20  eenDateLater).. 
+00026420: 2066 696e 616c 4772 6565 6e44 6174 6520   finalGreenDate 
+00026430: 3d20 6565 2e49 6d61 6765 436f 6c6c 6563  = ee.ImageCollec
+00026440: 7469 6f6e 285b 7072 6564 6963 7465 6431  tion([predicted1
+00026450: 2c70 7265 6469 6374 6564 325d 292e 7175  ,predicted2]).qu
+00026460: 616c 6974 794d 6f73 6169 6328 2770 7265  alityMosaic('pre
+00026470: 6469 6374 6564 2729 2e73 656c 6563 7428  dicted').select(
+00026480: 5b27 7065 616b 4461 7465 275d 292e 7265  ['peakDate']).re
+00026490: 6e61 6d65 285b 2770 6561 6b4a 756c 6961  name(['peakJulia
+000264a0: 6e44 6179 275d 290d 0a0d 0a20 2066 696e  nDay'])....  fin
+000264b0: 616c 4772 6565 6e44 6174 6520 3d20 6669  alGreenDate = fi
+000264c0: 6e61 6c47 7265 656e 4461 7465 2e77 6865  nalGreenDate.whe
+000264d0: 7265 2866 696e 616c 4772 6565 6e44 6174  re(finalGreenDat
+000264e0: 652e 6c74 2830 292c 2067 7265 656e 4461  e.lt(0), greenDa
+000264f0: 7465 2e61 6464 2831 2929 2e6d 756c 7469  te.add(1)).multi
+00026500: 706c 7928 3336 3529 2e69 6e74 3136 2829  ply(365).int16()
+00026510: 3b0d 0a0d 0a20 2023 436f 6e76 6572 7420  ;....  #Convert 
+00026520: 746f 206d 6f6e 7468 2061 6e64 2064 6179  to month and day
+00026530: 206f 6620 6d6f 6e74 680d 0a20 2067 7265   of month..  gre
+00026540: 656e 4d6f 6e74 6820 3d20 6669 6e61 6c47  enMonth = finalG
+00026550: 7265 656e 4461 7465 2e72 656d 6170 286a  reenDate.remap(j
+00026560: 756c 6961 6e44 6179 2c6d 6f6e 7468 5265  ulianDay,monthRe
+00026570: 6d61 7029 2e72 656e 616d 6528 5b27 7065  map).rename(['pe
+00026580: 616b 4d6f 6e74 6827 5d29 0d0a 2020 6772  akMonth'])..  gr
+00026590: 6565 6e4d 6f6e 7468 4461 7920 3d20 6669  eenMonthDay = fi
+000265a0: 6e61 6c47 7265 656e 4461 7465 2e72 656d  nalGreenDate.rem
+000265b0: 6170 286a 756c 6961 6e44 6179 2c6d 6f6e  ap(julianDay,mon
+000265c0: 7468 4461 7952 656d 6170 292e 7265 6e61  thDayRemap).rena
+000265d0: 6d65 285b 2770 6561 6b44 6179 4f66 4d6f  me(['peakDayOfMo
+000265e0: 6e74 6827 5d29 0d0a 2020 6772 6565 6e53  nth'])..  greenS
+000265f0: 7461 636b 203d 2066 696e 616c 4772 6565  tack = finalGree
+00026600: 6e44 6174 652e 6164 6442 616e 6473 2867  nDate.addBands(g
+00026610: 7265 656e 4d6f 6e74 6829 2e61 6464 4261  reenMonth).addBa
+00026620: 6e64 7328 6772 6565 6e4d 6f6e 7468 4461  nds(greenMonthDa
+00026630: 7929 0d0a 2020 7265 7475 726e 2067 7265  y)..  return gre
+00026640: 656e 5374 6163 6b0d 0a20 2023 4d61 702e  enStack..  #Map.
+00026650: 6164 644c 6179 6572 2867 7265 656e 5374  addLayer(greenSt
+00026660: 6163 6b2c 7b27 6d69 6e27 3a31 2c27 6d61  ack,{'min':1,'ma
+00026670: 7827 3a31 327d 2c27 6772 6565 6e4d 6f6e  x':12},'greenMon
+00026680: 7468 272c 4661 6c73 6529 0d0a 0d0a 2323  th',False)....##
+00026690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000266a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000266b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000266c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000266d0: 2323 2323 2323 230d 0a23 2323 2323 2323  #######..#######
+000266e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000266f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026720: 2323 0d0a 2346 756e 6374 696f 6e20 666f  ##..#Function fo
+00026730: 7220 6765 7474 696e 6720 6c65 6674 2073  r getting left s
+00026740: 756d 2075 6e64 6572 2074 6865 2063 7572  um under the cur
+00026750: 7665 2066 6f72 2061 2073 696e 676c 6520  ve for a single 
+00026760: 6772 6f77 696e 6720 7365 6173 6f6e 0d0a  growing season..
+00026770: 2354 616b 6573 2063 6172 6520 6f66 206e  #Takes care of n
+00026780: 6f72 6d61 6c69 7a61 7469 6f6e 2062 7920  ormalization by 
+00026790: 666f 7263 696e 6720 7468 6520 6d69 6e20  forcing the min 
+000267a0: 7661 6c75 6520 616c 6f6e 6720 7468 6520  value along the 
+000267b0: 6375 7276 6520 300d 0a23 6279 2074 616b  curve 0..#by tak
+000267c0: 696e 6720 7468 6520 616d 706c 6974 7564  ing the amplitud
+000267d0: 6520 6173 2074 6865 2069 6e74 6572 6365  e as the interce
+000267e0: 7074 0d0a 2341 7373 756d 6573 2074 6865  pt..#Assumes the
+000267f0: 2073 696e 2061 6e64 2063 6f73 2063 6f65   sin and cos coe
+00026800: 6666 7320 6172 6520 7468 6520 6861 726d  ffs are the harm
+00026810: 436f 6566 6673 0d0a 2374 3020 6973 2074  Coeffs..#t0 is t
+00026820: 6865 2073 7461 7274 2074 696d 6520 2864  he start time (d
+00026830: 6566 6175 6c74 7320 746f 2030 2928 6d69  efaults to 0)(mi
+00026840: 6e20 7661 6c75 6520 7368 6f75 6c64 2062  n value should b
+00026850: 6520 6275 7420 646f 6573 6e27 7420 6861  e but doesn't ha
+00026860: 7665 2074 6f20 6265 2030 290d 0a23 7431  ve to be 0)..#t1
+00026870: 2069 7320 7468 6520 656e 6420 7469 6d65   is the end time
+00026880: 2028 6465 6661 756c 7473 2074 6f20 3129   (defaults to 1)
+00026890: 286d 6178 2076 616c 7565 2073 686f 756c  (max value shoul
+000268a0: 6420 6265 2062 7574 2064 6f65 736e 2774  d be but doesn't
+000268b0: 2068 6176 6520 746f 2062 6520 3129 0d0a   have to be 1)..
+000268c0: 0d0a 2345 7861 6d70 6c65 206f 6620 7768  ..#Example of wh
+000268d0: 6174 2074 6869 7320 636f 6465 2069 7320  at this code is 
+000268e0: 646f 696e 6720 6361 6e20 6265 2066 6f75  doing can be fou
+000268f0: 6e64 2068 6572 653a 0d0a 2320 2068 7474  nd here:..#  htt
+00026900: 703a 2f2f 7777 772e 776f 6c66 7261 6d61  p://www.wolframa
+00026910: 6c70 6861 2e63 6f6d 2f69 6e70 7574 2f3f  lpha.com/input/?
+00026920: 693d 696e 7465 6772 6174 652b 302e 3135  i=integrate+0.15
+00026930: 3934 3930 3734 3932 3339 3932 3135 372b  949074923992157+
+00026940: 2532 422b 2d30 2e30 3832 3837 3539 392a  %2B+-0.08287599*
+00026950: 7369 6e28 322b 5049 2b54 292b 2532 422b  sin(2+PI+T)+%2B+
+00026960: 2d30 2e31 3132 3532 3031 3036 3133 2a63  -0.11252010613*c
+00026970: 6f73 2832 2b50 492b 5429 2b2b 6672 6f6d  os(2+PI+T)++from
+00026980: 2b30 2b74 6f2b 310d 0a64 6566 2067 6574  +0+to+1..def get
+00026990: 4172 6561 556e 6465 7243 7572 7665 2868  AreaUnderCurve(h
+000269a0: 6172 6d43 6f65 6666 732c 7430 3d20 302c  armCoeffs,t0= 0,
+000269b0: 7431 203d 2031 293a 0d0a 0d0a 2020 2350  t1 = 1):....  #P
+000269c0: 756c 6c20 6170 6172 7420 7468 6520 6d6f  ull apart the mo
+000269d0: 6465 6c0d 0a20 2061 6d70 6c69 7475 6465  del..  amplitude
+000269e0: 203d 2068 6172 6d43 6f65 6666 732e 7365   = harmCoeffs.se
+000269f0: 6c65 6374 285b 315d 292e 6879 706f 7428  lect([1]).hypot(
+00026a00: 6861 726d 436f 6566 6673 2e73 656c 6563  harmCoeffs.selec
+00026a10: 7428 5b30 5d29 290d 0a20 2069 6e74 6572  t([0]))..  inter
+00026a20: 6563 6570 744e 6f72 6d61 6c69 7a65 6420  eceptNormalized 
+00026a30: 3d20 616d 706c 6974 7564 6523 5768 656e  = amplitude#When
+00026a40: 206d 616b 696e 6720 7468 6520 6d69 6e20   making the min 
+00026a50: 302c 2074 6865 2069 6e74 6572 6365 7074  0, the intercept
+00026a60: 2062 6563 6f6d 6573 2074 6865 2061 6d70   becomes the amp
+00026a70: 6c69 7475 6465 2028 7468 6520 6879 706f  litude (the hypo
+00026a80: 7465 6e75 7365 290d 0a20 2073 696e 203d  tenuse)..  sin =
+00026a90: 2068 6172 6d43 6f65 6666 732e 7365 6c65   harmCoeffs.sele
+00026aa0: 6374 285b 305d 290d 0a20 2063 6f73 203d  ct([0])..  cos =
+00026ab0: 2068 6172 6d43 6f65 6666 732e 7365 6c65   harmCoeffs.sele
+00026ac0: 6374 285b 315d 290d 0a0d 0a20 2023 4669  ct([1])....  #Fi
+00026ad0: 6e64 2074 6865 2073 756d 2066 726f 6d20  nd the sum from 
+00026ae0: 2d20 696e 6669 6e69 7479 2074 6f20 300d  - infinity to 0.
+00026af0: 0a20 2073 756d 3020 3d20 696e 7465 7265  .  sum0 = intere
+00026b00: 6365 7074 4e6f 726d 616c 697a 6564 2e6d  ceptNormalized.m
+00026b10: 756c 7469 706c 7928 7430 295c 0d0a 2020  ultiply(t0)\..  
+00026b20: 2020 2020 2020 2020 2020 2e73 7562 7472            .subtr
+00026b30: 6163 7428 7369 6e2e 6469 7669 6465 2832  act(sin.divide(2
+00026b40: 2a6d 6174 682e 7069 292e 6d75 6c74 6970  *math.pi).multip
+00026b50: 6c79 286d 6174 682e 7369 6e28 322a 6d61  ly(math.sin(2*ma
+00026b60: 7468 2e70 692a 7430 2929 295c 0d0a 2020  th.pi*t0)))\..  
+00026b70: 2020 2020 2020 2020 2020 2e61 6464 2863            .add(c
+00026b80: 6f73 2e64 6976 6964 6528 322a 6d61 7468  os.divide(2*math
+00026b90: 2e70 6929 2e6d 756c 7469 706c 7928 6d61  .pi).multiply(ma
+00026ba0: 7468 2e63 6f73 2832 2a6d 6174 682e 7069  th.cos(2*math.pi
+00026bb0: 2a74 3029 2929 0d0a 2020 2346 696e 6420  *t0)))..  #Find 
+00026bc0: 7468 6520 7375 6d20 6672 6f6d 202d 2069  the sum from - i
+00026bd0: 6e66 696e 6974 7920 746f 2031 0d0a 2020  nfinity to 1..  
+00026be0: 7375 6d31 203d 2069 6e74 6572 6563 6570  sum1 = interecep
+00026bf0: 744e 6f72 6d61 6c69 7a65 642e 6d75 6c74  tNormalized.mult
+00026c00: 6970 6c79 2874 3129 5c0d 0a20 2020 2020  iply(t1)\..     
+00026c10: 2020 202e 7375 6274 7261 6374 2873 696e     .subtract(sin
+00026c20: 2e64 6976 6964 6528 322a 6d61 7468 2e70  .divide(2*math.p
+00026c30: 6929 2e6d 756c 7469 706c 7928 6d61 7468  i).multiply(math
+00026c40: 2e73 696e 2832 2a6d 6174 682e 7069 2a74  .sin(2*math.pi*t
+00026c50: 3129 2929 5c0d 0a20 2020 2020 2020 202e  1)))\..        .
+00026c60: 6164 6428 636f 732e 6469 7669 6465 2832  add(cos.divide(2
+00026c70: 2a6d 6174 682e 7069 292e 6d75 6c74 6970  *math.pi).multip
+00026c80: 6c79 286d 6174 682e 636f 7328 322a 6d61  ly(math.cos(2*ma
+00026c90: 7468 2e70 692a 7431 2929 290d 0a20 2023  th.pi*t1)))..  #
+00026ca0: 4669 6e64 2074 6865 2064 6966 6665 7265  Find the differe
+00026cb0: 6e63 650d 0a20 206c 6566 7453 756d 203d  nce..  leftSum =
+00026cc0: 2073 756d 312e 7375 6274 7261 6374 2873   sum1.subtract(s
+00026cd0: 756d 3029 2e72 656e 616d 6528 5b27 4155  um0).rename(['AU
+00026ce0: 4327 5d29 0d0a 2020 7265 7475 726e 206c  C'])..  return l
+00026cf0: 6566 7453 756d 0d0a 0d0a 2323 2323 2323  eftSum....######
+00026d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026d40: 2323 230d 0a23 2323 2323 2323 2323 2323  ###..###########
+00026d50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026d80: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+00026d90: 6465 6620 6765 7450 6861 7365 416d 706c  def getPhaseAmpl
+00026da0: 6974 7564 6550 6561 6b28 636f 6566 6673  itudePeak(coeffs
+00026db0: 2c74 3020 3d20 302c 7431 203d 2031 293a  ,t0 = 0,t1 = 1):
+00026dc0: 0d0a 2020 2350 6172 7365 2074 6865 206d  ..  #Parse the m
+00026dd0: 6f64 656c 0d0a 2020 6261 6e64 4e61 6d65  odel..  bandName
+00026de0: 7320 3d20 636f 6566 6673 2e62 616e 644e  s = coeffs.bandN
+00026df0: 616d 6573 2829 0d0a 2020 6261 6e64 4e75  ames()..  bandNu
+00026e00: 6d62 6572 203d 2062 616e 644e 616d 6573  mber = bandNames
+00026e10: 2e6c 656e 6774 6828 290d 0a20 206e 6f44  .length()..  noD
+00026e20: 6570 656e 6465 6e74 7320 3d20 6565 2e4e  ependents = ee.N
+00026e30: 756d 6265 7228 636f 6566 6673 2e67 6574  umber(coeffs.get
+00026e40: 2827 6e6f 4465 7065 6e64 656e 7473 2729  ('noDependents')
+00026e50: 290d 0a20 206d 6f64 656c 4c65 6e67 7468  )..  modelLength
+00026e60: 203d 2065 652e 4e75 6d62 6572 2863 6f65   = ee.Number(coe
+00026e70: 6666 732e 6765 7428 276d 6f64 656c 4c65  ffs.get('modelLe
+00026e80: 6e67 7468 2729 290d 0a20 2069 6e74 6572  ngth'))..  inter
+00026e90: 6365 7074 4261 6e64 7320 3d20 6565 2e4c  ceptBands = ee.L
+00026ea0: 6973 742e 7365 7175 656e 6365 2830 2c62  ist.sequence(0,b
+00026eb0: 616e 644e 756d 6265 722e 7375 6274 7261  andNumber.subtra
+00026ec0: 6374 2831 292c 6d6f 6465 6c4c 656e 6774  ct(1),modelLengt
+00026ed0: 6829 0d0a 0d0a 2020 6d6f 6465 6c73 203d  h)....  models =
+00026ee0: 2065 652e 4c69 7374 2e73 6571 7565 6e63   ee.List.sequenc
+00026ef0: 6528 302c 6e6f 4465 7065 6e64 656e 7473  e(0,noDependents
+00026f00: 2e73 7562 7472 6163 7428 3129 290d 0a0d  .subtract(1))...
+00026f10: 0a20 2064 6566 206d 6f64 656c 4765 7474  .  def modelGett
+00026f20: 6572 286d 6e29 3a0d 0a20 2020 206d 6e20  er(mn):..    mn 
+00026f30: 3d20 6565 2e4e 756d 6265 7228 6d6e 290d  = ee.Number(mn).
+00026f40: 0a20 2020 2072 6574 7572 6e20 6261 6e64  .    return band
+00026f50: 4e61 6d65 732e 736c 6963 6528 6d6e 2e6d  Names.slice(mn.m
+00026f60: 756c 7469 706c 7928 6d6f 6465 6c4c 656e  ultiply(modelLen
+00026f70: 6774 6829 2c6d 6e2e 6d75 6c74 6970 6c79  gth),mn.multiply
+00026f80: 286d 6f64 656c 4c65 6e67 7468 292e 6164  (modelLength).ad
+00026f90: 6428 6d6f 6465 6c4c 656e 6774 6829 290d  d(modelLength)).
+00026fa0: 0a0d 0a20 2070 6172 7365 644d 6f64 656c  ...  parsedModel
+00026fb0: 203d 6d6f 6465 6c73 2e6d 6170 286d 6f64   =models.map(mod
+00026fc0: 656c 4765 7474 6572 290d 0a0d 0a0d 0a20  elGetter)...... 
+00026fd0: 2023 7072 696e 7428 2750 6172 7365 6420   #print('Parsed 
+00026fe0: 6861 726d 6f6e 6963 2072 6567 7265 7373  harmonic regress
+00026ff0: 696f 6e20 6d6f 6465 6c27 2c70 6172 7365  ion model',parse
+00027000: 644d 6f64 656c 290d 0a0d 0a20 2023 4974  dModel)....  #It
+00027010: 6572 6174 6520 6163 726f 7373 206d 6f64  erate across mod
+00027020: 656c 7320 746f 2063 6f6e 7665 7274 2074  els to convert t
+00027030: 6f20 7068 6173 652c 2061 6d70 6c69 7475  o phase, amplitu
+00027040: 6465 2c20 616e 6420 7065 616b 0d0a 2020  de, and peak..  
+00027050: 6465 6620 7061 7047 6574 7465 7228 706d  def papGetter(pm
+00027060: 293a 0d0a 2020 2020 706d 203d 2065 652e  ):..    pm = ee.
+00027070: 4c69 7374 2870 6d29 3b0d 0a20 2020 206d  List(pm);..    m
+00027080: 6f64 656c 436f 6566 6673 203d 2063 6f65  odelCoeffs = coe
+00027090: 6666 732e 7365 6c65 6374 2870 6d29 0d0a  ffs.select(pm)..
+000270a0: 0d0a 2020 2020 696e 7465 7263 6570 7420  ..    intercept 
+000270b0: 3d20 6d6f 6465 6c43 6f65 6666 732e 7365  = modelCoeffs.se
+000270c0: 6c65 6374 2827 2e2a 5f69 6e74 6572 6365  lect('.*_interce
+000270d0: 7074 2729 0d0a 2020 2020 6861 726d 436f  pt')..    harmCo
+000270e0: 6566 6673 203d 206d 6f64 656c 436f 6566  effs = modelCoef
+000270f0: 6673 2e73 656c 6563 7428 272e 2a5f 3230  fs.select('.*_20
+00027100: 305f 7965 6172 2729 0d0a 2020 2020 6f75  0_year')..    ou
+00027110: 744e 616d 6520 3d20 6565 2e53 7472 696e  tName = ee.Strin
+00027120: 6728 6565 2e53 7472 696e 6728 706d 2e67  g(ee.String(pm.g
+00027130: 6574 2831 2929 2e73 706c 6974 2827 5f27  et(1)).split('_'
+00027140: 292e 6765 7428 3029 290d 0a20 2020 2073  ).get(0))..    s
+00027150: 6967 6e20 3d20 6565 2e4e 756d 6265 7228  ign = ee.Number(
+00027160: 6565 2e44 6963 7469 6f6e 6172 7928 6368  ee.Dictionary(ch
+00027170: 616e 6765 4469 7244 6963 7429 2e67 6574  angeDirDict).get
+00027180: 286f 7574 4e61 6d65 2929 2e6d 756c 7469  (outName)).multi
+00027190: 706c 7928 2d31 290d 0a0d 0a20 2020 2061  ply(-1)....    a
+000271a0: 6d70 6c69 7475 6465 203d 2068 6172 6d43  mplitude = harmC
+000271b0: 6f65 6666 732e 7365 6c65 6374 285b 315d  oeffs.select([1]
+000271c0: 292e 6879 706f 7428 6861 726d 436f 6566  ).hypot(harmCoef
+000271d0: 6673 2e73 656c 6563 7428 5b30 5d29 295c  fs.select([0]))\
+000271e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000271f0: 2e6d 756c 7469 706c 7928 3229 5c0d 0a20  .multiply(2)\.. 
+00027200: 2020 2020 2020 2020 2020 2020 202e 7265               .re
+00027210: 6e61 6d65 285b 6f75 744e 616d 652e 6361  name([outName.ca
+00027220: 7428 275f 616d 706c 6974 7564 6527 295d  t('_amplitude')]
+00027230: 290d 0a20 2020 2070 6861 7365 203d 2068  )..    phase = h
+00027240: 6172 6d43 6f65 6666 732e 7365 6c65 6374  armCoeffs.select
+00027250: 285b 305d 292e 6174 616e 3228 6861 726d  ([0]).atan2(harm
+00027260: 436f 6566 6673 2e73 656c 6563 7428 5b31  Coeffs.select([1
+00027270: 5d29 295c 0d0a 2020 2020 2020 2020 2020  ]))\..          
+00027280: 2020 2020 2e75 6e69 7453 6361 6c65 282d      .unitScale(-
+00027290: 6d61 7468 2e70 692c 206d 6174 682e 7069  math.pi, math.pi
+000272a0: 295c 0d0a 2020 2020 2020 2020 2020 2020  )\..            
+000272b0: 2020 2e72 656e 616d 6528 5b6f 7574 4e61    .rename([outNa
+000272c0: 6d65 2e63 6174 2827 5f70 6861 7365 2729  me.cat('_phase')
+000272d0: 5d29 0d0a 0d0a 2020 2020 2347 6574 2070  ])....    #Get p
+000272e0: 6561 6b20 6461 7465 2069 6e66 6f0d 0a20  eak date info.. 
+000272f0: 2020 2070 6561 6b44 6174 6520 3d20 6765     peakDate = ge
+00027300: 7450 6561 6b44 6174 6528 6861 726d 436f  tPeakDate(harmCo
+00027310: 6566 6673 2c73 6967 6e29 0d0a 2020 2020  effs,sign)..    
+00027320: 7065 616b 4461 7465 4261 6e64 4e61 6d65  peakDateBandName
+00027330: 7320 3d20 7065 616b 4461 7465 2e62 616e  s = peakDate.ban
+00027340: 644e 616d 6573 2829 0d0a 2020 2020 7065  dNames()..    pe
+00027350: 616b 4461 7465 4261 6e64 4e61 6d65 7320  akDateBandNames 
+00027360: 3d20 7065 616b 4461 7465 4261 6e64 4e61  = peakDateBandNa
+00027370: 6d65 732e 6d61 7028 6c61 6d62 6461 2062  mes.map(lambda b
+00027380: 6e3a 206f 7574 4e61 6d65 2e63 6174 2865  n: outName.cat(e
+00027390: 652e 5374 7269 6e67 2827 5f27 292e 6361  e.String('_').ca
+000273a0: 7428 6565 2e53 7472 696e 6728 626e 2929  t(ee.String(bn))
+000273b0: 2929 0d0a 0d0a 2020 2020 2347 6574 2074  ))....    #Get t
+000273c0: 6865 206c 6566 7420 7375 6d0d 0a20 2020  he left sum..   
+000273d0: 206c 6566 7453 756d 203d 2067 6574 4172   leftSum = getAr
+000273e0: 6561 556e 6465 7243 7572 7665 2868 6172  eaUnderCurve(har
+000273f0: 6d43 6f65 6666 732c 7430 2c74 3129 0d0a  mCoeffs,t0,t1)..
+00027400: 2020 2020 6c65 6674 5375 6d42 616e 644e      leftSumBandN
+00027410: 616d 6573 203d 206c 6566 7453 756d 2e62  ames = leftSum.b
+00027420: 616e 644e 616d 6573 2829 0d0a 2020 2020  andNames()..    
+00027430: 6c65 6674 5375 6d42 616e 644e 616d 6573  leftSumBandNames
+00027440: 203d 206c 6566 7453 756d 4261 6e64 4e61   = leftSumBandNa
+00027450: 6d65 732e 6d61 7028 6c61 6d62 6461 2062  mes.map(lambda b
+00027460: 6e3a 206f 7574 4e61 6d65 2e63 6174 2865  n: outName.cat(e
+00027470: 652e 5374 7269 6e67 2827 5f27 292e 6361  e.String('_').ca
+00027480: 7428 6565 2e53 7472 696e 6728 626e 2929  t(ee.String(bn))
+00027490: 2929 0d0a 0d0a 2020 2020 7265 7475 726e  ))....    return
+000274a0: 2061 6d70 6c69 7475 6465 5c0d 0a20 2020   amplitude\..   
+000274b0: 2020 2020 2020 2020 202e 6164 6442 616e           .addBan
+000274c0: 6473 2870 6861 7365 295c 0d0a 2020 2020  ds(phase)\..    
+000274d0: 2020 2020 2020 2020 2e61 6464 4261 6e64          .addBand
+000274e0: 7328 7065 616b 4461 7465 2e72 656e 616d  s(peakDate.renam
+000274f0: 6528 7065 616b 4461 7465 4261 6e64 4e61  e(peakDateBandNa
+00027500: 6d65 7329 295c 0d0a 2020 2020 2020 2020  mes))\..        
+00027510: 2020 2020 2e61 6464 4261 6e64 7328 6c65      .addBands(le
+00027520: 6674 5375 6d2e 7265 6e61 6d65 286c 6566  ftSum.rename(lef
+00027530: 7453 756d 4261 6e64 4e61 6d65 7329 290d  tSumBandNames)).
+00027540: 0a0d 0a0d 0a0d 0a20 2023 436f 6e76 6572  .......  #Conver
+00027550: 7420 746f 2061 6e20 696d 6167 650d 0a20  t to an image.. 
+00027560: 2070 6861 7365 416d 706c 6974 7564 6520   phaseAmplitude 
+00027570: 3d70 6172 7365 644d 6f64 656c 2e6d 6170  =parsedModel.map
+00027580: 2870 6170 4765 7474 6572 290d 0a0d 0a20  (papGetter).... 
+00027590: 2070 6861 7365 416d 706c 6974 7564 6520   phaseAmplitude 
+000275a0: 3d20 6565 2e49 6d61 6765 436f 6c6c 6563  = ee.ImageCollec
+000275b0: 7469 6f6e 2e66 726f 6d49 6d61 6765 7328  tion.fromImages(
+000275c0: 7068 6173 6541 6d70 6c69 7475 6465 290d  phaseAmplitude).
+000275d0: 0a0d 0a20 2070 6861 7365 416d 706c 6974  ...  phaseAmplit
+000275e0: 7564 6520 3d20 6565 2e49 6d61 6765 2863  ude = ee.Image(c
+000275f0: 6f6c 6c65 6374 696f 6e54 6f49 6d61 6765  ollectionToImage
+00027600: 2870 6861 7365 416d 706c 6974 7564 6529  (phaseAmplitude)
+00027610: 292e 666c 6f61 7428 295c 0d0a 2020 2020  ).float()\..    
+00027620: 2020 2020 2e63 6f70 7950 726f 7065 7274      .copyPropert
+00027630: 6965 7328 636f 6566 6673 2c5b 2773 7973  ies(coeffs,['sys
+00027640: 7465 6d3a 7469 6d65 5f73 7461 7274 275d  tem:time_start']
+00027650: 290d 0a20 2023 7072 696e 7428 2770 6127  )..  #print('pa'
+00027660: 2c70 6861 7365 416d 706c 6974 7564 6529  ,phaseAmplitude)
+00027670: 3b0d 0a20 2072 6574 7572 6e20 7068 6173  ;..  return phas
+00027680: 6541 6d70 6c69 7475 6465 3b0d 0a0d 0a23  eAmplitude;....#
+00027690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000276a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000276b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000276c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000276d0: 2323 2323 2323 2323 0d0a 2323 2323 2323  ########..######
+000276e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000276f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027720: 2323 230d 0a23 4675 6e63 7469 6f6e 2066  ###..#Function f
+00027730: 6f72 2061 7070 6c79 696e 6720 6861 726d  or applying harm
+00027740: 6f6e 6963 2072 6567 7265 7373 696f 6e20  onic regression 
+00027750: 6d6f 6465 6c20 746f 2073 6574 206f 6620  model to set of 
+00027760: 7072 6564 6963 746f 7220 7365 7473 0d0a  predictor sets..
+00027770: 6465 6620 6e65 7750 7265 6469 6374 2863  def newPredict(c
+00027780: 6f65 6666 732c 6861 726d 6f6e 6963 7329  oeffs,harmonics)
+00027790: 3a0d 0a20 2023 5061 7273 6520 7468 6520  :..  #Parse the 
+000277a0: 6d6f 6465 6c0d 0a20 2062 616e 644e 616d  model..  bandNam
+000277b0: 6573 203d 2063 6f65 6666 732e 6261 6e64  es = coeffs.band
+000277c0: 4e61 6d65 7328 290d 0a20 2062 616e 644e  Names()..  bandN
+000277d0: 756d 6265 7220 3d20 6261 6e64 4e61 6d65  umber = bandName
+000277e0: 732e 6c65 6e67 7468 2829 0d0a 2020 6e6f  s.length()..  no
+000277f0: 4465 7065 6e64 656e 7473 203d 2065 652e  Dependents = ee.
+00027800: 4e75 6d62 6572 2863 6f65 6666 732e 6765  Number(coeffs.ge
+00027810: 7428 276e 6f44 6570 656e 6465 6e74 7327  t('noDependents'
+00027820: 2929 0d0a 2020 6d6f 6465 6c4c 656e 6774  ))..  modelLengt
+00027830: 6820 3d20 6565 2e4e 756d 6265 7228 636f  h = ee.Number(co
+00027840: 6566 6673 2e67 6574 2827 6d6f 6465 6c4c  effs.get('modelL
+00027850: 656e 6774 6827 2929 0d0a 2020 696e 7465  ength'))..  inte
+00027860: 7263 6570 7442 616e 6473 203d 2065 652e  rceptBands = ee.
+00027870: 4c69 7374 2e73 6571 7565 6e63 6528 302c  List.sequence(0,
+00027880: 6261 6e64 4e75 6d62 6572 2e73 7562 7472  bandNumber.subtr
+00027890: 6163 7428 3129 2c6d 6f64 656c 4c65 6e67  act(1),modelLeng
+000278a0: 7468 290d 0a20 2074 696d 6542 616e 6420  th)..  timeBand 
+000278b0: 3d20 6565 2e4c 6973 7428 6861 726d 6f6e  = ee.List(harmon
+000278c0: 6963 732e 6765 7428 2769 6e64 4261 6e64  ics.get('indBand
+000278d0: 4e61 6d65 7327 2929 2e67 6574 2830 290d  Names')).get(0).
+000278e0: 0a20 2061 6374 7561 6c42 616e 6473 203d  .  actualBands =
+000278f0: 2068 6172 6d6f 6e69 6373 2e67 6574 2827   harmonics.get('
+00027900: 6465 7042 616e 644e 756d 6265 7273 2729  depBandNumbers')
+00027910: 0d0a 2020 696e 6442 616e 6473 203d 2068  ..  indBands = h
+00027920: 6172 6d6f 6e69 6373 2e67 6574 2827 696e  armonics.get('in
+00027930: 6442 616e 644e 756d 6265 7273 2729 0d0a  dBandNumbers')..
+00027940: 2020 696e 6442 616e 644e 616d 6573 203d    indBandNames =
+00027950: 2065 652e 4c69 7374 2868 6172 6d6f 6e69   ee.List(harmoni
+00027960: 6373 2e67 6574 2827 696e 6442 616e 644e  cs.get('indBandN
+00027970: 616d 6573 2729 290d 0a20 2064 6570 4261  ames'))..  depBa
+00027980: 6e64 4e61 6d65 7320 3d20 6565 2e4c 6973  ndNames = ee.Lis
+00027990: 7428 6861 726d 6f6e 6963 732e 6765 7428  t(harmonics.get(
+000279a0: 2764 6570 4261 6e64 4e61 6d65 7327 2929  'depBandNames'))
+000279b0: 0d0a 2020 7072 6564 6963 7465 6442 616e  ..  predictedBan
+000279c0: 644e 616d 6573 203d 2064 6570 4261 6e64  dNames = depBand
+000279d0: 4e61 6d65 732e 6d61 7028 6c61 6d62 6461  Names.map(lambda
+000279e0: 2064 6570 626e 6d73 3a65 652e 5374 7269   depbnms:ee.Stri
+000279f0: 6e67 2864 6570 626e 6d73 292e 6361 7428  ng(depbnms).cat(
+00027a00: 275f 7072 6564 6963 7465 6427 2929 0d0a  '_predicted'))..
+00027a10: 2020 7072 6564 6963 7465 6442 616e 644e    predictedBandN
+00027a20: 756d 6265 7273 203d 2065 652e 4c69 7374  umbers = ee.List
+00027a30: 2e73 6571 7565 6e63 6528 302c 7072 6564  .sequence(0,pred
+00027a40: 6963 7465 6442 616e 644e 616d 6573 2e6c  ictedBandNames.l
+00027a50: 656e 6774 6828 292e 7375 6274 7261 6374  ength().subtract
+00027a60: 2831 2929 0d0a 0d0a 2020 6d6f 6465 6c73  (1))....  models
+00027a70: 203d 2065 652e 4c69 7374 2e73 6571 7565   = ee.List.seque
+00027a80: 6e63 6528 302c 6e6f 4465 7065 6e64 656e  nce(0,noDependen
+00027a90: 7473 2e73 7562 7472 6163 7428 3129 290d  ts.subtract(1)).
+00027aa0: 0a20 2064 6566 206d 6e47 6574 7465 7228  .  def mnGetter(
+00027ab0: 6d6e 293a 0d0a 2020 2020 6d6e 203d 2065  mn):..    mn = e
+00027ac0: 652e 4e75 6d62 6572 286d 6e29 0d0a 2020  e.Number(mn)..  
+00027ad0: 2020 7265 7475 726e 2062 616e 644e 616d    return bandNam
+00027ae0: 6573 2e73 6c69 6365 286d 6e2e 6d75 6c74  es.slice(mn.mult
+00027af0: 6970 6c79 286d 6f64 656c 4c65 6e67 7468  iply(modelLength
+00027b00: 292c 6d6e 2e6d 756c 7469 706c 7928 6d6f  ),mn.multiply(mo
+00027b10: 6465 6c4c 656e 6774 6829 2e61 6464 286d  delLength).add(m
+00027b20: 6f64 656c 4c65 6e67 7468 2929 0d0a 0d0a  odelLength))....
+00027b30: 2020 7061 7273 6564 4d6f 6465 6c20 3d6d    parsedModel =m
+00027b40: 6f64 656c 732e 6d61 7028 6d6e 4765 7474  odels.map(mnGett
+00027b50: 6572 290d 0a0d 0a20 2023 7072 696e 7428  er)....  #print(
+00027b60: 2750 6172 7365 6420 6861 726d 6f6e 6963  'Parsed harmonic
+00027b70: 2072 6567 7265 7373 696f 6e20 6d6f 6465   regression mode
+00027b80: 6c27 2c70 6172 7365 644d 6f64 656c 2c70  l',parsedModel,p
+00027b90: 7265 6469 6374 6564 4261 6e64 4e61 6d65  redictedBandName
+00027ba0: 7329 0d0a 0d0a 2020 2341 7070 6c79 2070  s)....  #Apply p
+00027bb0: 6172 7365 6420 6d6f 6465 6c0d 0a20 2064  arsed model..  d
+00027bc0: 6566 2070 7265 6447 6574 7465 7228 696d  ef predGetter(im
+00027bd0: 6729 3a0d 0a20 2020 2074 696d 6520 3d20  g):..    time = 
+00027be0: 696d 672e 7365 6c65 6374 2874 696d 6542  img.select(timeB
+00027bf0: 616e 6429 0d0a 2020 2020 6163 7475 616c  and)..    actual
+00027c00: 203d 2069 6d67 2e73 656c 6563 7428 6163   = img.select(ac
+00027c10: 7475 616c 4261 6e64 7329 2e66 6c6f 6174  tualBands).float
+00027c20: 2829 0d0a 2020 2020 7072 6564 6963 746f  ()..    predicto
+00027c30: 7242 616e 6473 203d 2069 6d67 2e73 656c  rBands = img.sel
+00027c40: 6563 7428 696e 6442 616e 644e 616d 6573  ect(indBandNames
+00027c50: 290d 0a0d 0a20 2020 2023 4974 6572 6174  )....    #Iterat
+00027c60: 6520 6163 726f 7373 2065 6163 6820 6d6f  e across each mo
+00027c70: 6465 6c20 666f 7220 6561 6368 2064 6570  del for each dep
+00027c80: 656e 6465 6e74 2076 6172 6961 626c 650d  endent variable.
+00027c90: 0a20 2020 2064 6566 2070 6d47 6574 7465  .    def pmGette
+00027ca0: 7228 706d 293a 0d0a 2020 2020 2020 706d  r(pm):..      pm
+00027cb0: 203d 2065 652e 4c69 7374 2870 6d29 0d0a   = ee.List(pm)..
+00027cc0: 2020 2020 2020 6d6f 6465 6c43 6f65 6666        modelCoeff
+00027cd0: 7320 3d20 636f 6566 6673 2e73 656c 6563  s = coeffs.selec
+00027ce0: 7428 706d 290d 0a20 2020 2020 206f 7574  t(pm)..      out
+00027cf0: 4e61 6d65 203d 2065 652e 5374 7269 6e67  Name = ee.String
+00027d00: 2870 6d2e 6765 7428 3129 292e 6361 7428  (pm.get(1)).cat(
+00027d10: 275f 7072 6564 6963 7465 6427 290d 0a20  '_predicted').. 
+00027d20: 2020 2020 2069 6e74 6572 6365 7074 203d       intercept =
+00027d30: 206d 6f64 656c 436f 6566 6673 2e73 656c   modelCoeffs.sel
+00027d40: 6563 7428 6d6f 6465 6c43 6f65 6666 732e  ect(modelCoeffs.
+00027d50: 6261 6e64 4e61 6d65 7328 292e 736c 6963  bandNames().slic
+00027d60: 6528 302c 3129 290d 0a20 2020 2020 206f  e(0,1))..      o
+00027d70: 7468 6572 7320 3d20 6d6f 6465 6c43 6f65  thers = modelCoe
+00027d80: 6666 732e 7365 6c65 6374 286d 6f64 656c  ffs.select(model
+00027d90: 436f 6566 6673 2e62 616e 644e 616d 6573  Coeffs.bandNames
+00027da0: 2829 2e73 6c69 6365 2831 2c4e 6f6e 6529  ().slice(1,None)
+00027db0: 290d 0a0d 0a20 2020 2020 2070 7265 6469  )....      predi
+00027dc0: 6374 6564 203d 2070 7265 6469 6374 6f72  cted = predictor
+00027dd0: 4261 6e64 732e 6d75 6c74 6970 6c79 286f  Bands.multiply(o
+00027de0: 7468 6572 7329 2e72 6564 7563 6528 6565  thers).reduce(ee
+00027df0: 2e52 6564 7563 6572 2e73 756d 2829 292e  .Reducer.sum()).
+00027e00: 6164 6428 696e 7465 7263 6570 7429 2e66  add(intercept).f
+00027e10: 6c6f 6174 2829 0d0a 2020 2020 2020 7265  loat()..      re
+00027e20: 7475 726e 2070 7265 6469 6374 6564 2e66  turn predicted.f
+00027e30: 6c6f 6174 2829 0d0a 0d0a 0d0a 2020 2020  loat()......    
+00027e40: 7072 6564 6963 7465 644c 6973 7420 3d70  predictedList =p
+00027e50: 6172 7365 644d 6f64 656c 2e6d 6170 2870  arsedModel.map(p
+00027e60: 6d47 6574 7465 7229 0d0a 0d0a 2020 2020  mGetter)....    
+00027e70: 2343 6f6e 7665 7274 2074 6f20 616e 2069  #Convert to an i
+00027e80: 6d61 6765 0d0a 2020 2020 7072 6564 6963  mage..    predic
+00027e90: 7465 644c 6973 7420 3d20 6565 2e49 6d61  tedList = ee.Ima
+00027ea0: 6765 436f 6c6c 6563 7469 6f6e 2e66 726f  geCollection.fro
+00027eb0: 6d49 6d61 6765 7328 7072 6564 6963 7465  mImages(predicte
+00027ec0: 644c 6973 7429 0d0a 2020 2020 7072 6564  dList)..    pred
+00027ed0: 6963 7465 6449 6d61 6765 203d 2063 6f6c  ictedImage = col
+00027ee0: 6c65 6374 696f 6e54 6f49 6d61 6765 2870  lectionToImage(p
+00027ef0: 7265 6469 6374 6564 4c69 7374 292e 7365  redictedList).se
+00027f00: 6c65 6374 2870 7265 6469 6374 6564 4261  lect(predictedBa
+00027f10: 6e64 4e75 6d62 6572 732c 7072 6564 6963  ndNumbers,predic
+00027f20: 7465 6442 616e 644e 616d 6573 290d 0a0d  tedBandNames)...
+00027f30: 0a20 2020 2023 5365 7420 736f 6d65 206d  .    #Set some m
+00027f40: 6574 6164 6174 610d 0a20 2020 206f 7574  etadata..    out
+00027f50: 203d 2061 6374 7561 6c2e 6164 6442 616e   = actual.addBan
+00027f60: 6473 2870 7265 6469 6374 6564 496d 6167  ds(predictedImag
+00027f70: 652e 666c 6f61 7428 2929 5c0d 0a20 2020  e.float())\..   
+00027f80: 202e 636f 7079 5072 6f70 6572 7469 6573   .copyProperties
+00027f90: 2869 6d67 2c5b 2773 7973 7465 6d3a 7469  (img,['system:ti
+00027fa0: 6d65 5f73 7461 7274 272c 2773 7973 7465  me_start','syste
+00027fb0: 6d3a 7469 6d65 5f65 6e64 275d 290d 0a20  m:time_end']).. 
+00027fc0: 2020 2072 6574 7572 6e20 6f75 740d 0a0d     return out...
+00027fd0: 0a20 2070 7265 6469 6374 6564 203d 6861  .  predicted =ha
+00027fe0: 726d 6f6e 6963 732e 6d61 7028 7072 6564  rmonics.map(pred
+00027ff0: 4765 7474 6572 290d 0a0d 0a20 2070 7265  Getter)....  pre
+00028000: 6469 6374 6564 203d 2065 652e 496d 6167  dicted = ee.Imag
+00028010: 6543 6f6c 6c65 6374 696f 6e28 7072 6564  eCollection(pred
+00028020: 6963 7465 6429 0d0a 0d0a 2020 234d 6170  icted)....  #Map
+00028030: 2e61 6464 4c61 7965 7228 7072 6564 6963  .addLayer(predic
+00028040: 7465 642c 7b7d 2c27 7072 6564 6963 7465  ted,{},'predicte
+00028050: 6427 2c46 616c 7365 290d 0a0d 0a20 2072  d',False)....  r
+00028060: 6574 7572 6e20 7072 6564 6963 7465 640d  eturn predicted.
+00028070: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
+00028080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000280a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000280b0: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
+000280c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000280d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000280e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000280f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028100: 2323 2323 2323 230d 0a23 4675 6e63 7469  #######..#Functi
+00028110: 6f6e 2074 6f20 6765 7420 6120 6475 6d6d  on to get a dumm
+00028120: 7920 696d 6167 6520 7374 6163 6b20 666f  y image stack fo
+00028130: 7220 7379 6e74 6865 7469 6320 7469 6d65  r synthetic time
+00028140: 2073 6572 6965 730d 0a64 6566 2067 6574   series..def get
+00028150: 4461 7465 5374 6163 6b28 7374 6172 7459  DateStack(startY
+00028160: 6561 722c 656e 6459 6561 722c 7374 6172  ear,endYear,star
+00028170: 744a 756c 6961 6e2c 656e 644a 756c 6961  tJulian,endJulia
+00028180: 6e2c 6672 6571 7565 6e63 7929 3a0d 0a20  n,frequency):.. 
+00028190: 2079 6561 7273 203d 2065 652e 4c69 7374   years = ee.List
+000281a0: 2e73 6571 7565 6e63 6528 7374 6172 7459  .sequence(startY
+000281b0: 6561 722c 656e 6459 6561 7229 0d0a 2020  ear,endYear)..  
+000281c0: 6461 7465 7320 3d20 6565 2e4c 6973 742e  dates = ee.List.
+000281d0: 7365 7175 656e 6365 2873 7461 7274 4a75  sequence(startJu
+000281e0: 6c69 616e 2c65 6e64 4a75 6c69 616e 2c66  lian,endJulian,f
+000281f0: 7265 7175 656e 6379 290d 0a0d 0a20 2064  requency)....  d
+00028200: 6566 2079 7247 6574 7465 7228 7972 293a  ef yrGetter(yr):
+00028210: 0d0a 2020 2020 6465 6620 6447 6574 7465  ..    def dGette
+00028220: 7228 6429 3a0d 0a20 2020 2020 2072 6574  r(d):..      ret
+00028230: 7572 6e20 6565 2e44 6174 652e 6672 6f6d  urn ee.Date.from
+00028240: 594d 4428 7972 2c31 2c31 292e 6164 7661  YMD(yr,1,1).adva
+00028250: 6e63 6528 642c 2764 6179 2729 0d0a 2020  nce(d,'day')..  
+00028260: 2020 6473 203d 2064 6174 6573 2e6d 6170    ds = dates.map
+00028270: 2864 4765 7474 6572 290d 0a20 2020 2072  (dGetter)..    r
+00028280: 6574 7572 6e20 6473 0d0a 0d0a 2020 6461  eturn ds....  da
+00028290: 7465 5365 7473 203d 2079 6561 7273 2e6d  teSets = years.m
+000282a0: 6170 2879 7247 6574 7465 7229 0d0a 0d0a  ap(yrGetter)....
+000282b0: 2020 6c20 3d20 7261 6e67 6528 312c 6c65    l = range(1,le
+000282c0: 6e28 696e 6465 784e 616d 6573 292b 3129  n(indexNames)+1)
+000282d0: 0d0a 2020 6c20 3d20 5b69 2569 2066 6f72  ..  l = [i%i for
+000282e0: 2069 2069 6e20 6c5d 0d0a 2020 6320 3d20   i in l]..  c = 
+000282f0: 6565 2e49 6d61 6765 286c 292e 7265 6e61  ee.Image(l).rena
+00028300: 6d65 2869 6e64 6578 4e61 6d65 7329 0d0a  me(indexNames)..
+00028310: 2020 6320 3d20 632e 6469 7669 6465 2863    c = c.divide(c
+00028320: 290d 0a0d 0a20 2064 6174 6553 6574 7320  )....  dateSets 
+00028330: 3d20 6461 7465 5365 7473 2e66 6c61 7474  = dateSets.flatt
+00028340: 656e 2829 0d0a 0d0a 2020 6465 6620 6474  en()....  def dt
+00028350: 4765 7474 6572 2864 7429 3a0d 0a20 2020  Getter(dt):..   
+00028360: 2064 7420 3d20 6565 2e44 6174 6528 6474   dt = ee.Date(dt
+00028370: 290d 0a20 2020 2079 203d 2064 742e 6765  )..    y = dt.ge
+00028380: 7428 2779 6561 7227 290d 0a20 2020 2064  t('year')..    d
+00028390: 203d 2064 742e 6765 7446 7261 6374 696f   = dt.getFractio
+000283a0: 6e28 2779 6561 7227 290d 0a20 2020 2069  n('year')..    i
+000283b0: 203d 2065 652e 496d 6167 6528 792e 6164   = ee.Image(y.ad
+000283c0: 6428 6429 292e 666c 6f61 7428 292e 7365  d(d)).float().se
+000283d0: 6c65 6374 285b 305d 2c5b 2779 6561 7227  lect([0],['year'
+000283e0: 5d29 0d0a 0d0a 2020 2020 6920 3d20 632e  ])....    i = c.
+000283f0: 6164 6442 616e 6473 2869 292e 666c 6f61  addBands(i).floa
+00028400: 7428 295c 0d0a 2020 2020 2020 2e73 6574  t()\..      .set
+00028410: 2827 7379 7374 656d 3a74 696d 655f 7374  ('system:time_st
+00028420: 6172 7427 2c64 742e 6d69 6c6c 6973 2829  art',dt.millis()
+00028430: 295c 0d0a 2020 2020 2020 2e73 6574 2827  )\..      .set('
+00028440: 7379 7374 656d 3a74 696d 655f 656e 6427  system:time_end'
+00028450: 2c64 742e 6164 7661 6e63 6528 6672 6571  ,dt.advance(freq
+00028460: 7565 6e63 792c 2764 6179 2729 2e6d 696c  uency,'day').mil
+00028470: 6c69 7328 2929 0d0a 2020 2020 7265 7475  lis())..    retu
+00028480: 726e 2069 0d0a 2020 7374 6163 6b20 3d20  rn i..  stack = 
+00028490: 6461 7465 5365 7473 2e6d 6170 2864 7447  dateSets.map(dtG
+000284a0: 6574 7465 7229 0d0a 2020 7374 6163 6b20  etter)..  stack 
+000284b0: 3d20 6565 2e49 6d61 6765 436f 6c6c 6563  = ee.ImageCollec
+000284c0: 7469 6f6e 2e66 726f 6d49 6d61 6765 7328  tion.fromImages(
+000284d0: 7374 6163 6b29 0d0a 2020 7265 7475 726e  stack)..  return
+000284e0: 2073 7461 636b 0d0a 0d0a 2323 2323 2323   stack....######
+000284f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028530: 2323 230d 0a23 2323 2323 2323 2323 2323  ###..###########
+00028540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028550: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028570: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+00028580: 6465 6620 6765 7448 6172 6d6f 6e69 6343  def getHarmonicC
+00028590: 6f65 6666 6963 6965 6e74 7341 6e64 4669  oefficientsAndFi
+000285a0: 7428 616c 6c49 6d61 6765 732c 696e 6465  t(allImages,inde
+000285b0: 784e 616d 6573 2c77 6869 6368 4861 726d  xNames,whichHarm
+000285c0: 6f6e 6963 7320 3d20 5b32 5d2c 6465 7472  onics = [2],detr
+000285d0: 656e 6420 3d20 4661 6c73 6529 3a0d 0a0d  end = False):...
+000285e0: 0a20 2023 5365 6c65 6374 2064 6573 6972  .  #Select desir
+000285f0: 6564 2062 616e 6473 0d0a 2020 616c 6c49  ed bands..  allI
+00028600: 6e64 6963 6573 203d 2061 6c6c 496d 6167  ndices = allImag
+00028610: 6573 2e73 656c 6563 7428 696e 6465 784e  es.select(indexN
+00028620: 616d 6573 290d 0a0d 0a20 2023 4164 6420  ames)....  #Add 
+00028630: 6461 7465 2062 616e 640d 0a20 2069 6620  date band..  if 
+00028640: 6465 7472 656e 643a 0d0a 2020 2020 616c  detrend:..    al
+00028650: 6c49 6e64 6963 6573 203d 2061 6c6c 496e  lIndices = allIn
+00028660: 6469 6365 732e 6d61 7028 6164 6444 6174  dices.map(addDat
+00028670: 6542 616e 6429 0d0a 2020 656c 7365 3a0d  eBand)..  else:.
+00028680: 0a20 2020 2061 6c6c 496e 6469 6365 7320  .    allIndices 
+00028690: 3d20 616c 6c49 6e64 6963 6573 2e6d 6170  = allIndices.map
+000286a0: 2861 6464 5965 6172 4672 6163 7469 6f6e  (addYearFraction
+000286b0: 4261 6e64 290d 0a0d 0a0d 0a20 2023 4164  Band)......  #Ad
+000286c0: 6420 696e 6465 7065 6e64 656e 7420 7072  d independent pr
+000286d0: 6564 6963 746f 7273 2028 6861 726d 6f6e  edictors (harmon
+000286e0: 6963 7329 0d0a 2020 7769 7468 4861 726d  ics)..  withHarm
+000286f0: 6f6e 6963 7320 3d20 6765 7448 6172 6d6f  onics = getHarmo
+00028700: 6e69 6373 3228 616c 6c49 6e64 6963 6573  nics2(allIndices
+00028710: 2c27 7965 6172 272c 7768 6963 6848 6172  ,'year',whichHar
+00028720: 6d6f 6e69 6373 2c64 6574 7265 6e64 290d  monics,detrend).
+00028730: 0a20 2077 6974 6848 6172 6d6f 6e69 6373  .  withHarmonics
+00028740: 426e 7320 3d20 6565 2e49 6d61 6765 2877  Bns = ee.Image(w
+00028750: 6974 6848 6172 6d6f 6e69 6373 2e66 6972  ithHarmonics.fir
+00028760: 7374 2829 292e 6261 6e64 4e61 6d65 7328  st()).bandNames(
+00028770: 292e 736c 6963 6528 6c65 6e28 696e 6465  ).slice(len(inde
+00028780: 784e 616d 6573 292b 312c 4e6f 6e65 290d  xNames)+1,None).
+00028790: 0a0d 0a20 2023 4f70 7469 6f6e 616c 6c79  ...  #Optionally
+000287a0: 2063 6861 7274 2074 6865 2063 6f6c 6c65   chart the colle
+000287b0: 6374 696f 6e20 7769 7468 2068 6172 6d6f  ction with harmo
+000287c0: 6e69 6373 0d0a 0d0a 2020 2346 6974 2061  nics....  #Fit a
+000287d0: 206c 696e 6561 7220 7265 6772 6573 7369   linear regressi
+000287e0: 6f6e 206d 6f64 656c 0d0a 2020 636f 6566  on model..  coef
+000287f0: 6673 203d 206e 6577 526f 6275 7374 4d75  fs = newRobustMu
+00028800: 6c74 6970 6c65 4c69 6e65 6172 3228 7769  ltipleLinear2(wi
+00028810: 7468 4861 726d 6f6e 6963 7329 0d0a 0d0a  thHarmonics)....
+00028820: 2020 2343 616e 2076 6973 7561 6c69 7a65    #Can visualize
+00028830: 2074 6865 2070 6861 7365 2061 6e64 2061   the phase and a
+00028840: 6d70 6c69 7475 6465 2069 6620 6f6e 6c79  mplitude if only
+00028850: 2074 6865 2066 6972 7374 2028 5b32 5d29   the first ([2])
+00028860: 2068 6172 6d6f 6e69 6320 6973 2063 686f   harmonic is cho
+00028870: 7365 6e0d 0a20 2023 2069 6620 7768 6963  sen..  # if whic
+00028880: 6848 6172 6d6f 6e69 6373 203d 3d20 327b  hHarmonics == 2{
+00028890: 0d0a 2020 2320 2020 2070 6120 3d20 6765  ..  #    pa = ge
+000288a0: 7450 6861 7365 416d 706c 6974 7564 6528  tPhaseAmplitude(
+000288b0: 636f 6566 6673 293b 0d0a 2020 2320 202f  coeffs);..  #  /
+000288c0: 2f20 5475 726e 2074 6865 2048 5356 2064  / Turn the HSV d
+000288d0: 6174 6120 696e 746f 2061 6e20 5247 4220  ata into an RGB 
+000288e0: 696d 6167 6520 616e 6420 6164 6420 6974  image and add it
+000288f0: 2074 6f20 7468 6520 6d61 702e 0d0a 2020   to the map...  
+00028900: 2320 2073 6561 736f 6e61 6c69 7479 203d  #  seasonality =
+00028910: 2070 612e 7365 6c65 6374 285b 312c 305d   pa.select([1,0]
+00028920: 292e 6164 6442 616e 6473 2861 6c6c 496e  ).addBands(allIn
+00028930: 6469 6365 732e 7365 6c65 6374 285b 696e  dices.select([in
+00028940: 6465 784e 616d 6573 5b30 5d5d 292e 6d65  dexNames[0]]).me
+00028950: 616e 2829 292e 6873 7654 6f52 6762 2829  an()).hsvToRgb()
+00028960: 3b0d 0a20 2023 2020 2f2f 204d 6170 2e61  ;..  #  // Map.a
+00028970: 6464 4c61 7965 7228 7365 6173 6f6e 616c  ddLayer(seasonal
+00028980: 6974 792c 207b 7d2c 2027 5365 6173 6f6e  ity, {}, 'Season
+00028990: 616c 6974 7927 293b 0d0a 2020 2320 207d  ality');..  #  }
+000289a0: 0d0a 0d0a 0d0a 0d0a 2020 234d 6170 2e61  ........  #Map.a
+000289b0: 6464 4c61 7965 7228 636f 6566 6673 2c7b  ddLayer(coeffs,{
+000289c0: 7d2c 2748 6172 6d6f 6e69 6320 5265 6772  },'Harmonic Regr
+000289d0: 6573 7369 6f6e 2043 6f65 6666 6963 6965  ession Coefficie
+000289e0: 6e74 7327 2c46 616c 7365 290d 0a20 2070  nts',False)..  p
+000289f0: 7265 6469 6374 6564 203d 206e 6577 5072  redicted = newPr
+00028a00: 6564 6963 7428 636f 6566 6673 2c77 6974  edict(coeffs,wit
+00028a10: 6848 6172 6d6f 6e69 6373 290d 0a20 2072  hHarmonics)..  r
+00028a20: 6574 7572 6e20 5b63 6f65 6666 732c 7072  eturn [coeffs,pr
+00028a30: 6564 6963 7465 645d 0d0a 2323 2323 2323  edicted]..######
+00028a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028a80: 2323 230d 0a23 2323 2323 2323 2323 2323  ###..###########
+00028a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028ac0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+00028ad0: 2353 696d 706c 6520 7072 6564 6963 7420  #Simple predict 
+00028ae0: 6675 6e63 7469 6f6e 2066 6f72 2068 6172  function for har
+00028af0: 6d6f 6e69 6320 636f 6566 6669 6369 656e  monic coefficien
+00028b00: 7473 0d0a 2345 7870 6563 7473 2063 6f65  ts..#Expects coe
+00028b10: 6666 7320 6672 6f6d 2067 6574 4861 726d  ffs from getHarm
+00028b20: 6f6e 6963 436f 6566 6669 6369 656e 7473  onicCoefficients
+00028b30: 416e 6446 6974 2066 756e 6374 696f 6e0d  AndFit function.
+00028b40: 0a23 4461 7465 2069 6d61 6765 2069 7320  .#Date image is 
+00028b50: 6578 7065 6374 6564 2074 6f20 6265 2079  expected to be y
+00028b60: 7979 792e 6464 2077 6865 7265 2064 6420  yyy.dd where dd 
+00028b70: 6973 2074 6865 2064 6179 206f 6620 7965  is the day of ye
+00028b80: 6172 202f 2033 3635 2028 7072 6f70 6f72  ar / 365 (propor
+00028b90: 7469 6f6e 206f 6620 7965 6172 290d 0a23  tion of year)..#
+00028ba0: 6578 2e20 7379 6e74 6849 6d61 6765 2863  ex. synthImage(c
+00028bb0: 6f65 6666 732c 6565 2e49 6d61 6765 285b  oeffs,ee.Image([
+00028bc0: 3230 3139 2e36 5d29 2c5b 2762 6c75 6527  2019.6]),['blue'
+00028bd0: 2c27 6772 6565 6e27 2c27 7265 6427 2c27  ,'green','red','
+00028be0: 6e69 7227 2c27 7377 6972 3127 2c27 7377  nir','swir1','sw
+00028bf0: 6972 3227 2c27 4e42 5227 2c27 4e44 5649  ir2','NBR','NDVI
+00028c00: 275d 2c5b 322c 345d 2c74 7275 6529 0d0a  '],[2,4],true)..
+00028c10: 6465 6620 7379 6e74 6849 6d61 6765 2863  def synthImage(c
+00028c20: 6f65 6666 732c 6461 7465 496d 6167 652c  oeffs,dateImage,
+00028c30: 696e 6465 784e 616d 6573 2c68 6172 6d6f  indexNames,harmo
+00028c40: 6e69 6373 2c64 6574 7265 6e64 293a 0d0a  nics,detrend):..
+00028c50: 2020 2353 6574 2075 7020 636f 6e73 7461    #Set up consta
+00028c60: 6e74 2069 6d61 6765 2074 6f20 6d75 6c74  nt image to mult
+00028c70: 6970 6c79 2063 6f65 6666 7320 6279 0d0a  iply coeffs by..
+00028c80: 2020 636f 6e73 7449 6d61 6765 203d 2065    constImage = e
+00028c90: 652e 496d 6167 6528 3129 0d0a 2020 6966  e.Image(1)..  if
+00028ca0: 2064 6574 7265 6e64 3a63 6f6e 7374 496d   detrend:constIm
+00028cb0: 6167 6520 3d20 636f 6e73 7449 6d61 6765  age = constImage
+00028cc0: 2e61 6464 4261 6e64 7328 6461 7465 496d  .addBands(dateIm
+00028cd0: 6167 6529 0d0a 2020 666f 7220 6861 726d  age)..  for harm
+00028ce0: 2069 6e20 6861 726d 6f6e 6963 733a 0d0a   in harmonics:..
+00028cf0: 2020 2020 636f 6e73 7449 6d61 6765 203d      constImage =
+00028d00: 2063 6f6e 7374 496d 6167 652e 6164 6442   constImage.addB
+00028d10: 616e 6473 2865 652e 496d 6167 6528 5b64  ands(ee.Image([d
+00028d20: 6174 6549 6d61 6765 2e6d 756c 7469 706c  ateImage.multipl
+00028d30: 7928 6861 726d 2a6d 6174 682e 7069 292e  y(harm*math.pi).
+00028d40: 7369 6e28 295d 292e 7265 6e61 6d65 285b  sin()]).rename([
+00028d50: 277b 7d5f 7369 6e27 2e66 6f72 6d61 7428  '{}_sin'.format(
+00028d60: 6861 726d 2a31 3030 295d 2929 2020 2020  harm*100)]))    
+00028d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028d80: 2020 200d 0a20 2066 6f72 2068 6172 6d20     ..  for harm 
+00028d90: 696e 2068 6172 6d6f 6e69 6373 3a0d 0a20  in harmonics:.. 
+00028da0: 2020 2063 6f6e 7374 496d 6167 6520 3d20     constImage = 
+00028db0: 636f 6e73 7449 6d61 6765 2e61 6464 4261  constImage.addBa
+00028dc0: 6e64 7328 6565 2e49 6d61 6765 285b 6461  nds(ee.Image([da
+00028dd0: 7465 496d 6167 652e 6d75 6c74 6970 6c79  teImage.multiply
+00028de0: 2868 6172 6d2a 6d61 7468 2e70 6929 2e63  (harm*math.pi).c
+00028df0: 6f73 2829 5d29 2e72 656e 616d 6528 5b27  os()]).rename(['
+00028e00: 7b7d 5f63 6f73 272e 666f 726d 6174 2868  {}_cos'.format(h
+00028e10: 6172 6d2a 3130 3029 5d29 290d 0a20 200d  arm*100)]))..  .
+00028e20: 0a20 2023 2063 6f65 6666 7373 426e 203d  .  # coeffssBn =
+00028e30: 2063 6f65 6666 732e 7365 6c65 6374 2865   coeffs.select(e
+00028e40: 652e 5374 7269 6e67 2869 6e64 6578 4e61  e.String(indexNa
+00028e50: 6d65 735b 305d 292e 6361 7428 275f 2e2a  mes[0]).cat('_.*
+00028e60: 2729 290d 0a20 2023 2070 7269 6e74 2863  '))..  # print(c
+00028e70: 6f6e 7374 496d 6167 652e 6261 6e64 4e61  onstImage.bandNa
+00028e80: 6d65 7328 292e 6765 7449 6e66 6f28 292c  mes().getInfo(),
+00028e90: 636f 6566 6673 7342 6e2e 6261 6e64 4e61  coeffssBn.bandNa
+00028ea0: 6d65 7328 292e 6765 7449 6e66 6f28 2929  mes().getInfo())
+00028eb0: 0d0a 2020 2350 7265 6469 6374 2076 616c  ..  #Predict val
+00028ec0: 7565 7320 666f 7220 6561 6368 2062 616e  ues for each ban
+00028ed0: 640d 0a20 206f 7574 203d 2065 652e 496d  d..  out = ee.Im
+00028ee0: 6167 6528 3129 3b0d 0a20 2064 6566 2070  age(1);..  def p
+00028ef0: 7265 6469 6374 5772 6170 7065 7228 626e  redictWrapper(bn
+00028f00: 2c6f 7574 293a 0d0a 2020 2020 626e 203d  ,out):..    bn =
+00028f10: 2065 652e 5374 7269 6e67 2862 6e29 0d0a   ee.String(bn)..
+00028f20: 2020 2020 2353 656c 6563 7420 636f 6566      #Select coef
+00028f30: 6673 2066 6f72 2074 6861 7420 6261 6e64  fs for that band
+00028f40: 0d0a 2020 2020 636f 6566 6673 7342 6e20  ..    coeffssBn 
+00028f50: 3d20 636f 6566 6673 2e73 656c 6563 7428  = coeffs.select(
+00028f60: 6565 2e53 7472 696e 6728 626e 292e 6361  ee.String(bn).ca
+00028f70: 7428 275f 2e2a 2729 290d 0a20 2020 2070  t('_.*'))..    p
+00028f80: 7265 6469 6374 6564 203d 2063 6f6e 7374  redicted = const
+00028f90: 496d 6167 652e 6d75 6c74 6970 6c79 2863  Image.multiply(c
+00028fa0: 6f65 6666 7373 426e 292e 7265 6475 6365  oeffssBn).reduce
+00028fb0: 2827 7375 6d27 292e 7265 6e61 6d65 2862  ('sum').rename(b
+00028fc0: 6e29 0d0a 2020 2020 7265 7475 726e 2065  n)..    return e
+00028fd0: 652e 496d 6167 6528 6f75 7429 2e61 6464  e.Image(out).add
+00028fe0: 4261 6e64 7328 7072 6564 6963 7465 6429  Bands(predicted)
+00028ff0: 0d0a 0d0a 2020 6f75 7420 3d20 6565 2e49  ....  out = ee.I
+00029000: 6d61 6765 2865 652e 4c69 7374 2869 6e64  mage(ee.List(ind
+00029010: 6578 4e61 6d65 7329 2e69 7465 7261 7465  exNames).iterate
+00029020: 2870 7265 6469 6374 5772 6170 7065 722c  (predictWrapper,
+00029030: 6f75 7429 293b 0d0a 0d0a 2020 6f75 7420  out));....  out 
+00029040: 3d20 6f75 742e 7365 6c65 6374 2865 652e  = out.select(ee.
+00029050: 4c69 7374 2e73 6571 7565 6e63 6528 312c  List.sequence(1,
+00029060: 206f 7574 2e62 616e 644e 616d 6573 2829   out.bandNames()
+00029070: 2e73 697a 6528 292e 7375 6274 7261 6374  .size().subtract
+00029080: 2831 2929 290d 0a0d 0a20 2072 6574 7572  (1)))....  retur
+00029090: 6e20 6f75 740d 0a23 2323 2323 2323 2323  n out..#########
+000290a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000290b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000290c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000290d0: 2323 2323 2323 2323 2323 2323 0d0a 2357  ############..#W
+000290e0: 7261 7070 6572 2066 756e 6374 696f 6e20  rapper function 
+000290f0: 746f 2067 6574 2063 6c69 6d61 7465 2064  to get climate d
+00029100: 6174 610d 0a23 2053 7570 706f 7274 733a  ata..# Supports:
+00029110: 0d0a 2320 4e41 5341 2f4f 524e 4c2f 4441  ..# NASA/ORNL/DA
+00029120: 594d 4554 5f56 330d 0a23 204e 4153 412f  YMET_V3..# NASA/
+00029130: 4f52 4e4c 2f44 4159 4d45 545f 5634 0d0a  ORNL/DAYMET_V4..
+00029140: 2320 5543 5342 2d43 4847 2f43 4849 5250  # UCSB-CHG/CHIRP
+00029150: 532f 4441 494c 5920 2870 7265 6369 7069  S/DAILY (precipi
+00029160: 7461 7469 6f6e 206f 6e6c 7929 0d0a 2361  tation only)..#a
+00029170: 6e64 2070 6f73 7369 626c 7920 6f74 6865  nd possibly othe
+00029180: 7273 0d0a 6465 6620 6765 7443 6c69 6d61  rs..def getClima
+00029190: 7465 5772 6170 7065 7228 636f 6c6c 6563  teWrapper(collec
+000291a0: 7469 6f6e 4e61 6d65 2c73 7475 6479 4172  tionName,studyAr
+000291b0: 6561 2c73 7461 7274 5965 6172 2c65 6e64  ea,startYear,end
+000291c0: 5965 6172 2c73 7461 7274 4a75 6c69 616e  Year,startJulian
+000291d0: 2c65 6e64 4a75 6c69 616e 2c74 696d 6562  ,endJulian,timeb
+000291e0: 7566 6665 722c 7765 6967 6874 732c 636f  uffer,weights,co
+000291f0: 6d70 6f73 6974 696e 6752 6564 7563 6572  mpositingReducer
+00029200: 2c65 7870 6f72 7443 6f6d 706f 7369 7465  ,exportComposite
+00029210: 7320 3d20 4661 6c73 652c 6578 706f 7274  s = False,export
+00029220: 5061 7468 526f 6f74 203d 204e 6f6e 652c  PathRoot = None,
+00029230: 6372 7320 3d20 4e6f 6e65 2c74 7261 6e73  crs = None,trans
+00029240: 666f 726d 203d 204e 6f6e 652c 7363 616c  form = None,scal
+00029250: 6520 3d20 4e6f 6e65 2c65 7870 6f72 7442  e = None,exportB
+00029260: 616e 6473 203d 204e 6f6e 6529 3a0d 0a20  ands = None):.. 
+00029270: 2061 7267 7320 3d20 666f 726d 6174 4172   args = formatAr
+00029280: 6773 286c 6f63 616c 7328 2929 0d0a 2020  gs(locals())..  
+00029290: 6966 2027 6172 6773 2720 696e 2061 7267  if 'args' in arg
+000292a0: 732e 6b65 7973 2829 3a0d 0a20 2020 2064  s.keys():..    d
+000292b0: 656c 2061 7267 735b 2761 7267 7327 5d0d  el args['args'].
+000292c0: 0a20 2070 7269 6e74 2861 7267 7329 0d0a  .  print(args)..
+000292d0: 0d0a 2020 2350 7265 7061 7265 2064 6174  ..  #Prepare dat
+000292e0: 6573 0d0a 2020 2357 7261 7020 7468 6520  es..  #Wrap the 
+000292f0: 6461 7465 7320 6966 206e 6565 6465 640d  dates if needed.
+00029300: 0a20 2077 7261 704f 6666 7365 7420 3d20  .  wrapOffset = 
+00029310: 300d 0a20 2069 6620 7374 6172 744a 756c  0..  if startJul
+00029320: 6961 6e20 3e20 656e 644a 756c 6961 6e3a  ian > endJulian:
+00029330: 0d0a 2020 2020 7772 6170 4f66 6673 6574  ..    wrapOffset
+00029340: 203d 2033 3635 0d0a 0d0a 2020 7374 6172   = 365....  star
+00029350: 7444 6174 6520 3d20 6565 2e44 6174 652e  tDate = ee.Date.
+00029360: 6672 6f6d 594d 4428 7374 6172 7459 6561  fromYMD(startYea
+00029370: 722c 312c 3129 2e61 6476 616e 6365 2873  r,1,1).advance(s
+00029380: 7461 7274 4a75 6c69 616e 2d31 2c27 6461  tartJulian-1,'da
+00029390: 7927 290d 0a20 2065 6e64 4461 7465 203d  y')..  endDate =
+000293a0: 2065 652e 4461 7465 2e66 726f 6d59 4d44   ee.Date.fromYMD
+000293b0: 2865 6e64 5965 6172 2c31 2c31 292e 6164  (endYear,1,1).ad
+000293c0: 7661 6e63 6528 656e 644a 756c 6961 6e2d  vance(endJulian-
+000293d0: 312b 7772 6170 4f66 6673 6574 2c27 6461  1+wrapOffset,'da
+000293e0: 7927 290d 0a20 2070 7269 6e74 2827 5374  y')..  print('St
+000293f0: 6172 7420 616e 6420 656e 6420 6461 7465  art and end date
+00029400: 733a 272c 2073 7461 7274 4461 7465 2e66  s:', startDate.f
+00029410: 6f72 6d61 7428 2759 5959 592d 4d4d 2d64  ormat('YYYY-MM-d
+00029420: 6427 292e 6765 7449 6e66 6f28 292c 2065  d').getInfo(), e
+00029430: 6e64 4461 7465 2e66 6f72 6d61 7428 2759  ndDate.format('Y
+00029440: 5959 592d 4d4d 2d64 6427 292e 6765 7449  YYY-MM-dd').getI
+00029450: 6e66 6f28 2929 0d0a 2020 7072 696e 7428  nfo())..  print(
+00029460: 274a 756c 6961 6e20 6461 7973 2061 7265  'Julian days are
+00029470: 3a27 2c73 7461 7274 4a75 6c69 616e 2c65  :',startJulian,e
+00029480: 6e64 4a75 6c69 616e 290d 0a0d 0a20 2023  ndJulian)....  #
+00029490: 4765 7420 636c 696d 6174 6520 6461 7461  Get climate data
+000294a0: 0d0a 2020 6320 3d20 6565 2e49 6d61 6765  ..  c = ee.Image
+000294b0: 436f 6c6c 6563 7469 6f6e 2863 6f6c 6c65  Collection(colle
+000294c0: 6374 696f 6e4e 616d 6529 5c0d 0a20 2020  ctionName)\..   
+000294d0: 2020 2020 2020 2020 2e66 696c 7465 7242          .filterB
+000294e0: 6f75 6e64 7328 7374 7564 7941 7265 6129  ounds(studyArea)
+000294f0: 5c0d 0a20 2020 2020 2020 2020 2020 2e66  \..           .f
+00029500: 696c 7465 7244 6174 6528 7374 6172 7444  ilterDate(startD
+00029510: 6174 652c 656e 6444 6174 652e 6164 7661  ate,endDate.adva
+00029520: 6e63 6528 312c 2764 6179 2729 295c 0d0a  nce(1,'day'))\..
+00029530: 2020 2020 2020 2020 2020 202e 6669 6c74             .filt
+00029540: 6572 2865 652e 4669 6c74 6572 2e63 616c  er(ee.Filter.cal
+00029550: 656e 6461 7252 616e 6765 2873 7461 7274  endarRange(start
+00029560: 4a75 6c69 616e 2c65 6e64 4a75 6c69 616e  Julian,endJulian
+00029570: 2929 0d0a 0d0a 2020 2353 6574 2074 6f20  ))....  #Set to 
+00029580: 6170 7072 6f70 7269 6174 6520 7265 7361  appropriate resa
+00029590: 6d70 6c69 6e67 206d 6574 686f 640d 0a20  mpling method.. 
+000295a0: 2063 203d 2063 2e6d 6170 286c 616d 6264   c = c.map(lambd
+000295b0: 6120 696d 673a 2069 6d67 2e72 6573 616d  a img: img.resam
+000295c0: 706c 6528 2762 6963 7562 6963 2729 290d  ple('bicubic')).
+000295d0: 0a20 204d 6170 2e61 6464 4c61 7965 7228  .  Map.addLayer(
+000295e0: 632c 7b7d 2c27 5261 7720 436c 696d 6174  c,{},'Raw Climat
+000295f0: 6527 2c46 616c 7365 290d 0a0d 0a20 2023  e',False)....  #
+00029600: 4372 6561 7465 2063 6f6d 706f 7369 7465  Create composite
+00029610: 2074 696d 6520 7365 7269 6573 0d0a 2020   time series..  
+00029620: 7473 203d 2063 6f6d 706f 7369 7465 5469  ts = compositeTi
+00029630: 6d65 5365 7269 6573 2863 2c73 7461 7274  meSeries(c,start
+00029640: 5965 6172 2c65 6e64 5965 6172 2c73 7461  Year,endYear,sta
+00029650: 7274 4a75 6c69 616e 2c65 6e64 4a75 6c69  rtJulian,endJuli
+00029660: 616e 2c74 696d 6562 7566 6665 722c 7765  an,timebuffer,we
+00029670: 6967 6874 732c 4e6f 6e65 2c63 6f6d 706f  ights,None,compo
+00029680: 7369 7469 6e67 5265 6475 6365 7229 0d0a  sitingReducer)..
+00029690: 2020 7473 203d 2065 652e 496d 6167 6543    ts = ee.ImageC
+000296a0: 6f6c 6c65 6374 696f 6e28 7473 2e6d 6170  ollection(ts.map
+000296b0: 286c 616d 6264 6120 6920 3a20 692e 666c  (lambda i : i.fl
+000296c0: 6f61 7428 2929 290d 0a0d 0a20 2023 4578  oat()))....  #Ex
+000296d0: 706f 7274 2063 6f6d 706f 7369 7465 2063  port composite c
+000296e0: 6f6c 6c65 6374 696f 6e0d 0a20 2069 6620  ollection..  if 
+000296f0: 6578 706f 7274 436f 6d70 6f73 6974 6573  exportComposites
+00029700: 3a0d 0a20 2020 2023 5365 7420 7570 2065  :..    #Set up e
+00029710: 7870 6f72 7420 6261 6e64 7320 6966 206e  xport bands if n
+00029720: 6f74 2073 7065 6369 6669 6564 0d0a 2020  ot specified..  
+00029730: 2020 6966 2065 7870 6f72 7442 616e 6473    if exportBands
+00029740: 203d 3d20 4e6f 6e65 3a0d 0a20 2020 2020   == None:..     
+00029750: 2065 7870 6f72 7442 616e 6473 203d 2065   exportBands = e
+00029760: 652e 4c69 7374 2865 652e 496d 6167 6528  e.List(ee.Image(
+00029770: 7473 2e66 6972 7374 2829 292e 6261 6e64  ts.first()).band
+00029780: 4e61 6d65 7328 2929 0d0a 0d0a 2020 2020  Names())....    
+00029790: 6578 706f 7274 436f 6c6c 6563 7469 6f6e  exportCollection
+000297a0: 2865 7870 6f72 7450 6174 6852 6f6f 742c  (exportPathRoot,
+000297b0: 636f 6c6c 6563 7469 6f6e 4e61 6d65 2e73  collectionName.s
+000297c0: 706c 6974 2827 2f27 295b 2d31 5d2c 7374  plit('/')[-1],st
+000297d0: 7564 7941 7265 612c 2063 7273 2c74 7261  udyArea, crs,tra
+000297e0: 6e73 666f 726d 2c73 6361 6c65 2c74 732c  nsform,scale,ts,
+000297f0: 7374 6172 7459 6561 722c 656e 6459 6561  startYear,endYea
+00029800: 722c 7374 6172 744a 756c 6961 6e2c 656e  r,startJulian,en
+00029810: 644a 756c 6961 6e2c 636f 6d70 6f73 6974  dJulian,composit
+00029820: 696e 6752 6564 7563 6572 2c74 696d 6562  ingReducer,timeb
+00029830: 7566 6665 722c 6578 706f 7274 4261 6e64  uffer,exportBand
+00029840: 7329 0d0a 0d0a 2020 7265 7475 726e 2074  s)....  return t
+00029850: 7323 2323 230d 0a23 2323 2323 2323 2323  s####..#########
+00029860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029890: 2323 2323 2323 2323 2323 2323 0d0a 2341  ############..#A
+000298a0: 6464 7320 6162 736f 6c75 7465 2064 6966  dds absolute dif
+000298b0: 6665 7265 6e63 6520 6672 6f6d 2061 2073  ference from a s
+000298c0: 7065 6369 6669 6564 2062 616e 6420 7375  pecified band su
+000298d0: 6d6d 6172 697a 6564 2062 7920 6120 7072  mmarized by a pr
+000298e0: 6f76 6964 6564 2070 6572 6365 6e74 696c  ovided percentil
+000298f0: 650d 0a23 496e 7465 6e64 6564 2066 6f72  e..#Intended for
+00029900: 2063 7573 746f 6d20 736f 7274 696e 6720   custom sorting 
+00029910: 6163 726f 7373 2063 6f6c 6c65 6374 696f  across collectio
+00029920: 6e73 0d0a 6465 6620 6164 6441 6273 4469  ns..def addAbsDi
+00029930: 6666 2869 6e43 6f6c 6c65 6374 696f 6e2c  ff(inCollection,
+00029940: 2071 7561 6c69 7479 4261 6e64 2c20 7065   qualityBand, pe
+00029950: 7263 656e 7469 6c65 2c73 6967 6e29 3a0d  rcentile,sign):.
+00029960: 0a20 2062 6573 7451 7561 6c69 7479 203d  .  bestQuality =
+00029970: 2069 6e43 6f6c 6c65 6374 696f 6e2e 7365   inCollection.se
+00029980: 6c65 6374 285b 7175 616c 6974 7942 616e  lect([qualityBan
+00029990: 645d 292e 7265 6475 6365 2865 652e 5265  d]).reduce(ee.Re
+000299a0: 6475 6365 722e 7065 7263 656e 7469 6c65  ducer.percentile
+000299b0: 285b 7065 7263 656e 7469 6c65 5d29 290d  ([percentile])).
+000299c0: 0a20 2064 6566 2077 2869 6d61 6765 293a  .  def w(image):
+000299d0: 0d0a 2020 2020 6465 6c74 6120 3d20 696d  ..    delta = im
+000299e0: 6167 652e 7365 6c65 6374 285b 7175 616c  age.select([qual
+000299f0: 6974 7942 616e 645d 292e 7375 6274 7261  ityBand]).subtra
+00029a00: 6374 2862 6573 7451 7561 6c69 7479 292e  ct(bestQuality).
+00029a10: 6162 7328 292e 6d75 6c74 6970 6c79 2873  abs().multiply(s
+00029a20: 6967 6e29 0d0a 2020 2020 7265 7475 726e  ign)..    return
+00029a30: 2069 6d61 6765 2e61 6464 4261 6e64 7328   image.addBands(
+00029a40: 6465 6c74 612e 7365 6c65 6374 285b 305d  delta.select([0]
+00029a50: 2c20 5b27 6465 6c74 6127 5d29 290d 0a20  , ['delta'])).. 
+00029a60: 206f 7574 203d 2069 6e43 6f6c 6c65 6374   out = inCollect
+00029a70: 696f 6e2e 6d61 7028 7729 0d0a 2020 7265  ion.map(w)..  re
+00029a80: 7475 726e 206f 7574 0d0a 0d0a 2323 2323  turn out....####
+00029a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029ad0: 230d 0a23 4d65 7468 6f64 2066 6f72 2061  #..#Method for a
+00029ae0: 7070 6c79 696e 6720 7468 6520 7175 616c  pplying the qual
+00029af0: 6974 794d 6f73 6169 6320 6675 6e63 7469  ityMosaic functi
+00029b00: 6f6e 2075 7369 6e67 2061 2073 7065 6369  on using a speci
+00029b10: 6669 6564 2070 6572 6365 6e74 696c 650d  fied percentile.
+00029b20: 0a23 5573 6566 756c 2077 6865 6e20 7468  .#Useful when th
+00029b30: 6520 6d61 7820 6f66 2074 6865 2071 7561  e max of the qua
+00029b40: 6c69 7479 2062 616e 6420 6973 206e 6f74  lity band is not
+00029b50: 2077 6861 7420 6973 2077 616e 7465 640d   what is wanted.
+00029b60: 0a64 6566 2063 7573 746f 6d51 7561 6c69  .def customQuali
+00029b70: 7479 4d6f 7361 6963 2869 6e43 6f6c 6c65  tyMosaic(inColle
+00029b80: 6374 696f 6e2c 7175 616c 6974 7942 616e  ction,qualityBan
+00029b90: 642c 7065 7263 656e 7469 6c65 293a 0d0a  d,percentile):..
+00029ba0: 2020 2341 6464 2061 6e20 6162 736f 6c75    #Add an absolu
+00029bb0: 7465 2064 6966 6665 7265 6e63 6520 6672  te difference fr
+00029bc0: 6f6d 2074 6865 2073 7065 6369 6669 6564  om the specified
+00029bd0: 2070 6572 6365 6e74 696c 650d 0a20 2023   percentile..  #
+00029be0: 5468 6973 2069 7320 696e 7665 7274 6564  This is inverted
+00029bf0: 2066 6f72 2074 6865 2071 7561 6c69 7479   for the quality
+00029c00: 4d6f 7361 6963 2066 756e 6374 696f 6e20  Mosaic function 
+00029c10: 746f 2070 726f 7065 726c 7920 7072 696f  to properly prio
+00029c20: 7269 7469 7a65 0d0a 2020 696e 436f 6c6c  ritize..  inColl
+00029c30: 6563 7469 6f6e 4465 6c74 6120 3d20 6164  ectionDelta = ad
+00029c40: 6441 6273 4469 6666 2869 6e43 6f6c 6c65  dAbsDiff(inColle
+00029c50: 6374 696f 6e2c 2071 7561 6c69 7479 4261  ction, qualityBa
+00029c60: 6e64 2c20 7065 7263 656e 7469 6c65 2c2d  nd, percentile,-
+00029c70: 3129 0d0a 0d0a 2020 2341 7070 6c79 2074  1)....  #Apply t
+00029c80: 6865 2071 7561 6c69 7479 4d6f 7361 6963  he qualityMosaic
+00029c90: 2066 756e 6374 696f 6e0d 0a20 2072 6574   function..  ret
+00029ca0: 7572 6e20 696e 436f 6c6c 6563 7469 6f6e  urn inCollection
+00029cb0: 4465 6c74 612e 7175 616c 6974 794d 6f73  Delta.qualityMos
+00029cc0: 6169 6328 2764 656c 7461 2729 0d0a 0d0a  aic('delta')....
+00029cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029d10: 2323 2323 230d 0a23 4f6e 2d74 6865 2d66  #####..#On-the-f
+00029d20: 6c79 2062 6173 6963 2077 6174 6572 206d  ly basic water m
+00029d30: 6173 6b69 6e67 206d 6574 686f 640d 0a23  asking method..#
+00029d40: 5468 6973 206d 6574 686f 6420 6973 2075  This method is u
+00029d50: 7365 6420 746f 2070 726f 7669 6465 2061  sed to provide a
+00029d60: 2074 696d 652d 7365 6e73 6974 6976 6520   time-sensitive 
+00029d70: 7761 7465 7220 6d61 736b 0d0a 2354 6869  water mask..#Thi
+00029d80: 7320 6d65 7468 6f64 2074 656e 6473 2074  s method tends t
+00029d90: 6f20 776f 726b 2077 656c 6c20 6966 2074  o work well if t
+00029da0: 6865 7265 2069 7320 6e6f 2077 6574 2073  here is no wet s
+00029db0: 6e6f 7720 7072 6573 656e 740d 0a23 5765  now present..#We
+00029dc0: 7420 736e 6f77 206f 7665 7220 666c 6174  t snow over flat
+00029dd0: 2061 7265 6173 2063 616e 2072 6573 756c   areas can resul
+00029de0: 7420 696e 2066 616c 7365 2070 6f73 6974  t in false posit
+00029df0: 6976 6573 0d0a 2344 6573 6967 6e65 6420  ives..#Designed 
+00029e00: 746f 2077 6f72 6b20 7769 7468 2054 4f41  to work with TOA
+00029e10: 2064 6174 612e 2053 5220 6461 7461 2077   data. SR data w
+00029e20: 696c 6c20 7265 7375 6c74 2069 6e20 6661  ill result in fa
+00029e30: 6c73 6520 6e65 6761 7469 7665 7320 286f  lse negatives (o
+00029e40: 6d69 7373 696f 6e29 0d0a 6465 6620 7369  mission)..def si
+00029e50: 6d70 6c65 5761 7465 724d 6173 6b28 696d  mpleWaterMask(im
+00029e60: 672c 636f 6e74 7261 6374 5069 7865 6c73  g,contractPixels
+00029e70: 203d 2030 2c73 6c6f 7065 5f74 6872 6573   = 0,slope_thres
+00029e80: 6820 3d20 3130 2c65 6c65 7661 7469 6f6e  h = 10,elevation
+00029e90: 496d 6167 6550 6174 6820 3d20 2255 5347  ImagePath = "USG
+00029ea0: 532f 3344 4550 2f31 306d 222c 656c 6576  S/3DEP/10m",elev
+00029eb0: 6174 696f 6e46 6f63 616c 4d65 616e 5261  ationFocalMeanRa
+00029ec0: 6469 7573 203d 2035 2e35 293a 0d0a 2020  dius = 5.5):..  
+00029ed0: 696d 6720 3d20 6164 6454 4341 6e67 6c65  img = addTCAngle
+00029ee0: 7328 696d 6729 0d0a 2020 6e65 6420 3d20  s(img)..  ned = 
+00029ef0: 6565 2e49 6d61 6765 2865 6c65 7661 7469  ee.Image(elevati
+00029f00: 6f6e 496d 6167 6550 6174 6829 2e72 6573  onImagePath).res
+00029f10: 616d 706c 6528 2762 6963 7562 6963 2729  ample('bicubic')
+00029f20: 0d0a 2020 736c 6f70 6520 3d20 6565 2e54  ..  slope = ee.T
+00029f30: 6572 7261 696e 2e73 6c6f 7065 286e 6564  errain.slope(ned
+00029f40: 2e66 6f63 616c 5f6d 6561 6e28 656c 6576  .focal_mean(elev
+00029f50: 6174 696f 6e46 6f63 616c 4d65 616e 5261  ationFocalMeanRa
+00029f60: 6469 7573 2929 0d0a 2020 666c 6174 203d  dius))..  flat =
+00029f70: 2073 6c6f 7065 2e6c 7465 2873 6c6f 7065   slope.lte(slope
+00029f80: 5f74 6872 6573 6829 0d0a 0d0a 2020 7761  _thresh)....  wa
+00029f90: 7465 724d 6173 6b20 3d20 696d 672e 7365  terMask = img.se
+00029fa0: 6c65 6374 285b 2774 6341 6e67 6c65 4257  lect(['tcAngleBW
+00029fb0: 275d 292e 6774 6528 2d30 2e30 3529 5c0d  ']).gte(-0.05)\.
+00029fc0: 0a20 2020 202e 416e 6428 696d 672e 7365  .    .And(img.se
+00029fd0: 6c65 6374 285b 2774 6341 6e67 6c65 4247  lect(['tcAngleBG
+00029fe0: 275d 292e 6c74 6528 302e 3035 2929 5c0d  ']).lte(0.05))\.
+00029ff0: 0a20 2020 202e 416e 6428 696d 672e 7365  .    .And(img.se
+0002a000: 6c65 6374 285b 2762 7269 6768 746e 6573  lect(['brightnes
+0002a010: 7327 5d29 2e6c 7428 302e 3329 295c 0d0a  s']).lt(0.3))\..
+0002a020: 2020 2020 2e41 6e64 2866 6c61 7429 2e66      .And(flat).f
+0002a030: 6f63 616c 5f6d 696e 2863 6f6e 7472 6163  ocal_min(contrac
+0002a040: 7450 6978 656c 7329 0d0a 0d0a 2020 7265  tPixels)....  re
+0002a050: 7475 726e 2077 6174 6572 4d61 736b 2e72  turn waterMask.r
+0002a060: 656e 616d 6528 5b27 7761 7465 724d 6173  ename(['waterMas
+0002a070: 6b27 5d29 0d0a 2323 2323 2323 2323 2323  k'])..##########
+0002a080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0002a090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0002a0a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0002a0b0: 2323 2323 2323 2323 2323 230d 0a23 4a65  ###########..#Je
+0002a0c0: 6666 2048 6f20 4d65 7468 6f64 2066 6f72  ff Ho Method for
+0002a0d0: 2061 6c67 616c 2062 6c6f 6f6d 2064 6574   algal bloom det
+0002a0e0: 6563 7469 6f6e 0d0a 2368 7474 7073 3a2f  ection..#https:/
+0002a0f0: 2f77 7777 2e6e 6174 7572 652e 636f 6d2f  /www.nature.com/
+0002a100: 6172 7469 636c 6573 2f73 3431 3538 362d  articles/s41586-
+0002a110: 3031 392d 3136 3438 2d37 0d0a 0d0a 2320  019-1648-7....# 
+0002a120: 5369 6d70 6c69 6669 6564 2053 6372 6970  Simplified Scrip
+0002a130: 7420 666f 7220 4c61 6e64 7361 7420 5761  t for Landsat Wa
+0002a140: 7465 7220 5175 616c 6974 790d 0a23 2050  ter Quality..# P
+0002a150: 726f 6475 6365 7320 6120 6d61 7020 6f66  roduces a map of
+0002a160: 2061 6e20 616c 6761 6c20 626c 6f6f 6d20   an algal bloom 
+0002a170: 696e 204c 616b 6520 4572 6965 206f 6e20  in Lake Erie on 
+0002a180: 3230 3131 2f39 2f33 0d0a 2320 4372 6561  2011/9/3..# Crea
+0002a190: 7465 6420 6f6e 2031 322f 372f 3230 3135  ted on 12/7/2015
+0002a1a0: 2062 7920 4a65 6666 2048 6f0d 0a0d 0a23   by Jeff Ho....#
+0002a1b0: 2053 7065 6369 6669 6573 2061 2074 6872   Specifies a thr
+0002a1c0: 6573 686f 6c64 2066 6f72 2068 7565 2074  eshold for hue t
+0002a1d0: 6f20 6573 7469 6d61 7465 2022 6772 6565  o estimate "gree
+0002a1e0: 6e22 2070 6978 656c 730d 0a23 2074 6869  n" pixels..# thi
+0002a1f0: 7320 6973 2075 7365 6420 6173 2061 6e20  s is used as an 
+0002a200: 6164 6469 7469 6f6e 616c 2066 696c 7465  additional filte
+0002a210: 7220 746f 2072 6566 696e 6520 7468 6520  r to refine the 
+0002a220: 616c 676f 7269 7468 6d20 6162 6f76 650d  algorithm above.
+0002a230: 0a64 6566 2048 6f43 616c 6347 7265 656e  .def HoCalcGreen
+0002a240: 6e65 7373 2869 6d67 293a 0d0a 2020 236d  ness(img):..  #m
+0002a250: 6170 2072 2c20 672c 2061 6e64 2062 2066  ap r, g, and b f
+0002a260: 6f72 206d 6f72 6520 7265 6164 6162 6c65  or more readable
+0002a270: 2061 6c67 6562 7261 2062 656c 6f77 0d0a   algebra below..
+0002a280: 2020 7220 3d20 696d 672e 7365 6c65 6374    r = img.select
+0002a290: 285b 2772 6564 275d 290d 0a20 2067 203d  (['red'])..  g =
+0002a2a0: 2069 6d67 2e73 656c 6563 7428 5b27 6772   img.select(['gr
+0002a2b0: 6565 6e27 5d29 0d0a 2020 6220 3d20 696d  een'])..  b = im
+0002a2c0: 672e 7365 6c65 6374 285b 2762 6c75 6527  g.select(['blue'
+0002a2d0: 5d29 0d0a 0d0a 2020 2363 616c 6375 6c61  ])....  #calcula
+0002a2e0: 7465 2069 6e74 656e 7369 7479 2c20 6875  te intensity, hu
+0002a2f0: 650d 0a20 2049 203d 2072 2e61 6464 2867  e..  I = r.add(g
+0002a300: 292e 6164 6428 6229 2e72 656e 616d 6528  ).add(b).rename(
+0002a310: 5b27 4927 5d29 0d0a 2020 6d69 6e73 203d  ['I'])..  mins =
+0002a320: 2072 2e6d 696e 2867 292e 6d69 6e28 6229   r.min(g).min(b)
+0002a330: 2e72 656e 616d 6528 5b27 6d69 6e73 275d  .rename(['mins']
+0002a340: 290d 0a20 2048 203d 206d 696e 732e 7768  )..  H = mins.wh
+0002a350: 6572 6528 6d69 6e73 2e65 7128 7229 2c28  ere(mins.eq(r),(
+0002a360: 622e 7375 6274 7261 6374 2872 2929 2e64  b.subtract(r)).d
+0002a370: 6976 6964 6528 492e 7375 6274 7261 6374  ivide(I.subtract
+0002a380: 2872 2e6d 756c 7469 706c 7928 3329 2929  (r.multiply(3)))
+0002a390: 2e61 6464 2831 2920 290d 0a20 2048 203d  .add(1) )..  H =
+0002a3a0: 2048 2e77 6865 7265 286d 696e 732e 6571   H.where(mins.eq
+0002a3b0: 2867 292c 2872 2e73 7562 7472 6163 7428  (g),(r.subtract(
+0002a3c0: 6729 292e 6469 7669 6465 2849 2e73 7562  g)).divide(I.sub
+0002a3d0: 7472 6163 7428 672e 6d75 6c74 6970 6c79  tract(g.multiply
+0002a3e0: 2833 2929 292e 6164 6428 3229 2029 0d0a  (3))).add(2) )..
+0002a3f0: 2020 4820 3d20 482e 7768 6572 6528 6d69    H = H.where(mi
+0002a400: 6e73 2e65 7128 6229 2c28 672e 7375 6274  ns.eq(b),(g.subt
+0002a410: 7261 6374 2862 2929 2e64 6976 6964 6528  ract(b)).divide(
+0002a420: 492e 7375 6274 7261 6374 2862 2e6d 756c  I.subtract(b.mul
+0002a430: 7469 706c 7928 3329 2929 2029 0d0a 0d0a  tiply(3))) )....
+0002a440: 2020 2370 6978 656c 7320 7769 7468 2068    #pixels with h
+0002a450: 7565 2062 656c 6f77 2031 2e36 206d 6f72  ue below 1.6 mor
+0002a460: 6520 6c69 6b65 6c79 2074 6f20 6265 2062  e likely to be b
+0002a470: 6c6f 6f6d 2061 6e64 206e 6f74 2073 7573  loom and not sus
+0002a480: 7065 6e64 6564 2073 6564 696d 656e 740d  pended sediment.
+0002a490: 0a20 2048 7468 7265 7368 203d 2048 2e6c  .  Hthresh = H.l
+0002a4a0: 7465 2831 2e36 290d 0a0d 0a20 2072 6574  te(1.6)....  ret
+0002a4b0: 7572 6e20 482e 7265 6e61 6d65 2827 4827  urn H.rename('H'
+0002a4c0: 290d 0a0d 0a0d 0a23 4170 706c 7920 626c  )......#Apply bl
+0002a4d0: 6f6f 6d20 6465 7465 6374 696f 6e20 616c  oom detection al
+0002a4e0: 676f 7269 7468 6d0d 0a64 6566 2048 6f43  gorithm..def HoC
+0002a4f0: 616c 6341 6c67 6f72 6974 686d 3128 696d  alcAlgorithm1(im
+0002a500: 6167 6529 3a0d 0a20 2074 7275 6563 6f6c  age):..  truecol
+0002a510: 6f72 203d 2031 2023 7368 6f77 2074 7275  or = 1 #show tru
+0002a520: 6520 636f 6c6f 7220 696d 6167 6520 6173  e color image as
+0002a530: 2077 656c 6c0d 0a20 2074 6573 7454 6872   well..  testThr
+0002a540: 6573 6820 3d20 4661 6c73 6520 2320 6164  esh = False # ad
+0002a550: 6420 6120 6269 6e61 7279 2069 6d61 6765  d a binary image
+0002a560: 2063 6c61 7373 6966 7969 6e67 2069 6e74   classifying int
+0002a570: 6f20 2262 6c6f 6f6d 2261 6e64 2022 6e6f  o "bloom"and "no
+0002a580: 6e2d 626c 6f6f 6d0d 0a20 2062 6c6f 6f6d  n-bloom..  bloom
+0002a590: 5468 7265 7368 6f6c 6420 3d20 302e 3032  Threshold = 0.02
+0002a5a0: 3334 3620 2374 6872 6573 686f 6c64 2066  346 #threshold f
+0002a5b0: 6f72 2063 6c61 7373 6966 6963 6174 696f  or classificatio
+0002a5c0: 6e20 6669 7420 6261 7365 6420 6f6e 206f  n fit based on o
+0002a5d0: 7468 6572 2064 6174 610d 0a20 2067 7265  ther data..  gre
+0002a5e0: 656e 6573 7354 6872 6573 686f 6c64 203d  enessThreshold =
+0002a5f0: 2031 2e36 0d0a 0d0a 2020 2320 416c 676f   1.6....  # Algo
+0002a600: 7269 7468 6d20 3120 6261 7365 6420 6f6e  rithm 1 based on
+0002a610: 3a0d 0a20 2023 2057 616e 672c 204d 2e2c  :..  # Wang, M.,
+0002a620: 2026 2053 6869 2c20 572e 2028 3230 3037   & Shi, W. (2007
+0002a630: 292e 2054 6865 204e 4952 2d53 5749 5220  ). The NIR-SWIR 
+0002a640: 636f 6d62 696e 6564 2061 746d 6f73 7068  combined atmosph
+0002a650: 6572 6963 0d0a 2020 2320 2063 6f72 7265  eric..  #  corre
+0002a660: 6374 696f 6e20 6170 7072 6f61 6368 2066  ction approach f
+0002a670: 6f72 204d 4f44 4953 206f 6365 616e 2063  or MODIS ocean c
+0002a680: 6f6c 6f72 2064 6174 6120 7072 6f63 6573  olor data proces
+0002a690: 7369 6e67 2e0d 0a20 2023 2020 4f70 7469  sing...  #  Opti
+0002a6a0: 6373 2045 7870 7265 7373 2c20 3135 2832  cs Express, 15(2
+0002a6b0: 3429 2c20 3135 3732 32e2 8093 3135 3733  4), 15722...1573
+0002a6c0: 332e 0d0a 0d0a 2020 2320 4164 6420 7365  3.....  # Add se
+0002a6d0: 636f 6e64 6172 7920 6669 6c74 6572 2075  condary filter u
+0002a6e0: 7369 6e67 2067 7265 656e 6e65 7373 2066  sing greenness f
+0002a6f0: 756e 6374 696f 6e20 6265 6c6f 770d 0a20  unction below.. 
+0002a700: 2069 6d61 6765 203d 2069 6d61 6765 2e61   image = image.a
+0002a710: 6464 4261 6e64 7328 486f 4361 6c63 4772  ddBands(HoCalcGr
+0002a720: 6565 6e6e 6573 7328 696d 6167 6529 290d  eenness(image)).
+0002a730: 0a0d 0a20 2023 2041 7070 6c79 2061 6c67  ...  # Apply alg
+0002a740: 6f72 6974 686d 2031 3a20 4234 202d 2031  orithm 1: B4 - 1
+0002a750: 2e30 332a 4235 0d0a 2020 2362 6c6f 6f6d  .03*B5..  #bloom
+0002a760: 3120 3d20 696d 6167 652e 7365 6c65 6374  1 = image.select
+0002a770: 2827 6e69 7227 292e 7375 6274 7261 6374  ('nir').subtract
+0002a780: 2869 6d61 6765 2e73 656c 6563 7428 2773  (image.select('s
+0002a790: 7769 7231 2729 2e6d 756c 7469 706c 7928  wir1').multiply(
+0002a7a0: 312e 3033 2929 2e72 656e 616d 6528 2762  1.03)).rename('b
+0002a7b0: 6c6f 6f6d 3127 290d 0a0d 0a20 2023 2047  loom1')....  # G
+0002a7c0: 6574 2062 696e 6172 7920 696d 6167 6520  et binary image 
+0002a7d0: 6279 2061 7070 6c79 696e 6720 7468 6520  by applying the 
+0002a7e0: 7468 7265 7368 6f6c 640d 0a20 2062 6c6f  threshold..  blo
+0002a7f0: 6f6d 315f 6d61 736b 203d 2069 6d61 6765  om1_mask = image
+0002a800: 2e73 656c 6563 7428 2248 2229 2e6c 7465  .select("H").lte
+0002a810: 2867 7265 656e 6573 7354 6872 6573 686f  (greenessThresho
+0002a820: 6c64 292e 7265 6e61 6d65 285b 2262 6c6f  ld).rename(["blo
+0002a830: 6f6d 315f 6d61 736b 225d 290d 0a0d 0a0d  om1_mask"]).....
+0002a840: 0a20 2072 6574 7572 6e20 696d 6167 655c  .  return image\
+0002a850: 0d0a 2020 2020 2020 2020 2020 2e61 6464  ..          .add
+0002a860: 4261 6e64 7328 626c 6f6f 6d31 295c 0d0a  Bands(bloom1)\..
+0002a870: 2020 2020 2020 2020 2020 2e61 6464 4261            .addBa
+0002a880: 6e64 7328 626c 6f6f 6d31 5f6d 6173 6b29  nds(bloom1_mask)
+0002a890: 0d0a 0d0a 0d0a 0d0a 0d0a 2320 2f2f 2f2f  ..........# ////
 0002a8a0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a8b0: 2f2f 0d0a 0d0a 0d0a 7465 7374 4172 6561  //......testArea
-0002a8c0: 7320 3d20 7b7d 3b0d 0a74 6573 7441 7265  s = {};..testAre
-0002a8d0: 6173 5b27 434f 275d 203d 2065 652e 4765  as['CO'] = ee.Ge
-0002a8e0: 6f6d 6574 7279 2e50 6f6c 7967 6f6e 280d  ometry.Polygon(.
-0002a8f0: 0a20 2020 2020 2020 205b 5b5b 2d31 3038  .        [[[-108
-0002a900: 2e32 3836 3330 3530 3930 3634 3735 392c  .28630509064759,
-0002a910: 2033 382e 3038 3533 3433 3633 3831 3230   38.085343638120
-0002a920: 3932 355d 2c0d 0a20 2020 2020 2020 2020  925],..         
-0002a930: 205b 2d31 3038 2e32 3836 3330 3530 3930   [-108.286305090
-0002a940: 3634 3735 392c 2033 372e 3138 3035 3132  64759, 37.180512
-0002a950: 3230 3039 3239 3435 5d2c 0d0a 2020 2020  20092945],..    
-0002a960: 2020 2020 2020 5b2d 3130 362e 3734 3832        [-106.7482
-0002a970: 3139 3135 3331 3437 3539 2c20 3337 2e31  1915314759, 37.1
-0002a980: 3830 3531 3232 3030 3932 3934 355d 2c0d  8051220092945],.
-0002a990: 0a20 2020 2020 2020 2020 205b 2d31 3036  .          [-106
-0002a9a0: 2e37 3438 3231 3931 3533 3134 3735 392c  .74821915314759,
-0002a9b0: 2033 382e 3038 3533 3433 3633 3831 3230   38.085343638120
-0002a9c0: 3932 355d 5d5d 2c20 4e6f 6e65 2c20 4661  925]]], None, Fa
-0002a9d0: 6c73 6529 0d0a 7465 7374 4172 6561 735b  lse)..testAreas[
-0002a9e0: 2743 4f5f 4e6f 7274 6827 5d20 3d20 6565  'CO_North'] = ee
-0002a9f0: 2e47 656f 6d65 7472 792e 506f 6c79 676f  .Geometry.Polygo
-0002aa00: 6e28 0d0a 2020 2020 2020 2020 5b5b 5b2d  n(..        [[[-
-0002aa10: 3130 362e 3431 3937 3738 3639 3333 3935  106.419778693395
-0002aa20: 3234 2c20 3430 2e39 3739 3437 3730 3233  24, 40.979477023
-0002aa30: 3933 3233 345d 2c0d 0a20 2020 2020 2020  93234],..       
-0002aa40: 2020 205b 2d31 3036 2e34 3139 3737 3836     [-106.4197786
-0002aa50: 3933 3339 3532 342c 2033 392e 3936 3430  9339524, 39.9640
-0002aa60: 3633 3231 3831 3430 3031 5d2c 0d0a 2020  6321814001],..  
-0002aa70: 2020 2020 2020 2020 5b2d 3130 352e 3230          [-105.20
-0002aa80: 3537 3839 3433 3535 3832 3734 2c20 3339  578943558274, 39
-0002aa90: 2e39 3634 3036 3332 3138 3134 3030 315d  .96406321814001]
-0002aaa0: 2c0d 0a20 2020 2020 2020 2020 205b 2d31  ,..          [-1
-0002aab0: 3035 2e32 3035 3738 3934 3335 3538 3237  05.2057894355827
-0002aac0: 342c 2034 302e 3937 3934 3737 3032 3339  4, 40.9794770239
-0002aad0: 3332 3334 5d5d 5d2c 204e 6f6e 652c 2046  3234]]], None, F
-0002aae0: 616c 7365 290d 0a74 6573 7441 7265 6173  alse)..testAreas
-0002aaf0: 5b27 4341 275d 203d 6565 2e47 656f 6d65  ['CA'] =ee.Geome
-0002ab00: 7472 792e 506f 6c79 676f 6e28 0d0a 2020  try.Polygon(..  
-0002ab10: 2020 2020 2020 5b5b 5b2d 3131 392e 3936        [[[-119.96
-0002ab20: 3338 3337 3630 3238 3735 3036 2c20 3337  383760287506, 37
-0002ab30: 2e31 3338 3135 3035 3734 3130 3837 3134  .138150574108714
-0002ab40: 5d2c 0d0a 2020 2020 2020 2020 2020 5b2d  ],..          [-
-0002ab50: 3131 392e 3936 3338 3337 3630 3238 3735  119.963837602875
-0002ab60: 3036 2c20 3336 2e34 3037 3734 3431 3231  06, 36.407744121
-0002ab70: 3036 3432 345d 2c0d 0a20 2020 2020 2020  06424],..       
-0002ab80: 2020 205b 2d31 3137 2e39 3533 3333 3935     [-117.9533395
-0002ab90: 3536 3030 3030 362c 2033 362e 3430 3737  5600006, 36.4077
-0002aba0: 3434 3132 3130 3634 3234 5d2c 0d0a 2020  4412106424],..  
-0002abb0: 2020 2020 2020 2020 5b2d 3131 372e 3935          [-117.95
-0002abc0: 3333 3339 3535 3630 3030 3036 2c20 3337  333955600006, 37
-0002abd0: 2e31 3338 3135 3035 3734 3130 3837 3134  .138150574108714
-0002abe0: 5d5d 5d2c 204e 6f6e 652c 2046 616c 7365  ]]], None, False
-0002abf0: 290d 0a0d 0a74 6573 7441 7265 6173 5b27  )....testAreas['
-0002ac00: 4341 5f53 6d61 6c6c 275d 203d 2065 652e  CA_Small'] = ee.
-0002ac10: 4765 6f6d 6574 7279 2e50 6f6c 7967 6f6e  Geometry.Polygon
-0002ac20: 280d 0a20 2020 2020 2020 205b 5b5b 2d31  (..        [[[-1
-0002ac30: 3233 2e32 3235 3636 3936 3833 3734 3632  23.2256696837462
-0002ac40: 352c 2033 392e 3637 3732 3039 3539 3932  5, 39.6772095992
-0002ac50: 3639 3135 355d 2c0d 0a20 2020 2020 2020  69155],..       
-0002ac60: 2020 205b 2d31 3233 2e32 3235 3636 3936     [-123.2256696
-0002ac70: 3833 3734 3632 352c 2033 382e 3939 3331  8374625, 38.9931
-0002ac80: 3739 3530 3436 3937 3538 365d 2c0d 0a20  79504697586],.. 
-0002ac90: 2020 2020 2020 2020 205b 2d31 3232 2e36           [-122.6
-0002aca0: 3034 3934 3231 3434 3638 3337 352c 2033  0494214468375, 3
-0002acb0: 382e 3939 3331 3739 3530 3436 3937 3538  8.99317950469758
-0002acc0: 365d 2c0d 0a20 2020 2020 2020 2020 205b  6],..          [
-0002acd0: 2d31 3232 2e36 3034 3934 3231 3434 3638  -122.60494214468
-0002ace0: 3337 352c 2033 392e 3637 3732 3039 3539  375, 39.67720959
-0002acf0: 3932 3639 3135 355d 5d5d 2c20 4e6f 6e65  9269155]]], None
-0002ad00: 2c20 4661 6c73 6529 0d0a 0d0a 7465 7374  , False)....test
-0002ad10: 4172 6561 735b 2748 4927 5d20 3d20 6565  Areas['HI'] = ee
-0002ad20: 2e47 656f 6d65 7472 792e 506f 6c79 676f  .Geometry.Polygo
-0002ad30: 6e28 0d0a 2020 2020 2020 2020 5b5b 5b2d  n(..        [[[-
-0002ad40: 3136 302e 3530 3832 3438 3734 3435 3035  160.508248744505
-0002ad50: 3434 2c20 3232 2e36 3539 3831 3435 3133  44, 22.659814513
-0002ad60: 3930 3934 3734 5d2c 0d0a 2020 2020 2020  909474],..      
-0002ad70: 2020 2020 5b2d 3136 302e 3530 3832 3438      [-160.508248
-0002ad80: 3734 3435 3035 3434 2c20 3138 2e35 3437  74450544, 18.547
-0002ad90: 3530 3330 3939 3539 3832 375d 2c0d 0a20  50309959827],.. 
-0002ada0: 2020 2020 2020 2020 205b 2d31 3534 2e33           [-154.3
-0002adb0: 3535 3930 3439 3934 3530 3534 342c 2031  5590499450544, 1
-0002adc0: 382e 3534 3735 3033 3039 3935 3938 3237  8.54750309959827
-0002add0: 5d2c 0d0a 2020 2020 2020 2020 2020 5b2d  ],..          [-
-0002ade0: 3135 342e 3335 3539 3034 3939 3435 3035  154.355904994505
-0002adf0: 3434 2c20 3232 2e36 3539 3831 3435 3133  44, 22.659814513
-0002ae00: 3930 3934 3734 5d5d 5d2c 204e 6f6e 652c  909474]]], None,
-0002ae10: 2046 616c 7365 290d 0a                    False)..
+0002a8b0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a8c0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a8d0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a8e0: 2f2f 2f2f 2f2f 0d0a 2320 2f2f 2045 4e44  //////..# // END
+0002a8f0: 2046 554e 4354 494f 4e53 0d0a 2320 2f2f   FUNCTIONS..# //
+0002a900: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a910: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a920: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a930: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a940: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 0d0a  //////////////..
+0002a950: 0d0a 0d0a 7465 7374 4172 6561 7320 3d20  ....testAreas = 
+0002a960: 7b7d 3b0d 0a74 6573 7441 7265 6173 5b27  {};..testAreas['
+0002a970: 434f 275d 203d 2065 652e 4765 6f6d 6574  CO'] = ee.Geomet
+0002a980: 7279 2e50 6f6c 7967 6f6e 280d 0a20 2020  ry.Polygon(..   
+0002a990: 2020 2020 205b 5b5b 2d31 3038 2e32 3836       [[[-108.286
+0002a9a0: 3330 3530 3930 3634 3735 392c 2033 382e  30509064759, 38.
+0002a9b0: 3038 3533 3433 3633 3831 3230 3932 355d  085343638120925]
+0002a9c0: 2c0d 0a20 2020 2020 2020 2020 205b 2d31  ,..          [-1
+0002a9d0: 3038 2e32 3836 3330 3530 3930 3634 3735  08.2863050906475
+0002a9e0: 392c 2033 372e 3138 3035 3132 3230 3039  9, 37.1805122009
+0002a9f0: 3239 3435 5d2c 0d0a 2020 2020 2020 2020  2945],..        
+0002aa00: 2020 5b2d 3130 362e 3734 3832 3139 3135    [-106.74821915
+0002aa10: 3331 3437 3539 2c20 3337 2e31 3830 3531  314759, 37.18051
+0002aa20: 3232 3030 3932 3934 355d 2c0d 0a20 2020  220092945],..   
+0002aa30: 2020 2020 2020 205b 2d31 3036 2e37 3438         [-106.748
+0002aa40: 3231 3931 3533 3134 3735 392c 2033 382e  21915314759, 38.
+0002aa50: 3038 3533 3433 3633 3831 3230 3932 355d  085343638120925]
+0002aa60: 5d5d 2c20 4e6f 6e65 2c20 4661 6c73 6529  ]], None, False)
+0002aa70: 0d0a 7465 7374 4172 6561 735b 2743 4f5f  ..testAreas['CO_
+0002aa80: 4e6f 7274 6827 5d20 3d20 6565 2e47 656f  North'] = ee.Geo
+0002aa90: 6d65 7472 792e 506f 6c79 676f 6e28 0d0a  metry.Polygon(..
+0002aaa0: 2020 2020 2020 2020 5b5b 5b2d 3130 362e          [[[-106.
+0002aab0: 3431 3937 3738 3639 3333 3935 3234 2c20  41977869339524, 
+0002aac0: 3430 2e39 3739 3437 3730 3233 3933 3233  40.9794770239323
+0002aad0: 345d 2c0d 0a20 2020 2020 2020 2020 205b  4],..          [
+0002aae0: 2d31 3036 2e34 3139 3737 3836 3933 3339  -106.41977869339
+0002aaf0: 3532 342c 2033 392e 3936 3430 3633 3231  524, 39.96406321
+0002ab00: 3831 3430 3031 5d2c 0d0a 2020 2020 2020  814001],..      
+0002ab10: 2020 2020 5b2d 3130 352e 3230 3537 3839      [-105.205789
+0002ab20: 3433 3535 3832 3734 2c20 3339 2e39 3634  43558274, 39.964
+0002ab30: 3036 3332 3138 3134 3030 315d 2c0d 0a20  06321814001],.. 
+0002ab40: 2020 2020 2020 2020 205b 2d31 3035 2e32           [-105.2
+0002ab50: 3035 3738 3934 3335 3538 3237 342c 2034  0578943558274, 4
+0002ab60: 302e 3937 3934 3737 3032 3339 3332 3334  0.97947702393234
+0002ab70: 5d5d 5d2c 204e 6f6e 652c 2046 616c 7365  ]]], None, False
+0002ab80: 290d 0a74 6573 7441 7265 6173 5b27 4341  )..testAreas['CA
+0002ab90: 275d 203d 6565 2e47 656f 6d65 7472 792e  '] =ee.Geometry.
+0002aba0: 506f 6c79 676f 6e28 0d0a 2020 2020 2020  Polygon(..      
+0002abb0: 2020 5b5b 5b2d 3131 392e 3936 3338 3337    [[[-119.963837
+0002abc0: 3630 3238 3735 3036 2c20 3337 2e31 3338  60287506, 37.138
+0002abd0: 3135 3035 3734 3130 3837 3134 5d2c 0d0a  150574108714],..
+0002abe0: 2020 2020 2020 2020 2020 5b2d 3131 392e            [-119.
+0002abf0: 3936 3338 3337 3630 3238 3735 3036 2c20  96383760287506, 
+0002ac00: 3336 2e34 3037 3734 3431 3231 3036 3432  36.4077441210642
+0002ac10: 345d 2c0d 0a20 2020 2020 2020 2020 205b  4],..          [
+0002ac20: 2d31 3137 2e39 3533 3333 3935 3536 3030  -117.95333955600
+0002ac30: 3030 362c 2033 362e 3430 3737 3434 3132  006, 36.40774412
+0002ac40: 3130 3634 3234 5d2c 0d0a 2020 2020 2020  106424],..      
+0002ac50: 2020 2020 5b2d 3131 372e 3935 3333 3339      [-117.953339
+0002ac60: 3535 3630 3030 3036 2c20 3337 2e31 3338  55600006, 37.138
+0002ac70: 3135 3035 3734 3130 3837 3134 5d5d 5d2c  150574108714]]],
+0002ac80: 204e 6f6e 652c 2046 616c 7365 290d 0a0d   None, False)...
+0002ac90: 0a74 6573 7441 7265 6173 5b27 4341 5f53  .testAreas['CA_S
+0002aca0: 6d61 6c6c 275d 203d 2065 652e 4765 6f6d  mall'] = ee.Geom
+0002acb0: 6574 7279 2e50 6f6c 7967 6f6e 280d 0a20  etry.Polygon(.. 
+0002acc0: 2020 2020 2020 205b 5b5b 2d31 3233 2e32         [[[-123.2
+0002acd0: 3235 3636 3936 3833 3734 3632 352c 2033  2566968374625, 3
+0002ace0: 392e 3637 3732 3039 3539 3932 3639 3135  9.67720959926915
+0002acf0: 355d 2c0d 0a20 2020 2020 2020 2020 205b  5],..          [
+0002ad00: 2d31 3233 2e32 3235 3636 3936 3833 3734  -123.22566968374
+0002ad10: 3632 352c 2033 382e 3939 3331 3739 3530  625, 38.99317950
+0002ad20: 3436 3937 3538 365d 2c0d 0a20 2020 2020  4697586],..     
+0002ad30: 2020 2020 205b 2d31 3232 2e36 3034 3934       [-122.60494
+0002ad40: 3231 3434 3638 3337 352c 2033 382e 3939  214468375, 38.99
+0002ad50: 3331 3739 3530 3436 3937 3538 365d 2c0d  3179504697586],.
+0002ad60: 0a20 2020 2020 2020 2020 205b 2d31 3232  .          [-122
+0002ad70: 2e36 3034 3934 3231 3434 3638 3337 352c  .60494214468375,
+0002ad80: 2033 392e 3637 3732 3039 3539 3932 3639   39.677209599269
+0002ad90: 3135 355d 5d5d 2c20 4e6f 6e65 2c20 4661  155]]], None, Fa
+0002ada0: 6c73 6529 0d0a 0d0a 7465 7374 4172 6561  lse)....testArea
+0002adb0: 735b 2748 4927 5d20 3d20 6565 2e47 656f  s['HI'] = ee.Geo
+0002adc0: 6d65 7472 792e 506f 6c79 676f 6e28 0d0a  metry.Polygon(..
+0002add0: 2020 2020 2020 2020 5b5b 5b2d 3136 302e          [[[-160.
+0002ade0: 3530 3832 3438 3734 3435 3035 3434 2c20  50824874450544, 
+0002adf0: 3232 2e36 3539 3831 3435 3133 3930 3934  22.6598145139094
+0002ae00: 3734 5d2c 0d0a 2020 2020 2020 2020 2020  74],..          
+0002ae10: 5b2d 3136 302e 3530 3832 3438 3734 3435  [-160.5082487445
+0002ae20: 3035 3434 2c20 3138 2e35 3437 3530 3330  0544, 18.5475030
+0002ae30: 3939 3539 3832 375d 2c0d 0a20 2020 2020  9959827],..     
+0002ae40: 2020 2020 205b 2d31 3534 2e33 3535 3930       [-154.35590
+0002ae50: 3439 3934 3530 3534 342c 2031 382e 3534  499450544, 18.54
+0002ae60: 3735 3033 3039 3935 3938 3237 5d2c 0d0a  750309959827],..
+0002ae70: 2020 2020 2020 2020 2020 5b2d 3135 342e            [-154.
+0002ae80: 3335 3539 3034 3939 3435 3035 3434 2c20  35590499450544, 
+0002ae90: 3232 2e36 3539 3831 3435 3133 3930 3934  22.6598145139094
+0002aea0: 3734 5d5d 5d2c 204e 6f6e 652c 2046 616c  74]]], None, Fal
+0002aeb0: 7365 290d 0a                             se)..
```

### Comparing `geeViz-2023.7.3/geeViz/migrateGEEAssets.py` & `geeViz-2023.7.4/geeViz/migrateGEEAssets.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/phEEnoViz.py` & `geeViz-2023.7.4/geeViz/phEEnoViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz/taskManagerLib.py` & `geeViz-2023.7.4/geeViz/taskManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/geeViz.egg-info/PKG-INFO` & `geeViz-2023.7.4/geeViz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geeViz-2023.7.3/geeViz.egg-info/SOURCES.txt` & `geeViz-2023.7.4/geeViz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.3/setup.py` & `geeViz-2023.7.4/setup.py`

 * *Files identical despite different names*

