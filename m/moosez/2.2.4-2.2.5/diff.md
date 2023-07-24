# Comparing `tmp/moosez-2.2.4.tar.gz` & `tmp/moosez-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.2.4.tar", last modified: Sun Jul 23 18:59:30 2023, max compression
+gzip compressed data, was "moosez-2.2.5.tar", last modified: Mon Jul 24 10:38:06 2023, max compression
```

## Comparing `moosez-2.2.4.tar` & `moosez-2.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:59:30.419277 moosez-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-23 18:59:18.000000 moosez-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-23 18:59:30.419277 moosez-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-07-23 18:59:18.000000 moosez-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:59:30.419277 moosez-2.2.4/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-23 18:59:18.000000 moosez-2.2.4/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:59:30.419277 moosez-2.2.4/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-23 18:59:30.000000 moosez-2.2.4/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-23 18:59:30.000000 moosez-2.2.4/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 18:59:30.000000 moosez-2.2.4/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-23 18:59:30.000000 moosez-2.2.4/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-23 18:59:30.000000 moosez-2.2.4/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-23 18:59:30.000000 moosez-2.2.4/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 18:59:30.419277 moosez-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-23 18:59:18.000000 moosez-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:06.823222 moosez-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 10:37:55.000000 moosez-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-24 10:38:06.823222 moosez-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-07-24 10:37:55.000000 moosez-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:06.823222 moosez-2.2.5/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-24 10:37:55.000000 moosez-2.2.5/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:06.823222 moosez-2.2.5/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-24 10:38:06.000000 moosez-2.2.5/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 10:38:06.000000 moosez-2.2.5/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:38:06.000000 moosez-2.2.5/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 10:38:06.000000 moosez-2.2.5/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-24 10:38:06.000000 moosez-2.2.5/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 10:38:06.000000 moosez-2.2.5/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:38:06.823222 moosez-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-24 10:37:55.000000 moosez-2.2.5/setup.py
```

### Comparing `moosez-2.2.4/LICENSE` & `moosez-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/PKG-INFO` & `moosez-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.2.4
+Version: 2.2.5
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.2.4/moosez/constants.py` & `moosez-2.2.5/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez/display.py` & `moosez-2.2.5/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez/download.py` & `moosez-2.2.5/moosez/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to download the necessary
 # binaries and models for the moosez.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 import requests
-from rich.progress import Progress
-
+from rich.progress import Progress, TextColumn, BarColumn, FileSizeColumn, TransferSpeedColumn, TimeRemainingColumn
+from rich.console import Console
 from moosez import constants
 from moosez import resources
-
+import zipfile
 
 def binary(system_info, url):
     """
     Downloads the binary for the current system.
     :param system_info: A dictionary containing the system information.
     :param url: The url to download the binary from.
     """
@@ -49,41 +49,66 @@
     model_info = resources.MODELS[model_name]
     url = model_info["url"]
     filename = os.path.join(model_path, model_info["filename"])
     directory = os.path.join(model_path, model_info["directory"])
 
     if not os.path.exists(directory):
         logging.info(f" Downloading {directory}")
-        # show progress using rich
+
+        # Show progress using rich
         response = requests.get(url, stream=True)
         total_size = int(response.headers.get("Content-Length", 0))
         chunk_size = 1024 * 10
 
-        with Progress() as progress:
+        console = Console()
+        progress = Progress(
+            TextColumn("[bold blue]{task.description}"),
+            BarColumn(bar_width=None),
+            "[progress.percentage]{task.percentage:>3.0f}%",
+            "•",
+            FileSizeColumn(),
+            TransferSpeedColumn(),
+            TimeRemainingColumn(),
+            console=console,
+            expand=True
+        )
+
+        with progress:
             task = progress.add_task(f"[white] Downloading {model_name}...", total=total_size)
             for chunk in response.iter_content(chunk_size=chunk_size):
                 open(filename, "ab").write(chunk)
                 progress.update(task, advance=chunk_size)
 
         # Unzip the model
-        import zipfile
-        with Progress() as progress:
+        progress = Progress(
+            TextColumn("[bold blue]{task.description}"),
+            BarColumn(bar_width=None),
+            "[progress.percentage]{task.percentage:>3.0f}%",
+            "•",
+            FileSizeColumn(),
+            TransferSpeedColumn(),
+            TimeRemainingColumn(),
+            console=console,
+            expand=True
+        )
+
+        with progress:
             with zipfile.ZipFile(filename, 'r') as zip_ref:
                 total_size = sum((file.file_size for file in zip_ref.infolist()))
                 task = progress.add_task(f"[white] Extracting {model_name}...", total=total_size)
-                # Get the parent directory of 'directory'
                 parent_directory = os.path.dirname(directory)
                 for file in zip_ref.infolist():
                     zip_ref.extract(file, parent_directory)
                     extracted_size = file.file_size
                     progress.update(task, advance=extracted_size)
 
         logging.info(f" {os.path.basename(directory)} extracted.")
 
         # Delete the zip file
         os.remove(filename)
         print(f"{constants.ANSI_GREEN} {os.path.basename(directory)} - download complete. {constants.ANSI_RESET}")
         logging.info(f" {os.path.basename(directory)} - download complete.")
     else:
-        print(f"{constants.ANSI_GREEN} A local instance of {os.path.basename(directory)} has been detected. "
-              f"{constants.ANSI_RESET}")
+        print(
+            f"{constants.ANSI_GREEN} A local instance of {os.path.basename(directory)} has been detected. {constants.ANSI_RESET}")
         logging.info(f" A local instance of {os.path.basename(directory)} has been detected.")
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `moosez-2.2.4/moosez/file_utilities.py` & `moosez-2.2.5/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez/image_conversion.py` & `moosez-2.2.5/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez/image_processing.py` & `moosez-2.2.5/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez/input_validation.py` & `moosez-2.2.5/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez/moosez.py` & `moosez-2.2.5/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez/predict.py` & `moosez-2.2.5/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez/resources.py` & `moosez-2.2.5/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.4/moosez.egg-info/PKG-INFO` & `moosez-2.2.5/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.2.4
+Version: 2.2.5
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.2.4/setup.py` & `moosez-2.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.2.4',
+    version='2.2.5',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

