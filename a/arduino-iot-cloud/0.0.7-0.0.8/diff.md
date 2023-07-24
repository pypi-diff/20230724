# Comparing `tmp/arduino_iot_cloud-0.0.7.tar.gz` & `tmp/arduino_iot_cloud-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arduino_iot_cloud-0.0.7.tar", last modified: Thu Apr 27 11:04:59 2023, max compression
+gzip compressed data, was "arduino_iot_cloud-0.0.8.tar", last modified: Mon Jul 24 15:36:44 2023, max compression
```

## Comparing `arduino_iot_cloud-0.0.7.tar` & `arduino_iot_cloud-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.707756 arduino_iot_cloud-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/examples/micropython.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.707756 arduino_iot_cloud-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/ucloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/umqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/ussl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:44.261013 arduino_iot_cloud-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-24 15:36:44.261013 arduino_iot_cloud-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:44.257013 arduino_iot_cloud-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/examples/micropython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:36:44.261013 arduino_iot_cloud-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:44.257013 arduino_iot_cloud-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:44.261013 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 15:36:44.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/ucloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/umqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/ussl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:44.261013 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-24 15:36:44.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-24 15:36:44.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:36:44.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 15:36:44.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 15:36:44.000000 arduino_iot_cloud-0.0.8/src/arduino_iot_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:44.261013 arduino_iot_cloud-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/tests/ci.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1733 2023-07-24 15:36:29.000000 arduino_iot_cloud-0.0.8/tests/ci.sh
```

### Comparing `arduino_iot_cloud-0.0.7/LICENSE` & `arduino_iot_cloud-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.7/PKG-INFO` & `arduino_iot_cloud-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arduino_iot_cloud
-Version: 0.0.7
+Version: 0.0.8
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
@@ -48,16 +48,16 @@
 ```
 
 Your `secrets.py` file should look like this:
 
 ```python
 WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
 WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
-DEVICE_ID  = b"" # Provided by Arduino cloud when creating a device.
-SECRET_KEY = b"" # Provided by Arduino cloud when creating a device.
+DEVICE_ID  = "" # Provided by Arduino cloud when creating a device.
+SECRET_KEY = "" # Provided by Arduino cloud when creating a device.
 ```
 
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
```

### Comparing `arduino_iot_cloud-0.0.7/README.md` & `arduino_iot_cloud-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 ```
 
 Your `secrets.py` file should look like this:
 
 ```python
 WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
 WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
-DEVICE_ID  = b"" # Provided by Arduino cloud when creating a device.
-SECRET_KEY = b"" # Provided by Arduino cloud when creating a device.
+DEVICE_ID  = "" # Provided by Arduino cloud when creating a device.
+SECRET_KEY = "" # Provided by Arduino cloud when creating a device.
 ```
 
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
```

### Comparing `arduino_iot_cloud-0.0.7/examples/example.py` & `arduino_iot_cloud-0.0.8/examples/example.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.7/examples/micropython.py` & `arduino_iot_cloud-0.0.8/examples/micropython.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.7/package.json` & `arduino_iot_cloud-0.0.8/package.json`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.7/pyproject.toml` & `arduino_iot_cloud-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/__init__.py` & `arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/ucloud.py` & `arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/ucloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,19 @@
 
 import time
 import logging
 from senml import SenmlPack
 from senml import SenmlRecord
 from arduino_iot_cloud.umqtt import MQTTClient
 
+import asyncio
+from asyncio import CancelledError
 try:
-    import asyncio
-    from asyncio import CancelledError
     from asyncio import InvalidStateError
-except ImportError:
-    import uasyncio as asyncio
-    from uasyncio.core import CancelledError
-
+except (ImportError, AttributeError):
     # MicroPython doesn't have this exception
     class InvalidStateError(Exception):
         pass
 
 # Server/port for basic auth.
 _DEFAULT_SERVER = "iot.arduino.cc"
 
@@ -171,18 +168,27 @@
             ntp_timeout=3
     ):
         self.tasks = {}
         self.records = {}
         self.thing_id = None
         self.keepalive = keepalive
         self.last_ping = timestamp()
-        self.device_topic = b"/a/d/" + device_id + b"/e/i"
         self.senmlpack = SenmlPack("", self.senml_generic_callback)
         self.started = False
 
+        # Convert args to bytes if they are passed as strings.
+        if isinstance(device_id, str):
+            device_id = bytes(device_id, "utf-8")
+        if username is not None and isinstance(username, str):
+            username = bytes(username, "utf-8")
+        if password is not None and isinstance(password, str):
+            password = bytes(password, "utf-8")
+
+        self.device_topic = b"/a/d/" + device_id + b"/e/i"
+
         # Update RTC from NTP server on MicroPython.
         self.update_systime(ntp_server, ntp_timeout)
 
         # MicroPython does not support secure elements yet, and key/cert
         # must be loaded from DER files and passed as binary blobs.
         if "keyfile" in ssl_params and "der" in ssl_params["keyfile"]:
             with open(ssl_params.pop("keyfile"), "rb") as f:
@@ -370,15 +376,15 @@
             for name in list(self.tasks):
                 task = self.tasks[name]
                 try:
                     if task.done():
                         self.tasks.pop(name)
                         self.records.pop(name, None)
                         if isinstance(task_except, DoneException):
-                            logging.error(f"task: {name} complete.")
+                            logging.info(f"task: {name} complete.")
                         elif task_except is not None:
                             logging.error(f"task: {name} raised exception: {str(task_except)}.")
                         if name == "mqtt_task":
                             self.create_task("conn_task", self.conn_task)
                         break   # Break after the first task is removed.
                 except (CancelledError, InvalidStateError):
                     pass
```

### Comparing `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/umqtt.py` & `arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/umqtt.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/ussl.py` & `arduino_iot_cloud-0.0.8/src/arduino_iot_cloud/ussl.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/PKG-INFO` & `arduino_iot_cloud-0.0.8/src/arduino_iot_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arduino-iot-cloud
-Version: 0.0.7
+Version: 0.0.8
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
@@ -48,16 +48,16 @@
 ```
 
 Your `secrets.py` file should look like this:
 
 ```python
 WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
 WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
-DEVICE_ID  = b"" # Provided by Arduino cloud when creating a device.
-SECRET_KEY = b"" # Provided by Arduino cloud when creating a device.
+DEVICE_ID  = "" # Provided by Arduino cloud when creating a device.
+SECRET_KEY = "" # Provided by Arduino cloud when creating a device.
 ```
 
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
```

