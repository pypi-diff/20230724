# Comparing `tmp/unstructured_inference-0.5.5.tar.gz` & `tmp/unstructured_inference-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.5.5.tar", last modified: Fri Jul  7 13:44:51 2023, max compression
+gzip compressed data, was "unstructured_inference-0.5.6.tar", last modified: Mon Jul 24 19:17:08 2023, max compression
```

## Comparing `unstructured_inference-0.5.5.tar` & `unstructured_inference-0.5.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.112177 unstructured_inference-0.5.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.116177 unstructured_inference-0.5.5/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.120177 unstructured_inference-0.5.5/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/chipper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/detectron2onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24262 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.116177 unstructured_inference-0.5.5/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-07 13:44:50.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-07 13:44:51.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:44:50.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-07 13:44:50.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 13:44:50.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.136584 unstructured_inference-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-24 19:17:08.136584 unstructured_inference-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.116584 unstructured_inference-0.5.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 19:17:08.140585 unstructured_inference-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.120584 unstructured_inference-0.5.6/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.128584 unstructured_inference-0.5.6/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.136584 unstructured_inference-0.5.6/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/chipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24262 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.136584 unstructured_inference-0.5.6/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.124584 unstructured_inference-0.5.6/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-24 19:17:07.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 19:17:08.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:17:07.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-24 19:17:07.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:17:07.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.5.5/PKG-INFO` & `unstructured_inference-0.5.6/unstructured_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unstructured_inference
-Version: 0.5.5
+Name: unstructured-inference
+Version: 0.5.6
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -29,15 +29,15 @@
         
         ### Detectron2
         
         [Detectron2](https://github.com/facebookresearch/detectron2) is required for using models from the [layoutparser model zoo](#using-models-from-the-layoutparser-model-zoo) 
         but is not automatically installed with this package. 
         For MacOS and Linux, build from source with:
         ```shell
-        pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
+        pip install 'git+https://github.com/facebookresearch/detectron2.git@a2e43ea#egg=detectron2'
         ```
         Other install options can be found in the 
         [Detectron2 installation guide](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
         
         Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
         See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
         tips on installing Detectron2 on Windows.
```

### Comparing `unstructured_inference-0.5.5/README.md` & `unstructured_inference-0.5.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ### Detectron2
 
 [Detectron2](https://github.com/facebookresearch/detectron2) is required for using models from the [layoutparser model zoo](#using-models-from-the-layoutparser-model-zoo) 
 but is not automatically installed with this package. 
 For MacOS and Linux, build from source with:
 ```shell
-pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
+pip install 'git+https://github.com/facebookresearch/detectron2.git@a2e43ea#egg=detectron2'
 ```
 Other install options can be found in the 
 [Detectron2 installation guide](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
 
 Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
 See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
 tips on installing Detectron2 on Windows.
```

### Comparing `unstructured_inference-0.5.5/setup.py` & `unstructured_inference-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/inference/elements.py` & `unstructured_inference-0.5.6/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/inference/layout.py` & `unstructured_inference-0.5.6/unstructured_inference/inference/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import os
 import tempfile
+from pathlib import PurePath
 from typing import BinaryIO, Collection, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import pdf2image
 from pdfminer import psparser
 from pdfminer.high_level import extract_pages
 from PIL import Image
@@ -73,40 +74,55 @@
         filename: str,
         detection_model: Optional[UnstructuredObjectDetectionModel] = None,
         element_extraction_model: Optional[UnstructuredElementExtractionModel] = None,
         fixed_layouts: Optional[List[Optional[List[TextRegion]]]] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         extract_tables: bool = False,
+        pdf_image_dpi: int = 200,
     ) -> DocumentLayout:
         """Creates a DocumentLayout from a pdf file."""
         logger.info(f"Reading PDF for file: {filename} ...")
-        layouts, images = load_pdf(filename)
-        if len(layouts) > len(images):
+
+        # Store pdf images for later use
+        output_dir = create_image_output_dir(filename)
+        layouts, _image_paths = load_pdf(
+            filename,
+            pdf_image_dpi,
+            output_folder=output_dir,
+            path_only=True,
+        )
+        image_paths = cast(List[str], _image_paths)
+        if len(layouts) > len(image_paths):
             raise RuntimeError(
-                "Some images were not loaded. Check that poppler is installed and in your $PATH.",
+                "Some images were not loaded. "
+                "Check that poppler is installed and in your $PATH.",
             )
         pages: List[PageLayout] = []
         if fixed_layouts is None:
             fixed_layouts = [None for _ in layouts]
-        for i, (image, layout, fixed_layout) in enumerate(zip(images, layouts, fixed_layouts)):
+        for i, (image_path, layout, fixed_layout) in enumerate(
+            zip(image_paths, layouts, fixed_layouts),
+        ):
             # NOTE(robinson) - In the future, maybe we detect the page number and default
             # to the index if it is not detected
-            page = PageLayout.from_image(
-                image,
-                number=i + 1,
-                detection_model=detection_model,
-                element_extraction_model=element_extraction_model,
-                layout=layout,
-                ocr_strategy=ocr_strategy,
-                ocr_languages=ocr_languages,
-                fixed_layout=fixed_layout,
-                extract_tables=extract_tables,
-            )
-            pages.append(page)
+            with Image.open(image_path) as image:
+                page = PageLayout.from_image(
+                    image,
+                    image_path=image_path,
+                    number=i + 1,
+                    detection_model=detection_model,
+                    element_extraction_model=element_extraction_model,
+                    layout=layout,
+                    ocr_strategy=ocr_strategy,
+                    ocr_languages=ocr_languages,
+                    fixed_layout=fixed_layout,
+                    extract_tables=extract_tables,
+                )
+                pages.append(page)
         return cls.from_pages(pages)
 
     @classmethod
     def from_image_file(
         cls,
         filename: str,
         detection_model: Optional[UnstructuredObjectDetectionModel] = None,
@@ -126,14 +142,15 @@
         except Exception as e:
             if os.path.isdir(filename) or os.path.isfile(filename):
                 raise e
             else:
                 raise FileNotFoundError(f'File "{filename}" not found!') from e
         page = PageLayout.from_image(
             image,
+            image_path=filename,
             detection_model=detection_model,
             element_extraction_model=element_extraction_model,
             layout=None,
             ocr_strategy=ocr_strategy,
             ocr_languages=ocr_languages,
             fixed_layout=fixed_layout,
             extract_tables=extract_tables,
@@ -145,23 +162,29 @@
     """Class for an individual PDF page."""
 
     def __init__(
         self,
         number: int,
         image: Image.Image,
         layout: Optional[List[TextRegion]],
+        image_metadata: Optional[dict] = None,
+        image_path: Optional[Union[str, PurePath]] = None,
         detection_model: Optional[UnstructuredObjectDetectionModel] = None,
         element_extraction_model: Optional[UnstructuredElementExtractionModel] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         extract_tables: bool = False,
     ):
         if detection_model is not None and element_extraction_model is not None:
             raise ValueError("Only one of detection_model and extraction_model should be passed.")
         self.image = image
+        if image_metadata is None:
+            image_metadata = {}
+        self.image_metadata = image_metadata
+        self.image_path = image_path
         self.image_array: Union[np.ndarray, None] = None
         self.layout = layout
         self.number = number
         self.detection_model = detection_model
         self.element_extraction_model = element_extraction_model
         self.elements: Collection[Union[LayoutElement, LocationlessLayoutElement]] = []
         if ocr_strategy not in VALID_OCR_STRATEGIES:
@@ -232,37 +255,43 @@
             for e in layout
         ]
         return elements
 
     def _get_image_array(self) -> Union[np.ndarray, None]:
         """Converts the raw image into a numpy array."""
         if self.image_array is None:
-            self.image_array = np.array(self.image)
+            if self.image:
+                self.image_array = np.array(self.image)
+            else:
+                image = Image.open(self.image_path)
+                self.image_array = np.array(image)
         return self.image_array
 
     def annotate(self, colors: Optional[Union[List[str], str]] = None) -> Image.Image:
         """Annotates the elements on the page image."""
         if colors is None:
             colors = ["red" for _ in self.elements]
         if isinstance(colors, str):
             colors = [colors]
         # If there aren't enough colors, just cycle through the colors a few times
         if len(colors) < len(self.elements):
             n_copies = (len(self.elements) // len(colors)) + 1
             colors = colors * n_copies
-        img = self.image.copy()
+        img = self.image.copy() if self.image else Image.open(self.image_path)
+
         for el, color in zip(self.elements, colors):
             if isinstance(el, Rectangle):
                 img = draw_bbox(img, el, color=color)
         return img
 
     @classmethod
     def from_image(
         cls,
         image: Image.Image,
+        image_path: Optional[Union[str, PurePath]],
         number: int = 1,
         detection_model: Optional[UnstructuredObjectDetectionModel] = None,
         element_extraction_model: Optional[UnstructuredElementExtractionModel] = None,
         layout: Optional[List[TextRegion]] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         extract_tables: bool = False,
@@ -282,51 +311,63 @@
         if page.element_extraction_model is not None:
             page.get_elements_using_image_extraction()
             return page
         if fixed_layout is None:
             page.get_elements_with_detection_model()
         else:
             page.elements = page.get_elements_from_layout(fixed_layout)
+
+        page.image_metadata = {
+            "format": page.image.format if page.image else None,
+            "width": page.image.width if page.image else None,
+            "height": page.image.height if page.image else None,
+        }
+        page.image_path = os.path.abspath(image_path) if image_path else None
+        page.image = None
+
         return page
 
 
 def process_data_with_model(
     data: BinaryIO,
     model_name: Optional[str],
     is_image: bool = False,
     ocr_strategy: str = "auto",
     ocr_languages: str = "eng",
     fixed_layouts: Optional[List[Optional[List[TextRegion]]]] = None,
     extract_tables: bool = False,
+    pdf_image_dpi: int = 200,
 ) -> DocumentLayout:
     """Processes pdf file in the form of a file handler (supporting a read method) into a
     DocumentLayout by using a model identified by model_name."""
     with tempfile.NamedTemporaryFile() as tmp_file:
         tmp_file.write(data.read())
         layout = process_file_with_model(
             tmp_file.name,
             model_name,
             is_image=is_image,
             ocr_strategy=ocr_strategy,
             ocr_languages=ocr_languages,
             fixed_layouts=fixed_layouts,
             extract_tables=extract_tables,
+            pdf_image_dpi=pdf_image_dpi,
         )
 
     return layout
 
 
 def process_file_with_model(
     filename: str,
     model_name: Optional[str],
     is_image: bool = False,
     ocr_strategy: str = "auto",
     ocr_languages: str = "eng",
     fixed_layouts: Optional[List[Optional[List[TextRegion]]]] = None,
     extract_tables: bool = False,
+    pdf_image_dpi: int = 200,
 ) -> DocumentLayout:
     """Processes pdf file with name filename into a DocumentLayout by using a model identified by
     model_name."""
     model = get_model(model_name)
     if isinstance(model, UnstructuredObjectDetectionModel):
         detection_model = model
         element_extraction_model = None
@@ -349,14 +390,15 @@
             filename,
             detection_model=detection_model,
             element_extraction_model=element_extraction_model,
             ocr_strategy=ocr_strategy,
             ocr_languages=ocr_languages,
             fixed_layouts=fixed_layouts,
             extract_tables=extract_tables,
+            pdf_image_dpi=pdf_image_dpi,
         )
     )
     return layout
 
 
 def get_element_from_block(
     block: TextRegion,
@@ -378,16 +420,17 @@
     )
     return element
 
 
 def load_pdf(
     filename: str,
     dpi: int = 200,
-    chunk_size: int = 100,
-) -> Tuple[List[List[TextRegion]], List[Image.Image]]:
+    output_folder: Union[str, PurePath] = None,  # type: ignore
+    path_only: bool = False,
+) -> Tuple[List[List[TextRegion]], Union[List[Image.Image], List[str]]]:
     """Loads the image and word objects from a pdf using pdfplumber and the image renderings of the
     pdf pages using pdf2image"""
     layouts = []
     for page in extract_pages(filename):
         layout = []
         height = page.height
         for element in page:
@@ -403,24 +446,30 @@
             )
             text_region = element_class(x1 * coef, y1 * coef, x2 * coef, y2 * coef, text=_text)
 
             if text_region.area() > 0:
                 layout.append(text_region)
         layouts.append(layout)
 
-    # Convert a PDF in small chunks of pages at a time (e.g. 1-10, 11-20... and so on)
-    info = pdf2image.pdfinfo_from_path(filename)
-    total_pages = info["Pages"]
-    images = []
-
-    for start_page in range(1, total_pages + 1, chunk_size):
-        end_page = min(start_page + chunk_size - 1, total_pages)
-        with tempfile.TemporaryDirectory() as tmpdir:
-            chunk_images = pdf2image.convert_from_path(
-                filename,
-                dpi=dpi,
-                first_page=start_page,
-                last_page=end_page,
-                output_folder=tmpdir,
-            )
-            images += chunk_images
+    if path_only and not output_folder:
+        raise ValueError("output_folder must be specified if path_only is true")
+
+    images = pdf2image.convert_from_path(
+        filename,
+        dpi=dpi,
+        output_folder=output_folder,
+        paths_only=path_only,
+    )
+
     return layouts, images
+
+
+def create_image_output_dir(
+    filename: Union[str, PurePath],
+) -> Union[str, PurePath]:
+    """Creates a directory to store the converted images from the pdf pages and returns the
+    directory path"""
+    parent_dir = os.path.abspath(os.path.dirname(filename))
+    f_name_without_extension = os.path.splitext(os.path.basename(filename))[0]
+    output_dir = os.path.join(parent_dir, f_name_without_extension)
+    os.makedirs(output_dir, exist_ok=True)
+    return output_dir
```

### Comparing `unstructured_inference-0.5.5/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.5.6/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/inference/ordering.py` & `unstructured_inference-0.5.6/unstructured_inference/inference/ordering.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/logger.py` & `unstructured_inference-0.5.6/unstructured_inference/logger.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/base.py` & `unstructured_inference-0.5.6/unstructured_inference/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 
+from unstructured_inference.logger import logger
 from unstructured_inference.models.chipper import MODEL_TYPES as CHIPPER_MODEL_TYPES
 from unstructured_inference.models.chipper import UnstructuredChipperModel
 from unstructured_inference.models.detectron2 import (
     MODEL_TYPES as DETECTRON2_MODEL_TYPES,
 )
 from unstructured_inference.models.detectron2 import (
     UnstructuredDetectronModel,
@@ -38,14 +39,22 @@
     elif model_name in DETECTRON2_ONNX_MODEL_TYPES:
         model = UnstructuredDetectronONNXModel()
         model.initialize(**DETECTRON2_ONNX_MODEL_TYPES[model_name])
     elif model_name in YOLOX_MODEL_TYPES:
         model = UnstructuredYoloXModel()
         model.initialize(**YOLOX_MODEL_TYPES[model_name])
     elif model_name in CHIPPER_MODEL_TYPES:
+        logger.warning(
+            "The Chipper model is currently in Beta and is not yet ready for production use. "
+            "You can reach out to the Unstructured engineering team in the Unstructured "
+            "community Slack if you have any feedback on the Chipper model. "
+            "You can join the community Slack here: "
+            "https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/"
+            "zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ",
+        )
         model = UnstructuredChipperModel()
         model.initialize(**CHIPPER_MODEL_TYPES[model_name])
     else:
         raise UnknownModelException(f"Unknown model type: {model_name}")
     return model
```

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/chipper.py` & `unstructured_inference-0.5.6/unstructured_inference/models/chipper.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.5.6/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/detectron2onnx.py` & `unstructured_inference-0.5.6/unstructured_inference/models/detectron2onnx.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/donut.py` & `unstructured_inference-0.5.6/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.5.6/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/tables.py` & `unstructured_inference-0.5.6/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.5.6/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.5.6/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/models/yolox.py` & `unstructured_inference-0.5.6/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.5.6/unstructured_inference/patches/pdfminer.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/utils.py` & `unstructured_inference-0.5.6/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference/visualize.py` & `unstructured_inference-0.5.6/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.5/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unstructured-inference
-Version: 0.5.5
+Name: unstructured_inference
+Version: 0.5.6
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -29,15 +29,15 @@
         
         ### Detectron2
         
         [Detectron2](https://github.com/facebookresearch/detectron2) is required for using models from the [layoutparser model zoo](#using-models-from-the-layoutparser-model-zoo) 
         but is not automatically installed with this package. 
         For MacOS and Linux, build from source with:
         ```shell
-        pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
+        pip install 'git+https://github.com/facebookresearch/detectron2.git@a2e43ea#egg=detectron2'
         ```
         Other install options can be found in the 
         [Detectron2 installation guide](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
         
         Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
         See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
         tips on installing Detectron2 on Windows.
```

### Comparing `unstructured_inference-0.5.5/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.5.6/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

