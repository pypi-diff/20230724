# Comparing `tmp/vit-pytorch-1.2.5.tar.gz` & `tmp/vit-pytorch-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-pytorch-1.2.5.tar", last modified: Mon Jul 24 13:44:13 2023, max compression
+gzip compressed data, was "vit-pytorch-1.2.6.tar", last modified: Mon Jul 24 20:55:00 2023, max compression
```

## Comparing `vit-pytorch-1.2.5.tar` & `vit-pytorch-1.2.6.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:13.778869 vit-pytorch-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 13:44:13.778869 vit-pytorch-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    60828 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:44:13.778869 vit-pytorch-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:13.770869 vit-pytorch-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:13.778869 vit-pytorch-1.2.5/vit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/ats_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/cait.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/cct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/cct_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/cross_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/crossformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/cvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/deepvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/dino.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/distill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/efficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/es_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/learnable_memory_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/levit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/local_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/max_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/mobile_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/mp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/mpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/nest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/parallel_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/pit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/regionvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/rvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/scalable_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/sep_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/simmim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/simple_flash_attn_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/simple_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/simple_vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/simple_vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/simple_vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/t2t.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/twins_svt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/vit_for_small_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/vit_with_patch_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-24 13:43:49.000000 vit-pytorch-1.2.5/vit_pytorch/vivit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:44:13.778869 vit-pytorch-1.2.5/vit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 13:44:13.000000 vit-pytorch-1.2.5/vit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-24 13:44:13.000000 vit-pytorch-1.2.5/vit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:44:13.000000 vit-pytorch-1.2.5/vit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:44:13.000000 vit-pytorch-1.2.5/vit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 13:44:13.000000 vit-pytorch-1.2.5/vit_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:55:00.472136 vit-pytorch-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 20:55:00.472136 vit-pytorch-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    62589 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:55:00.472136 vit-pytorch-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:55:00.468136 vit-pytorch-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:55:00.472136 vit-pytorch-1.2.6/vit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/ats_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/cait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/cct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/cct_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/cross_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/crossformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/cvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/deepvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/efficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/es_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/learnable_memory_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/levit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/local_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/max_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/mobile_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/mpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/na_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/parallel_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/pit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/regionvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/rvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/scalable_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/sep_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/simmim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/simple_flash_attn_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/simple_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/simple_vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/simple_vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/simple_vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/t2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/twins_svt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/vit_for_small_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/vit_with_patch_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-24 20:54:48.000000 vit-pytorch-1.2.6/vit_pytorch/vivit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:55:00.472136 vit-pytorch-1.2.6/vit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 20:55:00.000000 vit-pytorch-1.2.6/vit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-24 20:55:00.000000 vit-pytorch-1.2.6/vit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:55:00.000000 vit-pytorch-1.2.6/vit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:55:00.000000 vit-pytorch-1.2.6/vit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 20:55:00.000000 vit-pytorch-1.2.6/vit_pytorch.egg-info/top_level.txt
```

### Comparing `vit-pytorch-1.2.5/LICENSE` & `vit-pytorch-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/PKG-INFO` & `vit-pytorch-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.2.5
+Version: 1.2.6
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vit-pytorch-1.2.5/README.md` & `vit-pytorch-1.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ## Table of Contents
 
 - [Vision Transformer - Pytorch](#vision-transformer---pytorch)
 - [Install](#install)
 - [Usage](#usage)
 - [Parameters](#parameters)
 - [Simple ViT](#simple-vit)
+- [NaViT](#na-vit)
 - [Distillation](#distillation)
 - [Deep ViT](#deep-vit)
 - [CaiT](#cait)
 - [Token-to-Token ViT](#token-to-token-vit)
 - [CCT](#cct)
 - [Cross ViT](#cross-vit)
 - [PiT](#pit)
@@ -135,14 +136,52 @@
 )
 
 img = torch.randn(1, 3, 256, 256)
 
 preds = v(img) # (1, 1000)
 ```
 
+## NaViT
+
+<img src="./images/na_vit.png" width="450px"></img>
+
+<a href="https://arxiv.org/abs/2307.06304">This paper</a> proposes to leverage the flexibility of attention and masking for variable lengthed sequences to train images of multiple resolution, packed into a single batch. They demonstrate much faster training and improved accuracies, with the only cost being extra complexity in the architecture and dataloading. They use factorized 2d positional encodings, token dropping, as well as query-key normalization.
+
+You can use it as follows
+
+```python
+import torch
+from vit_pytorch.na_vit import NaViT
+
+v = NaViT(
+    image_size = 256,
+    patch_size = 32,
+    num_classes = 1000,
+    dim = 1024,
+    depth = 6,
+    heads = 16,
+    mlp_dim = 2048,
+    dropout = 0.1,
+    emb_dropout = 0.1
+)
+
+# 5 images of different resolutions - List[List[Tensor]]
+
+# for now, you'll have to correctly place images in same batch element as to not exceed maximum allowed sequence length for self-attention w/ masking
+
+images = [
+    [torch.randn(3, 256, 256), torch.randn(3, 128, 128)],
+    [torch.randn(3, 128, 256), torch.randn(3, 256, 128)],
+    [torch.randn(3, 64, 256)]
+]
+
+preds = v(images) # (5, 1000) - 5, because 5 images of different resolution above
+
+```
+
 ## Distillation
 
 <img src="./images/distill.png" width="300px"></img>
 
 A recent <a href="https://arxiv.org/abs/2012.12877">paper</a> has shown that use of a distillation token for distilling knowledge from convolutional nets to vision transformer can yield small and efficient vision transformers. This repository offers the means to do distillation easily.
 
 ex. distilling from Resnet50 (or any teacher) to a vision transformer
@@ -1931,14 +1970,22 @@
     publisher = {arXiv},
     year    = {2023},
     copyright = {Creative Commons Attribution 4.0 International}
 }
 ```
 
 ```bibtex
+@inproceedings{Dehghani2023PatchNP,
+    title   = {Patch n' Pack: NaViT, a Vision Transformer for any Aspect Ratio and Resolution},
+    author  = {Mostafa Dehghani and Basil Mustafa and Josip Djolonga and Jonathan Heek and Matthias Minderer and Mathilde Caron and Andreas Steiner and Joan Puigcerver and Robert Geirhos and Ibrahim M. Alabdulmohsin and Avital Oliver and Piotr Padlewski and Alexey A. Gritsenko and Mario Luvci'c and Neil Houlsby},
+    year    = {2023}
+}
+```
+
+```bibtex
 @misc{vaswani2017attention,
     title   = {Attention Is All You Need},
     author  = {Ashish Vaswani and Noam Shazeer and Niki Parmar and Jakob Uszkoreit and Llion Jones and Aidan N. Gomez and Lukasz Kaiser and Illia Polosukhin},
     year    = {2017},
     eprint  = {1706.03762},
     archivePrefix = {arXiv},
     primaryClass = {cs.CL}
```

#### html2text {}

```diff
@@ -1,67 +1,82 @@
 [./images/vit.gif] ## Table of Contents - [Vision Transformer - Pytorch]
 (#vision-transformer---pytorch) - [Install](#install) - [Usage](#usage) -
-[Parameters](#parameters) - [Simple ViT](#simple-vit) - [Distillation]
-(#distillation) - [Deep ViT](#deep-vit) - [CaiT](#cait) - [Token-to-Token ViT]
-(#token-to-token-vit) - [CCT](#cct) - [Cross ViT](#cross-vit) - [PiT](#pit) -
-[LeViT](#levit) - [CvT](#cvt) - [Twins SVT](#twins-svt) - [CrossFormer]
-(#crossformer) - [RegionViT](#regionvit) - [ScalableViT](#scalablevit) -
-[SepViT](#sepvit) - [MaxViT](#maxvit) - [NesT](#nest) - [MobileViT](#mobilevit)
-- [Masked Autoencoder](#masked-autoencoder) - [Simple Masked Image Modeling]
-(#simple-masked-image-modeling) - [Masked Patch Prediction](#masked-patch-
-prediction) - [Masked Position Prediction](#masked-position-prediction) -
-[Adaptive Token Sampling](#adaptive-token-sampling) - [Patch Merger](#patch-
-merger) - [Vision Transformer for Small Datasets](#vision-transformer-for-
-small-datasets) - [3D Vit](#3d-vit) - [ViVit](#vivit) - [Parallel ViT]
-(#parallel-vit) - [Learnable Memory ViT](#learnable-memory-vit) - [Dino](#dino)
-- [EsViT](#esvit) - [Accessing Attention](#accessing-attention) - [Research
-Ideas](#research-ideas) * [Efficient Attention](#efficient-attention) *
-[Combining with other Transformer improvements](#combining-with-other-
-transformer-improvements) - [FAQ](#faq) - [Resources](#resources) - [Citations]
-(#citations) ## Vision Transformer - Pytorch Implementation of Vision
-Transformer, a simple way to achieve SOTA in vision classification with only a
-single transformer encoder, in Pytorch. Significance is further explained in
-Yannic_Kilcher's video. There's really not much to code here, but may as well
-lay it out for everyone so we expedite the attention revolution. For a Pytorch
-implementation with pretrained models, please see Ross Wightman's repository
-here. The official Jax repository is here. A tensorflow2 translation also
-exists here, created by research scientist Junho_Kim! ð Flax_translation by
-Enrico_Shippole! ## Install ```bash $ pip install vit-pytorch ``` ## Usage
-```python import torch from vit_pytorch import ViT v = ViT( image_size = 256,
-patch_size = 32, num_classes = 1000, dim = 1024, depth = 6, heads = 16, mlp_dim
-= 2048, dropout = 0.1, emb_dropout = 0.1 ) img = torch.randn(1, 3, 256, 256)
-preds = v(img) # (1, 1000) ``` ## Parameters - `image_size`: int. Image size.
-If you have rectangular images, make sure your image size is the maximum of the
-width and height - `patch_size`: int. Number of patches. `image_size` must be
-divisible by `patch_size`. The number of patches is: ` n = (image_size /
-/ patch_size) ** 2` and `n` **must be greater than 16**. - `num_classes`: int.
-Number of classes to classify. - `dim`: int. Last dimension of output tensor
-after linear transformation `nn.Linear(..., dim)`. - `depth`: int. Number of
-Transformer blocks. - `heads`: int. Number of heads in Multi-head Attention
-layer. - `mlp_dim`: int. Dimension of the MLP (FeedForward) layer. -
-`channels`: int, default `3`. Number of image's channels. - `dropout`: float
-between `[0, 1]`, default `0.`. Dropout rate. - `emb_dropout`: float between `
-[0, 1]`, default `0`. Embedding dropout rate. - `pool`: string, either `cls`
-token pooling or `mean` pooling ## Simple ViT An_update from some of the same
-authors of the original paper proposes simplifications to `ViT` that allows it
-to train faster and better. Among these simplifications include 2d sinusoidal
-positional embedding, global average pooling (no CLS token), no dropout, batch
-sizes of 1024 rather than 4096, and use of RandAugment and MixUp augmentations.
-They also show that a simple linear at the end is not significantly worse than
-the original MLP head You can use it by importing the `SimpleViT` as shown
-below ```python import torch from vit_pytorch import SimpleViT v = SimpleViT
+[Parameters](#parameters) - [Simple ViT](#simple-vit) - [NaViT](#na-vit) -
+[Distillation](#distillation) - [Deep ViT](#deep-vit) - [CaiT](#cait) - [Token-
+to-Token ViT](#token-to-token-vit) - [CCT](#cct) - [Cross ViT](#cross-vit) -
+[PiT](#pit) - [LeViT](#levit) - [CvT](#cvt) - [Twins SVT](#twins-svt) -
+[CrossFormer](#crossformer) - [RegionViT](#regionvit) - [ScalableViT]
+(#scalablevit) - [SepViT](#sepvit) - [MaxViT](#maxvit) - [NesT](#nest) -
+[MobileViT](#mobilevit) - [Masked Autoencoder](#masked-autoencoder) - [Simple
+Masked Image Modeling](#simple-masked-image-modeling) - [Masked Patch
+Prediction](#masked-patch-prediction) - [Masked Position Prediction](#masked-
+position-prediction) - [Adaptive Token Sampling](#adaptive-token-sampling) -
+[Patch Merger](#patch-merger) - [Vision Transformer for Small Datasets]
+(#vision-transformer-for-small-datasets) - [3D Vit](#3d-vit) - [ViVit](#vivit)
+- [Parallel ViT](#parallel-vit) - [Learnable Memory ViT](#learnable-memory-vit)
+- [Dino](#dino) - [EsViT](#esvit) - [Accessing Attention](#accessing-attention)
+- [Research Ideas](#research-ideas) * [Efficient Attention](#efficient-
+attention) * [Combining with other Transformer improvements](#combining-with-
+other-transformer-improvements) - [FAQ](#faq) - [Resources](#resources) -
+[Citations](#citations) ## Vision Transformer - Pytorch Implementation of
+Vision_Transformer, a simple way to achieve SOTA in vision classification with
+only a single transformer encoder, in Pytorch. Significance is further
+explained in Yannic_Kilcher's video. There's really not much to code here, but
+may as well lay it out for everyone so we expedite the attention revolution.
+For a Pytorch implementation with pretrained models, please see Ross Wightman's
+repository here. The official Jax repository is here. A tensorflow2 translation
+also exists here, created by research scientist Junho_Kim! ð Flax
+translation by Enrico_Shippole! ## Install ```bash $ pip install vit-pytorch
+``` ## Usage ```python import torch from vit_pytorch import ViT v = ViT
 ( image_size = 256, patch_size = 32, num_classes = 1000, dim = 1024, depth = 6,
-heads = 16, mlp_dim = 2048 ) img = torch.randn(1, 3, 256, 256) preds = v(img) #
-(1, 1000) ``` ## Distillation [./images/distill.png] A recent paper has shown
-that use of a distillation token for distilling knowledge from convolutional
-nets to vision transformer can yield small and efficient vision transformers.
-This repository offers the means to do distillation easily. ex. distilling from
-Resnet50 (or any teacher) to a vision transformer ```python import torch from
-torchvision.models import resnet50 from vit_pytorch.distill import
-DistillableViT, DistillWrapper teacher = resnet50(pretrained = True) v =
+heads = 16, mlp_dim = 2048, dropout = 0.1, emb_dropout = 0.1 ) img =
+torch.randn(1, 3, 256, 256) preds = v(img) # (1, 1000) ``` ## Parameters -
+`image_size`: int. Image size. If you have rectangular images, make sure your
+image size is the maximum of the width and height - `patch_size`: int. Number
+of patches. `image_size` must be divisible by `patch_size`. The number of
+patches is: ` n = (image_size // patch_size) ** 2` and `n` **must be greater
+than 16**. - `num_classes`: int. Number of classes to classify. - `dim`: int.
+Last dimension of output tensor after linear transformation `nn.Linear(...,
+dim)`. - `depth`: int. Number of Transformer blocks. - `heads`: int. Number of
+heads in Multi-head Attention layer. - `mlp_dim`: int. Dimension of the MLP
+(FeedForward) layer. - `channels`: int, default `3`. Number of image's
+channels. - `dropout`: float between `[0, 1]`, default `0.`. Dropout rate. -
+`emb_dropout`: float between `[0, 1]`, default `0`. Embedding dropout rate. -
+`pool`: string, either `cls` token pooling or `mean` pooling ## Simple ViT An
+update from some of the same authors of the original paper proposes
+simplifications to `ViT` that allows it to train faster and better. Among these
+simplifications include 2d sinusoidal positional embedding, global average
+pooling (no CLS token), no dropout, batch sizes of 1024 rather than 4096, and
+use of RandAugment and MixUp augmentations. They also show that a simple linear
+at the end is not significantly worse than the original MLP head You can use it
+by importing the `SimpleViT` as shown below ```python import torch from
+vit_pytorch import SimpleViT v = SimpleViT( image_size = 256, patch_size = 32,
+num_classes = 1000, dim = 1024, depth = 6, heads = 16, mlp_dim = 2048 ) img =
+torch.randn(1, 3, 256, 256) preds = v(img) # (1, 1000) ``` ## NaViT [./images/
+na_vit.png] This_paper proposes to leverage the flexibility of attention and
+masking for variable lengthed sequences to train images of multiple resolution,
+packed into a single batch. They demonstrate much faster training and improved
+accuracies, with the only cost being extra complexity in the architecture and
+dataloading. They use factorized 2d positional encodings, token dropping, as
+well as query-key normalization. You can use it as follows ```python import
+torch from vit_pytorch.na_vit import NaViT v = NaViT( image_size = 256,
+patch_size = 32, num_classes = 1000, dim = 1024, depth = 6, heads = 16, mlp_dim
+= 2048, dropout = 0.1, emb_dropout = 0.1 ) # 5 images of different resolutions
+- List[List[Tensor]] # for now, you'll have to correctly place images in same
+batch element as to not exceed maximum allowed sequence length for self-
+attention w/ masking images = [ [torch.randn(3, 256, 256), torch.randn(3, 128,
+128)], [torch.randn(3, 128, 256), torch.randn(3, 256, 128)], [torch.randn(3,
+64, 256)] ] preds = v(images) # (5, 1000) - 5, because 5 images of different
+resolution above ``` ## Distillation [./images/distill.png] A recent paper has
+shown that use of a distillation token for distilling knowledge from
+convolutional nets to vision transformer can yield small and efficient vision
+transformers. This repository offers the means to do distillation easily. ex.
+distilling from Resnet50 (or any teacher) to a vision transformer ```python
+import torch from torchvision.models import resnet50 from vit_pytorch.distill
+import DistillableViT, DistillWrapper teacher = resnet50(pretrained = True) v =
 DistillableViT( image_size = 256, patch_size = 32, num_classes = 1000, dim =
 1024, depth = 6, heads = 8, mlp_dim = 2048, dropout = 0.1, emb_dropout = 0.1 )
 distiller = DistillWrapper( student = v, teacher = teacher, temperature = 3, #
 temperature of distillation alpha = 0.5, # trade between main loss and
 distillation loss hard = False # whether to use soft or hard distillation ) img
 = torch.randn(2, 3, 256, 256) labels = torch.randint(0, 1000, (2,)) loss =
 distiller(img, labels) loss.backward() # after lots of training above ... pred
@@ -673,18 +688,25 @@
 {Liu2022PatchDropoutEV, title = {PatchDropout: Economizing Vision Transformers
 Using Patch Dropout}, author = {Yue Liu and Christos Matsoukas and Fredrik
 Strand and Hossein Azizpour and Kevin Smith}, journal = {ArXiv}, year = {2022},
 volume = {abs/2208.07220} } ``` ```bibtex @misc{https://doi.org/10.48550/
 arxiv.2302.01327, doi = {10.48550/ARXIV.2302.01327}, url = {https://arxiv.org/
 abs/2302.01327}, author = {Kumar, Manoj and Dehghani, Mostafa and Houlsby,
 Neil}, title = {Dual PatchNorm}, publisher = {arXiv}, year = {2023}, copyright
-= {Creative Commons Attribution 4.0 International} } ``` ```bibtex @misc
-{vaswani2017attention, title = {Attention Is All You Need}, author = {Ashish
-Vaswani and Noam Shazeer and Niki Parmar and Jakob Uszkoreit and Llion Jones
-and Aidan N. Gomez and Lukasz Kaiser and Illia Polosukhin}, year = {2017},
-eprint = {1706.03762}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ```
-```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
-and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
-and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
-booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ``` *I visualise a time when we will be to robots what dogs are to humans,
-and Iâm rooting for the machines.* â Claude Shannon
+= {Creative Commons Attribution 4.0 International} } ``` ```bibtex
+@inproceedings{Dehghani2023PatchNP, title = {Patch n' Pack: NaViT, a Vision
+Transformer for any Aspect Ratio and Resolution}, author = {Mostafa Dehghani
+and Basil Mustafa and Josip Djolonga and Jonathan Heek and Matthias Minderer
+and Mathilde Caron and Andreas Steiner and Joan Puigcerver and Robert Geirhos
+and Ibrahim M. Alabdulmohsin and Avital Oliver and Piotr Padlewski and Alexey
+A. Gritsenko and Mario Luvci'c and Neil Houlsby}, year = {2023} } ``` ```bibtex
+@misc{vaswani2017attention, title = {Attention Is All You Need}, author =
+{Ashish Vaswani and Noam Shazeer and Niki Parmar and Jakob Uszkoreit and Llion
+Jones and Aidan N. Gomez and Lukasz Kaiser and Illia Polosukhin}, year =
+{2017}, eprint = {1706.03762}, archivePrefix = {arXiv}, primaryClass = {cs.CL}
+} ``` ```bibtex @inproceedings{dao2022flashattention, title = {Flash
+{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R
+{\'e}, Christopher}, booktitle = {Advances in Neural Information Processing
+Systems}, year = {2022} } ``` *I visualise a time when we will be to robots
+what dogs are to humans, and Iâm rooting for the machines.* â Claude
+Shannon
```

### Comparing `vit-pytorch-1.2.5/setup.py` & `vit-pytorch-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vit-pytorch',
   packages = find_packages(exclude=['examples']),
-  version = '1.2.5',
+  version = '1.2.6',
   license='MIT',
   description = 'Vision Transformer (ViT) - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vit-pytorch',
   keywords = [
```

### Comparing `vit-pytorch-1.2.5/vit_pytorch/ats_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/ats_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/cait.py` & `vit-pytorch-1.2.6/vit_pytorch/cait.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/cct.py` & `vit-pytorch-1.2.6/vit_pytorch/cct.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/cct_3d.py` & `vit-pytorch-1.2.6/vit_pytorch/cct_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/cross_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/cross_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/crossformer.py` & `vit-pytorch-1.2.6/vit_pytorch/crossformer.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/cvt.py` & `vit-pytorch-1.2.6/vit_pytorch/cvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/deepvit.py` & `vit-pytorch-1.2.6/vit_pytorch/deepvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/dino.py` & `vit-pytorch-1.2.6/vit_pytorch/dino.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/distill.py` & `vit-pytorch-1.2.6/vit_pytorch/distill.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/efficient.py` & `vit-pytorch-1.2.6/vit_pytorch/efficient.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/es_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/es_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/extractor.py` & `vit-pytorch-1.2.6/vit_pytorch/extractor.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/learnable_memory_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/learnable_memory_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/levit.py` & `vit-pytorch-1.2.6/vit_pytorch/levit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/local_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/local_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/mae.py` & `vit-pytorch-1.2.6/vit_pytorch/mae.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/max_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/max_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/mobile_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/mobile_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/mp3.py` & `vit-pytorch-1.2.6/vit_pytorch/mp3.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/mpp.py` & `vit-pytorch-1.2.6/vit_pytorch/mpp.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/nest.py` & `vit-pytorch-1.2.6/vit_pytorch/nest.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/parallel_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/parallel_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/pit.py` & `vit-pytorch-1.2.6/vit_pytorch/pit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/recorder.py` & `vit-pytorch-1.2.6/vit_pytorch/recorder.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/regionvit.py` & `vit-pytorch-1.2.6/vit_pytorch/regionvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/rvt.py` & `vit-pytorch-1.2.6/vit_pytorch/rvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/scalable_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/scalable_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/sep_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/sep_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/simmim.py` & `vit-pytorch-1.2.6/vit_pytorch/simmim.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/simple_flash_attn_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/simple_flash_attn_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/simple_vit.py` & `vit-pytorch-1.2.6/vit_pytorch/simple_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/simple_vit_1d.py` & `vit-pytorch-1.2.6/vit_pytorch/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/simple_vit_3d.py` & `vit-pytorch-1.2.6/vit_pytorch/simple_vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/simple_vit_with_patch_dropout.py` & `vit-pytorch-1.2.6/vit_pytorch/simple_vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/t2t.py` & `vit-pytorch-1.2.6/vit_pytorch/t2t.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/twins_svt.py` & `vit-pytorch-1.2.6/vit_pytorch/twins_svt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/vit.py` & `vit-pytorch-1.2.6/vit_pytorch/vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/vit_1d.py` & `vit-pytorch-1.2.6/vit_pytorch/vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/vit_3d.py` & `vit-pytorch-1.2.6/vit_pytorch/vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/vit_for_small_dataset.py` & `vit-pytorch-1.2.6/vit_pytorch/vit_for_small_dataset.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/vit_with_patch_dropout.py` & `vit-pytorch-1.2.6/vit_pytorch/vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/vit_with_patch_merger.py` & `vit-pytorch-1.2.6/vit_pytorch/vit_with_patch_merger.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch/vivit.py` & `vit-pytorch-1.2.6/vit_pytorch/vivit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.5/vit_pytorch.egg-info/PKG-INFO` & `vit-pytorch-1.2.6/vit_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.2.5
+Version: 1.2.6
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vit-pytorch-1.2.5/vit_pytorch.egg-info/SOURCES.txt` & `vit-pytorch-1.2.6/vit_pytorch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 vit_pytorch/levit.py
 vit_pytorch/local_vit.py
 vit_pytorch/mae.py
 vit_pytorch/max_vit.py
 vit_pytorch/mobile_vit.py
 vit_pytorch/mp3.py
 vit_pytorch/mpp.py
+vit_pytorch/na_vit.py
 vit_pytorch/nest.py
 vit_pytorch/parallel_vit.py
 vit_pytorch/pit.py
 vit_pytorch/recorder.py
 vit_pytorch/regionvit.py
 vit_pytorch/rvt.py
 vit_pytorch/scalable_vit.py
```

