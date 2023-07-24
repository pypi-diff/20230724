# Comparing `tmp/carica-1.3.4.tar.gz` & `tmp/carica-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carica-1.3.4.tar", last modified: Sun May 21 21:55:47 2023, max compression
+gzip compressed data, was "carica-1.3.5.tar", last modified: Mon Jul 24 06:07:44 2023, max compression
```

## Comparing `carica-1.3.4.tar` & `carica-1.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 21:55:29.000000 carica-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15974 2023-05-21 21:55:47.100978 carica-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-05-21 21:55:29.000000 carica-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-21 21:55:29.000000 carica-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-21 21:55:47.104978 carica-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/carica/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27967 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/carica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/carica/interface/
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/interface/Serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/carica/models/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20387 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/models/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/models/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/typeChecking.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/carica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15974 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:07:44.243143 carica-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 06:07:26.000000 carica-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-07-24 06:07:44.243143 carica-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-24 06:07:26.000000 carica-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-24 06:07:26.000000 carica-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-24 06:07:44.243143 carica-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:07:44.239143 carica-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:07:44.239143 carica-1.3.5/src/carica/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27967 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/carica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:07:44.243143 carica-1.3.5/src/carica/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/interface/Serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:07:44.243143 carica-1.3.5/src/carica/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20387 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/models/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/models/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/typeChecking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-24 06:07:26.000000 carica-1.3.5/src/carica/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:07:44.239143 carica-1.3.5/src/carica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-07-24 06:07:44.000000 carica-1.3.5/src/carica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-24 06:07:44.000000 carica-1.3.5/src/carica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:07:44.000000 carica-1.3.5/src/carica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 06:07:44.000000 carica-1.3.5/src/carica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 06:07:44.000000 carica-1.3.5/src/carica.egg-info/top_level.txt
```

### Comparing `carica-1.3.4/LICENSE` & `carica-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carica-1.3.4/PKG-INFO` & `carica-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carica
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python module that populates variables from TOML config documents, and generates config documents from python variables.
 Home-page: https://github.com/Trimatix/carica
 Author: Jasper Law
 Author-email: trimatix.music@gmail.com
 Project-URL: Bug Tracker, https://github.com/Trimatix/carica/issues
 Keywords: config,cfg,python,toml,generate,auto-generate,orm
 Classifier: Programming Language :: Python :: 3.8
@@ -47,18 +47,18 @@
       alt="Pypi package version"
   /></a>
   <a href="https://pypi.org/project/Carica"
     ><img
       src="https://img.shields.io/pypi/pyversions/Carica.svg"
       alt="Minimum supported Python version"
   /></a>
-  <a href="https://github.com/Trimatix/Carica/blob/master/LICENSE"
+  <a href="https://pepy.tech/project/carica"
     ><img
-      src="https://img.shields.io/github/license/Trimatix/Carica.svg"
-      alt="License"
+      src="https://static.pepy.tech/badge/carica"
+      alt="Total PyPi Downloads"
 </p>
 <p align="center">
   <a href="https://sonarcloud.io/dashboard?id=Trimatix_Carica"
     ><img
       src="https://sonarcloud.io/api/project_badges/measure?project=Trimatix_Carica&metric=bugs"
       alt="SonarCloud bugs analysis"
   /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carica Version: 1.3.4 Summary: Python module that
+Metadata-Version: 2.1 Name: carica Version: 1.3.5 Summary: Python module that
 populates variables from TOML config documents, and generates config documents
 from python variables. Home-page: https://github.com/Trimatix/carica Author:
 Jasper Law Author-email: trimatix.music@gmail.com Project-URL: Bug Tracker,
 https://github.com/Trimatix/carica/issues Keywords:
 config,cfg,python,toml,generate,auto-generate,orm Classifier: Programming
 Language :: Python :: 3.8 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Requires-
```

### Comparing `carica-1.3.4/README.md` & `carica-1.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
       alt="Pypi package version"
   /></a>
   <a href="https://pypi.org/project/Carica"
     ><img
       src="https://img.shields.io/pypi/pyversions/Carica.svg"
       alt="Minimum supported Python version"
   /></a>
-  <a href="https://github.com/Trimatix/Carica/blob/master/LICENSE"
+  <a href="https://pepy.tech/project/carica"
     ><img
-      src="https://img.shields.io/github/license/Trimatix/Carica.svg"
-      alt="License"
+      src="https://static.pepy.tech/badge/carica"
+      alt="Total PyPi Downloads"
 </p>
 <p align="center">
   <a href="https://sonarcloud.io/dashboard?id=Trimatix_Carica"
     ><img
       src="https://sonarcloud.io/api/project_badges/measure?project=Trimatix_Carica&metric=bugs"
       alt="SonarCloud bugs analysis"
   /></a>
```

### Comparing `carica-1.3.4/setup.cfg` & `carica-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `carica-1.3.4/src/carica/carica.py` & `carica-1.3.5/src/carica/carica.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.4/src/carica/exceptions.py` & `carica-1.3.5/src/carica/exceptions.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.4/src/carica/interface/Serializable.py` & `carica-1.3.5/src/carica/interface/Serializable.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,14 @@
 
 # All types which are themselves primative, or can be serialized into primative types, as a shallow set
 serializableTypes: Tuple[Type] = tuple(t for t in primativeTypes) + (SerializableType,)
 
 TClass = TypeVar("TClass")
 TSerialized = TypeVar("TSerialized", bound=PrimativeType)
 
-class SerializesToType(SerializableType, Generic[TSerialized]):
+class SerializesToType(SerializableType, Generic[TSerialized], Protocol):
     def serialize(self, **kwargs) -> TSerialized: ...
 
     @classmethod
     def deserialize(cls: Type[TClass], data: TSerialized, **kwargs) -> TClass: ...
 
 SerializesToDict = SerializesToType[Mapping[str, PrimativeType]]
```

### Comparing `carica-1.3.4/src/carica/models/dataclasses.py` & `carica-1.3.5/src/carica/models/dataclasses.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.4/src/carica/models/path.py` & `carica-1.3.5/src/carica/models/path.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.4/src/carica/models/timedelta.py` & `carica-1.3.5/src/carica/models/timedelta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,53 @@
-from typing import Dict, TypeVar, Type
-from carica.interface.Serializable import ISerializable, PrimativeType
+from typing import Dict, TypeVar, Type, TypedDict
+
+from carica.interface.Serializable import SerializesToType
 from datetime import timedelta
 
 TSelf = TypeVar("TSelf", bound="SerializableTimedelta")
 
-class SerializableTimedelta(ISerializable, timedelta):
+class SerializedTimedelta(TypedDict):
+    days: float
+    seconds: float
+    microseconds: float
+    milliseconds: float
+    minutes: float
+    hours: float
+    weeks: float
+
+
+class SerializableTimedelta(SerializesToType[SerializedTimedelta], timedelta):
     """A serializable version of `datetime.timedelta`. For `datetime.datetime`, no extra handling is needed,
     as datetime is considered a primitive type by TOML.
     """
     @classmethod
     def fromTimedelta(cls, td: timedelta):
         """Create a new `SerializableTimedelta` from an existing `datetime.timedelta`.
 
         :param timedelta td: The timedelta to duplicate
         """
         return cls(days=td.days, seconds=td.seconds, microseconds=td.microseconds)
 
 
-    def serialize(self, **kwargs) -> Dict[str, int]:
+    def serialize(self, **kwargs) -> SerializedTimedelta:
         """Serialize this timedelta into the simplest representation possible - using the largest amounts of the largest
         units that will fit into this timedelta.
 
         :return: A dictionary containing all units, each possibly zero, to represent this timedelta.
         :rtype: Dict[str, int]
         """
-        data = {}
+        data: SerializedTimedelta = {
+            "weeks": 0,
+            "days": 0,
+            "hours": 0,
+            "minutes": 0,
+            "seconds": 0,
+            "milliseconds": 0,
+            "microseconds": 0
+        }
 
         data["weeks"] = 0 if self.days < 7 else self.days // 7
         data["days"] = self.days - data["weeks"] * 7
 
         data["hours"] = 0 if self.seconds < 3600 else self.seconds // 3600
         seconds = self.seconds - data["hours"] * 3600
         data["minutes"] = 0 if seconds < 60 else seconds // 60
@@ -37,11 +56,11 @@
         data["milliseconds"] = 0 if self.microseconds < 1000 else self.microseconds // 1000
         data["microseconds"] = self.microseconds - data["milliseconds"] * 1000
             
         return data
 
 
     @classmethod
-    def deserialize(cls: Type[TSelf], data: PrimativeType, **kwargs) -> TSelf:
+    def deserialize(cls: Type[TSelf], data: SerializedTimedelta, **kwargs) -> TSelf:
         if not isinstance(data, dict):
             raise TypeError(f"Invalid serialized {cls.__name__}: {data}")
         return cls(**data)
```

### Comparing `carica-1.3.4/src/carica/typeChecking.py` & `carica-1.3.5/src/carica/typeChecking.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.4/src/carica/util.py` & `carica-1.3.5/src/carica/util.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.4/src/carica.egg-info/PKG-INFO` & `carica-1.3.5/src/carica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carica
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python module that populates variables from TOML config documents, and generates config documents from python variables.
 Home-page: https://github.com/Trimatix/carica
 Author: Jasper Law
 Author-email: trimatix.music@gmail.com
 Project-URL: Bug Tracker, https://github.com/Trimatix/carica/issues
 Keywords: config,cfg,python,toml,generate,auto-generate,orm
 Classifier: Programming Language :: Python :: 3.8
@@ -47,18 +47,18 @@
       alt="Pypi package version"
   /></a>
   <a href="https://pypi.org/project/Carica"
     ><img
       src="https://img.shields.io/pypi/pyversions/Carica.svg"
       alt="Minimum supported Python version"
   /></a>
-  <a href="https://github.com/Trimatix/Carica/blob/master/LICENSE"
+  <a href="https://pepy.tech/project/carica"
     ><img
-      src="https://img.shields.io/github/license/Trimatix/Carica.svg"
-      alt="License"
+      src="https://static.pepy.tech/badge/carica"
+      alt="Total PyPi Downloads"
 </p>
 <p align="center">
   <a href="https://sonarcloud.io/dashboard?id=Trimatix_Carica"
     ><img
       src="https://sonarcloud.io/api/project_badges/measure?project=Trimatix_Carica&metric=bugs"
       alt="SonarCloud bugs analysis"
   /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carica Version: 1.3.4 Summary: Python module that
+Metadata-Version: 2.1 Name: carica Version: 1.3.5 Summary: Python module that
 populates variables from TOML config documents, and generates config documents
 from python variables. Home-page: https://github.com/Trimatix/carica Author:
 Jasper Law Author-email: trimatix.music@gmail.com Project-URL: Bug Tracker,
 https://github.com/Trimatix/carica/issues Keywords:
 config,cfg,python,toml,generate,auto-generate,orm Classifier: Programming
 Language :: Python :: 3.8 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Requires-
```

### Comparing `carica-1.3.4/src/carica.egg-info/SOURCES.txt` & `carica-1.3.5/src/carica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

