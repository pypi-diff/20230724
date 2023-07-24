# Comparing `tmp/vit-pytorch-1.2.7.tar.gz` & `tmp/vit-pytorch-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-pytorch-1.2.7.tar", last modified: Mon Jul 24 21:15:15 2023, max compression
+gzip compressed data, was "vit-pytorch-1.2.8.tar", last modified: Mon Jul 24 21:31:06 2023, max compression
```

## Comparing `vit-pytorch-1.2.7.tar` & `vit-pytorch-1.2.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:15:15.498545 vit-pytorch-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 21:15:15.498545 vit-pytorch-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    62662 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:15:15.498545 vit-pytorch-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:15:15.494545 vit-pytorch-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:15:15.498545 vit-pytorch-1.2.7/vit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/ats_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/cait.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/cct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/cct_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/cross_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/crossformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/cvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/deepvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/dino.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/distill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/efficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/es_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/learnable_memory_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/levit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/local_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/max_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/mobile_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/mp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/mpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/na_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/nest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/parallel_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/pit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/regionvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/rvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/scalable_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/sep_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/simmim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/simple_flash_attn_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/simple_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/simple_vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/simple_vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/simple_vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/t2t.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/twins_svt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/vit_for_small_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/vit_with_patch_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-24 21:14:58.000000 vit-pytorch-1.2.7/vit_pytorch/vivit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:15:15.498545 vit-pytorch-1.2.7/vit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 21:15:15.000000 vit-pytorch-1.2.7/vit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-24 21:15:15.000000 vit-pytorch-1.2.7/vit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:15:15.000000 vit-pytorch-1.2.7/vit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:15:15.000000 vit-pytorch-1.2.7/vit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 21:15:15.000000 vit-pytorch-1.2.7/vit_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:31:06.749235 vit-pytorch-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 21:31:06.749235 vit-pytorch-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    62662 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:31:06.749235 vit-pytorch-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:31:06.741234 vit-pytorch-1.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:31:06.745235 vit-pytorch-1.2.8/vit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/ats_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cct_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cross_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/crossformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/deepvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/efficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/es_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/learnable_memory_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/levit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/local_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/max_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/mobile_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/mpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/na_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/parallel_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/pit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/regionvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/rvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/scalable_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/sep_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simmim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_flash_attn_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/t2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/twins_svt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_for_small_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_with_patch_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vivit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:31:06.745235 vit-pytorch-1.2.8/vit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/top_level.txt
```

### Comparing `vit-pytorch-1.2.7/LICENSE` & `vit-pytorch-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/PKG-INFO` & `vit-pytorch-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.2.7
+Version: 1.2.8
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vit-pytorch-1.2.7/README.md` & `vit-pytorch-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/setup.py` & `vit-pytorch-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vit-pytorch',
   packages = find_packages(exclude=['examples']),
-  version = '1.2.7',
+  version = '1.2.8',
   license='MIT',
   description = 'Vision Transformer (ViT) - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vit-pytorch',
   keywords = [
```

### Comparing `vit-pytorch-1.2.7/vit_pytorch/ats_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/ats_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/cait.py` & `vit-pytorch-1.2.8/vit_pytorch/cait.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/cct.py` & `vit-pytorch-1.2.8/vit_pytorch/cct.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/cct_3d.py` & `vit-pytorch-1.2.8/vit_pytorch/cct_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/cross_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/cross_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/crossformer.py` & `vit-pytorch-1.2.8/vit_pytorch/crossformer.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/cvt.py` & `vit-pytorch-1.2.8/vit_pytorch/cvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/deepvit.py` & `vit-pytorch-1.2.8/vit_pytorch/deepvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/dino.py` & `vit-pytorch-1.2.8/vit_pytorch/dino.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/distill.py` & `vit-pytorch-1.2.8/vit_pytorch/distill.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/efficient.py` & `vit-pytorch-1.2.8/vit_pytorch/efficient.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/es_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/es_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/extractor.py` & `vit-pytorch-1.2.8/vit_pytorch/extractor.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/learnable_memory_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/learnable_memory_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/levit.py` & `vit-pytorch-1.2.8/vit_pytorch/levit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/local_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/local_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/mae.py` & `vit-pytorch-1.2.8/vit_pytorch/mae.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/max_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/max_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/mobile_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/mobile_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/mp3.py` & `vit-pytorch-1.2.8/vit_pytorch/mp3.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/mpp.py` & `vit-pytorch-1.2.8/vit_pytorch/mpp.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/na_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/na_vit.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,22 +134,33 @@
         for attn, ff in self.layers:
             x = attn(x, mask = mask, attn_mask = attn_mask) + x
             x = ff(x) + x
 
         return self.norm(x)
 
 class NaViT(nn.Module):
-    def __init__(self, *, image_size, patch_size, num_classes, dim, depth, heads, mlp_dim, channels = 3, dim_head = 64, dropout = 0., emb_dropout = 0., token_dropout_prob = 0.):
+    def __init__(self, *, image_size, patch_size, num_classes, dim, depth, heads, mlp_dim, channels = 3, dim_head = 64, dropout = 0., emb_dropout = 0., token_dropout_prob = None):
         super().__init__()
         image_height, image_width = pair(image_size)
 
         # what percent of tokens to dropout
-        # in paper, they found this should vary depending on resolution (todo - figure out how to do this, maybe with callback?)
+        # if int or float given, then assume constant dropout prob
+        # otherwise accept a callback that in turn calculates dropout prob from height and width
 
-        self.token_dropout_prob = token_dropout_prob
+        self.calc_token_dropout = calc_token_dropout = None
+
+        if callable(token_dropout_prob):
+            self.calc_token_dropout = token_dropout_prob
+
+        elif isinstance(token_dropout_prob, (float, int)):
+            assert 0. < token_dropout_prob < 1.
+            token_dropout_prob = float(token_dropout_prob)
+            self.calc_token_dropout = lambda height, width: token_dropout_prob
+
+        # calculate patching related stuff
 
         assert divisible_by(image_height, patch_size) and divisible_by(image_width, patch_size), 'Image dimensions must be divisible by the patch size.'
 
         patch_height_dim, patch_width_dim = (image_height // patch_size), (image_width // patch_size)
         patch_dim = channels * (patch_size ** 2)
 
         self.channels = channels
@@ -186,15 +197,15 @@
     def device(self):
         return next(self.parameters()).device
 
     def forward(
         self,
         batched_images: List[List[Tensor]] # assume different resolution images already grouped correctly
     ):
-        p, c, device, has_token_dropout = self.patch_size, self.channels, self.device, self.token_dropout_prob > 0.
+        p, c, device, has_token_dropout = self.patch_size, self.channels, self.device, exists(self.calc_token_dropout)
 
         arange = partial(torch.arange, device = device)
         pad_sequence = partial(orig_pad_sequence, batch_first = True)
 
         # process images into variable lengthed sequences with attention mask
 
         num_images = []
@@ -223,16 +234,18 @@
 
                 pos = rearrange(pos, 'h w c -> (h w) c')
                 seq = rearrange(image, 'c (h p1) (w p2) -> (h w) (c p1 p2)', p1 = p, p2 = p)
 
                 seq_len = seq.shape[-2]
 
                 if has_token_dropout:
-                    num_keep = max(1, int(seq_len * (1 - self.token_dropout_prob)))
+                    token_dropout = self.calc_token_dropout(*image_dims)
+                    num_keep = max(1, int(seq_len * (1 - token_dropout)))
                     keep_indices = torch.randn((seq_len,), device = device).topk(num_keep, dim = -1).indices
+
                     seq = seq[keep_indices]
                     pos = pos[keep_indices]
 
                 image_ids = F.pad(image_ids, (0, seq.shape[-2]), value = image_id)
                 sequences.append(seq)
                 positions.append(pos)
```

### Comparing `vit-pytorch-1.2.7/vit_pytorch/nest.py` & `vit-pytorch-1.2.8/vit_pytorch/nest.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/parallel_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/parallel_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/pit.py` & `vit-pytorch-1.2.8/vit_pytorch/pit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/recorder.py` & `vit-pytorch-1.2.8/vit_pytorch/recorder.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/regionvit.py` & `vit-pytorch-1.2.8/vit_pytorch/regionvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/rvt.py` & `vit-pytorch-1.2.8/vit_pytorch/rvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/scalable_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/scalable_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/sep_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/sep_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/simmim.py` & `vit-pytorch-1.2.8/vit_pytorch/simmim.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/simple_flash_attn_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/simple_flash_attn_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/simple_vit.py` & `vit-pytorch-1.2.8/vit_pytorch/simple_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/simple_vit_1d.py` & `vit-pytorch-1.2.8/vit_pytorch/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/simple_vit_3d.py` & `vit-pytorch-1.2.8/vit_pytorch/simple_vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/simple_vit_with_patch_dropout.py` & `vit-pytorch-1.2.8/vit_pytorch/simple_vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/t2t.py` & `vit-pytorch-1.2.8/vit_pytorch/t2t.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/twins_svt.py` & `vit-pytorch-1.2.8/vit_pytorch/twins_svt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/vit.py` & `vit-pytorch-1.2.8/vit_pytorch/vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/vit_1d.py` & `vit-pytorch-1.2.8/vit_pytorch/vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/vit_3d.py` & `vit-pytorch-1.2.8/vit_pytorch/vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/vit_for_small_dataset.py` & `vit-pytorch-1.2.8/vit_pytorch/vit_for_small_dataset.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/vit_with_patch_dropout.py` & `vit-pytorch-1.2.8/vit_pytorch/vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/vit_with_patch_merger.py` & `vit-pytorch-1.2.8/vit_pytorch/vit_with_patch_merger.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch/vivit.py` & `vit-pytorch-1.2.8/vit_pytorch/vivit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.7/vit_pytorch.egg-info/PKG-INFO` & `vit-pytorch-1.2.8/vit_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.2.7
+Version: 1.2.8
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vit-pytorch-1.2.7/vit_pytorch.egg-info/SOURCES.txt` & `vit-pytorch-1.2.8/vit_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

