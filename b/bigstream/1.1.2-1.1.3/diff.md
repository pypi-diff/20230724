# Comparing `tmp/bigstream-1.1.2.tar.gz` & `tmp/bigstream-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigstream-1.1.2.tar", last modified: Thu Feb 23 15:24:00 2023, max compression
+gzip compressed data, was "bigstream-1.1.3.tar", last modified: Mon Jul 24 18:46:25 2023, max compression
```

## Comparing `bigstream-1.1.2.tar` & `bigstream-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 fleishmang (61373) scicompsoft (93099)        0 2023-02-23 15:24:00.598148 bigstream-1.1.2/
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.2/LICENSE.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      293 2023-02-23 15:24:00.596679 bigstream-1.1.2/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     8682 2023-01-09 21:39:42.000000 bigstream-1.1.2/README.md
-drwxr-xr-x   0 fleishmang (61373) scicompsoft (93099)        0 2023-02-23 15:24:00.575155 bigstream-1.1.2/bigstream/
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)        5 2021-11-27 21:30:14.000000 bigstream-1.1.2/bigstream/__init__.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)    37881 2023-02-22 18:08:37.000000 bigstream-1.1.2/bigstream/align.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     8325 2022-12-08 13:54:28.000000 bigstream-1.1.2/bigstream/application_pipelines.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     7732 2022-12-05 17:16:08.000000 bigstream-1.1.2/bigstream/configure_irm.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     4037 2023-01-09 15:33:05.000000 bigstream-1.1.2/bigstream/features.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     6090 2023-01-09 14:15:26.000000 bigstream-1.1.2/bigstream/level_set.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)     3347 2023-01-09 15:43:02.000000 bigstream-1.1.2/bigstream/metrics.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)    16816 2023-02-23 15:21:28.000000 bigstream-1.1.2/bigstream/motion_correct.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)    22003 2023-02-23 15:17:02.000000 bigstream-1.1.2/bigstream/piecewise_align.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)    17210 2023-01-11 22:28:38.000000 bigstream-1.1.2/bigstream/piecewise_transform.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)    12953 2023-02-23 13:58:04.000000 bigstream-1.1.2/bigstream/transform.py
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)    21134 2023-02-22 21:48:46.000000 bigstream-1.1.2/bigstream/utility.py
-drwxr-xr-x   0 fleishmang (61373) scicompsoft (93099)        0 2023-02-23 15:24:00.592580 bigstream-1.1.2/bigstream.egg-info/
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      293 2023-02-23 15:23:59.000000 bigstream-1.1.2/bigstream.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      497 2023-02-23 15:24:00.000000 bigstream-1.1.2/bigstream.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)        1 2023-02-23 15:23:59.000000 bigstream-1.1.2/bigstream.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      256 2023-02-23 15:23:59.000000 bigstream-1.1.2/bigstream.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)       10 2023-02-23 15:24:00.000000 bigstream-1.1.2/bigstream.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)       38 2023-02-23 15:24:00.598988 bigstream-1.1.2/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicompsoft (93099)      806 2023-02-23 15:23:51.000000 bigstream-1.1.2/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-24 18:46:15.361060 bigstream-1.1.3/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1083 2023-01-03 22:45:33.000000 bigstream-1.1.3/LICENSE.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-24 18:46:15.359979 bigstream-1.1.3/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.1.3/README.md
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-24 18:46:15.336662 bigstream-1.1.3/bigstream/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    40044 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8325 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/application_pipelines.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7732 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/configure_irm.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     4460 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/features.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6090 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/level_set.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7210 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/metrics.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16816 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/motion_correct.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22137 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/piecewise_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17210 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/piecewise_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16456 2023-07-21 16:14:18.000000 bigstream-1.1.3/bigstream/stitch.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    14133 2023-07-11 16:34:08.000000 bigstream-1.1.3/bigstream/transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21225 2023-07-11 20:23:49.000000 bigstream-1.1.3/bigstream/utility.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2023-07-24 18:46:15.355776 bigstream-1.1.3/bigstream.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      265 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      517 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      268 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2023-07-24 18:46:15.000000 bigstream-1.1.3/bigstream.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2023-07-24 18:46:15.362742 bigstream-1.1.3/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      829 2023-07-24 18:43:59.000000 bigstream-1.1.3/setup.py
```

### Comparing `bigstream-1.1.2/LICENSE.txt` & `bigstream-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.2/README.md` & `bigstream-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BigStream
 ---
 
 ![warp](resources/warp_interpolation.gif)
+![certificate](resources/rnrexm_certificate.png)
 
 BigStream is a library of tools for 3D registration including images too large to fit into memory and/or too large to register in a single (multi-threaded) process. BigStream can automate chunking of the alignment problem into overlapping blocks, distributes the blocks to independent workers running in parallel, and stitches the results into a single smooth transform. BigStream includes global affine, piecewise affine, and piecewise deformable alignments; it also includes tools for finding feature points of interest, applying transforms, and inverting transforms. The tools can be used individually to construct custom workflows, but pipelines are also provided for specific alignment problems.
 
 ## Installation
 ---
 > pip install bigstream
```

### Comparing `bigstream-1.1.2/bigstream/align.py` & `bigstream-1.1.3/bigstream/align.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 import SimpleITK as sitk
 import bigstream.utility as ut
 from bigstream.configure_irm import configure_irm
 from bigstream.transform import apply_transform, compose_transform_list
 from bigstream.metrics import patch_mutual_information
 from bigstream import features
+from scipy.spatial import cKDTree
 import cv2
 
 # TODO: bug! fix_spacing is overwritten after resolve_sampling is called
 #       but downstream functions rely on it having the original value
 
 
 def resolve_sampling(
@@ -70,20 +71,25 @@
 
 
 def feature_point_ransac_affine_align(
     fix, mov,
     fix_spacing,
     mov_spacing,
     blob_sizes,
+    alignment_spacing=None,
     num_sigma_max=15,
     cc_radius=12,
     nspots=5000,
     match_threshold=0.7,
+    max_spot_match_distance=None,
     align_threshold=2.0,
-    diagonal_constraint=0.75,
+    diagonal_constraint=0.25,
+    fix_spot_detection_kwargs={},
+    mov_spot_detection_kwargs={},
+    ransac_affine_kwargs={},
     fix_spots=None,
     mov_spots=None,
     fix_mask=None,
     mov_mask=None,
     fix_origin=None,
     mov_origin=None,
     static_transform_list=[],
@@ -170,81 +176,138 @@
     affine_matrix : 2d array 4x4
         An affine matrix matching the moving image to the fixed image
     """
 
     # establish default
     if default is None: default = np.eye(fix.ndim + 1)
 
+    # skip sample and determine mask spacings
+    X = resolve_sampling(
+        fix, mov,
+        fix_mask, mov_mask,
+        fix_spacing, mov_spacing,
+        alignment_spacing,
+    )
+    fix = X[0]
+    mov = X[1]
+    fix_mask = X[2]
+    mov_mask = X[3]
+    fix_spacing = X[4]
+    mov_spacing = X[5]
+    fix_mask_spacing = X[6]
+    mov_mask_spacing = X[7]
+
     # apply static transforms
     if static_transform_list:
         mov = apply_transform(
             fix, mov, fix_spacing, mov_spacing,
             transform_list=static_transform_list,
             fix_origin=fix_origin,
             mov_origin=mov_origin,
         )
+        if mov_mask is not None:
+            mov_mask = apply_transform(
+                fix.astype(mov_mask.dtype), mov_mask, fix_spacing, mov_spacing,
+                transform_list=static_transform_list,
+                fix_origin=fix_origin, 
+                mov_origin=mov_origin,
+                interpolate_with_nn=True,
+            )
+        mov_spacing = fix_spacing
 
-    # get spots
+    # get fix spots
+    print('computing fixed spots', flush=True)
     if fix_spots is None:
+        fix_kwargs = {
+            'num_sigma':min(blob_sizes[1] - blob_sizes[0], num_sigma_max),
+            'exclude_border':cc_radius,
+            'mask':fix_mask,
+        }
+        fix_kwargs = {**fix_kwargs, **fix_spot_detection_kwargs}
         fix_spots = features.blob_detection(
             fix, blob_sizes[0], blob_sizes[1],
-            num_sigma=min(blob_sizes[1]-blob_sizes[0], num_sigma_max),
-            exclude_border=cc_radius,
+            **fix_kwargs,
         )
+    print(f'found {len(fix_spots)} fixed spots')
+    if len(fix_spots) < 100:
+        print('insufficient fixed spots found, returning default', flush=True)
+        return default
+
+    # get mov spots
+    print('computing moving spots', flush=True)
     if mov_spots is None:
+        mov_kwargs = {
+            'num_sigma':min(blob_sizes[1] - blob_sizes[0], num_sigma_max),
+            'exclude_border':cc_radius,
+            'mask':mov_mask,
+        }
+        mov_kwargs = {**mov_kwargs, **mov_spot_detection_kwargs}
         mov_spots = features.blob_detection(
             mov, blob_sizes[0], blob_sizes[1],
-            num_sigma=min(blob_sizes[1]-blob_sizes[0], num_sigma_max),
-            exclude_border=cc_radius,
+            **mov_kwargs,
         )
-
-    # TODO: implement masking, remove spots not in foreground
+    print(f'found {len(mov_spots)} moving spots')
+    if len(mov_spots) < 100:
+        print('insufficient moving spots found, returning default', flush=True)
+        return default
 
     # sort
+    print('sorting spots', flush=True)
     sort_idx = np.argsort(fix_spots[:, 3])[::-1]
     fix_spots = fix_spots[sort_idx, :3][:nspots]
     sort_idx = np.argsort(mov_spots[:, 3])[::-1]
     mov_spots = mov_spots[sort_idx, :3][:nspots]
 
     # get contexts
+    print('extracting contexts', flush=True)
     fix_spot_contexts = features.get_contexts(fix, fix_spots, cc_radius)
     mov_spot_contexts = features.get_contexts(mov, mov_spots, cc_radius)
 
     # convert to physical units
     fix_spots = fix_spots * fix_spacing
     mov_spots = mov_spots * mov_spacing
 
-    # get point correspondences
+    # get pairwise correlations
+    print('computing pairwise correlations', flush=True)
     correlations = features.pairwise_correlation(
         fix_spot_contexts, mov_spot_contexts,
     )
+
+    # apply distance filter
+    if max_spot_match_distance is not None:
+        fix_kdtree = cKDTree(fix_spots)
+        valid_pairs = fix_kdtree.query_ball_tree(
+            cKDTree(mov_spots), max_spot_match_distance,
+        )
+        for iii, fancy_index in enumerate(valid_pairs):
+            correlations[iii, fancy_index] += 1
+        match_threshold += 1
+
+    # get matching points
     fix_spots, mov_spots = features.match_points(
         fix_spots, mov_spots,
         correlations, match_threshold,
     )
-
-    # check spot counts
-    if fix_spots.shape[0] < 50:
-        print('Fewer than 50 spots found in fixed image, returning default')
-        return default
-    if mov_spots.shape[0] < 50:
-        print('Fewer than 50 spots found in moving image, returning default')
+    print(f'{len(fix_spots)} matched spots')
+    if len(fix_spots) < 50 or len(mov_spots) < 50:
+        print('insufficient point matches found, returning default', flush=True)
         return default
 
     # align
+    print('aligning', flush=True)
     r, Aff, inline = cv2.estimateAffine3D(
         fix_spots, mov_spots,
         ransacThreshold=align_threshold,
         confidence=0.999,
         **kwargs,
     )
 
     # ensure affine is sensible
-    if np.any( np.diag(Aff) < diagonal_constraint ):
-        print("Degenerate affine produced, returning default")
+    if np.any( np.abs(np.diag(Aff) - 1) > diagonal_constraint ):
+        print("Degenerate affine produced, returning default", flush=True)
         return default
 
     # augment to 4x4 matrix and return
     affine = np.eye(4)
     affine[:3, :] = Aff
     return affine
```

### Comparing `bigstream-1.1.2/bigstream/application_pipelines.py` & `bigstream-1.1.3/bigstream/application_pipelines.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.2/bigstream/configure_irm.py` & `bigstream-1.1.3/bigstream/configure_irm.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.2/bigstream/features.py` & `bigstream-1.1.3/bigstream/features.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import numpy as np
-from fishspot.filter import white_tophat
+from fishspot.filter import white_tophat, apply_foreground_mask
 from fishspot.detect import detect_spots_log
+from scipy.stats.mstats import winsorize
 
 
 def blob_detection(
     image,
     min_blob_radius,
     max_blob_radius,
+    winsorize_limits=None,
+    background_subtract=False,
+    mask=None,
     **kwargs,
 ):
     """
     Find discrete blobs in an image
 
     Parameters
     ----------
@@ -27,21 +31,26 @@
     -------
     blob_coordinates_and_intensities : nd-array Nx4
         The first three columns of the array are the coordinates of the
         detected blobs. The last column is the image intensity at the
         detected coordinate location.
     """
 
-    wth = white_tophat(image, max_blob_radius)
+    processed_image = np.copy(image)
+    if winsorize_limits is not None:
+        processed_image = winsorize(processed_image, limits=winsorize_limits)
+    if background_subtract:
+        processed_image = white_tophat(processed_image, max_blob_radius)
     spots = detect_spots_log(
-        wth,
+        processed_image,
         min_blob_radius,
         max_blob_radius,
         **kwargs,
     ).astype(int)
+    if mask is not None: spots = apply_foreground_mask(spots, mask)
     intensities = image[spots[:, 0], spots[:, 1], spots[:, 2]]
     return np.hstack((spots[:, :3], intensities[..., None]))
 
 
 def get_contexts(image, coords, radius):
     """
     Get neighborhoods of a set of coordinates
```

### Comparing `bigstream-1.1.2/bigstream/level_set.py` & `bigstream-1.1.3/bigstream/level_set.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.2/bigstream/motion_correct.py` & `bigstream-1.1.3/bigstream/motion_correct.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.2/bigstream/piecewise_align.py` & `bigstream-1.1.3/bigstream/piecewise_align.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from itertools import product
 from scipy.interpolate import LinearNDInterpolator
 from dask.distributed import as_completed, wait
 from ClusterWrap.decorator import cluster
 import bigstream.utility as ut
 from bigstream.align import alignment_pipeline
-from bigstream.transform import apply_transform
+from bigstream.transform import apply_transform, compose_transform_list
 from bigstream.transform import apply_transform_to_coordinates
 from bigstream.transform import compose_transforms
 
 
 @cluster
 def distributed_piecewise_alignment_pipeline(
     fix,
@@ -135,29 +135,32 @@
         the displacement vector.
     """
 
     # temporary file paths and create zarr images
     temporary_directory = tempfile.TemporaryDirectory(
         prefix='.', dir=temporary_directory or os.getcwd(),
     )
+    zarr_blocks = [128,] * fix.ndim
     fix_zarr_path = temporary_directory.name + '/fix.zarr'
     mov_zarr_path = temporary_directory.name + '/mov.zarr'
     fix_mask_zarr_path = temporary_directory.name + '/fix_mask.zarr'
     mov_mask_zarr_path = temporary_directory.name + '/mov_mask.zarr'
-    fix_zarr = ut.numpy_to_zarr(fix, blocksize, fix_zarr_path)
-    mov_zarr = ut.numpy_to_zarr(mov, blocksize, mov_zarr_path)
-    if fix_mask is not None: fix_mask_zarr = ut.numpy_to_zarr(fix_mask, blocksize, fix_mask_zarr_path)
-    if mov_mask is not None: mov_mask_zarr = ut.numpy_to_zarr(mov_mask, blocksize, mov_mask_zarr_path)
+    fix_zarr = ut.numpy_to_zarr(fix, zarr_blocks, fix_zarr_path)
+    mov_zarr = ut.numpy_to_zarr(mov, zarr_blocks, mov_zarr_path)
+    fix_mask_zarr = None
+    if fix_mask is not None: fix_mask_zarr = ut.numpy_to_zarr(fix_mask, zarr_blocks, fix_mask_zarr_path)
+    mov_mask_zarr = None
+    if mov_mask is not None: mov_mask_zarr = ut.numpy_to_zarr(mov_mask, zarr_blocks, mov_mask_zarr_path)
 
     # zarr files for initial deformations
     new_list = []
     for iii, transform in enumerate(static_transform_list):
         if transform.shape != (4, 4) and len(transform.shape) != 1:
             path = temporary_directory.name + f'/deform{iii}.zarr'
-            transform = ut.numpy_to_zarr(transform, tuple(blocksize) + (transform.shape[-1],), path)
+            transform = ut.numpy_to_zarr(transform, tuple(zarr_blocks) + (transform.shape[-1],), path)
         new_list.append(transform)
     static_transform_list = new_list
 
     # zarr file for output (if write_path is given)
     if write_path:
         output_transform = ut.create_zarr(
             write_path,
@@ -200,14 +203,15 @@
         neighbor_flags = {tuple(o): tuple(index + o) in indices for o in neighbor_offsets}
         new_indices.append((index, coords, neighbor_flags))
     indices = new_indices
 
     # establish all keyword arguments
     steps = [(a, {**kwargs, **b}) for a, b in steps]
 
+
     # closure for alignment pipeline
     def align_single_block(
         indices,
         static_transform_list,
     ):
 
         # print some feedback
@@ -254,23 +258,24 @@
         mov_start = np.min(mov_block_coords, axis=0)
         mov_stop = np.max(mov_block_coords, axis=0)
         mov_start = np.maximum(0, mov_start)
         mov_stop = np.minimum(np.array(mov_zarr.shape)-1, mov_stop)
         mov_slices = tuple(slice(a, b) for a, b in zip(mov_start, mov_stop))
         mov = mov_zarr[mov_slices]
 
+        # XXX if input masks are zarr arrays this doesn't work, nothing at paths
         # read masks
         fix_mask, mov_mask = None, None
-        if os.path.isdir(fix_mask_zarr_path):
+        if fix_mask_zarr is not None:
             ratio = np.array(fix_mask_zarr.shape) / fix_zarr.shape
             start = np.round( ratio * fix_block_coords[0] ).astype(int)
             stop = np.round( ratio * (fix_block_coords[-1] + 1) ).astype(int)
             fix_mask_slices = tuple(slice(a, b) for a, b in zip(start, stop))
             fix_mask = fix_mask_zarr[fix_mask_slices]
-        if os.path.isdir(mov_mask_zarr_path):
+        if mov_mask_zarr is not None:
             ratio = np.array(mov_mask_zarr.shape) / mov_zarr.shape
             start = np.round( ratio * mov_start ).astype(int)
             stop = np.round( ratio * mov_stop ).astype(int)
             mov_mask_slices = tuple(slice(a, b) for a, b in zip(start, stop))
             mov_mask = mov_mask_zarr[mov_mask_slices]
 
         # get moving image origin
@@ -344,14 +349,15 @@
             write_group = np.sum(np.array(block_index) % 3 * (9, 3, 1))
             while not (write_group < time.time() / write_group_interval % 27 < write_group + .5):
                 time.sleep(1)
             output_transform[fix_slices] = output_transform[fix_slices] + transform
             return True
     # END CLOSURE
 
+
     # submit all alignments to cluster
     futures = cluster.client.map(
         align_single_block, indices,
         static_transform_list=static_transform_list,
     )
 
     # handle output for in memory and out of memory cases
@@ -364,31 +370,35 @@
                 transform[indices[iii][1]] += result
         return transform
     else:
         all_written = np.all( cluster.client.gather(futures) )
         return output_transform
 
 
-# TODO: this function not yet refactored
+# TODO: THIS FUNCTION CURRENTLY DOES NOT WORK FOR LARGER THAN MEMORY TRANSFORMS
 @cluster
 def nested_distributed_piecewise_alignment_pipeline(
     fix,
     mov,
     fix_spacing,
     mov_spacing,
     schedule,
     static_transform_list=None,
     fix_mask=None,
     mov_mask=None,
     cluster=None,
     cluster_kwargs={},
+    temporary_directory=None,
+    write_path=None,
     **kwargs,
 ):
     """
     Compose multiple calls to distributed_piecewise_alignment_pipeline with one function call.
+    Be sure you understand how distributed_piecewise_alignment_pipeline and all its arguments
+    work before you use this function.
 
     Parameters
     ----------
     fix : ndarray
         the fixed image
 
     mov : ndarray
@@ -404,17 +414,19 @@
         The spacing in physical units (e.g. mm or um) between voxels
         of the moving image.
         Length must equal `mov.ndim`
 
     schedule : list of tuples in this form [(tuple, [(str, dict), (str, dict), ...]), ...]
         The blocksize and steps arguments for each call to distributed_piecewise_alignment_pipeline
         An example:
-            step1 = ( (3, 1, 1), [('affine', affine_kwargs)] )
-            step2 = ( (
-
+            step1 = ( (256, 256, 256), [('affine', affine_kwargs)] )
+            step2 = ( (128, 128, 128), [('affine', affine_kwargs), ('deform', deform_kwargs)] )
+            schedule = [step1, step2]
+        In this example, affine alignment will be done on all 256^3 blocks of the image.
+        Subsequently, affine + deformable alignment will be done on all 128^3 blocks of the image.
 
     static_transform_list : list of numpy arrays (default: [])
         Transforms applied to moving image before applying query transform
         Assumed to have the same domain as the fixed image, though sampling
         can be different. I.e. the origin and span are the same (in physical
         units) but the number of voxels can be different.
 
@@ -438,134 +450,74 @@
     cluster_kwargs : dict (default: {})
         Arguments passed to ClusterWrap.cluster
         If working with an LSF cluster, this will be
         ClusterWrap.janelia_lsf_cluster. If on a workstation
         this will be ClusterWrap.local_cluster.
         This is how distribution parameters are specified.
 
+    temporary_directory : string (default: None)
+        Temporary files are created during alignment. The temporary files will be
+        in their own folder within the `temporary_directory`. The default is the
+        current directory. Temporary files are removed if the function completes
+        successfully.
+
+    write_path : string (default: None)
+        If the transforms found by this function are too large to fit into main
+        process memory, set this parameter to a folder where the transforms
+        can be written to disk as separate zarr files
+
     kwargs : any additional arguments
         Passed to `distributed_piecewise_alignment_pipeline`
 
     Returns
     -------
-    field : ndarray
+    field : nd array or zarr.core.Array
+        Composition of all alignments into a single displacement vector field.
     """
 
+    # temporary file paths and create zarr images
+    temporary_directory = tempfile.TemporaryDirectory(
+        prefix='.', dir=temporary_directory or os.getcwd(),
+    )
+    zarr_blocks = [128,] * fix.ndim
+    fix_zarr_path = temporary_directory.name + '/fix.zarr'
+    mov_zarr_path = temporary_directory.name + '/mov.zarr'
+    fix_mask_zarr_path = temporary_directory.name + '/fix_mask.zarr'
+    mov_mask_zarr_path = temporary_directory.name + '/mov_mask.zarr'
+    fix_zarr = ut.numpy_to_zarr(fix, zarr_blocks, fix_zarr_path)
+    mov_zarr = ut.numpy_to_zarr(mov, zarr_blocks, mov_zarr_path)
+    fix_mask_zarr = None
+    if fix_mask is not None: fix_mask_zarr = ut.numpy_to_zarr(fix_mask, zarr_blocks, fix_mask_zarr_path)
+    mov_mask_zarr = None
+    if mov_mask is not None: mov_mask_zarr = ut.numpy_to_zarr(mov_mask, zarr_blocks, mov_mask_zarr_path)
 
+    # zarr files for initial deformations
+    new_list = []
+    for iii, transform in enumerate(static_transform_list):
+        if transform.shape != (4, 4) and len(transform.shape) != 1:
+            path = temporary_directory.name + f'/deform{iii}.zarr'
+            transform = ut.numpy_to_zarr(transform, tuple(zarr_blocks) + (transform.shape[-1],), path)
+        new_list.append(transform)
+    static_transform_list = new_list
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-def old()
-
-    # set working copies of moving data
-    if static_transform_list is not None:
-        current_moving = apply_transform(
-            fix, mov, fix_spacing, mov_spacing,
-            transform_list=static_transform_list,
-        )
-        current_moving_mask = None
-        if mov_mask is not None:
-            current_moving_mask = apply_transform(
-                fix, mov_mask, fix_spacing, mov_spacing,
-                transform_list=static_transform_list,
-            )
-            current_moving_mask = (current_moving_mask > 0).astype(np.uint8)
-    else:
-        current_moving = np.copy(mov)
-        current_moving_mask = None if mov_mask is None else np.copy(mov_mask)
-
-    # initialize container and Loop over outer levels
-    counter = 0  # count each call to distributed_piecewise_affine_align
-    deform = np.zeros(fix.shape + (3,), dtype=np.float32)
-    for outer_level, inner_list in enumerate(block_schedule):
-
-        # initialize inner container and Loop over inner levels
-        ddd = np.zeros_like(deform)
-        for inner_level, nblocks in enumerate(inner_list):
-
-            # determine parameter settings
-            if parameter_schedule is not None:
-                instance_kwargs = {**kwargs, **parameter_schedule[counter]}
-            else:
-                instance_kwargs = kwargs
-
-            # align
-            ddd += distributed_piecewise_alignment_pipeline(
-                fix, current_moving,
-                fix_spacing, fix_spacing,  # images should be on same grid
-                nblocks=nblocks,
-                fix_mask=fix_mask,
-                mov_mask=current_moving_mask,
-                cluster=cluster,
-                cluster_kwargs=cluster_kwargs,
-                **instance_kwargs,
-            )
-
-            # increment counter
-            counter += 1
-
-        # take mean
-        ddd = ddd / len(inner_list)
-
-        # if not first iteration, compose with existing deform
-        if outer_level > 0:
-            deform = compose_transforms(deform, ddd, fix_spacing,)
-        else:
-            deform = ddd
-
-        # combine with initial transforms if given
-        if static_transform_list is not None:
-            transform_list = static_transform_list + [deform,]
-        else:
-            transform_list = [deform,]
-
-        # update working copy of image
-        current_moving = apply_transform(
-            fix, mov, fix_spacing, mov_spacing,
-            transform_list=transform_list,
+    # loop over the schedule
+    for iii, (blocksize, steps) in enumerate(schedule):
+        local_write_path = None
+        if write_path: local_write_path = write_path + '/{iii}.zarr'
+        deform = distributed_piecewise_alignment_pipeline(
+            fix_zarr, mov_zarr, fix_spacing, mov_spacing,
+            steps, blocksize,
+            static_transform_list=static_transform_list,
+            fix_mask=fix_mask_zarr,
+            mov_mask=mov_mask_zarr,
+            write_path=local_write_path,
+            cluster=cluster,
+            **kwargs,
         )
-        # update working copy of mask
-        if mov_mask is not None:
-            current_moving_mask = apply_transform(
-                fix, mov_mask, fix_spacing, mov_spacing,
-                transform_list=transform_list,
-            )
-            current_moving_mask = (current_moving_mask > 0).astype(np.uint8)
+        # TODO: THIS DOES NOT WORK WITH LARGER THAN MEMORY TRANSFORMS
+        if iii > 0:
+            deform = compose_transforms(static_transform_list.pop(), deform, fix_spacing)
+        static_transform_list.append(deform)
 
-        # write intermediates
-        if intermediates_path is not None:
-            ois = str(outer_level)
-            deform_path = (intermediates_path + '/twist_deform_{}.npy').format(ois)
-            image_path = (intermediates_path + '/twist_image_{}.npy').format(ois)
-            mask_path = (intermediates_path + '/twist_mask_{}.npy').format(ois)
-            np.save(deform_path, deform)
-            np.save(image_path, current_moving)
-            if mov_mask is not None:
-                np.save(mask_path, current_moving_mask)
-
-    # return deform
-    return deform
-    
+    # return in the requested format
+    return static_transform_list.pop()
```

### Comparing `bigstream-1.1.2/bigstream/piecewise_transform.py` & `bigstream-1.1.3/bigstream/piecewise_transform.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.1.2/bigstream/transform.py` & `bigstream-1.1.3/bigstream/transform.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Resample moving image onto fixed image through a list
     of transforms.
 
     Parameters
     ----------
     fix : ndarray
         the fixed image
+        Optionally, this can be a tuple specifying a shape.
 
     mov : ndarray
         the moving image; `fix.ndim` must equal `mov.ndim`
 
     fix_spacing : 1d array
         The spacing in physical units (e.g. mm or um) between voxels
         of the fixed image. Length must equal `fix.ndim`.
@@ -82,43 +83,52 @@
     # set global number of threads
     if "LSB_DJOB_NUMPROC" in os.environ:
         ncores = int(os.environ["LSB_DJOB_NUMPROC"])
     else:
         ncores = psutil.cpu_count(logical=False)
     sitk.ProcessObject.SetGlobalDefaultNumberOfThreads(2*ncores)
 
-    # convert images to sitk objects
-    dtype = fix.dtype
-    fix = sitk.Cast(ut.numpy_to_sitk(fix, fix_spacing, fix_origin), sitk.sitkFloat32)
-    mov = sitk.Cast(ut.numpy_to_sitk(mov, mov_spacing, mov_origin), sitk.sitkFloat32)
-
     # construct transform
     fix_spacing = np.array(fix_spacing)
     if transform_spacing is None: transform_spacing = fix_spacing
     transform = ut.transform_list_to_composite_transform(
         transform_list, transform_spacing, transform_origin,
     )
 
     # set up resampler object
     resampler = sitk.ResampleImageFilter()
     resampler.SetNumberOfThreads(2*ncores)
-    resampler.SetReferenceImage(fix)
-    resampler.SetTransform(transform)
 
+    # set reference data
+    if isinstance(fix, tuple):
+        dtype = mov.dtype
+        resampler.SetSize(fix[::-1])
+        resampler.SetOutputSpacing(fix_spacing[::-1])
+        if fix_origin is not None:
+            resampler.SetOutputOrigin(fix_origin[::-1])
+    else:
+        dtype = fix.dtype
+        fix = sitk.Cast(ut.numpy_to_sitk(fix, fix_spacing, fix_origin), sitk.sitkFloat32)
+        resampler.SetReferenceImage(fix)
+
+    # set moving image and transform
+    mov = sitk.Cast(ut.numpy_to_sitk(mov, mov_spacing, mov_origin), sitk.sitkFloat32)
+    resampler.SetTransform(transform)
+        
     # check for NN interpolation
     if interpolate_with_nn:
         resampler.SetInterpolator(sitk.sitkNearestNeighbor)
 
     # check for NN extrapolation
     if extrapolate_with_nn:
         resampler.SetUseNearestNeighborExtrapolator(True)
 
     # execute, return as numpy array
     resampled = resampler.Execute(mov)
-    return sitk.GetArrayFromImage(resampled).astype(dtype)
+    return sitk.GetArrayViewFromImage(resampled).astype(dtype)
 
 
 def apply_transform_to_coordinates(
     coordinates,
     transform_list,
     transform_spacing=None,
     transform_origin=None,
@@ -192,125 +202,150 @@
 
     return coordinates
 
 
 def compose_displacement_vector_fields(
     first_field,
     second_field,
-    spacing,
+    first_spacing,
+    second_spacing,
 ):
     """
     Compose two displacement vector fields into a single field
 
     Parameters
     ----------
     first_field : nd-array
         The first field
 
     second_field : nd-array
         The second field
 
-    spacing : 1d-array
-        The voxel spacing for the two fields (fields must have same spacing)
+    first_spacing : 1d-array
+        The voxel spacing for the first field
+
+    second_spacing : 1d-array
+        The voxel spacing for the second field
 
     Returns
     -------
     composite_field : nd-array
         The single field composition of first_field and second_field
+        The second field is the one learned second. In this case, the composition
+        is going to be on the same voxel grid and spacing as the second field.
     """
 
     # container for warped first field
-    first_field_warped = np.empty_like(first_field)
+    first_field_warped = np.empty_like(second_field)
 
     # loop over components
     for iii in range(3):
 
         # warp first field with second
         first_field_warped[..., iii] = apply_transform(
-            first_field[..., iii], first_field[..., iii],
-            spacing, spacing,
+            second_field[..., iii], first_field[..., iii],
+            second_spacing, first_spacing,
             transform_list=[second_field,],
             extrapolate_with_nn=True,
         )
 
     # combine warped first field and second field
     return first_field_warped + second_field
 
 
-def compose_transforms(transform_one, transform_two, spacing):
+def compose_transforms(
+    first_transform,
+    second_transform,
+    first_spacing,
+    second_spacing,
+):
     """
     Compose two transforms into a single transform
 
     Parameters
     ----------
-    transform_one : nd-array
+    first_transform : nd-array
         Can be either a 4x4 affine matrix or a displacement vector field
 
-    transform_two : nd-array
+    second_transform : nd-array
         Can be either a 4x4 affine matrix or a displacement vector field
 
-    spacing : 1d-array
-        The voxel spacing for the two transforms (transforms must have same spacing)
-        Ignored for affine matrices.
+    first_spacing : 1d-array
+        The voxel spacing for the first transform
+        Ignored for affine transforms (just put in a dummy value)
+
+    second_spacing : 1d-array
+        The voxel spacing for the second transform
+        Ignored for affine transforms (just put in a dummy value)
 
     Returns
     -------
     composite_transform : nd-array
-        The single transform composition of transform_one and transform_two
+        The single transform composition of first_transform and second_transform
         If both given transforms are affine this is a 4x4 matrix. Otherwise,
         it is a displacement vector field.
     """
 
     # two affines
-    if transform_one.shape == (4, 4) and transform_two.shape == (4, 4):
-        return np.matmul(transform_one, transform_two)
+    if first_transform.shape == (4, 4) and second_transform.shape == (4, 4):
+        return np.matmul(first_transform, second_transform)
 
     # one affine, two field
-    elif transform_one.shape == (4, 4):
-        transform_one = ut.matrix_to_displacement_field(
-            transform_one, transform_two.shape[:-1], spacing,
+    elif first_transform.shape == (4, 4):
+        first_transform = ut.matrix_to_displacement_field(
+            first_transform, second_transform.shape[:-1], second_spacing,
         )
+        first_spacing = second_spacing
 
     # one field, two affine
-    elif transform_two.shape == (4, 4):
-        transform_two = ut.matrix_to_displacement_field(
-            transform_two, transform_one.shape[:-1], spacing,
+    elif second_transform.shape == (4, 4):
+        second_transform = ut.matrix_to_displacement_field(
+            second_transform, first_transform.shape[:-1], first_spacing,
         )
+        second_spacing = first_spacing
 
     # compose fields
     return compose_displacement_vector_fields(
-        transform_one, transform_two, spacing,
+        first_transform, second_transform, first_spacing, second_spacing,
     )
 
 
-def compose_transform_list(transforms, spacing):
+def compose_transform_list(transforms, spacings):
     """
     Compose a list of transforms into a single transform
 
     Parameters
     ----------
     transforms : list
         Elements of list must be either 4x4 affine matrices or displacement
         vector fields
 
-    spacing : 1d-array
-        The voxel spacing of all transforms in the list (all transforms must
-        have the same spacing). Ignored for affine transforms.
+    spacings : list of 1d-arrays
+        The voxel spacing of all transforms in the list
+        Ignored for affine transforms (just put in a dummy value)
 
     Returns
     -------
     composite_transform : nd-array
         The single transform composition of all elements in transforms.
         If all transforms are affine, this is a 4x4 matrix. Otherwise,
         it is a displacement vector field.
     """
 
+    # ensure spacings is a list
+    if not isinstance(spacings, list):
+        spacings = [spacings,] * len(transforms)
+
     transform = transforms.pop()
+    transform_spacing = spacings.pop()
     while transforms:
-        transform = compose_transforms(transforms.pop(), transform, spacing)
+        transform = compose_transforms(
+            transforms.pop(), transform,
+            spacings.pop(), transform_spacing,
+        )
     return transform
 
 
 def invert_displacement_vector_field(
     field,
     spacing,
     iterations=10,
```

### Comparing `bigstream-1.1.2/bigstream/utility.py` & `bigstream-1.1.3/bigstream/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 from scipy.spatial.transform import Rotation
 import SimpleITK as sitk
 import zarr
 from zarr.indexing import BasicIndexer
-from numcodecs import Blosc
 from distributed import Lock
 import glob
 import h5py
 from ClusterWrap.decorator import cluster
+from zarr import blosc
 
 
 def skip_sample(image, spacing, ss_spacing):
     """
     Return a subset of the voxels in an image to approximate a different
     sampling rate
 
@@ -390,15 +390,15 @@
     if origin is None: origin = np.zeros(len(shape))
     if direction is None: direction = np.eye(len(shape))
     df = sitk.TransformToDisplacementField(
         bspline, sitk.sitkVectorFloat64,
         shape[::-1], origin[::-1], spacing[::-1],
         direction[::-1, ::-1].ravel(),
     )
-    return sitk.GetArrayFromImage(df).astype(np.float32)[..., ::-1]
+    return sitk.GetArrayViewFromImage(df).astype(np.float32)[..., ::-1]
 
 
 # TODO: function that takes a numpy array and return transform type
 
 
 def relative_spacing(query, reference, reference_spacing):
     """
@@ -463,15 +463,23 @@
             a = spacing[iii] if isinstance(spacing, tuple) else spacing
             b = origin[iii] if isinstance(origin, tuple) else origin
             t = field_to_displacement_field_transform(t, a, b)
         transform.AddTransform(t)
     return transform
 
 
-def create_zarr(path, shape, chunks, dtype, chunk_locked=False, client=None):
+def create_zarr(
+    path,
+    shape,
+    chunks,
+    dtype,
+    multithreaded=False,
+    chunk_locked=False,
+    client=None,
+):
     """
     Create a new zarr array on disk
 
     Parameters
     ----------
     path : string
         The location of the new zarr array
@@ -493,23 +501,24 @@
 
     Returns
     -------
     zarr_array : zarr array
         Reference to the newly created zarr array on disk
     """
 
-    compressor = Blosc(
-        cname='zstd', clevel=4, shuffle=Blosc.BITSHUFFLE,
-    )
+    synchronizer = None
+    if multithreaded:
+        blosc.use_threads = True
+        synchronizer = zarr.ThreadSynchronizer()
     zarr_disk = zarr.open(
         path, 'w',
         shape=shape,
         chunks=chunks,
         dtype=dtype,
-        compressor=compressor,
+        synchronizer=synchronizer,
     )
 
     # this code is currently never used within bigstream
     # keeping it aroung in case a use case comes up
     if chunk_locked:
         indexer = BasicIndexer(slice(None), zarr_disk)
         keys = (zarr_disk._chunk_key(idx.chunk_coords) for idx in indexer)
@@ -517,15 +526,15 @@
         lock['.zarray'] = Lock('.zarray', client=client)
         zarr_disk = zarr.open(
             store=zarr_disk.store, path=zarr_disk.path,
             synchronizer=lock, mode='r+',
         )
 
     return zarr_disk
-    
+
 
 def numpy_to_zarr(array, chunks, path):
     """
     Convert a numpy array to a zarr array on disk
 
     Parameters
     ----------
```

### Comparing `bigstream-1.1.2/setup.py` & `bigstream-1.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bigstream",
-    version="1.1.2",
+    version="1.1.3",
     author="Greg M. Fleishman",
     author_email="greg.nli10me@gmail.com",
     description="Tools for distributed alignment of massive images",
     url="https://github.com/GFleishman/bigstream",
     license="MIT",
     packages=setuptools.find_packages(),
     include_package_data=True,
@@ -17,13 +17,14 @@
         'bokeh>=2.4.3',
         'dask>=2022.9.1',
         'dask[array]>=2022.9.1',
         'dask[delayed]>=2022.9.1',
         'dask[distributed]>=2022.9.1',
         'ClusterWrap>=0.3.0',
         'zarr>=2.12.0',
+        'h5py>=3.8.0',
         'numcodecs>=0.9.1',
         'fishspot>=0.2.3',
         'SimpleITK>=2.2.0',
         'tifffile>=2022.10.10'
     ]
 )
```

