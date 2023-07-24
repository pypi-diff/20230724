# Comparing `tmp/eventdetector_ts-1.0.4.tar.gz` & `tmp/eventdetector_ts-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventdetector_ts-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eventdetector_ts-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eventdetector_ts-1.0.4.tar` & `eventdetector_ts-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2023-07-20 12:55:07.352016 eventdetector_ts-1.0.4/LICENSE
--rw-r--r--   0        0        0     9461 2023-07-21 11:33:27.408160 eventdetector_ts-1.0.4/README.md
--rw-r--r--   0        0        0     6217 2023-07-20 17:52:46.056050 eventdetector_ts-1.0.4/eventdetector_ts/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 07:12:45.920022 eventdetector_ts-1.0.4/eventdetector_ts/data/__init__.py
--rw-r--r--   0        0        0    20804 2023-07-21 17:54:15.480210 eventdetector_ts-1.0.4/eventdetector_ts/data/helpers.py
--rw-r--r--   0        0        0     2168 2023-07-21 16:36:06.500153 eventdetector_ts-1.0.4/eventdetector_ts/data/interval.py
--rw-r--r--   0        0        0       64 2023-05-09 10:09:45.592180 eventdetector_ts-1.0.4/eventdetector_ts/metamodel/__init__.py
--rw-r--r--   0        0        0    21779 2023-07-21 17:56:22.596212 eventdetector_ts-1.0.4/eventdetector_ts/metamodel/meta_model.py
--rw-r--r--   0        0        0    12788 2023-07-21 11:37:16.692162 eventdetector_ts-1.0.4/eventdetector_ts/metamodel/utils.py
--rw-r--r--   0        0        0       60 2023-05-09 10:13:53.384183 eventdetector_ts-1.0.4/eventdetector_ts/models/__init__.py
--rw-r--r--   0        0        0     6836 2023-05-17 05:43:25.080012 eventdetector_ts-1.0.4/eventdetector_ts/models/helpers.py
--rw-r--r--   0        0        0    33455 2023-07-21 10:50:59.900128 eventdetector_ts-1.0.4/eventdetector_ts/models/models_builder.py
--rw-r--r--   0        0        0    12722 2023-07-21 10:51:06.600129 eventdetector_ts-1.0.4/eventdetector_ts/models/models_trainer.py
--rw-r--r--   0        0        0       53 2023-05-10 06:54:30.672029 eventdetector_ts-1.0.4/eventdetector_ts/optimization/__init__.py
--rw-r--r--   0        0        0      781 2023-05-15 09:49:54.420030 eventdetector_ts-1.0.4/eventdetector_ts/optimization/algorithms.py
--rw-r--r--   0        0        0    11507 2023-07-21 16:36:06.500153 eventdetector_ts-1.0.4/eventdetector_ts/optimization/event_extraction_pipeline.py
--rw-r--r--   0        0        0      180 2023-05-26 13:37:24.600319 eventdetector_ts-1.0.4/eventdetector_ts/plotter/__init__.py
--rw-r--r--   0        0        0     1358 2023-07-21 10:50:59.912129 eventdetector_ts-1.0.4/eventdetector_ts/plotter/helpers.py
--rw-r--r--   0        0        0    11202 2023-07-21 10:50:59.896129 eventdetector_ts-1.0.4/eventdetector_ts/plotter/plotter.py
--rw-r--r--   0        0        0       53 2023-05-23 06:48:12.328047 eventdetector_ts-1.0.4/eventdetector_ts/prediction/__init__.py
--rw-r--r--   0        0        0     7874 2023-07-21 10:50:59.876129 eventdetector_ts-1.0.4/eventdetector_ts/prediction/prediction.py
--rw-r--r--   0        0        0     1011 2023-07-21 10:50:59.968129 eventdetector_ts-1.0.4/eventdetector_ts/prediction/utils.py
--rw-r--r--   0        0        0     1472 2023-07-21 17:57:58.624213 eventdetector_ts-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    10850 1970-01-01 00:00:00.000000 eventdetector_ts-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 12:55:07.352016 eventdetector_ts-1.0.5/LICENSE
+-rw-r--r--   0        0        0     9647 2023-07-24 09:59:30.540082 eventdetector_ts-1.0.5/README.md
+-rw-r--r--   0        0        0     6217 2023-07-20 17:52:46.056050 eventdetector_ts-1.0.5/eventdetector_ts/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:12:45.920022 eventdetector_ts-1.0.5/eventdetector_ts/data/__init__.py
+-rw-r--r--   0        0        0    20804 2023-07-21 17:54:15.480210 eventdetector_ts-1.0.5/eventdetector_ts/data/helpers.py
+-rw-r--r--   0        0        0     2168 2023-07-21 16:36:06.500153 eventdetector_ts-1.0.5/eventdetector_ts/data/interval.py
+-rw-r--r--   0        0        0       64 2023-05-09 10:09:45.592180 eventdetector_ts-1.0.5/eventdetector_ts/metamodel/__init__.py
+-rw-r--r--   0        0        0    21779 2023-07-21 17:56:22.596212 eventdetector_ts-1.0.5/eventdetector_ts/metamodel/meta_model.py
+-rw-r--r--   0        0        0    12788 2023-07-21 11:37:16.692162 eventdetector_ts-1.0.5/eventdetector_ts/metamodel/utils.py
+-rw-r--r--   0        0        0       60 2023-05-09 10:13:53.384183 eventdetector_ts-1.0.5/eventdetector_ts/models/__init__.py
+-rw-r--r--   0        0        0     6836 2023-05-17 05:43:25.080012 eventdetector_ts-1.0.5/eventdetector_ts/models/helpers.py
+-rw-r--r--   0        0        0    33455 2023-07-21 10:50:59.900128 eventdetector_ts-1.0.5/eventdetector_ts/models/models_builder.py
+-rw-r--r--   0        0        0    12722 2023-07-21 10:51:06.600129 eventdetector_ts-1.0.5/eventdetector_ts/models/models_trainer.py
+-rw-r--r--   0        0        0       53 2023-05-10 06:54:30.672029 eventdetector_ts-1.0.5/eventdetector_ts/optimization/__init__.py
+-rw-r--r--   0        0        0      781 2023-05-15 09:49:54.420030 eventdetector_ts-1.0.5/eventdetector_ts/optimization/algorithms.py
+-rw-r--r--   0        0        0    11507 2023-07-21 16:36:06.500153 eventdetector_ts-1.0.5/eventdetector_ts/optimization/event_extraction_pipeline.py
+-rw-r--r--   0        0        0      180 2023-05-26 13:37:24.600319 eventdetector_ts-1.0.5/eventdetector_ts/plotter/__init__.py
+-rw-r--r--   0        0        0     1358 2023-07-21 10:50:59.912129 eventdetector_ts-1.0.5/eventdetector_ts/plotter/helpers.py
+-rw-r--r--   0        0        0    11202 2023-07-21 10:50:59.896129 eventdetector_ts-1.0.5/eventdetector_ts/plotter/plotter.py
+-rw-r--r--   0        0        0       53 2023-05-23 06:48:12.328047 eventdetector_ts-1.0.5/eventdetector_ts/prediction/__init__.py
+-rw-r--r--   0        0        0     7874 2023-07-21 10:50:59.876129 eventdetector_ts-1.0.5/eventdetector_ts/prediction/prediction.py
+-rw-r--r--   0        0        0     1011 2023-07-21 10:50:59.968129 eventdetector_ts-1.0.5/eventdetector_ts/prediction/utils.py
+-rw-r--r--   0        0        0     1472 2023-07-24 10:05:33.852087 eventdetector_ts-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11036 1970-01-01 00:00:00.000000 eventdetector_ts-1.0.5/PKG-INFO
```

### Comparing `eventdetector_ts-1.0.4/LICENSE` & `eventdetector_ts-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/README.md` & `eventdetector_ts-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+<h1 align="center">
+<img src="https://raw.githubusercontent.com/menouarazib/eventdetector/a4d7e137f88a4a476ba6d07f43337ec39543a522/images/logo_eventdetector.svg" width="400">
+</h1><br>
+
 Universal Event Detection in Time Series
 ==========================================================
 
 Welcome to **Event Detector**, a Python package for detecting events in time series data. The emphasis of this package
 is on offering useful machine learning functionalities, such as customizing and fitting the model on multidimensional
 time series, training on large datasets, ensemble models, and providing rich support for event detection in time
 series.
```

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/__init__.py` & `eventdetector_ts-1.0.5/eventdetector_ts/__init__.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/data/helpers.py` & `eventdetector_ts-1.0.5/eventdetector_ts/data/helpers.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/data/interval.py` & `eventdetector_ts-1.0.5/eventdetector_ts/data/interval.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/metamodel/meta_model.py` & `eventdetector_ts-1.0.5/eventdetector_ts/metamodel/meta_model.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/metamodel/utils.py` & `eventdetector_ts-1.0.5/eventdetector_ts/metamodel/utils.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/models/helpers.py` & `eventdetector_ts-1.0.5/eventdetector_ts/models/helpers.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/models/models_builder.py` & `eventdetector_ts-1.0.5/eventdetector_ts/models/models_builder.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/models/models_trainer.py` & `eventdetector_ts-1.0.5/eventdetector_ts/models/models_trainer.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/optimization/algorithms.py` & `eventdetector_ts-1.0.5/eventdetector_ts/optimization/algorithms.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/optimization/event_extraction_pipeline.py` & `eventdetector_ts-1.0.5/eventdetector_ts/optimization/event_extraction_pipeline.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/plotter/helpers.py` & `eventdetector_ts-1.0.5/eventdetector_ts/plotter/helpers.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/plotter/plotter.py` & `eventdetector_ts-1.0.5/eventdetector_ts/plotter/plotter.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/prediction/prediction.py` & `eventdetector_ts-1.0.5/eventdetector_ts/prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/eventdetector_ts/prediction/utils.py` & `eventdetector_ts-1.0.5/eventdetector_ts/prediction/utils.py`

 * *Files identical despite different names*

### Comparing `eventdetector_ts-1.0.4/pyproject.toml` & `eventdetector_ts-1.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "eventdetector_ts"
-version = "1.0.4"
+version = "1.0.5"
 description = "This package provides an easy-to-use and efficient solution for event detection in time series data. It includes various functionalities and tools that enable users to apply our framework to their own data sets and customize the detection process according to their specific needs."
 keywords = ["Event Detection", "Time Series", "Universal Approximation Theory", "Deep Learning", "Stacking Ensemble Learning"]
 authors = [
     { name = "Menouar Azib", email = "menouar.azib@akkodis.com" }
 ]
 
 maintainers = [
```

### Comparing `eventdetector_ts-1.0.4/PKG-INFO` & `eventdetector_ts-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventdetector_ts
-Version: 1.0.4
+Version: 1.0.5
 Summary: This package provides an easy-to-use and efficient solution for event detection in time series data. It includes various functionalities and tools that enable users to apply our framework to their own data sets and customize the detection process according to their specific needs.
 Keywords: Event Detection,Time Series,Universal Approximation Theory,Deep Learning,Stacking Ensemble Learning
 Author-email: Menouar Azib <menouar.azib@akkodis.com>
 Maintainer-email: Menouar Azib <menouar.azib@akkodis.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,18 @@
 Requires-Dist: colorlog==6.7.0
 Requires-Dist: pydot==1.4.2
 Requires-Dist: pyqt5==5.15.9
 Requires-Dist: tqdm==4.64.1
 Project-URL: Bug Tracker, https://github.com/menouarazib/eventdetector/issues
 Project-URL: Homepage, https://github.com/menouarazib/eventdetector
 
+<h1 align="center">
+<img src="https://raw.githubusercontent.com/menouarazib/eventdetector/a4d7e137f88a4a476ba6d07f43337ec39543a522/images/logo_eventdetector.svg" width="400">
+</h1><br>
+
 Universal Event Detection in Time Series
 ==========================================================
 
 Welcome to **Event Detector**, a Python package for detecting events in time series data. The emphasis of this package
 is on offering useful machine learning functionalities, such as customizing and fitting the model on multidimensional
 time series, training on large datasets, ensemble models, and providing rich support for event detection in time
 series.
```

