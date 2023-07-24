# Comparing `tmp/fdfat-0.1.8.tar.gz` & `tmp/fdfat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdfat-0.1.8.tar", last modified: Sun Jul 23 03:30:36 2023, max compression
+gzip compressed data, was "fdfat-0.1.9.tar", last modified: Mon Jul 24 08:54:55 2023, max compression
```

## Comparing `fdfat-0.1.8.tar` & `fdfat-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.154784 fdfat-0.1.8/
--rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.8/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3473 2023-07-23 03:30:36.154618 fdfat-0.1.8/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     2192 2023-07-18 03:39:26.000000 fdfat-0.1.8/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.145483 fdfat-0.1.8/fdfat/
--rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-23 03:29:24.000000 fdfat-0.1.8/fdfat/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.147405 fdfat-0.1.8/fdfat/cfg/
--rw-r--r--   0 ryan       (501) staff       (20)     4751 2023-07-22 12:39:57.000000 fdfat-0.1.8/fdfat/cfg/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     2066 2023-07-22 13:11:56.000000 fdfat-0.1.8/fdfat/cfg/default.yaml
--rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.8/fdfat/cfg/default_data.yaml
--rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.8/fdfat/cfg/yaml_utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.148799 fdfat-0.1.8/fdfat/cli/
--rw-r--r--   0 ryan       (501) staff       (20)     1309 2023-07-19 01:45:05.000000 fdfat-0.1.8/fdfat/cli/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.149069 fdfat-0.1.8/fdfat/data/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.8/fdfat/data/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     7464 2023-07-22 13:09:08.000000 fdfat-0.1.8/fdfat/data/dataloader.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.149961 fdfat-0.1.8/fdfat/engine/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.8/fdfat/engine/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3389 2023-07-19 03:25:31.000000 fdfat-0.1.8/fdfat/engine/base.py
--rw-r--r--   0 ryan       (501) staff       (20)     3311 2023-07-18 03:36:34.000000 fdfat-0.1.8/fdfat/engine/exporter.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.150297 fdfat-0.1.8/fdfat/engine/loop/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.8/fdfat/engine/loop/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3782 2023-07-23 01:59:53.000000 fdfat-0.1.8/fdfat/engine/loop/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     3458 2023-07-23 02:00:13.000000 fdfat-0.1.8/fdfat/engine/loop/validator.py
--rw-r--r--   0 ryan       (501) staff       (20)     1535 2023-07-19 01:44:18.000000 fdfat-0.1.8/fdfat/engine/predictor.py
--rw-r--r--   0 ryan       (501) staff       (20)     6611 2023-07-19 01:06:49.000000 fdfat-0.1.8/fdfat/engine/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     3020 2023-07-19 06:42:33.000000 fdfat-0.1.8/fdfat/engine/validator.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.150501 fdfat-0.1.8/fdfat/metric/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.8/fdfat/metric/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-19 05:25:08.000000 fdfat-0.1.8/fdfat/metric/metric.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.151649 fdfat-0.1.8/fdfat/nn/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.8/fdfat/nn/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3580 2023-07-18 03:43:41.000000 fdfat-0.1.8/fdfat/nn/conv.py
--rw-r--r--   0 ryan       (501) staff       (20)     4885 2023-07-19 03:56:24.000000 fdfat-0.1.8/fdfat/nn/model.py
--rw-r--r--   0 ryan       (501) staff       (20)     5050 2023-07-18 03:43:18.000000 fdfat-0.1.8/fdfat/nn/module.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.152654 fdfat-0.1.8/fdfat/utils/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.8/fdfat/utils/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.8/fdfat/utils/logger.py
--rw-r--r--   0 ryan       (501) staff       (20)     7948 2023-07-17 10:24:57.000000 fdfat-0.1.8/fdfat/utils/model_utils.py
--rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-19 05:38:27.000000 fdfat-0.1.8/fdfat/utils/pose_estimation.py
--rw-r--r--   0 ryan       (501) staff       (20)     6137 2023-07-19 06:45:12.000000 fdfat-0.1.8/fdfat/utils/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-23 03:30:36.146200 fdfat-0.1.8/fdfat.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3473 2023-07-23 03:30:36.000000 fdfat-0.1.8/fdfat.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      893 2023-07-23 03:30:36.000000 fdfat-0.1.8/fdfat.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-23 03:30:36.000000 fdfat-0.1.8/fdfat.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-23 03:30:36.000000 fdfat-0.1.8/fdfat.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-23 03:30:36.000000 fdfat-0.1.8/fdfat.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-23 03:30:36.000000 fdfat-0.1.8/fdfat.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.8/requirements.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-23 03:30:36.154846 fdfat-0.1.8/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.8/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.531970 fdfat-0.1.9/
+-rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.9/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3473 2023-07-24 08:54:55.531830 fdfat-0.1.9/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2192 2023-07-18 03:39:26.000000 fdfat-0.1.9/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.512013 fdfat-0.1.9/fdfat/
+-rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-24 08:54:34.000000 fdfat-0.1.9/fdfat/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.516304 fdfat-0.1.9/fdfat/cfg/
+-rw-r--r--   0 ryan       (501) staff       (20)     4751 2023-07-22 12:39:57.000000 fdfat-0.1.9/fdfat/cfg/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2066 2023-07-22 13:11:56.000000 fdfat-0.1.9/fdfat/cfg/default.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.9/fdfat/cfg/default_data.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.9/fdfat/cfg/yaml_utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.516802 fdfat-0.1.9/fdfat/cli/
+-rw-r--r--   0 ryan       (501) staff       (20)     1309 2023-07-19 01:45:05.000000 fdfat-0.1.9/fdfat/cli/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.517232 fdfat-0.1.9/fdfat/data/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.9/fdfat/data/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7464 2023-07-22 13:09:08.000000 fdfat-0.1.9/fdfat/data/dataloader.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.521264 fdfat-0.1.9/fdfat/engine/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.9/fdfat/engine/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3389 2023-07-19 03:25:31.000000 fdfat-0.1.9/fdfat/engine/base.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3311 2023-07-18 03:36:34.000000 fdfat-0.1.9/fdfat/engine/exporter.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.523475 fdfat-0.1.9/fdfat/engine/loop/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.9/fdfat/engine/loop/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3782 2023-07-23 01:59:53.000000 fdfat-0.1.9/fdfat/engine/loop/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3458 2023-07-23 02:00:13.000000 fdfat-0.1.9/fdfat/engine/loop/validator.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1535 2023-07-19 01:44:18.000000 fdfat-0.1.9/fdfat/engine/predictor.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6611 2023-07-19 01:06:49.000000 fdfat-0.1.9/fdfat/engine/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3020 2023-07-19 06:42:33.000000 fdfat-0.1.9/fdfat/engine/validator.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.524600 fdfat-0.1.9/fdfat/metric/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.9/fdfat/metric/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-19 05:25:08.000000 fdfat-0.1.9/fdfat/metric/metric.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.528988 fdfat-0.1.9/fdfat/nn/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.9/fdfat/nn/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5018 2023-07-24 08:33:43.000000 fdfat-0.1.9/fdfat/nn/conv.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7844 2023-07-24 08:52:00.000000 fdfat-0.1.9/fdfat/nn/model.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4732 2023-07-23 06:50:57.000000 fdfat-0.1.9/fdfat/nn/module.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4546 2023-07-24 05:05:41.000000 fdfat-0.1.9/fdfat/nn/module2.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4979 2023-07-24 08:49:54.000000 fdfat-0.1.9/fdfat/nn/module3.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.531397 fdfat-0.1.9/fdfat/utils/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.9/fdfat/utils/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.9/fdfat/utils/logger.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7948 2023-07-17 10:24:57.000000 fdfat-0.1.9/fdfat/utils/model_utils.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-19 05:38:27.000000 fdfat-0.1.9/fdfat/utils/pose_estimation.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6137 2023-07-19 06:45:12.000000 fdfat-0.1.9/fdfat/utils/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 08:54:55.513827 fdfat-0.1.9/fdfat.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3473 2023-07-24 08:54:55.000000 fdfat-0.1.9/fdfat.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      933 2023-07-24 08:54:55.000000 fdfat-0.1.9/fdfat.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-24 08:54:55.000000 fdfat-0.1.9/fdfat.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-24 08:54:55.000000 fdfat-0.1.9/fdfat.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-24 08:54:55.000000 fdfat-0.1.9/fdfat.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-24 08:54:55.000000 fdfat-0.1.9/fdfat.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.9/requirements.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-24 08:54:55.532020 fdfat-0.1.9/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.9/setup.py
```

### Comparing `fdfat-0.1.8/PKG-INFO` & `fdfat-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.8/README.md` & `fdfat-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/cfg/__init__.py` & `fdfat-0.1.9/fdfat/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/cfg/default.yaml` & `fdfat-0.1.9/fdfat/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/cfg/yaml_utils.py` & `fdfat-0.1.9/fdfat/cfg/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/cli/__init__.py` & `fdfat-0.1.9/fdfat/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/data/dataloader.py` & `fdfat-0.1.9/fdfat/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/engine/base.py` & `fdfat-0.1.9/fdfat/engine/base.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/engine/exporter.py` & `fdfat-0.1.9/fdfat/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/engine/loop/trainer.py` & `fdfat-0.1.9/fdfat/engine/loop/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/engine/loop/validator.py` & `fdfat-0.1.9/fdfat/engine/loop/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/engine/predictor.py` & `fdfat-0.1.9/fdfat/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/engine/trainer.py` & `fdfat-0.1.9/fdfat/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/engine/validator.py` & `fdfat-0.1.9/fdfat/engine/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/metric/metric.py` & `fdfat-0.1.9/fdfat/metric/metric.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/nn/conv.py` & `fdfat-0.1.9/fdfat/nn/conv.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 
 import torch
 from torch import nn
 
-__all__ = ['autopad', 'Conv', 'DWConv', 'Concat', 'IdentifyBlock', 'initialize_weights']
+__all__ = ['autopad', 'Conv', 'DWConv', 'Concat', 'IdentifyBlock', 'C2f', 'Bottleneck', 'initialize_weights']
 
 def initialize_weights(model):
     """Initialize model weights to random values."""
     for m in model.modules():
         t = type(m)
         if t is nn.Conv2d:
             pass  # nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='relu')
@@ -32,16 +32,14 @@
     def __init__(self, c1, c2, k=1, s=1, p=None, g=1, d=1, act=True):
         """Initialize Conv layer with given arguments including activation."""
         super().__init__()
         self.conv = nn.Conv2d(c1, c2, k, s, autopad(k, p, d), groups=g, dilation=d, bias=False)
         self.bn = nn.BatchNorm2d(c2)
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
 
-        # initialize_weights(self)
-
     def forward(self, x):
         """Apply convolution, batch normalization and activation to input tensor."""
         return self.act(self.bn(self.conv(x)))
 
     def forward_fuse(self, x):
         """Perform transposed convolution of 2D data."""
         return self.act(self.conv(x))
@@ -86,21 +84,55 @@
         self.conv3 = Conv(expand_ch, out_ch, k=1, act=False)
 
         self.need_fuse = in_ch == out_ch
         self.need_pool = stride == 2
         if self.need_fuse and self.need_pool:
             self.pool = nn.MaxPool2d(2, stride=2)
 
-        # initialize_weights(self)
-
     def forward(self, x):
         
         ex = self.conv1(x)
         de = self.conv2(ex)
         sq = self.conv3(de)
 
         if self.need_fuse:
             if self.need_pool:
                 x = self.pool(x)
             return sq + x
         else:
-            return sq
+            return sq
+
+class Bottleneck(nn.Module):
+    """Standard bottleneck."""
+
+    def __init__(self, c1, c2, shortcut=True, g=1, k=(3, 3), e=0.5):  # ch_in, ch_out, shortcut, groups, kernels, expand
+        super().__init__()
+        c_ = int(c2 * e)  # hidden channels
+        self.cv1 = Conv(c1, c_, k[0], 1)
+        self.cv2 = Conv(c_, c2, k[1], 1, g=g)
+        self.add = shortcut and c1 == c2
+
+    def forward(self, x):
+        """'forward()' applies the YOLOv5 FPN to input data."""
+        return x + self.cv2(self.cv1(x)) if self.add else self.cv2(self.cv1(x))
+
+class C2f(nn.Module):
+    """CSP Bottleneck with 2 convolutions."""
+
+    def __init__(self, c1, c2, n=1, shortcut=False, g=1, e=0.5):  # ch_in, ch_out, number, shortcut, groups, expansion
+        super().__init__()
+        self.c = int(c2 * e)  # hidden channels
+        self.cv1 = Conv(c1, 2 * self.c, 1, 1)
+        self.cv2 = Conv((2 + n) * self.c, c2, 1)  # optional act=FReLU(c2)
+        self.m = nn.ModuleList(Bottleneck(self.c, self.c, shortcut, g, k=((3, 3), (3, 3)), e=1.0) for _ in range(n))
+
+    def forward(self, x):
+        """Forward pass through C2f layer."""
+        y = list(self.cv1(x).chunk(2, 1))
+        y.extend(m(y[-1]) for m in self.m)
+        return self.cv2(torch.cat(y, 1))
+
+    def forward_split(self, x):
+        """Forward pass using split() instead of chunk()."""
+        y = list(self.cv1(x).split((self.c, self.c), 1))
+        y.extend(m(y[-1]) for m in self.m)
+        return self.cv2(torch.cat(y, 1))
```

### Comparing `fdfat-0.1.8/fdfat/nn/model.py` & `fdfat-0.1.9/fdfat/nn/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from torch import nn
 
 from fdfat.utils.model_utils import intersect_dicts
 from fdfat.utils.logger import LOGGER
 
 from .conv import *
 from . import module
+from . import module2
+from . import module3
 
 class BaseModel(nn.Module):
 
     def __init__(self):
         super().__init__()
 
     def forward(self, x):
@@ -78,14 +80,110 @@
         return x
 
 class LightWeightModelSiLU(LightWeightModel):
 
     def __init__(self, imgz=128, muliplier=1, pose_rotation=False, act=True):
         super().__init__(imgz=imgz, muliplier=muliplier, pose_rotation=pose_rotation, act=nn.SiLU())
 
+class LightWeightPyramicModel(BaseModel):
+
+    default_act = nn.ReLU6()  # default activation
+
+    def __init__(self, imgz=128, muliplier=1, pose_rotation=False, act=True):
+        super().__init__()
+        self.pose_rotation = pose_rotation
+
+        self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
+
+        # backbone, output size = size/4
+        self.backbone = module2.LightWeightBackbone(muliplier=muliplier, act=self.act)
+
+        # mainstream, output size:
+        # x1 = size/8
+        # x2 = size/16
+        # x3 = size/16
+        self.mainstream = module2.MainStreamModule(muliplier=muliplier, act=self.act)
+
+        if pose_rotation:
+            self.aux = module2.AuxiliaryBackbone(int(32*muliplier), 3, muliplier=muliplier, act=self.act)
+            
+        output_ch = int((64 + 128 + 128)*muliplier)
+        self.logit = module2.FERegress(output_ch, 70*2)
+
+        self.concat = Concat()
+
+        initialize_weights(self)
+
+    def forward(self, x):
+
+        x = self.backbone(x)
+        
+        if self.pose_rotation:
+            aux = self.aux(x)
+
+        x = self.mainstream(x)
+        
+        x = self.logit(x)
+
+        if self.pose_rotation:
+            x = self.concat([x, aux])
+
+        return x
+
+class LightWeightPyramicModelSiLU(LightWeightPyramicModel):
+
+    def __init__(self, imgz=128, muliplier=1, pose_rotation=False, act=True):
+        super().__init__(imgz=imgz, muliplier=muliplier, pose_rotation=pose_rotation, act=nn.SiLU())
+
+class LightWeightCSPModel(BaseModel):
+
+    default_act = nn.ReLU6()  # default activation
+
+    def __init__(self, imgz=128, muliplier=1, pose_rotation=False, act=True):
+        super().__init__()
+        self.pose_rotation = pose_rotation
+
+        self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
+
+        # backbone, output size = size/4
+        self.backbone = module3.LightWeightBackbone(muliplier=muliplier, act=self.act)
+
+        self.mainstream = module3.MainStreamModule(muliplier=muliplier, act=self.act)
+
+        if pose_rotation:
+            self.aux = module3.AuxiliaryBackbone(int(32*muliplier), 3, muliplier=muliplier, act=self.act)
+            
+        output_ch = int((64 + 96 + 96)*muliplier)
+        self.logit = module3.FERegress(output_ch, 70*2)
+
+        self.concat = Concat()
+
+        initialize_weights(self)
+
+    def forward(self, x):
+
+        x = self.backbone(x)
+        
+        if self.pose_rotation:
+            aux = self.aux(x)
+
+        x = self.mainstream(x)
+        
+        x = self.logit(x)
+
+        if self.pose_rotation:
+            x = self.concat([x, aux])
+
+        return x
+
+class LightWeightCSPModelSiLU(LightWeightCSPModel):
+
+    def __init__(self, imgz=128, muliplier=1, pose_rotation=False, act=True):
+        super().__init__(imgz=imgz, muliplier=muliplier, pose_rotation=pose_rotation, act=nn.SiLU())
+
 class LandmarkModel(BaseModel):
 
     def __init__(self, imgz=128, muliplier=1, pose_rotation=False):
         super().__init__()
         
         self.stack1 = nn.Sequential(
             nn.Conv2d( 3, int(32*muliplier), 3, stride=2, padding=2),
```

### Comparing `fdfat-0.1.8/fdfat/nn/module.py` & `fdfat-0.1.9/fdfat/nn/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 
         self.conv21 = IdentifyBlock(16, int(16*muliplier), expand_rate, stride=2, act=self.act)
         self.conv22 = IdentifyBlock(int(16*muliplier), int(16*muliplier), expand_rate, act=self.act)
         self.conv23 = IdentifyBlock(int(16*muliplier), int(16*muliplier), expand_rate, act=self.act)
         self.conv24 = IdentifyBlock(int(16*muliplier), int(16*muliplier), expand_rate, act=self.act)
         self.conv25 = IdentifyBlock(int(16*muliplier), int(16*muliplier), expand_rate, act=self.act)
 
-        # initialize_weights(self)
-
     def forward(self, x):
 
         x = self.conv11(x)
         x = self.conv21(x)
         x = self.conv22(x)
         x = self.conv23(x)
         x = self.conv24(x)
@@ -62,16 +60,14 @@
         self.stack2 = nn.Sequential(
             nn.Linear(int(128*muliplier), out_ch*3),
             nn.Tanh(),
             nn.Linear(out_ch*3, out_ch),
             nn.Tanh()
         )
 
-        # initialize_weights(self)
-
     def forward(self, x):
 
         x = self.stack1(x)
         x = x.flatten(start_dim=1)
         x = self.stack2(x)
 
         return x
@@ -92,22 +88,18 @@
         self.conv24 = IdentifyBlock(int(64*muliplier), int(64*muliplier), expand_rate*2, stride=1, act=self.act)
         self.conv25 = IdentifyBlock(int(64*muliplier), int(64*muliplier), expand_rate*2, stride=1, act=self.act)
 
         # Pyramic scale
         self.convp1 = IdentifyBlock(int(64*muliplier), int(128*muliplier), expand_rate, stride=1, act=self.act)
         self.convp2 = IdentifyBlock(int(128*muliplier), int(128*muliplier), expand_rate, stride=2, act=self.act)
         self.convp3 = IdentifyBlock(int(128*muliplier), int(128*muliplier), expand_rate, stride=1, act=self.act)
-        # self.convp2 = Conv(int(128*muliplier), int(128*muliplier), k=3, s=2, act=nn.SiLU())
-        # self.convp3 = Conv(int(128*muliplier), int(128*muliplier), k=3, act=nn.SiLU())
 
         self.concat = Concat()
         self.global_pool = nn.AdaptiveAvgPool2d((1, 1))
 
-        # initialize_weights(self)
-
     def forward(self, x):
 
         x = self.conv11(x)
 
         x = self.conv21(x)
         x = self.conv22(x)
         x = self.conv23(x)
@@ -135,12 +127,11 @@
         self.stack = nn.Sequential(
             nn.Linear(in_ch, int(out_ch*2)),
             nn.Tanh(),
             nn.Linear(int(out_ch*2), out_ch),
             nn.Tanh()
         )
 
-        # initialize_weights(self)
-
     def forward(self, x):
         x = self.stack(x)
-        return x
+        return x
+
```

### Comparing `fdfat-0.1.8/fdfat/utils/logger.py` & `fdfat-0.1.9/fdfat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/utils/model_utils.py` & `fdfat-0.1.9/fdfat/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/utils/pose_estimation.py` & `fdfat-0.1.9/fdfat/utils/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat/utils/utils.py` & `fdfat-0.1.9/fdfat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/fdfat.egg-info/PKG-INFO` & `fdfat-0.1.9/fdfat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.8/fdfat.egg-info/SOURCES.txt` & `fdfat-0.1.9/fdfat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,12 +27,14 @@
 fdfat/engine/loop/validator.py
 fdfat/metric/__init__.py
 fdfat/metric/metric.py
 fdfat/nn/__init__.py
 fdfat/nn/conv.py
 fdfat/nn/model.py
 fdfat/nn/module.py
+fdfat/nn/module2.py
+fdfat/nn/module3.py
 fdfat/utils/__init__.py
 fdfat/utils/logger.py
 fdfat/utils/model_utils.py
 fdfat/utils/pose_estimation.py
 fdfat/utils/utils.py
```

### Comparing `fdfat-0.1.8/requirements.txt` & `fdfat-0.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.8/setup.py` & `fdfat-0.1.9/setup.py`

 * *Files identical despite different names*

