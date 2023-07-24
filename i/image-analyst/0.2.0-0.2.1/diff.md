# Comparing `tmp/image_analyst-0.2.0.tar.gz` & `tmp/image_analyst-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst-0.2.0.tar", max compression
+gzip compressed data, was "image_analyst-0.2.1.tar", max compression
```

## Comparing `image_analyst-0.2.0.tar` & `image_analyst-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2023-07-14 16:39:57.000153 image_analyst-0.2.0/LICENSE
--rw-r--r--   0        0        0     1439 2023-07-23 23:01:30.126478 image_analyst-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2824 2023-07-23 22:59:20.674924 image_analyst-0.2.0/README.md
--rw-r--r--   0        0        0     3262 2023-07-14 16:30:33.796322 image_analyst-0.2.0/src/image_analyst/analyzers.py
--rw-r--r--   0        0        0      860 2023-07-14 16:31:22.972890 image_analyst-0.2.0/src/image_analyst/exceptions.py
--rw-r--r--   0        0        0    10784 2023-07-14 20:52:32.058152 image_analyst-0.2.0/src/image_analyst/image.py
--rw-r--r--   0        0        0     1928 2023-07-14 15:36:16.430223 image_analyst-0.2.0/src/image_analyst/models.py
--rw-r--r--   0        0        0     5491 2023-07-23 22:46:03.393714 image_analyst-0.2.0/src/image_analyst/trackers.py
--rw-r--r--   0        0        0     5524 2023-07-17 20:50:29.903823 image_analyst-0.2.0/src/image_analyst/utils.py
--rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 image_analyst-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-14 16:39:57.000153 image_analyst-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1430 2023-07-24 00:04:30.178746 image_analyst-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2808 2023-07-24 00:04:48.049952 image_analyst-0.2.1/README.md
+-rw-r--r--   0        0        0     3262 2023-07-14 16:30:33.796322 image_analyst-0.2.1/src/image_analyst/analyzers.py
+-rw-r--r--   0        0        0      860 2023-07-14 16:31:22.972890 image_analyst-0.2.1/src/image_analyst/exceptions.py
+-rw-r--r--   0        0        0    10784 2023-07-14 20:52:32.058152 image_analyst-0.2.1/src/image_analyst/image.py
+-rw-r--r--   0        0        0     1928 2023-07-14 15:36:16.430223 image_analyst-0.2.1/src/image_analyst/models.py
+-rw-r--r--   0        0        0     5491 2023-07-23 22:46:03.393714 image_analyst-0.2.1/src/image_analyst/trackers.py
+-rw-r--r--   0        0        0     5524 2023-07-17 20:50:29.903823 image_analyst-0.2.1/src/image_analyst/utils.py
+-rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 image_analyst-0.2.1/PKG-INFO
```

### Comparing `image_analyst-0.2.0/LICENSE` & `image_analyst-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst-0.2.0/pyproject.toml` & `image_analyst-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst"
-version = "0.2.0"
+version = "0.2.1"
 description = "ImageAnalyst is a library that simplifies image analysis."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalyst"
 keywords = ["image", "analysis"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -12,31 +12,31 @@
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.3"
-#image-analyst-cv2 = {version = "^0.1.1", optional = true, extras = ["cv2"]}
-#image-analyst-hf = {version = "^0.1.1", optional = true, python = ">=3.9, <3.12"}
-#image-analyst-tf = {version = "^0.1.2", optional = true, python = ">=3.9, <3.12"}
-#image-analyst-onnx = {version = "^0.1.1", optional = true}
+image-analyst-cv2 = {version = "^0.2.0", optional = true, extras = ["cv2"]}
+image-analyst-hf = {version = "^0.2.0", optional = true, python = ">=3.9, <3.12"}
+image-analyst-tf = {version = "^0.2.0", optional = true, python = ">=3.9, <3.12"}
+image-analyst-onnx = {version = "^0.2.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.7.0"
 
-#[tool.poetry.extras]
-#cv2 = ["image-analyst-cv2"]
-#hf = ["image-analyst-hf"]
-#tf = ["image-analyst-tf"]
-#onnx = ["image-analyst-onnx"]
+[tool.poetry.extras]
+cv2 = ["image-analyst-cv2"]
+hf = ["image-analyst-hf"]
+tf = ["image-analyst-tf"]
+onnx = ["image-analyst-onnx"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 relative_files = true
```

### Comparing `image_analyst-0.2.0/README.md` & `image_analyst-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 ## Requirements
 
 The application requires:
 
 - [Python](https://www.python.org/) ~= 3.9
 - [pip](https://pip.pypa.io/en/stable/)
-<!--
+
 ## Extras
 
 The application has some extras that can be installed:
 
 - [cv2](https://github.com/BergLucas/ImageAnalystCV2)
 - [hf](https://github.com/BergLucas/ImageAnalystHF)
 - [tf](https://github.com/BergLucas/ImageAnalystTF)
 - [onnx](https://github.com/BergLucas/ImageAnalystONNX)
-!-->
+
 ## Download & Installation
 
 There is two ways to download and install the application.
 
 ### Using PyPI
 
 You can download and install the application using [PyPI](https://pypi.org/project/image-analyst/). To do so, run the following command:
@@ -36,15 +36,15 @@
 You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalyst/releases). Then, you can install the application by running the following command:
 
 ```bash
 pip install image_analyst-X.X.X-py3-none-any.whl
 ```
 
 (Note: The X.X.X must be replaced by the version that you want to install.)
-<!--
+
 ## Example
 
 This example allows you to track objects from your webcam. It requires the `cv2` extra.
 
 ```python
 from image_analyst.cv2.utils import convert_image, create_frame_generator
 from image_analyst.cv2.models import YoloV3OpenCV
@@ -73,11 +73,11 @@
         cv2.imshow("Tracking", frame)
 
         if cv2.waitKey(1) & 0xFF == ord('q'):
             break
 
 cv2.destroyAllWindows()
 ```
-!-->
+
 ## License
 
 All code is licensed for others under a MIT license (see [LICENSE](https://github.com/BergLucas/ImageAnalyst/blob/main/LICENSE)).
```

### Comparing `image_analyst-0.2.0/src/image_analyst/analyzers.py` & `image_analyst-0.2.1/src/image_analyst/analyzers.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.2.0/src/image_analyst/exceptions.py` & `image_analyst-0.2.1/src/image_analyst/exceptions.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.2.0/src/image_analyst/image.py` & `image_analyst-0.2.1/src/image_analyst/image.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.2.0/src/image_analyst/models.py` & `image_analyst-0.2.1/src/image_analyst/models.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.2.0/src/image_analyst/trackers.py` & `image_analyst-0.2.1/src/image_analyst/trackers.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.2.0/src/image_analyst/utils.py` & `image_analyst-0.2.1/src/image_analyst/utils.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.2.0/PKG-INFO` & `image_analyst-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: image-analyst
-Version: 0.2.0
+Version: 0.2.1
 Summary: ImageAnalyst is a library that simplifies image analysis.
 Home-page: https://github.com/BergLucas/ImageAnalyst
 Keywords: image,analysis
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cv2
+Provides-Extra: hf
+Provides-Extra: onnx
+Provides-Extra: tf
+Requires-Dist: image-analyst-cv2[cv2] (>=0.2.0,<0.3.0) ; extra == "cv2"
+Requires-Dist: image-analyst-hf (>=0.2.0,<0.3.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "hf")
+Requires-Dist: image-analyst-onnx (>=0.2.0,<0.3.0) ; extra == "onnx"
+Requires-Dist: image-analyst-tf (>=0.2.0,<0.3.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "tf")
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Project-URL: Repository, https://github.com/BergLucas/ImageAnalyst
 Description-Content-Type: text/markdown
 
 # ImageAnalyst
 
 ImageAnalyst is a library that simplifies image analysis. The library achieves this goal by standardizing the input and output
@@ -24,24 +32,24 @@
 
 ## Requirements
 
 The application requires:
 
 - [Python](https://www.python.org/) ~= 3.9
 - [pip](https://pip.pypa.io/en/stable/)
-<!--
+
 ## Extras
 
 The application has some extras that can be installed:
 
 - [cv2](https://github.com/BergLucas/ImageAnalystCV2)
 - [hf](https://github.com/BergLucas/ImageAnalystHF)
 - [tf](https://github.com/BergLucas/ImageAnalystTF)
 - [onnx](https://github.com/BergLucas/ImageAnalystONNX)
-!-->
+
 ## Download & Installation
 
 There is two ways to download and install the application.
 
 ### Using PyPI
 
 You can download and install the application using [PyPI](https://pypi.org/project/image-analyst/). To do so, run the following command:
@@ -55,15 +63,15 @@
 You can download the application on the [downloads page](https://github.com/BergLucas/ImageAnalyst/releases). Then, you can install the application by running the following command:
 
 ```bash
 pip install image_analyst-X.X.X-py3-none-any.whl
 ```
 
 (Note: The X.X.X must be replaced by the version that you want to install.)
-<!--
+
 ## Example
 
 This example allows you to track objects from your webcam. It requires the `cv2` extra.
 
 ```python
 from image_analyst.cv2.utils import convert_image, create_frame_generator
 from image_analyst.cv2.models import YoloV3OpenCV
@@ -92,12 +100,12 @@
         cv2.imshow("Tracking", frame)
 
         if cv2.waitKey(1) & 0xFF == ord('q'):
             break
 
 cv2.destroyAllWindows()
 ```
-!-->
+
 ## License
 
 All code is licensed for others under a MIT license (see [LICENSE](https://github.com/BergLucas/ImageAnalyst/blob/main/LICENSE)).
```

