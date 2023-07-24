# Comparing `tmp/energon_prometheus_exporter-0.0.5.tar.gz` & `tmp/energon_prometheus_exporter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energon_prometheus_exporter-0.0.5.tar", last modified: Mon Jul 24 01:54:40 2023, max compression
+gzip compressed data, was "energon_prometheus_exporter-0.0.6.tar", last modified: Mon Jul 24 02:23:35 2023, max compression
```

## Comparing `energon_prometheus_exporter-0.0.5.tar` & `energon_prometheus_exporter-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1074 2023-07-19 00:17:29.000000 energon_prometheus_exporter-0.0.5/LICENSE
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     6563 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/PKG-INFO
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     5823 2023-07-23 06:16:52.000000 energon_prometheus_exporter-0.0.5/README.md
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      793 2023-07-24 01:54:33.000000 energon_prometheus_exporter-0.0.5/pyproject.toml
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/setup.cfg
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 23:48:13.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/__ init __.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1912 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/UM25C.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/__ init __.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)      402 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/constants.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     4304 2023-07-19 00:38:20.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/driver.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     2845 2023-07-24 01:14:57.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/utils.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/__ init __.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    11192 2023-07-23 06:09:12.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/general_model.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    11948 2023-07-19 00:37:25.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_agx_orin.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    10812 2023-07-19 00:37:37.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_agx_xavier.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     5843 2023-07-19 00:37:45.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_nano_dev_kit.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     6246 2023-07-19 00:37:48.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_xavier_dev_kit.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     4770 2023-07-19 00:37:53.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/ubuntu_64.py
--rw-rw-r--   0 matteo    (1000) matteo    (1000)    14408 2023-07-23 06:07:50.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/prometheus_exporter.py
-drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 01:54:40.210758 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     6563 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/PKG-INFO
--rw-rw-r--   0 matteo    (1000) matteo    (1000)     1067 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/SOURCES.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/dependency_links.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       40 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/requires.txt
--rw-rw-r--   0 matteo    (1000) matteo    (1000)       28 2023-07-24 01:54:40.000000 energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/top_level.txt
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 02:23:35.250571 energon_prometheus_exporter-0.0.6/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1074 2023-07-19 00:17:29.000000 energon_prometheus_exporter-0.0.6/LICENSE
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6563 2023-07-24 02:23:35.246571 energon_prometheus_exporter-0.0.6/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     5823 2023-07-23 06:16:52.000000 energon_prometheus_exporter-0.0.6/README.md
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      793 2023-07-24 02:23:22.000000 energon_prometheus_exporter-0.0.6/pyproject.toml
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       38 2023-07-24 02:23:35.250571 energon_prometheus_exporter-0.0.6/setup.cfg
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 02:23:35.246571 energon_prometheus_exporter-0.0.6/src/
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 02:23:35.246571 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 23:48:13.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/__ init __.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 02:23:35.246571 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1912 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/UM25C.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/__ init __.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)      402 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/constants.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     4304 2023-07-24 02:08:26.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/driver.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     2845 2023-07-24 01:14:57.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/utils.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 02:23:35.246571 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        0 2023-07-18 17:47:19.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/__ init __.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    11401 2023-07-24 02:05:52.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/general_model.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    11948 2023-07-19 00:37:25.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/jetson_agx_orin.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    10812 2023-07-19 00:37:37.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/jetson_agx_xavier.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     5843 2023-07-19 00:37:45.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/jetson_nano_dev_kit.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6246 2023-07-19 00:37:48.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/jetson_xavier_dev_kit.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     5081 2023-07-24 02:22:27.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/ubuntu_64.py
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)    15041 2023-07-24 02:18:28.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/prometheus_exporter.py
+drwxrwxr-x   0 matteo    (1000) matteo    (1000)        0 2023-07-24 02:23:35.246571 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter.egg-info/
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     6563 2023-07-24 02:23:35.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter.egg-info/PKG-INFO
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)     1067 2023-07-24 02:23:35.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)        1 2023-07-24 02:23:35.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       40 2023-07-24 02:23:35.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter.egg-info/requires.txt
+-rw-rw-r--   0 matteo    (1000) matteo    (1000)       28 2023-07-24 02:23:35.000000 energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter.egg-info/top_level.txt
```

### Comparing `energon_prometheus_exporter-0.0.5/LICENSE` & `energon_prometheus_exporter-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/PKG-INFO` & `energon_prometheus_exporter-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energon_prometheus_exporter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Energon is a Prometheus compliant system monitoring tools, it focuses on the energy consumption and resource usage in constrained devices but it integrates reporting tools for desktop machine, too.
 Author-email: Matteo Mendula <mattemendu@gmail.com>
 Project-URL: Homepage, https://github.com/MatteoMendula/Energon_Prometheus_exporter
 Project-URL: Bug Tracker, https://github.com/MatteoMendula/Energon_Prometheus_exporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `energon_prometheus_exporter-0.0.5/README.md` & `energon_prometheus_exporter-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/pyproject.toml` & `energon_prometheus_exporter-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "energon_prometheus_exporter"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Matteo Mendula", email="mattemendu@gmail.com" },
 ]
 dependencies = [
 	"prometheus_client==0.17.0",
 	"PyBluez>=0.20",
 ]
```

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/UM25C.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/UM25C.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/driver.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/drivers/utils.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/general_model.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/general_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
             if not _interface_name.startswith("w"):
                 continue
 
             interface_name = utils.clean_metric_name_to_prometheus_format(_interface_name)
             
             link_quality = utils.run_command_and_get_output("iwconfig " + interface_name)
             data = {}
+            data["link_quality"] = constants.ERROR_WHILE_READING_VALUE
+            data["signal_level"] = constants.ERROR_WHILE_READING_VALUE
+            data["bit_rate"] = constants.ERROR_WHILE_READING_VALUE
             if not link_quality["error"] and len(link_quality["out_value"]) > 0:
                 self.link_quality["_keys"].append(interface_name)
                 rows = link_quality["out_value"].split("\n")
                 for row in rows:
                     _row = row.strip()
                     if _row.startswith("Link Quality"):
                         data["link_quality"] = _row.split("=")[1].split(" ")[0].split("/")[0]   # x/70
```

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_agx_orin.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/jetson_agx_orin.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_agx_xavier.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/jetson_agx_xavier.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_nano_dev_kit.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/jetson_nano_dev_kit.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/jetson_xavier_dev_kit.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/jetson_xavier_dev_kit.py`

 * *Files identical despite different names*

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/models/ubuntu_64.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/models/ubuntu_64.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,10 +80,15 @@
         self.temperature_metrics = {}
         self.temperature_metrics["_keys"] = []
         for zone in thermal_zones["out_value"].split("\\n"):
             if len(zone) == 0:
                 continue
             self.temperature_metrics["_keys"].append(zone)
             temp = utils.run_command_and_get_output("cat /sys/class/thermal/" + zone + "/temp")
-            if temp["error"] == True:
+            if temp["error"] == True or len(temp["out_value"]) == 0:
                 self.temperature_metrics["error"] = True
-            self.temperature_metrics[zone] = temp["out_value"]
+                self.temperature_metrics[zone] = constants.ERROR_WHILE_READING_VALUE
+                continue
+            self.temperature_metrics[zone] = temp["out_value"]
+            
+            print("Temperature: " + str(self.temperature_metrics[zone]))
+            print("Temperature length: ", len(str(self.temperature_metrics[zone])))
```

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter/prometheus_exporter.py` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter/prometheus_exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import argparse
 from prometheus_client import start_http_server, Gauge, Info
-from energon_prometheus_exporter.drivers import driver
+from energon_prometheus_exporter.drivers import driver, constants
 # import actualMeter
 # example: sudo python3 prometheus_exporter.py 00:15:A3:00:55:02
 
 parser = argparse.ArgumentParser()
 
 parser.add_argument(
     "-p",
@@ -168,17 +168,17 @@
             # handle new network interface
             if not hasattr(self, "network_quality_{}_link_quality".format(network_interface_name)):
                 setattr(self, "network_quality_{}_link_quality".format(network_interface_name), Gauge("energon_network_quality_{}_link_quality_x_over_70/70".format(network_interface_name), "Network metrics {} - link_quality [x/70]".format(network_interface_name)))
             if not hasattr(self, "network_quality_{}_signal_level".format(network_interface_name)):
                 setattr(self, "network_quality_{}_signal_level".format(network_interface_name), Gauge("energon_network_quality_{}_signal_level_dBm".format(network_interface_name), "Network metrics {} - signal_level [dBm]".format(network_interface_name)))
             if not hasattr(self, "network_quality_{}_bit_rate".format(network_interface_name)):
                 setattr(self, "network_quality_{}_bit_rate".format(network_interface_name), Gauge("energon_network_quality_{}_bit_rate_Mbs".format(network_interface_name), "Network metrics {} - bit_rate [Mb/s]".format(network_interface_name)))
-            getattr(self, "network_quality_{}_link_quality".format(network_interface_name)).set(self.energon.instantiated_model.link_quality[network_interface_name]["link_quality"])
-            getattr(self, "network_quality_{}_signal_level".format(network_interface_name)).set(self.energon.instantiated_model.link_quality[network_interface_name]["signal_level"])
-            getattr(self, "network_quality_{}_bit_rate".format(network_interface_name)).set(self.energon.instantiated_model.link_quality[network_interface_name]["bit_rate"])
+            getattr(self, "network_quality_{}_link_quality".format(network_interface_name)).set(self.energon.instantiated_model.link_quality[network_interface_name]["link_quality"] if self.energon.instantiated_model.link_quality[network_interface_name]["link_quality"] != constants.ERROR_WHILE_READING_VALUE else -1)
+            getattr(self, "network_quality_{}_signal_level".format(network_interface_name)).set(self.energon.instantiated_model.link_quality[network_interface_name]["signal_level"] if self.energon.instantiated_model.link_quality[network_interface_name]["signal_level"] != constants.ERROR_WHILE_READING_VALUE else -1)
+            getattr(self, "network_quality_{}_bit_rate".format(network_interface_name)).set(self.energon.instantiated_model.link_quality[network_interface_name]["bit_rate"] if self.energon.instantiated_model.link_quality[network_interface_name]["bit_rate"] != constants.ERROR_WHILE_READING_VALUE else -1)
 
         # cpu frequency metrics
         for core in self.energon.instantiated_model.cpu_frequency_metrics["_keys"]:
             getattr(self, "cpu_{}_frequency".format(core)).set(self.energon.instantiated_model.cpu_frequency_metrics[core])
 
         # cpu usage metrics
         for core in self.energon.instantiated_model.cpu_usage_percentage["_keys"]:
@@ -205,14 +205,17 @@
         self.ram_percent_used.set(self.energon.instantiated_model.ram_metrics["usage_percentage"])
 
         # gpu metrics
         self.gpu_total_usage_percentage.set(self.energon.instantiated_model.gpu_usage_percentage)
 
         # temperature metrics
         for temp_metric in self.energon.instantiated_model.temperature_metrics["_keys"]:
+            if self.energon.instantiated_model.temperature_metrics[temp_metric] == constants.ERROR_WHILE_READING_VALUE:
+                getattr(self, "temperature_{}".format(temp_metric)).set(-1)
+                continue
             getattr(self, "temperature_{}".format(temp_metric)).set(self.energon.instantiated_model.temperature_metrics[temp_metric])
 
     def run(self):
         """Run the metrics server"""
         print("Starting energon prometheus server")
         start_http_server(self.app_port)
         print("Energon prometheus server running on port " + str(self.app_port))
```

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/PKG-INFO` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energon-prometheus-exporter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Energon is a Prometheus compliant system monitoring tools, it focuses on the energy consumption and resource usage in constrained devices but it integrates reporting tools for desktop machine, too.
 Author-email: Matteo Mendula <mattemendu@gmail.com>
 Project-URL: Homepage, https://github.com/MatteoMendula/Energon_Prometheus_exporter
 Project-URL: Bug Tracker, https://github.com/MatteoMendula/Energon_Prometheus_exporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `energon_prometheus_exporter-0.0.5/src/energon_prometheus_exporter.egg-info/SOURCES.txt` & `energon_prometheus_exporter-0.0.6/src/energon_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

