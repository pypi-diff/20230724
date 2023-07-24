# Comparing `tmp/vision6D-0.3.0.tar.gz` & `tmp/vision6D-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-kiutxfiz\vision6D-0.3.0.tar", last modified: Sun Jul 16 17:15:01 2023, max compression
+gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-64h00lvn\vision6D-0.3.1.tar", last modified: Mon Jul 24 17:11:20 2023, max compression
```

## Comparing `vision6D-0.3.0.tar` & `vision6D-0.3.1.tar`

### file list

```diff
@@ -1,63 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.597773 vision6D-0.3.0/
--rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       33 2023-07-05 00:49:40.000000 vision6D-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1364 2023-07-16 17:15:01.598770 vision6D-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.3.0/README.md
--rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0     2111 2023-07-16 17:15:01.612773 vision6D-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      454 2023-07-07 18:51:59.000000 vision6D-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:00.793629 vision6D-0.3.0/test/
--rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.3.0/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.3.0/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:00.824629 vision6D-0.3.0/vision6D/
--rw-rw-rw-   0        0        0     1050 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.089003 vision6D-0.3.0/vision6D/components/
--rw-rw-rw-   0        0        0      512 2023-07-11 17:34:34.000000 vision6D-0.3.0/vision6D/components/__init__.py
--rw-rw-rw-   0        0        0     2035 2023-07-13 14:10:02.000000 vision6D-0.3.0/vision6D/components/bbox_store.py
--rw-rw-rw-   0        0        0     1938 2023-07-11 14:41:41.000000 vision6D-0.3.0/vision6D/components/camera_store.py
--rw-rw-rw-   0        0        0     2656 2023-07-16 03:30:44.000000 vision6D-0.3.0/vision6D/components/folder_store.py
--rw-rw-rw-   0        0        0     2648 2023-07-12 18:27:30.000000 vision6D-0.3.0/vision6D/components/image_store.py
--rw-rw-rw-   0        0        0     3142 2023-07-13 01:57:38.000000 vision6D-0.3.0/vision6D/components/mask_store.py
--rw-rw-rw-   0        0        0     7354 2023-07-11 17:33:12.000000 vision6D-0.3.0/vision6D/components/mesh_store.py
--rw-rw-rw-   0        0        0     1580 2023-07-07 15:56:19.000000 vision6D-0.3.0/vision6D/components/point_store.py
--rw-rw-rw-   0        0        0      242 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/components/singleton.py
--rw-rw-rw-   0        0        0     2179 2023-07-11 17:33:19.000000 vision6D-0.3.0/vision6D/components/video_store.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.309143 vision6D-0.3.0/vision6D/containers/
--rw-rw-rw-   0        0        0      614 2023-07-11 18:14:45.000000 vision6D-0.3.0/vision6D/containers/__init__.py
--rw-rw-rw-   0        0        0     5050 2023-07-16 01:09:17.000000 vision6D-0.3.0/vision6D/containers/bbox_container.py
--rw-rw-rw-   0        0        0     4027 2023-07-10 17:15:51.000000 vision6D-0.3.0/vision6D/containers/camera_container.py
--rw-rw-rw-   0        0        0     6131 2023-07-16 03:32:31.000000 vision6D-0.3.0/vision6D/containers/folder_container.py
--rw-rw-rw-   0        0        0     4372 2023-07-14 15:23:54.000000 vision6D-0.3.0/vision6D/containers/image_container.py
--rw-rw-rw-   0        0        0     5339 2023-07-16 01:10:24.000000 vision6D-0.3.0/vision6D/containers/mask_container.py
--rw-rw-rw-   0        0        0    18163 2023-07-13 02:06:31.000000 vision6D-0.3.0/vision6D/containers/mesh_container.py
--rw-rw-rw-   0        0        0    11304 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/containers/pnp_container.py
--rw-rw-rw-   0        0        0     1881 2023-07-07 15:47:13.000000 vision6D-0.3.0/vision6D/containers/point_container.py
--rw-rw-rw-   0        0        0    10367 2023-07-16 03:03:04.000000 vision6D-0.3.0/vision6D/containers/video_container.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.351771 vision6D-0.3.0/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.3.0/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0    11885 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/data/style.qss
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.367772 vision6D-0.3.0/vision6D/entry/
--rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.3.0/vision6D/entry/__init__.py
--rw-rw-rw-   0        0        0      632 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/entry/main.py
--rw-rw-rw-   0        0        0    37415 2023-07-16 03:29:17.000000 vision6D-0.3.0/vision6D/mainwindow.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.409770 vision6D-0.3.0/vision6D/tools/
--rw-rw-rw-   0        0        0       19 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/tools/__init__.py
--rw-rw-rw-   0        0        0    17321 2023-07-13 01:25:37.000000 vision6D-0.3.0/vision6D/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.594769 vision6D-0.3.0/vision6D/widgets/
--rw-rw-rw-   0        0        0      646 2023-07-11 17:29:38.000000 vision6D-0.3.0/vision6D/widgets/__init__.py
--rw-rw-rw-   0        0        0     3443 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/widgets/calibration_pop_window.py
--rw-rw-rw-   0        0        0     2026 2023-07-04 17:06:36.000000 vision6D-0.3.0/vision6D/widgets/camera_props_input_dialog.py
--rw-rw-rw-   0        0        0     1694 2023-07-12 14:56:42.000000 vision6D-0.3.0/vision6D/widgets/custom_qt_interactor.py
--rw-rw-rw-   0        0        0     5461 2023-07-13 02:49:34.000000 vision6D-0.3.0/vision6D/widgets/draw_bbox_window.py
--rw-rw-rw-   0        0        0     3882 2023-07-12 15:18:40.000000 vision6D-0.3.0/vision6D/widgets/draw_mask_window.py
--rw-rw-rw-   0        0        0     2535 2023-07-04 17:06:36.000000 vision6D-0.3.0/vision6D/widgets/get_text_dialog.py
--rw-rw-rw-   0        0        0     1281 2023-07-04 17:06:36.000000 vision6D-0.3.0/vision6D/widgets/popup_dialog.py
--rw-rw-rw-   0        0        0     7083 2023-07-10 15:16:47.000000 vision6D-0.3.0/vision6D/widgets/video_player.py
--rw-rw-rw-   0        0        0     5718 2023-07-04 17:06:36.000000 vision6D-0.3.0/vision6D/widgets/video_sampler.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:15:00.906629 vision6D-0.3.0/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1364 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1616 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.593782 vision6D-0.3.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-07-05 00:49:40.000000 vision6D-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1364 2023-07-24 17:11:20.594782 vision6D-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.3.1/README.md
+-rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2111 2023-07-24 17:11:20.609783 vision6D-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      454 2023-07-07 18:51:59.000000 vision6D-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.156788 vision6D-0.3.1/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.3.1/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.3.1/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.168783 vision6D-0.3.1/vision6D/
+-rw-rw-rw-   0        0        0     1050 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.318781 vision6D-0.3.1/vision6D/components/
+-rw-rw-rw-   0        0        0      512 2023-07-11 17:34:34.000000 vision6D-0.3.1/vision6D/components/__init__.py
+-rw-rw-rw-   0        0        0     2035 2023-07-13 14:10:02.000000 vision6D-0.3.1/vision6D/components/bbox_store.py
+-rw-rw-rw-   0        0        0     1938 2023-07-11 14:41:41.000000 vision6D-0.3.1/vision6D/components/camera_store.py
+-rw-rw-rw-   0        0        0     2656 2023-07-16 03:30:44.000000 vision6D-0.3.1/vision6D/components/folder_store.py
+-rw-rw-rw-   0        0        0     2648 2023-07-17 17:18:01.000000 vision6D-0.3.1/vision6D/components/image_store.py
+-rw-rw-rw-   0        0        0     3142 2023-07-13 01:57:38.000000 vision6D-0.3.1/vision6D/components/mask_store.py
+-rw-rw-rw-   0        0        0     7354 2023-07-11 17:33:12.000000 vision6D-0.3.1/vision6D/components/mesh_store.py
+-rw-rw-rw-   0        0        0     1580 2023-07-07 15:56:19.000000 vision6D-0.3.1/vision6D/components/point_store.py
+-rw-rw-rw-   0        0        0      242 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/components/singleton.py
+-rw-rw-rw-   0        0        0     2179 2023-07-11 17:33:19.000000 vision6D-0.3.1/vision6D/components/video_store.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.425781 vision6D-0.3.1/vision6D/containers/
+-rw-rw-rw-   0        0        0      614 2023-07-11 18:14:45.000000 vision6D-0.3.1/vision6D/containers/__init__.py
+-rw-rw-rw-   0        0        0     4733 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/bbox_container.py
+-rw-rw-rw-   0        0        0     4957 2023-07-18 15:12:42.000000 vision6D-0.3.1/vision6D/containers/camera_container.py
+-rw-rw-rw-   0        0        0     5691 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/folder_container.py
+-rw-rw-rw-   0        0        0     4266 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/image_container.py
+-rw-rw-rw-   0        0        0     5078 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/mask_container.py
+-rw-rw-rw-   0        0        0    17542 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/mesh_container.py
+-rw-rw-rw-   0        0        0    10954 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/containers/pnp_container.py
+-rw-rw-rw-   0        0        0     1881 2023-07-07 15:47:13.000000 vision6D-0.3.1/vision6D/containers/point_container.py
+-rw-rw-rw-   0        0        0     9491 2023-07-23 03:20:53.000000 vision6D-0.3.1/vision6D/containers/video_container.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.466785 vision6D-0.3.1/vision6D/data/
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.473785 vision6D-0.3.1/vision6D/data/icons/
+-rw-rw-rw-   0        0        0     4280 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/data/icons/copy.png
+-rw-rw-rw-   0        0        0    10905 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/data/icons/reset.png
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.3.1/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0    11885 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/data/style.qss
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.480785 vision6D-0.3.1/vision6D/entry/
+-rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.3.1/vision6D/entry/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/entry/main.py
+-rw-rw-rw-   0        0        0    41105 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0      221 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/path.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.487787 vision6D-0.3.1/vision6D/tools/
+-rw-rw-rw-   0        0        0       19 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/tools/__init__.py
+-rw-rw-rw-   0        0        0    17276 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.591782 vision6D-0.3.1/vision6D/widgets/
+-rw-rw-rw-   0        0        0      700 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3443 2023-07-04 17:06:35.000000 vision6D-0.3.1/vision6D/widgets/calibration_pop_window.py
+-rw-rw-rw-   0        0        0     2026 2023-07-04 17:06:36.000000 vision6D-0.3.1/vision6D/widgets/camera_props_input_dialog.py
+-rw-rw-rw-   0        0        0     1733 2023-07-17 22:11:41.000000 vision6D-0.3.1/vision6D/widgets/custom_qt_interactor.py
+-rw-rw-rw-   0        0        0     5287 2023-07-17 17:08:30.000000 vision6D-0.3.1/vision6D/widgets/draw_bbox_window.py
+-rw-rw-rw-   0        0        0     3708 2023-07-17 17:06:04.000000 vision6D-0.3.1/vision6D/widgets/draw_mask_window.py
+-rw-rw-rw-   0        0        0     2535 2023-07-04 17:06:36.000000 vision6D-0.3.1/vision6D/widgets/get_text_dialog.py
+-rw-rw-rw-   0        0        0     1281 2023-07-04 17:06:36.000000 vision6D-0.3.1/vision6D/widgets/popup_dialog.py
+-rw-rw-rw-   0        0        0      313 2023-07-24 17:09:36.000000 vision6D-0.3.1/vision6D/widgets/search_bar.py
+-rw-rw-rw-   0        0        0     7083 2023-07-10 15:16:47.000000 vision6D-0.3.1/vision6D/widgets/video_player.py
+-rw-rw-rw-   0        0        0     5718 2023-07-04 17:06:36.000000 vision6D-0.3.1/vision6D/widgets/video_sampler.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:11:20.242785 vision6D-0.3.1/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1364 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1723 2023-07-24 17:11:20.000000 vision6D-0.3.1/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 17:11:19.000000 vision6D-0.3.1/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.3.0/LICENSE` & `vision6D-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/PKG-INFO` & `vision6D-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.3.0
+Version: 0.3.1
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
 Project-URL: Documentation, https://vision6d.readthedocs.io/en/latest/
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.3.0/README.md` & `vision6D-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/setup.cfg` & `vision6D-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e33 2e30 0d0a 7572  sion = 0.3.0..ur
+00000020: 7369 6f6e 203d 2030 2e33 2e31 0d0a 7572  sion = 0.3.1..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.3.0/test/test_create_dataset.py` & `vision6D-0.3.1/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/test/test_projection.py` & `vision6D-0.3.1/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/__init__.py` & `vision6D-0.3.1/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/__init__.py` & `vision6D-0.3.1/vision6D/components/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/bbox_store.py` & `vision6D-0.3.1/vision6D/components/bbox_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/camera_store.py` & `vision6D-0.3.1/vision6D/components/camera_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/folder_store.py` & `vision6D-0.3.1/vision6D/components/folder_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/image_store.py` & `vision6D-0.3.1/vision6D/components/image_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/mask_store.py` & `vision6D-0.3.1/vision6D/components/mask_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/mesh_store.py` & `vision6D-0.3.1/vision6D/components/mesh_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/point_store.py` & `vision6D-0.3.1/vision6D/components/point_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/components/video_store.py` & `vision6D-0.3.1/vision6D/components/video_store.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/containers/__init__.py` & `vision6D-0.3.1/vision6D/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/containers/bbox_container.py` & `vision6D-0.3.1/vision6D/containers/bbox_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def load_bbox(self, bbox):
         # Add bbox surface object to the plot
         bbox_mesh = self.plotter.add_mesh(bbox, color="yellow", opacity=self.bbox_store.bbox_opacity, line_width=2)
         actor, _ = self.plotter.add_actor(bbox_mesh, pickable=True, name='bbox')
         self.bbox_store.bbox_actor = actor
                 
     def add_bbox(self, bbox_source):
-        if (self.image_store.image_path) or (self.image_store.image_source is not None):
+        if self.image_store.image_actor:
             bbox = self.bbox_store.add_bbox(bbox_source, self.image_store.width, self.image_store.height)
             self.load_bbox(bbox)
             
             # Add remove current image to removeMenu
             if 'bbox' not in self.track_actors_names:
                 self.track_actors_names.append('bbox')
                 self.add_button_actor_name('bbox')
@@ -74,38 +74,35 @@
             return 0
     
     def draw_bbox(self):
         def handle_output_path_change(output_path):
             if output_path:
                 self.bbox_store.bbox_path = output_path
                 self.add_bbox(self.bbox_store.bbox_path)
-        if self.image_store.image_path:
-            self.bbox_window = BboxWindow(self.image_store.image_path)
-            self.bbox_window.bbox_label.output_path_changed.connect(handle_output_path_change)
-        elif self.image_store.image_source is not None:
-            self.bbox_window = BboxWindow(self.image_store.image_source)
+        if self.image_store.image_actor:
+            image = utils.get_image_actor_scalars(self.image_store.image_actor)
+            self.bbox_window = BboxWindow(image)
             self.bbox_window.bbox_label.output_path_changed.connect(handle_output_path_change)
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
     def reset_bbox(self):
         if self.bbox_store.bbox_path:
             self.bbox_store.mirror_x = False
             self.bbox_store.mirror_y = False
             bbox = self.bbox_store.add_bbox(self.bbox_store.bbox_path, self.image_store.width, self.image_store.height)
             self.load_bbox(bbox)
 
     def export_bbox(self):
         if self.bbox_store.bbox_actor:
-            # Store the transformed bbox actor if there is any transformation
-            points = utils.get_bbox_actor_points(self.bbox_store.bbox_actor, self.bbox_store.bbox_bottom_point, self.bbox_store.bbox_offset)
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Bbox Files (*.npy)")
             if output_path:
                 if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
+                # Store the transformed bbox actor if there is any transformation
+                points = utils.get_bbox_actor_points(self.bbox_store.bbox_actor, self.bbox_store.bbox_bottom_point, self.bbox_store.bbox_offset)
                 np.save(output_path, points)
                 self.output_text.append(f"-> Export Bbox points to:\n {output_path}")
-                self.output_text.append(f"\n************************************************************\n")
             self.bbox_store.bbox_path = output_path
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a bounding box first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.3.0/vision6D/containers/camera_container.py` & `vision6D-0.3.1/vision6D/containers/camera_container.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 @software: Vision6D
 @file: camera_container.py
 @time: 2023-07-03 20:25
 @desc: create container for camera related actions in application
 '''
 
 import ast
+import math
+import pickle
+import pathlib
 
 import numpy as np
 import PIL.Image
 
 from PyQt5 import QtWidgets
 
 from ..components import CameraStore
@@ -72,7 +75,19 @@
                     QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Error occured, check the format of the input values", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def zoom_in(self):
         self.plotter.camera.zoom(2)
 
     def zoom_out(self):
         self.plotter.camera.zoom(0.5)
+
+    def export_camera_info(self):
+        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Camera Info Files (*.pkl)")
+        if output_path:
+            if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.pkl')
+            camera_intrinsics = self.camera_store.camera_intrinsics.astype('float32')
+            focal_length = (1080 / 2.0) / math.tan(math.radians(self.plotter.camera.view_angle / 2))
+            camera_intrinsics[0, 0] = focal_length
+            camera_intrinsics[1, 1] = focal_length
+            camera_position = self.plotter.camera.position
+            camera_info = {'camera_intrinsics': camera_intrinsics, 'camera_position': np.array(camera_position)}
+            with open(output_path,"wb") as f: pickle.dump(camera_info, f)
```

### Comparing `vision6D-0.3.0/vision6D/containers/folder_container.py` & `vision6D-0.3.1/vision6D/containers/folder_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,47 +56,43 @@
                 os.makedirs(pathlib.Path(self.folder_store.folder_path) / "vision6D" / "images", exist_ok=True)
                 output_image_path = pathlib.Path(self.folder_store.folder_path) / "vision6D" / "images" / f"{id}.png"
                 image_rendered = self.image_store.render_image(camera=self.plotter.camera.copy())
                 save_image = PIL.Image.fromarray(image_rendered)
                 save_image.save(output_image_path)
                 self.image_store.image_path = str(output_image_path)
                 self.output_text.append(f"-> Save image {self.folder_store.current_image} to {str(output_image_path)}")
-                self.output_text.append(f"\n************************************************************\n")
 
             if len(self.mesh_store.mesh_actors) > 0:
                 os.makedirs(pathlib.Path(self.folder_store.folder_path) / "vision6D" / "poses", exist_ok=True)
                 output_pose_path = pathlib.Path(self.folder_store.folder_path) / "vision6D" / "poses" / f"{id}.npy"
                 self.current_pose()
                 np.save(output_pose_path, self.mesh_store.transformation_matrix)
                 self.output_text.append(f"-> Save image {self.folder_store.current_image} pose to {str(output_pose_path)}:")
                 self.output_text.append(f"{self.mesh_store.transformation_matrix}")
-                self.output_text.append(f"\n************************************************************\n")
         
             # save mask if there is a mask  
             if self.mask_store.mask_actor is not None:
                 os.makedirs(pathlib.Path(self.folder_store.folder_path) / "vision6D" / "masks", exist_ok=True)
                 output_mask_path = pathlib.Path(self.folder_store.folder_path) / "vision6D" / "masks" / f"{id}.png"
                 mask_surface = self.mask_store.update_mask()
                 self.load_mask(mask_surface)
                 image = self.mask_store.render_mask(camera=self.plotter.camera.copy())
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_mask_path)
                 self.mask_store.mask_path = output_mask_path
                 self.output_text.append(f"-> Save image {self.folder_store.current_image} mask render to {output_mask_path}")
-                self.output_text.append(f"\n************************************************************\n")
 
             # save bbox if there is a bbox  
             if self.bbox_store.bbox_actor is not None:
                 os.makedirs(pathlib.Path(self.folder_store.folder_path) / "vision6D" / "bboxs", exist_ok=True)
                 output_bbox_path = pathlib.Path(self.folder_store.folder_path) / "vision6D" / "bboxs" / f"{id}.npy"
                 points = utils.get_bbox_actor_points(self.bbox_store.bbox_actor, self.bbox_store.bbox_bottom_point, self.bbox_store.bbox_offset)
                 np.save(output_bbox_path, points)
                 self.bbox_store.bbox_path = output_bbox_path
                 self.output_text.append(f"-> Save image {self.folder_store.current_image} bbox points to {output_bbox_path}")
-                self.output_text.append(f"\n************************************************************\n")
         else: 
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a folder!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
   
     def prev_info(self):
         if self.folder_store.folder_path:
             self.folder_store.prev_image()
             self.play_video_button.setText(f"Image ({self.folder_store.current_image}/{self.folder_store.total_image})")
```

### Comparing `vision6D-0.3.0/vision6D/containers/image_container.py` & `vision6D-0.3.1/vision6D/containers/image_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,19 +81,18 @@
         if not up: change *= -1
         self.image_store.update_opacity(change)
         self.plotter.add_actor(self.image_store.image_actor, pickable=False, name="image")
         self.check_button(actor_name='image')
 
     def export_image(self):
         if self.image_store.image_actor:
-            image_rendered = self.image_store.render_image(camera=self.plotter.camera.copy())
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Image Files (*.png)")
             if output_path:
                 if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
+                image_rendered = self.image_store.render_image(camera=self.plotter.camera.copy())
                 rendered_image = PIL.Image.fromarray(image_rendered)
                 rendered_image.save(output_path)
                 self.output_text.append(f"-> Export image render to:\n {output_path}")
-                self.output_text.append(f"\n************************************************************\n")
             self.image_store.image_path = output_path
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.3.0/vision6D/containers/mask_container.py` & `vision6D-0.3.1/vision6D/containers/mask_container.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,34 +88,31 @@
         self.check_button(actor_name='mask')
     
     def draw_mask(self):
         def handle_output_path_change(output_path):
             if output_path:
                 self.mask_store.mask_path = output_path
                 self.add_mask(self.mask_store.mask_path)
-        if self.image_store.image_path:
-            self.mask_window = MaskWindow(self.image_store.image_path)
-            self.mask_window.mask_label.output_path_changed.connect(handle_output_path_change)
-        elif self.image_store.image_source is not None:
-            self.mask_window = MaskWindow(self.image_store.image_source)
+        if self.image_store.image_actor:
+            image = utils.get_image_actor_scalars(self.image_store.image_actor)
+            self.mask_window = MaskWindow(image)
             self.mask_window.mask_label.output_path_changed.connect(handle_output_path_change)
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
     def export_mask(self):
         if self.mask_store.mask_actor:
-            # Store the transformed mask actor if there is any transformation
-            mask_surface = self.mask_store.update_mask()
-            self.load_mask(mask_surface)
-            image = self.mask_store.render_mask(camera=self.plotter.camera.copy())
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Mask Files (*.png)")
             if output_path:
                 if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
+                # Store the transformed mask actor if there is any transformation
+                mask_surface = self.mask_store.update_mask()
+                self.load_mask(mask_surface)
+                image = self.mask_store.render_mask(camera=self.plotter.camera.copy())
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
                 self.output_text.append(f"-> Export mask render to:\n {output_path}")
-                self.output_text.append(f"\n************************************************************\n")
             self.mask_store.mask_path = output_path
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a mask first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.3.0/vision6D/containers/mesh_container.py` & `vision6D-0.3.1/vision6D/containers/mesh_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         elif direction == 'y': self.mesh_store.mirror_y = not self.mesh_store.mirror_y
         transformation_matrix = self.mesh_store.initial_pose
         if self.mesh_store.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
         if self.mesh_store.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
         self.add_mesh(self.mesh_store.meshdict[self.mesh_store.reference], transformation_matrix)
         self.mesh_store.undo_poses.clear()
         self.output_text.append(f"-> Mirrored transformation matrix is: \n{transformation_matrix}")
-        self.output_text.append(f"\n************************************************************\n")
 
     def add_mesh(self, mesh_source, transformation_matrix=None):
         """ add a mesh to the pyqt frame """
         source_verts, source_faces = self.mesh_store.add_mesh(mesh_source)
         if self.mesh_store.mesh_info:
             mesh = self.plotter.add_mesh(self.mesh_store.mesh_info, color=self.mesh_store.mesh_colors[self.mesh_store.mesh_name], opacity=self.mesh_store.mesh_opacity[self.mesh_store.mesh_name], name=self.mesh_store.mesh_name)
             mesh.user_matrix = self.mesh_store.transformation_matrix if transformation_matrix is None else transformation_matrix
@@ -232,45 +231,42 @@
                     QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "It needs to be a 4 by 4 matrix", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok) 
             except: 
                 QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
     
     def reset_gt_pose(self):
         if self.mesh_store.initial_pose is not None:
             self.output_text.append(f"-> Reset the GT pose to: \n{self.mesh_store.initial_pose}")
-            self.output_text.append(f"\n************************************************************\n")
             self.register_pose(self.mesh_store.initial_pose)
             self.reset_camera()
 
     def update_gt_pose(self):
         if self.mesh_store.initial_pose is not None:
             self.mesh_store.initial_pose = self.mesh_store.transformation_matrix
             self.current_pose()
             self.output_text.append(f"-> Update the GT pose to: \n{self.mesh_store.initial_pose}")
-            self.output_text.append(f"\n************************************************************\n")
 
     def undo_pose(self):
         if self.button_group_actors_names.checkedButton():
             actor_name = self.button_group_actors_names.checkedButton().text()
             if actor_name in self.mesh_store.mesh_actors:
                 if self.mesh_store.undo_poses and len(self.mesh_store.undo_poses[actor_name]) != 0: 
                     self.mesh_store.undo_pose(actor_name)
                     # register the rest meshes' pose to current undoed pose
                     self.check_button(actor_name=actor_name)
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Choose a mesh actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def export_pose(self):
-        if self.mesh_store.reference: 
-            self.update_gt_pose()
+        if self.mesh_store.reference:
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Pose Files (*.npy)")
             if output_path:
                 if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.npy')
+                self.update_gt_pose()
                 np.save(output_path, self.mesh_store.transformation_matrix)
                 self.output_text.append(f"-> Saved:\n{self.mesh_store.transformation_matrix}\nExport to:\n {output_path}")
-                self.output_text.append(f"\n************************************************************\n")
             self.mesh_store.pose_path = output_path
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
     
     def export_mesh_render(self, save_render=True):
         image = None
         if self.mesh_store.reference:
@@ -278,30 +274,28 @@
             if save_render:
                 output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Mesh Files (*.png)")
                 if output_path:
                     if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
                     rendered_image = PIL.Image.fromarray(image)
                     rendered_image.save(output_path)
                     self.output_text.append(f"-> Export mesh render to:\n {output_path}")
-                    self.output_text.append(f"\n************************************************************\n")
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
         return image
 
     def export_segmesh_render(self):
         if self.mesh_store.reference and self.mask_store.mask_actor:
-            mask_surface = self.mask_store.update_mask()
-            self.load_mask(mask_surface)
-            segmask = self.mask_store.render_mask(camera=self.plotter.camera.copy())
-            if np.max(segmask) > 1: segmask = segmask / 255
-            image = self.mesh_store.render_mesh(camera=self.plotter.camera.copy())
-            image = (image * segmask).astype(np.uint8)
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "SegMesh Files (*.png)")
             if output_path:
                 if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
+                mask_surface = self.mask_store.update_mask()
+                self.load_mask(mask_surface)
+                segmask = self.mask_store.render_mask(camera=self.plotter.camera.copy())
+                if np.max(segmask) > 1: segmask = segmask / 255
+                image = self.mesh_store.render_mesh(camera=self.plotter.camera.copy())
+                image = (image * segmask).astype(np.uint8)
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
                 self.output_text.append(f"-> Export segmask render:\n to {output_path}")
-                self.output_text.append(f"\n************************************************************\n")
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a mesh or mask first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.3.0/vision6D/containers/pnp_container.py` & `vision6D-0.3.1/vision6D/containers/pnp_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,21 +93,20 @@
                         vertices, faces = utils.get_mesh_actor_vertices_faces(self.mesh_store.mesh_actors[self.mesh_store.reference])
                         mesh = trimesh.Trimesh(vertices, faces, process=False)
                         predicted_pose = self.nocs_epnp(color_mask, mesh)
                         if self.mesh_store.mirror_x: predicted_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                         if self.mesh_store.mirror_y: predicted_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                         angular_distance = utils.angler_distance(predicted_pose[:3, :3], gt_pose[:3, :3])
                         translation_error = np.linalg.norm(predicted_pose[:3, 3] - gt_pose[:3, 3])
-                        self.output_text.append(f"Predicted pose with <span style='background-color:yellow; color:black;'>NOCS color</span>: ")
+                        self.output_text.append(f"Predicted pose with NOCS color: ")
                         self.output_text.append(f"{predicted_pose}")
                         self.output_text.append(f"GT Pose: ")
                         self.output_text.append(f"{gt_pose}")
                         self.output_text.append(f"Angular Error (in degree): {angular_distance}")
                         self.output_text.append(f"Translation Error: {translation_error}")
-                        self.output_text.append(f"\n************************************************************\n")
                     else:
                         QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Only works using EPnP with latlon mask", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 else:
                     QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             else:
                 QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "The mesh need to be colored, with gradient color", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
         else:
@@ -154,20 +153,19 @@
                     else: 
                         color_theme = 'LATLON'
                         if self.mesh_store.mirror_x: color_mask = color_mask[:, ::-1, :]
                         if self.mesh_store.mirror_y: color_mask = color_mask[::-1, :, :]
                         predicted_pose = self.latlon_epnp(color_mask, mesh)
                     angular_distance = utils.angler_distance(predicted_pose[:3, :3], gt_pose[:3, :3])
                     translation_error = np.linalg.norm(predicted_pose[:3, 3] - gt_pose[:3, 3])
-                    self.output_text.append(f"Predicted pose with <span style='background-color:yellow; color:black;'>{color_theme} color (masked)</span>: ")
+                    self.output_text.append(f"Predicted pose with {color_theme} color (masked): ")
                     self.output_text.append(f"{predicted_pose}")
                     self.output_text.append(f"GT Pose: ")
                     self.output_text.append(f"{gt_pose}")
                     self.output_text.append(f"Angular Error (in degree): {angular_distance}")
                     self.output_text.append(f"Translation Error: {translation_error}")
-                    self.output_text.append(f"\n************************************************************\n")
                 else:
                     QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(),"vision6D", "Clicked the wrong method")
             else:
                 QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(),"vision6D", "please load a mask first")
```

### Comparing `vision6D-0.3.0/vision6D/containers/point_container.py` & `vision6D-0.3.1/vision6D/containers/point_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/containers/video_container.py` & `vision6D-0.3.1/vision6D/containers/video_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         if video_path:
             if self.folder_store.folder_path: self.clear_plot() # main goal is to set folder_path to None
             self.hintLabel.hide()
             self.video_store.add_video(video_path)
             self.play_video_button.setEnabled(True)
             self.play_video_button.setText(f"Play ({self.video_store.current_frame}/{self.video_store.total_frame})")
             self.output_text.append(f"-> Load video {self.video_store.video_path} into vision6D")
-            self.output_text.append(f"\n************************************************************\n")
             self.load_per_frame_info()
             self.sample_video()
 
     def load_per_frame_info(self):
         video_frame = self.video_store.load_per_frame_info()
         if video_frame is not None: 
             self.add_image(video_frame)
@@ -97,64 +96,58 @@
                 os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "frames", exist_ok=True)
                 output_frame_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "frames" / f"frame_{self.video_store.current_frame}.png"
                 image_rendered = self.image_store.render_image(camera=self.plotter.camera.copy())
                 save_frame = PIL.Image.fromarray(image_rendered)
                 save_frame.save(output_frame_path)
                 self.image_store.image_path = str(output_frame_path)
                 self.output_text.append(f"-> Save frame {self.video_store.current_frame} to {str(output_frame_path)}")
-                self.output_text.append(f"\n************************************************************\n")
         
             # save gt_pose for each frame if there are any meshes
             if len(self.mesh_store.mesh_actors) > 0:
                 os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "poses", exist_ok=True)
                 output_pose_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "poses" / f"pose_{self.video_store.current_frame}.npy"
                 self.current_pose()
                 np.save(output_pose_path, self.mesh_store.transformation_matrix)
                 self.output_text.append(f"-> Save frame {self.video_store.current_frame} pose to {str(output_pose_path)}:")
                 self.output_text.append(f"{self.mesh_store.transformation_matrix}")
-                self.output_text.append(f"\n************************************************************\n")
 
             # save mask if there is a mask  
             if self.mask_store.mask_actor is not None:
                 os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "masks", exist_ok=True)
                 output_mask_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "masks" / f"mask_{self.video_store.current_frame}.png"
                 mask_surface = self.mask_store.update_mask()
                 self.load_mask(mask_surface)
                 image = self.mask_store.render_mask(camera=self.plotter.camera.copy())
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_mask_path)
                 self.mask_store.mask_path = output_mask_path
                 self.output_text.append(f"-> Save frame {self.video_store.current_frame} mask render to {output_mask_path}")
-                self.output_text.append(f"\n************************************************************\n")
 
             # save bbox if there is a bbox  
             if self.bbox_store.bbox_actor is not None:
                 os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "bboxs", exist_ok=True)
                 output_bbox_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "bboxs" / f"bbox_{self.video_store.current_frame}.npy"
                 points = utils.get_bbox_actor_points(self.bbox_store.bbox_actor, self.bbox_store.bbox_bottom_point, self.bbox_store.bbox_offset)
                 np.save(output_bbox_path, points)
                 self.bbox_store.bbox_path = output_bbox_path
                 self.output_text.append(f"-> Save frame {self.video_store.current_frame} bbox points to {output_bbox_path}")
-                self.output_text.append(f"\n************************************************************\n")
     
         else: 
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def prev_info(self):
         if self.video_store.video_path:
             self.video_store.prev_frame()
             pose_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "poses" / f"pose_{self.video_store.current_frame}.npy"
             if os.path.isfile(pose_path): 
                 self.mesh_store.transformation_matrix = np.load(pose_path)
                 self.register_pose(self.mesh_store.transformation_matrix)
                 self.output_text.append(f"-> Load saved frame {self.video_store.current_frame} pose: \n{self.mesh_store.transformation_matrix}")
-                self.output_text.append(f"\n************************************************************\n")
             else: 
                 self.output_text.append(f"-> No saved pose for frame {self.video_store.current_frame}")
-                self.output_text.append(f"\n************************************************************\n")
             self.play_video_button.setText(f"Play ({self.video_store.current_frame}/{self.video_store.total_frame})")
             self.load_per_frame_info()
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
     def next_info(self):
@@ -163,13 +156,12 @@
             self.video_store.next_frame()
             # load pose for the current frame if the pose exist
             pose_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "poses" / f"pose_{self.video_store.current_frame}.npy"
             if os.path.isfile(pose_path): 
                 self.mesh_store.transformation_matrix = np.load(pose_path)
                 self.register_pose(self.mesh_store.transformation_matrix)
                 self.output_text.append(f"-> Load saved frame {self.video_store.current_frame} pose: \n{self.mesh_store.transformation_matrix}")
-                self.output_text.append(f"\n************************************************************\n")
             self.play_video_button.setText(f"Play ({self.video_store.current_frame}/{self.video_store.total_frame})")
             self.load_per_frame_info()
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.3.0/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.3.1/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/data/style.qss` & `vision6D-0.3.1/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/entry/main.py` & `vision6D-0.3.1/vision6D/entry/main.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/mainwindow.py` & `vision6D-0.3.1/vision6D/mainwindow.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from PyQt5 import QtWidgets, QtGui
 from pyvistaqt import MainWindow
 from PyQt5.QtCore import Qt, QPoint
 
 # self defined package import
 from .widgets import CustomQtInteractor
 from .widgets import PopUpDialog
+from .widgets import SearchBar
 
 from .components import CameraStore
 from .components import ImageStore
 from .components import MaskStore
 from .components import BboxStore
 from .components import MeshStore
 from .components import PointStore
@@ -42,14 +43,16 @@
 from .containers import BboxContainer
 from .containers import MeshContainer
 from .containers import PointContainer
 from .containers import PnPContainer
 from .containers import VideoContainer
 from .containers import FolderContainer
 
+from .path import ICON_PATH
+
 np.set_printoptions(suppress=True)
 
 class MyMainWindow(MainWindow):
     def __init__(self, parent=None):
         QtWidgets.QMainWindow.__init__(self, parent)
         
         # Set up the main window layout
@@ -291,14 +294,15 @@
         exportMenu = mainMenu.addMenu('Export')
         exportMenu.addAction('Image', self.image_container.export_image)
         exportMenu.addAction('Mask', self.mask_container.export_mask)
         exportMenu.addAction('Bbox', self.bbox_container.export_bbox)
         exportMenu.addAction('Pose', self.mesh_container.export_pose)
         exportMenu.addAction('Mesh Render', self.mesh_container.export_mesh_render)
         exportMenu.addAction('SegMesh Render', self.mesh_container.export_segmesh_render)
+        exportMenu.addAction('Camera Info', self.camera_container.export_camera_info)
 
         # Add draw related actions
         DrawMenu = mainMenu.addMenu('Draw')
         DrawMenu.addAction('Mask', self.mask_container.draw_mask)
         DrawMenu.addAction('BBox', self.bbox_container.draw_bbox)
         # DrawMenu.addAction('Points', self.point_container.draw_point)
         DrawMenu.addAction('Reset Mask (t)', self.mask_container.reset_mask)
@@ -458,65 +462,149 @@
 
         #* Create the top widgets (layout)
         top_layout = QtWidgets.QHBoxLayout()
         top_layout.setContentsMargins(0, 0, 0, 0)
 
         # Create Grid layout for function buttons
         grid_layout = QtWidgets.QGridLayout()
+        
+        # Create a SearchBar for search bar
+        self.search_bar = SearchBar()
+        self.search_bar.setPlaceholderText("Search...")
+
+        # Add a signal to the QLineEdit object to connect to a function
+        self.search_bar.textChanged.connect(self.handle_search)
+        self.search_bar.returnPressedSignal.connect(self.find_next)
 
+        # Add the search bar to the layout
+        grid_layout.addWidget(self.search_bar, 0, 0)
+        
         # Create the set camera button
-        copy_text_button = QtWidgets.QPushButton("Copy")
+        copy_pixmap = QtGui.QPixmap(str(ICON_PATH / "copy.png"))
+        copy_icon = QtGui.QIcon(copy_pixmap)
+        copy_text_button = QtWidgets.QPushButton()
+        copy_text_button.setIcon(copy_icon)  # Set copy icon
         copy_text_button.clicked.connect(self.copy_output_text)
-        grid_layout.addWidget(copy_text_button, 0, 2, 1, 1)
-
+        grid_layout.addWidget(copy_text_button, 0, 1)
+        
         # Create the actor pose button
-        clear_text_button = QtWidgets.QPushButton("Clear")
-        clear_text_button.clicked.connect(self.clear_output_text)
-        grid_layout.addWidget(clear_text_button, 0, 3, 1, 1)
+        reset_pixmap = QtGui.QPixmap(str(ICON_PATH / "reset.png"))
+        reset_icon = QtGui.QIcon(reset_pixmap)
+        reset_text_button = QtWidgets.QPushButton()
+        reset_text_button.setIcon(reset_icon) # Set reset icon
+        reset_text_button.clicked.connect(self.reset_output_text)
+        grid_layout.addWidget(reset_text_button, 0, 2)
 
         grid_widget = QtWidgets.QWidget()
         grid_widget.setLayout(grid_layout)
         top_layout.addWidget(grid_widget)
         output_layout.addLayout(top_layout)
 
         # Access to the system clipboard
         self.clipboard = QtGui.QGuiApplication.clipboard()
         output_layout.addWidget(self.output_text)
         self.output.setLayout(output_layout)
         self.panel_layout.addWidget(self.output)
+        
+    def handle_search(self, text):
+        # If there's text in the search bar
+        if text: self.highlight_keyword(text)
+        # If the search bar is empty
+        else: self.clear_highlight()
+        
+    def highlight_keyword(self, keyword):
+        # Get QTextDocument from QTextEdit
+        doc = self.output_text.document()
+
+        # Default text format
+        default_format = QtGui.QTextCharFormat()
+
+        # Text format for highlighted words
+        highlight_format = QtGui.QTextCharFormat()
+        highlight_format.setBackground(QtGui.QBrush(QtGui.QColor("yellow")))
+        highlight_format.setForeground(QtGui.QBrush(QtGui.QColor("black")))
+
+        # Clear all previous highlights
+        cursor = QtGui.QTextCursor(doc)
+        cursor.beginEditBlock()
+        block_format = cursor.blockFormat()
+        cursor.select(QtGui.QTextCursor.Document)
+        cursor.setBlockFormat(block_format)
+        cursor.setCharFormat(default_format)
+        cursor.clearSelection()
+        cursor.endEditBlock()
+        cursor.setPosition(0)
+
+        # Loop through each occurrence of the keyword
+        occurrence_found = False
+        while not cursor.isNull() and not cursor.atEnd():
+            cursor = doc.find(keyword, cursor)
+            if not cursor.isNull():
+                if not occurrence_found:
+                    self.output_text.setTextCursor(cursor)
+                    occurrence_found = True
+                cursor.mergeCharFormat(highlight_format)
+                
+        if not occurrence_found:
+            cursor.setPosition(0)
+            self.output_text.setTextCursor(cursor)  # Set QTextEdit cursor to the beginning if no match found
+    
+    def find_next(self):
+        keyword = self.search_bar.text()
+        # Get the QTextCursor from the QTextEdit
+        cursor = self.output_text.textCursor()
+        # Move the cursor to the position after the current selection
+        cursor.setPosition(cursor.position() + cursor.selectionEnd() - cursor.selectionStart())
+        # Use the QTextDocument's find method to find the next occurrence
+        found_cursor = self.output_text.document().find(keyword, cursor)
+        if not found_cursor.isNull(): 
+            self.output_text.setTextCursor(found_cursor)
+
+    def clear_highlight(self):
+        doc = self.output_text.document()
+        default_format = QtGui.QTextCharFormat()
+        cursor = QtGui.QTextCursor(doc)
+        cursor.beginEditBlock()
+        block_format = cursor.blockFormat()
+        cursor.select(QtGui.QTextCursor.Document)
+        cursor.setBlockFormat(block_format)
+        cursor.setCharFormat(default_format)
+        cursor.clearSelection()
+        cursor.endEditBlock()
+        cursor.setPosition(0)
+        self.output_text.setTextCursor(cursor)  # Set QTextEdit cursor to the beginning
 
     #^ Plotter
     def create_plotter(self):
         self.frame = QtWidgets.QFrame()
         self.frame.setFixedSize(*self.window_size)
         self.plotter = CustomQtInteractor(self.frame, self)
         # self.plotter.setFixedSize(*self.window_size)
         self.signal_close.connect(self.plotter.close)
 
     def show_plot(self):
         self.plotter.enable_joystick_actor_style()
         self.plotter.enable_trackball_actor_style()
         
-        self.plotter.add_axes()
+        self.plotter.add_axes(color='white')
         self.plotter.add_camera_orientation_widget()
 
         self.plotter.show()
         self.show()
 
     def register_pose(self, pose):
         for actor_name, actor in self.mesh_store.mesh_actors.items():
             actor.user_matrix = pose
             self.plotter.add_actor(actor, pickable=True, name=actor_name)
 
     def current_pose(self, text=None, output_text=True):
         self.mesh_store.current_pose()
         if text and output_text: 
-            self.output_text.append(f"--> Current <span style='background-color:yellow; color:black;'>{text}</span> pose is:")
+            self.output_text.append(f"--> Current {text} pose is:")
             self.output_text.append(f"{self.mesh_store.transformation_matrix}")
-            self.output_text.append(f"\n************************************************************\n")
         self.register_pose(self.mesh_store.transformation_matrix)
 
     def button_actor_name_clicked(self, text, output_text=True):
         if text in self.mesh_store.mesh_actors:
             self.color_button.setText(self.mesh_store.mesh_colors[text])
             self.mesh_store.reference = text
             self.current_pose(text=text, output_text=output_text)
@@ -583,15 +671,15 @@
                 QtWidgets.QMessageBox.warning(self, 'vision6D', "Only be able to color mesh actors", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
         else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
  
     def copy_output_text(self):
         self.clipboard.setText(self.output_text.toPlainText())
         
-    def clear_output_text(self):
+    def reset_output_text(self):
         self.output_text.clear()
 
     def add_workspace(self, workspace_path='', prompt=False):
         if prompt:
             workspace_path, _ = QtWidgets.QFileDialog().getOpenFileName(None, "Open file", "", "Files (*.json)")
         if workspace_path:
             if self.workspace_path: self.clear_plot()
```

### Comparing `vision6D-0.3.0/vision6D/tools/utils.py` & `vision6D-0.3.1/vision6D/tools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 @software: Vision6D
 @file: utils.py
 @time: 2023-07-03 20:34
 @desc: the util functions for whole application
 '''
 
 import __future__
+import os
 import copy
+import json
 import logging
-
-import numpy as np
 import pathlib
 
+import numpy as np
 import pyvista as pv
 import matplotlib.pyplot as plt
 from easydict import EasyDict
 import trimesh
 from PIL import Image
 import cv2
 # import pygeodesic.geodesic as geodesic
 import vtk.util.numpy_support as vtknp
-import json
+
+from ..path import LATLON_PATH
+
 logger = logging.getLogger("vision6D")
 
 def fread(fid, _len, _type):
     if _len == 0:
         return np.empty(0)
     if _type == "int16":
         _type = np.int16
@@ -284,16 +287,16 @@
 
     rt = np.vstack((np.hstack((R, t)), np.array([0,0,0,1])))
 
     return rt
 
 def load_latitude_longitude():
     # get the latitude and longitude
-    latlon_path = pathlib.Path.cwd() / "vision6D" / "data" / "ossiclesCoordinateMapping.json" # latlon_map_path = pkg_resources.resource_filename('vision6D', 'data/ossiclesCoordinateMapping.json')
-    with open(latlon_path, "r") as f: data = json.load(f)
+    # latlon_map_path = pkg_resources.resource_filename('vision6D', 'data/ossiclesCoordinateMapping.json')
+    with open(LATLON_PATH, "r") as f: data = json.load(f)
     
     latitude = np.array(data['latitude']).reshape((len(data['latitude'])), 1)
     longitude = np.array(data['longitude']).reshape((len(data['longitude'])), 1)
     placeholder = np.zeros((len(data['longitude']), 1))
     
     # set the latlon attribute
     latlon = np.hstack((latitude, longitude, placeholder))
```

### Comparing `vision6D-0.3.0/vision6D/widgets/__init__.py` & `vision6D-0.3.1/vision6D/widgets/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 from .custom_qt_interactor import CustomQtInteractor
 from .get_text_dialog import GetTextDialog
 from .draw_mask_window import MaskWindow
 from .draw_bbox_window import BboxWindow
 from .popup_dialog import PopUpDialog
 from .video_player import VideoPlayer
 from .video_sampler import VideoSampler
+from .search_bar import SearchBar
+
 
 __all__ = [
     'CalibrationPopWindow',
     'CameraPropsInputDialog',
     'CustomQtInteractor',
     'GetTextDialog',
     'MaskWindow',
     'BboxWindow',
     'PopUpDialog',
     'VideoPlayer',
     'VideoSampler',
+    'SearchBar'
 ]
```

### Comparing `vision6D-0.3.0/vision6D/widgets/calibration_pop_window.py` & `vision6D-0.3.1/vision6D/widgets/calibration_pop_window.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/widgets/camera_props_input_dialog.py` & `vision6D-0.3.1/vision6D/widgets/camera_props_input_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/widgets/custom_qt_interactor.py` & `vision6D-0.3.1/vision6D/widgets/custom_qt_interactor.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import vtk
 from pyvistaqt import QtInteractor
 
 class CustomQtInteractor(QtInteractor):
     def __init__(self, parent=None, main_window=None):
         super().__init__(parent)
         self.main_window = main_window
+        self.set_background("4c4c4c")
         self.cell_picker = None
 
     def mousePressEvent(self, event):
         super().mousePressEvent(event)
         if event.button() == 1 or event.button() == 4:  # Left or middle mouse button
             self.press_callback(self.iren.interactor)
```

### Comparing `vision6D-0.3.0/vision6D/widgets/draw_bbox_window.py` & `vision6D-0.3.1/vision6D/widgets/draw_bbox_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,16 +111,14 @@
             rect = self.get_normalized_rect()
             painter.setPen(QPen(QColor(255, 0, 0), 2))
             painter.drawRect(rect)
 
 class BboxWindow(QtWidgets.QWidget):
     def __init__(self, image_source):
         super().__init__()
-        if isinstance(image_source, pathlib.WindowsPath) or isinstance(image_source, str):
-            image_source = np.array(PIL.Image.open(image_source), dtype='uint8')
         image = QtGui.QImage(image_source.tobytes(), image_source.shape[1], image_source.shape[0], image_source.shape[2]*image_source.shape[1], QtGui.QImage.Format_RGB888)
         pixmap = QtGui.QPixmap.fromImage(image)
         self.setFixedSize(pixmap.size())
 
         layout = QtWidgets.QVBoxLayout()
 
         #* setContentsMargins sets the width of the outside border around the layout
```

### Comparing `vision6D-0.3.0/vision6D/widgets/draw_mask_window.py` & `vision6D-0.3.1/vision6D/widgets/draw_mask_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,14 @@
             painter.setBrush(QtGui.QBrush(QtGui.QColor(0, 0, 255)))
             painter.drawEllipse(self.points.point(0), 2, 2)
             painter.drawPolyline(complete_points)
 
 class MaskWindow(QtWidgets.QWidget):
     def __init__(self, image_source):
         super().__init__()
-        if isinstance(image_source, pathlib.WindowsPath) or isinstance(image_source, str):
-            image_source = np.array(PIL.Image.open(image_source), dtype='uint8')
         image = QtGui.QImage(image_source.tobytes(), image_source.shape[1], image_source.shape[0], image_source.shape[2]*image_source.shape[1], QtGui.QImage.Format_RGB888)
         pixmap = QtGui.QPixmap.fromImage(image)
         self.setFixedSize(pixmap.size())
 
         layout = QtWidgets.QVBoxLayout()
 
         #* setContentsMargins sets the width of the outside border around the layout
```

### Comparing `vision6D-0.3.0/vision6D/widgets/get_text_dialog.py` & `vision6D-0.3.1/vision6D/widgets/get_text_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/widgets/popup_dialog.py` & `vision6D-0.3.1/vision6D/widgets/popup_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/widgets/video_player.py` & `vision6D-0.3.1/vision6D/widgets/video_player.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D/widgets/video_sampler.py` & `vision6D-0.3.1/vision6D/widgets/video_sampler.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.3.0/vision6D.egg-info/PKG-INFO` & `vision6D-0.3.1/vision6D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.3.0
+Version: 0.3.1
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
 Project-URL: Documentation, https://vision6d.readthedocs.io/en/latest/
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.3.0/vision6D.egg-info/SOURCES.txt` & `vision6D-0.3.1/vision6D.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 test/test_create_dataset.py
 test/test_projection.py
 vision6D/__init__.py
 vision6D/mainwindow.py
+vision6D/path.py
 vision6D.egg-info/PKG-INFO
 vision6D.egg-info/SOURCES.txt
 vision6D.egg-info/dependency_links.txt
 vision6D.egg-info/entry_points.txt
 vision6D.egg-info/requires.txt
 vision6D.egg-info/top_level.txt
 vision6D/components/__init__.py
@@ -32,21 +33,24 @@
 vision6D/containers/mask_container.py
 vision6D/containers/mesh_container.py
 vision6D/containers/pnp_container.py
 vision6D/containers/point_container.py
 vision6D/containers/video_container.py
 vision6D/data/ossiclesCoordinateMapping.json
 vision6D/data/style.qss
+vision6D/data/icons/copy.png
+vision6D/data/icons/reset.png
 vision6D/entry/__init__.py
 vision6D/entry/main.py
 vision6D/tools/__init__.py
 vision6D/tools/utils.py
 vision6D/widgets/__init__.py
 vision6D/widgets/calibration_pop_window.py
 vision6D/widgets/camera_props_input_dialog.py
 vision6D/widgets/custom_qt_interactor.py
 vision6D/widgets/draw_bbox_window.py
 vision6D/widgets/draw_mask_window.py
 vision6D/widgets/get_text_dialog.py
 vision6D/widgets/popup_dialog.py
+vision6D/widgets/search_bar.py
 vision6D/widgets/video_player.py
 vision6D/widgets/video_sampler.py
```

