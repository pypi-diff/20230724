# Comparing `tmp/torchmanager-1.1.4.tar.gz` & `tmp/torchmanager-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-1.1.4.tar", max compression
+gzip compressed data, was "torchmanager-1.1.5.tar", max compression
```

## Comparing `torchmanager-1.1.4.tar` & `torchmanager-1.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1318 2023-06-12 21:40:08.180158 torchmanager-1.1.4/LICENSE
--rw-r--r--   0        0        0      616 2023-06-29 21:59:25.541911 torchmanager-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      281 2023-06-29 21:58:18.783925 torchmanager-1.1.4/torchmanager/__init__.py
--rw-r--r--   0        0        0    11076 2023-06-29 21:59:25.543096 torchmanager-1.1.4/torchmanager/basic.py
--rw-r--r--   0        0        0      659 2023-06-29 21:59:25.543478 torchmanager-1.1.4/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4248 2023-06-29 21:59:25.543792 torchmanager-1.1.4/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4686 2023-06-29 21:59:25.544093 torchmanager-1.1.4/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3522 2023-06-29 21:59:25.548795 torchmanager-1.1.4/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1984 2023-06-29 21:59:25.549314 torchmanager-1.1.4/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4854 2023-06-29 21:59:25.549619 torchmanager-1.1.4/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2238 2023-06-29 21:59:25.549956 torchmanager-1.1.4/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2454 2023-06-29 21:59:25.550248 torchmanager-1.1.4/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      963 2023-06-29 21:58:18.786227 torchmanager-1.1.4/torchmanager/compatibility.py
--rw-r--r--   0        0        0       85 2023-06-28 18:44:00.539650 torchmanager-1.1.4/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6962 2023-06-29 21:58:18.786430 torchmanager-1.1.4/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2236 2023-06-29 21:58:18.786607 torchmanager-1.1.4/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      171 2023-06-29 21:58:18.786797 torchmanager-1.1.4/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5386 2023-06-29 21:58:18.786993 torchmanager-1.1.4/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1044 2023-06-29 21:58:18.787165 torchmanager-1.1.4/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     7061 2023-06-29 21:58:18.787416 torchmanager-1.1.4/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     2381 2023-06-29 21:58:18.787572 torchmanager-1.1.4/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      234 2023-06-29 21:58:18.787736 torchmanager-1.1.4/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     3272 2023-06-29 21:58:18.787899 torchmanager-1.1.4/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     2546 2023-06-29 21:58:18.788079 torchmanager-1.1.4/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     2633 2023-06-29 21:59:25.550538 torchmanager-1.1.4/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4000 2023-06-29 21:58:18.788645 torchmanager-1.1.4/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     9401 2023-06-29 21:58:18.789063 torchmanager-1.1.4/torchmanager/testing.py
--rw-r--r--   0        0        0      191 2023-06-29 21:58:18.789324 torchmanager-1.1.4/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4986 2023-06-29 21:58:18.789722 torchmanager-1.1.4/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0     2037 2023-06-29 21:58:18.789979 torchmanager-1.1.4/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    14893 2023-06-29 21:58:18.790239 torchmanager-1.1.4/torchmanager/training.py
--rw-r--r--   0        0        0      443 2023-06-29 21:58:18.790431 torchmanager-1.1.4/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      114 2023-06-29 21:58:18.790649 torchmanager-1.1.4/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     5587 2023-06-29 21:58:18.790848 torchmanager-1.1.4/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-06-28 18:44:00.542743 torchmanager-1.1.4/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-06-28 18:44:00.542862 torchmanager-1.1.4/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-06-29 21:58:18.791030 torchmanager-1.1.4/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-06-28 18:44:00.543066 torchmanager-1.1.4/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     2728 2023-06-29 21:58:18.791203 torchmanager-1.1.4/torchmanager_core/protocols.py
--rw-r--r--   0        0        0      204 2023-06-28 18:44:00.543293 torchmanager-1.1.4/torchmanager_core/typing.py
--rw-r--r--   0        0        0     7356 2023-06-29 21:59:25.550792 torchmanager-1.1.4/torchmanager_core/version.py
--rw-r--r--   0        0        0      163 2023-06-29 21:59:25.551054 torchmanager-1.1.4/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-06-28 18:44:00.543729 torchmanager-1.1.4/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 torchmanager-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-07-13 17:22:38.863844 torchmanager-1.1.5/LICENSE
+-rw-r--r--   0        0        0      616 2023-07-24 18:20:42.158872 torchmanager-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      281 2023-07-24 18:20:29.306791 torchmanager-1.1.5/torchmanager/__init__.py
+-rw-r--r--   0        0        0    11076 2023-07-24 18:20:29.307075 torchmanager-1.1.5/torchmanager/basic.py
+-rw-r--r--   0        0        0      659 2023-07-24 18:20:29.307303 torchmanager-1.1.5/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4248 2023-07-24 18:20:29.307524 torchmanager-1.1.5/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4686 2023-07-24 18:20:29.307738 torchmanager-1.1.5/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3522 2023-07-19 18:01:53.901655 torchmanager-1.1.5/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1984 2023-07-24 18:20:29.307933 torchmanager-1.1.5/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4854 2023-07-24 18:20:29.308143 torchmanager-1.1.5/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2238 2023-07-24 18:20:29.308326 torchmanager-1.1.5/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2454 2023-07-24 18:20:29.308508 torchmanager-1.1.5/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      963 2023-07-24 18:20:29.308686 torchmanager-1.1.5/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       85 2023-07-19 18:01:53.902732 torchmanager-1.1.5/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6962 2023-07-24 18:20:29.308901 torchmanager-1.1.5/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2236 2023-07-24 18:20:29.309114 torchmanager-1.1.5/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      195 2023-07-24 18:20:42.159166 torchmanager-1.1.5/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5386 2023-07-24 18:20:29.309487 torchmanager-1.1.5/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1351 2023-07-24 18:20:42.159410 torchmanager-1.1.5/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     7177 2023-07-24 18:20:42.159624 torchmanager-1.1.5/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     2381 2023-07-24 18:20:29.310038 torchmanager-1.1.5/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      234 2023-07-24 18:20:29.310249 torchmanager-1.1.5/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     3272 2023-07-24 18:20:29.310449 torchmanager-1.1.5/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     2546 2023-07-24 18:20:29.310667 torchmanager-1.1.5/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     2635 2023-07-24 18:20:42.159953 torchmanager-1.1.5/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4000 2023-07-24 18:20:29.311079 torchmanager-1.1.5/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     9401 2023-07-24 18:20:29.311297 torchmanager-1.1.5/torchmanager/testing.py
+-rw-r--r--   0        0        0      191 2023-07-24 18:20:29.311471 torchmanager-1.1.5/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4986 2023-07-24 18:20:29.311709 torchmanager-1.1.5/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0     2037 2023-07-24 18:20:29.311938 torchmanager-1.1.5/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    14893 2023-07-24 18:20:29.312204 torchmanager-1.1.5/torchmanager/training.py
+-rw-r--r--   0        0        0      443 2023-07-24 18:20:29.312496 torchmanager-1.1.5/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-24 18:20:29.312713 torchmanager-1.1.5/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     5587 2023-07-24 18:20:29.312937 torchmanager-1.1.5/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-07-19 18:01:53.907517 torchmanager-1.1.5/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-07-24 18:20:29.313320 torchmanager-1.1.5/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-07-24 18:20:29.313473 torchmanager-1.1.5/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-07-19 18:01:53.907838 torchmanager-1.1.5/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     2728 2023-07-24 18:20:29.313655 torchmanager-1.1.5/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0      204 2023-07-19 18:01:53.908282 torchmanager-1.1.5/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     7356 2023-07-24 18:20:42.160278 torchmanager-1.1.5/torchmanager_core/version.py
+-rw-r--r--   0        0        0      163 2023-07-24 18:20:29.314043 torchmanager-1.1.5/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-19 18:01:53.908597 torchmanager-1.1.5/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 torchmanager-1.1.5/PKG-INFO
```

### Comparing `torchmanager-1.1.4/LICENSE` & `torchmanager-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/pyproject.toml` & `torchmanager-1.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "torchmanager"
-version = "1.1.4"
-description = "PyTorch Training Manager v1.1.4"
+version = "1.1.5"
+description = "PyTorch Training Manager v1.1.5"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
```

### Comparing `torchmanager-1.1.4/torchmanager/basic.py` & `torchmanager-1.1.5/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/callbacks/__init__.py` & `torchmanager-1.1.5/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/callbacks/callback.py` & `torchmanager-1.1.5/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/callbacks/ckpt.py` & `torchmanager-1.1.5/torchmanager/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/callbacks/dynamic.py` & `torchmanager-1.1.5/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/callbacks/early_stop.py` & `torchmanager-1.1.5/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/callbacks/experiment.py` & `torchmanager-1.1.5/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/callbacks/lr.py` & `torchmanager-1.1.5/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/callbacks/tensorboard.py` & `torchmanager-1.1.5/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/compatibility.py` & `torchmanager-1.1.5/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/data/dataset.py` & `torchmanager-1.1.5/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/data/sliding.py` & `torchmanager-1.1.5/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/losses/cross_entropy.py` & `torchmanager-1.1.5/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/losses/dice.py` & `torchmanager-1.1.5/torchmanager/losses/dice.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,30 +6,36 @@
 
 class Dice(Loss):
     """
     The dice loss
 
     * extends: `.loss.Loss`
     """
-    _smooth: int
+    _dim: int
+    _smooth: float
     _softmax_input: bool
 
-    def __init__(self, smooth: int = 1, softmax_input: bool = True, **kwargs: Any) -> None:
+    def __init__(self, dim: int = 1, smooth: float = 1e-6, softmax_input: bool = True, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
-            - smooth: An `int` of smooth value to avoid dividing zero
+            - dim: An `int` of class dimension
+            - smooth: An `float` of smooth value to avoid dividing zero
             - softmax_input: A `bool` flag of if softmax the input
         """
         super().__init__(**kwargs)
+        self._dim = dim
         self._smooth = smooth
         self._softmax_input = softmax_input
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # softmax activation
-        input = F.softmax(input).view(-1) if self._softmax_input else input.view(-1)
+        num_classes = input.shape[self._dim]
+        input = input.softmax(self._dim).view(-1) if self._softmax_input else input.view(-1)
+        target = F.one_hot(target.view(-1), num_classes)
+        assert isinstance(target, torch.Tensor), "Target is not a valid `torch.Tensor`."
         target = target.view(-1)
 
         # calculate dice
         intersection = input * target
         return (2 * intersection.sum() + self._smooth) / (input.sum() + target.sum() + self._smooth)
```

### Comparing `torchmanager-1.1.4/torchmanager/losses/loss.py` & `torchmanager-1.1.5/torchmanager/losses/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         """
         super().__init__(loss_fn, target=target)
         self.weight = weight
 
     def __call__(self, input: Any, target: Any) -> torch.Tensor:
         m: torch.Tensor = super().__call__(input, target) * self.weight
         self._results[-1] *= self.weight
+        assert m.numel() == 1, _raise(TypeError(f"The returned loss must be a scalar tensor, got shape {m.shape}"))
         return m
 
     def forward(self, input: Any, target: Any) -> torch.Tensor:
         return super().forward(input, target)
 
 
 class MultiLosses(Loss):
```

### Comparing `torchmanager-1.1.4/torchmanager/losses/mse.py` & `torchmanager-1.1.5/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/metrics/accuracy.py` & `torchmanager-1.1.5/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/metrics/conf_met.py` & `torchmanager-1.1.5/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/metrics/iou.py` & `torchmanager-1.1.5/torchmanager/metrics/iou.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         assert dim > 0, _raise(ValueError(f"The dimension must be a positive number, got {dim}."))
         assert threshold >= 0 and threshold <= 1, _raise(ValueError(f"The threshold must be in range [0,1], got {threshold}."))
         self._dim = dim
         self._smooth = smooth
         self._threshold = threshold
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        input = input.argmax(self._dim) if input.shape[self._dim] > 1 else input > 0
+        input = input.argmax(self._dim) if input.shape[self._dim] > 1 else input > 0.5
         intersection = (input & target).float().sum()
         union = (input | target).float().sum()
         iou = (intersection + self._smooth) / (union + self._smooth)
         thresholded = torch.clamp(10 / (1 - self._threshold) * (iou - self._threshold), 0, 10).ceil() / 10
         return thresholded
```

### Comparing `torchmanager-1.1.4/torchmanager/metrics/metric.py` & `torchmanager-1.1.5/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/testing.py` & `torchmanager-1.1.5/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/train/checkpoint.py` & `torchmanager-1.1.5/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/train/learning_rate.py` & `torchmanager-1.1.5/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager/training.py` & `torchmanager-1.1.5/torchmanager/training.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager_core/devices/device.py` & `torchmanager-1.1.5/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager_core/errors/train.py` & `torchmanager-1.1.5/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager_core/protocols.py` & `torchmanager-1.1.5/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.4/torchmanager_core/version.py` & `torchmanager-1.1.5/torchmanager_core/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,16 +140,16 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.1")
-CURRENT = Version("v1.1.4")
-DESCRIPTION: str = "PyTorch Training Manager v1.1.4"
+CURRENT = Version("v1.1.5")
+DESCRIPTION: str = "PyTorch Training Manager v1.1.5"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager-1.1.4/PKG-INFO` & `torchmanager-1.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager
-Version: 1.1.4
-Summary: PyTorch Training Manager v1.1.4
+Version: 1.1.5
+Summary: PyTorch Training Manager v1.1.5
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

