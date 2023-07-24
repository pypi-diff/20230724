# Comparing `tmp/pymodaq_plugins_greateyes-1.0.0.tar.gz` & `tmp/pymodaq_plugins_greateyes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_greateyes-1.0.0.tar", last modified: Fri Jan 20 12:48:04 2023, max compression
+gzip compressed data, was "pymodaq_plugins_greateyes-1.0.1.tar", last modified: Mon Jul 24 06:47:36 2023, max compression
```

## Comparing `pymodaq_plugins_greateyes-1.0.0.tar` & `pymodaq_plugins_greateyes-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:48:04.079476 pymodaq_plugins_greateyes-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-01-20 12:48:04.079476 pymodaq_plugins_greateyes-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 12:48:04.079476 pymodaq_plugins_greateyes-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:48:04.075476 pymodaq_plugins_greateyes-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:48:04.075476 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:48:04.079476 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:48:04.079476 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33901 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/daq_2Dviewer_GreateyesCCD.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:48:04.079476 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 12:47:54.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:48:04.079476 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-01-20 12:48:04.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-20 12:48:04.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:48:04.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-20 12:48:04.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-20 12:48:04.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-20 12:48:04.000000 pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.562384 pymodaq_plugins_greateyes-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.562384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_move_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32624 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/daq_2Dviewer_GreateyesCCD.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.566384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 06:47:25.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:47:36.562384 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-24 06:47:36.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-24 06:47:36.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:47:36.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 06:47:36.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 06:47:36.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 06:47:36.000000 pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_greateyes-1.0.0/LICENSE` & `pymodaq_plugins_greateyes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_greateyes-1.0.0/PKG-INFO` & `pymodaq_plugins_greateyes-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_greateyes
-Version: 1.0.0
+Version: 1.0.1
 Summary: some word about your plugin
 Home-page: https://github.com/Attolab/pymodaq_plugins_greateyes
 Author: PyMoDAQ plugin for instruments from Greateyes (ALEX, ELSE, GE XXXX)
 Author-email: romain.geneaux@cea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_greateyes-1.0.0/README.rst` & `pymodaq_plugins_greateyes-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_greateyes-1.0.0/setup.py` & `pymodaq_plugins_greateyes-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/daq_2Dviewer_GreateyesCCD.py` & `pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/daq_2Dviewer_GreateyesCCD.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import numpy as np
 import time
 import sys, os
 from easydict import EasyDict as edict
 from PyQt5 import QtWidgets, QtCore
-from pymodaq.daq_utils.daq_utils import (
+from pymodaq.utils.daq_utils import (
     ThreadCommand,
     getLineInfo,
-    DataFromPlugins,
-    Axis,
 )
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base, comon_parameters
-from pymodaq.daq_utils.parameter.utils import iter_children
+from pymodaq.utils.data import Axis, DataFromPlugins, DataToExport
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters
+from pymodaq.utils.parameter.utils import iter_children
 
 # Import GreatEyes SDK: In the hardware folder must be placed greateyesSDK.py, greateyes.dll, geCommLib.dll
 HARDWARE_DIR = os.path.abspath(
     os.path.join(os.path.dirname(__file__), "..", "..", "hardware")
 )
 sys.path.append(HARDWARE_DIR)
 os.add_dll_directory(HARDWARE_DIR)
@@ -33,15 +32,15 @@
             "type": "group",
             "expanded": True,
             "children": [
                 {
                     "title": "Connection type",
                     "name": "connection_type",
                     "type": "list",
-                    "values": ["Ethernet", "USB"],
+                    "limits": ["Ethernet", "USB"],
                     "readonly": False,
                 },
                 {
                     "title": "Camera status",
                     "name": "camera_status",
                     "type": "str",
                     "value": "Not initialized",
@@ -279,14 +278,15 @@
     ]
 
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state)
 
         self.x_axis = None
         self.y_axis = None
+        self.axes = None
         self.data_shape = None
         self.controller = None
         self.callback_thread = None
 
     def ini_detector(self, controller=None):
         """Detector communication initialization
 
@@ -309,62 +309,34 @@
                 y_axis=None,
                 controller=None,
             )
         )
 
         try:
             # Start initializing
-            self.emit_status(
-                ThreadCommand("show_splash", ["Initializing Greateyes CCD Camera"])
-            )
-
             if self.settings.child(("controller_status")).value() == "Slave":
                 if controller is None:
                     raise Exception(
                         "no controller has been defined externally while this detector is a slave one"
                     )
                 else:
                     self.controller = controller
             else:
                 self.controller = ge
 
             self.update_status()
             self.ini_greateyes_camera()
 
-            self.x_axis = self.get_xaxis()
-            self.y_axis = self.get_yaxis()
+            self.get_xaxis()
+            self.get_yaxis()
             self.status.x_axis = self.x_axis
             self.status.y_axis = self.y_axis
 
             # initialize viewers pannel with the future type of data
-            # we perform a blocking measurement for simplicity here.
-
-            self.emit_status(ThreadCommand("show_splash", ["Taking one image"]))
-
-            self.data_grabed_signal_temp.emit(
-                [
-                    DataFromPlugins(
-                        name="CCD Image",
-                        data=[
-                            self.controller.PerformMeasurement_Blocking_DynBitDepth(
-                                correctBias=self.settings.child(
-                                    "acquisition_settings", "do_correct_bias"
-                                ).value()
-                            ).astype(np.float)
-                        ],
-                        dim="Data2D",
-                        labels=["dat0"],
-                        x_axis=self.y_axis,
-                        y_axis=self.x_axis,
-                    ),
-                ]
-            )
-            self.settings.child(
-                "acquisition_settings", "timing_settings", "last_meas_time"
-            ).setValue("{:.1f}".format(self.controller.GetLastMeasTimeNeeded() * 1000))
+            self.prepare_data()
 
             self.status.info = "Camera initialized correctly"
             self.status.initialized = True
             self.status.controller = self.controller
             self.emit_status(ThreadCommand("close_splash"))
             return self.status
 
@@ -390,28 +362,24 @@
         # USB
         if self.settings.child("camera_settings", "connection_type").value() == "USB":
             connectionSetupWorked = ge.SetupCameraInterface(
                 self.controller.connectionType_USB
             )
         # or Ethernet (needs connection to camera server)
         elif (
-            self.settings.child("camera_settings", "connection_type").value()
-            == "Ethernet"
+                self.settings.child("camera_settings", "connection_type").value()
+                == "Ethernet"
         ):
             connectionSetupWorked = ge.SetupCameraInterface(
                 self.controller.connectionType_Ethernet,
                 ipAddress=self.settings.child("camera_settings", "camera_IP").value(),
             )
             if connectionSetupWorked:
                 connectionSetupWorked = self.controller.ConnectToSingleCameraServer()
-                if connectionSetupWorked:
-                    self.emit_status(
-                        ThreadCommand("show_splash", ["Connected to Camera Server"])
-                    )
-                else:
+                if not connectionSetupWorked:
                     raise Exception("Could not connect to camera")
         else:
             connectionSetupWorked = False
             raise ValueError("Unsupported connection type")
 
         if not connectionSetupWorked:
             raise Exception("Could not connect to camera")
@@ -443,69 +411,61 @@
         if CameraConnected:
             self.settings.child("camera_settings", "camera_model_id").setValue(
                 CameraModel[0]
             )
             self.settings.child("camera_settings", "camera_model_str").setValue(
                 CameraModel[1]
             )
-            self.emit_status(
-                ThreadCommand("show_splash", ["Connected to Camera " + CameraModel[1]])
-            )
 
-            if self.controller.InitCamera(addr=addr):
-                self.emit_status(ThreadCommand("show_splash", ["Camera Initialized"]))
-            else:
+            if not self.controller.InitCamera(addr=addr):
                 self.controller.DisconnectCamera()
                 raise Exception(
                     "Could not connect to camera; " + self.controller.StatusMSG
                 )
 
         else:
             self.controller.DisconnectCamera()
             if (
-                self.settings.child("camera_settings", "connection_type").value()
-                == "Ethernet"
+                    self.settings.child("camera_settings", "connection_type").value()
+                    == "Ethernet"
             ):
                 self.controller.DisconnectCameraServer()
             raise Exception("Could not connect to camera; " + self.controller.StatusMSG)
 
         self.update_status()
 
         # Get Functions
         # =================================================
-        self.emit_status(
-            ThreadCommand("show_splash", ["Obtaining Camera parameters..."])
-        )
         self.settings.child("camera_settings", "firmware_version").setValue(
             self.controller.GetFirmwareVersion()
         )
         self.settings.child(
             "acquisition_settings", "timing_settings", "exposure_time"
         ).setLimits((1, self.controller.GetMaxExposureTime()))
 
         if not self.controller.SupportedSensorFeature(0):  # Supports Capacity Mode?
             self.settings.child("acquisition_settings", "capacity_mode").hide()
 
         if self.controller.SupportedSensorFeature(
-            1
+                1
         ):  # Checks if Horizontal Binning is supported
             self.settings.child(
                 "acquisition_settings", "image_settings", "bin_x"
             ).setLimits((1, self.controller.GetMaxBinningX()))
         else:
             self.settings.child(
                 "acquisition_settings", "image_settings", "bin_x"
             ).hide()
 
         self.settings.child(
             "acquisition_settings", "image_settings", "bin_y"
         ).setLimits((1, self.controller.GetMaxBinningY()))
 
         if not self.controller.SupportedSensorFeature(
-            2
+                2
         ):  # Checks if Horizontal Cropping is supported
             self.settings.child(
                 "acquisition_settings", "image_settings", "crop_x"
             ).hide()
 
         # GetNumberOfSensorOutputModes()
         # GetSensorOutputModeStrings() features not implemented yet.
@@ -514,20 +474,20 @@
         speeds = [50, 100, 250, 500, 1, 3]
         speedUnits = ["kHz", "kHz", "kHz", "kHz", "MHz", "MHz"]
 
         availableSpeeds = []
         for index, speed in enumerate(speeds):
             # try to set camera to the readout speed
             if self.controller.SetReadOutSpeed(
-                eval(
-                    "self.controller.readoutSpeed_"
-                    + str(speed)
-                    + "_"
-                    + speedUnits[index]
-                )
+                    eval(
+                        "self.controller.readoutSpeed_"
+                        + str(speed)
+                        + "_"
+                        + speedUnits[index]
+                    )
             ):
                 availableSpeeds.append(str(speed) + " " + speedUnits[index])
         self.settings.child(
             "acquisition_settings", "timing_settings", "readout_speed"
         ).setLimits(availableSpeeds)
         # by default set camera to the fastest readout speed
         self.settings.child(
@@ -569,15 +529,15 @@
             self.controller.TemperatureControl_SwitchOff()
 
         self.timerTemp = self.startTimer(3000)  # Timer event fired every 3 seconds
         if not self.settings.child("temperature_settings", "check_temperature").value():
             self.killTimer(self.timerTemp)
 
         self.update_image()
-        
+
         # Set up callback
         callback = GreateyesCallback(self.controller.DllIsBusy)
         callback.exposure = self.settings.child(
             "acquisition_settings", "timing_settings", "exposure_time"
         ).value()
         callback.timeout = self.settings.child(
             "acquisition_settings", "timing_settings", "timeout"
@@ -627,35 +587,35 @@
         elif param.name() == "timeout":
             # Update callback
             self.callback_thread.callback.timeout = param.value()
 
         elif param.name() == "readout_speed":
             speed, unit = param.value().split()
             if not self.controller.SetReadOutSpeed(
-                eval("self.controller.readoutSpeed_" + speed + "_" + unit)
+                    eval("self.controller.readoutSpeed_" + speed + "_" + unit)
             ):
                 self.emit_status(
                     ThreadCommand(
                         "Update_Status", ["Could not update readout speed", "log"]
                     )
                 )
 
         elif param.name() in iter_children(
-            self.settings.child("acquisition_settings", "image_settings")
+                self.settings.child("acquisition_settings", "image_settings")
         ):
             self.update_image()
 
         elif param.name() == "set_point":
             if self.settings.child("temperature_settings", "do_temperature").value():
                 self.controller.TemperatureControl_SetTemperature(param.value())
 
         elif param.name() == "do_temperature":
             if param.value():
                 self.controller.TemperatureControl_Init()
-                self.controller.TemperatureControl_SetTemperature(param.value())
+                self.controller.TemperatureControl_SetTemperature(self.settings['temperature_settings', 'set_point'])
             else:
                 self.controller.TemperatureControl_SwitchOff()
 
         elif param.name() == "check_temperature":
             if param.value():
                 self.timerTemp = self.startTimer(3000)
             else:
@@ -682,19 +642,16 @@
         Returns
         -------
         1D numpy array
             Contains a vector of integer corresponding to the horizontal camera pixels.
         """
         if self.controller is not None:
             Nx = self.settings.child("acquisition_settings", "N_x").value()
-            self.x_axis = Axis(
-                data=np.linspace(0, Nx - 1, Nx, dtype=int), label="Pixels"
-            )
-
-            self.emit_x_axis()
+            xaxis = np.linspace(0, Nx, Nx, endpoint=False)
+            self.x_axis = Axis(data=xaxis, label='Pixels', index=1)
         else:
             raise (Exception("Controller not defined"))
         return self.x_axis
 
     def get_yaxis(self):
         """
         Obtain the vertical axis of the image.
@@ -703,18 +660,16 @@
         -------
         1D numpy array
             Contains a vector of integer corresponding to the vertical camera pixels.
         """
         if self.controller is not None:
 
             Ny = self.settings.child("acquisition_settings", "N_y").value()
-            self.y_axis = Axis(
-                data=np.linspace(0, Ny - 1, Ny, dtype=int), label="Pixels"
-            )
-            self.emit_y_axis()
+            yaxis = np.linspace(0, Ny, Ny, endpoint=False)
+            self.y_axis = Axis(data=yaxis, label='Pixels', index=0)
         else:
             raise (Exception("Controller not defined"))
         return self.y_axis
 
     def update_image(self):
         self.controller.SetupCropMode2D(
             self.settings.child(
@@ -754,16 +709,16 @@
 
     def close(self):
         """
         Terminate the communication protocol
         """
         if self.controller.DisconnectCamera():
             if (
-                self.settings.child("camera_settings", "connection_type").value()
-                == "Ethernet"
+                    self.settings.child("camera_settings", "connection_type").value()
+                    == "Ethernet"
             ):
                 if ge.DisconnectCameraServer():
                     msg = "Successfully disconnected Camera Server and Camera"
                 else:
                     msg = "Error while disconnecting Camera Server"
             else:
                 msg = "Successfully disconnected USB Camera"
@@ -794,33 +749,38 @@
             self.callback_signal.emit()  # will trigger the wait for acquisition
 
         except Exception as e:
             self.emit_status(ThreadCommand("Update_Status", [str(e), "log"]))
 
         ## remember to check measurement time if parameter is ticked
 
-    def prepare_data(self):
+    def prepare_data(self, show = False):
         width, height, bytesPerPixel = self.controller.GetImageSize()
+        self.get_xaxis()
         # GetMeasurement function allocates memory by itself, no need to do it
 
         # Switches viewer type depending on image size
-        data_shape = "Data2D" if height != 1 else "Data1D"
+        if height != 1:
+            data_shape = "Data2D"
+            self.get_yaxis()
+            axes = [self.x_axis, self.y_axis]
+        else:
+            data_shape = "Data1D"
+            self.x_axis.index = 0
+            axes = [self.x_axis]
+
         if data_shape != self.data_shape:
             self.data_shape = data_shape
+            self.axes = axes
             # init the viewers
-            self.data_grabed_signal_temp.emit(
-                [
-                    DataFromPlugins(
-                        name="Camera ",
-                        data=[np.squeeze(np.zeros((height, width)).astype(np.float))],
-                        dim=self.data_shape,
-                        labels="Camera",
-                    )
-                ]
-            )
+            self.dte_signal_temp.emit(DataToExport('Greateyes',
+                                                   data=[DataFromPlugins(name='CCD Image', data=[
+                                                       np.squeeze(np.zeros((height, width)).astype(float))],
+                                                                         dim=self.data_shape, labels=['Camera'],
+                                                                         axes=self.axes), ]))
 
     def emit_data(self):
         """
         Fonction used to emit data obtained by callback.
         See Also
         --------
         daq_utils.ThreadCommand
@@ -831,32 +791,27 @@
                     ThreadCommand("Update_Status", ["Measurement timed out", "log"])
                 )
 
             else:
                 size_y = self.settings.child("acquisition_settings", "N_y").value()
                 size_x = self.settings.child("acquisition_settings", "N_x").value()
                 data = self.controller.GetMeasurementData_DynBitDepth()
-                self.data_grabed_signal.emit(
-                    [
-                        DataFromPlugins(
-                            name="Camera",
-                            data=[np.squeeze(data.reshape(size_y, size_x)).astype(np.float)],
-                            dim=self.data_shape,
-                            labels="Camera",
-                        )
-                    ]
-                )
+                self.dte_signal.emit(DataToExport('Greateyes',
+                                                  data=[DataFromPlugins(name='CCD Image', data=[
+                                                      np.squeeze(data.reshape(size_y, size_x)).astype(float)],
+                                                                        dim=self.data_shape, axes=self.axes), ]))
+
                 self.settings.child("camera_settings", "camera_status").setValue(
                     "Data received"
                 )
 
                 QtWidgets.QApplication.processEvents()  # here to be sure the timeevents are executed even if in continuous grab mode
 
                 if self.settings.child(
-                    "acquisition_settings", "timing_settings", "check_meas_time"
+                        "acquisition_settings", "timing_settings", "check_meas_time"
                 ):
                     self.settings.child(
                         "acquisition_settings", "timing_settings", "last_meas_time"
                     ).setValue(
                         "{:.1f}".format(self.controller.GetLastMeasTimeNeeded() * 1000)
                     )
         except Exception as e:
@@ -871,28 +826,28 @@
     """
     Callback to wait for acquisitions to finish
     """
 
     data_sig = QtCore.pyqtSignal()
 
     def __init__(
-        self,
-        wait_fn,
+            self,
+            wait_fn,
     ):
         super(GreateyesCallback, self).__init__()
         self.wait_fn = wait_fn
         self.timedout = False
         self.exposure = 0
         self.timeout = 0
 
     def wait_for_acquisition(self):
         t_meas = 0
         dt = 5  # refresh rate in ms
         t_crit = (
-            self.exposure + self.timeout
+                self.exposure + self.timeout
         )  # time after which we cancel the measurement
 
         while self.wait_fn():  # DLL is busy
             time.sleep(dt / 1000)
             t_meas = t_meas + dt
             if t_meas >= t_crit:  # if measurement takes took long
                 if ge.StopMeasurement():
@@ -906,27 +861,27 @@
     this method start a DAQ_Viewer object with this defined plugin as detector
     Returns
     -------
 
     """
     import sys
     from PyQt5 import QtWidgets
-    from pymodaq.daq_utils.gui_utils import DockArea
-    from pymodaq.daq_viewer.daq_viewer_main import DAQ_Viewer
+    from pymodaq.utils.gui_utils import DockArea
+    from pymodaq.control_modules.daq_viewer import DAQ_Viewer
     from pathlib import Path
 
     app = QtWidgets.QApplication(sys.argv)
     win = QtWidgets.QMainWindow()
     area = DockArea()
     win.setCentralWidget(area)
     win.resize(1000, 500)
     win.setWindowTitle("PyMoDAQ Viewer")
     detector = Path(__file__).stem[13:]
     det_type = f"DAQ{Path(__file__).stem[4:6].upper()}"
-    prog = DAQ_Viewer(area, title="Testing", DAQ_type=det_type)
+    prog = DAQ_Viewer(area, title="Testing")
     win.show()
     prog.detector = detector
     prog.init_det()
 
     sys.exit(app.exec_())
```

### Comparing `pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/PKG-INFO` & `pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-greateyes
-Version: 1.0.0
+Version: 1.0.1
 Summary: some word about your plugin
 Home-page: https://github.com/Attolab/pymodaq_plugins_greateyes
 Author: PyMoDAQ plugin for instruments from Greateyes (ALEX, ELSE, GE XXXX)
 Author-email: romain.geneaux@cea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_greateyes-1.0.0/src/pymodaq_plugins_greateyes.egg-info/SOURCES.txt` & `pymodaq_plugins_greateyes-1.0.1/src/pymodaq_plugins_greateyes.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,11 +6,17 @@
 src/pymodaq_plugins_greateyes/__init__.py
 src/pymodaq_plugins_greateyes.egg-info/PKG-INFO
 src/pymodaq_plugins_greateyes.egg-info/SOURCES.txt
 src/pymodaq_plugins_greateyes.egg-info/dependency_links.txt
 src/pymodaq_plugins_greateyes.egg-info/entry_points.txt
 src/pymodaq_plugins_greateyes.egg-info/requires.txt
 src/pymodaq_plugins_greateyes.egg-info/top_level.txt
+src/pymodaq_plugins_greateyes/daq_move_plugins/__init__.py
 src/pymodaq_plugins_greateyes/daq_viewer_plugins/__init__.py
+src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_0D/__init__.py
+src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_1D/__init__.py
 src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/__init__.py
 src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_2D/daq_2Dviewer_GreateyesCCD.py
-src/pymodaq_plugins_greateyes/hardware/__init__.py
+src/pymodaq_plugins_greateyes/daq_viewer_plugins/plugins_ND/__init__.py
+src/pymodaq_plugins_greateyes/extension/__init__.py
+src/pymodaq_plugins_greateyes/hardware/__init__.py
+src/pymodaq_plugins_greateyes/models/__init__.py
```

