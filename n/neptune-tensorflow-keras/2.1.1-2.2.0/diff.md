# Comparing `tmp/neptune_tensorflow_keras-2.1.1.tar.gz` & `tmp/neptune_tensorflow_keras-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_tensorflow_keras-2.1.1.tar", max compression
+gzip compressed data, was "neptune_tensorflow_keras-2.2.0.tar", max compression
```

## Comparing `neptune_tensorflow_keras-2.1.1.tar` & `neptune_tensorflow_keras-2.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4205 2023-03-31 14:50:59.736962 neptune_tensorflow_keras-2.1.1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-03-31 14:50:59.736962 neptune_tensorflow_keras-2.1.1/LICENSE
--rw-r--r--   0        0        0     2594 2023-03-31 14:50:59.736962 neptune_tensorflow_keras-2.1.1/README.md
--rw-r--r--   0        0        0     2587 2023-03-31 14:51:11.949227 neptune_tensorflow_keras-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      737 2023-03-31 14:50:59.736962 neptune_tensorflow_keras-2.1.1/src/neptune_tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     6836 2023-03-31 14:50:59.736962 neptune_tensorflow_keras-2.1.1/src/neptune_tensorflow_keras/impl/__init__.py
--rw-r--r--   0        0        0      759 2023-03-31 14:50:59.736962 neptune_tensorflow_keras-2.1.1/src/neptune_tensorflow_keras/impl/version.py
--rw-r--r--   0        0        0     4566 1970-01-01 00:00:00.000000 neptune_tensorflow_keras-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4384 2023-07-24 09:09:32.946049 neptune_tensorflow_keras-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-07-24 09:09:32.946049 neptune_tensorflow_keras-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2594 2023-07-24 09:09:32.946049 neptune_tensorflow_keras-2.2.0/README.md
+-rw-r--r--   0        0        0     2587 2023-07-24 09:09:49.198231 neptune_tensorflow_keras-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-07-24 09:09:32.946049 neptune_tensorflow_keras-2.2.0/src/neptune_tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0     6844 2023-07-24 09:09:32.946049 neptune_tensorflow_keras-2.2.0/src/neptune_tensorflow_keras/impl/__init__.py
+-rw-r--r--   0        0        0      759 2023-07-24 09:09:32.946049 neptune_tensorflow_keras-2.2.0/src/neptune_tensorflow_keras/impl/version.py
+-rw-r--r--   0        0        0     4566 1970-01-01 00:00:00.000000 neptune_tensorflow_keras-2.2.0/PKG-INFO
```

### Comparing `neptune_tensorflow_keras-2.1.1/CHANGELOG.md` & `neptune_tensorflow_keras-2.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## neptune-tensorflow-keras 2.2.0
+
+### Fixes
+- Support logging learning_rate in Multi-GPU training set-up ([#57](https://github.com/neptune-ai/neptune-tensorflow-keras/pull/57))
+
 ## neptune-tensorflow-keras 2.1.0
 
 ### Changes
 - Removed `neptune` and `neptune-client` from base requirements.
 - Added checking `neptune` or `neptune-client` installation during runtime.
 
 ## neptune-tensorflow-keras 2.0.0
```

### Comparing `neptune_tensorflow_keras-2.1.1/LICENSE` & `neptune_tensorflow_keras-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_tensorflow_keras-2.1.1/README.md` & `neptune_tensorflow_keras-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `neptune_tensorflow_keras-2.1.1/pyproject.toml` & `neptune_tensorflow_keras-2.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 repository = "https://github.com/neptune-ai/neptune-tensorflow-keras"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations-and-supported-tools/model-training/tensorflow-keras"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-tensorflow-keras"
 readme = "README.md"
-version = "2.1.1"
+version = "2.2.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_tensorflow_keras-2.1.1/src/neptune_tensorflow_keras/__init__.py` & `neptune_tensorflow_keras-2.2.0/src/neptune_tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_tensorflow_keras-2.1.1/src/neptune_tensorflow_keras/impl/__init__.py` & `neptune_tensorflow_keras-2.2.0/src/neptune_tensorflow_keras/impl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             self._model_logger["visualization"] = _model_diagram(self.model)
 
     def on_train_batch_end(self, batch, logs=None):
         if self._log_on_batch:
             self._log_metrics(logs, "train", "batch")
 
     def on_epoch_begin(self, epoch, logs=None):
-        self._model_logger["learning_rate"].append(self.model.optimizer.learning_rate)
+        self._model_logger["learning_rate"].append(self.model.optimizer.learning_rate.numpy())
 
     def on_epoch_end(self, epoch, logs=None):
         self._log_metrics(logs, "train", "epoch")
 
     def on_test_batch_end(self, batch, logs=None):
         if self._log_on_batch:
             self._log_metrics(logs, "validation", "batch")
```

### Comparing `neptune_tensorflow_keras-2.1.1/src/neptune_tensorflow_keras/impl/version.py` & `neptune_tensorflow_keras-2.2.0/src/neptune_tensorflow_keras/impl/version.py`

 * *Files identical despite different names*

### Comparing `neptune_tensorflow_keras-2.1.1/PKG-INFO` & `neptune_tensorflow_keras-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-tensorflow-keras
-Version: 2.1.1
+Version: 2.2.0
 Summary: Neptune.ai tensorflow-keras integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
```

