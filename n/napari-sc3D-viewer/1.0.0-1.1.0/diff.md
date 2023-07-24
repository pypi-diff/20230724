# Comparing `tmp/napari-sc3D-viewer-1.0.0.tar.gz` & `tmp/napari-sc3D-viewer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sc3D-viewer-1.0.0.tar", last modified: Thu Jul  6 09:09:38 2023, max compression
+gzip compressed data, was "napari-sc3D-viewer-1.1.0.tar", last modified: Mon Jul 24 07:48:03 2023, max compression
```

## Comparing `napari-sc3D-viewer-1.0.0.tar` & `napari-sc3D-viewer-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.538357 napari-sc3D-viewer-1.0.0/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1079 2023-05-17 08:01:30.000000 napari-sc3D-viewer-1.0.0/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)       96 2022-05-02 08:05:43.000000 napari-sc3D-viewer-1.0.0/MANIFEST.in
--rw-r--r--   0 leo.guignard   (501) staff       (20)    11999 2023-07-06 09:09:38.538450 napari-sc3D-viewer-1.0.0/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)    10720 2023-05-17 08:13:17.000000 napari-sc3D-viewer-1.0.0/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      727 2023-07-06 09:09:17.000000 napari-sc3D-viewer-1.0.0/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1834 2023-07-06 09:09:38.538844 napari-sc3D-viewer-1.0.0/setup.cfg
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.535232 napari-sc3D-viewer-1.0.0/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.537168 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)    11999 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      688 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       70 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/entry_points.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)      112 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       19 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.538051 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/
--rw-r--r--   0 leo.guignard   (501) staff       (20)      102 2023-07-06 09:09:17.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    41446 2023-07-06 09:07:36.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_display_embryo.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.538267 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_tests/
--rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-05-02 08:05:43.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_tests/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     5051 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_tests/test_widget.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    15701 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_umap_selection.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1175 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_utils.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     5939 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_widget_load.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    12359 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_widget_register.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      562 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/napari.yaml
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:03.119831 napari-sc3D-viewer-1.1.0/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1079 2023-05-17 08:01:30.000000 napari-sc3D-viewer-1.1.0/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       96 2022-05-02 08:05:43.000000 napari-sc3D-viewer-1.1.0/MANIFEST.in
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    11999 2023-07-24 07:48:03.119913 napari-sc3D-viewer-1.1.0/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    10720 2023-05-17 08:13:17.000000 napari-sc3D-viewer-1.1.0/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      727 2023-07-24 07:47:53.000000 napari-sc3D-viewer-1.1.0/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1834 2023-07-24 07:48:03.120303 napari-sc3D-viewer-1.1.0/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:03.116655 napari-sc3D-viewer-1.1.0/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:03.118370 napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    11999 2023-07-24 07:48:03.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      688 2023-07-24 07:48:03.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-07-24 07:48:03.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       70 2023-07-24 07:48:03.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      112 2023-07-24 07:48:03.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       19 2023-07-24 07:48:03.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:03.119245 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      102 2023-07-24 07:47:53.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    42949 2023-07-20 10:23:28.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_display_embryo.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-24 07:48:03.119718 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_tests/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-05-02 08:05:43.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_tests/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     5051 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_tests/test_widget.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    15701 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_umap_selection.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1175 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_utils.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     5939 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_widget_load.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    12359 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_widget_register.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      562 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/napari.yaml
```

### Comparing `napari-sc3D-viewer-1.0.0/LICENSE` & `napari-sc3D-viewer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-1.0.0/PKG-INFO` & `napari-sc3D-viewer-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sc3D-viewer
-Version: 1.0.0
+Version: 1.1.0
 Summary: A plugin to visualize 3D single cell omics
 Home-page: https://github.com/GuignardLab/napari-sc3D-viewer
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/napari-sc3D-viewer/issues
 Project-URL: Documentation, https://github.com/GuignardLab/napari-sc3D-viewer#README.md
```

### Comparing `napari-sc3D-viewer-1.0.0/README.md` & `napari-sc3D-viewer-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-1.0.0/pyproject.toml` & `napari-sc3D-viewer-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 line-length = 79
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `napari-sc3D-viewer-1.0.0/setup.cfg` & `napari-sc3D-viewer-1.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-sc3D-viewer
-version = 1.0.0
+version = 1.1.0
 author = Leo Guignard
 author_email = leo.guignard@univ-amu.fr
 url = https://github.com/GuignardLab/napari-sc3D-viewer
 license = MIT
 description = A plugin to visualize 3D single cell omics
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/PKG-INFO` & `napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sc3D-viewer
-Version: 1.0.0
+Version: 1.1.0
 Summary: A plugin to visualize 3D single cell omics
 Home-page: https://github.com/GuignardLab/napari-sc3D-viewer
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/napari-sc3D-viewer/issues
 Project-URL: Documentation, https://github.com/GuignardLab/napari-sc3D-viewer#README.md
```

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/SOURCES.txt` & `napari-sc3D-viewer-1.1.0/src/napari_sc3D_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_display_embryo.py` & `napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_display_embryo.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     FigureCanvasQTAgg as FigureCanvas,
 )
 from matplotlib.backends.backend_qt5agg import (
     NavigationToolbar2QT as NavigationToolbar,
 )
 from matplotlib import cm, colors
 import numpy as np
+from random import sample
 
 try:
     from pyvista import PolyData
 
     pyvista = True
 except Exception as e:
     print(
@@ -190,24 +191,55 @@
             error_points_selection(show=self.show)
             return
 
         # If necessary, change the color of the cells
         if (
             points.metadata["gene"] is not None
             or points.metadata["2genes"] is not None
+            or self.color_map_tissues != self.original_color_map_tissues
         ):
+            self.color_map_tissues = self.original_color_map_tissues.copy()
             points.face_color = [
                 self.color_map_tissues[self.embryo.tissue[c]]
                 for c in points.properties["cells"]
             ]
             points.face_color_mode = "direct"
             points.metadata["gene"] = None
             points.metadata["2genes"] = None
         points.refresh()
 
+    def recolor_tissues(self):
+        # Get the points and make sure they are correctly selected
+        points = self.viewer.layers.selection.active
+        if points is None or points.as_layer_data_tuple()[-1] != "points":
+            error_points_selection(show=self.show)
+            return
+
+        # Change the color of the cells
+        tissues = set(
+            [
+                self.embryo.tissue[c]
+                for c in points.properties["cells"][points.shown]
+            ]
+        )
+        nb_tissues = len(tissues)+1
+        subset_map = {t: i+1 for i, t in enumerate(sample(tissues, len(tissues)))}
+        self.color_map_tissues = {
+            t: cm.tab20(subset_map.get(t, 0) / nb_tissues)
+            for t in self.embryo.all_tissues
+        }
+        points.face_color = [
+            self.color_map_tissues[self.embryo.tissue[c]]
+            for c in points.properties["cells"]
+        ]
+        points.face_color_mode = "direct"
+        points.metadata["gene"] = None
+        points.metadata["2genes"] = None
+        points.refresh()
+
     def select_tissues(self):
         """
         Display a set of tissues according to user selection
         """
         # Get the points and make sure they are correctly selected
         points = self.viewer.layers.selection.active
         if points is None or points.as_layer_data_tuple()[-1] != "points":
@@ -578,14 +610,18 @@
         run_select = widgets.FunctionGui(
             self.select_tissues, call_button="Select Tissues"
         )
         run_tissues = widgets.FunctionGui(
             self.show_tissues, call_button="Cell type colouring"
         )
 
+        recolor_tissues = widgets.FunctionGui(
+            self.recolor_tissues, call_button="Recolour tissues"
+        )
+
         # Coloring by tissues
         run_legend = widgets.FunctionGui(
             self.disp_legend, call_button="Display legend"
         )
 
         select_container = widgets.Container(
             widgets=[self.select_tissues_choices, run_select], labels=False
@@ -593,15 +629,15 @@
         display_container = widgets.Container(
             widgets=[run_tissues, run_legend],
             layout="horizontal",
             labels=False,
         )
         display_container.native.layout().addStretch(1)
         tissue_container = widgets.Container(
-            widgets=[select_container, display_container], labels=False
+            widgets=[select_container, recolor_tissues, display_container], labels=False
         )
         tissue_container.native.layout().addStretch(1)
         return tissue_container
 
     def build_surf_container(self):
         """
         Function that builds the qt container to build the surfaces
@@ -1029,14 +1065,15 @@
         properties["gene"] = [0 for _ in cells]
         if 0 < len(self.embryo.all_tissues.difference(self.color_map_tissues)):
             nb_tissues = len(self.embryo.all_tissues)
             self.color_map_tissues = {
                 v: cm.tab20(i / nb_tissues)
                 for i, v in enumerate(self.embryo.all_tissues)
             }
+        self.original_color_map_tissues = self.color_map_tissues.copy()
         colors_rgb = [
             self.color_map_tissues.get(self.embryo.tissue[c], [0, 0, 0])
             for c in cells
         ]
 
         self.viewer.dims.ndisplay = 3
         points = self.viewer.add_points(
@@ -1048,14 +1085,15 @@
             size=15,
         )
 
         self.all_tissues = [
             self.embryo.corres_tissue.get(t, f"{t}")
             for t in self.embryo.all_tissues
         ]
+        self.all_tissues = sorted(self.all_tissues)
 
         tissue_container = self.build_tissue_selection()
         surf_container = self.build_surf_container()
         self.tab1 = QTabWidget()
         self.tab1.addTab(tissue_container.native, "Tissues")
         last_tab = self.tab1.addTab(surf_container.native, "Surfaces")
         self.tab1.nb_tabs = last_tab
```

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_tests/test_widget.py` & `napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_umap_selection.py` & `napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_umap_selection.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_utils.py` & `napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_widget_load.py` & `napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_widget_load.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_widget_register.py` & `napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/_widget_register.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/napari.yaml` & `napari-sc3D-viewer-1.1.0/src/napari_sc3d_viewer/napari.yaml`

 * *Files identical despite different names*

