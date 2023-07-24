# Comparing `tmp/gigagan-pytorch-0.2.4.tar.gz` & `tmp/gigagan-pytorch-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.2.4.tar", last modified: Mon Jul 24 16:39:54 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.2.5.tar", last modified: Mon Jul 24 16:41:33 2023, max compression
```

## Comparing `gigagan-pytorch-0.2.4.tar` & `gigagan-pytorch-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:54.188828 gigagan-pytorch-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 16:39:54.188828 gigagan-pytorch-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:54.188828 gigagan-pytorch-0.2.4/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    83586 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:39:54.188828 gigagan-pytorch-0.2.4/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 16:39:54.000000 gigagan-pytorch-0.2.4/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 16:39:54.000000 gigagan-pytorch-0.2.4/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:39:54.000000 gigagan-pytorch-0.2.4/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 16:39:54.000000 gigagan-pytorch-0.2.4/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 16:39:54.000000 gigagan-pytorch-0.2.4/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:39:54.188828 gigagan-pytorch-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 16:39:42.000000 gigagan-pytorch-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83641 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/setup.py
```

### Comparing `gigagan-pytorch-0.2.4/LICENSE` & `gigagan-pytorch-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.4/PKG-INFO` & `gigagan-pytorch-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.2.4
+Version: 0.2.5
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.2.4/README.md` & `gigagan-pytorch-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.4/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.2.5/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.4/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.2.5/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.4/gigagan_pytorch/data.py` & `gigagan-pytorch-0.2.5/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.4/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.2.5/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -2043,16 +2043,17 @@
 
         self.train_dl = self.accelerator.prepare(self.train_dl)
 
     # generate function
 
     @torch.inference_mode()
     def generate(self, *args, **kwargs):
-        self.G_ema.eval()
-        return self.G_ema(*args, **kwargs)
+        model = self.G_ema if self.has_ema_generator else self.G
+        model.eval()
+        return model(*args, **kwargs)
 
     # create EMA generator
 
     def create_ema_generator(
         self,
         update_every = 10,
         update_after_step = 100,
```

### Comparing `gigagan-pytorch-0.2.4/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.2.5/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.4/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.2.5/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.4/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.2.5/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.4/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.2.4
+Version: 0.2.5
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.2.4/setup.py` & `gigagan-pytorch-0.2.5/setup.py`

 * *Files identical despite different names*

