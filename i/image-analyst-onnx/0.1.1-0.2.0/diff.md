# Comparing `tmp/image_analyst_onnx-0.1.1.tar.gz` & `tmp/image_analyst_onnx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst_onnx-0.1.1.tar", max compression
+gzip compressed data, was "image_analyst_onnx-0.2.0.tar", max compression
```

## Comparing `image_analyst_onnx-0.1.1.tar` & `image_analyst_onnx-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_onnx-0.1.1/LICENSE
--rw-r--r--   0        0        0     1121 2023-07-17 12:27:57.975682 image_analyst_onnx-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1188 2023-07-17 11:20:58.380078 image_analyst_onnx-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_onnx-0.1.1/src/image_analyst/onnx/__init__.py
--rw-r--r--   0        0        0    10172 2023-07-17 12:27:15.333068 image_analyst_onnx-0.1.1/src/image_analyst/onnx/models.py
--rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 image_analyst_onnx-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_onnx-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1121 2023-07-23 23:23:52.502556 image_analyst_onnx-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1188 2023-07-17 11:20:58.380078 image_analyst_onnx-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_onnx-0.2.0/src/image_analyst/onnx/__init__.py
+-rw-r--r--   0        0        0    10172 2023-07-23 23:23:45.587120 image_analyst_onnx-0.2.0/src/image_analyst/onnx/models.py
+-rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 image_analyst_onnx-0.2.0/PKG-INFO
```

### Comparing `image_analyst_onnx-0.1.1/LICENSE` & `image_analyst_onnx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst_onnx-0.1.1/pyproject.toml` & `image_analyst_onnx-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst-onnx"
-version = "0.1.1"
+version = "0.2.0"
 description = "ImageAnalyst ONNX is an extension to the ImageAnalyst library, providing additional models and functions using onnx."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalystONNX"
 keywords = ["image", "analysis", "onnx"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -12,15 +12,15 @@
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.3"
-image-analyst = "^0.1.2"
+image-analyst = "^0.2.0"
 onnxruntime = "^1.15.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
```

### Comparing `image_analyst_onnx-0.1.1/README.md` & `image_analyst_onnx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `image_analyst_onnx-0.1.1/src/image_analyst/onnx/models.py` & `image_analyst_onnx-0.2.0/src/image_analyst/onnx/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,20 +62,20 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV7Onnx: the new YoloV7Onnx.
         """
         try:
             model_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.1/onnx-yolov7-coco.onnx",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.2.0/onnx-yolov7-coco.onnx",  # noqa: E501
                 "onnx-yolov7-coco.onnx",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.1/onnx-yolov7-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.2.0/onnx-yolov7-coco.names",  # noqa: E501
                 "onnx-yolov7-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV7 model."
             ) from e
@@ -123,20 +123,20 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV7Onnx: the new YoloV7Onnx.
         """
         try:
             model_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.1/onnx-yolov7-tiny-coco.onnx",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.2.0/onnx-yolov7-tiny-coco.onnx",  # noqa: E501
                 "onnx-yolov7-tiny-coco.onnx",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.1.1/onnx-yolov7-tiny-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystONNX/releases/download/v0.2.0/onnx-yolov7-tiny-coco.names",  # noqa: E501
                 "onnx-yolov7-tiny-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV7 model."
             ) from e
```

### Comparing `image_analyst_onnx-0.1.1/PKG-INFO` & `image_analyst_onnx-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: image-analyst-onnx
-Version: 0.1.1
+Version: 0.2.0
 Summary: ImageAnalyst ONNX is an extension to the ImageAnalyst library, providing additional models and functions using onnx.
 Home-page: https://github.com/BergLucas/ImageAnalystONNX
 Keywords: image,analysis,onnx
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: image-analyst (>=0.1.2,<0.2.0)
+Requires-Dist: image-analyst (>=0.2.0,<0.3.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: onnxruntime (>=1.15.1,<2.0.0)
 Project-URL: Repository, https://github.com/BergLucas/ImageAnalystONNX
 Description-Content-Type: text/markdown
 
 # ImageAnalyst ONNX
```

