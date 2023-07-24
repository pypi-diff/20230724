# Comparing `tmp/magnify-0.4.2.tar.gz` & `tmp/magnify-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.4.2.tar", max compression
+gzip compressed data, was "magnify-0.4.3.tar", max compression
```

## Comparing `magnify-0.4.2.tar` & `magnify-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.4.2/README.md
--rw-r--r--   0        0        0     1631 2023-07-11 23:37:15.500967 magnify-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      243 2023-07-11 23:37:20.385082 magnify-0.4.2/src/magnify/__init__.py
--rw-r--r--   0        0        0     3692 2023-07-11 23:24:08.976685 magnify-0.4.2/src/magnify/filter.py
--rw-r--r--   0        0        0    26135 2023-07-11 23:36:11.587453 magnify-0.4.2/src/magnify/find.py
--rw-r--r--   0        0        0     7516 2023-07-07 19:57:46.832323 magnify-0.4.2/src/magnify/identify.py
--rw-r--r--   0        0        0     1278 2023-07-07 22:23:16.867076 magnify-0.4.2/src/magnify/pipeline.py
--rw-r--r--   0        0        0      318 2023-07-07 19:04:45.491234 magnify-0.4.2/src/magnify/plot/__init__.py
--rw-r--r--   0        0        0     2345 2023-07-07 19:04:45.527235 magnify-0.4.2/src/magnify/plot/image.py
--rw-r--r--   0        0        0     1856 2023-07-07 19:04:45.511235 magnify-0.4.2/src/magnify/plot/ndplot.py
--rw-r--r--   0        0        0     2501 2023-07-07 19:04:45.551236 magnify-0.4.2/src/magnify/plot/relation.py
--rw-r--r--   0        0        0      694 2023-07-07 19:04:45.503235 magnify-0.4.2/src/magnify/plot/style.py
--rw-r--r--   0        0        0      446 2023-07-11 23:37:04.000697 magnify-0.4.2/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1180 2023-07-07 19:09:00.448530 magnify-0.4.2/src/magnify/preprocess.py
--rw-r--r--   0        0        0    14930 2023-07-11 23:23:45.940234 magnify-0.4.2/src/magnify/reader.py
--rw-r--r--   0        0        0     2926 2023-07-07 23:43:18.929994 magnify-0.4.2/src/magnify/registry.py
--rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.4.2/src/magnify/stitch.py
--rw-r--r--   0        0        0     2639 2023-07-07 19:50:21.414864 magnify-0.4.2/src/magnify/utils.py
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 magnify-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     6810 2023-07-12 00:26:39.628258 magnify-0.4.3/README.md
+-rw-r--r--   0        0        0     1631 2023-07-24 20:34:49.455097 magnify-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-07-24 20:36:09.904739 magnify-0.4.3/src/magnify/__init__.py
+-rw-r--r--   0        0        0     3692 2023-07-11 23:24:08.976685 magnify-0.4.3/src/magnify/filter.py
+-rw-r--r--   0        0        0    26310 2023-07-21 22:41:35.379539 magnify-0.4.3/src/magnify/find.py
+-rw-r--r--   0        0        0     7457 2023-07-21 22:33:38.454373 magnify-0.4.3/src/magnify/identify.py
+-rw-r--r--   0        0        0     2193 2023-07-24 20:33:50.749884 magnify-0.4.3/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      318 2023-07-07 19:04:45.491234 magnify-0.4.3/src/magnify/plot/__init__.py
+-rw-r--r--   0        0        0     3834 2023-07-24 19:31:38.438103 magnify-0.4.3/src/magnify/plot/image.py
+-rw-r--r--   0        0        0     1812 2023-07-21 22:14:48.625892 magnify-0.4.3/src/magnify/plot/ndplot.py
+-rw-r--r--   0        0        0     2501 2023-07-07 19:04:45.551236 magnify-0.4.3/src/magnify/plot/relation.py
+-rw-r--r--   0        0        0      694 2023-07-07 19:04:45.503235 magnify-0.4.3/src/magnify/plot/style.py
+-rw-r--r--   0        0        0      482 2023-07-12 00:24:50.913763 magnify-0.4.3/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1180 2023-07-07 19:09:00.448530 magnify-0.4.3/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    14930 2023-07-11 23:23:45.940234 magnify-0.4.3/src/magnify/reader.py
+-rw-r--r--   0        0        0     2745 2023-07-24 20:31:13.646550 magnify-0.4.3/src/magnify/registry.py
+-rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.4.3/src/magnify/stitch.py
+-rw-r--r--   0        0        0     1792 2023-07-21 22:30:51.702747 magnify-0.4.3/src/magnify/utils.py
+-rw-r--r--   0        0        0     8005 1970-01-01 00:00:00.000000 magnify-0.4.3/PKG-INFO
```

### Comparing `magnify-0.4.2/pyproject.toml` & `magnify-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.4.2"
+version = "0.4.3"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
```

### Comparing `magnify-0.4.2/src/magnify/filter.py` & `magnify-0.4.3/src/magnify/filter.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.2/src/magnify/find.py` & `magnify-0.4.3/src/magnify/find.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,15 @@
                 assay.x[..., t] = assay.x[..., t - 1]
                 assay.y[..., t] = assay.y[..., t - 1]
 
             # Compute the roi, foreground and background masks for all buttons.
             assay.roi[:, :, :, t], assay.fg[:, :, :, t], assay.bg[:, :, :, t] = self.find_rois(
                 images, t, do_search, assay
             )
-        assay = assay.stack(mark=("mark_row", "mark_col"), create_index=True).transpose(
-            "mark", ...
-        )
+        assay = assay.stack(mark=("mark_row", "mark_col"), create_index=True).transpose("mark", ...)
 
         return assay
 
     def find_centers(self, images: xr.DataArray, assay: xr.Dataset):
         points = np.empty((0, 2))
         min_button_dist = round(min(self.row_dist, self.col_dist) / 2)
         if min_button_dist % 2 == 0:
@@ -499,14 +497,20 @@
             # Set the background to be everything else in the region,
             # which could include other beads.
             bgs[i] = ~fgs[i]
 
         assay.fg[:] = fgs
         assay.bg[:] = bgs
         assay.roi[:] = rois
+        assay = assay.assign_coords(
+            valid=(
+                ("mark", "time"),
+                np.ones((assay.sizes["mark"], assay.sizes["time"]), dtype=bool),
+            ),
+        )
         return assay
 
     @registry.components.register("find_beads")
     def make(
         min_bead_radius: int = 5,
         max_bead_radius: int = 25,
         roi_length: int = 61,
```

### Comparing `magnify-0.4.2/src/magnify/identify.py` & `magnify-0.4.3/src/magnify/identify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import re
 
 import numpy as np
 import pandas as pd
 import scipy
 import sklearn.mixture
 
@@ -166,11 +167,10 @@
         proportions = np.sum(probs, axis=0) / X.shape[0]
 
     # Assign each bead a code based on the clustering we just found.
     clust = np.argmax(probs, axis=1)
     tag_names.append("outlier")
     assay = assay.assign_coords(
         tag=("mark", np.array(tag_names)[clust]),
-        valid=(("mark", "time"), np.ones((len(tag_names), assay.sizes["time"]), dtype=bool)),
     )
 
     return assay
```

### Comparing `magnify-0.4.2/src/magnify/plot/ndplot.py` & `magnify-0.4.3/src/magnify/plot/ndplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 def ndplot(
     assay,
     plot_function,
     grid: str | list[str] | None = None,
     slider: str | list[str] | None = None,
     **kwargs,
 ):
-    assay = utils.to_explicit_coords(assay)
     grid = [dim for dim in utils.to_list(grid) if dim in assay.indexes]
     slider = [dim for dim in utils.to_list(slider) if dim in assay.indexes]
 
     def to_holomap(subassay):
         if slider:
             slider_coords = [subassay[dim].values for dim in slider]
             return hv.HoloMap(
```

### Comparing `magnify-0.4.2/src/magnify/plot/relation.py` & `magnify-0.4.3/src/magnify/plot/relation.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.2/src/magnify/plot/style.py` & `magnify-0.4.3/src/magnify/plot/style.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.2/src/magnify/preprocess.py` & `magnify-0.4.3/src/magnify/preprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.2/src/magnify/reader.py` & `magnify-0.4.3/src/magnify/reader.py`

 * *Files identical despite different names*

### Comparing `magnify-0.4.2/src/magnify/registry.py` & `magnify-0.4.3/src/magnify/registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,17 +32,15 @@
 def ps_chip(**kwargs):
     # Button centers are apart 375um vertically and 655um horizontally.
     # Assuming a 4x objective and 2x2 binning each pixel is 3.22um.
     defaults = confection.Config(dict(row_dist=375 / 3.22, col_dist=655 / 3.22))
     config = defaults.merge(confection.Config(kwargs))
     pipe = Pipeline("read", config=config)
     pipe.add_pipe("identify_buttons")
-    pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("stitch")
-    pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("find_buttons")
     pipe.add_pipe("filter_expression")
     pipe.add_pipe("filter_nonround")
     pipe.add_pipe("filter_leaky")
     pipe.add_pipe("drop")
 
     return pipe
@@ -66,33 +64,30 @@
 
     return pipe
 
 
 def mrbles(**kwargs):
     pipe = Pipeline("read", config=kwargs)
     pipe.add_pipe("flatfield_correct")
-    pipe.add_pipe("vertical_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("find_beads")
     pipe.add_pipe("identify_mrbles")
     pipe.add_pipe("drop")
 
     return pipe
 
 
 def beads(**kwargs):
     pipe = Pipeline("read", config=kwargs)
     pipe.add_pipe("flatfield_correct")
-    pipe.add_pipe("vertical_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("find_beads")
     pipe.add_pipe("drop")
 
     return pipe
 
 
 def image(**kwargs):
     pipe = Pipeline("read", config=kwargs)
-    pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("drop")
     return pipe
```

### Comparing `magnify-0.4.2/src/magnify/stitch.py` & `magnify-0.4.3/src/magnify/stitch.py`

 * *Files identical despite different names*

