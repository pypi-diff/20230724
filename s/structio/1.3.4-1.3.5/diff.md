# Comparing `tmp/structio-1.3.4.tar.gz` & `tmp/structio-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.3.4.tar", last modified: Sat Jul 15 00:11:42 2023, max compression
+gzip compressed data, was "structio-1.3.5.tar", last modified: Mon Jul 24 14:03:38 2023, max compression
```

## Comparing `structio-1.3.4.tar` & `structio-1.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:42.979097 structio-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-07-15 00:11:42.979097 structio-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-07-15 00:11:23.000000 structio-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-15 00:11:23.000000 structio-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 00:11:42.979097 structio-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:42.979097 structio-1.3.4/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-07-15 00:11:42.000000 structio-1.3.4/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-15 00:11:42.000000 structio-1.3.4/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:11:42.000000 structio-1.3.4/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 00:11:42.000000 structio-1.3.4/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-07-15 00:11:23.000000 structio-1.3.4/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:38.704007 structio-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-24 14:03:38.704007 structio-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-07-24 14:03:17.000000 structio-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 14:03:17.000000 structio-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:03:38.704007 structio-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:03:38.704007 structio-1.3.5/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-24 14:03:38.000000 structio-1.3.5/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 14:03:38.000000 structio-1.3.5/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:03:38.000000 structio-1.3.5/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 14:03:38.000000 structio-1.3.5/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-07-24 14:03:17.000000 structio-1.3.5/structio.py
```

### Comparing `structio-1.3.4/PKG-INFO` & `structio-1.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.4
+Version: 1.3.5
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -142,27 +142,23 @@
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
 **buffer**: the current content of the object (read only).
 
-**pos**: the current position in the object.
-
-**end**: the length of the object (read only).
-
 **endian**: the default endian that would be used by the object (read only).
 
 **encoding**: the default encoding used by string methods (read only).
 
 **errors**: the default error handling behavior when encoding or decoding strings (read only).
 
 ### Methods
 
-**StructIO(b=b'', struct=structio._struct)**
+**StructIO(b=b'', struct=_struct)**
 
 Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
```

### Comparing `structio-1.3.4/README.md` & `structio-1.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -134,27 +134,23 @@
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
 **buffer**: the current content of the object (read only).
 
-**pos**: the current position in the object.
-
-**end**: the length of the object (read only).
-
 **endian**: the default endian that would be used by the object (read only).
 
 **encoding**: the default encoding used by string methods (read only).
 
 **errors**: the default error handling behavior when encoding or decoding strings (read only).
 
 ### Methods
 
-**StructIO(b=b'', struct=structio._struct)**
+**StructIO(b=b'', struct=_struct)**
 
 Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
```

### Comparing `structio-1.3.4/structio.egg-info/PKG-INFO` & `structio-1.3.5/structio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.4
+Version: 1.3.5
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -142,27 +142,23 @@
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
 **buffer**: the current content of the object (read only).
 
-**pos**: the current position in the object.
-
-**end**: the length of the object (read only).
-
 **endian**: the default endian that would be used by the object (read only).
 
 **encoding**: the default encoding used by string methods (read only).
 
 **errors**: the default error handling behavior when encoding or decoding strings (read only).
 
 ### Methods
 
-**StructIO(b=b'', struct=structio._struct)**
+**StructIO(b=b'', struct=_struct)**
 
 Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
```

### Comparing `structio-1.3.4/structio.py` & `structio-1.3.5/structio.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,26 +139,14 @@
         self._struct = struct
         
     @property
     def buffer(self):
         return self.getvalue()
         
     @property
-    def pos(self):
-        return self.tell()
-        
-    @pos.setter
-    def pos(self, value):
-        self.seek(value)
-        
-    @property
-    def end(self):
-        return len(self.getvalue())
-        
-    @property
     def endian(self):
         return self._struct.endian
         
     @property
     def encoding(self):
         return self._struct.encoding
```

