# Comparing `tmp/VisualFlow-0.2.0.tar.gz` & `tmp/VisualFlow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisualFlow-0.2.0.tar", last modified: Fri Jul 21 13:13:13 2023, max compression
+gzip compressed data, was "VisualFlow-0.2.1.tar", last modified: Mon Jul 24 01:14:30 2023, max compression
```

## Comparing `VisualFlow-0.2.0.tar` & `VisualFlow-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-21 13:13:13.985535 VisualFlow-0.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8244 2023-07-21 13:13:13.985535 VisualFlow-0.2.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6105 2023-07-19 20:33:59.000000 VisualFlow-0.2.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-21 13:13:13.985535 VisualFlow-0.2.0/VisualFlow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-07-19 18:28:47.000000 VisualFlow-0.2.0/VisualFlow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21083 2023-07-21 13:11:39.000000 VisualFlow-0.2.0/VisualFlow/augmentations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2869 2023-07-19 17:57:18.000000 VisualFlow-0.2.0/VisualFlow/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17605 2023-07-19 18:28:37.000000 VisualFlow-0.2.0/VisualFlow/visualflow.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-21 13:13:13.985535 VisualFlow-0.2.0/VisualFlow.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8244 2023-07-21 13:13:13.000000 VisualFlow-0.2.0/VisualFlow.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-07-21 13:13:13.000000 VisualFlow-0.2.0/VisualFlow.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-21 13:13:13.000000 VisualFlow-0.2.0/VisualFlow.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-07-21 13:13:13.000000 VisualFlow-0.2.0/VisualFlow.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-07-21 13:13:13.000000 VisualFlow-0.2.0/VisualFlow.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-21 13:13:13.985535 VisualFlow-0.2.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-07-21 13:12:38.000000 VisualFlow-0.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 01:14:30.522659 VisualFlow-0.2.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8357 2023-07-24 01:14:30.522659 VisualFlow-0.2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6202 2023-07-24 01:10:08.000000 VisualFlow-0.2.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 01:14:30.522659 VisualFlow-0.2.1/VisualFlow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-07-19 18:28:47.000000 VisualFlow-0.2.1/VisualFlow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24278 2023-07-24 01:02:59.000000 VisualFlow-0.2.1/VisualFlow/augmentations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2869 2023-07-19 17:57:18.000000 VisualFlow-0.2.1/VisualFlow/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17605 2023-07-19 18:28:37.000000 VisualFlow-0.2.1/VisualFlow/visualflow.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 01:14:30.522659 VisualFlow-0.2.1/VisualFlow.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8357 2023-07-24 01:14:30.000000 VisualFlow-0.2.1/VisualFlow.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-07-24 01:14:30.000000 VisualFlow-0.2.1/VisualFlow.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-24 01:14:30.000000 VisualFlow-0.2.1/VisualFlow.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-07-24 01:14:30.000000 VisualFlow-0.2.1/VisualFlow.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-07-24 01:14:30.000000 VisualFlow-0.2.1/VisualFlow.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-24 01:14:30.522659 VisualFlow-0.2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-07-24 01:13:32.000000 VisualFlow-0.2.1/setup.py
```

### Comparing `VisualFlow-0.2.0/PKG-INFO` & `VisualFlow-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: VisualFlow
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library for object detection format conversion
 Home-page: https://github.com/Ojas-Sharma/VisualFlow
 Author: Ojas Sharma
 Author-email: ojassharma1607@gmail.com
 License: UNKNOWN
 Description: # VisualFlow
         
         ![VisualFlow Logo](images/vf_logo.webp)
         
         [![PyPI version](https://badge.fury.io/py/visualflow.svg)](https://badge.fury.io/py/visualflow)
+        [![Downloads](https://static.pepy.tech/badge/visualflow)](https://pepy.tech/project/visualflow)
         [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
         
         VisualFlow is a Python library for object detection that provides conversion functions between Pascal VOC, YOLO, and COCO formats. It aims to simplify the process of converting annotated datasets between these popular object detection formats.
         
         We have started this library with the vision of providing end to end object detection, from formatting all the way to inferencing multiple types of object detection models.
         
         Our initial version of VisualFlow allows format conversions between PASCAL VOC, COCO and YOLO. Stay tuned for future updates!
@@ -177,14 +178,15 @@
         ## Contributing
         
         Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/Ojas-Sharma/VisualFlow).
         
         ## License
         
         [MIT](https://choosealicense.com/licenses/mit/)
+        
 Keywords: object-detection cvtoolkit pascal-voc yolo coco computer-vision detr image-classification detection format conversion
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `VisualFlow-0.2.0/README.md` & `VisualFlow-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # VisualFlow
 
 ![VisualFlow Logo](images/vf_logo.webp)
 
 [![PyPI version](https://badge.fury.io/py/visualflow.svg)](https://badge.fury.io/py/visualflow)
+[![Downloads](https://static.pepy.tech/badge/visualflow)](https://pepy.tech/project/visualflow)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 VisualFlow is a Python library for object detection that provides conversion functions between Pascal VOC, YOLO, and COCO formats. It aims to simplify the process of converting annotated datasets between these popular object detection formats.
 
 We have started this library with the vision of providing end to end object detection, from formatting all the way to inferencing multiple types of object detection models.
 
 Our initial version of VisualFlow allows format conversions between PASCAL VOC, COCO and YOLO. Stay tuned for future updates!
@@ -168,8 +169,8 @@
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/Ojas-Sharma/VisualFlow).
 
 ## License
 
-[MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `VisualFlow-0.2.0/VisualFlow/augmentations.py` & `VisualFlow-0.2.1/VisualFlow/augmentations.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import math
 import random
 from PIL import Image, ImageDraw, ImageEnhance, ImageFilter
 import colorsys
 import os
 import shutil
 from .utils import *
+from tqdm import tqdm
 
 def read_yolo_txt_file(file_path):
     data_list = []
 
     with open(file_path, 'r') as file:
         for line in file:
             numbers = line.strip().split()
@@ -32,43 +33,47 @@
 
 
 def cutout(image_dir=None, labels_dir=None, output_dir=None, max_num_cutouts=3):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, ext = os.path.splitext(image_name)
-            # Load the image
-            image = Image.open(image_path)
-            image_width, image_height = image.size
-            # Create a copy of the original image
-            augmented_image = image.copy()
-            cutout_size=(40, 40)
-
-            # Apply cut-out augmentation
-            draw = ImageDraw.Draw(augmented_image)
-            augmented_bbox_list = []
-            for _ in range(max_num_cutouts):
-                cutout_xmin = random.randint(0, image_width - int(cutout_size[0]))
-                cutout_ymin = random.randint(0, image_height - int(cutout_size[1]))
-                cutout_xmax = cutout_xmin + int(cutout_size[0])
-                cutout_ymax = cutout_ymin + int(cutout_size[1])
-                cutout_bbox = (cutout_xmin, cutout_ymin, cutout_xmax, cutout_ymax)
-                augmented_bbox_list.append(cutout_bbox)
-
-                # Fill the selected bounding box with black pixels
-                draw.rectangle(cutout_bbox, fill=(0, 0, 0))
-            new_image_name = f"{image_name}_cutout_{max_num_cutouts}{ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            augmented_image.save(new_image_path)
-        except OSError:
-            print(f"{image}: Skipped due to OSError")
+    with tqdm(total=len(image_paths), desc="Applying Cutouts...") as pbar:
+        for image_name in image_paths:
+            try:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, ext = os.path.splitext(image_name)
+                # Load the image
+                image = Image.open(image_path)
+                image = image.convert("RGB")
+                image_width, image_height = image.size
+                # Create a copy of the original image
+                augmented_image = image.copy()
+                cutout_size=(40, 40)
+
+                # Apply cut-out augmentation
+                draw = ImageDraw.Draw(augmented_image)
+                augmented_bbox_list = []
+                for _ in range(max_num_cutouts):
+                    cutout_xmin = random.randint(0, image_width - int(cutout_size[0]))
+                    cutout_ymin = random.randint(0, image_height - int(cutout_size[1]))
+                    cutout_xmax = cutout_xmin + int(cutout_size[0])
+                    cutout_ymax = cutout_ymin + int(cutout_size[1])
+                    cutout_bbox = (cutout_xmin, cutout_ymin, cutout_xmax, cutout_ymax)
+                    augmented_bbox_list.append(cutout_bbox)
+
+                    # Fill the selected bounding box with black pixels
+                    draw.rectangle(cutout_bbox, fill=(0, 0, 0))
+                new_image_name = f"{image_name}_cutout_{max_num_cutouts}{ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                augmented_image.save(new_image_path)
+            except Exception as e:
+                print(f"{image_name}{ext}: Skipped due to OSError")
+                print(e)
+            pbar.update(1)
     if (labels_dir):
         labels = os.listdir(labels_dir)
         output_labels_dir = os.path.join(output_dir, "labels")
         os.makedirs(output_labels_dir, exist_ok=True)
         for label in labels:
             label_path = os.path.join(labels_dir, label)
             label_name, ext = os.path.splitext(label)
@@ -77,25 +82,29 @@
             shutil.copy(label_path, new_label_path)
 
 def grayscale(image_dir=None, labels_dir=None, output_dir=None):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, ext = os.path.splitext(image_name)
-            image = Image.open(image_path)
-            grayscale_image = image.convert('L')
-            new_image_name = f"{image_name}_grayscale_{ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            grayscale_image.save(new_image_path)
-        except OSError:
-            print(f"{image}: Skipped due to OSError")
+    with tqdm(total=len(image_paths), desc="Grayscaling...") as pbar:
+        for image_name in image_paths:
+            try:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, ext = os.path.splitext(image_name)
+                image = Image.open(image_path)
+                image = image.convert("RGB")
+                grayscale_image = image.convert('L')
+                new_image_name = f"{image_name}_grayscale_{ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                grayscale_image.save(new_image_path)
+            except Exception as e:
+                print(f"{image_name}{ext}: Skipped due to OSError")
+                print(e)
+            pbar.update(1)
 
     if (labels_dir):
         labels = os.listdir(labels_dir)
         output_labels_dir = os.path.join(output_dir, "labels")
         os.makedirs(output_labels_dir, exist_ok=True)
         for label in labels:
             label_path = os.path.join(labels_dir, label)
@@ -106,26 +115,30 @@
 
 
 def brightness(image_dir=None, labels_dir=None, output_dir=None, factor=1.5):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, ext = os.path.splitext(image_name)
-            image = Image.open(image_path)
-            enhancer = ImageEnhance.Brightness(image)
-            brightened_image = enhancer.enhance(factor)
-            new_image_name = f"{image_name}_brightened_{factor}{ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            brightened_image.save(new_image_path)
-        except OSError:
-            print(f"{image}: Skipped due to OSError")
+    with tqdm(total=len(image_paths), desc="Applying Brightness...") as pbar:
+        for image_name in image_paths:
+            try:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, ext = os.path.splitext(image_name)
+                image = Image.open(image_path)
+                image = image.convert("RGB")
+                enhancer = ImageEnhance.Brightness(image)
+                brightened_image = enhancer.enhance(factor)
+                new_image_name = f"{image_name}_brightened_{factor}{ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                brightened_image.save(new_image_path)
+            except Exception as e:
+                print(f"{image_name}{ext}: Skipped due to OSError")
+                print(e)
+            pbar.update(1)
 
     if (labels_dir):
         labels = os.listdir(labels_dir)
         output_labels_dir = os.path.join(output_dir, "labels")
         os.makedirs(output_labels_dir, exist_ok=True)
         for label in labels:
             label_path = os.path.join(labels_dir, label)
@@ -135,34 +148,37 @@
             shutil.copy(label_path, new_label_path)
 
 def noise(image_dir=None, labels_dir=None, output_dir=None):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, ext = os.path.splitext(image_name)
-            # Load the image
-            image = cv2.imread(image_path)
-            # Generate random Gaussian noise
-            mean = 0
-            stddev = 180
-            noise = np.zeros(image.shape, np.uint8)
-            cv2.randn(noise, mean, stddev)
-            # Add noise to image
-            noisy_img = cv2.add(image, noise)
-            noisy_img = cv2.cvtColor(noisy_img, cv2.COLOR_BGR2RGB)
-            noisy_img = Image.fromarray(noisy_img)
-            new_image_name = f"{image_name}_noise{ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            noisy_img.save(new_image_path)
-        except OSError:
-            print(f"{image}: Skipped due to OSError")
+    with tqdm(total=len(image_paths), desc="Adding Noise...") as pbar:
+        for image_name in image_paths:
+            try:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, ext = os.path.splitext(image_name)
+                # Load the image
+                image = cv2.imread(image_path)
+                # Generate random Gaussian noise
+                mean = 0
+                stddev = 180
+                noise = np.zeros(image.shape, np.uint8)
+                cv2.randn(noise, mean, stddev)
+                # Add noise to image
+                noisy_img = cv2.add(image, noise)
+                noisy_img = cv2.cvtColor(noisy_img, cv2.COLOR_BGR2RGB)
+                noisy_img = Image.fromarray(noisy_img)
+                new_image_name = f"{image_name}_noise{ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                noisy_img.save(new_image_path)
+            except Exception as e:
+                print(f"{image_name}{ext}: Skipped due to OSError")
+                print(e)
+            pbar.update(1)
 
     if (labels_dir):
         labels = os.listdir(labels_dir)
         output_labels_dir = os.path.join(output_dir, "labels")
         os.makedirs(output_labels_dir, exist_ok=True)
         for label in labels:
             label_path = os.path.join(labels_dir, label)
@@ -173,26 +189,30 @@
 
 
 def blur(image_dir=None, labels_dir=None, output_dir=None):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, ext = os.path.splitext(image_name)
-            image = Image.open(image_path)
-            # Apply blur
-            blurred_image = image.filter(ImageFilter.BLUR)
-            new_image_name = f"{image_name}_blurred{ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            blurred_image.save(new_image_path)
-        except OSError:
-            print(f"{image}: Skipped due to OSError")
+    with tqdm(total=len(image_paths), desc="Blurring...") as pbar:
+        for image_name in image_paths:
+            try:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, ext = os.path.splitext(image_name)
+                image = Image.open(image_path)
+                image = image.convert("RGB")
+                # Apply blur
+                blurred_image = image.filter(ImageFilter.BLUR)
+                new_image_name = f"{image_name}_blurred{ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                blurred_image.save(new_image_path)
+            except Exception as e:
+                print(f"{image_name}{ext}: Skipped due to OSError")
+                print(e)
+            pbar.update(1)
 
     if (labels_dir):
         labels = os.listdir(labels_dir)
         output_labels_dir = os.path.join(output_dir, "labels")
         os.makedirs(output_labels_dir, exist_ok=True)
         for label in labels:
             label_path = os.path.join(labels_dir, label)
@@ -202,35 +222,39 @@
             shutil.copy(label_path, new_label_path)
 
 def hue(image_dir=None, labels_dir=None, output_dir=None):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, ext = os.path.splitext(image_name)
-            image = Image.open(image_path)
-            # Convert the image to the HSV color space
-            hsv_image = image.convert('HSV')
-            # Split the HSV image into separate channels
-            h, s, v = hsv_image.split()
-            # Adjust the hue channel by a certain value
-            hue_shift = 60  # Adjust the hue by 30 degrees (you can change this value as desired)
-            shifted_hue = h.point(lambda x: (x + hue_shift) % 256)
-            # Merge the modified hue channel with the original saturation and value channels
-            modified_hsv_image = Image.merge('HSV', (shifted_hue, s, v))
-            # Convert the modified HSV image back to the RGB color space
-            modified_rgb_image = modified_hsv_image.convert('RGB')
-            new_image_name = f"{image_name}_hue{ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            modified_rgb_image.save(new_image_path)
-        except OSError:
-            print(f"{image}: Skipped due to OSError")
+    with tqdm(total=len(image_paths), desc="Applying Hue...") as pbar:
+        for image_name in image_paths:
+            try:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, ext = os.path.splitext(image_name)
+                image = Image.open(image_path)
+                image = image.convert("RGB")
+                # Convert the image to the HSV color space
+                hsv_image = image.convert('HSV')
+                # Split the HSV image into separate channels
+                h, s, v = hsv_image.split()
+                # Adjust the hue channel by a certain value
+                hue_shift = 60  # Adjust the hue by 30 degrees (you can change this value as desired)
+                shifted_hue = h.point(lambda x: (x + hue_shift) % 256)
+                # Merge the modified hue channel with the original saturation and value channels
+                modified_hsv_image = Image.merge('HSV', (shifted_hue, s, v))
+                # Convert the modified HSV image back to the RGB color space
+                modified_rgb_image = modified_hsv_image.convert('RGB')
+                new_image_name = f"{image_name}_hue{ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                modified_rgb_image.save(new_image_path)
+            except Exception as e:
+                print(f"{image_name}{ext}: Skipped due to OSError")
+                print(e)
+            pbar.update(1)
 
     if (labels_dir):
         labels = os.listdir(labels_dir)
         output_labels_dir = os.path.join(output_dir, "labels")
         os.makedirs(output_labels_dir, exist_ok=True)
         for label in labels:
             label_path = os.path.join(labels_dir, label)
@@ -240,27 +264,31 @@
             shutil.copy(label_path, new_label_path)
 
 def exposure(image_dir=None, labels_dir=None, output_dir=None, factor=2.0):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, ext = os.path.splitext(image_name)
-            image = Image.open(image_path)
-            # Adjust the exposure
-            enhancer = ImageEnhance.Contrast(image)
-            exposure_adjusted_image = enhancer.enhance(factor)
-            new_image_name = f"{image_name}_exposure_{factor}{ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            exposure_adjusted_image.save(new_image_path)
-        except OSError:
-            print(f"{image}: Skipped due to OSError")
+    with tqdm(total=len(image_paths), desc="Applying Exposure...") as pbar:
+        for image_name in image_paths:
+            try:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, ext = os.path.splitext(image_name)
+                image = Image.open(image_path)
+                image = image.convert("RGB")
+                # Adjust the exposure
+                enhancer = ImageEnhance.Contrast(image)
+                exposure_adjusted_image = enhancer.enhance(factor)
+                new_image_name = f"{image_name}_exposure_{factor}{ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                exposure_adjusted_image.save(new_image_path)
+            except Exception as e:
+                print(f"{image_name}{ext}: Skipped due to OSError")
+                print(e)
+            pbar.update(1)
 
     if (labels_dir):
         labels = os.listdir(labels_dir)
         output_labels_dir = os.path.join(output_dir, "labels")
         os.makedirs(output_labels_dir, exist_ok=True)
         for label in labels:
             label_path = os.path.join(labels_dir, label)
@@ -271,158 +299,168 @@
 
 def flip90(image_dir=None, labels_dir=None, output_dir=None):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     output_labels_dir = os.path.join(output_dir, "labels")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, image_ext = os.path.splitext(image_name)
-            label_name, label_ext = image_name, ".txt"
-            label_path = os.path.join(labels_dir, label_name + label_ext)
-            new_image_name = f"{image_name}_flip90{image_ext}"
-            new_label_name = f"{label_name}_flip90{label_ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            new_label_path = os.path.join(output_labels_dir, new_label_name)
-            image = Image.open(image_path)
-            image_width, image_height = image.size
-            # Rotate the image by 90 degrees clockwise
-            rotated_image = image.rotate(90, expand=True)
-            rotated_image.save(new_image_path)
-            bboxes = read_yolo_txt_file(label_path)
-            new_bboxes = []
-            for bbox in bboxes:
-                converted_bbox = yolo2pascalvoc(bbox[1], bbox[2], bbox[3], bbox[4], image_width, image_height)
-                x_min,y_min,x_max,y_max = converted_bbox
-                new_xmin = y_min
-                new_ymin = image_width-x_max
-                new_xmax = y_max
-                new_ymax = image_width-x_min
-                new_yolo_bbox = pascalvoc2yolo(new_xmin,new_ymin,new_xmax,new_ymax, image_height, image_width)
-                new_bboxes.append([int(bbox[0]), new_yolo_bbox[0], new_yolo_bbox[1], new_yolo_bbox[2], new_yolo_bbox[3]])
+    with tqdm(total=len(image_paths), desc="Flipping...") as pbar:
+        for image_name in image_paths:
             try:
-                save_yolo_txt_file(new_bboxes, new_label_path)
-            except ValueError as e:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, image_ext = os.path.splitext(image_name)
+                label_name, label_ext = image_name, ".txt"
+                label_path = os.path.join(labels_dir, label_name + label_ext)
+                new_image_name = f"{image_name}_flip90{image_ext}"
+                new_label_name = f"{label_name}_flip90{label_ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                new_label_path = os.path.join(output_labels_dir, new_label_name)
+                image = Image.open(image_path)
+                image = image.convert("RGB")
+                image_width, image_height = image.size
+                # Rotate the image by 90 degrees clockwise
+                rotated_image = image.rotate(90, expand=True)
+                rotated_image.save(new_image_path)
+                bboxes = read_yolo_txt_file(label_path)
+                new_bboxes = []
+                for bbox in bboxes:
+                    converted_bbox = yolo2pascalvoc(bbox[1], bbox[2], bbox[3], bbox[4], image_width, image_height)
+                    x_min,y_min,x_max,y_max = converted_bbox
+                    new_xmin = y_min
+                    new_ymin = image_width-x_max
+                    new_xmax = y_max
+                    new_ymax = image_width-x_min
+                    new_yolo_bbox = pascalvoc2yolo(new_xmin,new_ymin,new_xmax,new_ymax, image_height, image_width)
+                    new_bboxes.append([int(bbox[0]), new_yolo_bbox[0], new_yolo_bbox[1], new_yolo_bbox[2], new_yolo_bbox[3]])
+                try:
+                    save_yolo_txt_file(new_bboxes, new_label_path)
+                except ValueError as e:
+                    print(e)
+            except Exception as e:
+                print(f"{image_name}{image_ext}: Skipped due to OSError")
                 print(e)
-        except OSError:
-            print(f"{image_name}: Skipped due to OSError")
+            pbar.update(1)
 
 def shear(image_dir=None, labels_dir=None, output_dir=None, shear_factor = 0.2):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     output_labels_dir = os.path.join(output_dir, "labels")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            shear_factor = (-1 * shear_factor, shear_factor)
-            shear_factor = random.uniform(*shear_factor)
-            image_path = os.path.join(image_dir, image_name)
-            image_name, image_ext = os.path.splitext(image_name)
-            label_name, label_ext = image_name, ".txt"
-            label_path = os.path.join(labels_dir, label_name + label_ext)
-            new_image_name = f"{image_name}_sheared{image_ext}"
-            new_label_name = f"{label_name}_sheared{label_ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            new_label_path = os.path.join(output_labels_dir, new_label_name)
-            img = cv2.imread(image_path)
-            w,h = img.shape[1], img.shape[0]
-            M = np.array([[1, abs(shear_factor), 0],[0,1,0]])
-            nW =  img.shape[1] + abs(shear_factor*img.shape[0])
-            img = cv2.warpAffine(img, M, (int(nW), img.shape[0]))
-            img = cv2.resize(img, (w,h))
-            scale_factor_x = nW / w
-            img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-            img = Image.fromarray(img)
-            img.save(new_image_path)
-            # Rotate the image by 90 degrees clockwise
-            bboxes = read_yolo_txt_file(label_path)
-            converted_bboxes = []
-            for bbox in bboxes:
-                converted_bbox = yolo2pascalvoc(bbox[1], bbox[2], bbox[3], bbox[4], w, h)
-                converted_bboxes.append(converted_bbox)
-            converted_bboxes = np.array(converted_bboxes)
-            converted_bboxes[:,[0,2]] += ((converted_bboxes[:,[1,3]]) * abs(shear_factor) ).astype(int)
-            converted_bboxes[:,:4] /= [scale_factor_x, 1, scale_factor_x, 1]
-            new_bboxes = []
-            for idx, converted_bbox in enumerate(converted_bboxes):
-                new_yolo_bbox = pascalvoc2yolo(converted_bbox[0], converted_bbox[1], converted_bbox[2], converted_bbox[3], w, h)
-                new_bboxes.append([int(bboxes[idx][0]), new_yolo_bbox[0], new_yolo_bbox[1], new_yolo_bbox[2], new_yolo_bbox[3]])
+    with tqdm(total=len(image_paths), desc="Shearing...") as pbar:
+        for image_name in image_paths:
             try:
-                save_yolo_txt_file(new_bboxes, new_label_path)
-            except ValueError as e:
+                shear_factor = (-1 * shear_factor, shear_factor)
+                shear_factor = random.uniform(*shear_factor)
+                image_path = os.path.join(image_dir, image_name)
+                image_name, image_ext = os.path.splitext(image_name)
+                label_name, label_ext = image_name, ".txt"
+                label_path = os.path.join(labels_dir, label_name + label_ext)
+                new_image_name = f"{image_name}_sheared{image_ext}"
+                new_label_name = f"{label_name}_sheared{label_ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                new_label_path = os.path.join(output_labels_dir, new_label_name)
+                img = cv2.imread(image_path)
+                w,h = img.shape[1], img.shape[0]
+                M = np.array([[1, abs(shear_factor), 0],[0,1,0]])
+                nW =  img.shape[1] + abs(shear_factor*img.shape[0])
+                img = cv2.warpAffine(img, M, (int(nW), img.shape[0]))
+                img = cv2.resize(img, (w,h))
+                scale_factor_x = nW / w
+                img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+                img = Image.fromarray(img)
+                img.save(new_image_path)
+                # Rotate the image by 90 degrees clockwise
+                bboxes = read_yolo_txt_file(label_path)
+                converted_bboxes = []
+                for bbox in bboxes:
+                    converted_bbox = yolo2pascalvoc(bbox[1], bbox[2], bbox[3], bbox[4], w, h)
+                    converted_bboxes.append(converted_bbox)
+                converted_bboxes = np.array(converted_bboxes)
+                converted_bboxes[:,[0,2]] += ((converted_bboxes[:,[1,3]]) * abs(shear_factor) ).astype(int)
+                converted_bboxes[:,:4] /= [scale_factor_x, 1, scale_factor_x, 1]
+                new_bboxes = []
+                for idx, converted_bbox in enumerate(converted_bboxes):
+                    new_yolo_bbox = pascalvoc2yolo(converted_bbox[0], converted_bbox[1], converted_bbox[2], converted_bbox[3], w, h)
+                    new_bboxes.append([int(bboxes[idx][0]), new_yolo_bbox[0], new_yolo_bbox[1], new_yolo_bbox[2], new_yolo_bbox[3]])
+                try:
+                    save_yolo_txt_file(new_bboxes, new_label_path)
+                except ValueError as e:
+                    print(e)
+            except Exception as e:
+                print(f"{image_name}{image_ext}: Skipped due to OSError")
                 print(e)
-        except OSError:
-            print(f"{image_name}: Skipped due to OSError")
+            pbar.update(1)
 
 def rotate(image_dir=None, labels_dir=None, output_dir=None, angle=30):
     os.makedirs(output_dir, exist_ok=True)
     image_paths = os.listdir(image_dir)
     output_images_dir = os.path.join(output_dir, "images")
     output_labels_dir = os.path.join(output_dir, "labels")
     os.makedirs(output_images_dir, exist_ok=True)
-    for image_name in image_paths:
-        try:
-            image_path = os.path.join(image_dir, image_name)
-            image_name, image_ext = os.path.splitext(image_name)
-            label_name, label_ext = image_name, ".txt"
-            label_path = os.path.join(labels_dir, label_name + label_ext)
-            new_image_name = f"{image_name}_rotate_{angle}.png"
-            new_label_name = f"{label_name}_rotate_{angle}{label_ext}"
-            new_image_path = os.path.join(output_images_dir, new_image_name)
-            new_label_path = os.path.join(output_labels_dir, new_label_name)
-            image = Image.open(image_path)
-            image = image.convert("RGBA")
-            image_width, image_height = image.size
-            new_image = image.copy()
-            draw = ImageDraw.Draw(new_image)
-            bboxes = read_yolo_txt_file(label_path)
-            converted_bboxes = []
-            for bbox in bboxes:
-                converted_bbox = yolo2pascalvoc(bbox[1], bbox[2], bbox[3], bbox[4], image_width, image_height)
-                converted_bboxes.append(converted_bbox)
-            new_bboxes = []
-            for idx, bbox in enumerate(converted_bboxes):
-                xmin, ymin, xmax, ymax = bbox
-                roi = image.crop((xmin, ymin, xmax, ymax))
-                rotated_roi = roi.rotate(angle, resample=Image.BILINEAR, expand=True)
-                width, height = rotated_roi.size
-                cx, cy = width / 2, height / 2
-                radian_angle = math.radians(angle)
-                cos_theta = math.cos(radian_angle)
-                sin_theta = math.sin(radian_angle)
-                # new_width = width*cos_theta + height*sin_theta
-                # new_height = height*cos_theta + width*sin_theta
-                new_xmin = int(cx + (xmin - cx) * cos_theta - (ymin - cy) * sin_theta)
-                new_ymin = int(cy + (xmin - cx) * sin_theta + (ymin - cy) * cos_theta)
-                new_xmax = new_xmin + width
-                new_ymax = new_ymin + height
-                new_yolo_bbox = pascalvoc2yolo(new_xmin, new_ymin, new_xmax, new_ymax, image_width, image_height)
-                new_bboxes.append([int(bboxes[idx][0]), new_yolo_bbox[0], new_yolo_bbox[1], new_yolo_bbox[2], new_yolo_bbox[3]])
-                # Resize the rotated ROI to match the adjusted bounding box size
-                # rotated_roi = rotated_roi.resize((new_width, new_height))
-                draw.rectangle([(xmin, ymin), (xmax, ymax)], fill='black')
-                # Paste the rotated ROI back into the new image at the appropriate location
-                new_image.paste(rotated_roi, (new_xmin, new_ymin), mask=rotated_roi)
-            new_image.save(new_image_path)
+    with tqdm(total=len(image_paths), desc="Rotating...") as pbar:
+        for image_name in image_paths:
             try:
-                save_yolo_txt_file(new_bboxes, new_label_path)
-            except ValueError as e:
+                image_path = os.path.join(image_dir, image_name)
+                image_name, image_ext = os.path.splitext(image_name)
+                label_name, label_ext = image_name, ".txt"
+                label_path = os.path.join(labels_dir, label_name + label_ext)
+                new_image_name = f"{image_name}_rotate_{angle}.png"
+                new_label_name = f"{label_name}_rotate_{angle}{label_ext}"
+                new_image_path = os.path.join(output_images_dir, new_image_name)
+                new_label_path = os.path.join(output_labels_dir, new_label_name)
+                image = Image.open(image_path)
+                image = image.convert("RGBA")
+                image_width, image_height = image.size
+                new_image = image.copy()
+                draw = ImageDraw.Draw(new_image)
+                bboxes = read_yolo_txt_file(label_path)
+                converted_bboxes = []
+                for bbox in bboxes:
+                    converted_bbox = yolo2pascalvoc(bbox[1], bbox[2], bbox[3], bbox[4], image_width, image_height)
+                    converted_bboxes.append(converted_bbox)
+                new_bboxes = []
+                for idx, bbox in enumerate(converted_bboxes):
+                    xmin, ymin, xmax, ymax = bbox
+                    roi = image.crop((xmin, ymin, xmax, ymax))
+                    rotated_roi = roi.rotate(angle, resample=Image.BILINEAR, expand=True)
+                    width, height = rotated_roi.size
+                    cx, cy = width / 2, height / 2
+                    radian_angle = math.radians(angle)
+                    cos_theta = math.cos(radian_angle)
+                    sin_theta = math.sin(radian_angle)
+                    # new_width = width*cos_theta + height*sin_theta
+                    # new_height = height*cos_theta + width*sin_theta
+                    new_xmin = int(cx + (xmin - cx) * cos_theta - (ymin - cy) * sin_theta)
+                    new_ymin = int(cy + (xmin - cx) * sin_theta + (ymin - cy) * cos_theta)
+                    new_xmax = new_xmin + width
+                    new_ymax = new_ymin + height
+                    new_yolo_bbox = pascalvoc2yolo(new_xmin, new_ymin, new_xmax, new_ymax, image_width, image_height)
+                    new_bboxes.append([int(bboxes[idx][0]), new_yolo_bbox[0], new_yolo_bbox[1], new_yolo_bbox[2], new_yolo_bbox[3]])
+                    # Resize the rotated ROI to match the adjusted bounding box size
+                    # rotated_roi = rotated_roi.resize((new_width, new_height))
+                    draw.rectangle([(xmin, ymin), (xmax, ymax)], fill='black')
+                    # Paste the rotated ROI back into the new image at the appropriate location
+                    new_image.paste(rotated_roi, (new_xmin, new_ymin), mask=rotated_roi)
+                new_image.save(new_image_path)
+                try:
+                    save_yolo_txt_file(new_bboxes, new_label_path)
+                except ValueError as e:
+                    print(e)
+            except Exception as e:
+                print(f"{image_name}{image_ext}: Skipped due to OSError")
                 print(e)
-        except OSError:
-            print(f"{image_name}: Skipped due to OSError")
+            pbar.update(1)
 
 
 
 # Example usage
-# cutout(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output", max_num_cutouts=3)
-# grayscale(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output")
-# brightness(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output")
-# noise(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output")
-# blur(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output")
-# hue(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output")
-# exposure(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output")
-# flip90(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output")
-# shear(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output")
-# rotate(image_dir="./test/images", labels_dir="./test/labels", output_dir="./output", angle=30)
+# cutout(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output", max_num_cutouts=3)
+# grayscale(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output")
+# brightness(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output")
+# noise(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output")
+# blur(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output")
+# hue(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output")
+# exposure(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output")
+# flip90(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output")
+# shear(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output")
+# rotate(image_dir="/home/ubuntu/test/train/images", labels_dir="/home/ubuntu/test/train/labels", output_dir="/home/ubuntu/test/output", angle=30)
```

### Comparing `VisualFlow-0.2.0/VisualFlow/utils.py` & `VisualFlow-0.2.1/VisualFlow/utils.py`

 * *Files identical despite different names*

### Comparing `VisualFlow-0.2.0/VisualFlow/visualflow.py` & `VisualFlow-0.2.1/VisualFlow/visualflow.py`

 * *Files identical despite different names*

### Comparing `VisualFlow-0.2.0/VisualFlow.egg-info/PKG-INFO` & `VisualFlow-0.2.1/VisualFlow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: VisualFlow
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library for object detection format conversion
 Home-page: https://github.com/Ojas-Sharma/VisualFlow
 Author: Ojas Sharma
 Author-email: ojassharma1607@gmail.com
 License: UNKNOWN
 Description: # VisualFlow
         
         ![VisualFlow Logo](images/vf_logo.webp)
         
         [![PyPI version](https://badge.fury.io/py/visualflow.svg)](https://badge.fury.io/py/visualflow)
+        [![Downloads](https://static.pepy.tech/badge/visualflow)](https://pepy.tech/project/visualflow)
         [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
         
         VisualFlow is a Python library for object detection that provides conversion functions between Pascal VOC, YOLO, and COCO formats. It aims to simplify the process of converting annotated datasets between these popular object detection formats.
         
         We have started this library with the vision of providing end to end object detection, from formatting all the way to inferencing multiple types of object detection models.
         
         Our initial version of VisualFlow allows format conversions between PASCAL VOC, COCO and YOLO. Stay tuned for future updates!
@@ -177,14 +178,15 @@
         ## Contributing
         
         Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/Ojas-Sharma/VisualFlow).
         
         ## License
         
         [MIT](https://choosealicense.com/licenses/mit/)
+        
 Keywords: object-detection cvtoolkit pascal-voc yolo coco computer-vision detr image-classification detection format conversion
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `VisualFlow-0.2.0/setup.py` & `VisualFlow-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='VisualFlow',
-    version='0.2.0',
+    version='0.2.1',
     author='Ojas Sharma',
     author_email='ojassharma1607@gmail.com',
     description='A Python library for object detection format conversion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Ojas-Sharma/VisualFlow',
     packages=find_packages(),
```

