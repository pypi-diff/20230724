# Comparing `tmp/oneat-6.0.4.tar.gz` & `tmp/oneat-6.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.0.4.tar", last modified: Mon Jul 24 17:18:17 2023, max compression
+gzip compressed data, was "oneat-6.0.7.tar", last modified: Mon Jul 24 17:30:59 2023, max compression
```

## Comparing `oneat-6.0.4.tar` & `oneat-6.0.7.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.172024 oneat-6.0.4/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.0.4/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.0.4/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.147398 oneat-6.0.4/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.150395 oneat-6.0.4/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.0.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.0.4/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.151278 oneat-6.0.4/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.0.4/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.0.4/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.151418 oneat-6.0.4/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.0.4/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.0.4/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.0.4/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.0.4/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.0.4/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.0.4/1
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.4/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.0.4/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 17:18:17.172128 oneat-6.0.4/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.0.4/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.156061 oneat-6.0.4/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.0.4/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.0.4/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.0.4/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.0.4/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.0.4/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.0.4/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.0.4/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.0.4/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.157633 oneat-6.0.4/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.0.4/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.4/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.0.4/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.0.4/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.0.4/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.0.4/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.0.4/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-24 17:18:17.175604 oneat-6.0.4/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.147846 oneat-6.0.4/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.158376 oneat-6.0.4/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.161849 oneat-6.0.4/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13041 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38166 2023-07-24 17:17:00.000000 oneat-6.0.4/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.163848 oneat-6.0.4/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.0.4/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.164775 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.165587 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.165942 oneat-6.0.4/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.171014 oneat-6.0.4/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-24 17:18:17.000000 oneat-6.0.4/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.0.4/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:18:17.159101 oneat-6.0.4/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 17:18:17.000000 oneat-6.0.4/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-24 17:18:17.000000 oneat-6.0.4/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-24 17:18:17.000000 oneat-6.0.4/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-24 17:18:17.000000 oneat-6.0.4/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-24 17:18:17.000000 oneat-6.0.4/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-24 17:18:17.000000 oneat-6.0.4/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.0.4/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.795600 oneat-6.0.7/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.0.7/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.0.7/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.771548 oneat-6.0.7/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.774366 oneat-6.0.7/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.0.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.0.7/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.775574 oneat-6.0.7/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.0.7/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.0.7/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.775714 oneat-6.0.7/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.0.7/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.0.7/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.0.7/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.0.7/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.0.7/1
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.7/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.0.7/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 17:30:59.795689 oneat-6.0.7/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.0.7/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.778690 oneat-6.0.7/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.0.7/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.0.7/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.0.7/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.0.7/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.0.7/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.0.7/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.0.7/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.0.7/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.779785 oneat-6.0.7/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.0.7/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.7/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.0.7/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.0.7/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.0.7/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.0.7/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.0.7/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-24 17:30:59.796042 oneat-6.0.7/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.771993 oneat-6.0.7/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.782796 oneat-6.0.7/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.786797 oneat-6.0.7/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13041 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38299 2023-07-24 17:28:51.000000 oneat-6.0.7/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.788813 oneat-6.0.7/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.0.7/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.789670 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.790467 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.790855 oneat-6.0.7/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.794658 oneat-6.0.7/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-24 17:30:59.000000 oneat-6.0.7/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.0.7/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-24 17:30:59.783537 oneat-6.0.7/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-24 17:30:59.000000 oneat-6.0.7/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-24 17:30:59.000000 oneat-6.0.7/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-24 17:30:59.000000 oneat-6.0.7/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-24 17:30:59.000000 oneat-6.0.7/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-24 17:30:59.000000 oneat-6.0.7/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-24 17:30:59.000000 oneat-6.0.7/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.0.7/tox.ini
```

### Comparing `oneat-6.0.4/.DS_Store` & `oneat-6.0.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/.github/workflows/test_and_deploy.yml` & `oneat-6.0.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/.gitignore` & `oneat-6.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/.pre-commit-config.yaml` & `oneat-6.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/LICENSE` & `oneat-6.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/PKG-INFO` & `oneat-6.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.0.4
+Version: 6.0.7
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.0.4/README.md` & `oneat-6.0.7/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/images/Xenopus_example.jpg` & `oneat-6.0.7/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/images/Xenopus_example.png` & `oneat-6.0.7/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/images/ch_0_crop.png` & `oneat-6.0.7/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/images/ch_1_crop.png` & `oneat-6.0.7/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/images/ch_2_crop.png` & `oneat-6.0.7/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/images/ch_3_crop.png` & `oneat-6.0.7/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/images/ch_4_crop.png` & `oneat-6.0.7/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/images/ch_5_crop.png` & `oneat-6.0.7/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/licenses/Apache-2` & `oneat-6.0.7/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/licenses/BSD-3` & `oneat-6.0.7/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/licenses/GPL-3` & `oneat-6.0.7/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/licenses/LGPL-3` & `oneat-6.0.7/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/licenses/MIT` & `oneat-6.0.7/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/licenses/MPL-2` & `oneat-6.0.7/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/setup.cfg` & `oneat-6.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.0.7/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.0.7/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.0.7/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.0.7/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/__init__.py` & `oneat-6.0.7/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/config.py` & `oneat-6.0.7/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.0.7/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/loss.py` & `oneat-6.0.7/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.0.7/src/oneat/NEATModels/neat_vollnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import tensorflow as tf
 from tqdm import tqdm
 from oneat.NEATModels import nets
 from oneat.NEATModels.nets import Concat
 from oneat.NEATModels.loss import volume_yolo_loss
 from oneat.pretrained import get_registered_models, get_model_details, get_model_instance
 from pathlib import Path
-from keras.models import load_model
+from tensorflow.keras.models import load_model
 from tifffile import imread
-from sklearn.utils import class_weight
 
-class NEATDenseVollNet(object):
+
+class NEATVollNet(object):
     """
     Parameters
     ----------
     
     NpzDirectory : Specify the location of npz file containing the training data with movies and labels
     
     TrainModelName : Specify the name of the npz file containing training data and labels
@@ -32,15 +32,15 @@
     
     Categories_Name : List of class names and labels
     
     model_dir : Directory location where trained model weights are to be read or written from
     
     model_keras : The model as it appears as a Keras function
     
-    model : If re-training model = model_dir else None as default
+    model_weights : If re-training model_weights = model_dir else None as default
     
     
     epochs :  Number of training epochs, 55 by default
     
     batch_size : batch_size to be used for training, 20 by default
     
     
@@ -132,15 +132,15 @@
         self.axes = None
         self.X_val = None
         self.Y_val = None
         self.Trainingmodel = None
         self.Xoriginal = None
         self.Xoriginal_val = None
 
-        self.model_keras = nets.DenseVollNet
+        self.model_keras = nets.VollNet
 
         self.last_activation = 'softmax'
         self.entropy = 'notbinary'
         self.yolo_loss = volume_yolo_loss(self.categories, self.gridx, self.gridy, self.gridz, self.nboxes,
                                           self.box_vector, self.entropy)
 
     @classmethod   
@@ -175,24 +175,21 @@
         self.Y = self.Y.reshape((self.Y.shape[0],1, 1, 1, self.Y.shape[1]))
         self.Y_val = self.Y_val.reshape((self.Y_val.shape[0],1, 1, 1, self.Y_val.shape[1]))
 
     def TrainModel(self):
 
         #ZYXT
         input_shape = (self.X.shape[1], self.X.shape[2], self.X.shape[3], self.X.shape[4])
+        print(self.X.shape)
+        print(input_shape)
         Path(self.model_dir).mkdir(exist_ok=True)
 
-
-        Y_class = self.Y[:, :, :, :, :self.categories]
-        class_weights = class_weight.compute_class_weight('balanced',
-                                                 np.unique(Y_class),
-                                                 Y_class)
+  
         Y_rest = self.Y[:, :, :, :, self.categories:]
-
-        
+        print(Y_rest.shape)
 
 
         dummyY = np.zeros(
             [self.Y.shape[0], self.Y.shape[1], self.Y.shape[2], self.Y.shape[3], self.categories + self.nboxes * self.box_vector])
         dummyY[:,:, :, :, :self.Y.shape[-1]] = self.Y
 
         dummyY_val = np.zeros([self.Y_val.shape[0], self.Y_val.shape[1], self.Y_val.shape[2], self.Y_val.shape[3],
@@ -206,51 +203,53 @@
                                                                                                                  self.categories: self.categories + self.box_vector]
             dummyY_val[:, :, :,:,
             self.categories + b * self.box_vector:self.categories + (b + 1) * self.box_vector] = self.Y_val[:, :, :,:,
                                                                                                  self.categories: self.categories + self.box_vector]
 
         self.Y = dummyY
         self.Y_val = dummyY_val
+        print(self.Y.shape)
 
         self.Trainingmodel = self.model_keras(input_shape, self.categories, 
                                               box_vector=Y_rest.shape[-1], yolo_loss = self.yolo_loss, nboxes=self.nboxes,
                                               stage_number=self.stage_number,
                                               depth=self.depth, start_kernel=self.start_kernel,
                                               mid_kernel=self.mid_kernel, 
                                               startfilter=self.startfilter, input_model=self.model_dir,
                                               last_activation=self.last_activation)
 
         sgd = tf.keras.optimizers.Adam(learning_rate=self.learning_rate)
         self.Trainingmodel.compile(optimizer=sgd, loss=self.yolo_loss, metrics=['accuracy'])
         self.Trainingmodel.summary()
-       
-   
+        
         # Keras callbacks
+        log_dir = "logs/fit/" + datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
+        tensorboard_callback = callbacks.TensorBoard(log_dir=log_dir, histogram_freq=1)
         lrate = callbacks.ReduceLROnPlateau(monitor='loss', factor=0.1, patience=4, verbose=1)
         hrate = callbacks.History()
-        srate = callbacks.ModelCheckpoint(self.model_dir, monitor='loss',
-                                          save_best_only=False, save_weights_only=False, mode='auto')
+        srate = callbacks.ModelCheckpoint(self.model_dir, monitor='loss', verbose=1,
+                                          save_best_only=False, save_weights_only=False, mode='auto', period=1)
         prate = plotters.PlotVolumeHistory(self.Trainingmodel, self.X_val, self.Y_val, self.key_categories, self.key_cord,
                                      self.gridx, self.gridy, self.gridz, plot=self.show, nboxes=self.nboxes)
+
         
-       
         # Train the model and save as a h5 file
-        self.Trainingmodel.fit(self.X, self.Y, batch_size=self.batch_size,class_weight=class_weights,
-                               epochs=self.epochs, validation_data=(self.X_val, self.Y_val),
-                               callbacks=[lrate, hrate, srate, prate])
+        self.Trainingmodel.fit(self.X, self.Y, batch_size=self.batch_size,
+                               epochs=self.epochs, validation_data=(self.X_val, self.Y_val), shuffle=True,
+                               callbacks=[lrate, hrate, srate, prate, tensorboard_callback])
 
 
         self.Trainingmodel.save(self.model_dir)
     """
     The input image and seg image are numpy arrays that have to be read prior to being loaded in the function
     """
     def get_markers(self, 
                     segimage : np.ndarray):
 
-        self.segimage = segimage.astype(np.uint16)
+        self.segimage = segimage
         print('Obtaining Markers')
         self.pad_width = (self.config['imagey'], self.config['imagex'])
         self.markers = GenerateVolumeMarkers(self.segimage, pad_width = self.pad_width)
         self.marker_tree = MakeForest(self.markers)
         self.segimage = None         
 
         return self.marker_tree
```

### Comparing `oneat-6.0.4/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.0.7/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/neat_focus.py` & `oneat-6.0.7/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.0.7/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.0.7/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.0.7/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.0.7/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.0.7/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import tensorflow as tf
 from tqdm import tqdm
 from oneat.NEATModels import nets
 from oneat.NEATModels.nets import Concat
 from oneat.NEATModels.loss import volume_yolo_loss
 from oneat.pretrained import get_registered_models, get_model_details, get_model_instance
 from pathlib import Path
-from tensorflow.keras.models import load_model
+from keras.models import load_model
 from tifffile import imread
+from sklearn.utils import class_weight
 
-
-class NEATVollNet(object):
+class NEATDenseVollNet(object):
     """
     Parameters
     ----------
     
     NpzDirectory : Specify the location of npz file containing the training data with movies and labels
     
     TrainModelName : Specify the name of the npz file containing training data and labels
@@ -32,15 +32,15 @@
     
     Categories_Name : List of class names and labels
     
     model_dir : Directory location where trained model weights are to be read or written from
     
     model_keras : The model as it appears as a Keras function
     
-    model_weights : If re-training model_weights = model_dir else None as default
+    model : If re-training model = model_dir else None as default
     
     
     epochs :  Number of training epochs, 55 by default
     
     batch_size : batch_size to be used for training, 20 by default
     
     
@@ -132,15 +132,15 @@
         self.axes = None
         self.X_val = None
         self.Y_val = None
         self.Trainingmodel = None
         self.Xoriginal = None
         self.Xoriginal_val = None
 
-        self.model_keras = nets.VollNet
+        self.model_keras = nets.DenseVollNet
 
         self.last_activation = 'softmax'
         self.entropy = 'notbinary'
         self.yolo_loss = volume_yolo_loss(self.categories, self.gridx, self.gridy, self.gridz, self.nboxes,
                                           self.box_vector, self.entropy)
 
     @classmethod   
@@ -175,21 +175,25 @@
         self.Y = self.Y.reshape((self.Y.shape[0],1, 1, 1, self.Y.shape[1]))
         self.Y_val = self.Y_val.reshape((self.Y_val.shape[0],1, 1, 1, self.Y_val.shape[1]))
 
     def TrainModel(self):
 
         #ZYXT
         input_shape = (self.X.shape[1], self.X.shape[2], self.X.shape[3], self.X.shape[4])
-        print(self.X.shape)
-        print(input_shape)
         Path(self.model_dir).mkdir(exist_ok=True)
 
-  
+
+        Y_class = self.Y[:, :, :, :, :self.categories]
+        class_weights = class_weight.compute_class_weight('balanced',
+                                                 classes = np.unique(Y_class),
+                                                 y = Y_class)
+        class_weights = dict(zip(np.unique(self.categories), class_weights))                                         
         Y_rest = self.Y[:, :, :, :, self.categories:]
-        print(Y_rest.shape)
+
+        
 
 
         dummyY = np.zeros(
             [self.Y.shape[0], self.Y.shape[1], self.Y.shape[2], self.Y.shape[3], self.categories + self.nboxes * self.box_vector])
         dummyY[:,:, :, :, :self.Y.shape[-1]] = self.Y
 
         dummyY_val = np.zeros([self.Y_val.shape[0], self.Y_val.shape[1], self.Y_val.shape[2], self.Y_val.shape[3],
@@ -203,53 +207,51 @@
                                                                                                                  self.categories: self.categories + self.box_vector]
             dummyY_val[:, :, :,:,
             self.categories + b * self.box_vector:self.categories + (b + 1) * self.box_vector] = self.Y_val[:, :, :,:,
                                                                                                  self.categories: self.categories + self.box_vector]
 
         self.Y = dummyY
         self.Y_val = dummyY_val
-        print(self.Y.shape)
 
         self.Trainingmodel = self.model_keras(input_shape, self.categories, 
                                               box_vector=Y_rest.shape[-1], yolo_loss = self.yolo_loss, nboxes=self.nboxes,
                                               stage_number=self.stage_number,
                                               depth=self.depth, start_kernel=self.start_kernel,
                                               mid_kernel=self.mid_kernel, 
                                               startfilter=self.startfilter, input_model=self.model_dir,
                                               last_activation=self.last_activation)
 
         sgd = tf.keras.optimizers.Adam(learning_rate=self.learning_rate)
         self.Trainingmodel.compile(optimizer=sgd, loss=self.yolo_loss, metrics=['accuracy'])
         self.Trainingmodel.summary()
-        
+       
+   
         # Keras callbacks
-        log_dir = "logs/fit/" + datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
-        tensorboard_callback = callbacks.TensorBoard(log_dir=log_dir, histogram_freq=1)
         lrate = callbacks.ReduceLROnPlateau(monitor='loss', factor=0.1, patience=4, verbose=1)
         hrate = callbacks.History()
-        srate = callbacks.ModelCheckpoint(self.model_dir, monitor='loss', verbose=1,
-                                          save_best_only=False, save_weights_only=False, mode='auto', period=1)
+        srate = callbacks.ModelCheckpoint(self.model_dir, monitor='loss',
+                                          save_best_only=False, save_weights_only=False, mode='auto')
         prate = plotters.PlotVolumeHistory(self.Trainingmodel, self.X_val, self.Y_val, self.key_categories, self.key_cord,
                                      self.gridx, self.gridy, self.gridz, plot=self.show, nboxes=self.nboxes)
-
         
+       
         # Train the model and save as a h5 file
-        self.Trainingmodel.fit(self.X, self.Y, batch_size=self.batch_size,
-                               epochs=self.epochs, validation_data=(self.X_val, self.Y_val), shuffle=True,
-                               callbacks=[lrate, hrate, srate, prate, tensorboard_callback])
+        self.Trainingmodel.fit(self.X, self.Y, batch_size=self.batch_size,class_weight=class_weights,
+                               epochs=self.epochs, validation_data=(self.X_val, self.Y_val),
+                               callbacks=[lrate, hrate, srate, prate])
 
 
         self.Trainingmodel.save(self.model_dir)
     """
     The input image and seg image are numpy arrays that have to be read prior to being loaded in the function
     """
     def get_markers(self, 
                     segimage : np.ndarray):
 
-        self.segimage = segimage
+        self.segimage = segimage.astype(np.uint16)
         print('Obtaining Markers')
         self.pad_width = (self.config['imagey'], self.config['imagex'])
         self.markers = GenerateVolumeMarkers(self.segimage, pad_width = self.pad_width)
         self.marker_tree = MakeForest(self.markers)
         self.segimage = None         
 
         return self.marker_tree
```

### Comparing `oneat-6.0.4/src/oneat/NEATModels/nets.py` & `oneat-6.0.7/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.0.7/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.0.7/src/oneat/NEATUtils/MovieCreator.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/NMS.py` & `oneat-6.0.7/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.0.7/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.0.7/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.0.7/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.0.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/plotters.py` & `oneat-6.0.7/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/NEATUtils/utils.py` & `oneat-6.0.7/src/oneat/NEATUtils/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/__init__.py` & `oneat-6.0.7/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/_tests/test_nets.py` & `oneat-6.0.7/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/_tests/utils.py` & `oneat-6.0.7/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.0.7/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/_tests/variables/variables.index` & `oneat-6.0.7/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat/pretrained.py` & `oneat-6.0.7/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/src/oneat.egg-info/PKG-INFO` & `oneat-6.0.7/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.0.4
+Version: 6.0.7
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.0.4/src/oneat.egg-info/SOURCES.txt` & `oneat-6.0.7/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-6.0.4/tox.ini` & `oneat-6.0.7/tox.ini`

 * *Files identical despite different names*

