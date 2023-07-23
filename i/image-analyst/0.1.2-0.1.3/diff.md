# Comparing `tmp/image_analyst-0.1.2.tar.gz` & `tmp/image_analyst-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst-0.1.2.tar", max compression
+gzip compressed data, was "image_analyst-0.1.3.tar", max compression
```

## Comparing `image_analyst-0.1.2.tar` & `image_analyst-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2023-07-14 16:39:57.000153 image_analyst-0.1.2/LICENSE
--rw-r--r--   0        0        0     1430 2023-07-16 20:40:07.447385 image_analyst-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      885 2023-07-14 16:43:27.012629 image_analyst-0.1.2/README.md
--rw-r--r--   0        0        0     3262 2023-07-14 16:30:33.796322 image_analyst-0.1.2/src/image_analyst/analyzers.py
--rw-r--r--   0        0        0      860 2023-07-14 16:31:22.972890 image_analyst-0.1.2/src/image_analyst/exceptions.py
--rw-r--r--   0        0        0    10784 2023-07-14 20:52:32.058152 image_analyst-0.1.2/src/image_analyst/image.py
--rw-r--r--   0        0        0     1928 2023-07-14 15:36:16.430223 image_analyst-0.1.2/src/image_analyst/models.py
--rw-r--r--   0        0        0     6421 2023-07-14 16:35:39.510440 image_analyst-0.1.2/src/image_analyst/trackers.py
--rw-r--r--   0        0        0     5505 2023-07-14 16:34:33.341203 image_analyst-0.1.2/src/image_analyst/utils.py
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 image_analyst-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-14 16:39:57.000153 image_analyst-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1430 2023-07-17 13:08:32.781715 image_analyst-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2833 2023-07-17 11:08:33.804661 image_analyst-0.1.3/README.md
+-rw-r--r--   0        0        0     3262 2023-07-14 16:30:33.796322 image_analyst-0.1.3/src/image_analyst/analyzers.py
+-rw-r--r--   0        0        0      860 2023-07-14 16:31:22.972890 image_analyst-0.1.3/src/image_analyst/exceptions.py
+-rw-r--r--   0        0        0    10784 2023-07-14 20:52:32.058152 image_analyst-0.1.3/src/image_analyst/image.py
+-rw-r--r--   0        0        0     1928 2023-07-14 15:36:16.430223 image_analyst-0.1.3/src/image_analyst/models.py
+-rw-r--r--   0        0        0     6421 2023-07-14 16:35:39.510440 image_analyst-0.1.3/src/image_analyst/trackers.py
+-rw-r--r--   0        0        0     5505 2023-07-14 16:34:33.341203 image_analyst-0.1.3/src/image_analyst/utils.py
+-rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 image_analyst-0.1.3/PKG-INFO
```

### Comparing `image_analyst-0.1.2/LICENSE` & `image_analyst-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.2/pyproject.toml` & `image_analyst-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst"
-version = "0.1.2"
+version = "0.1.3"
 description = "ImageAnalyst is a library that simplifies image analysis."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalyst"
 keywords = ["image", "analysis"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -12,18 +12,18 @@
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.3"
-image-analyst-cv2 = {version = "^0.1.0", optional = true, extras = ["cv2"]}
-image-analyst-hf = {version = "^0.1.0", optional = true, python = ">=3.9, <3.12"}
-image-analyst-tf = {version = "^0.1.1", optional = true, python = ">=3.9, <3.12"}
-image-analyst-onnx = {version = "^0.1.0", optional = true}
+image-analyst-cv2 = {version = "^0.1.1", optional = true, extras = ["cv2"]}
+image-analyst-hf = {version = "^0.1.1", optional = true, python = ">=3.9, <3.12"}
+image-analyst-tf = {version = "^0.1.2", optional = true, python = ">=3.9, <3.12"}
+image-analyst-onnx = {version = "^0.1.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.7.0"
```

### Comparing `image_analyst-0.1.2/src/image_analyst/analyzers.py` & `image_analyst-0.1.3/src/image_analyst/analyzers.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.2/src/image_analyst/exceptions.py` & `image_analyst-0.1.3/src/image_analyst/exceptions.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.2/src/image_analyst/image.py` & `image_analyst-0.1.3/src/image_analyst/image.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.2/src/image_analyst/models.py` & `image_analyst-0.1.3/src/image_analyst/models.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.2/src/image_analyst/trackers.py` & `image_analyst-0.1.3/src/image_analyst/trackers.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.2/src/image_analyst/utils.py` & `image_analyst-0.1.3/src/image_analyst/utils.py`

 * *Files identical despite different names*

