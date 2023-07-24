# Comparing `tmp/pymodaq_plugins_stellarnet-1.0.2.tar.gz` & `tmp/pymodaq_plugins_stellarnet-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_stellarnet-1.0.2.tar", last modified: Mon Mar 28 12:12:28 2022, max compression
+gzip compressed data, was "pymodaq_plugins_stellarnet-2.0.1.tar", last modified: Mon Jul 24 10:10:36 2023, max compression
```

## Comparing `pymodaq_plugins_stellarnet-1.0.2.tar` & `pymodaq_plugins_stellarnet-2.0.1.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    21395 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2510 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.118114 pymodaq_plugins_stellarnet-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.118114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_move_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11141 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Stellarnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/hardware/
--rw-r--r--   0 runner    (1001) docker     (121)    41586 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/hardware/MyCaL-C20111832-VIS-IC2.CAL
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11842 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/hardware/stellarnet.hex
--rw-r--r--   0 runner    (1001) docker     (121)    23608 2022-03-28 12:12:15.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/hardware/stellarnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 12:12:28.122114 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-03-28 12:12:27.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-03-28 12:12:27.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-28 12:12:27.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-28 12:12:27.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-03-28 12:12:27.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-28 12:12:27.000000 pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.362010 pymodaq_plugins_stellarnet-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-24 10:10:36.362010 pymodaq_plugins_stellarnet-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:10:36.362010 pymodaq_plugins_stellarnet-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_move_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Stellarnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.362010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/hardware/MyCaL-C20111832-VIS-IC2.CAL
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/hardware/stellarnet.hex
+-rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/hardware/stellarnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.362010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 10:10:22.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:10:36.358010 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-24 10:10:36.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-24 10:10:36.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:10:36.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-24 10:10:36.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 10:10:36.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 10:10:36.000000 pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_stellarnet-1.0.2/PKG-INFO` & `pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
-Name: pymodaq_plugins_stellarnet
-Version: 1.0.2
+Name: pymodaq-plugins-stellarnet
+Version: 2.0.1
 Summary: Plugin for StellarNet spectrometers
 Home-page: https://github.com/Attolab/pymodaq_plugins_stellarnet
 Author: Romain Géneaux
 Author-email: romain.geneaux@cea.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 License-File: LICENSE
 
 pymodaq_plugins_stellarnet (StellarNet)
 #######################################
@@ -70,9 +69,7 @@
 
 Installation notes
 ++++++++++++++++++
 **!! Warning !!** The plugin uses pyusb version 1.0.0b1 or earlier - haven't tested for later versions.
 On windows, the installation of appropriate drivers working with pyusb can be fidly. I had most success using Zadig (https://zadig.akeo.ie/) to update the spectrometer drivers. Sadly if you change the drivers to work with python, the software provided by StellarNet will not work anymore. Hopefully the PyMoDAQ plugin works well enough so that you won't need the constructor software anymore :-)
 
 Tested on Windows 10 with the driver WinUSB (v6.1.7600.16385).
-
-
```

### Comparing `pymodaq_plugins_stellarnet-1.0.2/README.rst` & `pymodaq_plugins_stellarnet-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Stellarnet.py` & `pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Stellarnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import numpy as np
 from easydict import EasyDict as edict
-from pymodaq.daq_utils.daq_utils import (
+from pymodaq.utils.daq_utils import (
     ThreadCommand,
     getLineInfo,
-    DataFromPlugins,
-    Axis,
 )
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base, comon_parameters
+from pymodaq.utils.data import Axis, DataFromPlugins, DataToExport
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters
 from PyQt5 import QtWidgets
 import usb
 from ...hardware import stellarnet as sn
-from scipy.ndimage.filters import uniform_filter1d
+from scipy.ndimage import uniform_filter1d
 import os, glob
 
 
 class DAQ_1DViewer_Stellarnet(DAQ_Viewer_base):
     """
     """
 
@@ -128,15 +127,15 @@
                 self.calib_on = False
 
         elif param.name() == "cal_path":
             self.do_irradiance_calibration()
 
         elif param.name() == "take_snap":
             try:
-                self.snapshot = self.parent.datas[0]['data'][0]   # Get currently displayed data
+                self.snapshot = self.parent.datas[0]['data'][0]  # Get currently displayed data
                 self.settings.child("take_snap").setValue(False)
 
             except Exception as e:
                 self.emit_status(
                     ThreadCommand("Update_Status", [getLineInfo() + str(e), "log"])
                 )
                 self.status.info = getLineInfo() + str(e)
@@ -206,36 +205,33 @@
                     self.controller,
                     "window_width",
                     self.settings.child("x_smooth").value(),
                 )
 
             # get the x_axis (you may want to to this also in the commit settings if x_axis may have changed
             data_x_axis = self.get_wl_axis()
-            self.x_axis = [Axis(data=data_x_axis, label="Wavelength", units="m")]
-            self.emit_x_axis()
+            self.x_axis = Axis(data=data_x_axis, label="Wavelength", units="m")
+            self.x_axis.index = 0
 
             # initialize viewers pannel with the future type of data
             name = usb.util.get_string(
                 self.controller._device, 100, self.controller._device.iProduct
             )
             data_init = [
-                (
-                    DataFromPlugins(
-                        name=name,
-                        dim="Data1D",
-                        data=[np.asarray(self.controller.read_spectrum())],
-                        x_axis=Axis(data=data_x_axis, label="Wavelength", units="m"),
-                    )
+                DataFromPlugins(
+                    name=name,
+                    dim="Data1D",
+                    data=[np.asarray(self.controller.read_spectrum())],
+                    axes=[self.x_axis],
                 )
             ]
             QtWidgets.QApplication.processEvents()
-            self.data_grabed_signal_temp.emit(data_init)
-            self.data_grabed_signal_temp.emit(
-                data_init
-            )  # works the second time for some reason
+            self.dte_signal_temp.emit(DataToExport('Stellarnet', data=data_init))
+            self.dte_signal_temp.emit(DataToExport('Stellarnet', data=data_init))
+            # works the second time for some reason
 
             try:
                 self.do_irradiance_calibration()
             except Exception as e:
                 self.emit_status(
                     ThreadCommand("Update_Status", [getLineInfo() + str(e), "log"])
                 )
@@ -262,15 +258,14 @@
 
     def get_data(self):
         data = np.asarray(self.moving_average(self.controller.read_spectrum()))
         if self.calib_on and self.calib_file_ok:
             data = data * self.calibration
         return data
 
-
     def do_irradiance_calibration(self):
         calibration = []
         try:
             with open(self.settings.child("cal_path").value(), "r") as file:
                 for line in file:
                     if line[0].isdigit():
                         calibration.append(np.fromstring(line, sep=" "))
@@ -328,14 +323,15 @@
 
         data_tot = [self.get_data()]
 
         if self.snapshot is not None:
             data_tot.append(self.snapshot)
             label.append("Snapshot")
 
-        self.data_grabed_signal.emit(
-            [
-                DataFromPlugins(
-                    name="StellarNet", data=data_tot, dim="Data1D", labels=label, x_axis=self.x_axis[0]
-                )
-            ]
-        )
+        self.dte_signal.emit(DataToExport('Stellarnet',
+                                          data=[DataFromPlugins(
+                                              name="StellarNet", data=data_tot, dim="Data1D", labels=label,
+                                              axes=[self.x_axis])]))
+
+    def stop(self):
+        self.emit_status(ThreadCommand('Update_Status', ['Stopping Acquisition']))
+        return ''
```

### Comparing `pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/hardware/MyCaL-C20111832-VIS-IC2.CAL` & `pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/hardware/MyCaL-C20111832-VIS-IC2.CAL`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/hardware/stellarnet.hex` & `pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/hardware/stellarnet.hex`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet/hardware/stellarnet.py` & `pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet/hardware/stellarnet.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/PKG-INFO` & `pymodaq_plugins_stellarnet-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
-Name: pymodaq-plugins-stellarnet
-Version: 1.0.2
+Name: pymodaq_plugins_stellarnet
+Version: 2.0.1
 Summary: Plugin for StellarNet spectrometers
 Home-page: https://github.com/Attolab/pymodaq_plugins_stellarnet
 Author: Romain Géneaux
 Author-email: romain.geneaux@cea.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 License-File: LICENSE
 
 pymodaq_plugins_stellarnet (StellarNet)
 #######################################
@@ -70,9 +69,7 @@
 
 Installation notes
 ++++++++++++++++++
 **!! Warning !!** The plugin uses pyusb version 1.0.0b1 or earlier - haven't tested for later versions.
 On windows, the installation of appropriate drivers working with pyusb can be fidly. I had most success using Zadig (https://zadig.akeo.ie/) to update the spectrometer drivers. Sadly if you change the drivers to work with python, the software provided by StellarNet will not work anymore. Hopefully the PyMoDAQ plugin works well enough so that you won't need the constructor software anymore :-)
 
 Tested on Windows 10 with the driver WinUSB (v6.1.7600.16385).
-
-
```

### Comparing `pymodaq_plugins_stellarnet-1.0.2/src/pymodaq_plugins_stellarnet.egg-info/SOURCES.txt` & `pymodaq_plugins_stellarnet-2.0.1/src/pymodaq_plugins_stellarnet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,13 @@
 src/pymodaq_plugins_stellarnet/daq_move_plugins/__init__.py
 src/pymodaq_plugins_stellarnet/daq_viewer_plugins/__init__.py
 src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_0D/__init__.py
 src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/__init__.py
 src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Stellarnet.py
 src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_2D/__init__.py
 src/pymodaq_plugins_stellarnet/daq_viewer_plugins/plugins_ND/__init__.py
+src/pymodaq_plugins_stellarnet/extension/__init__.py
 src/pymodaq_plugins_stellarnet/hardware/MyCaL-C20111832-VIS-IC2.CAL
 src/pymodaq_plugins_stellarnet/hardware/__init__.py
 src/pymodaq_plugins_stellarnet/hardware/stellarnet.hex
-src/pymodaq_plugins_stellarnet/hardware/stellarnet.py
+src/pymodaq_plugins_stellarnet/hardware/stellarnet.py
+src/pymodaq_plugins_stellarnet/models/__init__.py
```

