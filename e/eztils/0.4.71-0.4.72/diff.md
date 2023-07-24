# Comparing `tmp/eztils-0.4.71.tar.gz` & `tmp/eztils-0.4.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.71.tar", max compression
+gzip compressed data, was "eztils-0.4.72.tar", max compression
```

## Comparing `eztils-0.4.71.tar` & `eztils-0.4.72.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1075 2023-07-24 06:09:32.639912 eztils-0.4.71/LICENSE
--rw-r--r--   0        0        0    12741 2023-07-24 06:09:32.639912 eztils-0.4.71/README.md
--rw-r--r--   0        0        0      542 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/__init__.py
--rw-r--r--   0        0        0     3689 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/dict_operations.py
--rw-r--r--   0        0        0     2246 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/itertools.py
--rw-r--r--   0        0        0     2458 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/logging.py
--rw-r--r--   0        0        0     1432 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/math.py
--rw-r--r--   0        0        0     2812 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/serialization.py
--rw-r--r--   0        0        0     1091 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/structures.py
--rw-r--r--   0        0        0     4296 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/git/__init__.py
--rw-r--r--   0        0        0     1779 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/__init__.py
--rw-r--r--   0        0        0    15657 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/distributions.py
--rw-r--r--   0        0        0      155 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/lightning.py
--rw-r--r--   0        0        0      173 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/math.py
--rw-r--r--   0        0        0     2550 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/modules.py
--rw-r--r--   0        0        0     1420 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/parameters.py
--rw-r--r--   0        0        0     1746 2023-07-24 06:09:32.643912 eztils-0.4.71/eztils/torch/tensor_creators.py
--rw-r--r--   0        0        0     3001 2023-07-24 06:09:32.643912 eztils-0.4.71/eztils/torch/to.py
--rw-r--r--   0        0        0     3611 2023-07-24 06:09:32.643912 eztils-0.4.71/pyproject.toml
--rw-r--r--   0        0        0    13946 1970-01-01 00:00:00.000000 eztils-0.4.71/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-24 06:58:03.175239 eztils-0.4.72/LICENSE
+-rw-r--r--   0        0        0    12741 2023-07-24 06:58:03.179240 eztils-0.4.72/README.md
+-rw-r--r--   0        0        0      542 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/dict_operations.py
+-rw-r--r--   0        0        0     2246 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/itertools.py
+-rw-r--r--   0        0        0     2458 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/logging.py
+-rw-r--r--   0        0        0     1432 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/math.py
+-rw-r--r--   0        0        0     2812 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/serialization.py
+-rw-r--r--   0        0        0     1091 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/structures.py
+-rw-r--r--   0        0        0     4296 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/git/__init__.py
+-rw-r--r--   0        0        0     1779 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/__init__.py
+-rw-r--r--   0        0        0    15646 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/distributions.py
+-rw-r--r--   0        0        0      155 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/lightning.py
+-rw-r--r--   0        0        0      173 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/math.py
+-rw-r--r--   0        0        0     2550 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/modules.py
+-rw-r--r--   0        0        0     1420 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/parameters.py
+-rw-r--r--   0        0        0     1746 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/tensor_creators.py
+-rw-r--r--   0        0        0     3001 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/to.py
+-rw-r--r--   0        0        0     3611 2023-07-24 06:58:03.179240 eztils-0.4.72/pyproject.toml
+-rw-r--r--   0        0        0    13946 1970-01-01 00:00:00.000000 eztils-0.4.72/PKG-INFO
```

### Comparing `eztils-0.4.71/LICENSE` & `eztils-0.4.72/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/README.md` & `eztils-0.4.72/README.md`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/__init__.py` & `eztils-0.4.72/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/default/__init__.py` & `eztils-0.4.72/eztils/default/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/default/dict_operations.py` & `eztils-0.4.72/eztils/default/dict_operations.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/default/itertools.py` & `eztils-0.4.72/eztils/default/itertools.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/default/logging.py` & `eztils-0.4.72/eztils/default/logging.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/default/math.py` & `eztils-0.4.72/eztils/default/math.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/default/serialization.py` & `eztils-0.4.72/eztils/default/serialization.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/default/structures.py` & `eztils-0.4.72/eztils/default/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/git/__init__.py` & `eztils-0.4.72/eztils/git/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/torch/__init__.py` & `eztils-0.4.72/eztils/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/torch/distributions.py` & `eztils-0.4.72/eztils/torch/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from torch.distributions import Bernoulli as TorchBernoulli
 from torch.distributions import Beta as TorchBeta
 from torch.distributions import Distribution as TorchDistribution
 from torch.distributions import Independent as TorchIndependent
 from torch.distributions import Normal as TorchNormal
 from torch.distributions import kl_divergence
 from torch.distributions.utils import _sum_rightmost
-from torchtyping import TensorType
 
 from eztils.default.math import create_stats_ordered_dict
 from eztils.torch.math import atanh
 from eztils.torch.tensor_creators import ones, tensor, zeros
 from eztils.torch.to import to_np
 
 
@@ -221,17 +220,17 @@
     Construct a gaussian mixture model using gumbel softmax for backprop.
     https://bochang.me/blog/posts/pytorch-distributions/#table
 
     """
 
     def __init__(
         self,
-        mean: TensorType["batch", "num_gaussians", "action_dim"],
-        std: TensorType["batch", "num_gaussians", "action_dim"],
-        weights: TensorType["batch", "num_gaussians"],
+        mean,  #: TensorType["batch", "num_gaussians", "action_dim"],
+        std,  #: TensorType["batch", "num_gaussians", "action_dim"],
+        weights,  #: TensorType["batch", "num_gaussians"],
     ):
         if len(mean.shape) == 2:
             mean = mean.unsqueeze(dim=0)
         if len(std.shape) == 2:
             std = std.unsqueeze(dim=0)
         if len(weights.shape) == 1:
             weights = weights.unsqueeze(dim=0)
@@ -352,17 +351,17 @@
         )
         return stats
 
 
 class GaussianMixture(TanhGaussianMixture):
     def __init__(
         self,
-        mean: TensorType["batch", "num_gaussians", "action_dim"],
-        std: TensorType["batch", "num_gaussians", "action_dim"],
-        weights: TensorType["batch", "num_gaussians"],
+        mean,  #: TensorType["batch", "num_gaussians", "action_dim"],
+        std,  #: TensorType["batch", "num_gaussians", "action_dim"],
+        weights,  #: TensorType["batch", "num_gaussians"],
     ):
         super().__init__(mean, std, weights)
 
     def log_prob(self, value):
         assert (
             value.shape[-1] == self.mean.shape[-1]
         ), f"{value} must have shape [{self.batch_shape[0]}, {self.batch_shape[1]}, {self.event_shape[0]}]"
```

### Comparing `eztils-0.4.71/eztils/torch/modules.py` & `eztils-0.4.72/eztils/torch/modules.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/torch/parameters.py` & `eztils-0.4.72/eztils/torch/parameters.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/torch/tensor_creators.py` & `eztils-0.4.72/eztils/torch/tensor_creators.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/eztils/torch/to.py` & `eztils-0.4.72/eztils/torch/to.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.71/pyproject.toml` & `eztils-0.4.72/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.71"
+version = "0.4.72"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `eztils-0.4.71/PKG-INFO` & `eztils-0.4.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.71
+Version: 0.4.72
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

