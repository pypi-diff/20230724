# Comparing `tmp/indipydriver-1.0.0.tar.gz` & `tmp/indipydriver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-1.0.0.tar", last modified: Sun Jul 16 14:57:36 2023, max compression
+gzip compressed data, was "indipydriver-1.0.1.tar", last modified: Mon Jul 24 21:23:01 2023, max compression
```

## Comparing `indipydriver-1.0.0.tar` & `indipydriver-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-1.0.0/LICENSE
--rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-1.0.0/README.md
--rw-r--r--   0        0        0      573 2023-07-16 14:51:11.000000 indipydriver-1.0.0/indipydriver/__init__.py
--rw-r--r--   0        0        0    17081 2023-07-09 09:46:38.000000 indipydriver-1.0.0/indipydriver/comms.py
--rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-1.0.0/indipydriver/events.py
--rw-r--r--   0        0        0    21510 2023-07-13 19:40:55.000000 indipydriver-1.0.0/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    10816 2023-07-13 20:27:03.000000 indipydriver-1.0.0/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    11759 2023-07-09 08:25:23.000000 indipydriver-1.0.0/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    42713 2023-07-08 21:53:53.000000 indipydriver-1.0.0/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2023-07-16 14:50:33.000000 indipydriver-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-1.0.1/README.md
+-rw-r--r--   0        0        0      573 2023-07-24 21:14:10.000000 indipydriver-1.0.1/indipydriver/__init__.py
+-rw-r--r--   0        0        0    17081 2023-07-09 09:46:38.000000 indipydriver-1.0.1/indipydriver/comms.py
+-rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-1.0.1/indipydriver/events.py
+-rw-r--r--   0        0        0    21548 2023-07-24 20:31:23.000000 indipydriver-1.0.1/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    10816 2023-07-13 20:27:03.000000 indipydriver-1.0.1/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    11759 2023-07-24 20:59:57.000000 indipydriver-1.0.1/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    42713 2023-07-08 21:53:53.000000 indipydriver-1.0.1/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2023-07-24 21:13:56.000000 indipydriver-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-1.0.1/PKG-INFO
```

### Comparing `indipydriver-1.0.0/LICENSE` & `indipydriver-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.0/README.md` & `indipydriver-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.0/indipydriver/__init__.py` & `indipydriver-1.0.1/indipydriver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "1.0.0"
+version = "1.0.1"
```

### Comparing `indipydriver-1.0.0/indipydriver/comms.py` & `indipydriver-1.0.1/indipydriver/comms.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.0/indipydriver/events.py` & `indipydriver-1.0.1/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.0/indipydriver/ipydriver.py` & `indipydriver-1.0.1/indipydriver/ipydriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,14 +255,15 @@
         await self.send(xmldata)
 
     async def send_getProperties(self, devicename=None, vectorname=None):
         """Sends a getProperties request - which is used to snoop data from other devices
            on the network, if devicename given, it must not be a device of this driver as
            the point of this is to snoop on remote devices."""
         xmldata = ET.Element('getProperties')
+        xmldata.set("version", "1.7")
         if devicename is None:
             await self.send(xmldata)
             self.snoopall = True
             return
         if devicename in self.devices:
             self._reporterror("Cannot snoop on a device already controlled by this driver")
             return
```

### Comparing `indipydriver-1.0.0/indipydriver/ipyserver.py` & `indipydriver-1.0.1/indipydriver/ipyserver.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.0/indipydriver/propertymembers.py` & `indipydriver-1.0.1/indipydriver/propertymembers.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
         if not value:
             raise ValueError(f"The BLOBMember {self.name} value cannot be empty")
         self._membervalue = value
 
 
     def defblob(self):
         """Returns a defBlob, does not contain a membervalue"""
-        xmldata = ET.Element('defBlob')
+        xmldata = ET.Element('defBLOB')
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         return xmldata
 
 
     def oneblob(self):
         """Returns xml of a oneBLOB"""
```

### Comparing `indipydriver-1.0.0/indipydriver/propertyvectors.py` & `indipydriver-1.0.1/indipydriver/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.0/pyproject.toml` & `indipydriver-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "1.0.0"
+version = "1.0.1"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-1.0.0/PKG-INFO` & `indipydriver-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

