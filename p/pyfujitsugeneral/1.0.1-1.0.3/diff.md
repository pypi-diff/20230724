# Comparing `tmp/pyfujitsugeneral-1.0.1.tar.gz` & `tmp/pyfujitsugeneral-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfujitsugeneral-1.0.1.tar", last modified: Fri Mar 10 17:05:15 2023, max compression
+gzip compressed data, was "pyfujitsugeneral-1.0.3.tar", last modified: Mon Jul 24 13:56:12 2023, max compression
```

## Comparing `pyfujitsugeneral-1.0.1.tar` & `pyfujitsugeneral-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-03-10 17:05:15.586479 pyfujitsugeneral-1.0.1/
--rw-r--r--   0 bigmoby    (501) staff       (20)     1102 2023-03-01 12:48:11.000000 pyfujitsugeneral-1.0.1/LICENSE
--rw-r--r--   0 bigmoby    (501) staff       (20)      655 2023-03-10 17:05:15.586741 pyfujitsugeneral-1.0.1/PKG-INFO
--rw-r--r--   0 bigmoby    (501) staff       (20)       98 2023-03-01 15:50:34.000000 pyfujitsugeneral-1.0.1/README.md
-drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-03-10 17:05:15.569772 pyfujitsugeneral-1.0.1/pyfujitsugeneral/
--rw-r--r--   0 bigmoby    (501) staff       (20)      111 2023-03-01 15:43:25.000000 pyfujitsugeneral-1.0.1/pyfujitsugeneral/__init__.py
--rw-r--r--   0 bigmoby    (501) staff       (20)     7128 2023-03-02 17:55:28.000000 pyfujitsugeneral-1.0.1/pyfujitsugeneral/api.py
--rw-r--r--   0 bigmoby    (501) staff       (20)    15731 2023-03-10 16:59:02.000000 pyfujitsugeneral-1.0.1/pyfujitsugeneral/splitAC.py
-drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-03-10 17:05:15.585572 pyfujitsugeneral-1.0.1/pyfujitsugeneral.egg-info/
--rw-r--r--   0 bigmoby    (501) staff       (20)      655 2023-03-10 17:05:15.000000 pyfujitsugeneral-1.0.1/pyfujitsugeneral.egg-info/PKG-INFO
--rw-r--r--   0 bigmoby    (501) staff       (20)      316 2023-03-10 17:05:15.000000 pyfujitsugeneral-1.0.1/pyfujitsugeneral.egg-info/SOURCES.txt
--rw-r--r--   0 bigmoby    (501) staff       (20)        1 2023-03-10 17:05:15.000000 pyfujitsugeneral-1.0.1/pyfujitsugeneral.egg-info/dependency_links.txt
--rw-r--r--   0 bigmoby    (501) staff       (20)       38 2023-03-10 17:05:15.000000 pyfujitsugeneral-1.0.1/pyfujitsugeneral.egg-info/requires.txt
--rw-r--r--   0 bigmoby    (501) staff       (20)       17 2023-03-10 17:05:15.000000 pyfujitsugeneral-1.0.1/pyfujitsugeneral.egg-info/top_level.txt
--rw-r--r--   0 bigmoby    (501) staff       (20)       79 2023-03-10 17:05:15.590303 pyfujitsugeneral-1.0.1/setup.cfg
--rw-r--r--   0 bigmoby    (501) staff       (20)      955 2023-03-10 17:01:35.000000 pyfujitsugeneral-1.0.1/setup.py
+drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-07-24 13:56:12.803065 pyfujitsugeneral-1.0.3/
+-rw-r--r--   0 bigmoby    (501) staff       (20)     1102 2023-03-01 12:48:11.000000 pyfujitsugeneral-1.0.3/LICENSE
+-rw-r--r--   0 bigmoby    (501) staff       (20)      655 2023-07-24 13:56:12.803406 pyfujitsugeneral-1.0.3/PKG-INFO
+-rw-r--r--   0 bigmoby    (501) staff       (20)       98 2023-03-01 15:50:34.000000 pyfujitsugeneral-1.0.3/README.md
+drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-07-24 13:56:12.794311 pyfujitsugeneral-1.0.3/pyfujitsugeneral/
+-rw-r--r--   0 bigmoby    (501) staff       (20)      111 2023-03-01 15:43:25.000000 pyfujitsugeneral-1.0.3/pyfujitsugeneral/__init__.py
+-rw-r--r--   0 bigmoby    (501) staff       (20)     7162 2023-03-17 14:33:49.000000 pyfujitsugeneral-1.0.3/pyfujitsugeneral/api.py
+-rw-r--r--   0 bigmoby    (501) staff       (20)    16731 2023-07-24 13:22:53.000000 pyfujitsugeneral-1.0.3/pyfujitsugeneral/splitAC.py
+drwxr-xr-x   0 bigmoby    (501) staff       (20)        0 2023-07-24 13:56:12.802042 pyfujitsugeneral-1.0.3/pyfujitsugeneral.egg-info/
+-rw-r--r--   0 bigmoby    (501) staff       (20)      655 2023-07-24 13:56:12.000000 pyfujitsugeneral-1.0.3/pyfujitsugeneral.egg-info/PKG-INFO
+-rw-r--r--   0 bigmoby    (501) staff       (20)      316 2023-07-24 13:56:12.000000 pyfujitsugeneral-1.0.3/pyfujitsugeneral.egg-info/SOURCES.txt
+-rw-r--r--   0 bigmoby    (501) staff       (20)        1 2023-07-24 13:56:12.000000 pyfujitsugeneral-1.0.3/pyfujitsugeneral.egg-info/dependency_links.txt
+-rw-r--r--   0 bigmoby    (501) staff       (20)       38 2023-07-24 13:56:12.000000 pyfujitsugeneral-1.0.3/pyfujitsugeneral.egg-info/requires.txt
+-rw-r--r--   0 bigmoby    (501) staff       (20)       17 2023-07-24 13:56:12.000000 pyfujitsugeneral-1.0.3/pyfujitsugeneral.egg-info/top_level.txt
+-rw-r--r--   0 bigmoby    (501) staff       (20)       79 2023-07-24 13:56:12.806640 pyfujitsugeneral-1.0.3/setup.cfg
+-rw-r--r--   0 bigmoby    (501) staff       (20)      955 2023-07-24 13:53:14.000000 pyfujitsugeneral-1.0.3/setup.py
```

### Comparing `pyfujitsugeneral-1.0.1/LICENSE` & `pyfujitsugeneral-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfujitsugeneral-1.0.1/PKG-INFO` & `pyfujitsugeneral-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfujitsugeneral
-Version: 1.0.1
+Version: 1.0.3
 Summary: Python Library for interacting with Fujitsu General split air conditioners API
 Home-page: https://github.com/bigmoby/pyfujitsugeneral
 Download-URL: https://github.com/bigmoby/pyfujitsugeneral
 Author: Fabio Mauro, Mehdi Modarressi
 Author-email: bigmoby.pymeianlike@gmail.com
 License: MIT License
 Keywords: Fujitsu General air conditioners
```

### Comparing `pyfujitsugeneral-1.0.1/pyfujitsugeneral/api.py` & `pyfujitsugeneral-1.0.3/pyfujitsugeneral/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,29 +88,29 @@
         response = self._call_api(
             "get",
             self._API_GET_PROPERTIES_URL.format(DSN=dsn),
             access_token=access_token,
         )
         return response.json()
 
-    def _set_device_property(self, propertyCode, value):
+    def _set_device_property(self, propertyCode: int, value: Any) -> Response:
         access_token = self._read_token()
         if not self._check_token_validity(access_token):
             access_token = self._authenticate()
 
         response = self._call_api(
             "post",
             self._API_SET_PROPERTIES_URL.format(property=propertyCode),
             propertyValue=value,
             access_token=access_token,
         )
 
         return response
 
-    def _get_device_property(self, propertyCode):
+    def _get_device_property(self, propertyCode) -> Response:
         access_token = self._read_token()
         if not self._check_token_validity(access_token):
             access_token = self._authenticate()
 
         response = self._call_api(
             "get",
             self._API_SET_PROPERTIES_URL.format(property=propertyCode),
```

### Comparing `pyfujitsugeneral-1.0.1/pyfujitsugeneral/splitAC.py` & `pyfujitsugeneral-1.0.3/pyfujitsugeneral/splitAC.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.powerful_mode = self._properties
         self.min_heat = self._properties  # TODO Missing device setting method
         self.outdoor_low_noise = self._properties  # TODO Missing device setting method
         self.operation_mode = self._properties  # type: ignore
         self.adjust_temperature = self._properties
 
     # Method for getting new (refreshing) properties values
-    def refresh_properties(self):
+    def refresh_properties(self) -> None:
         self._properties = self._api._get_device_properties(self._dsn)
         self.device_name = self._properties
         self.adjust_temperature = self._properties
         self.af_vertical_swing = self._properties
         self.af_vertical_direction = self._properties
         self.af_horizontal_swing = self._properties
         self.af_horizontal_direction = self._properties
@@ -223,14 +223,35 @@
             )
         elif isinstance(properties, int):
             self._api._set_device_property(self.operation_mode["key"], properties)
             self.refresh_properties()
         else:
             raise Exception("Wrong usage of the method!")
 
+    @property # property to get display temperature in degree C
+    def display_temperature_degree(self) -> float | None:
+        data = None
+        if self._display_temperature is not None:
+            data = round(((self._display_temperature["value"] / 100 - 32) / 9 * 5),1)
+        return data
+    
+    @property # property returns display temperature dict in 10 times of degree C
+    def display_temperature(self): 
+        return self._display_temperature(self)
+    
+    @display_temperature.setter
+    def display_temperature(self,properties):
+        if isinstance(properties,(list, tuple)):
+            self._display_temperature = self._get_prop_from_json("display_temperature",properties)
+        elif isinstance(properties,int) or isinstance(properties,float):
+            self._api._set_device_property(self.display_temperature["key"],properties)
+            self.refresh_properties()
+        else:
+            raise Exception("Wrong usage of the method!")
+            
     @property  # property to get temperature in degree C
     def adjust_temperature_degree(self) -> float | None:
         data = None
         if self._adjust_temperature is not None:
             data = round((self._adjust_temperature["value"] / 10), 1)
         return data
 
@@ -328,15 +349,15 @@
             raise Exception("Wrong usage of the method or direction out of range!")
 
     @property
     def af_horizontal_swing(self):
         return self._af_horizontal_swing
 
     @af_horizontal_swing.setter
-    def af_horizontal_swing(self, properties):
+    def af_horizontal_swing(self, properties: Any):
         if isinstance(properties, (list, tuple)):
             self._af_horizontal_swing = self._get_prop_from_json(
                 "af_horizontal_swing", properties
             )
         elif isinstance(properties, int):
             self._api._set_device_property(self.af_horizontal_swing["key"], properties)
             self.refresh_properties()
@@ -344,15 +365,15 @@
             raise Exception("Wrong usage of the method!")
 
     @property
     def af_vertical_direction(self):
         return self._af_vertical_direction
 
     @af_vertical_direction.setter
-    def af_vertical_direction(self, properties):
+    def af_vertical_direction(self, properties: Any) -> None:
         if isinstance(properties, (list, tuple)):
             self._af_vertical_direction = self._get_prop_from_json(
                 "af_vertical_move_step1", properties
             )
         elif isinstance(properties, int):
             self._api._set_device_property(
                 self.af_vertical_direction["key"], properties
@@ -379,15 +400,15 @@
             raise Exception("Wrong usage of the method!")
 
     @property
     def device_name(self) -> dict[str, Any] | None:
         return self._device_name
 
     @device_name.setter
-    def device_name(self, properties):
+    def device_name(self, properties: Any) -> None:
         self._device_name = self._get_prop_from_json("device_name", properties)
 
     @property
     def op_status(self) -> dict[str, Any] | None:
         return self._get_prop_from_json("op_status", self._properties)
 
     def get_op_status_desc(self) -> str | None:
@@ -398,33 +419,31 @@
             data = (
                 DICT_OP_MODE[status] if status in DICT_OP_MODE else f"Unknown {status}"
             )
             return data
         return data
 
     # Get a property history
-    def _get_device_property_history(self, propertyCode):
+    def _get_device_property_history(self, propertyCode: int) -> Any:
         propertyHistory = self._api._get_device_property(propertyCode)
         propertyHistory = propertyHistory.json()
 
         return propertyHistory
 
     # Translate the operation mode to descriptive values and reverse
     def _operation_mode_translate(self, operation_mode: Any) -> Any:
 
         DICT_OPERATION_MODE = {
             "off": 0,
-            "unknown": 1,
-            "auto": 2,
-            "cool": 3,
+            "heat": 1,
+            "cool": 2,
+            "auto": 3,
             "dry": 4,
             "fan_only": 5,
-            "heat": 6,
             0: "off",
-            1: "unknown",
-            2: "auto",
-            3: "cool",
+            1: "heat",
+            2: "cool",
+            3: "auto",
             4: "dry",
             5: "fan_only",
-            6: "heat",
         }
         return DICT_OPERATION_MODE[operation_mode]
```

### Comparing `pyfujitsugeneral-1.0.1/pyfujitsugeneral.egg-info/PKG-INFO` & `pyfujitsugeneral-1.0.3/pyfujitsugeneral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfujitsugeneral
-Version: 1.0.1
+Version: 1.0.3
 Summary: Python Library for interacting with Fujitsu General split air conditioners API
 Home-page: https://github.com/bigmoby/pyfujitsugeneral
 Download-URL: https://github.com/bigmoby/pyfujitsugeneral
 Author: Fabio Mauro, Mehdi Modarressi
 Author-email: bigmoby.pymeianlike@gmail.com
 License: MIT License
 Keywords: Fujitsu General air conditioners
```

### Comparing `pyfujitsugeneral-1.0.1/setup.py` & `pyfujitsugeneral-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "1.0.1"
+__version__ = "1.0.3"
 
 setup(
     name="pyfujitsugeneral",
     py_modules=["pyfujitsugeneral"],
     version=__version__,
     description="Python Library for interacting with Fujitsu General split air conditioners API",
     long_description="Python Library for interacting with Fujitsu General split air conditioners API",
```

