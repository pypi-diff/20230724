# Comparing `tmp/zod-0.2.8.tar.gz` & `tmp/zod-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.2.8.tar", max compression
+gzip compressed data, was "zod-0.2.9.tar", max compression
```

## Comparing `zod-0.2.8.tar` & `zod-0.2.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2023-06-21 10:05:53.391525 zod-0.2.8/LICENSE
--rw-r--r--   0        0        0     4809 2023-06-21 10:05:53.391525 zod-0.2.8/README.md
--rw-r--r--   0        0        0     1783 2023-06-21 10:05:53.395525 zod-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      982 2023-06-21 10:05:53.395525 zod-0.2.8/zod/__init__.py
--rw-r--r--   0        0        0     4083 2023-06-21 10:05:53.395525 zod-0.2.8/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/lane.py
--rw-r--r--   0        0        0     4931 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/object.py
--rw-r--r--   0        0        0     2850 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-06-21 10:05:53.395525 zod-0.2.8/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    14496 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/download_zod.py
--rw-r--r--   0        0        0     7431 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6032 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1324 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/main.py
--rw-r--r--   0        0        0      655 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/utils.py
--rw-r--r--   0        0        0     4658 2023-06-21 10:05:53.395525 zod-0.2.8/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2403 2023-06-21 10:05:53.395525 zod-0.2.8/zod/constants.py
--rw-r--r--   0        0        0      184 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5044 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     4911 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5268 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     4441 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/sequence.py
--rw-r--r--   0        0        0     1004 2023-06-21 10:05:53.395525 zod-0.2.8/zod/data_classes/vehicle_data.py
--rw-r--r--   0        0        0       65 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12046 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0      437 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      355 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8399 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-06-21 10:05:53.395525 zod-0.2.8/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/geometry.py
--rw-r--r--   0        0        0     1044 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-06-21 10:05:53.395525 zod-0.2.8/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     8041 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/lidar_3d.py
--rw-r--r--   0        0        0     6028 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-06-21 10:05:53.395525 zod-0.2.8/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-06-21 10:05:53.399526 zod-0.2.8/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-06-21 10:05:53.399526 zod-0.2.8/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-06-21 10:05:53.399526 zod-0.2.8/zod/zod_drives.py
--rw-r--r--   0        0        0     1047 2023-06-21 10:05:53.399526 zod-0.2.8/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-06-21 10:05:53.399526 zod-0.2.8/zod/zod_sequences.py
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-21 12:50:03.778136 zod-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4809 2023-06-21 12:50:03.778136 zod-0.2.9/README.md
+-rw-r--r--   0        0        0     1783 2023-06-21 12:50:03.778136 zod-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-06-21 12:50:03.778136 zod-0.2.9/zod/__init__.py
+-rw-r--r--   0        0        0     4083 2023-06-21 12:50:03.778136 zod-0.2.9/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/lane.py
+-rw-r--r--   0        0        0     4931 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-06-21 12:50:03.778136 zod-0.2.9/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    15086 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/download_zod.py
+-rw-r--r--   0        0        0     7431 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6032 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1324 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/main.py
+-rw-r--r--   0        0        0      655 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/utils.py
+-rw-r--r--   0        0        0     4658 2023-06-21 12:50:03.778136 zod-0.2.9/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-06-21 12:50:03.778136 zod-0.2.9/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4911 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-06-21 12:50:03.778136 zod-0.2.9/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12046 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-06-21 12:50:03.778136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0      437 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      355 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8399 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-06-21 12:50:03.782136 zod-0.2.9/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/geometry.py
+-rw-r--r--   0        0        0     1044 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-06-21 12:50:03.782136 zod-0.2.9/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     8041 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/lidar_3d.py
+-rw-r--r--   0        0        0     6028 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-06-21 12:50:03.782136 zod-0.2.9/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-06-21 12:50:03.782136 zod-0.2.9/zod/zod_drives.py
+-rw-r--r--   0        0        0     1147 2023-06-21 12:50:03.782136 zod-0.2.9/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-06-21 12:50:03.782136 zod-0.2.9/zod/zod_sequences.py
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.9/PKG-INFO
```

### Comparing `zod-0.2.8/LICENSE` & `zod-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/README.md` & `zod-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/pyproject.toml` & `zod-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.2.8"
+version = "0.2.9"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.2.8/zod/__init__.py` & `zod-0.2.9/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/_zod_dataset.py` & `zod-0.2.9/zod/_zod_dataset.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/anno/lane.py` & `zod-0.2.9/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/anno/object.py` & `zod-0.2.9/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/anno/parser.py` & `zod-0.2.9/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/anno/tsr/class_map.py` & `zod-0.2.9/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/anno/tsr/traffic_sign.py` & `zod-0.2.9/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/cli/download_zod.py` & `zod-0.2.9/zod/cli/download_zod.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     file_path: str
     extract_dir: str
     dl_dir: str
     rm: bool
     dry_run: bool
     size: int
     extract: bool
+    extract_already_downloaded: bool
 
 
 @dataclass
 class FilterSettings:
     """Filter settings."""
 
     version: Version
@@ -77,14 +78,15 @@
     """Download settings."""
 
     url: str
     output_dir: str
     rm: bool
     dry_run: bool
     extract: bool
+    extract_already_downloaded: bool
     parallel: bool
 
     def __str__(self):
         return "\n".join([f"    {key}: {value}" for key, value in self.__dict__.items()])
 
 
 class ResumableDropbox(dropbox.Dropbox):
@@ -186,23 +188,28 @@
                 tar.extract(member=member, path=output_dir)
                 pbar.update(1)
     tqdm.write(f"Extracted {pbar.n} files from {osp.basename(tar_path)}.")
 
 
 def _download_and_extract(dbx: ResumableDropbox, info: DownloadExtractInfo):
     """Download a file from a Dropbox share link to a local path."""
+    should_extract = info.extract
     download_path = osp.join(info.dl_dir, osp.basename(info.file_path))
     if osp.exists(download_path) and osp.getsize(download_path) == info.size:
-        tqdm.write(f"File {download_path} already exists. Skipping download.")
+        if not info.extract_already_downloaded:
+            tqdm.write(f"File {download_path} already exists. Skipping download and extraction.")
+            should_extract = False
+        else:
+            tqdm.write(f"File {download_path} already exists. Skipping download.")
     elif info.dry_run:
         typer.echo(f"Would download {info.file_path} to {download_path}")
     else:
         _download(download_path, dbx, info)
 
-    if info.extract:
+    if should_extract:
         if info.dry_run:
             typer.echo(f"Would extract {download_path} to {info.extract_dir}")
             return
         else:
             _extract(download_path, info.extract_dir)
 
     if info.rm and not info.dry_run:
@@ -253,14 +260,15 @@
             file_path=f"/{dirname}/" + entry.name,
             dl_dir=dl_dir,
             extract_dir=dl_settings.output_dir,
             size=entry.size,
             rm=dl_settings.rm,
             dry_run=dl_settings.dry_run,
             extract=dl_settings.extract,
+            extract_already_downloaded=dl_settings.extract_already_downloaded,
         )
         for entry in entries
         if _filter_entry(entry, filter_settings)
     ]
     if not files_to_download:
         typer.echo("No files to download. Perhaps you specified too many filters?")
         return
@@ -351,14 +359,17 @@
         prompt_required=False,
         rich_help_panel=REQ,
     ),
     # General download settings
     rm: bool = typer.Option(False, help="Remove the downloaded archives", rich_help_panel=GEN),
     dry_run: bool = typer.Option(False, help="Print what would be downloaded", rich_help_panel=GEN),
     extract: bool = typer.Option(True, help="Unpack the archives", rich_help_panel=GEN),
+    extract_already_downloaded: bool = typer.Option(
+        False, help="Extract already downloaded archives", rich_help_panel=GEN
+    ),
     parallel: bool = typer.Option(True, help="Download files in parallel", rich_help_panel=GEN),
     no_confirm: bool = typer.Option(
         False,
         "-y",
         "--no-confirm/--confirm",
         help="Don't ask for confirmation",
         is_flag=True,
@@ -384,14 +395,15 @@
     """Download the Zenseact Open Dataset."""
     download_settings = DownloadSettings(
         url=url,
         output_dir=output_dir,
         rm=rm,
         dry_run=dry_run,
         extract=extract,
+        extract_already_downloaded=extract_already_downloaded,
         parallel=parallel,
     )
     filter_settings = FilterSettings(
         version=version,
         annotations=annotations,
         images=images,
         blur=blur,
```

### Comparing `zod-0.2.8/zod/cli/extract_tsr_patches.py` & `zod-0.2.9/zod/cli/extract_tsr_patches.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/cli/generate_coco_json.py` & `zod-0.2.9/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/cli/main.py` & `zod-0.2.9/zod/cli/main.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/cli/utils.py` & `zod-0.2.9/zod/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/cli/visualize_lidar.py` & `zod-0.2.9/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/constants.py` & `zod-0.2.9/zod/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/box.py` & `zod-0.2.9/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/calibration.py` & `zod-0.2.9/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/ego_motion.py` & `zod-0.2.9/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/frame.py` & `zod-0.2.9/zod/data_classes/frame.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/geometry.py` & `zod-0.2.9/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/info.py` & `zod-0.2.9/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/metadata.py` & `zod-0.2.9/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/sensor.py` & `zod-0.2.9/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/sequence.py` & `zod-0.2.9/zod/data_classes/sequence.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/data_classes/vehicle_data.py` & `zod-0.2.9/zod/data_classes/vehicle_data.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_experimental/eval.py` & `zod-0.2.9/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_experimental/matching.py` & `zod-0.2.9/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_experimental/utils.py` & `zod-0.2.9/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.2.9/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.2.9/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.2.9/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.2.9/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.2.9/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.2.9/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/utils/compensation.py` & `zod-0.2.9/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/utils/geometry.py` & `zod-0.2.9/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/utils/polygon_transformations.py` & `zod-0.2.9/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/utils/utils.py` & `zod-0.2.9/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/utils/visualization.py` & `zod-0.2.9/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/bev_utils.py` & `zod-0.2.9/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/colorlabeler.py` & `zod-0.2.9/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/lidar_3d.py` & `zod-0.2.9/zod/visualization/lidar_3d.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/lidar_bev.py` & `zod-0.2.9/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/lidar_on_image.py` & `zod-0.2.9/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/object_visualization.py` & `zod-0.2.9/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/oxts_on_image.py` & `zod-0.2.9/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/oxts_visualization.py` & `zod-0.2.9/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/visualization/polygon_utils.py` & `zod-0.2.9/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/zod_drives.py` & `zod-0.2.9/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/zod/zod_frames.py` & `zod-0.2.9/zod/zod_frames.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         info = super().__getitem__(frame_id)
         return ZodFrame(info)
 
     @property
     def trainval_files(self) -> Dict[str, str]:
         return TRAINVAL_FILES[FRAMES]
 
-    def get_subclass_counts(self) -> Dict[str, int]:
+    def get_subclass_counts(self, require_3d=False) -> Dict[str, int]:
         """Will scan the dataset and return all subclasses and their counts."""
         subclasses = defaultdict(int)
         for frame in tqdm(self, desc="Processing annotations..."):
             for obj in frame.get_annotation(AnnotationProject.OBJECT_DETECTION):
+                if require_3d and obj.box3d is None:
+                    continue
                 subclasses[obj.subclass] += 1
         return subclasses
```

### Comparing `zod-0.2.8/zod/zod_sequences.py` & `zod-0.2.9/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.8/PKG-INFO` & `zod-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.2.8
+Version: 0.2.9
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

