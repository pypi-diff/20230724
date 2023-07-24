# Comparing `tmp/hot-fair-utilities-1.0.52.tar.gz` & `tmp/hot-fair-utilities-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hot-fair-utilities-1.0.52.tar", last modified: Tue Jun 20 05:16:44 2023, max compression
+gzip compressed data, was "hot-fair-utilities-1.1.1.tar", last modified: Mon Jul 24 06:43:34 2023, max compression
```

## Comparing `hot-fair-utilities-1.0.52.tar` & `hot-fair-utilities-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.770195 hot-fair-utilities-1.0.52/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43175 2023-06-20 05:16:44.770195 hot-fair-utilities-1.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.762195 hot-fair-utilities-1.0.52/hot_fair_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/georeferencing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.762195 hot-fair-utilities-1.0.52/hot_fair_utilities/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/inference/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.766195 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/building_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/get_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/merge_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/polygonize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/vectorize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.766195 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/clip_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/fix_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/reproject_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.770195 hot-fair-utilities-1.0.52/hot_fair_utilities/training/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/ramp_config_base.json
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/run_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.762195 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43175 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:16:44.770195 hot-fair-utilities-1.0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.060154 hot-fair-utilities-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    42190 2023-07-24 06:43:34.060154 hot-fair-utilities-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.052154 hot-fair-utilities-1.1.1/hot_fair_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/georeferencing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.056154 hot-fair-utilities-1.1.1/hot_fair_utilities/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/inference/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.056154 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/building_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/get_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/merge_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/polygonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/vectorize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.056154 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/clip_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/fix_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/reproject_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.060154 hot-fair-utilities-1.1.1/hot_fair_utilities/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/ramp_config_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/run_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/hot_fair_utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:34.056154 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42190 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 06:43:34.000000 hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:43:34.060154 hot-fair-utilities-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:43:23.000000 hot-fair-utilities-1.1.1/setup.py
```

### Comparing `hot-fair-utilities-1.0.52/LICENSE` & `hot-fair-utilities-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/PKG-INFO` & `hot-fair-utilities-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.0.52
+Version: 1.1.1
 Summary: Utilities for AI - Assisted Mapping fAIr
-Author-email: Omdena <project@omdena.com>, Hot Tech Team <sysadmin@hotosm.org>
+Author-email: Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -672,100 +672,65 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # hot_fair_utilities ( Utilities for AI Assisted Mapping fAIr )
-Initially lib was developed during Open AI Challenge with [Omdeena](https://omdena.com/). Learn more about challenge from [here](https://www.hotosm.org/tech-blog/hot-tech-talk-open-ai-challenge/)  
 
-## `hot_fair_utilities` Installation
-
-hot_fair_utilities is collection of utilities which contains core logic for model data prepration , training and postprocessing . It can support multiple models , Currently ramp is supported. 
-
-1. To get started clone this repo first : 
-    ```
-    git clone https://github.com/hotosm/fAIr-utilities.git
-    ```
-2. Setup your virtualenv with ```python 3.8``` ( Ramp is tested with python 3.8 )
+Initially lib was developed during Open AI Challenge with [Omdeena](https://omdena.com/). Learn more about challenge from [here](https://www.hotosm.org/tech-blog/hot-tech-talk-open-ai-challenge/)
 
-3. Install tensorflow ```2.9.2``` from [here] (https://www.tensorflow.org/install/pip) According to your os
-
-#### Setup Ramp : 
+## `hot_fair_utilities` Installation
 
-4. Copy your basemodel : Basemodel is derived from ramp basemodel 
-    ```
-    git clone https://github.com/radiantearth/model_ramp_baseline.git
-    ```
+Installing all libraries could be pain so we suggest you to use docker , If you like to do it bare , You can follow `.github/build.yml`
 
-5. Clone ramp working dir 
+Clone repo
 
-    ```
-    git clone https://github.com/kshitijrajsharma/ramp-code-fAIr.git ramp-code
-    ```
+```
+git clone https://github.com/hotosm/fAIr-utilities.git
+```
 
-6. Copy base model to ramp-code 
-    ```
-    cp -r model_ramp_baseline/data/input/checkpoint.tf ramp-code/ramp/checkpoint.tf
-    ```
+Navigate to fAIr-utilities
 
-7. Install native bindings 
-    - Install Numpy 
-        ```
-        pip install numpy==1.23.5
-        ```
-    - Install [gdal](https://gdal.org/index.html) .
+```
+cd fAIr-utilities
+```
+Build Docker
 
-        for eg : on Ubuntu 
-        ```
-        sudo add-apt-repository ppa:ubuntugis/ppa && sudo apt-get update
-        sudo apt-get install gdal-bin
-        sudo apt-get install libgdal-dev
-        export CPLUS_INCLUDE_PATH=/usr/include/gdal
-        export C_INCLUDE_PATH=/usr/include/gdal
-        pip install --global-option=build_ext --global-option="-I/usr/include/gdal" GDAL==`gdal-config --version`        
-        ```
-        on conda : 
-        ```
-        conda install -c conda-forge gdal
-        ```
-    - Install rasterio 
+```
+docker build --tag fairutils .
+```
 
-        for eg: on ubuntu : 
-        ```
-        sudo apt-get install -y python3-rasterio
-        ```
-        on conda : 
-        ```
-        conda install -c conda-forge rasterio
-        ```
+Run Container with default Jupyter Notebook , Or add `bash` at end to see terminal
 
-8. Install ramp requirements 
+```
+docker run -it --rm --gpus=all  -p 8888:8888 fairutils
+```
 
-    Install necessary requirements for ramp  and hot_fair_utilites
-         
-    ```
-    cd ramp-code && cd colab && make install  && cd ../.. && pip install -e .
-    ```
+[Optional] If you have downloaded RAMP already , By Default tf is set as Ramp_Home , You can change that by attaching your ramp-home volume to container as tf
 
+if not you can skip this step , Ramp code will be downloaded on package_test.ipynb
 
+```
+-v /home/hotosm/fAIr-utilities:/tf
+```
 
-## Conda Virtual Environment
-Create from env fle 
+## Test inside Docker Container
 
 ```
-conda env create -f environment.yml
+docker run -it --rm --gpus=all  -p 8888:8888 fairutils bash
 ```
-Create your own
 
 ```
-conda create -n fAIr python=3.8
-conda activate fAIr
-conda install -c conda-forge gdal
-conda install -c conda-forge geopandas
-pip install pyogrio rasterio tensorflow
-pip install -e hot_fair_utilities
+python test_app.py
 ```
 
-## Test Installation and workflow 
+## Test Installation and workflow
+
+You can run [`package_test.ipynb`](./Package_Test.ipynb) on your notebook from docker to test the installation and workflow with sample data provided , Or open with [collab and connect your runtime locally](https://research.google.com/colaboratory/local-runtimes.html#:~:text=In%20Colab%2C%20click%20the%20%22Connect,connected%20to%20your%20local%20runtime.)
+
+## Get started with development
+
+Now you can play with your data , use your own data , use different models for testing and also Help me Improve me !
 
-You can run ```package_test.ipynb``` to your pc to test the installation and workflow with sample data provided 
+### Version Control
+Follow [Version Control Docs](./docs/Version_control.md) to publish and maintain new version
```

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/georeferencing.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/georeferencing.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/inference/predict.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/inference/predict.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/inference/utils.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/inference/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/building_footprint.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/building_footprint.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/get_polygons.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/get_polygons.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/merge_polygons.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/merge_polygons.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/polygonize.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/polygonize.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/utils.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/vectorize.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/postprocessing/vectorize.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/clip_labels.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/clip_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/fix_labels.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/fix_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/preprocess.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/reproject_labels.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/preprocessing/reproject_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/training/cleanup.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/training/cleanup.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/training/prepare_data.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/training/prepare_data.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/training/ramp_config_base.json` & `hot-fair-utilities-1.1.1/hot_fair_utilities/training/ramp_config_base.json`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/training/run_training.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/training/run_training.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/training/train.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/training/train.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities/utils.py` & `hot-fair-utilities-1.1.1/hot_fair_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/PKG-INFO` & `hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.0.52
+Version: 1.1.1
 Summary: Utilities for AI - Assisted Mapping fAIr
-Author-email: Omdena <project@omdena.com>, Hot Tech Team <sysadmin@hotosm.org>
+Author-email: Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -672,100 +672,65 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # hot_fair_utilities ( Utilities for AI Assisted Mapping fAIr )
-Initially lib was developed during Open AI Challenge with [Omdeena](https://omdena.com/). Learn more about challenge from [here](https://www.hotosm.org/tech-blog/hot-tech-talk-open-ai-challenge/)  
 
-## `hot_fair_utilities` Installation
-
-hot_fair_utilities is collection of utilities which contains core logic for model data prepration , training and postprocessing . It can support multiple models , Currently ramp is supported. 
-
-1. To get started clone this repo first : 
-    ```
-    git clone https://github.com/hotosm/fAIr-utilities.git
-    ```
-2. Setup your virtualenv with ```python 3.8``` ( Ramp is tested with python 3.8 )
+Initially lib was developed during Open AI Challenge with [Omdeena](https://omdena.com/). Learn more about challenge from [here](https://www.hotosm.org/tech-blog/hot-tech-talk-open-ai-challenge/)
 
-3. Install tensorflow ```2.9.2``` from [here] (https://www.tensorflow.org/install/pip) According to your os
-
-#### Setup Ramp : 
+## `hot_fair_utilities` Installation
 
-4. Copy your basemodel : Basemodel is derived from ramp basemodel 
-    ```
-    git clone https://github.com/radiantearth/model_ramp_baseline.git
-    ```
+Installing all libraries could be pain so we suggest you to use docker , If you like to do it bare , You can follow `.github/build.yml`
 
-5. Clone ramp working dir 
+Clone repo
 
-    ```
-    git clone https://github.com/kshitijrajsharma/ramp-code-fAIr.git ramp-code
-    ```
+```
+git clone https://github.com/hotosm/fAIr-utilities.git
+```
 
-6. Copy base model to ramp-code 
-    ```
-    cp -r model_ramp_baseline/data/input/checkpoint.tf ramp-code/ramp/checkpoint.tf
-    ```
+Navigate to fAIr-utilities
 
-7. Install native bindings 
-    - Install Numpy 
-        ```
-        pip install numpy==1.23.5
-        ```
-    - Install [gdal](https://gdal.org/index.html) .
+```
+cd fAIr-utilities
+```
+Build Docker
 
-        for eg : on Ubuntu 
-        ```
-        sudo add-apt-repository ppa:ubuntugis/ppa && sudo apt-get update
-        sudo apt-get install gdal-bin
-        sudo apt-get install libgdal-dev
-        export CPLUS_INCLUDE_PATH=/usr/include/gdal
-        export C_INCLUDE_PATH=/usr/include/gdal
-        pip install --global-option=build_ext --global-option="-I/usr/include/gdal" GDAL==`gdal-config --version`        
-        ```
-        on conda : 
-        ```
-        conda install -c conda-forge gdal
-        ```
-    - Install rasterio 
+```
+docker build --tag fairutils .
+```
 
-        for eg: on ubuntu : 
-        ```
-        sudo apt-get install -y python3-rasterio
-        ```
-        on conda : 
-        ```
-        conda install -c conda-forge rasterio
-        ```
+Run Container with default Jupyter Notebook , Or add `bash` at end to see terminal
 
-8. Install ramp requirements 
+```
+docker run -it --rm --gpus=all  -p 8888:8888 fairutils
+```
 
-    Install necessary requirements for ramp  and hot_fair_utilites
-         
-    ```
-    cd ramp-code && cd colab && make install  && cd ../.. && pip install -e .
-    ```
+[Optional] If you have downloaded RAMP already , By Default tf is set as Ramp_Home , You can change that by attaching your ramp-home volume to container as tf
 
+if not you can skip this step , Ramp code will be downloaded on package_test.ipynb
 
+```
+-v /home/hotosm/fAIr-utilities:/tf
+```
 
-## Conda Virtual Environment
-Create from env fle 
+## Test inside Docker Container
 
 ```
-conda env create -f environment.yml
+docker run -it --rm --gpus=all  -p 8888:8888 fairutils bash
 ```
-Create your own
 
 ```
-conda create -n fAIr python=3.8
-conda activate fAIr
-conda install -c conda-forge gdal
-conda install -c conda-forge geopandas
-pip install pyogrio rasterio tensorflow
-pip install -e hot_fair_utilities
+python test_app.py
 ```
 
-## Test Installation and workflow 
+## Test Installation and workflow
+
+You can run [`package_test.ipynb`](./Package_Test.ipynb) on your notebook from docker to test the installation and workflow with sample data provided , Or open with [collab and connect your runtime locally](https://research.google.com/colaboratory/local-runtimes.html#:~:text=In%20Colab%2C%20click%20the%20%22Connect,connected%20to%20your%20local%20runtime.)
+
+## Get started with development
+
+Now you can play with your data , use your own data , use different models for testing and also Help me Improve me !
 
-You can run ```package_test.ipynb``` to your pc to test the installation and workflow with sample data provided 
+### Version Control
+Follow [Version Control Docs](./docs/Version_control.md) to publish and maintain new version
```

### Comparing `hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/SOURCES.txt` & `hot-fair-utilities-1.1.1/hot_fair_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.52/pyproject.toml` & `hot-fair-utilities-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hot-fair-utilities"
-version = "1.0.52"
+version = "1.1.1"
 description = "Utilities for AI - Assisted Mapping fAIr"
 readme = "README.md"
-authors = [{ name = "Omdena", email = "project@omdena.com" },{ name = "Hot Tech Team", email = "sysadmin@hotosm.org" }]
+authors = [{ name = "Hot Tech Team", email = "sysadmin@hotosm.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
 ]
 keywords = [
     "preprocessing", "inference", 
@@ -47,7 +47,14 @@
     ]
 
 [tool.isort]
 profile                   = "black"
 import_heading_stdlib     = "Standard library imports"
 import_heading_thirdparty = "Third party imports"
 import_heading_firstparty = "Reader imports"
+
+[tool.commitizen]
+name = "cz_conventional_commits"
+tag_format = "v$version"
+version_scheme = "semver"
+version_provider = "pep621"
+update_changelog_on_bump = true
```

