# Comparing `tmp/fast_perceiver-0.1.1.tar.gz` & `tmp/fast_perceiver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_perceiver-0.1.1.tar", max compression
+gzip compressed data, was "fast_perceiver-0.1.2.tar", max compression
```

## Comparing `fast_perceiver-0.1.1.tar` & `fast_perceiver-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6395 2023-07-23 22:15:29.848472 fast_perceiver-0.1.1/README.md
--rw-r--r--   0        0        0       30 2023-07-23 21:11:38.318260 fast_perceiver-0.1.1/fast_perceiver/__init__.py
--rw-r--r--   0        0        0     6721 2023-07-23 22:19:23.326326 fast_perceiver-0.1.1/fast_perceiver/modules.py
--rw-r--r--   0        0        0      385 2023-07-23 20:57:41.749091 fast_perceiver-0.1.1/fast_perceiver/utils.py
--rw-r--r--   0        0        0      752 2023-07-23 22:38:05.028207 fast_perceiver-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6920 1970-01-01 00:00:00.000000 fast_perceiver-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6395 2023-07-23 22:15:29.848472 fast_perceiver-0.1.2/README.md
+-rw-r--r--   0        0        0       30 2023-07-23 21:11:38.318260 fast_perceiver-0.1.2/fast_perceiver/__init__.py
+-rw-r--r--   0        0        0     6721 2023-07-23 22:19:23.326326 fast_perceiver-0.1.2/fast_perceiver/modules.py
+-rw-r--r--   0        0        0      385 2023-07-23 20:57:41.749091 fast_perceiver-0.1.2/fast_perceiver/utils.py
+-rw-r--r--   0        0        0      772 2023-07-23 22:40:16.435030 fast_perceiver-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6960 1970-01-01 00:00:00.000000 fast_perceiver-0.1.2/PKG-INFO
```

### Comparing `fast_perceiver-0.1.1/README.md` & `fast_perceiver-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fast_perceiver-0.1.1/fast_perceiver/modules.py` & `fast_perceiver-0.1.2/fast_perceiver/modules.py`

 * *Files identical despite different names*

### Comparing `fast_perceiver-0.1.1/pyproject.toml` & `fast_perceiver-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "fast-perceiver"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Kristian Klemon <kristian.klemon@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fast_perceiver"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 torch = {version = "^2.0.1", source = "pytorch-gpu-src"}
 torchvision = {version = "^0.15.2", source = "pytorch-gpu-src"}
 einops = "^0.6.1"
 flash-attn = "^2.0.0.post1"
+packaging = "^23.1"
 
 
 [[tool.poetry.source]]
 name = "pytorch-gpu-src"
 url = "https://download.pytorch.org/whl/cu118"
 priority = "explicit"
```

### Comparing `fast_perceiver-0.1.1/PKG-INFO` & `fast_perceiver-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: fast-perceiver
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Kristian Klemon
 Author-email: kristian.klemon@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: einops (>=0.6.1,<0.7.0)
 Requires-Dist: flash-attn (>=2.0.0.post1,<3.0.0)
+Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Description-Content-Type: text/markdown
 
 fast-perceiver
 =========================
```

