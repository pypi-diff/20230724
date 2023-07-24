# Comparing `tmp/pyvisonicalarm-0.1.0b4.tar.gz` & `tmp/pyvisonicalarm-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisonicalarm-0.1.0b4.tar", last modified: Thu Jul 13 18:57:06 2023, max compression
+gzip compressed data, was "pyvisonicalarm-0.1.0b5.tar", last modified: Mon Jul 24 12:08:07 2023, max compression
```

## Comparing `pyvisonicalarm-0.1.0b4.tar` & `pyvisonicalarm-0.1.0b5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/pyvisonicalarm/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/device_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 18:57:06.000000 pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:57:06.915189 pyvisonicalarm-0.1.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-13 18:56:55.000000 pyvisonicalarm-0.1.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/pyvisonicalarm/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20717 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/device_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 12:08:07.000000 pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:08:07.473995 pyvisonicalarm-0.1.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 12:07:55.000000 pyvisonicalarm-0.1.0b5/setup.py
```

### Comparing `pyvisonicalarm-0.1.0b4/LICENSE` & `pyvisonicalarm-0.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b4/PKG-INFO` & `pyvisonicalarm-0.1.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b4/README.md` & `pyvisonicalarm-0.1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b4/pyvisonicalarm/alarm.py` & `pyvisonicalarm-0.1.0b5/pyvisonicalarm/alarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+"""Control and access to alrm info"""
+
 from .classes import (
+    Alarm,
     Camera,
     Event,
     FeatureSet,
     Location,
     PanelInfo,
     Panel,
     Process,
@@ -63,36 +66,39 @@
     def disable_siren(self, mode="all"):
         """Disable the siren (mute the alarm)."""
         return self.__api.disable_siren(mode=mode)["process_token"]
 
     def disarm(self, partition=-1):
         """Send Disarm command to the alarm system."""
         return self.__api.disarm(partition)["process_token"]
-    
+
     def get_alarms(self):
-        return self.__api.get_alarms()
-    
+        """Return alarms."""
+        alarms = self.__api.get_alarms()
+        return [Alarm(alarm) for alarm in alarms]
+
     def get_alerts(self):
+        """Return alerts."""
         return self.__api.get_alerts()
 
     def get_cameras(self):
         """Fetch all the devices that are available."""
         cameras = self.__api.get_cameras()
         return [Camera(camera) for camera in cameras]
 
     def get_devices(self):
         """Fetch all the devices that are available."""
         device_list = []
         devices = self.__api.get_devices()
 
         for device in devices:
-            if DeviceClass := DEVICE_SUBTYPES.get(device["subtype"]):
-                device_list.append(DeviceClass(device))
-            elif DeviceClass := DEVICE_TYPES.get(device["device_type"]):
-                device_list.append(DeviceClass(device))
+            if device_class := DEVICE_SUBTYPES.get(device["subtype"]):
+                device_list.append(device_class(device))
+            elif device_class := DEVICE_TYPES.get(device["device_type"]):
+                device_list.append(device_class(device))
             else:
                 device_list.append(GenericDevice(device))
 
         return device_list
 
     def get_events(self, timestamp_hour_offset=2):
         """Get the last couple of events (60 events on my system)."""
@@ -126,15 +132,14 @@
 
     def get_rest_versions(self):
         """Fetch the supported API versions."""
         return self.api.get_version_info()["rest_versions"]
 
     def get_status(self):
         """Fetch the current state of the alarm system."""
-
         status = self.__api.get_status()
         return Status(status)
 
     def get_troubles(self):
         """Fetch all the troubles that are available."""
         troubles = self.__api.get_troubles()
         return [Trouble(trouble) for trouble in troubles]
@@ -167,17 +172,15 @@
 
     def password_reset(self, email):
         """Send a password reset link to the email address provided in the email argument."""
         return self.__api.password_reset(email)
 
     def password_reset_complete(self, reset_password_code, new_password):
         """Complete the password reset by entering the reset code received in the email and a new password."""
-        return self.__api.password_reset_complete(reset_password_code, new_password)[
-            "user_token"
-        ]
+        return self.__api.password_reset_complete(reset_password_code, new_password)["user_token"]
 
     def set_bypass_zone(self, zone, set_enabled):
         """Enabled or disable zone bypassing (for example, bypass a sensor to disable it)."""
         return self.__api.set_bypass_zone(zone, set_enabled)["process_token"]
 
     def set_name_user(self, user_id, name):
         """Set the name of a user by user ID."""
@@ -192,14 +195,12 @@
         rest_versions = self.api.get_version_info()["rest_versions"]
         rest_versions.sort(key=float)
         if version == "latest":
             self.__api.set_rest_version(rest_versions[-1])
         elif version in rest_versions:
             self.__api.set_rest_version(version)
         else:
-            raise UnsupportedRestAPIVersionError(
-                f"Rest API version {version} is not supported by server."
-            )
+            raise UnsupportedRestAPIVersionError(f"Rest API version {version} is not supported by server.")
 
     def set_user_code(self, user_id, user_code):
         """Set the code of a user by user ID."""
         return self.__api.set_user_code(user_code, user_id)["process_token"]
```

### Comparing `pyvisonicalarm-0.1.0b4/pyvisonicalarm/classes.py` & `pyvisonicalarm-0.1.0b5/pyvisonicalarm/classes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from dataclasses import dataclass
+"""Classes for Alarm Entities"""
+
 import functools
 import inspect
+from dataclasses import dataclass
 
 from .const import TEXT_UNKNOWN
 
 
 # Decorator function to set string output to title case
 def title_case(func):
+    """Format to title case"""
+
     def wrapper(*args, **kwargs):
         if result := func(*args, **kwargs):
             return str(result).title()
         return result
 
     return wrapper
 
@@ -18,35 +22,31 @@
 @dataclass
 class BaseClass:
     """Base class"""
 
     _data: dict
 
     def __repr__(self):
-        r = ""
-        attrs = inspect.getmembers(self, lambda a: not (inspect.isroutine(a)))
-        for i, a in enumerate([attr for attr in attrs if self._is_property(attr)]):
+        res = ""
+        attrs = inspect.getmembers(self, lambda a: not inspect.isroutine(a))
+        for i, attr in enumerate([attr for attr in attrs if self._is_property(attr)]):
             if i:
-                r = r + ", "
-            r = r + f"{a[0]} = {getattr(self, a[0])}"
-        return f"{type(self).__name__}({r})"
+                res = res + ", "
+            res = res + f"{attr[0]} = {getattr(self, attr[0])}"
+        return f"{type(self).__name__}({res})"
 
     def __str__(self):
-        r = {}
-        attrs = inspect.getmembers(self, lambda a: not (inspect.isroutine(a)))
-        for a in [attr for attr in attrs if self._is_property(attr)]:
-            r[a[0]] = getattr(self, a[0])
-        return f"{str(type(self))}: {r}"
+        res = {}
+        attrs = inspect.getmembers(self, lambda a: not inspect.isroutine(a))
+        for attr in [attr for attr in attrs if self._is_property(attr)]:
+            res[attr[0]] = getattr(self, attr[0])
+        return f"{str(type(self))}: {res}"
 
     def _is_property(self, attr) -> bool:
-        if not (
-            attr[0].startswith("__")
-            and attr[0].endswith("__")
-            or attr[0].startswith("_")
-        ):
+        if not (attr[0].startswith("__") and attr[0].endswith("__") or attr[0].startswith("_")):
             return True
         return False
 
     def _get_nested_key(self, path, *default):
         """Get key value in json by dotted notation or return default"""
         try:
             return functools.reduce(lambda x, y: x[y], path.split("."), self._data)
@@ -56,59 +56,66 @@
             return None
 
 
 @dataclass
 class Camera(BaseClass):
     """Class definition of an event in the alarm system."""
 
-    # Camera properties
     @property
     @title_case
     def location(self) -> str:
+        """Return camera location."""
         return self._data.get("location")
 
     @property
     def partitions(self) -> list[int]:
+        """Return camera partitions."""
         return self._data.get("partitions", [])
 
     @property
     def preenroll(self) -> bool:
+        """Pre-enroll camera."""
         return self._data.get("preenroll", False)
 
     @property
     def preview_path(self) -> str:
+        """Get camera preview path."""
         return self._data.get("preview_path")
 
     @property
     def status(self) -> str:
+        """Get camera status."""
         return self._data.get("status")
 
     @property
     def timestamp(self) -> str:
+        """Get camera timestamp."""
         # TODO: COnvert to datetime
         return self._data.get("timestamp")
 
     @property
     def zone(self) -> int:
+        """Get camera zone id."""
         return self._data.get("zone")
 
     @property
     @title_case
     def zone_name(self) -> str:
+        """Get camera zone name."""
         return self._data.get("zone_name")
 
 
 @dataclass
 class Event(BaseClass):
     """Class definition of an event in the alarm system."""
 
     # Event properties
     @property
-    def id(self) -> int:
-        """User ID."""
+    def id(self) -> int:  # pylint: disable=invalid-name
+        """Event ID."""
         return self._data.get("event", 0)
 
     @property
     def type_id(self) -> int:
         """Event type ID."""
         return self._data.get("type_id", 0)
 
@@ -165,80 +172,94 @@
 @dataclass
 class FeatureSet(BaseClass):
     """Class definition of an event in the alarm system."""
 
     # Event properties
     @property
     def events_enabled(self):
+        """Get if events enabled."""
         return self._get_nested_key("events.is_enabled")
 
     @property
     def datetime_enabled(self):
+        """Get if datetime enabled."""
         return self._get_nested_key("datetime.is_enabled")
 
     @property
     def partitions_enabled(self):
+        """Getof partitions enabled."""
         return self._get_nested_key("partitions.is_enabled")
 
     @property
     def partitions_has_labels(self):
+        """Get if partitions labels enabled."""
         return self._get_nested_key("partitions.is_labels_enabled")
 
     @property
     def partitions_max_count(self):
+        """Get max supported partitions."""
         return self._get_nested_key("partitions.max_partitions")
 
     @property
     def devices_enabled(self):
+        """Get if devices enabled."""
         return self._get_nested_key("devices.is_enabled")
 
     @property
     def sirens_can_enable(self):
+        """Get if can enable sirens."""
         return self._get_nested_key("sirens.can_enable")
 
     @property
     def sirens_can_disable(self):
+        """Get if can disable sirens."""
         return self._get_nested_key("sirens.can_disable")
 
     @property
     def home_automation_devices_enabled(self):
+        """Get if home automation devices enabled."""
         return self._get_nested_key("home_automation_devices.is_enabled")
 
     @property
     def state_enabled(self):
+        """Get if state enabled."""
         return self._get_nested_key("state.is_enabled")
 
     @property
     def state_can_set(self):
+        """Get if state can be set."""
         return self._get_nested_key("state.can_set")
 
     @property
     def state_can_get(self):
+        """Get if state can be read."""
         return self._get_nested_key("state.can_get")
 
     @property
     def faults_enabled(self):
+        """Get if faults enabled."""
         return self._get_nested_key("faults.is_enabled")
 
     @property
     def diagnostic_enabled(self):
+        """Get if diagnostic enabled."""
         return self._get_nested_key("diagnostic.is_enabled")
 
     @property
     def wifi_enabled(self):
+        """Get if wifi enabled."""
         return self._get_nested_key("wifi.is_enabled")
 
 
 @dataclass
 class Location(BaseClass):
     """Class definition of a location in the alarm system."""
 
-    # Location properties
     @property
-    def id(self):
+    def id(self):  # pylint: disable=invalid-name
         """Location ID."""
         return self._data.get("hel_id")
 
     @property
     @title_case
     def name(self):
         """Location name."""
@@ -248,71 +269,86 @@
     def is_editable(self):
         """Location is editable."""
         return self._data.get("is_editable")
 
 
 @dataclass
 class PanelInfoPartition(BaseClass):
+    """Class to hold partition info."""
+
     @property
-    def id(self) -> int:
+    def id(self) -> int:  # pylint: disable=invalid-name
+        """Partition ID."""
         return self._data.get("id")
 
     @property
     def active(self) -> bool:
+        """Get if partition active."""
         return self._data.get("active")
 
     @property
     def exit_delay_time(self) -> int:
+        """Get partition exit delay."""
         return self._data.get("exit_delay_time")
 
     @property
     def state_set(self) -> str:
+        """Get partition state."""
         return self._data.get("state_set")
 
     @property
     def name(self) -> str:
+        """Get partition name."""
         return self._data.get("name")
 
 
 @dataclass
 class PanelInfoFeatures(BaseClass):
+    """Class to hold panel features."""
+
     @property
     def video_on_demand(self) -> bool:
+        """Get if supports video."""
         return self._data.get("video_on_demand")
 
     @property
     def alert(self) -> bool:
+        """Get alerts."""
         return self._data.get("alert")
 
     @property
     def enabling_siren(self) -> bool:
+        """Get if supports enabling siren"""
         return self._data.get("enabling_siren")
 
     @property
     def disabling_siren(self) -> bool:
+        """Get if supports disabling siren."""
         return self._data.get("disabling_siren")
 
     @property
     def wi_fi_connection(self) -> bool:
+        """Get if supports wifi."""
         return self._data.get("wi_fi_connection")
 
     @property
     def set_date_time(self) -> bool:
+        """Get date time."""
         return self._data.get("set_date_time")
 
     @property
     def outputs_setup(self) -> bool:
+        """Get outputs."""
         return self._data.get("outputs_setup")
 
 
 @dataclass
 class PanelInfo(BaseClass):
     """Class definition of the general alarm system information."""
 
-    # PanelInfo properties
     @property
     @title_case
     def bypass_mode(self) -> str:
         """Bypass Mode"""
         return self._data.get("bypass_mode")
 
     @property
@@ -337,155 +373,234 @@
     def model(self) -> str:
         """Model name"""
         return self._data.get("model")
 
     @property
     def remote_admin_requires_user_acceptance(self) -> bool:
         """Programming requires user acceptance"""
-        return self._data.get(
-            "remote_switch_to_programming_mode_requires_user_acceptance"
-        )
+        return self._data.get("remote_switch_to_programming_mode_requires_user_acceptance")
 
     @property
     def serial(self) -> str:
         """Serial no"""
         return self._data.get("serial")
 
     @property
+    def multi_partitions(self) -> bool:
+        """Multi partitions enabled"""
+        return True if len(self._data.get("partitions")) > 1 else False
+
+    @property
     def partitions(self) -> list[PanelInfoPartition]:
         """Partitions info"""
-        return list(
-            [
-                PanelInfoPartition(partition)
-                for partition in self._data.get("partitions")
-            ]
-        )
+        return list([PanelInfoPartition(partition) for partition in self._data.get("partitions")])
 
     @property
     def features(self) -> PanelInfoFeatures:
+        """Get panel features."""
         return PanelInfoFeatures(self._data.get("features"))
 
 
 @dataclass
 class Panel(BaseClass):
     """Class definition of the general alarm system information."""
 
     # Panel properties
     @property
     def panel_serial(self) -> str:
+        """Get panel serial."""
         return self._data.get("panel_serial")
 
     @property
     def alias(self) -> str:
+        """Get panel alias."""
         return self._data.get("alias")
 
 
 @dataclass
 class Partition(BaseClass):
     """Class definition of a partition in the alarm system."""
 
     # Partition properties
     @property
-    def id(self) -> int:
+    def id(self) -> int:  # pylint: disable=invalid-name
+        """Get partition id"""
         return self._data.get("id")
 
     @property
     def state(self):
+        """Get partition state."""
         return self._data.get("state")
 
     @property
     def status(self) -> str:
+        """Get partition status."""
         return self._data.get("status")
 
     @property
     def ready(self) -> bool:
+        """Get if partition ready."""
         return self._data.get("ready")
 
     @property
     def options(self) -> list:
+        """Get partition options."""
         return self._data.get("options")
 
 
 @dataclass
 class Process(BaseClass):
     """Class definition of a process in the alarm system."""
 
     # Partition properties
     @property
     def token(self) -> str:
+        """Get process token."""
         return self._data.get("token")
 
     @property
     def status(self) -> str:
+        """Get process status."""
         return self._data.get("status")
 
     @property
     def message(self) -> str:
+        """Get process message."""
         return self._data.get("message")
 
     @property
     def error(self) -> str:
+        """Get process error."""
         return self._data.get("error")
 
 
 @dataclass
 class Status(BaseClass):
     """Class definition representing the status of the alarm system."""
 
     # Status properties
     @property
     def connected(self) -> bool:
+        """Get if connected."""
         return self._data.get("connected")
 
     @property
     def bba_connected(self) -> bool:
+        """Get if broadband connected."""
         return self._get_nested_key("connected_status.bba.is_connected", False)
 
     @property
     def bba_state(self) -> str:
+        """Get broadband connection state."""
         return self._get_nested_key("connected_status.bba.state", TEXT_UNKNOWN)
 
     @property
     def gprs_connected(self) -> bool:
+        """Get if GPRS connected."""
         return self._get_nested_key("connected_status.gprs.is_connected", False)
 
     @property
     def gprs_state(self) -> str:
+        """Get GPRS state."""
         return self._get_nested_key("connected_status.grps.state", TEXT_UNKNOWN)
 
     @property
     def discovery_completed(self) -> bool:
+        """Get if discovery completed."""
         return self._get_nested_key("discovery.completed")
 
     @property
     def discovery_stages(self) -> int:
+        """Get discovery stages."""
         return self._get_nested_key("discovery.stages")
 
     @property
     def discovery_in_queue(self) -> int:
+        """Get if discovery in queue."""
         return self._get_nested_key("discovery.in_queue")
 
     @property
     def discovery_triggered(self) -> bool:
+        """Get if discovery triggered."""
         return self._get_nested_key("discovery.triggered")
 
     @property
     def partitions(self) -> list[Partition]:
+        """Get partitions."""
         return [Partition(partition) for partition in self._data.get("partitions", [])]
 
     @property
     def rssi_level(self) -> int:
+        """Get RSSI signal level."""
         return self._get_nested_key("rssi.level")
 
     @property
     def rssi_network(self) -> str:
+        """Get RSSI signal network."""
         return self._get_nested_key("rssi.network")
 
 
 @dataclass
+class Alarm(BaseClass):
+    """Class definition of Alarm"""
+
+    @property
+    def device_type(self) -> str:
+        """Device type."""
+        return self._data.get("device_type")
+
+    @property
+    def alarm_type(self) -> str:
+        """Alarm type."""
+        return self._data.get("alarm_type")
+
+    @property
+    def date_time(self) -> str:
+        """Date time of alarm"""
+        return self._data.get("datetime")
+
+    @property
+    def has_video(self) -> bool:
+        """Has video."""
+        return self._data.get("has_video")
+
+    @property
+    def event_id(self) -> int:
+        """Event id."""
+        return self._data.get("evt_id")
+
+    @property
+    @title_case
+    def location(self) -> str:
+        """Location."""
+        return self._data.get("location")
+
+    @property
+    def partitions(self) -> list[int]:
+        """Partitions."""
+        return self._data.get("partitions")
+
+    @property
+    def zone(self) -> int:
+        """Zone ID."""
+        return self._data.get("zone")
+
+    @property
+    @title_case
+    def zone_name(self) -> str:
+        """Zone type."""
+        return self._data.get("zone_name")
+
+    @property
+    def zone_type(self) -> str:
+        """Zone type."""
+        return self._data.get("zone_type")
+
+
+@dataclass
 class Trouble(BaseClass):
     """Class definition of a trouble in the alarm system."""
 
     # Trouble properties
     @property
     def device_type(self) -> str:
         """Device type."""
@@ -526,15 +641,15 @@
 
 @dataclass
 class User(BaseClass):
     """Class definition of a user in the alarm system."""
 
     # User properties
     @property
-    def id(self) -> int:
+    def id(self) -> int:  # pylint: disable=invalid-name
         """User ID."""
         return self._data.get("id")
 
     @property
     @title_case
     def name(self) -> str:
         """User name."""
@@ -554,12 +669,14 @@
 @dataclass
 class WakeupSMS(BaseClass):
     """Class definition of a wakeup SMS in the alarm system."""
 
     # Wakeup SMS properties
     @property
     def phone_number(self) -> str:
+        """Get SMS phone number."""
         return self._data.get("phone")
 
     @property
     def message(self) -> str:
+        """Get sms message."""
         return self._data.get("sms")
```

### Comparing `pyvisonicalarm-0.1.0b4/pyvisonicalarm/const.py` & `pyvisonicalarm-0.1.0b5/pyvisonicalarm/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,31 @@
+"""Visonic API constants"""
+
+DEFAULT_REST_VERSION = "9.0"
+
 TEXT_UNKNOWN = "Unknown"
 TEXT_OPEN = "Open"
 TEXT_OPENED = "OPENED"
 TEXT_CLOSED = "Closed"
 TEXT_STATUS_HOME = "HOME"
 TEXT_STATUS_AWAY = "AWAY"
 TEXT_STATUS_DISARM = "DISARM"
 
 
 class RequestType:
+    """HTTP request type."""
+
     GET = "GET"
     POST = "POST"
 
 
 class VisonicURL:
-    BASE = "https://{}/rest_api"  #'https://[hostname]/rest_api/[rest_version]
+    """URL paths."""
+
+    BASE = "https://{}/rest_api"  # 'https://[hostname]/rest_api/[rest_version]
 
     ACCESS_GRANT = "access/grant"
     ACCESS_REVOKE = "access/revoke"
     ACTIVATE_SIREN = "activate_siren"
     ALARMS = "alarms"
     ALERTS = "alerts"
     APP_TYPE = "apptype"
```

### Comparing `pyvisonicalarm-0.1.0b4/pyvisonicalarm/core.py` & `pyvisonicalarm-0.1.0b5/pyvisonicalarm/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,56 @@
+"""API for Visonic Alarm"""
+
 import json
 import requests
 
 from .const import (
+    DEFAULT_REST_VERSION,
     TEXT_STATUS_AWAY,
     TEXT_STATUS_DISARM,
     TEXT_STATUS_HOME,
     RequestType,
     VisonicURL,
 )
-
-from .exceptions import *
+from .exceptions import (
+    AlreadyGrantedError,
+    AlreadyLinkedError,
+    AppIDRequiredError,
+    ConnectionTimeoutError,
+    EmailRequiredError,
+    InvalidUserCodeError,
+    LoginAttemptsLimitReachedError,
+    LoginTemporaryBlockedError,
+    NewPasswordStrengthError,
+    NotAllowedError,
+    NotFoundError,
+    PanelNotConnectedError,
+    PanelSerialIncorrectError,
+    PanelSerialRequiredError,
+    PasswordRequiredError,
+    ResetPasswordCodeIncorrectError,
+    SessionTokenError,
+    UnauthorizedError,
+    UndefinedBadRequestError,
+    UndefinedForbiddenError,
+    UserAuthRequiredError,
+    UserCodeIncorrectError,
+    UserCodeRequiredError,
+    WrongPanelSerialOrMasterUserCodeError,
+    WrongUsernameOrPasswordError,
+)
 
 
 class API(object):
     """Class used for communication with the Visonic API"""
 
     # Client configuration
     __app_type = "com.visonic.powermaxapp"
     __user_agent = "Dart/2.10 (dart:io)"
-    __rest_version = "10.0"
+    __rest_version = DEFAULT_REST_VERSION
 
     # API tokens
     __user_token = None
     __session_token = None
 
     # Use a session to reuse one TCP connection instead of creating a new
     # connection for every call to the API
@@ -75,18 +103,15 @@
                 if pair["key"] == "new_password":
                     raise NewPasswordStrengthError()
         elif api["error"] == 10004:  # WrongCombination
             for pair in api["extras"]:
                 if pair["value"] == "wrong_combination":
                     if pair["key"] == "email" or pair["key"] == "password":
                         raise WrongUsernameOrPasswordError()
-                    if (
-                        pair["key"] == "panel_serial"
-                        or pair["key"] == "master_user_code"
-                    ):
+                    if pair["key"] == "panel_serial" or pair["key"] == "master_user_code":
                         raise WrongPanelSerialOrMasterUserCodeError()
         elif api["error"] == 10021:  # WrongUserCode
             raise UserCodeIncorrectError()
         elif api["error"] == 400 and api["error_reason_code"] == "PanelNotConnected":
             raise PanelNotConnectedError()
 
         # Raise a generic error when the library has no
@@ -155,57 +180,51 @@
         if with_user_token:
             headers["User-Token"] = self.__user_token
 
         # Perform the request and raise an exception
         # if the response is not OK (HTML 200)
         try:
             if request_type == "GET":
-                response = self.__session.get(
-                    url, headers=headers, timeout=self.__timeout
-                )
+                response = self.__session.get(url, headers=headers, timeout=self.__timeout)
             elif request_type == "POST":
-                response = self.__session.post(
-                    url, headers=headers, data=data_json, timeout=self.__timeout
-                )
+                response = self.__session.post(url, headers=headers, data=data_json, timeout=self.__timeout)
             response.raise_for_status()
-        except requests.exceptions.ConnectTimeout:
+        except requests.exceptions.ConnectTimeout as exc:
             raise ConnectionTimeoutError(
                 f"Connection to '{self.__hostname}' timed out after {str(self.__timeout)} seconds."
-            )
-            return None
-        except requests.exceptions.HTTPError as e:
+            ) from exc
+        except requests.exceptions.HTTPError as exc:
             api = json.loads(response.content.decode("utf-8"))
-            if "400 Client Error: Bad Request" in str(e):
+            if "400 Client Error: Bad Request" in str(exc):
                 self.__raise_on_bad_request(response.content)
-            elif "401 Client Error: Unauthorized" in str(e):
+            elif "401 Client Error: Unauthorized" in str(exc):
                 self.__raise_on_unauthorized(response.content)
-            elif "403 Client Error: Forbidden" in str(e):
+            elif "403 Client Error: Forbidden" in str(exc):
                 self.__raise_on_forbidden(response.content)
-            elif "404 Client Error: Not Found" in str(e):
-                raise NotFoundError()
-            elif "420 Client Error:" in str(e):
-                # TODO: {'error': 10020, 'error_message': 'Login temporary blocked', 'error_reason_code': 'LoginTemporaryBlocked', 'extras': [{'key': 'timeout', 'value': 44}]} // 44 = seconds to unblocked
-                # print(api)
+            elif "404 Client Error: Not Found" in str(exc):
+                raise NotFoundError() from exc
+            elif "420 Client Error:" in str(exc):
+                # TODO: {'error': 10020, 'error_message': 'Login temporary blocked', 'error_reason_code':
+                # 'LoginTemporaryBlocked', 'extras': [{'key': 'timeout', 'value': 44}]} // 44 = seconds to unblocked
                 raise LoginTemporaryBlockedError(
-                    f"Login is temporary blocked due to too many failed login attempts ({api['extras'][0]['count']} seconds remaining)."
-                )
-            elif "440 Client Error: Session token not found" in str(e):
-                raise SessionTokenError()
-            elif "442 Client Error: Login attempts limit reached" in str(e):
-                raise LoginAttemptsLimitReachedError("Login attempts limit reached.")
-            elif "444 Client Error: Wrong user code" in str(e):
-                raise InvalidUserCodeError(
-                    "Authentication failed due to wrong user code."
-                )
+                    f"Login is temporary blocked due to too many failed login attempts "
+                    f"({api['extras'][0]['count']} seconds remaining)."
+                ) from exc
+            elif "440 Client Error: Session token not found" in str(exc):
+                raise SessionTokenError() from exc
+            elif "442 Client Error: Login attempts limit reached" in str(exc):
+                raise LoginAttemptsLimitReachedError("Login attempts limit reached.") from exc
+            elif "444 Client Error: Wrong user code" in str(exc):
+                raise InvalidUserCodeError("Authentication failed due to wrong user code.") from exc
             else:
                 print(api)
                 raise
 
         # Check HTTP response code
-        if response.status_code == requests.codes.ok:
+        if response.status_code == 200:
             return json.loads(response.content.decode("utf-8"))
         else:
             return None
 
     ######################
     # Public API methods #
     ######################
@@ -226,15 +245,15 @@
         return self.__user_token
 
     @property
     def app_id(self):
         """Property to keep track of the user id (UUID) beeing used."""
         return self.__app_id
 
-    def get_version_info(self):
+    def get_version_info(self) -> dict:
         """Find out which REST API versions are supported."""
         return self.__send_request(
             VisonicURL.VERSION,
             with_session_token=False,
             with_user_token=False,
             request_type=RequestType.GET,
         )
@@ -269,25 +288,21 @@
         except requests.HTTPError:
             return False
 
     def access_grant(self, user_id, email):
         """Grant a user access to the alarm panel via the API."""
         user_data = {"user": user_id, "email": email}
         user_json = json.dumps(user_data, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.ACCESS_GRANT, data_json=user_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.ACCESS_GRANT, data_json=user_json, request_type=RequestType.POST)
 
     def access_revoke(self, user_id):
         """Revoke access to the alarm panel via the API for a user."""
         user_data = {"user": user_id}
         user_json = json.dumps(user_data, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.ACCESS_REVOKE, data_json=user_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.ACCESS_REVOKE, data_json=user_json, request_type=RequestType.POST)
 
     def activate_siren(self):
         """Activate the siren (sound the alarm)."""
         siren_data = {}
         siren_json = json.dumps(siren_data, separators=(",", ":"))
         return self.__send_request(
             VisonicURL.ACTIVATE_SIREN,
@@ -341,14 +356,20 @@
         """The general panel information is only supported in version 4.0."""
         return self.__send_request(VisonicURL.PANEL_INFO)
 
     def get_panels(self):
         """Get a list of panels."""
         return self.__send_request(VisonicURL.PANELS)
 
+    def get_preview_image(self, image_path: str):
+        """Get preview image for camera"""
+        if image_path:
+            return self.__send_request(image_path.replace("/rest_api", ""))
+        return None
+
     def get_process_status(self, process_token):
         """Get the current status of a process running on API server."""
         return self.__send_request(VisonicURL.PROCESS_STATUS.format(process_token))
 
     def get_smart_devices(self):
         """Get a list of smart devices."""
         return self.__send_request(VisonicURL.SMART_DEVICES)
@@ -370,28 +391,24 @@
         Note: Only master users can see the active_user_ids!"""
         return self.__send_request(VisonicURL.USERS)
 
     def get_wakeup_sms(self):
         """Get the settings needed to wake up the alarm panel via SMS."""
         return self.__send_request(VisonicURL.WAKEUP_SMS)
 
-    def panel_add(
-        self, alias: str, panel_serial: str, access_proof: str, master_user_code: str
-    ):
+    def panel_add(self, alias: str, panel_serial: str, access_proof: str, master_user_code: str):
         """Add a new alarm panel to the user account. A master user code is required."""
         panel_data = {
             "alias": alias,
             "panel_serial": panel_serial,
             "access_proof": access_proof,
             "master_user_code": master_user_code,
         }
         panel_json = json.dumps(panel_data, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.PANEL_ADD, data_json=panel_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.PANEL_ADD, data_json=panel_json, request_type=RequestType.POST)
 
     def panel_login(self, panel_serial: str, user_code: str):
         """Try to login to the alarm panel and get a session token."""
         login_info = {
             "user_code": user_code,
             "app_type": self.__app_type,
             "app_id": self.__app_id,
@@ -414,29 +431,25 @@
     def panel_rename(self, alias: str, panel_serial: str):
         """Rename an alarm panel."""
         panel_data = {
             "panel_serial": panel_serial,
             "alias": alias,
         }
         panel_json = json.dumps(panel_data, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.PANEL_RENAME, data_json=panel_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.PANEL_RENAME, data_json=panel_json, request_type=RequestType.POST)
 
     def panel_unlink(self, panel_serial: str, password: str, app_id: str):
         """Unlink an alarm panel from the user account."""
         panel_data = {
             "panel_serial": panel_serial,
             "password": password,
             "app_id": app_id,
         }
         panel_json = json.dumps(panel_data, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.PANEL_UNLINK, data_json=panel_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.PANEL_UNLINK, data_json=panel_json, request_type=RequestType.POST)
 
     def password_reset(self, email: str):
         """Request a password reset email. An email will be sent to the email address provided."""
         reset_data = {"email": email}
         reset_json = json.dumps(reset_data, separators=(",", ":"))
         return self.__send_request(
             VisonicURL.PASSWORD_RESET,
@@ -474,57 +487,45 @@
         bypass_json = json.dumps(bypass_data, separators=(",", ":"))
         return self.__send_request(
             VisonicURL.SET_BYPASS_ZONE,
             data_json=bypass_json,
             request_type=RequestType.POST,
         )
 
-    def set_name(self, object_class: str, id: int, name: str):
+    def set_name(self, object_class: str, device_id: int, name: str):
         """Set the name of any type of object in the alarm system."""
-        name_data = {"class": object_class, "id": id, "name": name}
+        name_data = {"class": object_class, "id": device_id, "name": name}
         name_json = json.dumps(name_data, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.SET_NAME, data_json=name_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.SET_NAME, data_json=name_json, request_type=RequestType.POST)
 
     def set_user_code(self, user_code: str, user_id: str):
         """Set the code of a user in the alarm system."""
         code_data = {"user_code": user_code, "user_id": user_id}
         code_json = json.dumps(code_data, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.SET_USER_CODE, data_json=code_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.SET_USER_CODE, data_json=code_json, request_type=RequestType.POST)
 
     def arm_home(self, partition: int):
         """Arm in Home mode."""
         arm_info = {"partition": partition, "state": TEXT_STATUS_HOME}
         arm_json = json.dumps(arm_info, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.SET_STATE, data_json=arm_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.SET_STATE, data_json=arm_json, request_type=RequestType.POST)
 
     def arm_away(self, partition: id):
         """Arm in Away mode."""
         arm_info = {"partition": partition, "state": TEXT_STATUS_AWAY}
         arm_json = json.dumps(arm_info, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.SET_STATE, data_json=arm_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.SET_STATE, data_json=arm_json, request_type=RequestType.POST)
 
     def disarm(self, partition: id):
         """Disarm the alarm system."""
         disarm_info = {"partition": partition, "state": TEXT_STATUS_DISARM}
         disarm_json = json.dumps(disarm_info, separators=(",", ":"))
-        return self.__send_request(
-            VisonicURL.SET_STATE, data_json=disarm_json, request_type=RequestType.POST
-        )
+        return self.__send_request(VisonicURL.SET_STATE, data_json=disarm_json, request_type=RequestType.POST)
 
     def send_get(self, url):
         """Send a custom POST request."""
         return self.__send_request(url)
 
     def send_post(self, url, data):
         """Send a custom POST request."""
         data_json = json.dumps(data, separators=(",", ":"))
-        return self.__send_request(
-            url, data_json=data_json, request_type=RequestType.POST
-        )
+        return self.__send_request(url, data_json=data_json, request_type=RequestType.POST)
```

### Comparing `pyvisonicalarm-0.1.0b4/pyvisonicalarm/devices.py` & `pyvisonicalarm-0.1.0b5/pyvisonicalarm/devices.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,94 @@
+"""Device type classes"""
+
 from dataclasses import dataclass
 from datetime import datetime
+
 from .classes import BaseClass, title_case
 from .const import TEXT_CLOSED, TEXT_OPEN, TEXT_OPENED, TEXT_UNKNOWN
 
 
 @dataclass
 class Device(BaseClass):
     """Base class definition of a device in the alarm system."""
 
-    # Device properties
     @property
     def bypass(self) -> bool | None:
+        """Get if bypass enabled."""
         return self._get_nested_key("traits.bypass.enabled", None)
 
     @property
     def device_number(self) -> int:
+        """Get device number."""
         return self._data.get("device_number", 0)
 
     @property
     def device_type(self) -> str:
+        """Get device type."""
         return self._data.get("device_type")
 
     @property
     def enrollment_id(self) -> str:
+        """Get enrollment id."""
         return self._data.get("enrollment_id")
 
     @property
-    def id(self) -> int:
+    def id(self) -> int:  # pylint: disable=invalid-name
+        """Get device id."""
         return self._data.get("id", 0)
 
     @property
     @title_case
     def location(self) -> str:
+        """Get device location."""
         return self._get_nested_key("traits.location.name")
 
     @property
     def name(self) -> str:
+        """Get device name."""
         return self._data.get("name", TEXT_UNKNOWN)
 
     @property
     def partitions(self) -> list:
+        """Get device partitions."""
         return self._data.get("partitions", [])
 
     @property
     def preenroll(self) -> bool:
+        """Get if device in preenroll."""
         return self._data.get("preenroll", False)
 
     @property
     def removable(self) -> bool:
+        """Get if device removeable."""
         return self._data.get("removable", False)
 
     @property
     def renamable(self) -> bool:
+        """Get if device renameable."""
         return self._data.get("renamable", False)
 
     @property
     def soak(self) -> bool:
+        """Get if device part of soak test."""
         return self._get_nested_key("traits.soak.enabled", False)
 
     @property
     def subtype(self) -> str:
+        """Get device subtype."""
         return self._data.get("subtype", TEXT_UNKNOWN)
 
     @property
     def warnings(self) -> list:
+        """Get device warnings."""
         return self._data.get("warnings", [])
 
     @property
     def zone_type(self) -> str:
+        """Get device zone type."""
         return self._data.get("zone_type", TEXT_UNKNOWN)
 
 
 @dataclass
 class CameraDevice(Device):
     """Camera device class definition."""
 
@@ -85,71 +102,81 @@
         """Returns the current state of the contact."""
         if self.warnings:
             for warning in self.warnings:
                 if warning["type"] == TEXT_OPENED:
                     return TEXT_OPEN
         return TEXT_CLOSED
 
+
 @dataclass
 class MotionDevice(Device):
     """Motion sensor device class definition."""
 
     @property
     def brightness(self) -> int:
+        """Get brightness level."""
         return self._get_nested_key("traits.meteo_info.brightness.value")
-    
+
     @property
     def brightness_last_updated(self) -> datetime:
+        """Get brightness last updated."""
         return self._get_nested_key("traits.meteo_info.brightness.date")
 
     @property
     def temperature(self) -> float:
+        """Get temperature."""
         return self._get_nested_key("traits.meteo_info.temperature.value")
-    
+
     @property
     def temperature_last_updated(self) -> datetime:
+        """Get temperature last updated."""
         return self._get_nested_key("traits.meteo_info.temperature.date")
 
 
 @dataclass
 class GenericDevice(Device):
     """Smoke device class definition."""
 
 
 @dataclass
 class GSMDevice(Device):
     """GSM device class definition."""
 
     @property
     def signal_level(self) -> str | None:
+        """Get signal level."""
         return self._get_nested_key("traits.signal_level.level")
 
 
 @dataclass
 class KeyFobDevice(Device):
     """KeyFob device class definition."""
 
     @property
     def owner_id(self) -> int:
+        """Get owner id."""
         return self._get_nested_key("traits.owner.id", 0)
 
     @property
     def owner_name(self) -> str:
+        """Get owner name."""
         return self._get_nested_key("traits.owner.name", TEXT_UNKNOWN)
 
 
 @dataclass
 class PGMDevice(Device):
     """PGM device class definition."""
 
     @property
     def parent_id(self) -> int:
+        """Get parent id."""
         return self._get_nested_key("traits.parent.id", 0)
 
     @property
     def parent_port(self) -> int:
+        """Get parent port."""
         return self._get_nested_key("traits.parent.port", 0)
 
 
 @dataclass
 class SmokeDevice(Device):
     """Smoke device class definition."""
```

### Comparing `pyvisonicalarm-0.1.0b4/pyvisonicalarm.egg-info/PKG-INFO` & `pyvisonicalarm-0.1.0b5/pyvisonicalarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b4/setup.py` & `pyvisonicalarm-0.1.0b5/setup.py`

 * *Files identical despite different names*

