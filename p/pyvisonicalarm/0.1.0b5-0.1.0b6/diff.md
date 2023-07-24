# Comparing `tmp/pyvisonicalarm-0.1.0b5.tar.gz` & `tmp/pyvisonicalarm-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisonicalarm-0.1.0b5.tar", last modified: Mon Jul 24 12:08:07 2023, max compression
+gzip compressed data, was "pyvisonicalarm-0.1.0b6.tar", last modified: Mon Jul 24 16:31:27 2023, max compression
```

## Comparing `pyvisonicalarm-0.1.0b5.tar` & `pyvisonicalarm-0.1.0b6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/pyvisonicalarm/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    20717 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/device_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:31:27.264212 pyvisonicalarm-0.1.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-24 16:31:27.264212 pyvisonicalarm-0.1.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:31:27.260212 pyvisonicalarm-0.1.0b6/pyvisonicalarm/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20717 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm/device_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:31:27.264212 pyvisonicalarm-0.1.0b6/pyvisonicalarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-24 16:31:27.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 16:31:27.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:31:27.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 16:31:27.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 16:31:27.000000 pyvisonicalarm-0.1.0b6/pyvisonicalarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:31:27.264212 pyvisonicalarm-0.1.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 16:31:15.000000 pyvisonicalarm-0.1.0b6/setup.py
```

### Comparing `pyvisonicalarm-0.1.0b5/LICENSE` & `pyvisonicalarm-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b5/PKG-INFO` & `pyvisonicalarm-0.1.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b5/README.md` & `pyvisonicalarm-0.1.0b6/README.md`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b5/pyvisonicalarm/alarm.py` & `pyvisonicalarm-0.1.0b6/pyvisonicalarm/alarm.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b5/pyvisonicalarm/classes.py` & `pyvisonicalarm-0.1.0b6/pyvisonicalarm/classes.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b5/pyvisonicalarm/const.py` & `pyvisonicalarm-0.1.0b6/pyvisonicalarm/const.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b5/pyvisonicalarm/core.py` & `pyvisonicalarm-0.1.0b6/pyvisonicalarm/core.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b5/pyvisonicalarm/device_definitions.py` & `pyvisonicalarm-0.1.0b6/pyvisonicalarm/device_definitions.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,28 @@
     ContactDevice,
     GSMDevice,
     GenericDevice,
     KeyFobDevice,
     MotionDevice,
     PGMDevice,
     SmokeDevice,
+    TagDevice,
 )
 
 
 DEVICE_TYPES = {
     "GSM": GSMDevice,
     "PGM": PGMDevice,
 }
 
 DEVICE_SUBTYPES = {
     "CONTACT": ContactDevice,
+    "CONTACT_AUX": ContactDevice,
     "MC303_VANISH": ContactDevice,
     "MOTION_CAMERA": CameraDevice,
     "SMOKE": SmokeDevice,
     "BASIC_KEYFOB": KeyFobDevice,
     "KEYFOB_ARM_LED": KeyFobDevice,
+    "GENERIC_PROXY_TAG": TagDevice,
     "FLAT_PIR_SMART": MotionDevice,
     "WL_SIREN": GenericDevice,
 }
```

### Comparing `pyvisonicalarm-0.1.0b5/pyvisonicalarm/devices.py` & `pyvisonicalarm-0.1.0b6/pyvisonicalarm/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,19 @@
     @property
     def owner_name(self) -> str:
         """Get owner name."""
         return self._get_nested_key("traits.owner.name", TEXT_UNKNOWN)
 
 
 @dataclass
+class TagDevice(Device):
+    """Tag device class definition"""
+
+
+@dataclass
 class PGMDevice(Device):
     """PGM device class definition."""
 
     @property
     def parent_id(self) -> int:
         """Get parent id."""
         return self._get_nested_key("traits.parent.id", 0)
```

### Comparing `pyvisonicalarm-0.1.0b5/pyvisonicalarm/exceptions.py` & `pyvisonicalarm-0.1.0b6/pyvisonicalarm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/PKG-INFO` & `pyvisonicalarm-0.1.0b6/pyvisonicalarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b5/setup.py` & `pyvisonicalarm-0.1.0b6/setup.py`

 * *Files identical despite different names*

