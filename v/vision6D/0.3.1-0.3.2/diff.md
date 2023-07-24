# Comparing `tmp/vision6D-0.3.1.tar.gz` & `tmp/vision6D-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-64h00lvn\vision6D-0.3.1.tar", last modified: Mon Jul 24 17:11:20 2023, max compression
+gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-6og_s1pb\vision6D-0.3.2.tar", last modified: Mon Jul 24 18:57:18 2023, max compression
```

## Comparing `vision6D-0.3.1.tar` & `vision6D-0.3.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.593782 vision6D-0.3.1/
--rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       33 2023-07-05 00:49:40.000000 vision6D-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1364 2023-07-24 17:11:20.594782 vision6D-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.3.1/README.md
--rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     2111 2023-07-24 17:11:20.609783 vision6D-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      454 2023-07-07 18:51:59.000000 vision6D-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.156788 vision6D-0.3.1/test/
--rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.3.1/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.3.1/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.168783 vision6D-0.3.1/vision6D/
--rw-rw-rw-   0        0        0     1050 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.318781 vision6D-0.3.1/vision6D/components/
--rw-rw-rw-   0        0        0      512 2023-07-11 17:34:34.000000 vision6D-0.3.1/vision6D/components/__init__.py
--rw-rw-rw-   0        0        0     2035 2023-07-13 14:10:02.000000 vision6D-0.3.1/vision6D/components/bbox_store.py
--rw-rw-rw-   0        0        0     1938 2023-07-11 14:41:41.000000 vision6D-0.3.1/vision6D/components/camera_store.py
--rw-rw-rw-   0        0        0     2656 2023-07-16 03:30:44.000000 vision6D-0.3.1/vision6D/components/folder_store.py
--rw-rw-rw-   0        0        0     2648 2023-07-17 17:18:01.000000 vision6D-0.3.1/vision6D/components/image_store.py
--rw-rw-rw-   0        0        0     3142 2023-07-13 01:57:38.000000 vision6D-0.3.1/vision6D/components/mask_store.py
--rw-rw-rw-   0        0        0     7354 2023-07-11 17:33:12.000000 vision6D-0.3.1/vision6D/components/mesh_store.py
--rw-rw-rw-   0        0        0     1580 2023-07-07 15:56:19.000000 vision6D-0.3.1/vision6D/components/point_store.py
--rw-rw-rw-   0        0        0      242 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/components/singleton.py
--rw-rw-rw-   0        0        0     2179 2023-07-11 17:33:19.000000 vision6D-0.3.1/vision6D/components/video_store.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.425781 vision6D-0.3.1/vision6D/containers/
--rw-rw-rw-   0        0        0      614 2023-07-11 18:14:45.000000 vision6D-0.3.1/vision6D/containers/__init__.py
--rw-rw-rw-   0        0        0     4733 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/bbox_container.py
--rw-rw-rw-   0        0        0     4957 2023-07-18 15:12:42.000000 vision6D-0.3.1/vision6D/containers/camera_container.py
--rw-rw-rw-   0        0        0     5691 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/folder_container.py
--rw-rw-rw-   0        0        0     4266 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/image_container.py
--rw-rw-rw-   0        0        0     5078 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/mask_container.py
--rw-rw-rw-   0        0        0    17542 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/mesh_container.py
--rw-rw-rw-   0        0        0    10954 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/containers/pnp_container.py
--rw-rw-rw-   0        0        0     1881 2023-07-07 15:47:13.000000 vision6D-0.3.1/vision6D/containers/point_container.py
--rw-rw-rw-   0        0        0     9491 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/video_container.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.466785 vision6D-0.3.1/vision6D/data/
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.473785 vision6D-0.3.1/vision6D/data/icons/
--rw-rw-rw-   0        0        0     4280 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/data/icons/copy.png
--rw-rw-rw-   0        0        0    10905 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/data/icons/reset.png
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.3.1/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0    11885 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/data/style.qss
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.480785 vision6D-0.3.1/vision6D/entry/
--rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.3.1/vision6D/entry/__init__.py
--rw-rw-rw-   0        0        0      632 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/entry/main.py
--rw-rw-rw-   0        0        0    41105 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0      221 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/path.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.487787 vision6D-0.3.1/vision6D/tools/
--rw-rw-rw-   0        0        0       19 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/tools/__init__.py
--rw-rw-rw-   0        0        0    17276 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.591782 vision6D-0.3.1/vision6D/widgets/
--rw-rw-rw-   0        0        0      700 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/widgets/__init__.py
--rw-rw-rw-   0        0        0     3443 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/widgets/calibration_pop_window.py
--rw-rw-rw-   0        0        0     2026 2023-07-04 17:06:36.000000 vision6D-0.3.1/vision6D/widgets/camera_props_input_dialog.py
--rw-rw-rw-   0        0        0     1733 2023-07-17 22:11:41.000000 vision6D-0.3.1/vision6D/widgets/custom_qt_interactor.py
--rw-rw-rw-   0        0        0     5287 2023-07-17 17:08:30.000000 vision6D-0.3.1/vision6D/widgets/draw_bbox_window.py
--rw-rw-rw-   0        0        0     3708 2023-07-17 17:06:04.000000 vision6D-0.3.1/vision6D/widgets/draw_mask_window.py
--rw-rw-rw-   0        0        0     2535 2023-07-04 17:06:36.000000 vision6D-0.3.1/vision6D/widgets/get_text_dialog.py
--rw-rw-rw-   0        0        0     1281 2023-07-04 17:06:36.000000 vision6D-0.3.1/vision6D/widgets/popup_dialog.py
--rw-rw-rw-   0        0        0      313 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/widgets/search_bar.py
--rw-rw-rw-   0        0        0     7083 2023-07-10 15:16:47.000000 vision6D-0.3.1/vision6D/widgets/video_player.py
--rw-rw-rw-   0        0        0     5718 2023-07-04 17:06:36.000000 vision6D-0.3.1/vision6D/widgets/video_sampler.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.242785 vision6D-0.3.1/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1364 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1723 2023-07-24 17:11:20.000000 vision6D-0.3.1/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.632045 vision6D-0.3.2/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-07-05 00:49:40.000000 vision6D-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1364 2023-07-24 18:57:18.633046 vision6D-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.3.2/README.md
+-rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     2111 2023-07-24 18:57:18.640046 vision6D-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      454 2023-07-07 18:51:59.000000 vision6D-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.026783 vision6D-0.3.2/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.3.2/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.3.2/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.042270 vision6D-0.3.2/vision6D/
+-rw-rw-rw-   0        0        0     1050 2023-07-04 17:06:35.000000 vision6D-0.3.2/vision6D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.246560 vision6D-0.3.2/vision6D/components/
+-rw-rw-rw-   0        0        0      512 2023-07-11 17:34:34.000000 vision6D-0.3.2/vision6D/components/__init__.py
+-rw-rw-rw-   0        0        0     2035 2023-07-13 14:10:02.000000 vision6D-0.3.2/vision6D/components/bbox_store.py
+-rw-rw-rw-   0        0        0     1938 2023-07-11 14:41:41.000000 vision6D-0.3.2/vision6D/components/camera_store.py
+-rw-rw-rw-   0        0        0     2656 2023-07-16 03:30:44.000000 vision6D-0.3.2/vision6D/components/folder_store.py
+-rw-rw-rw-   0        0        0     2648 2023-07-17 17:18:01.000000 vision6D-0.3.2/vision6D/components/image_store.py
+-rw-rw-rw-   0        0        0     3142 2023-07-13 01:57:38.000000 vision6D-0.3.2/vision6D/components/mask_store.py
+-rw-rw-rw-   0        0        0     7354 2023-07-11 17:33:12.000000 vision6D-0.3.2/vision6D/components/mesh_store.py
+-rw-rw-rw-   0        0        0     1580 2023-07-07 15:56:19.000000 vision6D-0.3.2/vision6D/components/point_store.py
+-rw-rw-rw-   0        0        0      242 2023-07-04 17:06:35.000000 vision6D-0.3.2/vision6D/components/singleton.py
+-rw-rw-rw-   0        0        0     2179 2023-07-11 17:33:19.000000 vision6D-0.3.2/vision6D/components/video_store.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.394434 vision6D-0.3.2/vision6D/containers/
+-rw-rw-rw-   0        0        0      614 2023-07-11 18:14:45.000000 vision6D-0.3.2/vision6D/containers/__init__.py
+-rw-rw-rw-   0        0        0     4733 2023-07-23 03:20:53.000000 vision6D-0.3.2/vision6D/containers/bbox_container.py
+-rw-rw-rw-   0        0        0     4957 2023-07-18 15:12:42.000000 vision6D-0.3.2/vision6D/containers/camera_container.py
+-rw-rw-rw-   0        0        0     5691 2023-07-23 03:20:53.000000 vision6D-0.3.2/vision6D/containers/folder_container.py
+-rw-rw-rw-   0        0        0     4266 2023-07-23 03:20:53.000000 vision6D-0.3.2/vision6D/containers/image_container.py
+-rw-rw-rw-   0        0        0     5078 2023-07-23 03:20:53.000000 vision6D-0.3.2/vision6D/containers/mask_container.py
+-rw-rw-rw-   0        0        0    17542 2023-07-23 03:20:53.000000 vision6D-0.3.2/vision6D/containers/mesh_container.py
+-rw-rw-rw-   0        0        0    10954 2023-07-24 17:09:36.000000 vision6D-0.3.2/vision6D/containers/pnp_container.py
+-rw-rw-rw-   0        0        0     1881 2023-07-07 15:47:13.000000 vision6D-0.3.2/vision6D/containers/point_container.py
+-rw-rw-rw-   0        0        0     9491 2023-07-23 03:20:53.000000 vision6D-0.3.2/vision6D/containers/video_container.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.439455 vision6D-0.3.2/vision6D/data/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.480448 vision6D-0.3.2/vision6D/data/icons/
+-rw-rw-rw-   0        0        0     4280 2023-07-24 17:09:36.000000 vision6D-0.3.2/vision6D/data/icons/copy.png
+-rw-rw-rw-   0        0        0    10905 2023-07-24 17:09:36.000000 vision6D-0.3.2/vision6D/data/icons/reset.png
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.3.2/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0    11885 2023-07-04 17:06:35.000000 vision6D-0.3.2/vision6D/data/style.qss
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.490245 vision6D-0.3.2/vision6D/entry/
+-rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.3.2/vision6D/entry/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-07-04 17:06:35.000000 vision6D-0.3.2/vision6D/entry/main.py
+-rw-rw-rw-   0        0        0    41105 2023-07-24 18:56:17.000000 vision6D-0.3.2/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0      221 2023-07-24 17:09:36.000000 vision6D-0.3.2/vision6D/path.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.498889 vision6D-0.3.2/vision6D/tools/
+-rw-rw-rw-   0        0        0       19 2023-07-04 17:06:35.000000 vision6D-0.3.2/vision6D/tools/__init__.py
+-rw-rw-rw-   0        0        0    17276 2023-07-24 17:09:36.000000 vision6D-0.3.2/vision6D/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.628046 vision6D-0.3.2/vision6D/widgets/
+-rw-rw-rw-   0        0        0      700 2023-07-24 17:09:36.000000 vision6D-0.3.2/vision6D/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3443 2023-07-04 17:06:35.000000 vision6D-0.3.2/vision6D/widgets/calibration_pop_window.py
+-rw-rw-rw-   0        0        0     2026 2023-07-04 17:06:36.000000 vision6D-0.3.2/vision6D/widgets/camera_props_input_dialog.py
+-rw-rw-rw-   0        0        0     1733 2023-07-17 22:11:41.000000 vision6D-0.3.2/vision6D/widgets/custom_qt_interactor.py
+-rw-rw-rw-   0        0        0     5287 2023-07-17 17:08:30.000000 vision6D-0.3.2/vision6D/widgets/draw_bbox_window.py
+-rw-rw-rw-   0        0        0     3708 2023-07-17 17:06:04.000000 vision6D-0.3.2/vision6D/widgets/draw_mask_window.py
+-rw-rw-rw-   0        0        0     2535 2023-07-04 17:06:36.000000 vision6D-0.3.2/vision6D/widgets/get_text_dialog.py
+-rw-rw-rw-   0        0        0     1281 2023-07-04 17:06:36.000000 vision6D-0.3.2/vision6D/widgets/popup_dialog.py
+-rw-rw-rw-   0        0        0      313 2023-07-24 17:09:36.000000 vision6D-0.3.2/vision6D/widgets/search_bar.py
+-rw-rw-rw-   0        0        0     7083 2023-07-10 15:16:47.000000 vision6D-0.3.2/vision6D/widgets/video_player.py
+-rw-rw-rw-   0        0        0     5718 2023-07-04 17:06:36.000000 vision6D-0.3.2/vision6D/widgets/video_sampler.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:57:18.146576 vision6D-0.3.2/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1364 2023-07-24 18:57:17.000000 vision6D-0.3.2/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1723 2023-07-24 18:57:17.000000 vision6D-0.3.2/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 18:57:17.000000 vision6D-0.3.2/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-24 18:57:17.000000 vision6D-0.3.2/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-07-24 18:57:17.000000 vision6D-0.3.2/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 18:57:17.000000 vision6D-0.3.2/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.3.1/LICENSE` & `vision6D-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/PKG-INFO` & `vision6D-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.3.1
+Version: 0.3.2
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
 Project-URL: Documentation, https://vision6d.readthedocs.io/en/latest/
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.3.1/README.md` & `vision6D-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/setup.cfg` & `vision6D-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e33 2e31 0d0a 7572  sion = 0.3.1..ur
+00000020: 7369 6f6e 203d 2030 2e33 2e32 0d0a 7572  sion = 0.3.2..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.3.1/test/test_create_dataset.py` & `vision6D-0.3.2/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/test/test_projection.py` & `vision6D-0.3.2/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/__init__.py` & `vision6D-0.3.2/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/__init__.py` & `vision6D-0.3.2/vision6D/components/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/bbox_store.py` & `vision6D-0.3.2/vision6D/components/bbox_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/camera_store.py` & `vision6D-0.3.2/vision6D/components/camera_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/folder_store.py` & `vision6D-0.3.2/vision6D/components/folder_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/image_store.py` & `vision6D-0.3.2/vision6D/components/image_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/mask_store.py` & `vision6D-0.3.2/vision6D/components/mask_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/mesh_store.py` & `vision6D-0.3.2/vision6D/components/mesh_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/point_store.py` & `vision6D-0.3.2/vision6D/components/point_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/components/video_store.py` & `vision6D-0.3.2/vision6D/components/video_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/__init__.py` & `vision6D-0.3.2/vision6D/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/bbox_container.py` & `vision6D-0.3.2/vision6D/containers/bbox_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/camera_container.py` & `vision6D-0.3.2/vision6D/containers/camera_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/folder_container.py` & `vision6D-0.3.2/vision6D/containers/folder_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/image_container.py` & `vision6D-0.3.2/vision6D/containers/image_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/mask_container.py` & `vision6D-0.3.2/vision6D/containers/mask_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/mesh_container.py` & `vision6D-0.3.2/vision6D/containers/mesh_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/pnp_container.py` & `vision6D-0.3.2/vision6D/containers/pnp_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/point_container.py` & `vision6D-0.3.2/vision6D/containers/point_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/containers/video_container.py` & `vision6D-0.3.2/vision6D/containers/video_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/data/icons/copy.png` & `vision6D-0.3.2/vision6D/data/icons/copy.png`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/data/icons/reset.png` & `vision6D-0.3.2/vision6D/data/icons/reset.png`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.3.2/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/data/style.qss` & `vision6D-0.3.2/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/entry/main.py` & `vision6D-0.3.2/vision6D/entry/main.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/mainwindow.py` & `vision6D-0.3.2/vision6D/mainwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -810,14 +810,14 @@
 
         self.mesh_store.reset()
         self.point_store.reset()
         self.video_store.reset()
         self.folder_store.reset()
         self.workspace_path = ''
         self.track_actors_names.clear()
-        self.clear_output_text()
+        self.reset_output_text()
 
         self.color_button.setText("Color")
         self.play_video_button.setText("Play Video")
         self.opacity_spinbox.setValue(0.3)
         
         self.hintLabel.show()
```

### Comparing `vision6D-0.3.1/vision6D/tools/utils.py` & `vision6D-0.3.2/vision6D/tools/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/__init__.py` & `vision6D-0.3.2/vision6D/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/calibration_pop_window.py` & `vision6D-0.3.2/vision6D/widgets/calibration_pop_window.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/camera_props_input_dialog.py` & `vision6D-0.3.2/vision6D/widgets/camera_props_input_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/custom_qt_interactor.py` & `vision6D-0.3.2/vision6D/widgets/custom_qt_interactor.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/draw_bbox_window.py` & `vision6D-0.3.2/vision6D/widgets/draw_bbox_window.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/draw_mask_window.py` & `vision6D-0.3.2/vision6D/widgets/draw_mask_window.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/get_text_dialog.py` & `vision6D-0.3.2/vision6D/widgets/get_text_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/popup_dialog.py` & `vision6D-0.3.2/vision6D/widgets/popup_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/video_player.py` & `vision6D-0.3.2/vision6D/widgets/video_player.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D/widgets/video_sampler.py` & `vision6D-0.3.2/vision6D/widgets/video_sampler.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.1/vision6D.egg-info/PKG-INFO` & `vision6D-0.3.2/vision6D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.3.1
+Version: 0.3.2
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
 Project-URL: Documentation, https://vision6d.readthedocs.io/en/latest/
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.3.1/vision6D.egg-info/SOURCES.txt` & `vision6D-0.3.2/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

