# Comparing `tmp/image_analyst_cv2-0.1.1.tar.gz` & `tmp/image_analyst_cv2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst_cv2-0.1.1.tar", max compression
+gzip compressed data, was "image_analyst_cv2-0.2.0.tar", max compression
```

## Comparing `image_analyst_cv2-0.1.1.tar` & `image_analyst_cv2-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_cv2-0.1.1/LICENSE
--rw-r--r--   0        0        0     1339 2023-07-17 12:44:00.452585 image_analyst_cv2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1282 2023-07-17 11:16:30.761026 image_analyst_cv2-0.1.1/README.md
--rw-r--r--   0        0        0      203 2023-07-14 17:57:00.279840 image_analyst_cv2-0.1.1/src/image_analyst/cv2/__init__.py
--rw-r--r--   0        0        0      923 2023-07-14 17:26:29.985398 image_analyst_cv2-0.1.1/src/image_analyst/cv2/image.py
--rw-r--r--   0        0        0     9621 2023-07-17 12:43:43.910829 image_analyst_cv2-0.1.1/src/image_analyst/cv2/models.py
--rw-r--r--   0        0        0     4189 2023-07-14 17:33:56.616784 image_analyst_cv2-0.1.1/src/image_analyst/cv2/utils.py
--rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 image_analyst_cv2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_cv2-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1339 2023-07-23 23:08:04.652222 image_analyst_cv2-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1282 2023-07-17 11:16:30.761026 image_analyst_cv2-0.2.0/README.md
+-rw-r--r--   0        0        0      203 2023-07-14 17:57:00.279840 image_analyst_cv2-0.2.0/src/image_analyst/cv2/__init__.py
+-rw-r--r--   0        0        0      923 2023-07-14 17:26:29.985398 image_analyst_cv2-0.2.0/src/image_analyst/cv2/image.py
+-rw-r--r--   0        0        0     9621 2023-07-17 12:54:06.154135 image_analyst_cv2-0.2.0/src/image_analyst/cv2/models.py
+-rw-r--r--   0        0        0     4208 2023-07-17 20:48:27.448489 image_analyst_cv2-0.2.0/src/image_analyst/cv2/utils.py
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 image_analyst_cv2-0.2.0/PKG-INFO
```

### Comparing `image_analyst_cv2-0.1.1/LICENSE` & `image_analyst_cv2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst_cv2-0.1.1/pyproject.toml` & `image_analyst_cv2-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst-cv2"
-version = "0.1.1"
+version = "0.2.0"
 description = "ImageAnalyst CV2 is an extension to the ImageAnalyst library, providing additional models and functions using cv2."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalystCV2"
 keywords = ["image", "analysis", "cv2"]
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
 opencv-contrib-python = {version = "^4.8.0.74", optional = true}
 opencv-contrib-python-headless = {version = "^4.8.0.74", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
```

### Comparing `image_analyst_cv2-0.1.1/README.md` & `image_analyst_cv2-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `image_analyst_cv2-0.1.1/src/image_analyst/cv2/image.py` & `image_analyst_cv2-0.2.0/src/image_analyst/cv2/image.py`

 * *Files identical despite different names*

### Comparing `image_analyst_cv2-0.1.1/src/image_analyst/cv2/models.py` & `image_analyst_cv2-0.2.0/src/image_analyst/cv2/models.py`

 * *Files identical despite different names*

### Comparing `image_analyst_cv2-0.1.1/src/image_analyst/cv2/utils.py` & `image_analyst_cv2-0.2.0/src/image_analyst/cv2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from image_analyst.utils import NmsFunction
 from image_analyst.image import ImageFormat
 from image_analyst.models import Detection
-from typing import Optional, Generator
+from typing import Optional, Generator, Union
 from contextlib import contextmanager
 import numpy as np
 import cv2
 
 
 class NmsCV2(NmsFunction):
     """A CV2 implementation of the Non-maximum Suppression (NMS) algorithm."""
@@ -77,22 +77,22 @@
         return formatted_image.astype(np.float32) / 255
     else:
         raise ValueError(f"Unsupported image dtype: {target_dtype}")
 
 
 @contextmanager
 def create_frame_generator(
-    path_or_id: str | int,
+    path_or_id: Union[str, int],
     api_preference: cv2.VideoCaptureAPIs = cv2.CAP_ANY,
     video_options: Optional[dict[cv2.VideoCaptureProperties, float]] = None,
 ) -> Generator[Generator[np.ndarray, None, None], None, None]:
     """Creates a generator that yields the frames a video.
 
     Args:
-        path_or_id (str | int): the path or id of the video.
+        path_or_id (Union[str, int]): the path or id of the video.
         api_preference (cv2.VideoCaptureAPIs, optional): the API preference.
             Defaults to cv2.CAP_ANY.
         video_options (Optional[dict[cv2.VideoCaptureProperties, float]], optional):
             the video options. Defaults to None.
 
     Yields:
         Generator[Generator[np.ndarray, None, None], None, None]: a generator
```

### Comparing `image_analyst_cv2-0.1.1/PKG-INFO` & `image_analyst_cv2-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: image-analyst-cv2
-Version: 0.1.1
+Version: 0.2.0
 Summary: ImageAnalyst CV2 is an extension to the ImageAnalyst library, providing additional models and functions using cv2.
 Home-page: https://github.com/BergLucas/ImageAnalystCV2
 Keywords: image,analysis,cv2
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cv2
 Provides-Extra: cv2-headless
-Requires-Dist: image-analyst (>=0.1.2,<0.2.0)
+Requires-Dist: image-analyst (>=0.2.0,<0.3.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: opencv-contrib-python (>=4.8.0.74,<5.0.0.0) ; extra == "cv2"
 Requires-Dist: opencv-contrib-python-headless (>=4.8.0.74,<5.0.0.0) ; extra == "cv2-headless"
 Project-URL: Repository, https://github.com/BergLucas/ImageAnalystCV2
 Description-Content-Type: text/markdown
 
 # ImageAnalyst CV2
```

