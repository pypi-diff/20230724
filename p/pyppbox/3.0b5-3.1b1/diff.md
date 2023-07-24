# Comparing `tmp/pyppbox-3.0b5.tar.gz` & `tmp/pyppbox-3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-3.0b5.tar", last modified: Mon Jul  3 01:49:29 2023, max compression
+gzip compressed data, was "pyppbox-3.1b1.tar", last modified: Mon Jul 24 18:37:58 2023, max compression
```

## Comparing `pyppbox-3.0b5.tar` & `pyppbox-3.1b1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.471331 pyppbox-3.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-03 01:49:13.000000 pyppbox-3.0b5/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 01:49:13.000000 pyppbox-3.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 01:49:13.000000 pyppbox-3.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 01:49:29.471331 pyppbox-3.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-03 01:49:13.000000 pyppbox-3.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-03 01:49:13.000000 pyppbox-3.0b5/RELEASENOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/config/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/cfg.7z
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/detectors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/reiders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/cfg/trackers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/configtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    65385 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/myconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/config/unifiedstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.447331 pyppbox-3.0b5/pyppbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox/data/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/modules/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.459331 pyppbox-3.0b5/pyppbox/data/res/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/res/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/data/res/idmap.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.459331 pyppbox-3.0b5/pyppbox/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/assets/TReID.png
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/assets/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/guidemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/guihub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/guitools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/gui/tmp/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/tmp/input.tmp
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/tmp/ui.tmp
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_deepsort.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_facenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_gt.py
--rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_torchreid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_yolocls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/gui/ui_yoloult.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/detectors/yolocls/
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/detectors/yolocls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/detectors/yoloult/
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/detectors/yoloult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/reiders/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.463331 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/detect_face.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/facenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/model_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/centroid/
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/centroid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/sort/
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/modules/trackers/sort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/modules/trackers/sort/origin/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.467331 pyppbox-3.0b5/pyppbox/standalone/
--rw-r--r--   0 runner    (1001) docker     (123)    45150 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/standalone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.471331 pyppbox-3.0b5/pyppbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    26550 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/evatools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/gttools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/persontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/restools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyppbox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.455331 pyppbox-3.0b5/pyppbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 01:49:29.000000 pyppbox-3.0b5/pyppbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 01:49:13.000000 pyppbox-3.0b5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:49:29.471331 pyppbox-3.0b5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-03 01:49:13.000000 pyppbox-3.0b5/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 01:49:13.000000 pyppbox-3.0b5/requirements/pippackages_cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-03 01:49:13.000000 pyppbox-3.0b5/requirements/pippackages_cuda.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-03 01:49:13.000000 pyppbox-3.0b5/requirements/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:49:29.471331 pyppbox-3.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-03 01:49:13.000000 pyppbox-3.0b5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 01:49:13.000000 pyppbox-3.0b5/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.935798 pyppbox-3.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-24 18:37:43.000000 pyppbox-3.1b1/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 18:37:43.000000 pyppbox-3.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 18:37:43.000000 pyppbox-3.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-24 18:37:58.935798 pyppbox-3.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-24 18:37:43.000000 pyppbox-3.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-07-24 18:37:43.000000 pyppbox-3.1b1/RELEASENOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.923797 pyppbox-3.1b1/pyppbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.923797 pyppbox-3.1b1/pyppbox/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/config/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/cfg.7z
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/detectors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/reiders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/trackers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/configtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65550 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/myconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/unifiedstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.919798 pyppbox-3.1b1/pyppbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/data/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/modules/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/data/res/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/res/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/res/idmap.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/assets/TReID.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/assets/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/guidemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/guihub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/guitools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/gui/tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/tmp/input.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/tmp/ui.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_facenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_gt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23388 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_torchreid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_yolocls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_yoloult.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/detectors/yolocls/
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/detectors/yolocls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/detectors/yoloult/
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/detectors/yoloult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/reiders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/detect_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/facenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/model_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/centroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/centroid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/sort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/sort/origin/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/standalone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51396 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/standalone/mt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.935798 pyppbox-3.1b1/pyppbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26550 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/evatools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/gttools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/persontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/restools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.923797 pyppbox-3.1b1/pyppbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.935798 pyppbox-3.1b1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-24 18:37:43.000000 pyppbox-3.1b1/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 18:37:43.000000 pyppbox-3.1b1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-24 18:37:43.000000 pyppbox-3.1b1/requirements/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:37:58.935798 pyppbox-3.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-24 18:37:43.000000 pyppbox-3.1b1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 18:37:43.000000 pyppbox-3.1b1/setup_extra.yaml
```

### Comparing `pyppbox-3.0b5/GETSTARTED.md` & `pyppbox-3.1b1/GETSTARTED.md`

 * *Files 15% similar despite different names*

```diff
@@ -14,56 +14,55 @@
   - Python [[3.8-3.11]](https://www.python.org/downloads/)
   - Local pyppbox repo: `git clone https://github.com/rathaumons/pyppbox.git`
 
 * Before you install dependencies/requirements:
   - For Linux, recommend changing `python3` to `python`: `sudo apt install python-is-python3`
   - If you prefer conda + Python [3.8-3.11]: `conda create --name pyppbox_env python=3.10`
   - If you don't know whether to install only Tensorflow or PyTorch or both -> Check [Supported Modules](https://rathaumons.github.io/pyppbox/pyppbox/modules.html)
+  - For Tensorflow with GPU support -> [See here](https://www.tensorflow.org/install/pip)
 
 * Install dependencies/requirments under `pyppbox/requirements/`: 
-  - On Windows, run the `cmd`:
-    - For GPU: `install_req_p3_cuda.cmd` (Line 28 -> PyTorch + CUDA 11.8, change if you need to)
-    - For CPU-only: `install_req_p3_cpu.cmd`
-  - On Linux:
+  - On Windows, recommend using the `cmd` installer:
+    - For GPU: `install_req_py3_cuda.cmd` (Line 27 -> PyTorch + CUDA 11.8, change if you need to)
+    - For CPU-only: `install_req_py3_cpu.cmd`
+  - On Linux (Or Windows):
     - For GPU (Example for PyTorch CUDA 11.8):
       ```
       python -m pip install --upgrade pip
       pip uninstall -y ultralytics # Remove the official ultralytics
       pip install "setuptools>=67.2.0"
-      pip install -r pippackages_cuda.txt
       pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
+      pip install -r requirements.txt
       ```
     - For CPU-only:
       ```
       python -m pip install --upgrade pip
       pip uninstall -y ultralytics # Remove the official ultralytics
       pip install "setuptools>=67.2.0"
-      pip install -r pippackages_cpu.txt
       pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
+      pip install -r requirements.txt
       ```
   - On macOS:
     - For GPU: No support
     - For CPU:
       ```
       python -m pip install --upgrade pip
       pip uninstall -y ultralytics # Remove the official ultralytics
       pip install "setuptools>=67.2.0"
-      pip install -r pippackages_cpu.txt
-      pip install torch torchvision torchaudio
+      pip install -r requirements.txt
       ```
 
 * (Optional) For GPU-Only -> Verify the installed dependencies:
   - Execute the `test_gpu.py`
     - On Windows -> `test_gpu.cmd`
     - On Linux -> `python test_gpu.py`
   - If there is no error, then you are all good and ready to go.
-  - For OpenCV, the official `opencv-contrib-python` (No GPU support) is set in the `pippackages_cuda.txt` file. If you need GPU support, check our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) or build one from source by yourself.
+  - For OpenCV, the official `opencv-contrib-python` (No GPU support) is set in the `requirements.txt` file. If you need GPU support, check our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) or build one from source by yourself.
 
 * ⚠️ ***Notes:***
-  - For CPU-Only, Torchreid does not work on CPU -> `pyppbox-torchreid` is excluded from `pippackages_cpu.txt`.
   - For CPU-Only, YOLO Ultralytics uses GPU by default, you must set `cpu` as string for the parameter `device` in its configuration.
   - For GPU on Windows, [Tensorflow 2.11+ no long provides native GPU support](https://www.tensorflow.org/install/pip#windows-native). 
 
 
 ## 💽 Setup
 
 You need to install the main package which is `pyppbox` and the data for the modules you need `pyppbox-data-xxx`. If you want to have some fun for the demo on our [GTA_V_DATASET](https://github.com/rathaumons/PoseTReID_DATASET), you also need to install `pyppbox-data-gta5`.
@@ -109,18 +108,24 @@
     ```
     python
     import pyppbox
     pyppbox.launchGUI()
     ```
   - Now you should see the GUI of pyppbox for easy demo.
     <details><summary><ins>Show GUI example!</ins></summary><img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_gui.jpg"></details>
-  - For Linux, if the GUI does not work, you might need to install these:
+  - For ***Linux***, if the GUI does not work, you might need to install these:
     ```
     sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev
     ```
+  - For ***Ubuntu on WSL 2***, you need to install these:
+    ```
+    sudo apt-get install libgl1-mesa-glx
+    sudo apt-get install xdg-utils
+    sudo apt-get install libegl1
+    ```
 
 ## 📢 FYI
 
 ### 1️⃣ Customized OpenCV
 
 OpenCV is widely used in many well-known packages, but the majority of the prebuilt WHLs on the Internet including the official one on PyPI do not include GPU support. Thus, we build our custom one which includes NVIDIA [CUDA](https://developer.nvidia.com/cuda-downloads) & [cuDNN](https://developer.nvidia.com/rdp/cudnn-download) supports for the [OpenCV DNN module](https://docs.opencv.org/4.x/d2/d58/tutorial_table_of_content_dnn.html). In order to well distinguish from the rest, we decided to build and change the package name from `opencv-contrib-python` to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) -> [[Repo]](https://github.com/rathaumons/opencv-for-pyppbox) [[WHL]](https://github.com/rathaumons/opencv-for-pyppbox/releases)
```

### Comparing `pyppbox-3.0b5/LICENSE` & `pyppbox-3.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/PKG-INFO` & `pyppbox-3.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.0b5
+Version: 3.1b1
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -44,11 +44,11 @@
 
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
-* Intergrate GUI for easy configurations and demo.
+* Integrate GUI for easy configurations and demo.
 * Support YAML/JSON configurations -> File, raw string and ready dictionary.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.0b5/README.md` & `pyppbox-3.1b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
-* Intergrate GUI for easy configurations and demo.
+* Integrate GUI for easy configurations and demo.
 * Support YAML/JSON configurations -> File, raw string and ready dictionary.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.0b5/RELEASENOTES.md` & `pyppbox-3.1b1/RELEASENOTES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Release Notes 
 
 ## **pyppbox V3 - Make Simpler and Faster**
 
+* `pyppbox` [v3.1b1](https://github.com/rathaumons/pyppbox/tree/v3.1b1)
+
+  - Add multithreading support for standalone -> `ppbox.standalone.mt.MT`
+  - Add multithreading example -> See example 13
+  - Add CPU support for `Torchreid`
+  - Implement install requirements/dependencies -> See setup.py
+  - Simplify and improve requirements
+  - Update default config files
+  - Update and improve documentations
+  - Update and improve GUI
+
 * `pyppbox` [v3.0b5](https://github.com/rathaumons/pyppbox/tree/v3.0b5)
 
   - Fix a critical bug in GUI of FaceNet which can cause missing `train_data` configuration
   - Fix and improve documentation
   - **Known issue/limitation**: 
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
```

### Comparing `pyppbox-3.0b5/pyppbox/__init__.py` & `pyppbox-3.1b1/pyppbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     useInternalConfigDir, 
     useThisConfigDir,
     resetInternalConfig,
     generateConfig
 )
 
 
-__version__ = '3.0b5'
+__version__ = '3.1b1'
 __author__ = 'Ratha SIV'
 __description__ = 'Toolbox for people detecting, tracking, and re-identifying.'
 __homepage__ = 'https://rathaumons.github.io/pyppbox'
 __url__ = 'https://github.com/rathaumons/pyppbox.git'
```

### Comparing `pyppbox-3.0b5/pyppbox/config/__init__.py` & `pyppbox-3.1b1/pyppbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/config/cfg/detectors.yaml` & `pyppbox-3.1b1/pyppbox/config/cfg/detectors.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/config/cfg/reiders.yaml` & `pyppbox-3.1b1/pyppbox/config/cfg/reiders.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # --- # Torchreid
 # ri_name: Torchreid
 # classifier_pkl: data/modules/torchreid/classifier/gta5_osnet_ain_ms_d_c.pkl
 # train_data: data/datasets/GTA_V_DATASET/body_128x256
 # model_name: osnet_ain_x1_0
 # model_path: data/modules/torchreid/models/torchreid/osnet_ain_ms_d_c.pth.tar
 # min_confidence: 0.35
+# device: cuda
 ###########################################################
 ri_name: FaceNet
 gpu_mem: 0.585
 model_det: data/modules/facenet/models/det
 model_file: data/modules/facenet/models/20180402-114759/20180402-114759.pb
 classifier_pkl: data/modules/facenet/classifier/gta5.pkl
 train_data: data/datasets/GTA_V_DATASET/face_182x182
@@ -34,7 +35,8 @@
 ---
 ri_name: Torchreid
 classifier_pkl: data/modules/torchreid/classifier/gta5_osnet_ain_ms_d_c.pkl
 train_data: data/datasets/GTA_V_DATASET/body_128x256
 model_name: osnet_ain_x1_0
 model_path: data/modules/torchreid/models/torchreid/osnet_ain_ms_d_c.pth.tar
 min_confidence: 0.35
+device: cuda
```

### Comparing `pyppbox-3.0b5/pyppbox/config/cfg/trackers.yaml` & `pyppbox-3.1b1/pyppbox/config/cfg/trackers.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/config/configtools.py` & `pyppbox-3.1b1/pyppbox/config/configtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/config/myconfig.py` & `pyppbox-3.1b1/pyppbox/config/myconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -691,15 +691,15 @@
     """
     A class used to store the necessary configurations of reider FaceNet.
 
     Attributes
     ----------
     unified_strings : MyStrings, auto
         A :class:`MyStrings` object used to store unified strings.
-    tk_name : str
+    ri_name : str
         Configured name of reider FaceNet.
     gpu_mem : float
         Limit GPU memory usage.
     model_det : str
         Path of the det directory where stores .npy files.
     model_file : str
         Path of a pretrained model file for reider FaceNet.
@@ -805,27 +805,29 @@
     """
     A class used to store the necessary configurations of reider Torchreid.
 
     Attributes
     ----------
     unified_strings : MyStrings, auto
         A :class:`MyStrings` object used to store unified strings.
-    tk_name : str
+    ri_name : str
         Configured name of reider Torchreid.
     classifier_pkl : str
         Path of classifier PKL file.
     train_data : str
         Path of a data directory where there must be 2 or more sub-folders which classify 
         different people.
     model_name : str
         Name of a model corresponding to the pretrained model.
     model_path : str
         Path of a pretrained model file for reider Torchreid.
     min_confidence : float
         Mininum confidence of the prediction.
+    device : str
+        Parameter device for specifying a computing device.
     base_model_path : str
         Path of a base model corresponding to the pretrained model or :attr:`model_name`. 
     model_dict : TorchreidModelDict, auto
         A :class:`TorchreidModelDict` object used to store the dictionary of a Torchreid model.
     model_wh : tuple(int, int), auto
         A tuple used to store the input image size :code:`(width, height)` for a corresponding 
         Torchreid model.
@@ -873,14 +875,15 @@
                                                             self.configs['classifier_pkl'])
                 self.train_data = getAdaptiveAbsPathFDS(self.from_dir, 
                                                         self.configs['train_data'])
                 self.model_name = self.configs['model_name']
                 self.model_path = getAdaptiveAbsPathFDS(self.from_dir, 
                                                         self.configs['model_path'])
                 self.min_confidence = self.configs['min_confidence']
+                self.device = self.configs['device']
                 self.configs = self.getDocument()
                 self.base_model_path = getAdaptiveAbsPathFDS(
                     self.from_dir, 
                     joinFPathFull(getAncestorDir(self.model_path, 1), 'base')
                 )
                 self.model_dict = TorchreidModelDict()
                 self.model_wh = self.model_dict.getWH(getFileName(self.model_path))
@@ -1030,14 +1033,15 @@
                 "# --- # Torchreid\n"
                 "# ri_name: Torchreid\n"
                 "# classifier_pkl: data/modules/torchreid/classifier/gta5_osnet_ain_ms_d_c.pkl\n"
                 "# train_data: data/datasets/GTA_V_DATASET/body_128x256\n"
                 "# model_name: osnet_ain_x1_0\n"
                 "# model_path: data/modules/torchreid/models/torchreid/osnet_ain_ms_d_c.pth.tar\n"
                 "# min_confidence: 0.35\n"
+                "# device: cuda\n"
                 "###########################################################\n")
         return header
 
     def copyrightCMDHeader(self):
         """
         Return copyright header string.
```

### Comparing `pyppbox-3.0b5/pyppbox/config/unifiedstrings.py` & `pyppbox-3.1b1/pyppbox/config/unifiedstrings.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/gui/__init__.py` & `pyppbox-3.1b1/pyppbox/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/gui/assets/TReID.png` & `pyppbox-3.1b1/pyppbox/gui/assets/TReID.png`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/gui/assets/icon.ico` & `pyppbox-3.1b1/pyppbox/gui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/gui/assets/settings.ico` & `pyppbox-3.1b1/pyppbox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/gui/guidemo.py` & `pyppbox-3.1b1/pyppbox/gui/guidemo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/gui/guihub.py` & `pyppbox-3.1b1/pyppbox/gui/guihub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/gui/guitools.py` & `pyppbox-3.1b1/pyppbox/gui/guitools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_centroid.py` & `pyppbox-3.1b1/pyppbox/gui/ui_centroid.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.config.myconfig import MyConfigurator as MyCFG
 from pyppbox.utils.commontools import getInt
 
 
+unified_strings = UnifiedStrings()
+
 class Ui_Centroid(object):
 
     def __init__(self, cfg_mode, cfg_dir):
         self.cfg_dir = cfg_dir
         if cfg_mode == 0:
             self.mycfg = MyCFG()
         else:
@@ -74,14 +77,14 @@
 
     def loadCT(self):
         self.mycfg.setAllTCFG()
         self.ct_max_distance_lineEdit.setText(str(self.mycfg.tcfg_centroid.max_spread))
 
     def updateCFG(self, centroid_ui):
         centroid_doc = {
-            "tk_name": "Centroid",
+            "tk_name": unified_strings.getUnifiedFormat("Centroid"),
             "max_spread": getInt(self.ct_max_distance_lineEdit.text(), default_val=50)
         }
         sort_doc = self.mycfg.tcfg_sort.getDocument()
         deepsort_doc = self.mycfg.tcfg_deepsort.getDocument()
         self.mycfg.dumpAllTCFG([centroid_doc, sort_doc, deepsort_doc])
         centroid_ui.close()
```

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_deepsort.py` & `pyppbox-3.1b1/pyppbox/gui/ui_deepsort.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.config.myconfig import MyConfigurator as MyCFG
 from pyppbox.utils.commontools import (getAbsPathFDS, normalizePathFDS, 
                                        getGlobalRootDir, getAncestorDir, 
                                        getFloat, getInt)
 
 
+unified_strings = UnifiedStrings()
 root_dir = getGlobalRootDir()
 
 class Ui_DeepSORT(object):
 
     def __init__(self, cfg_mode, cfg_dir):
         self.cfg_dir = cfg_dir
         if cfg_mode == 0:
@@ -117,15 +119,15 @@
         self.ds_cosine_distance_lineEdit.setText(str(self.mycfg.tcfg_deepsort.max_cosine_distance))
         self.ds_max_overlap_lineEdit.setText(str(self.mycfg.tcfg_deepsort.nms_max_overlap))
         self.ds_nn_budget_lineEdit.setText(str(self.mycfg.tcfg_deepsort.nn_budget))
         self.ds_model_file_lineEdit.setText(getAbsPathFDS(self.mycfg.tcfg_deepsort.model_file))
 
     def updateCFG(self, YOLOForm):
         deepsort_doc = {
-            "tk_name": "DeepSORT",
+            "tk_name": unified_strings.getUnifiedFormat("DeepSORT"),
             "nn_budget": getInt(self.ds_nn_budget_lineEdit.text(), default_val=100),
             "nms_max_overlap": getFloat(self.ds_max_overlap_lineEdit.text(), default_val=0.5),
             "max_cosine_distance": getFloat(self.ds_cosine_distance_lineEdit.text(), default_val=0.1),
             "model_file": normalizePathFDS(root_dir, self.ds_model_file_lineEdit.text())
         }
         centroid_doc = self.mycfg.tcfg_centroid.getDocument()
         sort_doc = self.mycfg.tcfg_sort.getDocument()
```

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_facenet.py` & `pyppbox-3.1b1/pyppbox/gui/ui_facenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.config.myconfig import MyConfigurator as MyCFG
 from pyppbox.utils.commontools import (getAbsPathFDS, normalizePathFDS, 
                                        getGlobalRootDir, getAncestorDir, 
                                        get2Dlist, getFloat, getInt)
 
 
+unified_strings = UnifiedStrings()
 root_dir = getGlobalRootDir()
 
 class Ui_FaceNet(object):
 
     def __init__(self, cfg_mode, cfg_dir):
         self.cfg_dir = cfg_dir
         if cfg_mode == 0:
@@ -192,15 +194,15 @@
         self.fn_model_file_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_facenet.model_file))
         self.fn_model_det_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_facenet.model_det))
         self.fn_yl_h_calib_lineEdit.setText(str(self.mycfg.rcfg_facenet.yl_h_calibration))
         self.fn_yl_w_calib_lineEdit.setText(str(self.mycfg.rcfg_facenet.yl_w_calibration))
 
     def updateCFG(self, facenet_ui):
         facenet_doc = {
-            "ri_name": "FaceNet",
+            "ri_name": unified_strings.getUnifiedFormat("FaceNet"),
             "gpu_mem": getFloat(self.fn_gpu_mem_lineEdit.text(), default_val=0.585),
             "model_det": normalizePathFDS(root_dir, self.fn_model_det_lineEdit.text()), 
             "model_file": normalizePathFDS(root_dir, self.fn_model_file_lineEdit.text()),
             "classifier_pkl": normalizePathFDS(root_dir, self.fn_classifier_pkl_lineEdit.text()),
             "train_data": normalizePathFDS(root_dir, self.fn_train_data_lineEdit.text()),
             "batch_size": getInt(self.fn_batch_size_lineEdit.text(), default_val=0.5),
             "min_confidence": getFloat(self.fn_min_confidence_lineEdit.text(), default_val=0.75),
```

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_gt.py` & `pyppbox-3.1b1/pyppbox/gui/ui_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.config.myconfig import MyConfigurator as MyCFG
 from pyppbox.utils.commontools import (normalizePathFDS, getAbsPathFDS, 
                                        getGlobalRootDir, getAncestorDir)
 
 
+unified_strings = UnifiedStrings()
 root_dir = getGlobalRootDir()
 
 class Ui_GT(object):
 
     def __init__(self, cfg_mode, cfg_dir):
         self.cfg_dir = cfg_dir
         if cfg_mode == 0:
@@ -113,14 +115,14 @@
         file_filter = "Text (*.txt)"
         source_file, _ = QtWidgets.QFileDialog.getOpenFileName(None, "Input GT Map file", 
                                                                default_path, file_filter)
         if source_file:
             self.gt_map_lineEdit.setText(source_file)
 
     def updateCFG(self, gi_ui):
-        gt_doc = {"dt_name": "GT",
+        gt_doc = {"dt_name": unified_strings.getUnifiedFormat("GT"),
                   "gt_file": normalizePathFDS(root_dir, self.gt_file_lineEdit.text()),
                   "gt_map_file": normalizePathFDS(root_dir, self.gt_map_lineEdit.text())}
         yolo_doc = self.mycfg.dcfg_yolocs.getDocument()
         yolo_utlt_doc = self.mycfg.dcfg_yolout.getDocument()
         self.mycfg.dumpAllDCFG([yolo_doc, yolo_utlt_doc, gt_doc])
         gi_ui.close()
```

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_launcher.py` & `pyppbox-3.1b1/pyppbox/gui/ui_launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,8 +458,7 @@
     app = QtWidgets.QApplication(sys.argv)
     launcher = QtWidgets.QMainWindow()
     launcher.setWindowIcon(QtGui.QIcon(joinFPathFull(current_dir, "assets/settings.ico")))
     ui = Ui_PYPPBOXLauncher(cfg_mode=cfg_mode, cfg_dir=cfg_dir)
     ui.setupUi(launcher)
     launcher.show()
     sys.exit(app.exec())
-
```

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_sort.py` & `pyppbox-3.1b1/pyppbox/gui/ui_sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.config.myconfig import MyConfigurator as MyCFG
 from pyppbox.utils.commontools import getFloat, getInt
 
 
+unified_strings = UnifiedStrings()
+
 class Ui_SORT(object):
 
     def __init__(self, cfg_mode, cfg_dir):
         self.cfg_dir = cfg_dir
         if cfg_mode == 0:
             self.mycfg = MyCFG()
         else:
@@ -96,15 +99,15 @@
         self.mycfg.setAllTCFG()
         self.st_iou_threshold_lineEdit.setText(str(self.mycfg.tcfg_sort.iou_threshold))
         self.st_max_age_lineEdit.setText(str(self.mycfg.tcfg_sort.max_age))
         self.st_min_hits_lineEdit.setText(str(self.mycfg.tcfg_sort.min_hits))
 
     def updateCFG(self, sort_ui):
         sort_doc = {
-            "tk_name": "SORT",
+            "tk_name": unified_strings.getUnifiedFormat("SORT"),
             "max_age": getInt(self.st_max_age_lineEdit.text(), default_val=1),
             "min_hits": getInt(self.st_min_hits_lineEdit.text(), default_val=3),
             "iou_threshold": getFloat(self.st_iou_threshold_lineEdit.text(), default_val=0.3)
         }
         centroid_doc = self.mycfg.tcfg_centroid.getDocument()
         deepsort_doc = self.mycfg.tcfg_deepsort.getDocument()
         self.mycfg.dumpAllTCFG([centroid_doc, sort_doc, deepsort_doc])
```

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_torchreid.py` & `pyppbox-3.1b1/pyppbox/gui/ui_torchreid.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.config.myconfig import MyConfigurator as MyCFG
 from pyppbox.modules.reiders.torchreid.model_dict import TorchreidModelDict
 from pyppbox.utils.commontools import (getAbsPathFDS, normalizePathFDS, getFileName, 
                                        getGlobalRootDir, getAncestorDir, joinFPathFull,
-                                       getFloat)
+                                       getFloat, getInt)
 
 
+unified_strings = UnifiedStrings()
 root_dir = getGlobalRootDir()
 global_cfg_root = joinFPathFull(root_dir, 'cfg')
 internal_cfg_dir = joinFPathFull(global_cfg_root, 'configurations')
 
 class Ui_Torchreid(object):
 
     def __init__(self, cfg_mode, cfg_dir):
@@ -38,35 +40,35 @@
         if cfg_mode == 0:
             self.mycfg = MyCFG()
         else:
             self.mycfg = MyCFG(self.cfg_dir)
 
     def setupUi(self, torchreid_ui):
         torchreid_ui.setObjectName("torchreid_ui")
-        torchreid_ui.resize(390, 210)
+        torchreid_ui.resize(390, 240)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, 
                                            QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(torchreid_ui.sizePolicy().hasHeightForWidth())
         torchreid_ui.setSizePolicy(sizePolicy)
-        torchreid_ui.setMinimumSize(QtCore.QSize(390, 210))
-        torchreid_ui.setMaximumSize(QtCore.QSize(390, 210))
+        torchreid_ui.setMinimumSize(QtCore.QSize(390, 240))
+        torchreid_ui.setMaximumSize(QtCore.QSize(390, 240))
         self.dr_model_path_label = QtWidgets.QLabel(torchreid_ui)
         self.dr_model_path_label.setGeometry(QtCore.QRect(10, 100, 91, 16))
         self.dr_model_path_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
                                               QtCore.Qt.AlignmentFlag.AlignTrailing|
                                               QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.dr_model_path_label.setObjectName("dr_model_path_label")
         self.dr_min_confidence_lineEdit = QtWidgets.QLineEdit(torchreid_ui)
         self.dr_min_confidence_lineEdit.setGeometry(QtCore.QRect(110, 130, 241, 21))
         self.dr_min_confidence_lineEdit.setReadOnly(False)
         self.dr_min_confidence_lineEdit.setObjectName("dr_min_confidence_lineEdit")
         self.save_pushButton = QtWidgets.QPushButton(torchreid_ui)
-        self.save_pushButton.setGeometry(QtCore.QRect(150, 170, 91, 31))
+        self.save_pushButton.setGeometry(QtCore.QRect(150, 200, 91, 31))
         font = QtGui.QFont()
         font.setPointSize(12)
         self.save_pushButton.setFont(font)
         self.save_pushButton.setDefault(True)
         self.save_pushButton.setObjectName("save_pushButton")
         self.dr_min_confidence_label = QtWidgets.QLabel(torchreid_ui)
         self.dr_min_confidence_label.setGeometry(QtCore.QRect(10, 130, 91, 16))
@@ -112,14 +114,23 @@
         self.dr_classifier_pkl_pushButton = QtWidgets.QPushButton(torchreid_ui)
         self.dr_classifier_pkl_pushButton.setGeometry(QtCore.QRect(360, 10, 21, 24))
         self.dr_classifier_pkl_pushButton.setObjectName("dr_classifier_pkl_pushButton")
         self.dr_classifier_pkl_lineEdit = QtWidgets.QLineEdit(torchreid_ui)
         self.dr_classifier_pkl_lineEdit.setGeometry(QtCore.QRect(110, 10, 241, 21))
         self.dr_classifier_pkl_lineEdit.setReadOnly(True)
         self.dr_classifier_pkl_lineEdit.setObjectName("dr_classifier_pkl_lineEdit")
+        self.dr_devices_label = QtWidgets.QLabel(torchreid_ui)
+        self.dr_devices_label.setGeometry(QtCore.QRect(10, 160, 91, 16))
+        self.dr_devices_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|
+                                        QtCore.Qt.AlignmentFlag.AlignTrailing|
+                                        QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.dr_devices_label.setObjectName("dr_devices_label")
+        self.dr_device_lineEdit = QtWidgets.QLineEdit(torchreid_ui)
+        self.dr_device_lineEdit.setGeometry(QtCore.QRect(110, 160, 241, 21))
+        self.dr_device_lineEdit.setObjectName("dr_device_lineEdit")
         self.retranslateUi(torchreid_ui)
         # custom
         self.md = TorchreidModelDict()
         self.loadDR()
         self.dr_classifier_pkl_pushButton.clicked.connect(self.browseClassifierPKL)
         self.dr_train_data_pushButton.clicked.connect(self.browseTrainData)
         self.dr_model_path_pushButton.clicked.connect(self.browseModelPath)
@@ -128,37 +139,48 @@
 
     def retranslateUi(self, torchreid_ui):
         _translate = QtCore.QCoreApplication.translate
         torchreid_ui.setWindowTitle(_translate("torchreid_ui", "Torchreid"))
         self.dr_model_path_label.setText(_translate("torchreid_ui", "model_path"))
         self.save_pushButton.setText(_translate("torchreid_ui", "Save"))
         self.dr_min_confidence_label.setText(_translate("torchreid_ui", "min_confidence"))
+        self.dr_devices_label.setText(_translate("torchreid_ui", "device"))
+        self.dr_device_lineEdit.setPlaceholderText(_translate("torchreid_ui", "cuda"))
         self.dr_classifier_pkl_label.setText(_translate("torchreid_ui", "classifier_pkl"))
         self.dr_train_data_pushButton.setText(_translate("torchreid_ui", "..."))
         self.dr_model_path_pushButton.setText(_translate("torchreid_ui", "..."))
         self.dr_model_name_label.setText(_translate("torchreid_ui", "model_name"))
         self.dr_train_data_label.setText(_translate("torchreid_ui", "train_data"))
         self.dr_classifier_pkl_pushButton.setText(_translate("torchreid_ui", "..."))
 
     def loadDR(self):
         self.mycfg.setAllRCFG()
         self.dr_classifier_pkl_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_torchreid.classifier_pkl))
         self.dr_train_data_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_torchreid.train_data))
         self.dr_model_name_lineEdit.setText(str(self.mycfg.rcfg_torchreid.model_name))
         self.dr_model_path_lineEdit.setText(getAbsPathFDS(self.mycfg.rcfg_torchreid.model_path))
         self.dr_min_confidence_lineEdit.setText(str(self.mycfg.rcfg_torchreid.min_confidence))
+        self.dr_device_lineEdit.setText(str(self.mycfg.rcfg_torchreid.device))
 
     def updateCFG(self, torchreid_ui):
+        device = 'cuda'
+        if 'cpu' in self.dr_device_lineEdit.text().lower():
+            device = 'cpu'
+        elif 'cuda' in self.dr_device_lineEdit.text().lower():
+            device = 'cuda'
+        else:
+            device = getInt(self.dr_device_lineEdit.text())
         Torchreid_doc = {
-            "ri_name": "Torchreid",
+            "ri_name": unified_strings.getUnifiedFormat("Torchreid"),
             "classifier_pkl": normalizePathFDS(root_dir, self.dr_classifier_pkl_lineEdit.text()),
             "train_data": normalizePathFDS(root_dir, self.dr_train_data_lineEdit.text()),
             "model_name": self.dr_model_name_lineEdit.text(),
             "model_path": normalizePathFDS(root_dir, self.dr_model_path_lineEdit.text()),
-            "min_confidence": getFloat(self.dr_min_confidence_lineEdit.text(), default_val=0.35)
+            "min_confidence": getFloat(self.dr_min_confidence_lineEdit.text(), default_val=0.35),
+            "device": device
         }
         facenet_doc = self.mycfg.rcfg_facenet.getDocument()
         self.mycfg.dumpAllRCFG([facenet_doc, Torchreid_doc])
         torchreid_ui.close()
 
     def browseTrainData(self):
         default_path = getAncestorDir(self.mycfg.rcfg_torchreid.train_data)
```

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_yolocls.py` & `pyppbox-3.1b1/pyppbox/gui/ui_yolocls.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.config.myconfig import MyConfigurator as MyCFG
 from pyppbox.utils.commontools import (getAbsPathFDS, normalizePathFDS, 
                                        getGlobalRootDir, getAncestorDir, 
                                        getFloat, getInt)
 
 
+unified_strings = UnifiedStrings()
 root_dir = getGlobalRootDir()
 
 class Ui_YOLOCLS(object):
 
     def __init__(self, cfg_mode, cfg_dir):
         self.cfg_dir = cfg_dir
         if cfg_mode == 0:
@@ -161,17 +163,16 @@
         self.yl_model_cfg_file_lineEdit.setText(getAbsPathFDS(self.mycfg.dcfg_yolocs.model_cfg_file))
         self.yl_class_file_lineEdit.setText(getAbsPathFDS(self.mycfg.dcfg_yolocs.class_file))
         self.yl_model_weights_lineEdit.setText(getAbsPathFDS(self.mycfg.dcfg_yolocs.model_weights))
         self.yl_model_imgsize_lineEdit.setText(str(self.mycfg.dcfg_yolocs.model_image_size))
         self.yl_repspint_calib_lineEdit.setText(str(self.mycfg.dcfg_yolocs.repspoint_calibration))
 
     def updateCFG(self, yolocls_ui):
-        decorated_name = str(self.mycfg.dcfg_yolocs.dt_name).title().replace("Yolo", "YOLO")
         yolocs_doc = {
-            "dt_name": decorated_name,
+            "dt_name": unified_strings.getUnifiedFormat("YOLO_Classic"),
             "nms": getFloat(self.yl_nms_lineEdit.text(), default_val=0.45),
             "conf": getFloat(self.yl_conf_lineEdit.text(), default_val=0.5),
             "class_file": normalizePathFDS(root_dir, self.yl_class_file_lineEdit.text()),
             "model_cfg_file": normalizePathFDS(root_dir, self.yl_model_cfg_file_lineEdit.text()),
             "model_weights": normalizePathFDS(root_dir, self.yl_model_weights_lineEdit.text()),
             "model_image_size": getInt(self.yl_model_imgsize_lineEdit.text(), default_val=416),
             "repspoint_calibration": getFloat(self.yl_repspint_calib_lineEdit.text(), default_val=0.25)
@@ -200,8 +201,7 @@
     def browseModelWeights(self):
         default_path = getAncestorDir(self.mycfg.dcfg_yolocs.model_weights)
         weight_filter = "Weights (*.weights)"
         source_file, _ = QtWidgets.QFileDialog.getOpenFileName(None, "Model weights file", 
                                                                default_path, weight_filter)
         if source_file:
             self.yl_model_weights_lineEdit.setText(source_file)
-
```

### Comparing `pyppbox-3.0b5/pyppbox/gui/ui_yoloult.py` & `pyppbox-3.1b1/pyppbox/gui/ui_yoloult.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.config.myconfig import MyConfigurator as MyCFG
 from pyppbox.utils.commontools import (getAbsPathFDS, normalizePathFDS, 
                                        getGlobalRootDir, getAncestorDir, 
                                        getFloat, getInt)
 
-
+unified_strings = UnifiedStrings()
 root_dir = getGlobalRootDir()
 
 class Ui_YOLOULT(object):
 
     def __init__(self, cfg_mode, cfg_dir):
         self.cfg_dir = cfg_dir
         if cfg_mode == 0:
@@ -190,22 +191,23 @@
     def loadComboBoxes(self):
         if self.mycfg.dcfg_yolout.boxes is True:
             self.boxes_comboBox.setCurrentIndex(0)
         else:
             self.boxes_comboBox.setCurrentIndex(1)
 
     def updateCFG(self, yoloult_ui):
-        decorated_name = str(self.mycfg.dcfg_yolout.dt_name).title().replace("Yolo", "YOLO")
         device = 0
         if 'cpu' in self.device_lineEdit.text().lower():
             device = 'cpu'
+        elif 'cuda' in self.device_lineEdit.text().lower():
+            device = 'cuda'
         else:
             device = getInt(self.device_lineEdit.text())
         yolo_utlt_doc = {
-            "dt_name": decorated_name,
+            "dt_name": unified_strings.getUnifiedFormat("YOLO_Ultralytics"),
             "conf": getFloat(self.conf_lineEdit.text(), default_val=0.5),
             "iou": getFloat(self.iou_lineEdit.text(), default_val=0.7),
             "imgsz": getInt(self.imgsz_lineEdit.text(), default_val=416),
             "boxes": self.boxes_comboBox.currentText(),
             "device": device,
             "max_det": getInt(self.max_det_lineEdit.text(), default_val=100),
             "line_width": getInt(self.line_width_lineEdit.text(), default_val=500),
@@ -220,8 +222,7 @@
     def browseModelFile(self):
         default_path = getAncestorDir(self.mycfg.dcfg_yolout.model_file)
         model_filter = "Model (*.pt)"
         source_file, _ = QtWidgets.QFileDialog.getOpenFileName(None, "Model file", 
                                                                default_path, model_filter)
         if source_file:
             self.model_file_lineEdit.setText(source_file)
-
```

### Comparing `pyppbox-3.0b5/pyppbox/modules/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/detectors/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/detectors/yolocls/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/detectors/yolocls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/detectors/yoloult/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/detectors/yoloult/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,16 @@
             img,
             imgsz=int(self.cfg.imgsz),
             conf=float(self.cfg.conf),
             classes=classes,
             boxes=self.cfg.boxes,
             device=self.cfg.device,
             max_det=int(self.cfg.max_det),
-            line_width=self.cfg.line_width
+            line_width=self.cfg.line_width,
+            verbose=False
         )
         if self.cpu_only:
             numpy_dets = dets[0].numpy()
         else:
             numpy_dets = dets[0].cuda().cpu().to("cpu").numpy()
         dt_boxes_xyxy = numpy_dets.boxes.xyxy
         dt_confidences = numpy_dets.boxes.conf
@@ -228,15 +229,16 @@
             img,
             imgsz=int(self.cfg.imgsz),
             conf=float(self.cfg.conf),
             classes=0,
             boxes=self.cfg.boxes,
             device=self.cfg.device,
             max_det=int(self.cfg.max_det),
-            line_width=self.cfg.line_width
+            line_width=self.cfg.line_width,
+            verbose=False
         )
         if self.cpu_only:
             numpy_dets = dets[0].numpy()
         else:
             numpy_dets = dets[0].cuda().cpu().to("cpu").numpy()
         dt_boxes_xyxy = numpy_dets.boxes.xyxy
         dt_confidences = numpy_dets.boxes.conf
```

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/reiders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/facenet/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/reiders/facenet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py` & `pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/detect_face.py` & `pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/detect_face.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/facenet/origin/facenet.py` & `pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,19 @@
         self.unk = cfg.unified_strings.unk_did
         self.err = cfg.unified_strings.err_did
         self.mdir = cfg.base_model_path
         self.classifier_pkl = cfg.classifier_pkl
         self.train_data = cfg.train_data
         self.model_name = cfg.model_name
         self.model_path = cfg.model_path
+        self.device = cfg.device
         self.min_confidence = int(100 * cfg.min_confidence)
         # add_info_log("--------RI : Initializing ReID model ...")
-        self.extractor = deepreid_extractor(self.model_name, self.mdir, self.model_path)
+        self.extractor = deepreid_extractor(self.model_name, self.mdir, 
+                                            self.model_path, device=self.device)
         self.auto_load = auto_load
         if self.auto_load:
             self.load_classifier()
 
     def load_classifier(self):
         """Load the classifier model from the configurations.
         """
```

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/model_dict.py` & `pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/model_dict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/model_dict.yaml` & `pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/model_dict.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/reiders/torchreid/utils.py` & `pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,24 +63,24 @@
     image_paths = []
     if os.path.isdir(datadir):
         images = os.listdir(datadir)
         image_paths = [os.path.join(datadir, img) for img in images]
     return image_paths
 
 @silencer
-def deepreid_extractor(model_name, model_dir, model_path):
+def deepreid_extractor(model_name, model_dir, model_path, device='cuda'):
     ignore_this_logger("torchreid")
     ignore_this_logger("pyppbox_torchreid")
     from pyppbox_torchreid.utils import FeatureExtractor
     extractor = []
     try:
         extractor = FeatureExtractor(
             base_model_name = model_name,
             base_model_dir = model_dir,
             model_path = model_path,
-            device = 'cuda'
+            device = device
         )
     except Exception as e:
         msg = "deepreid_extractor() -> " + str(e)
         add_error_log(msg)
         raise ValueError(msg)
     return extractor
```

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/centroid/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/centroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/detection.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/detection.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/generate_detections.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/generate_detections.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/iou_matching.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/iou_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/nn_matching.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/nn_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/preprocessing.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/track.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/deepsort/origin/tracker.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/sort/__init__.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/modules/trackers/sort/origin/sort.py` & `pyppbox-3.1b1/pyppbox/modules/trackers/sort/origin/sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/standalone/__init__.py` & `pyppbox-3.1b1/pyppbox/standalone/mt.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,927 +38,952 @@
 # Classes & tools
 from pyppbox.utils.persontools import Person
 from pyppbox.utils.gttools import GTInterpreter
 from pyppbox.utils.evatools import NothingDetecter, NothingTracker, NothingReider, TKOReider
 from pyppbox.utils.commontools import getAbsPathFDS, isExist, getCVMat, getAncestorDir
 
 
-###########################################
-# Configurator
-###########################################
-
-__cfg__ = MyConfigurator()
-__unistrings__ = __cfg__.unified_strings
-__cfg_is_set__ = False
 __none_cfg__ = NoneCFG()
 __none_cfg__.set("Fiat Moneey")
 
-def __setInternalCFGDir__(load_all):
-    global __cfg__
-    __cfg__.__init__()
-    __cfg__.setMainModules()
-    if load_all:
-        add_info_log("---PYPPBOX : DT='" + 
-                     __cfg__.mcfg.detector + "', TK='" + 
-                     __cfg__.mcfg.tracker + "', RI='" + 
-                     __cfg__.mcfg.reider + "'")
-        __loadDefaultDetector__()
-        __loadDefaultTracker__()
-        __loadDefaultReIDer__()
-
-def setConfigDir(config_dir=None, load_all=False):
-    """Set configurations by a pointing to a config directory :obj:`config_dir`, 
-    where stores 4 required YAML files:
-    (1) main.yaml, tells what main detector/tracker/reider are chosen.
-    (2) detectors.yaml, stores all detectors' configurations.
-    (3) trackers.yaml, stores all trackers' configurations.
-    (4) reiders.yaml, stores all reiders' configurations.
-
-    Note: JSON file (.josn) is also supported.
-
-    Parameters
-    ----------
-    config_dir : str, default=None
-        A path of a config directory.
-        Set :code:`config_dir=None` to use the internal config directory 
-        :code:'{pyppbox root}/config/cfg'.
-    load_all : bool, default=False
-        Set :code:`load_all=True` to set and load the selected detector/tracker/reider 
-        according to the main configurations. 
-        Set :code:`load_all=False` to select and load a detector/tracker/reider manually later.
-    """
-    global __cfg__, __cfg_is_set__, __cfg__
-    __cfg_is_set__ = False
-    if config_dir == None:
-        add_info_log("---PYPPBOX : Now use the internal config directory")
-        __cfg_is_set__ = True
-        __setInternalCFGDir__(load_all=load_all)
-    elif isinstance(config_dir, str):
-        if isExist(config_dir):
-            add_info_log("---PYPPBOX : Now use custom config dir, config_dir='" 
-                  + str(config_dir) + "'")
-            __cfg__.setCustomCFG(cfg_dir=config_dir)
-            __cfg__.setMainModules()
-            __cfg_is_set__ = True
-            if load_all:
-                add_info_log("---PYPPBOX : DT='" + 
-                             __cfg__.mcfg.detector + "', TK='" + 
-                             __cfg__.mcfg.tracker + "', RI='" + 
-                             __cfg__.mcfg.reider + "'")
-                __loadDefaultDetector__()
-                __loadDefaultTracker__()
-                __loadDefaultReIDer__()
-        else:
-            add_warning_log("---PYPPBOX : config_dir='" + str(config_dir) + "' does not exist")
-            add_warning_log("---PYPPBOX : Switched to internal config directory")
-            __cfg_is_set__ = True
-            __setInternalCFGDir__(load_all=load_all)
-    else:
-        msg = "PYPPBOX : setConfigDir() -> config_dir='" + str(config_dir) + "' is not valid."
-        add_error_log(msg)
-        raise ValueError(msg)
-
-def setMainModules(main_yaml=None, load_all=True):
-    """Load and set the main detector, the main tracker, and the main reider all at once 
-    according to the given main configurations, :obj:`main_yaml`. If the :func:`setConfigDir()` 
-    has not yet been called, internal config directory will be used.
-
-    Parameters
-    ----------
-    main_yaml : str or dict, default=None
-        A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary of the 
-        main configurations or main.yaml. This :obj:`main_yaml` helps overwrite the original one 
-        configured earlier. Leave it as default :obj:`main_yaml=None`, to load and set according 
-        to the configurations in the config directory.
-    load_all : bool, default=True
-        Set :code:`load_all=True` to set and load the selected detector/tracker/reider according 
-        to the main configurations, which it is meant for using this :func:`setMainModules()` method.
-        Set :code:`load_all=False` to select and load a detector/tracker/reider manually later.
-    """
-    global __cfg__, __cfg_is_set__
-    if not __cfg_is_set__: setConfigDir()
-    __cfg__.setMainModules(main_yaml=main_yaml)
-    if load_all: 
-        add_info_log("---PYPPBOX : DT='" + 
-                     __cfg__.mcfg.detector + "', TK='" + 
-                     __cfg__.mcfg.tracker + "', RI='" + 
-                     __cfg__.mcfg.reider + "'")
-        __loadDefaultDetector__()
-        __loadDefaultTracker__()
-        __loadDefaultReIDer__()
+class MT(object):
 
-def getConfig():
-    """
-    Get the current :class:`MyConfigurator` object.
+    """An all-in-one class designed for easy detect, track, and reid people in a single threading 
+    or multithreading application.
+
+    Example:
     
-    Returns
-    -------
-    MyConfigurator
-        A :class:`MyConfigurator` object used to store and manage all the configurations of pyppbox.
-    """
-    global __cfg__
-    return __cfg__
+    >>> import cv2
+    >>> import threading
+    >>> from pyppbox.utils.visualizetools import visualizePeople
+    >>> from pyppbox.standalone import MT
+    >>> 
+    >>> def ppb_task(input, main_configs, name="Task"):
+    >>>     ppbmt = MT() # Use `MT` for multithreading
+    >>>     ppbmt.setMainModules(main_yaml=main_configs)
+    >>>     cap = cv2.VideoCapture(input)
+    >>>     while cap.isOpened():
+    >>>         hasFrame, frame = cap.read()
+    >>>         if hasFrame:
+    >>>             detected_people, _ = ppbmt.detectPeople(frame, img_is_mat=True, visual=False)
+    >>>             tracked_people = ppbmt.trackPeople(frame, detected_people, img_is_mat=True)
+    >>>             reidentified_people, reid_count = ppbmt.reidPeople(
+    >>>                 frame,
+    >>>                 tracked_people,
+    >>>                 img_is_mat=True
+    >>>             )
+    >>>             visualized_mat = visualizePeople(
+    >>>                 frame,
+    >>>                 reidentified_people,
+    >>>                 show_reid=reid_count
+    >>>             )
+    >>>             cv2.imshow("Multithreading (" + name + ")", visualized_mat)
+    >>>             if cv2.waitKey(1) & 0xFF == ord('q'):
+    >>>                 break
+    >>>         else:
+    >>>             break
+    >>>     cap.release()
+    >>> 
+    >>> if __name__ == '__main__':
+    >>>     input_one = "data/gta.mp4"
+    >>>     input_two = "data/gta.mp4"
+    >>>     main_configs_one = {'detector': 'YOLO_Classic',
+    >>>                         'tracker': 'SORT',
+    >>>                         'reider': 'Torchreid'}
+    >>>     main_configs_two = {'detector': 'YOLO_Classic',
+    >>>                         'tracker': 'Centroid',
+    >>>                         'reider': 'FaceNet'}
+    >>>     thread_one = threading.Thread(target=ppb_task, args=(input_one, main_configs_one, "Task 1"))
+    >>>     thread_two = threading.Thread(target=ppb_task, args=(input_two, main_configs_two, "Task 2"))
+    >>>     thread_one.start()
+    >>>     thread_two.start()
+    >>>     thread_one.join()
+    >>>     thread_two.join()
+    >>> 
+
+    """
+
+    def __init__(self):
+        # config
+        self.__cfg__ = MyConfigurator()
+        self.__unistrings__ = self.__cfg__.unified_strings
+        self.__cfg_is_set__ = False
+        # detector
+        self.__dt_is_set__ = False
+        self.__dt_cfg__ = []
+        self.__dt__ = []
+        # tracker
+        self.__tk_is_set__ = False
+        self.__tk_cfg__ = []
+        self.__tk__ = []
+        # reider
+        self.__ri_is_set__ = False
+        self.__ri_cfg__ = []
+        self.__ri__ = []
+        self.__deepidlistTMP__ = []
+        self.__faceidlistTMP__ = []
+
+
+    ###########################################
+    # Configurator
+    ###########################################
+
+    def __setInternalCFGDir__(self, load_all):
+        self.__cfg__.__init__()
+        self.__cfg__.setMainModules()
+        if load_all:
+            add_info_log("---PYPPBOX : DT='" + 
+                        self.__cfg__.mcfg.detector + "', TK='" + 
+                        self.__cfg__.mcfg.tracker + "', RI='" + 
+                        self.__cfg__.mcfg.reider + "'")
+            self.__loadDefaultDetector__()
+            self.__loadDefaultTracker__()
+            self.__loadDefaultReIDer__()
+
+    def setConfigDir(self, config_dir=None, load_all=False):
+        """Set configurations by a pointing to a config directory :obj:`config_dir`, 
+        where stores 4 required YAML files:
+        (1) main.yaml, tells what main detector/tracker/reider are chosen.
+        (2) detectors.yaml, stores all detectors' configurations.
+        (3) trackers.yaml, stores all trackers' configurations.
+        (4) reiders.yaml, stores all reiders' configurations.
+
+        Note: JSON file (.josn) is also supported.
+
+        Parameters
+        ----------
+        config_dir : str, default=None
+            A path of a config directory.
+            Set :code:`config_dir=None` to use the internal config directory 
+            :code:'{pyppbox root}/config/cfg'.
+        load_all : bool, default=False
+            Set :code:`load_all=True` to set and load the selected detector/tracker/reider 
+            according to the main configurations. 
+            Set :code:`load_all=False` to select and load a detector/tracker/reider manually later.
+        """
+        self.__cfg_is_set__ = False
+        if config_dir == None:
+            add_info_log("---PYPPBOX : Now use the internal config directory")
+            self.__cfg_is_set__ = True
+            self.__setInternalCFGDir__(load_all=load_all)
+        elif isinstance(config_dir, str):
+            if isExist(config_dir):
+                add_info_log("---PYPPBOX : Now use custom config dir, config_dir='" 
+                             + str(config_dir) + "'")
+                self.__cfg__.setCustomCFG(cfg_dir=config_dir)
+                self.__cfg__.setMainModules()
+                self.__cfg_is_set__ = True
+                if load_all:
+                    add_info_log("---PYPPBOX : DT='" + 
+                                 self.__cfg__.mcfg.detector + "', TK='" + 
+                                 self.__cfg__.mcfg.tracker + "', RI='" + 
+                                 self.__cfg__.mcfg.reider + "'")
+                    self.__loadDefaultDetector__()
+                    self.__loadDefaultTracker__()
+                    self.__loadDefaultReIDer__()
+            else:
+                add_warning_log("---PYPPBOX : config_dir='" + str(config_dir) + "' does not exist")
+                add_warning_log("---PYPPBOX : Switched to internal config directory")
+                self.__cfg_is_set__ = True
+                self.__setInternalCFGDir__(load_all=load_all)
+        else:
+            msg = "PYPPBOX : setConfigDir() -> config_dir='" + str(config_dir) + "' is not valid."
+            add_error_log(msg)
+            raise ValueError(msg)
 
+    def setMainModules(self, main_yaml=None, load_all=True):
+        """Load and set the main detector, the main tracker, and the main reider all at once 
+        according to the given main configurations, :obj:`main_yaml`. If the :func:`setConfigDir()` 
+        has not yet been called, internal config directory will be used.
+
+        Parameters
+        ----------
+        main_yaml : str or dict, default=None
+            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary of the 
+            main configurations or main.yaml. This :obj:`main_yaml` helps overwrite the original one 
+            configured earlier. Leave it as default :obj:`main_yaml=None`, to load and set according 
+            to the configurations in the config directory.
+        load_all : bool, default=True
+            Set :code:`load_all=True` to set and load the selected detector/tracker/reider according 
+            to the main configurations, which it is meant for using this :func:`setMainModules()` method.
+            Set :code:`load_all=False` to select and load a detector/tracker/reider manually later.
+        """
+        if not self.__cfg_is_set__: self.setConfigDir()
+        self.__cfg__.setMainModules(main_yaml=main_yaml)
+        if load_all: 
+            add_info_log("---PYPPBOX : DT='" + 
+                         self.__cfg__.mcfg.detector + "', TK='" + 
+                         self.__cfg__.mcfg.tracker + "', RI='" + 
+                         self.__cfg__.mcfg.reider + "'")
+            self.__loadDefaultDetector__()
+            self.__loadDefaultTracker__()
+            self.__loadDefaultReIDer__()
+
+    def getConfig(self):
+        """
+        Get the current :class:`MyConfigurator` object.
+        
+        Returns
+        -------
+        MyConfigurator
+            A :class:`MyConfigurator` object used to store and manage all the configurations of pyppbox.
+        """
+        return self.__cfg__
+
+
+    ###########################################
+    # Detector
+    ###########################################
+
+    def __setGTDTOnly__(self):
+        if self.__dt_is_set__:
+            if self.__dt_cfg__.dt_name.lower() == self.__unistrings__.gt:
+                if self.__tk_is_set__ or self.__ri_is_set__:
+                    self.__dt__.setDetectOnly(self.__unistrings__.unk_fid, self.__unistrings__.unk_did)
+                    msg = ("\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n"
+                        "---PYPPBOX : For DT='GT', if (TK!='None' or RI!='None')\n"
+                        "---PYPPBOX : -> Set detect_only=True for GT, DETECT ONLY mode.\n"
+                        "!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n")
+                    add_info_log(msg, add_new_line=True)
 
-###########################################
-# Detector
-###########################################
-
-__dt_is_set__ = False
-__dt_cfg__ = []
-__dt__ = []
-
-def __setGTDTOnly__():
-    global __dt_is_set__, __tk_is_set__, __ri_is_set__, __dt__, __dt_cfg__, __unistrings__
-    if __dt_is_set__:
-        if __dt_cfg__.dt_name.lower() == __unistrings__.gt:
-            if __tk_is_set__ or __ri_is_set__:
-                __dt__.setDetectOnly(__unistrings__.unk_fid, __unistrings__.unk_did)
+    def __revokeGTDTOnly__(self):
+        if self.__dt_is_set__:
+            if self.__dt_cfg__.dt_name.lower() == self.__unistrings__.gt:
+                if self.__tk_is_set__ and self.__ri_is_set__:
+                    if (self.__tk_cfg__.tk_name.lower() == self.__unistrings__.none and 
+                        self.__ri_cfg__.ri_name.lower() == self.__unistrings__.none):
+                        self.__dt__.setDetectOnly(self.__unistrings__.unk_fid, self.__unistrings__.unk_did, 
+                                                  detect_only=False)
+                        msg = ("\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n"
+                            "---PYPPBOX : TK='None' & RI='None'\n"
+                            "---PYPPBOX : -> Overwrite detect_only=False for GT, FULL GT mode."
+                            "\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n")
+                        add_info_log(msg, add_new_line=True)
+
+    def forceFullGTMode(self):
+        """Normally when :code:`DT='GT'`, pyppbox can automatically decide the GT mode based on the 
+        name of the tracker and/or the name of reider; however, if the decision is not satisfied 
+        (Should not happen), calling this :func:`forceFUllGTMode()` will overwrite :code:`detect_only=False`.
+        """
+        success = False
+        if self.__dt_is_set__:
+            if self.__dt_cfg__.dt_name.lower() == self.__unistrings__.gt:
+                self.__dt__.setDetectOnly(self.__unistrings__.unk_fid, self.__unistrings__.unk_did, 
+                                          detect_only=False)
+                success = True
                 msg = ("\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n"
-                       "---PYPPBOX : For DT='GT', if (TK!='None' or RI!='None')\n"
-                       "---PYPPBOX : -> Set detect_only=True for GT, DETECT ONLY mode.\n"
-                       "!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n")
+                    "---PYPPBOX : Overwrite detect_only=False for GT, FULL GT mode."
+                    "\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n")
                 add_info_log(msg, add_new_line=True)
 
-def __revokeGTDTOnly__():
-    global __dt_is_set__, __tk_is_set__, __ri_is_set__
-    global __dt__, __tk_cfg__, __ri_cfg__, __dt_cfg__, __unistrings__
-    if __dt_is_set__:
-        if __dt_cfg__.dt_name.lower() == __unistrings__.gt:
-            if __tk_is_set__ and __ri_is_set__:
-                if (__tk_cfg__.tk_name.lower() == __unistrings__.none and 
-                    __ri_cfg__.ri_name.lower() == __unistrings__.none):
-                    __dt__.setDetectOnly(__unistrings__.unk_fid, __unistrings__.unk_did, 
-                                         detect_only=False)
-                    msg = ("\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n"
-                           "---PYPPBOX : TK='None' & RI='None'\n"
-                           "---PYPPBOX : -> Overwrite detect_only=False for GT, FULL GT mode."
-                           "\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n")
-                    add_info_log(msg, add_new_line=True)
-
-def forceFullGTMode():
-    """Normally when :code:`DT='GT'`, pyppbox can automatically decide the GT mode based on the 
-    name of the tracker and/or the name of reider; however, if the decision is not satisfied 
-    (Should not happen), calling this :func:`forceFUllGTMode()` will overwrite :code:`detect_only=False`.
-    """
-    global __dt_is_set__, __dt__, __dt_cfg__, __unistrings__
-    success = False
-    if __dt_is_set__:
-        if __dt_cfg__.dt_name.lower() == __unistrings__.gt:
-            __dt__.setDetectOnly(__unistrings__.unk_fid, __unistrings__.unk_did, 
-                                 detect_only=False)
-            success = True
+        if not success:
             msg = ("\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n"
-                   "---PYPPBOX : Overwrite detect_only=False for GT, FULL GT mode."
-                   "\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n")
-            add_info_log(msg, add_new_line=True)
-
-    if not success:
-        msg = ("\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n"
-               "---PYPPBOX : DT!='GT' -> Failed to overwrite detect_only=False"
-               "\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n")
-        add_warning_log(msg, add_new_line=True)
-        
+                "---PYPPBOX : DT!='GT' -> Failed to overwrite detect_only=False"
+                "\n!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n")
+            add_warning_log(msg, add_new_line=True)
+            
+
+    def __loadDefaultDetector__(self):
+        if self.__cfg_is_set__:
+            if self.__cfg__.mcfg.detector.lower() == self.__unistrings__.yolo_cls:
+                from pyppbox.modules.detectors.yolocls import MyYOLOCLS
+                self.__dt_cfg__ = self.__cfg__.dcfg_yolocs
+                self.__dt__ = MyYOLOCLS(self.__dt_cfg__)
+                self.__dt_is_set__ = True
+            elif self.__cfg__.mcfg.detector.lower() == self.__unistrings__.yolo_ult:
+                from pyppbox.modules.detectors.yoloult import MyYOLOULT
+                self.__dt_cfg__ = self.__cfg__.dcfg_yolout
+                self.__dt__ = MyYOLOULT(self.__dt_cfg__)
+                self.__dt_is_set__ = True
+            elif self.__cfg__.mcfg.detector.lower() == self.__unistrings__.gt:
+                self.__dt_cfg__ = self.__cfg__.dcfg_gt
+                self.__dt__ = GTInterpreter()
+                self.__dt__.setGT(self.__dt_cfg__.gt_file)
+                self.__dt_is_set__ = True
+            elif self.__cfg__.mcfg.detector.lower() == self.__unistrings__.none:
+                self.__dt_cfg__ = __none_cfg__
+                self.__dt__ = NothingDetecter()
+                self.__dt_is_set__ = True
+            else: 
+                add_info_log("---PYPPBOX : The input detecor is not recognized.")
+                self.__dt_is_set__ = False
 
-def __loadDefaultDetector__():
-    global __unistrings__, __cfg__, __cfg_is_set__
-    global __dt__, __dt_cfg__, __dt_is_set__, __none_cfg__
-    if __cfg_is_set__:
-        if __cfg__.mcfg.detector.lower() == __unistrings__.yolo_cls:
-            from pyppbox.modules.detectors.yolocls import MyYOLOCLS
-            __dt_cfg__ = __cfg__.dcfg_yolocs
-            __dt__ = MyYOLOCLS(__dt_cfg__)
-            __dt_is_set__ = True
-        elif __cfg__.mcfg.detector.lower() == __unistrings__.yolo_ult:
-            from pyppbox.modules.detectors.yoloult import MyYOLOULT
-            __dt_cfg__ = __cfg__.dcfg_yolout
-            __dt__ = MyYOLOULT(__dt_cfg__)
-            __dt_is_set__ = True
-        elif __cfg__.mcfg.detector.lower() == __unistrings__.gt:
-            __dt_cfg__ = __cfg__.dcfg_gt
-            __dt__ = GTInterpreter()
-            __dt__.setGT(__dt_cfg__.gt_file)
-            __dt_is_set__ = True
-        elif __cfg__.mcfg.detector.lower() == __unistrings__.none:
-            __dt_cfg__ = __none_cfg__
-            __dt__ = NothingDetecter()
-            __dt_is_set__ = True
-        else: 
-            add_info_log("---PYPPBOX : The input detecor is not recognized.")
-            __dt_is_set__ = False
-
-def __setCustomDetector__(detector_dict):
-    global __unistrings__, __dt__, __dt_cfg__, __dt_is_set__, __none_cfg__
-    if detector_dict:
-        if detector_dict['dt_name'].lower() == __unistrings__.yolo_cls:
-            from pyppbox.modules.detectors.yolocls import MyYOLOCLS
-            __dt_cfg__ = DCFGYOLOCLS()
-            __dt_cfg__.set(detector_dict)
-            __dt__ = MyYOLOCLS(__dt_cfg__)
-            __dt_is_set__ = True
-            add_info_log("---PYPPBOX : Set detector='" + __dt_cfg__.dt_name + "'")
-        elif detector_dict['dt_name'].lower() == __unistrings__.yolo_ult:
-            from pyppbox.modules.detectors.yoloult import MyYOLOULT
-            __dt_cfg__ = DCFGYOLOULT()
-            __dt_cfg__.set(detector_dict)
-            __dt__ = MyYOLOULT(__dt_cfg__)
-            __dt_is_set__ = True
-            add_info_log("---PYPPBOX : Set detector='" + __dt_cfg__.dt_name + "'")
-        elif detector_dict['dt_name'].lower() == __unistrings__.gt:
-            __dt_cfg__ = DCFGGT()
-            __dt_cfg__.set(detector_dict)
-            __dt__ = GTInterpreter()
-            __dt__.setGT(__dt_cfg__.gt_file)
-            __dt_is_set__ = True
-            add_info_log("---PYPPBOX : Set detector='" + __dt_cfg__.dt_name + "'")
-        elif detector_dict['dt_name'].lower() == __unistrings__.none:
-            __dt_cfg__ = __none_cfg__
-            __dt__ = NothingDetecter()
-            __dt_is_set__ = True
-            add_info_log("---PYPPBOX : Set detector='" + __dt_cfg__.dt_name + "'")
-        else: 
-            __dt_is_set__ = False
-            add_warning_log("---PYPPBOX : detector='" + detector_dict['dt_name'] + 
-                            "' is not recognized.")
-
-def setMainDetector(detector=""):
-    """Set the main detector by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
-    dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
-    is optional. Different from the rest, setting the main detector by its name results 
-    in loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
-    If :func:`setConfigDir()` has not been called before, setting the main detector by a supported 
-    name results in referencing the internal config directory in order to load the 
-    corresponding configurations. 
-
-    Parameters
-    ----------
-    detector : str or dict, default=""
-        (1) Set :code:`detector=""` to set the main detector according to the main configurations 
-        or main.yaml and load its configurations from the detectors.yaml. 
-        (2) Set :code:`detector="YOLO_Classic"`.etc, to set YOLO Classic as the main detector and 
-        load its configurations from detectors.yaml.
-        (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
-        :code:`detector="[{'dt_name': 'YOLO_Ultralytics', 'conf': 0.5, 'iou': 0.7, 'imgsz': 416, 
-        'boxes': True, 'device': 0, 'max_det': 100, 'line_width': 500, 
-        'model_file': 'data/modules/yolo_ultralytics/yolov8l-pose.pt', 
-        'repspoint_calibration': 0.25}]"`.
-        (4) Set :code:`detector="a_suported_detector.yaml"` or :code:`detector="a_suported_detector.json"` 
-        to set the main detector and its configuration from a YAML file. 
-    """
-    global __unistrings__, __cfg__, __cfg_is_set__, __dt__
-    global __dt_cfg__, __dt_is_set__, __none_cfg__
-    __dt_is_set__ = False
-    __dt__ = []
-    if isinstance(detector, dict):
-        __setCustomDetector__(detector)
-    elif isinstance(detector, str):
-        if (isRawYAMLString(detector) or "yaml" in detector.lower() or 
-            "json" in detector.lower()):
-            __setCustomDetector__(getCFGDict(detector))
-        elif detector.lower() == "":
-            if not __cfg_is_set__: setConfigDir()
-            __loadDefaultDetector__()
-            add_info_log("---PYPPBOX : Use detector according to the \"main.yaml\"")
-        elif detector.lower() == __unistrings__.yolo_cls:
-            from pyppbox.modules.detectors.yolocls import MyYOLOCLS
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllDCFG()
-            __dt_cfg__ = __cfg__.dcfg_yolocs
-            __dt__ = MyYOLOCLS(__dt_cfg__)
-            __dt_is_set__ = True
-            add_info_log("---PYPPBOX : Set detector='" + str(detector) + "'")
-        elif detector.lower() == __unistrings__.yolo_ult:
-            from pyppbox.modules.detectors.yoloult import MyYOLOULT
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllDCFG()
-            __dt_cfg__ = __cfg__.dcfg_yolout
-            __dt__ = MyYOLOULT(__dt_cfg__)
-            __dt_is_set__ = True
-            add_info_log("---PYPPBOX : Set detector='" + str(detector) + "'")
-        elif detector.lower() == __unistrings__.gt:
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllDCFG()
-            __dt_cfg__ = __cfg__.dcfg_gt
-            __dt__ = GTInterpreter()
-            __dt__.setGT(__dt_cfg__.gt_file)
-            __dt_is_set__ = True
-            add_info_log("---PYPPBOX : Set detector='" + str(detector) + "'")
-        elif detector.lower() == __unistrings__.none:
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllDCFG()
-            __dt_cfg__ = __none_cfg__
-            __dt__ = NothingDetecter()
-            __dt_is_set__ = True
-            add_info_log("---PYPPBOX : Set detector='" + str(detector) + "'")
-    else:
-        add_warning_log("---PYPPBOX : detector='" + str(detector) + "' is not recognized.")
-
-def detectPeople(img, img_is_mat=False, visual=False, save=False, save_file=""): 
-    """Detect people by giving an image. :func:`setConfigDir()` or :func:`setMainDetector()` must 
-    be called in advance.
-
-    Parameters
-    ----------
-    img : str or Mat
-        Set an image file or a cv :obj:`Mat`.
-    img_is_mat : bool, default=False
-        Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
-    visual : bool, default=False
-        Decide whether to visualize like drawing bounding boxes and keypoints to the 
-        return :obj:`img`.
-    save : bool, default=False
-        Decide whether to save the return :obj:`img` to a JPG file.
-    save_file : str, default=""
-        Indicate a path of where to save the processed image.
-    
-    Returns
-    -------
-    list[Person, ...]
-        A  list of :class:`Person` object.
-    Mat
-        A cv :obj:`Mat` image.
-    """ 
-    global __unistrings__, __dt__, __dt_cfg__, __dt_is_set__
-    people = []
-    if __dt_is_set__: 
-        if not isinstance(__dt__, NothingDetecter):
-            if not img_is_mat: img = getCVMat(img)
-            if (__dt_cfg__.dt_name.lower() == __unistrings__.yolo_cls or 
-                __dt_cfg__.dt_name.lower() == __unistrings__.yolo_ult):
-                people, img = __dt__.detectPeople(img, visual=visual)
-            elif __dt_cfg__.dt_name.lower() == __unistrings__.gt:
-                people, img = __dt__.getPeople(img, visual=visual)
-            if save:
-                if isExist(getAncestorDir(str(save_file))):
-                    filename = getAbsPathFDS(str(save_file))
-                    cv2.imwrite(filename=filename, img=img)
-                else:
-                    msg = ("PYPPBOX : detectPeople() -> save_file='" + 
-                           str(save_file) + "' is not valid.")
-                    add_error_log(msg)
-                    raise ValueError(msg)
-    else:
-        add_warning_log("---PYPPBOX : detectPeople() -> The main detector is not set.")
-    return people, img
-
-
-###########################################
-# Tracker
-###########################################
-
-__tk_is_set__ = False
-__tk_cfg__ = []
-__tk__ = []
-
-def __loadDefaultTracker__():
-    global __unistrings__, __cfg__, __cfg_is_set__, __tk__
-    global __tk_cfg__, __tk_is_set__, __none_cfg__
-    if __cfg_is_set__:
-        if __cfg__.mcfg.tracker.lower() == __unistrings__.centroid:
-            from pyppbox.modules.trackers.centroid import MyCentroid
-            __tk_cfg__ = __cfg__.tcfg_centroid
-            __tk__ = MyCentroid(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-        elif __cfg__.mcfg.tracker.lower() == __unistrings__.sort:
-            from pyppbox.modules.trackers.sort import MySORT
-            __tk_cfg__ = __cfg__.tcfg_sort
-            __tk__ = MySORT(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-        elif __cfg__.mcfg.tracker.lower() == __unistrings__.deepsort:
-            from pyppbox.modules.trackers.deepsort import MyDeepSORT
-            __tk_cfg__ = __cfg__.tcfg_deepsort
-            __tk__ = MyDeepSORT(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-        elif __cfg__.mcfg.tracker.lower() == __unistrings__.none:
-            __tk_cfg__ = __none_cfg__
-            __tk__ = NothingTracker()
-            __tk_is_set__ = True
-        else: 
-            add_warning_log("---PYPPBOX : The input tracker is not recognized.")
-            __tk_is_set__ = False
-
-def __setCustomTracker__(tracker_dict):
-    global __unistrings__, __tk__, __tk_cfg__, __tk_is_set__, __none_cfg__
-    if tracker_dict:
-        if tracker_dict['tk_name'].lower() == __unistrings__.centroid:
-            from pyppbox.modules.trackers.centroid import MyCentroid
-            __tk_cfg__ = TCFGCentroid()
-            __tk_cfg__.set(tracker_dict)
-            __tk__ = MyCentroid(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-            add_info_log("---PYPPBOX : Set tracker='" + __tk_cfg__.tk_name + "'")
-        elif tracker_dict['tk_name'].lower() == __unistrings__.sort:
-            from pyppbox.modules.trackers.sort import MySORT
-            __tk_cfg__ = TCFGSORT()
-            __tk_cfg__.set(tracker_dict)
-            __tk__ = MySORT(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-            add_info_log("---PYPPBOX : Set tracker='" + __tk_cfg__.tk_name + "'")
-        elif tracker_dict['tk_name'].lower() == __unistrings__.deepsort:
-            from pyppbox.modules.trackers.deepsort import MyDeepSORT
-            __tk_cfg__ = TCFGDeepSORT()
-            __tk_cfg__.set(tracker_dict)
-            __tk__ = MyDeepSORT(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-            add_info_log("---PYPPBOX : Set tracker='" + __tk_cfg__.tk_name + "'")
-        elif tracker_dict['tk_name'].lower() == __unistrings__.none:
-            __tk_cfg__ = __none_cfg__
-            __tk__ = NothingTracker()
-            __tk_is_set__ = True
-            add_info_log("---PYPPBOX : Set tracker='" + __tk_cfg__.tk_name + "'")
+    def __setCustomDetector__(self, detector_dict):
+        if detector_dict:
+            if detector_dict['dt_name'].lower() == self.__unistrings__.yolo_cls:
+                from pyppbox.modules.detectors.yolocls import MyYOLOCLS
+                self.__dt_cfg__ = DCFGYOLOCLS()
+                self.__dt_cfg__.set(detector_dict)
+                self.__dt__ = MyYOLOCLS(self.__dt_cfg__)
+                self.__dt_is_set__ = True
+                add_info_log("---PYPPBOX : Set detector='" + self.__dt_cfg__.dt_name + "'")
+            elif detector_dict['dt_name'].lower() == self.__unistrings__.yolo_ult:
+                from pyppbox.modules.detectors.yoloult import MyYOLOULT
+                self.__dt_cfg__ = DCFGYOLOULT()
+                self.__dt_cfg__.set(detector_dict)
+                self.__dt__ = MyYOLOULT(self.__dt_cfg__)
+                self.__dt_is_set__ = True
+                add_info_log("---PYPPBOX : Set detector='" + self.__dt_cfg__.dt_name + "'")
+            elif detector_dict['dt_name'].lower() == self.__unistrings__.gt:
+                self.__dt_cfg__ = DCFGGT()
+                self.__dt_cfg__.set(detector_dict)
+                self.__dt__ = GTInterpreter()
+                self.__dt__.setGT(self.__dt_cfg__.gt_file)
+                self.__dt_is_set__ = True
+                add_info_log("---PYPPBOX : Set detector='" + self.__dt_cfg__.dt_name + "'")
+            elif detector_dict['dt_name'].lower() == self.__unistrings__.none:
+                self.__dt_cfg__ = __none_cfg__
+                self.__dt__ = NothingDetecter()
+                self.__dt_is_set__ = True
+                add_info_log("---PYPPBOX : Set detector='" + self.__dt_cfg__.dt_name + "'")
+            else: 
+                self.__dt_is_set__ = False
+                add_warning_log("---PYPPBOX : detector='" + detector_dict['dt_name'] + 
+                                "' is not recognized.")
+
+    def setMainDetector(self, detector=""):
+        """Set the main detector by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
+        dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
+        is optional. Different from the rest, setting the main detector by its name results 
+        in loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
+        If :func:`setConfigDir()` has not been called before, setting the main detector by a supported 
+        name results in referencing the internal config directory in order to load the 
+        corresponding configurations. 
+
+        Parameters
+        ----------
+        detector : str or dict, default=""
+            (1) Set :code:`detector=""` to set the main detector according to the main configurations 
+            or main.yaml and load its configurations from the detectors.yaml. 
+            (2) Set :code:`detector="YOLO_Classic"`.etc, to set YOLO Classic as the main detector and 
+            load its configurations from detectors.yaml.
+            (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
+            :code:`detector="[{'dt_name': 'YOLO_Ultralytics', 'conf': 0.5, 'iou': 0.7, 'imgsz': 416, 
+            'boxes': True, 'device': 0, 'max_det': 100, 'line_width': 500, 
+            'model_file': 'data/modules/yolo_ultralytics/yolov8l-pose.pt', 
+            'repspoint_calibration': 0.25}]"`.
+            (4) Set :code:`detector="a_supported_detector.yaml"` or :code:`detector="a_supported_detector.json"` 
+            to set the main detector and its configuration from a YAML file. 
+        """
+        self.__dt_is_set__ = False
+        self.__dt__ = []
+        if isinstance(detector, dict):
+            self.__setCustomDetector__(detector)
+        elif isinstance(detector, str):
+            if (isRawYAMLString(detector) or "yaml" in detector.lower() or 
+                "json" in detector.lower()):
+                self.__setCustomDetector__(getCFGDict(detector))
+            elif detector.lower() == "":
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__loadDefaultDetector__()
+                add_info_log("---PYPPBOX : Use detector according to the \"main.yaml\"")
+            elif detector.lower() == self.__unistrings__.yolo_cls:
+                from pyppbox.modules.detectors.yolocls import MyYOLOCLS
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllDCFG()
+                self.__dt_cfg__ = self.__cfg__.dcfg_yolocs
+                self.__dt__ = MyYOLOCLS(self.__dt_cfg__)
+                self.__dt_is_set__ = True
+                add_info_log("---PYPPBOX : Set detector='" + str(detector) + "'")
+            elif detector.lower() == self.__unistrings__.yolo_ult:
+                from pyppbox.modules.detectors.yoloult import MyYOLOULT
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllDCFG()
+                self.__dt_cfg__ = self.__cfg__.dcfg_yolout
+                self.__dt__ = MyYOLOULT(self.__dt_cfg__)
+                self.__dt_is_set__ = True
+                add_info_log("---PYPPBOX : Set detector='" + str(detector) + "'")
+            elif detector.lower() == self.__unistrings__.gt:
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllDCFG()
+                self.__dt_cfg__ = self.__cfg__.dcfg_gt
+                self.__dt__ = GTInterpreter()
+                self.__dt__.setGT(self.__dt_cfg__.gt_file)
+                self.__dt_is_set__ = True
+                add_info_log("---PYPPBOX : Set detector='" + str(detector) + "'")
+            elif detector.lower() == self.__unistrings__.none:
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllDCFG()
+                self.__dt_cfg__ = __none_cfg__
+                self.__dt__ = NothingDetecter()
+                self.__dt_is_set__ = True
+                add_info_log("---PYPPBOX : Set detector='" + str(detector) + "'")
         else:
-            __tk_is_set__ = False
-            add_warning_log("---PYPPBOX : tracker='" + tracker_dict['tk_name'] + 
-                  "' is not recognized")
-
-def setMainTracker(tracker=""):
-    """Set the main tracker by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
-    dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
-    is optional. Different from the rest, setting the main tracker by its name results 
-    in loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
-    If :func:`setConfigDir()` has not been called before, setting the main tracker by a supported 
-    name results in referencing the internal config directory in order to load the 
-    corresponding configurations. 
-
-    Parameters
-    ----------
-    tracker : str or dict, default=""
-        (1) Set :code:`tracker=""` to set the main tracker according to the main configurations or 
-        main.yaml and load its configurations from the trackers.yaml. 
-        (2) Set :code:`tracker="Centroid"`.etc, to set Centroid as the main tracker and load its 
-        configurations from trackers.yaml.
-        (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
-        :code:`tracker="[{'tk_name': 'SORT', 'max_age': 1, 'min_hits': 3, 'iou_threshold': 0.3}]"`.
-        (4) Set :code:`tracker="a_suported_tracker.yaml"` or :code:`tracker="a_suported_tracker.json"` 
-        to set the main tracker and its configuration from a YAML file. 
-    """
-    global __unistrings__, __cfg__, __cfg_is_set__, __tk__
-    global __tk_cfg__, __tk_is_set__, __none_cfg__
-    __tk_is_set__ = False
-    __tk__ = []
-    if isinstance(tracker, dict):
-        __setCustomTracker__(tracker)
-    elif isinstance(tracker, str):
-        if (isRawYAMLString(tracker) or "yaml" in tracker.lower() or 
-            "json" in tracker.lower()):
-            __setCustomTracker__(getCFGDict(tracker))
-        elif tracker.lower() == "default":
-            if not __cfg_is_set__: setConfigDir()
-            __loadDefaultTracker__()
-            add_info_log("---PYPPBOX : Use tracker according to the \"main.yaml\"")
-        elif tracker.lower() == __unistrings__.centroid:
-            from pyppbox.modules.trackers.centroid import MyCentroid
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllTCFG()
-            __tk_cfg__ = __cfg__.tcfg_centroid
-            __tk__ = MyCentroid(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-            add_info_log("---PYPPBOX : Set tracker='" + str(tracker) + "'")
-        elif tracker.lower() == __unistrings__.sort:
-            from pyppbox.modules.trackers.sort import MySORT
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllTCFG()
-            __tk_cfg__ = __cfg__.tcfg_sort
-            __tk__ = MySORT(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-            add_info_log("---PYPPBOX : Set tracker='" + str(tracker) + "'")
-        elif tracker.lower() == __unistrings__.deepsort:
-            from pyppbox.modules.trackers.deepsort import MyDeepSORT
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllTCFG()
-            __tk_cfg__ = __cfg__.tcfg_deepsort
-            __tk__ = MyDeepSORT(__tk_cfg__)
-            __tk_is_set__ = True
-            __setGTDTOnly__()
-            add_info_log("---PYPPBOX : Set tracker='" + str(tracker) + "'")
-        elif tracker.lower() == __unistrings__.none:
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllTCFG()
-            __tk_cfg__ = __none_cfg__
-            __tk__ = NothingTracker()
-            __tk_is_set__ = True
-            add_info_log("---PYPPBOX : Set tracker='" + str(tracker) + "'")
-    else:
-        add_warning_log("---PYPPBOX : tracker='" + str(tracker) + "' is not valid")
-
-def trackPeople(img, people, img_is_mat=False):
-    """Track people by giving an image and a list of detected people. :func:`setConfigDir()` 
-    or :func:`setMainTracker()` must be called in advance.
-
-    Parameters
-    ----------
-    img : str or Mat
-        Set an image file or a cv :obj:`Mat`.
-    people : list[Person, ...]
-        Set a list of :class:`Person` object which stores the detected people in the input :obj:`img`.
-    img_is_mat : bool, default=False
-        Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
-    
-    Returns
-    -------
-    list[Person, ...]
-        A list of :class:`Person` object which stores people with updated IDs.
-    """
-    global __tk__, __tk_cfg__, __tk_is_set__
-    res = []
-    if __tk_is_set__: 
-        if isinstance(people, list):
-            if not img_is_mat: img = getCVMat(img)
-            res = __tk__.update(people, img=img)
+            add_warning_log("---PYPPBOX : detector='" + str(detector) + "' is not recognized.")
+
+    def detectPeople(self, img, img_is_mat=False, visual=False, save=False, save_file=""): 
+        """Detect people by giving an image. :func:`setConfigDir()` or :func:`setMainDetector()` must 
+        be called in advance.
+
+        Parameters
+        ----------
+        img : str or Mat
+            Set an image file or a cv :obj:`Mat`.
+        img_is_mat : bool, default=False
+            Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
+        visual : bool, default=False
+            Decide whether to visualize like drawing bounding boxes and keypoints to the 
+            return :obj:`img`.
+        save : bool, default=False
+            Decide whether to save the return :obj:`img` to a JPG file.
+        save_file : str, default=""
+            Indicate a path of where to save the processed image.
+        
+        Returns
+        -------
+        list[Person, ...]
+            A  list of :class:`Person` object.
+        Mat
+            A cv :obj:`Mat` image.
+        """ 
+        people = []
+        if self.__dt_is_set__: 
+            if not isinstance(self.__dt__, NothingDetecter):
+                if not img_is_mat: img = getCVMat(img)
+                if (self.__dt_cfg__.dt_name.lower() == self.__unistrings__.yolo_cls or 
+                    self.__dt_cfg__.dt_name.lower() == self.__unistrings__.yolo_ult):
+                    people, img = self.__dt__.detectPeople(img, visual=visual)
+                elif self.__dt_cfg__.dt_name.lower() == self.__unistrings__.gt:
+                    people, img = self.__dt__.getPeople(img, visual=visual)
+                if save:
+                    if isExist(getAncestorDir(str(save_file))):
+                        filename = getAbsPathFDS(str(save_file))
+                        cv2.imwrite(filename=filename, img=img)
+                    else:
+                        msg = ("PYPPBOX : detectPeople() -> save_file='" + 
+                               str(save_file) + "' is not valid.")
+                        add_error_log(msg)
+                        raise ValueError(msg)
         else:
-            msg = "PYPPBOX : trackPeople() -> Input 'people' is not correct."
-            add_error_log(msg)
-            raise ValueError(msg)
-    else:
-        add_warning_log("---PYPPBOX : trackPeople() -> The main tracker is not set.")
-    return res
-
-
-###########################################
-# REIDer
-###########################################
-
-__ri_is_set__ = False
-__ri_cfg__ = []
-__ri__ = []
-__deepidlistTMP__ = []
-__faceidlistTMP__ = []
-
-def __loadDefaultReIDer__(auto_load=True):
-    global __unistrings__, __cfg__, __cfg_is_set__, __ri__, __ri_cfg__
-    global __ri_is_set__, __none_cfg__, __dt_cfg__, __tk_cfg__
-    if __cfg_is_set__:
-        if __cfg__.mcfg.reider.lower() == __unistrings__.facenet:
-            from pyppbox.modules.reiders.facenet import MyFaceNet
-            __ri_cfg__ = __cfg__.rcfg_facenet
-            __ri__ = MyFaceNet(__ri_cfg__, auto_load=auto_load)
-            __ri_is_set__ = True
-            __setGTDTOnly__()
-        elif __cfg__.mcfg.reider.lower() == __unistrings__.torchreid:
-            from pyppbox.modules.reiders.torchreid import MyTorchreid
-            __ri_cfg__ = __cfg__.rcfg_torchreid
-            __ri__ = MyTorchreid(__ri_cfg__, auto_load=auto_load)
-            __ri_is_set__ = True
-            __setGTDTOnly__()
-        elif __cfg__.mcfg.reider.lower() == __unistrings__.none:
-            if (__dt_cfg__.dt_name.lower() != __unistrings__.none and 
-                __tk_cfg__.tk_name.lower() != __unistrings__.none):
-                __ri__ = TKOReider(static=True)
+            add_warning_log("---PYPPBOX : detectPeople() -> The main detector is not set.")
+        return people, img
+
+
+    ###########################################
+    # Tracker
+    ###########################################
+
+    def __loadDefaultTracker__(self):
+        if self.__cfg_is_set__:
+            if self.__cfg__.mcfg.tracker.lower() == self.__unistrings__.centroid:
+                from pyppbox.modules.trackers.centroid import MyCentroid
+                self.__tk_cfg__ = self.__cfg__.tcfg_centroid
+                self.__tk__ = MyCentroid(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+            elif self.__cfg__.mcfg.tracker.lower() == self.__unistrings__.sort:
+                from pyppbox.modules.trackers.sort import MySORT
+                self.__tk_cfg__ = self.__cfg__.tcfg_sort
+                self.__tk__ = MySORT(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+            elif self.__cfg__.mcfg.tracker.lower() == self.__unistrings__.deepsort:
+                from pyppbox.modules.trackers.deepsort import MyDeepSORT
+                self.__tk_cfg__ = self.__cfg__.tcfg_deepsort
+                self.__tk__ = MyDeepSORT(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+            elif self.__cfg__.mcfg.tracker.lower() == self.__unistrings__.none:
+                self.__tk_cfg__ = __none_cfg__
+                self.__tk__ = NothingTracker()
+                self.__tk_is_set__ = True
+            else: 
+                add_warning_log("---PYPPBOX : The input tracker is not recognized.")
+                self.__tk_is_set__ = False
+
+    def __setCustomTracker__(self, tracker_dict):
+        if tracker_dict:
+            if tracker_dict['tk_name'].lower() == self.__unistrings__.centroid:
+                from pyppbox.modules.trackers.centroid import MyCentroid
+                self.__tk_cfg__ = TCFGCentroid()
+                self.__tk_cfg__.set(tracker_dict)
+                self.__tk__ = MyCentroid(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+                add_info_log("---PYPPBOX : Set tracker='" + self.__tk_cfg__.tk_name + "'")
+            elif tracker_dict['tk_name'].lower() == self.__unistrings__.sort:
+                from pyppbox.modules.trackers.sort import MySORT
+                self.__tk_cfg__ = TCFGSORT()
+                self.__tk_cfg__.set(tracker_dict)
+                self.__tk__ = MySORT(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+                add_info_log("---PYPPBOX : Set tracker='" + self.__tk_cfg__.tk_name + "'")
+            elif tracker_dict['tk_name'].lower() == self.__unistrings__.deepsort:
+                from pyppbox.modules.trackers.deepsort import MyDeepSORT
+                self.__tk_cfg__ = TCFGDeepSORT()
+                self.__tk_cfg__.set(tracker_dict)
+                self.__tk__ = MyDeepSORT(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+                add_info_log("---PYPPBOX : Set tracker='" + self.__tk_cfg__.tk_name + "'")
+            elif tracker_dict['tk_name'].lower() == self.__unistrings__.none:
+                self.__tk_cfg__ = __none_cfg__
+                self.__tk__ = NothingTracker()
+                self.__tk_is_set__ = True
+                add_info_log("---PYPPBOX : Set tracker='" + self.__tk_cfg__.tk_name + "'")
             else:
-                __ri__ = NothingReider()
-            __ri_cfg__ = __none_cfg__
-            __ri_is_set__ = True
-            __revokeGTDTOnly__()
+                self.__tk_is_set__ = False
+                add_warning_log("---PYPPBOX : tracker='" + tracker_dict['tk_name'] + 
+                                "' is not recognized")
+
+    def setMainTracker(self, tracker=""):
+        """Set the main tracker by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
+        dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
+        is optional. Different from the rest, setting the main tracker by its name results 
+        in loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
+        If :func:`setConfigDir()` has not been called before, setting the main tracker by a supported 
+        name results in referencing the internal config directory in order to load the 
+        corresponding configurations. 
+
+        Parameters
+        ----------
+        tracker : str or dict, default=""
+            (1) Set :code:`tracker=""` to set the main tracker according to the main configurations or 
+            main.yaml and load its configurations from the trackers.yaml. 
+            (2) Set :code:`tracker="Centroid"`.etc, to set Centroid as the main tracker and load its 
+            configurations from trackers.yaml.
+            (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
+            :code:`tracker="[{'tk_name': 'SORT', 'max_age': 1, 'min_hits': 3, 'iou_threshold': 0.3}]"`.
+            (4) Set :code:`tracker="a_supported_tracker.yaml"` or :code:`tracker="a_supported_tracker.json"` 
+            to set the main tracker and its configuration from a YAML file. 
+        """
+        self.__tk_is_set__ = False
+        self.__tk__ = []
+        if isinstance(tracker, dict):
+            self.__setCustomTracker__(tracker)
+        elif isinstance(tracker, str):
+            if (isRawYAMLString(tracker) or "yaml" in tracker.lower() or 
+                "json" in tracker.lower()):
+                self.__setCustomTracker__(getCFGDict(tracker))
+            elif tracker.lower() == "default":
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__loadDefaultTracker__()
+                add_info_log("---PYPPBOX : Use tracker according to the \"main.yaml\"")
+            elif tracker.lower() == self.__unistrings__.centroid:
+                from pyppbox.modules.trackers.centroid import MyCentroid
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllTCFG()
+                self.__tk_cfg__ = self.__cfg__.tcfg_centroid
+                self.__tk__ = MyCentroid(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+                add_info_log("---PYPPBOX : Set tracker='" + str(tracker) + "'")
+            elif tracker.lower() == self.__unistrings__.sort:
+                from pyppbox.modules.trackers.sort import MySORT
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllTCFG()
+                self.__tk_cfg__ = self.__cfg__.tcfg_sort
+                self.__tk__ = MySORT(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+                add_info_log("---PYPPBOX : Set tracker='" + str(tracker) + "'")
+            elif tracker.lower() == self.__unistrings__.deepsort:
+                from pyppbox.modules.trackers.deepsort import MyDeepSORT
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllTCFG()
+                self.__tk_cfg__ = self.__cfg__.tcfg_deepsort
+                self.__tk__ = MyDeepSORT(self.__tk_cfg__)
+                self.__tk_is_set__ = True
+                self.__setGTDTOnly__()
+                add_info_log("---PYPPBOX : Set tracker='" + str(tracker) + "'")
+            elif tracker.lower() == self.__unistrings__.none:
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllTCFG()
+                self.__tk_cfg__ = __none_cfg__
+                self.__tk__ = NothingTracker()
+                self.__tk_is_set__ = True
+                add_info_log("---PYPPBOX : Set tracker='" + str(tracker) + "'")
         else:
-            add_warning_log("---PYPPBOX : The input reider is not recognized.")
-            __ri_is_set__ = False
+            add_warning_log("---PYPPBOX : tracker='" + str(tracker) + "' is not valid")
 
-def __setCustomReIDer__(reider_dict, auto_load=True):
-    global __unistrings__, __cfg__, __ri__, __ri_cfg__, __ri_is_set__
-    global __none_cfg__, __dt_cfg__, __tk_cfg__
-    if reider_dict:
-        if reider_dict['ri_name'].lower() == __unistrings__.facenet:
-            from pyppbox.modules.reiders.facenet import MyFaceNet
-            __ri_cfg__ = RCFGFaceNet()
-            __ri_cfg__.set(reider_dict)
-            __ri__ = MyFaceNet(__ri_cfg__, auto_load=auto_load)
-            __ri_is_set__ = True
-            add_info_log("---PYPPBOX : Set reider='" + __ri_cfg__.ri_name + "'")
-            __setGTDTOnly__()
-        elif reider_dict['ri_name'].lower() == __unistrings__.torchreid:
-            from pyppbox.modules.reiders.torchreid import MyTorchreid
-            __ri_cfg__ = RCFGTorchreid()
-            __ri_cfg__.set(reider_dict)
-            __ri__ = MyTorchreid(__ri_cfg__, auto_load=auto_load)
-            __ri_is_set__ = True
-            add_info_log("---PYPPBOX : Set reider='" + __ri_cfg__.ri_name + "'")
-            __setGTDTOnly__()
-        elif reider_dict['ri_name'].lower() == __unistrings__.none:
-            if (__dt_cfg__.dt_name.lower() != __unistrings__.none and 
-                __tk_cfg__.tk_name.lower() != __unistrings__.none):
-                __ri__ = TKOReider(static=True)
+    def trackPeople(self, img, people, img_is_mat=False):
+        """Track people by giving an image and a list of detected people. :func:`setConfigDir()` 
+        or :func:`setMainTracker()` must be called in advance.
+
+        Parameters
+        ----------
+        img : str or Mat
+            Set an image file or a cv :obj:`Mat`.
+        people : list[Person, ...]
+            Set a list of :class:`Person` object which stores the detected people in the input :obj:`img`.
+        img_is_mat : bool, default=False
+            Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
+        
+        Returns
+        -------
+        list[Person, ...]
+            A list of :class:`Person` object which stores people with updated IDs.
+        """
+        res = []
+        if self.__tk_is_set__: 
+            if isinstance(people, list):
+                if not img_is_mat: img = getCVMat(img)
+                res = self.__tk__.update(people, img=img)
             else:
-                __ri__ = NothingReider()
-            __ri_cfg__ = __none_cfg__
-            __ri_is_set__ = True
-            add_info_log("---PYPPBOX : Set reider='" + __ri_cfg__.ri_name + "'")
-            __revokeGTDTOnly__()
-        else :
-            __ri_is_set__ = False
-            add_warning_log("---PYPPBOX : reider='" + reider_dict['ri_name'] + 
-                  "' is not recognized")
-
-def setMainReIDer(reider="", auto_load=True):
-    """Set the main reider by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
-    dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
-    is optional. Different from the rest, setting the main reider by its name results in 
-    loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
-    If :func:`setConfigDir()` has not been called before, setting the main reider by a supported 
-    name results in referencing the internal config directory in order to load the 
-    corresponding configurations. 
-
-    Parameters
-    ----------
-    reider : str or dict, default=""
-        (1) Set :code:`reider=""` to set the main reider according to the main configurations 
-        or main.yaml and load its configurations from the reiders.yaml. 
-        (2) Set :code:`reider="FaceNet"`.etc, to set FaceNet as a reider and load its 
-        configurations from reiders.yaml.
-        (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
-        :code:`reider="[{'ri_name': 'Torchreid', 
-        'classifier_pkl': 'data/modules/torchreid/classifier/gta5_osnet_ain_ms_d_c.pkl', 
-        'train_data': 'data/datasets/GTA_V_DATASET/body_128x256', 'model_name': 'osnet_ain_x1_0', 
-        'model_path': 'data/modules/torchreid/models/torchreid/osnet_ain_ms_d_c.pth.tar', 
-        'min_confidence': 0.35}]"`.
-        (4) Set :code:`reider="a_suported_reider.yaml"` or :code:`reider="a_suported_reider.json"` 
-        to set a the main reider and its configurations from a YAML file. 
-    auto_load : bool, default=True
-        All supported reiders are Pytorch or Tensorflow based module, thus they need to 
-        initial and load their models/weights. :obj:`auto_load` is used to decide whether to 
-        load the reider automatically once the reider is set. Keep the :code:`auto_load=True` 
-        if it is meant for using :func:`reidPeople()`; however, even if the :code:`auto_load=False`, 
-        the :func:`reidPeople()` will initial and load the reider by itself, but it requires 
-        some time to do so.
-    """
-    global __unistrings__, __cfg__, __cfg_is_set__, __ri__
-    global __ri_cfg__, __ri_is_set__, __none_cfg__
-    __ri_is_set__ = False
-    __ri__ = []
-    if isinstance(reider, dict):
-        __setCustomReIDer__(reider, auto_load)
-    elif isinstance(reider, str):
-        if (isRawYAMLString(reider) or "yaml" in reider.lower() or 
-            "json" in reider.lower()):
-            __setCustomReIDer__(getCFGDict(reider), auto_load)
-        elif reider.lower() == "default":
-            if not __cfg_is_set__: setConfigDir()
-            __loadDefaultReIDer__(auto_load=auto_load)
-            add_info_log("---PYPPBOX : Use reider according to the \"main.yaml\"")
-        elif reider.lower() == __unistrings__.facenet:
-            from pyppbox.modules.reiders.facenet import MyFaceNet
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllRCFG()
-            __ri_cfg__ = __cfg__.rcfg_facenet
-            __ri__ = MyFaceNet(__ri_cfg__, auto_load=auto_load)
-            __ri_is_set__ = True
-            add_info_log("---PYPPBOX : Set reider='" + str(reider) + "'")
-            __setGTDTOnly__()
-        elif reider.lower() == __unistrings__.torchreid:
-            from pyppbox.modules.reiders.torchreid import MyTorchreid
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllRCFG()
-            __ri_cfg__ = __cfg__.rcfg_torchreid
-            __ri__ = MyTorchreid(__ri_cfg__, auto_load=auto_load)
-            __ri_is_set__ = True
-            add_info_log("---PYPPBOX : Set reider='" + str(reider) + "'")
-            __setGTDTOnly__()
-        elif reider.lower() == __unistrings__.none:
-            if not __cfg_is_set__: setConfigDir()
-            __cfg__.setAllRCFG()
-            if (__dt_cfg__.dt_name.lower() != __unistrings__.none and 
-                __tk_cfg__.tk_name.lower() != __unistrings__.none):
-                __ri__ = TKOReider(static=True)
+                msg = "PYPPBOX : trackPeople() -> Input 'people' is not correct."
+                add_error_log(msg)
+                raise ValueError(msg)
+        else:
+            add_warning_log("---PYPPBOX : trackPeople() -> The main tracker is not set.")
+        return res
+
+
+    ###########################################
+    # REIDer
+    ###########################################
+
+    def __loadDefaultReIDer__(self, auto_load=True):
+        if self.__cfg_is_set__:
+            if self.__cfg__.mcfg.reider.lower() == self.__unistrings__.facenet:
+                from pyppbox.modules.reiders.facenet import MyFaceNet
+                self.__ri_cfg__ = self.__cfg__.rcfg_facenet
+                self.__ri__ = MyFaceNet(self.__ri_cfg__, auto_load=auto_load)
+                self.__ri_is_set__ = True
+                self.__setGTDTOnly__()
+            elif self.__cfg__.mcfg.reider.lower() == self.__unistrings__.torchreid:
+                from pyppbox.modules.reiders.torchreid import MyTorchreid
+                self.__ri_cfg__ = self.__cfg__.rcfg_torchreid
+                self.__ri__ = MyTorchreid(self.__ri_cfg__, auto_load=auto_load)
+                self.__ri_is_set__ = True
+                self.__setGTDTOnly__()
+            elif self.__cfg__.mcfg.reider.lower() == self.__unistrings__.none:
+                if (self.__dt_cfg__.dt_name.lower() != self.__unistrings__.none and 
+                    self.__tk_cfg__.tk_name.lower() != self.__unistrings__.none):
+                    self.__ri__ = TKOReider(static=True)
+                else:
+                    self.__ri__ = NothingReider()
+                self.__ri_cfg__ = __none_cfg__
+                self.__ri_is_set__ = True
+                self.__revokeGTDTOnly__()
             else:
-                __ri__ = NothingReider()
-            __ri_cfg__ = __none_cfg__
-            __ri_is_set__ = True
-            add_info_log("---PYPPBOX : Set reider='" + str(reider) + "'")
-            __revokeGTDTOnly__()
-    else:
-        add_warning_log("---PYPPBOX : reider='" + str(reider) + "' is not valid")
-
-def reidPeople(img, people, deduplicate=True, img_is_mat=False):
-    """Re-identify people by giving an image and a list of detected or tracked people. 
-    :func:`setConfigDir()` or :func:`setMainReIDer()` must be called in advance.
-
-    Parameters
-    ----------
-    img : str or Mat
-        Set an image file or a cv :obj:`Mat`.
-    people : list[Person, ...]
-        Set a list of :class:`Person` object which stores the detected or tracked people in 
-        the input :obj:`img`.
-    deduplicate : bool, default=True
-        Indicate whether to re-reid people who have the same face ids or deep ids.
-    img_is_mat : bool, default=False
-        Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
-    
-    Returns
-    -------
-    list[Person, ...]
-        A list of :class:`Person` object which stores people with the updated IDs.
-    tuple(int, int)
-        A tuple of (ReID count, ReID deduplicate count).
-    """
-    global __ri__, __ri_cfg__, __ri_is_set__, __unistrings__
-    res = []
-    reid_count = [0, 0]
-    if __ri_is_set__:
-        # if not isinstance(__ri__, TKOReider) and not isinstance(__ri__, NothingReider):
-        if __ri_cfg__.ri_name.lower() != __unistrings__.none:
-            if not __ri__.auto_load:
-                __ri__.load_classifier()
-                __ri__.auto_load = True
-        if isinstance(people, list):
-            if len(people) > 0:
-                if isinstance(people[0], Person):
-                    if not img_is_mat: img = getCVMat(img)
-                    res, reid_count[0] = __reidNormal__(img, people)
-                    if deduplicate: res, reid_count[1] = __reidDupkiller__(img, res)
+                add_warning_log("---PYPPBOX : The input reider is not recognized.")
+                self.__ri_is_set__ = False
+
+    def __setCustomReIDer__(self, reider_dict, auto_load=True):
+        if reider_dict:
+            if reider_dict['ri_name'].lower() == self.__unistrings__.facenet:
+                from pyppbox.modules.reiders.facenet import MyFaceNet
+                self.__ri_cfg__ = RCFGFaceNet()
+                self.__ri_cfg__.set(reider_dict)
+                self.__ri__ = MyFaceNet(self.__ri_cfg__, auto_load=auto_load)
+                self.__ri_is_set__ = True
+                add_info_log("---PYPPBOX : Set reider='" + self.__ri_cfg__.ri_name + "'")
+                self.__setGTDTOnly__()
+            elif reider_dict['ri_name'].lower() == self.__unistrings__.torchreid:
+                from pyppbox.modules.reiders.torchreid import MyTorchreid
+                self.__ri_cfg__ = RCFGTorchreid()
+                self.__ri_cfg__.set(reider_dict)
+                self.__ri__ = MyTorchreid(self.__ri_cfg__, auto_load=auto_load)
+                self.__ri_is_set__ = True
+                add_info_log("---PYPPBOX : Set reider='" + self.__ri_cfg__.ri_name + "'")
+                self.__setGTDTOnly__()
+            elif reider_dict['ri_name'].lower() == self.__unistrings__.none:
+                if (self.__dt_cfg__.dt_name.lower() != self.__unistrings__.none and 
+                    self.__tk_cfg__.tk_name.lower() != self.__unistrings__.none):
+                    self.__ri__ = TKOReider(static=True)
                 else:
-                    msg = "PYPPBOX : reidPeople() -> Input 'people' has unsupported element."
-                    add_error_log(msg)
-                    raise ValueError(msg)
+                    self.__ri__ = NothingReider()
+                self.__ri_cfg__ = __none_cfg__
+                self.__ri_is_set__ = True
+                add_info_log("---PYPPBOX : Set reider='" + self.__ri_cfg__.ri_name + "'")
+                self.__revokeGTDTOnly__()
+            else :
+                self.__ri_is_set__ = False
+                add_warning_log("---PYPPBOX : reider='" + reider_dict['ri_name'] + 
+                                "' is not recognized")
+
+    def setMainReIDer(self, reider="", auto_load=True):
+        """Set the main reider by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
+        dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
+        is optional. Different from the rest, setting the main reider by its name results in 
+        loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
+        If :func:`setConfigDir()` has not been called before, setting the main reider by a supported 
+        name results in referencing the internal config directory in order to load the 
+        corresponding configurations. 
+
+        Parameters
+        ----------
+        reider : str or dict, default=""
+            (1) Set :code:`reider=""` to set the main reider according to the main configurations 
+            or main.yaml and load its configurations from the reiders.yaml. 
+            (2) Set :code:`reider="FaceNet"`.etc, to set FaceNet as a reider and load its 
+            configurations from reiders.yaml.
+            (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
+            :code:`reider="[{'ri_name': 'Torchreid', 
+            'classifier_pkl': 'data/modules/torchreid/classifier/gta5_osnet_ain_ms_d_c.pkl', 
+            'train_data': 'data/datasets/GTA_V_DATASET/body_128x256', 'model_name': 'osnet_ain_x1_0', 
+            'model_path': 'data/modules/torchreid/models/torchreid/osnet_ain_ms_d_c.pth.tar', 
+            'min_confidence': 0.35}]"`.
+            (4) Set :code:`reider="a_supported_reider.yaml"` or :code:`reider="a_supported_reider.json"` 
+            to set a the main reider and its configurations from a YAML file. 
+        auto_load : bool, default=True
+            All supported reiders are Pytorch or Tensorflow based module, thus they need to 
+            initial and load their models/weights. :obj:`auto_load` is used to decide whether to 
+            load the reider automatically once the reider is set. Keep the :code:`auto_load=True` 
+            if it is meant for using :func:`reidPeople()`; however, even if the :code:`auto_load=False`, 
+            the :func:`reidPeople()` will initial and load the reider by itself, but it requires 
+            some time to do so.
+        """
+        self.__ri_is_set__ = False
+        self.__ri__ = []
+        if isinstance(reider, dict):
+            self.__setCustomReIDer__(reider, auto_load)
+        elif isinstance(reider, str):
+            if (isRawYAMLString(reider) or "yaml" in reider.lower() or 
+                "json" in reider.lower()):
+                self.__setCustomReIDer__(getCFGDict(reider), auto_load)
+            elif reider.lower() == "default":
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__loadDefaultReIDer__(auto_load=auto_load)
+                add_info_log("---PYPPBOX : Use reider according to the \"main.yaml\"")
+            elif reider.lower() == self.__unistrings__.facenet:
+                from pyppbox.modules.reiders.facenet import MyFaceNet
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllRCFG()
+                self.__ri_cfg__ = self.__cfg__.rcfg_facenet
+                self.__ri__ = MyFaceNet(self.__ri_cfg__, auto_load=auto_load)
+                self.__ri_is_set__ = True
+                add_info_log("---PYPPBOX : Set reider='" + str(reider) + "'")
+                self.__setGTDTOnly__()
+            elif reider.lower() == self.__unistrings__.torchreid:
+                from pyppbox.modules.reiders.torchreid import MyTorchreid
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllRCFG()
+                self.__ri_cfg__ = self.__cfg__.rcfg_torchreid
+                self.__ri__ = MyTorchreid(self.__ri_cfg__, auto_load=auto_load)
+                self.__ri_is_set__ = True
+                add_info_log("---PYPPBOX : Set reider='" + str(reider) + "'")
+                self.__setGTDTOnly__()
+            elif reider.lower() == self.__unistrings__.none:
+                if not self.__cfg_is_set__: self.setConfigDir()
+                self.__cfg__.setAllRCFG()
+                if (self.__dt_cfg__.dt_name.lower() != self.__unistrings__.none and 
+                    self.__tk_cfg__.tk_name.lower() != self.__unistrings__.none):
+                    self.__ri__ = TKOReider(static=True)
+                else:
+                    self.__ri__ = NothingReider()
+                self.__ri_cfg__ = __none_cfg__
+                self.__ri_is_set__ = True
+                add_info_log("---PYPPBOX : Set reider='" + str(reider) + "'")
+                self.__revokeGTDTOnly__()
         else:
-            msg = "PYPPBOX : reidPeople() -> The input 'people' is invalid."
-            add_error_log(msg)
-            raise ValueError(msg)
-    else:
-        add_warning_log("---PYPPBOX : reidPeople() -> The main ReIDer is not set.")
-    return res, tuple(reid_count)
-
-def __reidNormal__(img, people):
-    global __ri_cfg__
-    if __ri_cfg__.ri_name.lower() == __unistrings__.facenet:
-        return __reidFaceNormal__(img, people)
-    elif __ri_cfg__.ri_name.lower() == __unistrings__.torchreid:
-        return __reidDeepNormal__(img, people)
-    else:
-        return __reidEmpty__(img, people)
-
-def __reidDupkiller__(img, people):
-    global __ri_cfg__
-    if __ri_cfg__.ri_name.lower() == __unistrings__.facenet:
-        return __reidDupFacekiller__(img, people)
-    elif __ri_cfg__.ri_name.lower() == __unistrings__.torchreid:
-        return __reidDupDeepkiller__(img, people)
-    else:
-        return __reidEmpty__(img, people)
-
-def __reidEmpty__(_, people):
-    global __unistrings__, __ri__, __ri_cfg__
-    index = 0
-    for person in people:
-        deepid = str(person.deepid)
-        if __unistrings__.err_did in deepid or __unistrings__.unk_did in deepid:
-            people[index].deepid = __ri__.recognize(__unistrings__.unk_did)
-        index += 1
-    return people, 0
-
-def __reidDeepNormal__(img, people):
-    global __unistrings__, __ri__, __ri_cfg__, __deepidlistTMP__
-    reid_count = 0
-    index = 0
-    __deepidlistTMP__ = []
-    for person in people:
-        deepid = person.deepid
-        if __unistrings__.err_did in deepid or __unistrings__.unk_did in deepid:
-            miniframe = img.copy()
-            try:
-                [x1, y1, x2, y2] = person.box_xyxy
-                miniframe = miniframe[y1:y2, x1:x2]
-                people[index].deepid, people[index].deepid_conf = __ri__.recognize(
-                    cv2.resize(miniframe, __ri_cfg__.model_wh), 
-                    is_bgr=True
-                )
-                reid_count += 1
-            except Exception as e:
-                add_warning_log("---PYPPBOX : __reidDeepNormal__() -> " + str(e))
-        __deepidlistTMP__.append(deepid)
-        index += 1
-    return people, reid_count
-
-def __reidDupDeepkiller__(img, people):
-    global __ri__, __ri_cfg__, __deepidlistTMP__
-    reid_count = 0
-    if len(__deepidlistTMP__) != len(set(__deepidlistTMP__)):
-        ddeepids = [k for k, v in Counter(__deepidlistTMP__).items() if v > 1]
-        for ddeepid in ddeepids:
-            index = 0
-            for person in people:
+            add_warning_log("---PYPPBOX : reider='" + str(reider) + "' is not valid")
+
+    def reidPeople(self, img, people, deduplicate=True, img_is_mat=False):
+        """Re-identify people by giving an image and a list of detected or tracked people. 
+        :func:`setConfigDir()` or :func:`setMainReIDer()` must be called in advance.
+
+        Parameters
+        ----------
+        img : str or Mat
+            Set an image file or a cv :obj:`Mat`.
+        people : list[Person, ...]
+            Set a list of :class:`Person` object which stores the detected or tracked people in 
+            the input :obj:`img`.
+        deduplicate : bool, default=True
+            Indicate whether to re-reid people who have the same face ids or deep ids.
+        img_is_mat : bool, default=False
+            Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
+        
+        Returns
+        -------
+        list[Person, ...]
+            A list of :class:`Person` object which stores people with the updated IDs.
+        tuple(int, int)
+            A tuple of (ReID count, ReID deduplicate count).
+        """
+        res = []
+        reid_count = [0, 0]
+        if self.__ri_is_set__:
+            if self.__ri_cfg__.ri_name.lower() != self.__unistrings__.none:
+                if not self.__ri__.auto_load:
+                    self.__ri__.load_classifier()
+                    self.__ri__.auto_load = True
+            if isinstance(people, list):
+                if len(people) > 0:
+                    if isinstance(people[0], Person):
+                        if not img_is_mat: img = getCVMat(img)
+                        res, reid_count[0] = self.__reidNormal__(img, people)
+                        if deduplicate: res, reid_count[1] = self.__reidDupkiller__(img, res)
+                    else:
+                        msg = "PYPPBOX : reidPeople() -> Input 'people' has unsupported element."
+                        add_error_log(msg)
+                        raise ValueError(msg)
+            else:
+                msg = "PYPPBOX : reidPeople() -> The input 'people' is invalid."
+                add_error_log(msg)
+                raise ValueError(msg)
+        else:
+            add_warning_log("---PYPPBOX : reidPeople() -> The main ReIDer is not set.")
+        return res, tuple(reid_count)
+
+    def __reidNormal__(self, img, people):
+        if self.__ri_cfg__.ri_name.lower() == self.__unistrings__.facenet:
+            return self.__reidFaceNormal__(img, people)
+        elif self.__ri_cfg__.ri_name.lower() == self.__unistrings__.torchreid:
+            return self.__reidDeepNormal__(img, people)
+        else:
+            return self.__reidEmpty__(img, people)
+
+    def __reidDupkiller__(self, img, people):
+        if self.__ri_cfg__.ri_name.lower() == self.__unistrings__.facenet:
+            return self.__reidDupFacekiller__(img, people)
+        elif self.__ri_cfg__.ri_name.lower() == self.__unistrings__.torchreid:
+            return self.__reidDupDeepkiller__(img, people)
+        else:
+            return self.__reidEmpty__(img, people)
+
+    def __reidEmpty__(self, _, people):
+        index = 0
+        for person in people:
+            deepid = str(person.deepid)
+            if self.__unistrings__.err_did in deepid or self.__unistrings__.unk_did in deepid:
+                people[index].deepid = self.__ri__.recognize(self.__unistrings__.unk_did)
+            index += 1
+        return people, 0
+
+    def __reidDeepNormal__(self, img, people):
+        reid_count = 0
+        index = 0
+        self.__deepidlistTMP__ = []
+        for person in people:
+            deepid = person.deepid
+            if self.__unistrings__.err_did in deepid or self.__unistrings__.unk_did in deepid:
+                miniframe = img.copy()
                 try:
-                    if person.deepid == ddeepid:
-                        [x1, y1, x2, y2] = person.box_xyxy
-                        miniframe = img.copy()
-                        miniframe = miniframe[y1:y2, x1:x2]
-                        people[index].deepid, people[index].deepid_conf = __ri__.recognize(
-                            cv2.resize(miniframe, __ri_cfg__.model_wh), 
-                            is_bgr=True
-                        )
-                        reid_count += 1
+                    [x1, y1, x2, y2] = person.box_xyxy
+                    miniframe = miniframe[y1:y2, x1:x2]
+                    people[index].deepid, people[index].deepid_conf = self.__ri__.recognize(
+                        cv2.resize(miniframe, self.__ri_cfg__.model_wh), 
+                        is_bgr=True
+                    )
+                    reid_count += 1
                 except Exception as e:
-                    add_warning_log("---PYPPBOX : __reidDupDeepkiller__() -> " + str(e))
-                index += 1
-    return people, reid_count
-
-def __reidFaceNormal__(img, people):
-    global __unistrings__, __cfg__, __ri__, __faceidlistTMP__
-    reid_count = 0
-    index = 0
-    __faceidlistTMP__ = []
-    for person in people:
-        faceid = person.faceid
-        if __unistrings__.err_fid in faceid or __unistrings__.unk_fid in faceid:
-            (x, y) = person.repspoint
-            miniframe = img.copy()
-            try:
-                miniframe = miniframe[
-                    y + int(__cfg__.rcfg_facenet.yl_h_calibration[0]):
-                    y + int(__cfg__.rcfg_facenet.yl_h_calibration[1]), 
-                    x + int(__cfg__.rcfg_facenet.yl_w_calibration[0]):
-                    x + int(__cfg__.rcfg_facenet.yl_w_calibration[1])
-                ]
-                people[index].faceid, people[index].faceid_conf = __ri__.recognize(
-                    miniframe, 
-                    is_bgr=True
-                )
-                reid_count += 1
-            except Exception as e:
-                add_warning_log("---PYPPBOX : __reidFaceNormal__() -> " + str(e))
-        __faceidlistTMP__.append(faceid)
-        index += 1
-    return people, reid_count
-
-def __reidDupFacekiller__(img, people):
-    global __ri__, __cfg__, __faceidlistTMP__
-    reid_count = 0
-    if len(__faceidlistTMP__) != len(set(__faceidlistTMP__)):
-        dfaceids = [k for k, v in Counter(__faceidlistTMP__).items() if v > 1]
-        for dfaceid in dfaceids:
-            index = 0
-            for person in people:
+                    add_warning_log("---PYPPBOX : __reidDeepNormal__() -> " + str(e))
+            self.__deepidlistTMP__.append(deepid)
+            index += 1
+        return people, reid_count
+
+    def __reidDupDeepkiller__(self, img, people):
+        reid_count = 0
+        if len(self.__deepidlistTMP__) != len(set(self.__deepidlistTMP__)):
+            ddeepids = [k for k, v in Counter(self.__deepidlistTMP__).items() if v > 1]
+            for ddeepid in ddeepids:
+                index = 0
+                for person in people:
+                    try:
+                        if person.deepid == ddeepid:
+                            [x1, y1, x2, y2] = person.box_xyxy
+                            miniframe = img.copy()
+                            miniframe = miniframe[y1:y2, x1:x2]
+                            people[index].deepid, people[index].deepid_conf = self.__ri__.recognize(
+                                cv2.resize(miniframe, self.__ri_cfg__.model_wh), 
+                                is_bgr=True
+                            )
+                            reid_count += 1
+                    except Exception as e:
+                        add_warning_log("---PYPPBOX : __reidDupDeepkiller__() -> " + str(e))
+                    index += 1
+        return people, reid_count
+
+    def __reidFaceNormal__(self, img, people):
+        reid_count = 0
+        index = 0
+        self.__faceidlistTMP__ = []
+        for person in people:
+            faceid = person.faceid
+            if self.__unistrings__.err_fid in faceid or self.__unistrings__.unk_fid in faceid:
+                (x, y) = person.repspoint
+                miniframe = img.copy()
                 try:
-                    if person.faceid == dfaceid:
-                        (x, y) = person.repspoint
-                        miniframe = img.copy()
-                        miniframe = miniframe[
-                            y + int(__cfg__.rcfg_facenet.yl_h_calibration[0]):
-                            y + int(__cfg__.rcfg_facenet.yl_h_calibration[1]), 
-                            x + int(__cfg__.rcfg_facenet.yl_w_calibration[0]):
-                            x + int(__cfg__.rcfg_facenet.yl_w_calibration[1])
-                        ]
-                        people[index].faceid, people[index].faceid_conf = __ri__.recognize(
-                            miniframe, 
-                            is_bgr=True
-                        )
-                        reid_count += 1
+                    miniframe = miniframe[
+                        y + int(self.__cfg__.rcfg_facenet.yl_h_calibration[0]):
+                        y + int(self.__cfg__.rcfg_facenet.yl_h_calibration[1]), 
+                        x + int(self.__cfg__.rcfg_facenet.yl_w_calibration[0]):
+                        x + int(self.__cfg__.rcfg_facenet.yl_w_calibration[1])
+                    ]
+                    people[index].faceid, people[index].faceid_conf = self.__ri__.recognize(
+                        miniframe, 
+                        is_bgr=True
+                    )
+                    reid_count += 1
                 except Exception as e:
-                    add_warning_log("---PYPPBOX : __reidDupFacekiller__() -> " + str(e))
-                index += 1
-    return people, reid_count
-
-def trainReIDClassifier(reider="Default", train_data="", classifier_pkl=""):
-    """Train classifier of a reider by pointing to a data directory. Calling 
-    :func:`setConfigDir()` or :func:`setMainReIDer()` in advance is not required.
-
-    Parameters
-    ----------
-    reider : str or dict, default="Default" 
-        A supported name, a raw YAML/JSON string, a ready YAML/JSON dictionary, or a 
-        YAML/JSON file which is passed to :func:`setMainReIDer(reider=reider, auto_load=False)`.
-    train_data : str, default=""
-        A path of data to train, where consists of 2 or more sub-folders which classify 
-        2 or more people. Set :code:`train_data=""` or keep default to use the configured 
-        :obj:`train_data` according to the input :code:`reider`. All images in this the sub-folders 
-        must be 128x256 for Torchreid and 182x182 for FaceNet.
-    classifier_pkl : str, default=""
-        A file path for the classifier PKL file. Set :code:`classifier_pkl=""` or keep default 
-        to use the configured :obj:`classifier_pkl` in the input :obj:`reider`.
-    """
-    global __ri__, __ri_cfg__, __ri_is_set__
-    setMainReIDer(reider=reider, auto_load=False)
-    if __ri_is_set__:
-        valid_train_data = True
-        valid_pkl = True
-        if train_data != "":
-            if isExist(train_data): 
-                __ri_cfg__.train_data = getAbsPathFDS(train_data)
-            else: 
-                valid_train_data = False
-                add_error_log("---PYPPBOX : train_data='" + str(train_data) + 
-                              "' does not exist.")
-        if classifier_pkl != "":
-            if not isExist(getAncestorDir(classifier_pkl)):
-                valid_pkl = False
-                add_error_log("---PYPPBOX : classifier_pkl='" + str(classifier_pkl) + 
-                              "' is not valid.")
-            if valid_pkl: __ri_cfg__.classifier_pkl = getAbsPathFDS(classifier_pkl)
-        if valid_train_data and valid_pkl:
-            from pyppbox.modules.reiders.facenet import MyFaceNet
-            from pyppbox.modules.reiders.torchreid import MyTorchreid
-            if isinstance(__ri__, MyFaceNet):
-                __ri__ = MyFaceNet(__ri_cfg__, auto_load=False)
-                add_info_log("------------- FaceNet --------------")
-            elif isinstance(__ri__, MyTorchreid):
-                __ri__ = MyTorchreid(__ri_cfg__, auto_load=False)
-                add_info_log("------------ Torchreid -------------")
-            add_info_log("---PYPPBOX : train_data='" + str(__ri_cfg__.train_data) + "'")
-            add_info_log("---PYPPBOX : classifier_pkl='" + str(__ri_cfg__.classifier_pkl) + "'")
-            __ri__.train_classifier()
+                    add_warning_log("---PYPPBOX : __reidFaceNormal__() -> " + str(e))
+            self.__faceidlistTMP__.append(faceid)
+            index += 1
+        return people, reid_count
+
+    def __reidDupFacekiller__(self, img, people):
+        reid_count = 0
+        if len(self.__faceidlistTMP__) != len(set(self.__faceidlistTMP__)):
+            dfaceids = [k for k, v in Counter(self.__faceidlistTMP__).items() if v > 1]
+            for dfaceid in dfaceids:
+                index = 0
+                for person in people:
+                    try:
+                        if person.faceid == dfaceid:
+                            (x, y) = person.repspoint
+                            miniframe = img.copy()
+                            miniframe = miniframe[
+                                y + int(self.__cfg__.rcfg_facenet.yl_h_calibration[0]):
+                                y + int(self.__cfg__.rcfg_facenet.yl_h_calibration[1]), 
+                                x + int(self.__cfg__.rcfg_facenet.yl_w_calibration[0]):
+                                x + int(self.__cfg__.rcfg_facenet.yl_w_calibration[1])
+                            ]
+                            people[index].faceid, people[index].faceid_conf = self.__ri__.recognize(
+                                miniframe, 
+                                is_bgr=True
+                            )
+                            reid_count += 1
+                    except Exception as e:
+                        add_warning_log("---PYPPBOX : __reidDupFacekiller__() -> " + str(e))
+                    index += 1
+        return people, reid_count
+
+    def trainReIDClassifier(self, reider="Default", train_data="", classifier_pkl=""):
+        """Train classifier of a reider by pointing to a data directory. Calling 
+        :func:`setConfigDir()` or :func:`setMainReIDer()` in advance is not required.
+
+        Parameters
+        ----------
+        reider : str or dict, default="Default" 
+            A supported name, a raw YAML/JSON string, a ready YAML/JSON dictionary, or a 
+            YAML/JSON file which is passed to :func:`setMainReIDer(reider=reider, auto_load=False)`.
+        train_data : str, default=""
+            A path of data to train, where consists of 2 or more sub-folders which classify 
+            2 or more people. Set :code:`train_data=""` or keep default to use the configured 
+            :obj:`train_data` according to the input :code:`reider`. All images in this the sub-folders 
+            must be 128x256 for Torchreid and 182x182 for FaceNet.
+        classifier_pkl : str, default=""
+            A file path for the classifier PKL file. Set :code:`classifier_pkl=""` or keep default 
+            to use the configured :obj:`classifier_pkl` in the input :obj:`reider`.
+        """
+        self.setMainReIDer(reider=reider, auto_load=False)
+        if self.__ri_is_set__:
+            valid_train_data = True
+            valid_pkl = True
+            if train_data != "":
+                if isExist(train_data): 
+                    self.__ri_cfg__.train_data = getAbsPathFDS(train_data)
+                else: 
+                    valid_train_data = False
+                    add_error_log("---PYPPBOX : train_data='" + str(train_data) + 
+                                  "' does not exist.")
+            if classifier_pkl != "":
+                if not isExist(getAncestorDir(classifier_pkl)):
+                    valid_pkl = False
+                    add_error_log("---PYPPBOX : classifier_pkl='" + str(classifier_pkl) + 
+                                  "' is not valid.")
+                if valid_pkl: self.__ri_cfg__.classifier_pkl = getAbsPathFDS(classifier_pkl)
+            if valid_train_data and valid_pkl:
+                from pyppbox.modules.reiders.facenet import MyFaceNet
+                from pyppbox.modules.reiders.torchreid import MyTorchreid
+                if isinstance(self.__ri__, MyFaceNet):
+                    self.__ri__ = MyFaceNet(self.__ri_cfg__, auto_load=False)
+                    add_info_log("------------- FaceNet --------------")
+                elif isinstance(self.__ri__, MyTorchreid):
+                    self.__ri__ = MyTorchreid(self.__ri_cfg__, auto_load=False)
+                    add_info_log("------------ Torchreid -------------")
+                add_info_log("---PYPPBOX : train_data='" + str(self.__ri_cfg__.train_data) + "'")
+                add_info_log("---PYPPBOX : classifier_pkl='" + str(self.__ri_cfg__.classifier_pkl) + "'")
+                self.__ri__.train_classifier()
```

### Comparing `pyppbox-3.0b5/pyppbox/utils/__init__.py` & `pyppbox-3.1b1/pyppbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/utils/commontools.py` & `pyppbox-3.1b1/pyppbox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/utils/evatools.py` & `pyppbox-3.1b1/pyppbox/utils/evatools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/utils/gttools.py` & `pyppbox-3.1b1/pyppbox/utils/gttools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/utils/logtools.py` & `pyppbox-3.1b1/pyppbox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/utils/persontools.py` & `pyppbox-3.1b1/pyppbox/utils/persontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/utils/restools.py` & `pyppbox-3.1b1/pyppbox/utils/restools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox/utils/visualizetools.py` & `pyppbox-3.1b1/pyppbox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/pyppbox.egg-info/PKG-INFO` & `pyppbox-3.1b1/pyppbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.0b5
+Version: 3.1b1
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -44,11 +44,11 @@
 
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
-* Intergrate GUI for easy configurations and demo.
+* Integrate GUI for easy configurations and demo.
 * Support YAML/JSON configurations -> File, raw string and ready dictionary.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.0b5/pyppbox.egg-info/SOURCES.txt` & `pyppbox-3.1b1/pyppbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,19 @@
 pyppbox/modules/trackers/deepsort/origin/preprocessing.py
 pyppbox/modules/trackers/deepsort/origin/track.py
 pyppbox/modules/trackers/deepsort/origin/tracker.py
 pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
 pyppbox/modules/trackers/sort/__init__.py
 pyppbox/modules/trackers/sort/origin/sort.py
 pyppbox/standalone/__init__.py
+pyppbox/standalone/mt.py
 pyppbox/utils/__init__.py
 pyppbox/utils/commontools.py
 pyppbox/utils/evatools.py
 pyppbox/utils/gttools.py
 pyppbox/utils/logtools.py
 pyppbox/utils/persontools.py
 pyppbox/utils/restools.py
 pyppbox/utils/visualizetools.py
 requirements/README.md
-requirements/pippackages_cpu.txt
-requirements/pippackages_cuda.txt
+requirements/requirements.txt
 requirements/test_gpu.py
```

### Comparing `pyppbox-3.0b5/requirements/test_gpu.py` & `pyppbox-3.1b1/requirements/test_gpu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.0b5/setup.py` & `pyppbox-3.1b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,40 @@
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 from setuptools import find_packages, setup
 
-def main():
+
+def read_requirements():
+    with open("requirements/requirements.txt") as req_txt:
+        return [line for line in req_txt.read().splitlines()]
+
+def get_version_string():
+    version_py = "pyppbox/__init__.py"
+    with open(version_py) as version_file:
+        for line in version_file.read().splitlines():
+            if line.startswith('__version__'):
+                delim = '"' if '"' in line else "'"
+                return line.split(delim)[1]
+
+def get_packages():
+    import yaml
+    from yaml.loader import SafeLoader
+    packages = find_packages()
+    package_data = {}
+    with open("setup_extra.yaml") as setup_extra:
+        extra_dict = yaml.load(setup_extra, Loader=SafeLoader)
+        packages = packages + extra_dict['extra_data']
+        packages = list(set(packages))
+        for p in packages: package_data.update({p: ["*"]})
+    return packages, package_data
+
+def main_setup():
     long_description = open("README.md", encoding="utf-8").read()
     packages, package_data = get_packages()
     setup(
         name="pyppbox",
         version=get_version_string(),
         url="https://github.com/rathaumons/pyppbox",
         license="GPL-3.0-or-later",
@@ -33,15 +58,15 @@
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=packages,
         package_data=package_data,
         include_package_data=True,
         author="Ratha SIV",
         maintainer="rathaROG",
-        install_requires=["PyYAML", "setuptools>=67.2.0"],
+        install_requires=read_requirements(),
         keywords=['Toolbox', 'People Detecting', 'People Tracking', 'People Re-Identification'],
         python_requires=">=3.8",
         classifiers=[
             "Development Status :: 4 - Beta",
             "Environment :: Console",
             "Intended Audience :: Developers",
             "Intended Audience :: Education",
@@ -61,29 +86,9 @@
             "Operating System :: Microsoft :: Windows",
             "Operating System :: POSIX",
             "Operating System :: Unix",
             "Operating System :: MacOS",
         ],
     )
 
-def get_packages():
-    import yaml
-    from yaml.loader import SafeLoader
-    packages = find_packages()
-    package_data = {}
-    with open("setup_extra.yaml") as setup_extra:
-        extra_dict = yaml.load(setup_extra, Loader=SafeLoader)
-        packages = packages + extra_dict['extra_data']
-        packages = list(set(packages))
-        for p in packages: package_data.update({p: ["*"]})
-    return packages, package_data
-
-def get_version_string():
-    version_py = "pyppbox/__init__.py"
-    with open(version_py) as version_file:
-        for line in version_file.read().splitlines():
-            if line.startswith('__version__'):
-                delim = '"' if '"' in line else "'"
-                return line.split(delim)[1]
-
 if __name__ == "__main__":
-    main()
+    main_setup()
```

### Comparing `pyppbox-3.0b5/setup_extra.yaml` & `pyppbox-3.1b1/setup_extra.yaml`

 * *Files identical despite different names*

