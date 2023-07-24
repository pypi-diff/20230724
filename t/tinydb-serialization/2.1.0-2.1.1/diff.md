# Comparing `tmp/tinydb-serialization-2.1.0.tar.gz` & `tmp/tinydb_serialization-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinydb-serialization-2.1.0.tar", last modified: Sat Jan 23 15:25:14 2021, max compression
+gzip compressed data, was "tinydb_serialization-2.1.1.tar", max compression
```

## Comparing `tinydb-serialization-2.1.0.tar` & `tinydb_serialization-2.1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1082 2021-01-23 15:24:52.984241 tinydb-serialization-2.1.0/LICENSE
--rw-r--r--   0        0        0     3719 2021-01-23 15:24:52.984241 tinydb-serialization-2.1.0/README.rst
--rw-r--r--   0        0        0     1122 2021-01-23 15:24:52.984241 tinydb-serialization-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     5741 2021-01-23 15:24:52.984241 tinydb-serialization-2.1.0/tinydb_serialization/__init__.py
--rw-r--r--   0        0        0      303 2021-01-23 15:24:52.984241 tinydb-serialization-2.1.0/tinydb_serialization/serializers.py
--rw-r--r--   0        0        0     4500 2021-01-23 15:25:14.566383 tinydb-serialization-2.1.0/setup.py
--rw-r--r--   0        0        0     4792 2021-01-23 15:25:14.566774 tinydb-serialization-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-24 19:22:21.242161 tinydb_serialization-2.1.1/LICENSE
+-rw-r--r--   0        0        0     4412 2023-07-24 19:22:21.242161 tinydb_serialization-2.1.1/README.rst
+-rw-r--r--   0        0        0     1147 2023-07-24 19:22:21.242161 tinydb_serialization-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5823 2023-07-24 19:22:21.242161 tinydb_serialization-2.1.1/tinydb_serialization/__init__.py
+-rw-r--r--   0        0        0      303 2023-07-24 19:22:21.242161 tinydb_serialization-2.1.1/tinydb_serialization/serializers.py
+-rw-r--r--   0        0        0     5437 1970-01-01 00:00:00.000000 tinydb_serialization-2.1.1/PKG-INFO
```

### Comparing `tinydb-serialization-2.1.0/LICENSE` & `tinydb_serialization-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinydb-serialization-2.1.0/README.rst` & `tinydb_serialization-2.1.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 To use a serializer, create a ``SerializationMiddleware`` instance with
 the storage class you want to use and register the serializers you want
 to use. Then you pass the middleware instance as the storage to TinyDB:
 
 .. code-block:: python
 
     >>> from tinydb import TinyDB, Query
+    >>> from tinydb.storages import JSONStorage
     >>> from tinydb_serialization import SerializationMiddleware
     >>> from tinydb_serialization.serializers import DateTimeSerializer
     >>>
     >>> from datetime import datetime
     >>>
     >>> serialization = SerializationMiddleware(JSONStorage)
     >>> serialization.register_serializer(DateTimeSerializer(), 'TinyDate')
@@ -32,14 +33,20 @@
     >>> db.all()
     [{'date': datetime.datetime(2000, 1, 1, 12, 0)}]
     >>> query = Query()
     >>> db.insert({'date': datetime(2010, 1, 1, 12, 0, 0)})
     >>> db.search(query.date > datetime(2005, 1, 1))
     [{'date': datetime.datetime(2010, 1, 1, 12, 0)}]
 
+
+**Important:** A ``SerializationMiddleware`` instance always wraps a database's storage.
+This means that the ``SerializationMiddleware`` instance **cannot** be shared
+between multiple ``TinyDB`` instances as they would use the same underlying storage
+instance and thus share all data between both instances.
+
 Provided Serializers
 --------------------
 
 - ``tinydb_serialization.serializers.DateTimeSerializer``: serializes ``datetime`` objects
   as ISO 8601 formatted strings
 
 Creating Custom Serializers
@@ -62,14 +69,21 @@
         def decode(self, s):
             return datetime.fromisoformat(s)
 
 
 Changelog
 *********
 
+**v2.1.1** (2023-07-24)
+-----------------------
+
+- Fix VSCode Pylance type error (see `pull request #14 <https://github.com/msiemens/tinydb-serialization/pull/14>`_)
+- Add support for storages that encode as binary strings (see `pull request #17 <https://github.com/msiemens/tinydb-serialization/pull/17>`_)
+- Drop Python 3.7 support
+
 **v2.1.0** (2021-01-23)
 -----------------------
 
 - Include the ``DateTimeSerializer`` in this package (see `issue #10 <https://github.com/msiemens/tinydb-serialization/pull/10>`_)
 - Drop Python 3.6 support (as 3.7 is needed for date parsing)
 
 **v2.0.0** (2020-05-26)
```

### Comparing `tinydb-serialization-2.1.0/tinydb_serialization/__init__.py` & `tinydb_serialization-2.1.1/tinydb_serialization/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,42 +8,39 @@
 itervalues = getattr(dict, 'itervalues', dict.values)
 
 
 class Serializer(ABC):
     """
     The abstract base class for Serializers.
     Allows TinyDB to handle arbitrary objects by running them through a list
-    of registerd serializers.
+    of registered serializers.
     Every serializer has to tell which class it can handle.
     """
 
-    @property
-    @abstractmethod
-    def OBJ_CLASS(self):
-        raise NotImplementedError('To be overriden!')
+    OBJ_CLASS: object
 
     @abstractmethod
     def encode(self, obj):
         """
         Encode an object.
         :param obj:
         :return:
         :rtype: str
         """
-        raise NotImplementedError('To be overriden!')
+        raise NotImplementedError('To be overridden!')
 
     @abstractmethod
     def decode(self, s):
         """
         Decode an object.
         :param s:
         :type s: str
         :return:
         """
-        raise NotImplementedError('To be overriden!')
+        raise NotImplementedError('To be overridden!')
 
 
 def _enumerate_element(element):
     """
     Make an element enumerable.
 
     For dicts: return an iterator over the items (key, value).
@@ -61,16 +58,19 @@
     Recursively decode an element.
 
     Takes into account elements in nested dicts, lists and tuples
     """
 
     for key, value in _enumerate_element(element):
         try:
-            if value.startswith(tag):
-                encoded = value[len(tag):]
+            typed_tag = tag
+            if type(value) == bytes:
+                typed_tag = tag.encode()
+            if value.startswith(typed_tag):
+                encoded = value[len(typed_tag):]
                 element[key] = serializer.decode(encoded)
 
         except AttributeError:
             # Not a string
             if isinstance(value, (dict, list, tuple)):
                 _decode_deep(value, serializer, tag)
 
@@ -81,34 +81,34 @@
 
     Takes into account elements in nested dicts, lists and tuples
     """
 
     for key, value in _enumerate_element(element):
         if isinstance(value, obj_class):
             encoded = serializer.encode(value)
-            element[key] = tag + encoded
+            element[key] = (tag if type(encoded) == str else tag.encode()) + encoded
 
         elif isinstance(value, (dict, list, tuple)):
             _encode_deep(value, serializer, tag, obj_class)
 
 
-def has_encodable(element, obj_class):
+def has_encodeable(element, obj_class):
     """
-    Check whether the element in question has an encodable item.
+    Check whether the element in question has an encodeable item.
     """
 
-    found_encodable = False
+    found_encodeable = False
 
     for key, value in _enumerate_element(element):
         if isinstance(value, (dict, list, tuple)):
-            found_encodable |= has_encodable(value, obj_class)
+            found_encodeable |= has_encodeable(value, obj_class)
         else:
-            found_encodable |= isinstance(value, obj_class)
+            found_encodeable |= isinstance(value, obj_class)
 
-    return found_encodable
+    return found_encodeable
 
 
 class SerializationMiddleware(Middleware):
     """
     Provide custom serialization for TinyDB.
     This middleware allows users of TinyDB to register custom serializations.
     The serialized data will be passed to the wrapped storage and data that
@@ -170,15 +170,15 @@
             tag = '{{{0}}}:'.format(serializer_name)
 
             for table_name in data:
                 table = data[table_name]
 
                 for eid in table:
                     # Before writing, copy data if we haven't already.
-                    if not data_copied and has_encodable(data[table_name][eid],
+                    if not data_copied and has_encodeable(data[table_name][eid],
                                                          obj_class):
                         data = deepcopy(data)
                         data_copied = True
 
                     item = data[table_name][eid]
                     _encode_deep(item, serializer, tag, obj_class)
```

### Comparing `tinydb-serialization-2.1.0/PKG-INFO` & `tinydb_serialization-2.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: tinydb-serialization
-Version: 2.1.0
+Version: 2.1.1
 Summary: Serialization for objects that TinyDB otherwise couldn't handle
 License: MIT
 Keywords: database,nosql
 Author: Markus Siemens
 Author-email: markus@m-siemens.de
-Requires-Python: >=3.5,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Utilities
 Requires-Dist: tinydb (>=4.0,<5.0)
 Description-Content-Type: text/x-rst
 
@@ -42,14 +41,15 @@
 To use a serializer, create a ``SerializationMiddleware`` instance with
 the storage class you want to use and register the serializers you want
 to use. Then you pass the middleware instance as the storage to TinyDB:
 
 .. code-block:: python
 
     >>> from tinydb import TinyDB, Query
+    >>> from tinydb.storages import JSONStorage
     >>> from tinydb_serialization import SerializationMiddleware
     >>> from tinydb_serialization.serializers import DateTimeSerializer
     >>>
     >>> from datetime import datetime
     >>>
     >>> serialization = SerializationMiddleware(JSONStorage)
     >>> serialization.register_serializer(DateTimeSerializer(), 'TinyDate')
@@ -59,14 +59,20 @@
     >>> db.all()
     [{'date': datetime.datetime(2000, 1, 1, 12, 0)}]
     >>> query = Query()
     >>> db.insert({'date': datetime(2010, 1, 1, 12, 0, 0)})
     >>> db.search(query.date > datetime(2005, 1, 1))
     [{'date': datetime.datetime(2010, 1, 1, 12, 0)}]
 
+
+**Important:** A ``SerializationMiddleware`` instance always wraps a database's storage.
+This means that the ``SerializationMiddleware`` instance **cannot** be shared
+between multiple ``TinyDB`` instances as they would use the same underlying storage
+instance and thus share all data between both instances.
+
 Provided Serializers
 --------------------
 
 - ``tinydb_serialization.serializers.DateTimeSerializer``: serializes ``datetime`` objects
   as ISO 8601 formatted strings
 
 Creating Custom Serializers
@@ -89,14 +95,21 @@
         def decode(self, s):
             return datetime.fromisoformat(s)
 
 
 Changelog
 *********
 
+**v2.1.1** (2023-07-24)
+-----------------------
+
+- Fix VSCode Pylance type error (see `pull request #14 <https://github.com/msiemens/tinydb-serialization/pull/14>`_)
+- Add support for storages that encode as binary strings (see `pull request #17 <https://github.com/msiemens/tinydb-serialization/pull/17>`_)
+- Drop Python 3.7 support
+
 **v2.1.0** (2021-01-23)
 -----------------------
 
 - Include the ``DateTimeSerializer`` in this package (see `issue #10 <https://github.com/msiemens/tinydb-serialization/pull/10>`_)
 - Drop Python 3.6 support (as 3.7 is needed for date parsing)
 
 **v2.0.0** (2020-05-26)
```

