# Comparing `tmp/vc_filter-1.1.19.tar.gz` & `tmp/vc_filter-1.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vc_filter-1.1.19.tar", max compression
+gzip compressed data, was "vc_filter-1.1.20.tar", max compression
```

## Comparing `vc_filter-1.1.19.tar` & `vc_filter-1.1.20.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     2762 2022-01-30 19:57:29.984822 vc_filter-1.1.19/README.md
--rw-r--r--   0        0        0      448 2023-07-05 15:44:09.804097 vc_filter-1.1.19/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-05 15:32:04.946498 vc_filter-1.1.19/vc_filter/.DS_Store
--rw-r--r--   0        0        0       37 2022-01-02 07:31:26.000000 vc_filter-1.1.19/vc_filter/__init__.py
--rw-r--r--   0        0        0     5128 2023-07-04 12:36:37.709170 vc_filter-1.1.19/vc_filter/code.py
--rw-r--r--   0        0        0     3364 1970-01-01 00:00:00.000000 vc_filter-1.1.19/PKG-INFO
+-rw-r--r--   0        0        0     3943 2023-07-24 10:21:55.619470 vc_filter-1.1.20/README.md
+-rw-r--r--   0        0        0      451 2023-07-24 10:50:11.353043 vc_filter-1.1.20/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-24 10:25:39.039726 vc_filter-1.1.20/vc_filter/.DS_Store
+-rw-r--r--   0        0        0       29 2023-07-23 09:29:16.213378 vc_filter-1.1.20/vc_filter/__init__.py
+-rw-r--r--   0        0        0     6148 2023-07-24 09:57:54.709483 vc_filter-1.1.20/vc_filter/src/.DS_Store
+-rw-r--r--   0        0        0     2836 2023-07-24 09:02:48.112820 vc_filter-1.1.20/vc_filter/src/apply.py
+-rw-r--r--   0        0        0     2110 2023-07-23 15:43:56.005398 vc_filter-1.1.20/vc_filter/src/others.py
+-rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 vc_filter-1.1.20/PKG-INFO
```

### Comparing `vc_filter-1.1.19/PKG-INFO` & `vc_filter-1.1.20/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: vc-filter
-Version: 1.1.19
-Summary: VC-filter is a new edge detection algorithm based on the Visual Cortex study
-License: MIT
-Author: Boris Kravtsov
-Author-email: kravtsov.development@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: opencv-python-headless (>=4.8.0.74,<5.0.0.0)
-Description-Content-Type: text/markdown
-
 ## VC FILTER
 VC filter is a new high-quality edge detector based on the Visual Cortex study
 
 ### Installation
 ```
 pip install vc-filter
 ```
@@ -65,28 +49,57 @@
 Where else can we find edge detectors tuned to different angles? D.Huebel and T.Wiesel discovered such 
 detectors (orientation-selective neurons) in the visual cortex over 60 years ago, but their role 
 is still unclear. We guess that **orientation-selective neurons compose outline image of 
 the visible object in the same way as the set of modified Sobel filters in our method**.
 
 ### How to use:
 ```Python
-import cv2 as cv
-from vc_filter import vc_filter
+from pathlib import Path
 
-def contrast_enhancement(image_in, contrast_param):
+import vc_filter
 
-    image_out = image_in * contrast_param
+def opencv_recommended_filter(image):
+    """
+    https://docs.opencv.org/3.4/d5/db5/tutorial_laplace_operator.html
+    """
+    # Remove noise by blurring with a Gaussian filter
+    image_gauss = cv.GaussianBlur(image, (3, 3), cv.BORDER_DEFAULT)
 
-    image_out[image_out > 255] = 255
+    # Convert the image to grayscale
+    image_in_gray = cv.cvtColor(image_gauss, cv.COLOR_BGR2GRAY)
 
-    return image_out
+    # Apply Laplace function
+    image_out_gray = cv.Laplacian(image_in_gray, cv.CV_16S, ksize=3)
 
+    # converting back to uint8
+    abs_image_out_gray = cv.convertScaleAbs(image_out_gray)
 
-image = cv.imread(path_in, cv.IMREAD_UNCHANGED)
+    return abs_image_out_gray
 
-image_edges = vc_filter(image)
+def contrast_enhancement(image, contrast_param):
+    image_contrast = image * contrast_param
+    image_contrast[image_contrast > 255] = 255
+    return image_contrast
 
-image_edges_enh = contrast_enhancement(image_edges, 2.0)
 
-cv.imwrite(path_out, image_edges_enh)
-```
+""" Get input image """
+path_in = Path.cwd() / 'DATA' / 'image_in.png'
+image_in = cv.imread(str(path_in), cv.IMREAD_UNCHANGED)
+
+""" OpenCV recommended filter """
+# -------------------------------------------------------------
+edges_opencv = opencv_recommended_filter(image_in)
+
+path_opencv = Path.cwd() / 'DATA' / 'edges_opencv.png'
+cv.imwrite(str(path_opencv), edges_opencv)
+# -------------------------------------------------------------
 
+""" VC filter """
+# -------------------------------------------------------------
+edges_vcf = vc_filter.apply(image_in)
+
+edges_vcf_enh = contrast_enhancement(edges_vcf, 1.7)
+
+path_vcf_enh = Path.cwd() / 'DATA' / 'edges_vcf_enh.png'
+cv.imwrite(str(path_vcf_enh), edges_vcf_enh)
+# -------------------------------------------------------------
+```
```

