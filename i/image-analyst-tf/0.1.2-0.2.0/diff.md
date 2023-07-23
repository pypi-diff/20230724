# Comparing `tmp/image_analyst_tf-0.1.2.tar.gz` & `tmp/image_analyst_tf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst_tf-0.1.2.tar", max compression
+gzip compressed data, was "image_analyst_tf-0.2.0.tar", max compression
```

## Comparing `image_analyst_tf-0.1.2.tar` & `image_analyst_tf-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_tf-0.1.2/LICENSE
--rw-r--r--   0        0        0     1182 2023-07-17 11:29:18.851147 image_analyst_tf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1185 2023-07-17 11:27:00.632197 image_analyst_tf-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_tf-0.1.2/src/image_analyst/tf/__init__.py
--rw-r--r--   0        0        0    13634 2023-07-17 11:28:24.714731 image_analyst_tf-0.1.2/src/image_analyst/tf/models.py
--rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 image_analyst_tf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_tf-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1182 2023-07-23 23:45:20.506039 image_analyst_tf-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-07-17 11:27:00.632197 image_analyst_tf-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_tf-0.2.0/src/image_analyst/tf/__init__.py
+-rw-r--r--   0        0        0    13634 2023-07-23 23:44:25.280103 image_analyst_tf-0.2.0/src/image_analyst/tf/models.py
+-rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 image_analyst_tf-0.2.0/PKG-INFO
```

### Comparing `image_analyst_tf-0.1.2/LICENSE` & `image_analyst_tf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst_tf-0.1.2/pyproject.toml` & `image_analyst_tf-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst-tf"
-version = "0.1.2"
+version = "0.2.0"
 description = "ImageAnalyst TF is an extension to the ImageAnalyst library, providing additional models and functions using tensorflow."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalystTF"
 keywords = ["image", "analysis", "tensorflow"]
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
 tensorflow = "^2.10.0"
 tensorflow-io-gcs-filesystem = "^0.29, !=0.32.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
```

### Comparing `image_analyst_tf-0.1.2/README.md` & `image_analyst_tf-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `image_analyst_tf-0.1.2/src/image_analyst/tf/models.py` & `image_analyst_tf-0.2.0/src/image_analyst/tf/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,20 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV7Tflite: the new YoloV7Tflite.
         """
         try:
             model_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.2/tf-yolov7-coco.tflite",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.2.0/tf-yolov7-coco.tflite",  # noqa: E501
                 "tf-yolov7-coco.tflite",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.2/tf-yolov7-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.2.0/tf-yolov7-coco.names",  # noqa: E501
                 "tf-yolov7-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV7 model."
             ) from e
@@ -107,20 +107,20 @@
             ValueError: if the score threshold is not between 0 and 1.
 
         Returns:
             YoloV7Tflite: the new YoloV7Tflite.
         """
         try:
             model_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.2/tf-yolov7-tiny-coco.tflite",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.2.0/tf-yolov7-tiny-coco.tflite",  # noqa: E501
                 "tf-yolov7-tiny-coco.tflite",
                 report_callback,
             )
             labels_path = download_file(
-                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.1.2/tf-yolov7-tiny-coco.names",  # noqa: E501
+                "https://github.com/BergLucas/ImageAnalystTF/releases/download/v0.2.0/tf-yolov7-tiny-coco.names",  # noqa: E501
                 "tf-yolov7-tiny-coco.names",
                 report_callback,
             )
         except DownloadFailedException as e:
             raise ModelLoadingFailedException(
                 "Cannot download the YoloV7 model."
             ) from e
```

### Comparing `image_analyst_tf-0.1.2/PKG-INFO` & `image_analyst_tf-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: image-analyst-tf
-Version: 0.1.2
+Version: 0.2.0
 Summary: ImageAnalyst TF is an extension to the ImageAnalyst library, providing additional models and functions using tensorflow.
 Home-page: https://github.com/BergLucas/ImageAnalystTF
 Keywords: image,analysis,tensorflow
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
 Requires-Dist: tensorflow (>=2.10.0,<3.0.0)
 Requires-Dist: tensorflow-io-gcs-filesystem (>=0.29,<0.30)
 Project-URL: Repository, https://github.com/BergLucas/ImageAnalystTF
 Description-Content-Type: text/markdown
 
 # ImageAnalyst TF
```

