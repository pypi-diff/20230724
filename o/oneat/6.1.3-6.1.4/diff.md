# Comparing `tmp/oneat-6.1.3.tar.gz` & `tmp/oneat-6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.1.3.tar", last modified: Mon Jul 24 18:08:55 2023, max compression
+gzip compressed data, was "oneat-6.1.4.tar", last modified: Mon Jul 24 18:12:26 2023, max compression
```

## Comparing `oneat-6.1.3.tar` & `oneat-6.1.4.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.583920 oneat-6.1.3/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.1.3/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.1.3/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.560051 oneat-6.1.3/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.562965 oneat-6.1.3/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.1.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.1.3/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.564113 oneat-6.1.3/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.1.3/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.1.3/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.564257 oneat-6.1.3/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.1.3/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.1.3/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.1.3/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.1.3/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.1.3/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.1.3/1
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.3/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.1.3/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 18:08:55.584004 oneat-6.1.3/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.1.3/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.567239 oneat-6.1.3/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.1.3/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.1.3/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.1.3/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.1.3/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.1.3/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.1.3/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.1.3/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.1.3/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.570324 oneat-6.1.3/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.1.3/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.3/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.1.3/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.1.3/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.1.3/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.1.3/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.1.3/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-24 18:08:55.584353 oneat-6.1.3/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.560493 oneat-6.1.3/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.571041 oneat-6.1.3/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.574868 oneat-6.1.3/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13599 2023-07-24 18:08:17.000000 oneat-6.1.3/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38374 2023-07-24 18:05:13.000000 oneat-6.1.3/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.577122 oneat-6.1.3/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.1.3/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.577946 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.578770 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.579118 oneat-6.1.3/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.582929 oneat-6.1.3/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-24 18:08:55.000000 oneat-6.1.3/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.1.3/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:08:55.571760 oneat-6.1.3/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 18:08:55.000000 oneat-6.1.3/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-24 18:08:55.000000 oneat-6.1.3/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-24 18:08:55.000000 oneat-6.1.3/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-24 18:08:55.000000 oneat-6.1.3/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-24 18:08:55.000000 oneat-6.1.3/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-24 18:08:55.000000 oneat-6.1.3/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.1.3/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.531300 oneat-6.1.4/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.1.4/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.1.4/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.506391 oneat-6.1.4/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.509582 oneat-6.1.4/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.1.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.1.4/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.510677 oneat-6.1.4/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.1.4/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.1.4/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.510834 oneat-6.1.4/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.1.4/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.1.4/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.1.4/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.1.4/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.1.4/1
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.4/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.1.4/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 18:12:26.531391 oneat-6.1.4/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.1.4/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.515524 oneat-6.1.4/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.1.4/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.1.4/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.1.4/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.1.4/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.1.4/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.1.4/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.1.4/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.1.4/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.517145 oneat-6.1.4/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.1.4/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.4/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.1.4/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.1.4/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.1.4/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.1.4/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.1.4/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-24 18:12:26.531734 oneat-6.1.4/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.506913 oneat-6.1.4/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.517875 oneat-6.1.4/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.521659 oneat-6.1.4/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.1.4/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38374 2023-07-24 18:05:13.000000 oneat-6.1.4/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.523689 oneat-6.1.4/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.1.4/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.524539 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.525403 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.525800 oneat-6.1.4/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.530363 oneat-6.1.4/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-24 18:12:26.000000 oneat-6.1.4/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.1.4/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:12:26.518687 oneat-6.1.4/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 18:12:26.000000 oneat-6.1.4/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-24 18:12:26.000000 oneat-6.1.4/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-24 18:12:26.000000 oneat-6.1.4/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-24 18:12:26.000000 oneat-6.1.4/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-24 18:12:26.000000 oneat-6.1.4/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-24 18:12:26.000000 oneat-6.1.4/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.1.4/tox.ini
```

### Comparing `oneat-6.1.3/.DS_Store` & `oneat-6.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/.github/workflows/test_and_deploy.yml` & `oneat-6.1.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/.gitignore` & `oneat-6.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/.pre-commit-config.yaml` & `oneat-6.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/LICENSE` & `oneat-6.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/PKG-INFO` & `oneat-6.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.1.3
+Version: 6.1.4
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.1.3/README.md` & `oneat-6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/images/Xenopus_example.jpg` & `oneat-6.1.4/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/images/Xenopus_example.png` & `oneat-6.1.4/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/images/ch_0_crop.png` & `oneat-6.1.4/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/images/ch_1_crop.png` & `oneat-6.1.4/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/images/ch_2_crop.png` & `oneat-6.1.4/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/images/ch_3_crop.png` & `oneat-6.1.4/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/images/ch_4_crop.png` & `oneat-6.1.4/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/images/ch_5_crop.png` & `oneat-6.1.4/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/licenses/Apache-2` & `oneat-6.1.4/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/licenses/BSD-3` & `oneat-6.1.4/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/licenses/GPL-3` & `oneat-6.1.4/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/licenses/LGPL-3` & `oneat-6.1.4/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/licenses/MIT` & `oneat-6.1.4/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/licenses/MPL-2` & `oneat-6.1.4/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/setup.cfg` & `oneat-6.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.1.4/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.1.4/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.1.4/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.1.4/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/__init__.py` & `oneat-6.1.4/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/config.py` & `oneat-6.1.4/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.1.4/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/loss.py` & `oneat-6.1.4/src/oneat/NEATModels/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             # Apply class weights to the classification loss
             sample_weights = tf.reduce_sum(class_weights * tf.one_hot(tf.argmax(true_box_class, axis=-1), categories), axis=1)
 
             # Compute the weighted mean of the classification loss
             loss_class_weighted = tf.reduce_sum(loss_class * sample_weights) / tf.reduce_sum(sample_weights)
 
             # Adding it all up
-            combined_loss = loss_xywht + loss_conf + loss_class_weighted
+            combinedloss = loss_xywht + loss_conf + loss_class_weighted
 
        
 
         return combinedloss 
         
     return loss
```

### Comparing `oneat-6.1.3/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.1.4/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.1.4/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/neat_focus.py` & `oneat-6.1.4/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.1.4/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.1.4/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.1.4/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.1.4/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.1.4/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATModels/nets.py` & `oneat-6.1.4/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.1.4/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.1.4/src/oneat/NEATUtils/MovieCreator.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/NMS.py` & `oneat-6.1.4/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.1.4/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.1.4/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.1.4/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.1.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/plotters.py` & `oneat-6.1.4/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/NEATUtils/utils.py` & `oneat-6.1.4/src/oneat/NEATUtils/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/__init__.py` & `oneat-6.1.4/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/_tests/test_nets.py` & `oneat-6.1.4/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/_tests/utils.py` & `oneat-6.1.4/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.1.4/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/_tests/variables/variables.index` & `oneat-6.1.4/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat/pretrained.py` & `oneat-6.1.4/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/src/oneat.egg-info/PKG-INFO` & `oneat-6.1.4/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.1.3
+Version: 6.1.4
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.1.3/src/oneat.egg-info/SOURCES.txt` & `oneat-6.1.4/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-6.1.3/tox.ini` & `oneat-6.1.4/tox.ini`

 * *Files identical despite different names*

