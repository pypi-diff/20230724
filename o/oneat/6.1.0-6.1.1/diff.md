# Comparing `tmp/oneat-6.1.0.tar.gz` & `tmp/oneat-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.1.0.tar", last modified: Mon Jul 24 17:48:01 2023, max compression
+gzip compressed data, was "oneat-6.1.1.tar", last modified: Mon Jul 24 18:03:18 2023, max compression
```

## Comparing `oneat-6.1.0.tar` & `oneat-6.1.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.971953 oneat-6.1.0/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.1.0/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.1.0/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.948010 oneat-6.1.0/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.950768 oneat-6.1.0/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.1.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.1.0/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.952026 oneat-6.1.0/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.1.0/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.1.0/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.952167 oneat-6.1.0/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.1.0/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.1.0/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.1.0/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.1.0/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.1.0/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.1.0/1
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.0/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.1.0/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 17:48:01.972043 oneat-6.1.0/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.1.0/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.955145 oneat-6.1.0/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.1.0/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.1.0/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.1.0/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.1.0/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.1.0/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.1.0/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.1.0/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.1.0/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.956259 oneat-6.1.0/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.1.0/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.0/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.1.0/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.1.0/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.1.0/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.1.0/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.1.0/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-24 17:48:01.972388 oneat-6.1.0/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.948462 oneat-6.1.0/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.957012 oneat-6.1.0/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.960785 oneat-6.1.0/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13041 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38385 2023-07-24 17:47:24.000000 oneat-6.1.0/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.965322 oneat-6.1.0/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.1.0/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.966142 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.966965 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.967330 oneat-6.1.0/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.971064 oneat-6.1.0/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-24 17:48:01.000000 oneat-6.1.0/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.1.0/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:48:01.957794 oneat-6.1.0/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 17:48:01.000000 oneat-6.1.0/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-24 17:48:01.000000 oneat-6.1.0/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-24 17:48:01.000000 oneat-6.1.0/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-24 17:48:01.000000 oneat-6.1.0/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-24 17:48:01.000000 oneat-6.1.0/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-24 17:48:01.000000 oneat-6.1.0/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.1.0/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.364331 oneat-6.1.1/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.1.1/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.1.1/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.350144 oneat-6.1.1/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.352322 oneat-6.1.1/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.1.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.1.1/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.353127 oneat-6.1.1/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.1.1/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.1.1/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.353261 oneat-6.1.1/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.1.1/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.1.1/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.1.1/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.1.1/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.1.1/1
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.1/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.1.1/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 18:03:18.364421 oneat-6.1.1/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.1.1/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.354810 oneat-6.1.1/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.1.1/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.1.1/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.1.1/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.1.1/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.1.1/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.1.1/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.1.1/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.1.1/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.355520 oneat-6.1.1/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.1.1/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.1/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.1.1/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.1.1/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.1.1/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.1.1/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.1.1/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-24 18:03:18.364763 oneat-6.1.1/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.350580 oneat-6.1.1/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.355979 oneat-6.1.1/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.358701 oneat-6.1.1/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13604 2023-07-24 18:02:43.000000 oneat-6.1.1/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38401 2023-07-24 18:02:43.000000 oneat-6.1.1/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.359793 oneat-6.1.1/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.1.1/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.360472 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.361132 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.361527 oneat-6.1.1/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.364222 oneat-6.1.1/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-24 18:03:18.000000 oneat-6.1.1/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.1.1/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 18:03:18.356599 oneat-6.1.1/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 18:03:18.000000 oneat-6.1.1/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-24 18:03:18.000000 oneat-6.1.1/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-24 18:03:18.000000 oneat-6.1.1/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-24 18:03:18.000000 oneat-6.1.1/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-24 18:03:18.000000 oneat-6.1.1/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-24 18:03:18.000000 oneat-6.1.1/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.1.1/tox.ini
```

### Comparing `oneat-6.1.0/.DS_Store` & `oneat-6.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/.github/workflows/test_and_deploy.yml` & `oneat-6.1.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/.gitignore` & `oneat-6.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/.pre-commit-config.yaml` & `oneat-6.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/LICENSE` & `oneat-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/PKG-INFO` & `oneat-6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.1.0
+Version: 6.1.1
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.1.0/README.md` & `oneat-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/images/Xenopus_example.jpg` & `oneat-6.1.1/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/images/Xenopus_example.png` & `oneat-6.1.1/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/images/ch_0_crop.png` & `oneat-6.1.1/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/images/ch_1_crop.png` & `oneat-6.1.1/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/images/ch_2_crop.png` & `oneat-6.1.1/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/images/ch_3_crop.png` & `oneat-6.1.1/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/images/ch_4_crop.png` & `oneat-6.1.1/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/images/ch_5_crop.png` & `oneat-6.1.1/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/licenses/Apache-2` & `oneat-6.1.1/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/licenses/BSD-3` & `oneat-6.1.1/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/licenses/GPL-3` & `oneat-6.1.1/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/licenses/LGPL-3` & `oneat-6.1.1/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/licenses/MIT` & `oneat-6.1.1/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/licenses/MPL-2` & `oneat-6.1.1/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/setup.cfg` & `oneat-6.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.1.1/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.1.1/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.1.1/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.1.1/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/__init__.py` & `oneat-6.1.1/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/config.py` & `oneat-6.1.1/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.1.1/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/loss.py` & `oneat-6.1.1/src/oneat/NEATModels/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,27 +285,38 @@
 
 
         return combinedloss 
         
     return loss 
 
 
-def volume_yolo_loss(categories, grid_h, grid_w, grid_d, nboxes, box_vector, entropy):
+def volume_yolo_loss(categories, grid_h, grid_w, grid_d, nboxes, box_vector, entropy, class_weights = None):
     def loss(y_true, y_pred):    
         event_grid = get_event_grid(grid_h, grid_w, grid_d, nboxes)
         true_box_class, true_box_xyz, true_box_whd, true_box_conf = extract_ground_event_volume_truth(y_true, categories, grid_h, grid_w,grid_d, nboxes, box_vector)
         pred_box_class, pred_box_xyz, pred_box_whd, pred_box_conf = extract_ground_event_volume_pred(y_pred, categories, grid_h, grid_w,grid_d, event_grid, nboxes, box_vector)
 
         loss_xywht = calc_loss_xyzwhd( true_box_xyz, pred_box_xyz, true_box_whd, pred_box_whd)
 
         loss_class   = calc_loss_class(true_box_class, pred_box_class, entropy)
 
         loss_conf = compute_conf_loss_volume(pred_box_whd, true_box_whd, pred_box_xyz,true_box_xyz,true_box_conf,pred_box_conf)
                     # Adding it all up   
-        combinedloss = (loss_xywht + loss_conf + loss_class)
+        if class_weights is None:             
+            combinedloss = (loss_xywht + loss_conf + loss_class)
+        else:
+            # Apply class weights to the classification loss
+            sample_weights = tf.reduce_sum(class_weights * tf.one_hot(tf.argmax(true_box_class, axis=-1), len(categories)), axis=1)
+
+            # Compute the weighted mean of the classification loss
+            loss_class_weighted = tf.reduce_sum(loss_class * sample_weights) / tf.reduce_sum(sample_weights)
+
+            # Adding it all up
+            combined_loss = loss_xywht + loss_conf + loss_class_weighted
+
        
 
         return combinedloss 
         
     return loss
```

### Comparing `oneat-6.1.0/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.1.1/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,15 @@
         self.Xoriginal = None
         self.Xoriginal_val = None
 
         self.model_keras = nets.DenseVollNet
 
         self.last_activation = 'softmax'
         self.entropy = 'notbinary'
-        self.yolo_loss = volume_yolo_loss(self.categories, self.gridx, self.gridy, self.gridz, self.nboxes,
-                                          self.box_vector, self.entropy)
+        
 
     @classmethod   
     def local_from_pretrained(cls, name_or_alias=None):
            try:
                print(cls)
                get_model_details(cls, name_or_alias, verbose=True)
                return get_model_instance(cls, name_or_alias)
@@ -184,15 +183,20 @@
 
         Y_class = self.Y[:, :, :, :, :self.categories]
         Y_class = Y_class[:,0,0,0,:]
         class_indices = np.argmax(Y_class, axis=1)
         class_weights = class_weight.compute_class_weight('balanced',
                                                  classes = np.unique(class_indices),
                                                  y = class_indices)
-        class_weights = dict(zip(np.unique(class_indices), class_weights))                                         
+        class_weights = dict(zip(np.unique(class_indices), class_weights))   
+
+        self.yolo_loss = volume_yolo_loss(self.categories, self.gridx, self.gridy, self.gridz, self.nboxes,
+                                          self.box_vector, self.entropy, class_weights)
+
+
         Y_rest = self.Y[:, :, :, :, self.categories:]
 
         dummyY = np.zeros(
             [self.Y.shape[0], self.Y.shape[1], self.Y.shape[2], self.Y.shape[3], self.categories + self.nboxes * self.box_vector])
         dummyY[:,:, :, :, :self.Y.shape[-1]] = self.Y
 
         dummyY_val = np.zeros([self.Y_val.shape[0], self.Y_val.shape[1], self.Y_val.shape[2], self.Y_val.shape[3],
@@ -233,16 +237,17 @@
                                      self.gridx, self.gridy, self.gridz, plot=self.show, nboxes=self.nboxes)
         
        
         # Train the model and save as a h5 file
         self.Trainingmodel.fit(self.X, self.Y, batch_size=self.batch_size,class_weight=class_weights,
                                epochs=self.epochs, validation_data=(self.X_val, self.Y_val),
                                callbacks=[lrate, hrate, srate, prate])
-
-
+      
+        
+       
         self.Trainingmodel.save(self.model_dir)
     """
     The input image and seg image are numpy arrays that have to be read prior to being loaded in the function
     """
     def get_markers(self, 
                     segimage : np.ndarray):
```

### Comparing `oneat-6.1.0/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.1.1/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/neat_focus.py` & `oneat-6.1.1/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.1.1/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.1.1/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.1.1/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.1.1/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.1.1/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATModels/nets.py` & `oneat-6.1.1/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.1.1/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.1.1/src/oneat/NEATUtils/MovieCreator.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/NMS.py` & `oneat-6.1.1/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.1.1/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.1.1/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.1.1/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.1.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/plotters.py` & `oneat-6.1.1/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/NEATUtils/utils.py` & `oneat-6.1.1/src/oneat/NEATUtils/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/__init__.py` & `oneat-6.1.1/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/_tests/test_nets.py` & `oneat-6.1.1/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/_tests/utils.py` & `oneat-6.1.1/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.1.1/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/_tests/variables/variables.index` & `oneat-6.1.1/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat/pretrained.py` & `oneat-6.1.1/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/src/oneat.egg-info/PKG-INFO` & `oneat-6.1.1/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.1.0
+Version: 6.1.1
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.1.0/src/oneat.egg-info/SOURCES.txt` & `oneat-6.1.1/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-6.1.0/tox.ini` & `oneat-6.1.1/tox.ini`

 * *Files identical despite different names*

