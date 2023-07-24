# Comparing `tmp/energon_prometheus_exporter-0.0.4.tar.gz` & `tmp/energon_prometheus_exporter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energon_prometheus_exporter-0.0.4.tar", last modified: Mon Jul 24 01:53:21 2023, max compression
+gzip compressed data, was "energon_prometheus_exporter-0.0.5.tar", last modified: Mon Jul 24 01:54:40 2023, max compression
```

## Comparing `energon_prometheus_exporter-0.0.4.tar` & `energon_prometheus_exporter-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:53:21.291280 energon_prometheus_exporter-0.0.4/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1074 2023-07-19 00:17:29.000000 energon_prometheus_exporter-0.0.4/LICENSE
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     6563 2023-07-24 01:53:21.291280 energon_prometheus_exporter-0.0.4/PKG-INFO
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     5823 2023-07-23 06:16:52.000000 energon_prometheus_exporter-0.0.4/README.md
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      793 2023-07-24 01:53:07.000000 energon_prometheus_exporter-0.0.4/pyproject.toml
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-07-24 01:53:21.291280 energon_prometheus_exporter-0.0.4/setup.cfg
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:53:21.291280 energon_prometheus_exporter-0.0.4/src/
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:53:21.291280 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 23:48:13.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/__ init __.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:53:21.291280 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1912 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/UM25C.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/__ init __.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      402 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/constants.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     4304 2023-07-19 00:38:20.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/driver.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     2845 2023-07-24 01:14:57.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/utils.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:53:21.291280 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/__ init __.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    11192 2023-07-23 06:09:12.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/general_model.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    11948 2023-07-19 00:37:25.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/jetson_agx_orin.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    10812 2023-07-19 00:37:37.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/jetson_agx_xavier.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     5843 2023-07-19 00:37:45.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/jetson_nano_dev_kit.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     6246 2023-07-19 00:37:48.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/jetson_xavier_dev_kit.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     4770 2023-07-19 00:37:53.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/ubuntu_64.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    14408 2023-07-23 06:07:50.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/prometheus_exporter.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:53:21.291280 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter.egg-info/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     6563 2023-07-24 01:53:21.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter.egg-info/PKG-INFO
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1067 2023-07-24 01:53:21.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter.egg-info/SOURCES.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-07-24 01:53:21.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter.egg-info/dependency_links.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       40 2023-07-24 01:53:21.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter.egg-info/requires.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       28 2023-07-24 01:53:21.000000 energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter.egg-info/top_level.txt
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1074 2023-07-19 00:17:29.000000 energon_prometheus_exporter-0.0.5/LICENSE
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6563 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     5823 2023-07-23 06:16:52.000000 energon_prometheus_exporter-0.0.5/README.md
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      793 2023-07-24 01:54:33.000000 energon_prometheus_exporter-0.0.5/pyproject.toml
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/setup.cfg
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 23:48:13.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/__ init __.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1912 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/UM25C.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/__ init __.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      402 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/constants.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     4304 2023-07-19 00:38:20.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/driver.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     2845 2023-07-24 01:14:57.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/utils.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/__ init __.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    11192 2023-07-23 06:09:12.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/general_model.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    11948 2023-07-19 00:37:25.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_agx_orin.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    10812 2023-07-19 00:37:37.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_agx_xavier.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     5843 2023-07-19 00:37:45.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_nano_dev_kit.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6246 2023-07-19 00:37:48.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_xavier_dev_kit.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     4770 2023-07-19 00:37:53.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/ubuntu_64.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    14408 2023-07-23 06:07:50.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/prometheus_exporter.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6563 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1067 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       40 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/requires.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       28 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/top_level.txt
```

### Comparing `energon_prometheus_exporter-0.0.4/LICENSE` & `energon_prometheus_exporter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/PKG-INFO` & `energon_prometheus_exporter-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energon_prometheus_exporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Energon is a Prometheus compliant system monitoring tools, it focuses on the energy consumption and resource usage in constrained devices but it integrates reporting tools for desktop machine, too.
 Author-email: Matteo Mendula <mattemendu@gmail.com>
 Project-URL: Homepage, https://github.com/MatteoMendula/Energon_Prometheus_exporter
 Project-URL: Bug Tracker, https://github.com/MatteoMendula/Energon_Prometheus_exporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `energon_prometheus_exporter-0.0.4/README.md` & `energon_prometheus_exporter-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/pyproject.toml` & `energon_prometheus_exporter-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "energon_prometheus_exporter"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Matteo Mendula", email="mattemendu@gmail.com" },
 ]
 dependencies = [
 	"prometheus_client==0.17.0",
-	"PyBluez==0.30",
+	"PyBluez>=0.20",
 ]
 description = "Energon is a Prometheus compliant system monitoring tools, it focuses on the energy consumption and resource usage in constrained devices but it integrates reporting tools for desktop machine, too."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/UM25C.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/UM25C.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/driver.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/drivers/utils.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/general_model.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/general_model.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/jetson_agx_orin.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_agx_orin.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/jetson_agx_xavier.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_agx_xavier.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/jetson_nano_dev_kit.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_nano_dev_kit.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/jetson_xavier_dev_kit.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_xavier_dev_kit.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/models/ubuntu_64.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/ubuntu_64.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter/prometheus_exporter.py` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter.egg-info/PKG-INFO` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energon-prometheus-exporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Energon is a Prometheus compliant system monitoring tools, it focuses on the energy consumption and resource usage in constrained devices but it integrates reporting tools for desktop machine, too.
 Author-email: Matteo Mendula <mattemendu@gmail.com>
 Project-URL: Homepage, https://github.com/MatteoMendula/Energon_Prometheus_exporter
 Project-URL: Bug Tracker, https://github.com/MatteoMendula/Energon_Prometheus_exporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `energon_prometheus_exporter-0.0.4/src/energon_prometheus_exporter.egg-info/SOURCES.txt` & `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

