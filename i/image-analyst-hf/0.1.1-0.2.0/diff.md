# Comparing `tmp/image_analyst_hf-0.1.1.tar.gz` & `tmp/image_analyst_hf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst_hf-0.1.1.tar", max compression
+gzip compressed data, was "image_analyst_hf-0.2.0.tar", max compression
```

## Comparing `image_analyst_hf-0.1.1.tar` & `image_analyst_hf-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_hf-0.1.1/LICENSE
--rw-r--r--   0        0        0     1384 2023-07-17 12:35:35.125571 image_analyst_hf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1188 2023-07-17 11:18:34.537877 image_analyst_hf-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_hf-0.1.1/src/image_analyst/hf/__init__.py
--rw-r--r--   0        0        0     5233 2023-07-15 00:39:37.379325 image_analyst_hf-0.1.1/src/image_analyst/hf/models.py
--rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 image_analyst_hf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_hf-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1384 2023-07-23 23:19:04.375141 image_analyst_hf-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1188 2023-07-17 11:18:34.537877 image_analyst_hf-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_hf-0.2.0/src/image_analyst/hf/__init__.py
+-rw-r--r--   0        0        0     5233 2023-07-15 00:39:37.379325 image_analyst_hf-0.2.0/src/image_analyst/hf/models.py
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 image_analyst_hf-0.2.0/PKG-INFO
```

### Comparing `image_analyst_hf-0.1.1/LICENSE` & `image_analyst_hf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst_hf-0.1.1/pyproject.toml` & `image_analyst_hf-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst-hf"
-version = "0.1.1"
+version = "0.2.0"
 description = "ImageAnalyst HF is an extension to the ImageAnalyst library, providing additional models and functions using huggingface."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalystHF"
 keywords = ["image", "analysis", "huggingface"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -12,15 +12,15 @@
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 numpy = "^1.24.3"
-image-analyst = "^0.1.2"
+image-analyst = "^0.2.0"
 transformers = {version = "^4.30.2", extras = ["onnxruntime", "tf", "tf-cpu", "timm", "torch", "torch-vision", "torchhub"]}
 tensorflow = "^2.10.0"
 tensorflow-text = "^2.10.0, !=2.11.0"
 tensorflow-io-gcs-filesystem = "^0.29, !=0.32.0"
 pillow = "^10.0.0"
 torch = "^2.0.1"
```

### Comparing `image_analyst_hf-0.1.1/README.md` & `image_analyst_hf-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `image_analyst_hf-0.1.1/src/image_analyst/hf/models.py` & `image_analyst_hf-0.2.0/src/image_analyst/hf/models.py`

 * *Files identical despite different names*

### Comparing `image_analyst_hf-0.1.1/PKG-INFO` & `image_analyst_hf-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: image-analyst-hf
-Version: 0.1.1
+Version: 0.2.0
 Summary: ImageAnalyst HF is an extension to the ImageAnalyst library, providing additional models and functions using huggingface.
 Home-page: https://github.com/BergLucas/ImageAnalystHF
 Keywords: image,analysis,huggingface
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: image-analyst (>=0.1.2,<0.2.0)
+Requires-Dist: image-analyst (>=0.2.0,<0.3.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: tensorflow (>=2.10.0,<3.0.0)
 Requires-Dist: tensorflow-io-gcs-filesystem (>=0.29,<0.30)
 Requires-Dist: tensorflow-text (>=2.10.0,<3.0.0,!=2.11.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers[onnxruntime,tf,tf-cpu,timm,torch,torch-vision,torchhub] (>=4.30.2,<5.0.0)
```

