# Comparing `tmp/flaxspeaker-0.0.1.tar.gz` & `tmp/flaxspeaker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaxspeaker-0.0.1.tar", last modified: Sun Jul 23 17:40:55 2023, max compression
+gzip compressed data, was "flaxspeaker-0.0.2.tar", last modified: Mon Jul 24 20:47:19 2023, max compression
```

## Comparing `flaxspeaker-0.0.1.tar` & `flaxspeaker-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-23 17:40:55.266647 flaxspeaker-0.0.1/
--rw-r--r--   0 quan      (1000) quan      (1000)    11524 2023-07-19 15:46:32.000000 flaxspeaker-0.0.1/LICENSE
--rw-r--r--   0 quan      (1000) quan      (1000)      726 2023-07-23 17:40:55.266647 flaxspeaker-0.0.1/PKG-INFO
--rw-r--r--   0 quan      (1000) quan      (1000)      252 2023-07-21 15:35:53.000000 flaxspeaker-0.0.1/README.md
-drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-23 17:40:55.256647 flaxspeaker-0.0.1/flaxspeaker/
--rw-r--r--   0 quan      (1000) quan      (1000)       21 2023-07-23 17:32:12.000000 flaxspeaker-0.0.1/flaxspeaker/__init__.py
--rw-r--r--   0 quan      (1000) quan      (1000)     1707 2023-07-21 18:01:45.000000 flaxspeaker-0.0.1/flaxspeaker/dataset.py
--rw-r--r--   0 quan      (1000) quan      (1000)     5924 2023-07-23 17:33:26.000000 flaxspeaker-0.0.1/flaxspeaker/evaluation.py
--rw-r--r--   0 quan      (1000) quan      (1000)     3873 2023-07-23 17:33:31.000000 flaxspeaker-0.0.1/flaxspeaker/feature_extraction.py
--rw-r--r--   0 quan      (1000) quan      (1000)     8845 2023-07-23 17:33:37.000000 flaxspeaker-0.0.1/flaxspeaker/neural_net.py
--rw-r--r--   0 quan      (1000) quan      (1000)      845 2023-07-23 17:33:40.000000 flaxspeaker-0.0.1/flaxspeaker/specaug.py
-drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-23 17:40:55.266647 flaxspeaker-0.0.1/flaxspeaker.egg-info/
--rw-r--r--   0 quan      (1000) quan      (1000)      726 2023-07-23 17:40:55.000000 flaxspeaker-0.0.1/flaxspeaker.egg-info/PKG-INFO
--rw-r--r--   0 quan      (1000) quan      (1000)      322 2023-07-23 17:40:55.000000 flaxspeaker-0.0.1/flaxspeaker.egg-info/SOURCES.txt
--rw-r--r--   0 quan      (1000) quan      (1000)        1 2023-07-23 17:40:55.000000 flaxspeaker-0.0.1/flaxspeaker.egg-info/dependency_links.txt
--rw-r--r--   0 quan      (1000) quan      (1000)       12 2023-07-23 17:40:55.000000 flaxspeaker-0.0.1/flaxspeaker.egg-info/top_level.txt
--rw-r--r--   0 quan      (1000) quan      (1000)       38 2023-07-23 17:40:55.266647 flaxspeaker-0.0.1/setup.cfg
--rw-r--r--   0 quan      (1000) quan      (1000)      721 2023-07-23 15:59:42.000000 flaxspeaker-0.0.1/setup.py
+drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-24 20:47:19.983025 flaxspeaker-0.0.2/
+-rw-r--r--   0 quan      (1000) quan      (1000)    11524 2023-07-19 15:46:32.000000 flaxspeaker-0.0.2/LICENSE
+-rw-r--r--   0 quan      (1000) quan      (1000)     3049 2023-07-24 20:47:19.983025 flaxspeaker-0.0.2/PKG-INFO
+-rw-r--r--   0 quan      (1000) quan      (1000)     2575 2023-07-24 20:46:24.000000 flaxspeaker-0.0.2/README.md
+drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-24 20:47:19.983025 flaxspeaker-0.0.2/flaxspeaker/
+-rw-r--r--   0 quan      (1000) quan      (1000)       21 2023-07-23 17:32:12.000000 flaxspeaker-0.0.2/flaxspeaker/__init__.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     2020 2023-07-24 20:30:11.000000 flaxspeaker-0.0.2/flaxspeaker/__main__.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     1707 2023-07-21 18:01:45.000000 flaxspeaker-0.0.2/flaxspeaker/dataset.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     5924 2023-07-23 18:00:14.000000 flaxspeaker-0.0.2/flaxspeaker/evaluation.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     3873 2023-07-23 17:33:31.000000 flaxspeaker-0.0.2/flaxspeaker/feature_extraction.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     1349 2023-07-24 20:30:37.000000 flaxspeaker-0.0.2/flaxspeaker/generate_csv.py
+-rw-r--r--   0 quan      (1000) quan      (1000)     8793 2023-07-23 18:10:00.000000 flaxspeaker-0.0.2/flaxspeaker/neural_net.py
+-rw-r--r--   0 quan      (1000) quan      (1000)      845 2023-07-23 17:33:40.000000 flaxspeaker-0.0.2/flaxspeaker/specaug.py
+drwxr-xr-x   0 quan      (1000) quan      (1000)        0 2023-07-24 20:47:19.983025 flaxspeaker-0.0.2/flaxspeaker.egg-info/
+-rw-r--r--   0 quan      (1000) quan      (1000)     3049 2023-07-24 20:47:19.000000 flaxspeaker-0.0.2/flaxspeaker.egg-info/PKG-INFO
+-rw-r--r--   0 quan      (1000) quan      (1000)      374 2023-07-24 20:47:19.000000 flaxspeaker-0.0.2/flaxspeaker.egg-info/SOURCES.txt
+-rw-r--r--   0 quan      (1000) quan      (1000)        1 2023-07-24 20:47:19.000000 flaxspeaker-0.0.2/flaxspeaker.egg-info/dependency_links.txt
+-rw-r--r--   0 quan      (1000) quan      (1000)       12 2023-07-24 20:47:19.000000 flaxspeaker-0.0.2/flaxspeaker.egg-info/top_level.txt
+-rw-r--r--   0 quan      (1000) quan      (1000)       38 2023-07-24 20:47:19.983025 flaxspeaker-0.0.2/setup.cfg
+-rw-r--r--   0 quan      (1000) quan      (1000)      721 2023-07-24 20:31:18.000000 flaxspeaker-0.0.2/setup.py
```

### Comparing `flaxspeaker-0.0.1/LICENSE` & `flaxspeaker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flaxspeaker-0.0.1/flaxspeaker/dataset.py` & `flaxspeaker-0.0.2/flaxspeaker/dataset.py`

 * *Files identical despite different names*

### Comparing `flaxspeaker-0.0.1/flaxspeaker/evaluation.py` & `flaxspeaker-0.0.2/flaxspeaker/evaluation.py`

 * *Files identical despite different names*

### Comparing `flaxspeaker-0.0.1/flaxspeaker/feature_extraction.py` & `flaxspeaker-0.0.2/flaxspeaker/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `flaxspeaker-0.0.1/flaxspeaker/neural_net.py` & `flaxspeaker-0.0.2/flaxspeaker/neural_net.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import time
 import jax
 import jax.numpy as jnp
 import flax
 from flax.training import train_state
 from flax import linen as nn
-import tensorflow as tf
 import optax
 import matplotlib.pyplot as plt
 import multiprocessing
 from typing import Optional
 import munch
 from functools import partial
 import sys
@@ -143,15 +142,14 @@
     """Create speaker encoder model."""
     if myconfig.model.use_transformer:
         encoder = TransformerSpeakerEncoder(
             transformer_config=myconfig.model.transformer)
     else:
         encoder = LstmSpeakerEncoder(lstm_config=myconfig.model.lstm)
 
-    tf.random.set_seed(0)
     init_rng = jax.random.PRNGKey(0)
     state = create_train_state(encoder, init_rng, myconfig)
     if load_from:
         state = load_model(load_from, state)
 
     return encoder, state
```

### Comparing `flaxspeaker-0.0.1/flaxspeaker/specaug.py` & `flaxspeaker-0.0.2/flaxspeaker/specaug.py`

 * *Files identical despite different names*

### Comparing `flaxspeaker-0.0.1/setup.py` & `flaxspeaker-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Setup script for the package."""
 
 import setuptools
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 with open("README.md", "r") as file_object:
     LONG_DESCRIPTION = file_object.read()
 
 setuptools.setup(
     name="flaxspeaker",
     version=VERSION,
```

