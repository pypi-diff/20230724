# Comparing `tmp/wsjtx_srv-0.4.tar.gz` & `tmp/wsjtx_srv-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsjtx_srv-0.4.tar", last modified: Sun May 14 17:55:13 2023, max compression
+gzip compressed data, was "wsjtx_srv-0.5.tar", last modified: Mon Jul 24 09:48:40 2023, max compression
```

## Comparing `wsjtx_srv-0.4.tar` & `wsjtx_srv-0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-14 17:55:13.011271 wsjtx_srv-0.4/
--rw-r--r--   0 ralf      (1000) priv      (1011)       39 2021-09-13 11:36:52.000000 wsjtx_srv-0.4/MANIFEST.in
--rw-r--r--   0 ralf      (1000) priv      (1011)     2579 2023-05-14 17:55:13.007271 wsjtx_srv-0.4/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     8175 2023-05-14 17:54:25.000000 wsjtx_srv-0.4/README.html
--rw-r--r--   0 ralf      (1000) priv      (1011)     1507 2023-04-23 07:21:15.000000 wsjtx_srv-0.4/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-14 17:55:12.967271 wsjtx_srv-0.4/bin/
--rwxr-xr-x   0 ralf      (1000) priv      (1011)      979 2021-10-26 11:43:05.000000 wsjtx_srv-0.4/bin/wbf
--rwxr-xr-x   0 ralf      (1000) priv      (1011)       56 2021-09-13 11:37:43.000000 wsjtx_srv-0.4/bin/wsjtx-srv
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-14 17:55:13.011271 wsjtx_srv-0.4/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2991 2023-05-14 17:53:55.000000 wsjtx_srv-0.4/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-14 17:55:12.979271 wsjtx_srv-0.4/wsjtx_srv/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-14 17:54:25.000000 wsjtx_srv-0.4/wsjtx_srv/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)       21 2021-09-13 11:36:52.000000 wsjtx_srv-0.4/wsjtx_srv/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    45636 2023-04-23 07:17:49.000000 wsjtx_srv-0.4/wsjtx_srv/wsjtx.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-14 17:55:13.003271 wsjtx_srv-0.4/wsjtx_srv.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)     2579 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      291 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       16 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       10 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/top_level.txt
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-24 09:48:40.324954 wsjtx_srv-0.5/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1575 2023-07-24 09:42:34.000000 wsjtx_srv-0.5/LICENSE
+-rw-r--r--   0 ralf      (1000) priv      (1011)       39 2021-09-13 11:36:52.000000 wsjtx_srv-0.5/MANIFEST.in
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2679 2023-07-24 09:48:40.324954 wsjtx_srv-0.5/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     8429 2023-07-24 09:48:37.000000 wsjtx_srv-0.5/README.html
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1685 2023-07-24 09:45:02.000000 wsjtx_srv-0.5/README.rst
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2902 2023-07-24 09:43:48.000000 wsjtx_srv-0.5/pyproject.toml
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-07-24 09:48:40.328954 wsjtx_srv-0.5/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     3208 2023-07-24 09:41:53.000000 wsjtx_srv-0.5/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-24 09:48:40.300954 wsjtx_srv-0.5/wsjtx_srv/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-07-24 09:48:37.000000 wsjtx_srv-0.5/wsjtx_srv/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)       21 2023-06-12 15:59:31.000000 wsjtx_srv-0.5/wsjtx_srv/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    47925 2023-06-13 05:30:57.000000 wsjtx_srv-0.5/wsjtx_srv/wsjtx.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-07-24 09:48:40.320954 wsjtx_srv-0.5/wsjtx_srv.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2679 2023-07-24 09:48:40.000000 wsjtx_srv-0.5/wsjtx_srv.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      328 2023-07-24 09:48:40.000000 wsjtx_srv-0.5/wsjtx_srv.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-07-24 09:48:40.000000 wsjtx_srv-0.5/wsjtx_srv.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       77 2023-07-24 09:48:40.000000 wsjtx_srv-0.5/wsjtx_srv.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       16 2023-07-24 09:48:40.000000 wsjtx_srv-0.5/wsjtx_srv.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       10 2023-07-24 09:48:40.000000 wsjtx_srv-0.5/wsjtx_srv.egg-info/top_level.txt
```

### Comparing `wsjtx_srv-0.4/PKG-INFO` & `wsjtx_srv-0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 Metadata-Version: 2.1
 Name: wsjtx_srv
-Version: 0.4
+Version: 0.5
 Summary: Library implementation of WSJTX companion program
 Home-page: https://github.com/schlatterbeck/wsjtx-srv
 Author: Ralf Schlatterbeck
-Author-email: rsc@runtux.com
+Author-email: Ralf Schlatterbeck <rsc@runtux.com>
 License: BSD License
-Description: wsjtx-srv: Library for WSJT-X server implementation
-        ===================================================
-        
-        :Author: Ralf Schlatterbeck <rsc@runtux.com>
-        
-        This implements a simple UDP server that binds to the WSJT-X_ UDP message
-        protocol port. It also provides everything for parsing and/or generating
-        WSJT-X_ telegrams.
-        
-        By default calling ``wsjtx-srv`` will provide a simple server that
-        colors all callsigns not in the ADIF file for the current band. It uses
-        the ADIF logfile from WSJT-X_ with a default path to that file. You can
-        specify the correct path for your installation either via
-        command-line (call ``wsjtx-srv`` with the ``--help`` option) or in the
-        environment variable ``WBF_PATH``. It has also an implementation that
-        looks up DXCC-entities in my log database, but only those that have been
-        confirmed via LOTW.
-        
-        The implementation of ``wsjtx-srv`` should give a rough idea of how to use
-        this in your own projects.
-        
-        There is a companion-program ``wbf`` standing for *worked before* that
-        takes a number of callsigns on the command-line and tells you the worked
-        before status.
-        
-        .. _WSJT-X: https://physics.princeton.edu/pulsar/k1jt/wsjtx.html
-        
-        Changes
-        -------
-        
-        Version 0.3: Small fixes
-        
-        - Compatibility with older protocol versions, thanks to Sampo Savolainen
-          for the patch
-        - Fix band lookup if no QSO on band
-        
-        Version 0.2: Fix setup.py install_requires
-        
-        Version 0.1: Initial implementation
-        
-        - Implement serialization and deserialization of WSJT-X_ telegrams and a
-          simple server
-        - First Release
-        
-        
+Project-URL: Homepage, https://github.com/schlatterbeck/wsjtx-srv
+Project-URL: Bug Tracker, https://github.com/schlatterbeck/wsjtx-srv/issues
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+wsjtx-srv: Library for WSJT-X server implementation
+===================================================
+
+:Author: Ralf Schlatterbeck <rsc@runtux.com>
+
+This implements a simple UDP server that binds to the WSJT-X_ UDP message
+protocol port. It also provides everything for parsing and/or generating
+WSJT-X_ telegrams.
+
+By default calling ``wsjtx-srv`` will provide a simple server that
+colors all callsigns not in the ADIF file for the current band. It uses
+the ADIF logfile from WSJT-X_ with a default path to that file. You can
+specify the correct path for your installation either via
+command-line (call ``wsjtx-srv`` with the ``--help`` option) or in the
+environment variable ``WBF_PATH``. It has also an implementation that
+looks up DXCC-entities in my log database, but only those that have been
+confirmed via LOTW.
+
+The implementation of ``wsjtx-srv`` should give a rough idea of how to use
+this in your own projects.
+
+There is a companion-program ``wbf`` standing for *worked before* that
+takes a number of callsigns on the command-line and tells you the worked
+before status.
+
+.. _WSJT-X: https://physics.princeton.edu/pulsar/k1jt/wsjtx.html
+
+Changes
+-------
+
+Version 0.5: Add pyproject.toml
+
+- Installation with new setuptools again possible
+
+Version 0.4: Move to setuptools
+
+- Seems previous releases had versioning problems with pypi
+
+Version 0.3: Small fixes
+
+- Compatibility with older protocol versions, thanks to Sampo Savolainen
+  for the patch
+- Fix band lookup if no QSO on band
+
+Version 0.2: Fix setup.py install_requires
+
+Version 0.1: Initial implementation
+
+- Implement serialization and deserialization of WSJT-X_ telegrams and a
+  simple server
+- First Release
+
```

### Comparing `wsjtx_srv-0.4/README.html` & `wsjtx_srv-0.5/README.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8" ?>
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
 <head>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-<meta name="generator" content="Docutils 0.16: http://docutils.sourceforge.net/" />
+<meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <title>wsjtx-srv: Library for WSJT-X server implementation</title>
 <meta name="author" content="Ralf Schlatterbeck &lt;rsc&#64;runtux.com&gt;" />
 <style type="text/css">
 
 /*
 :Author: David Goodger
 :Contact: goodger@users.sourceforge.net
@@ -301,14 +301,22 @@
 <p>The implementation of <tt class="docutils literal"><span class="pre">wsjtx-srv</span></tt> should give a rough idea of how to use
 this in your own projects.</p>
 <p>There is a companion-program <tt class="docutils literal">wbf</tt> standing for <em>worked before</em> that
 takes a number of callsigns on the command-line and tells you the worked
 before status.</p>
 <div class="section" id="changes">
 <h1>Changes</h1>
+<p>Version 0.5: Add pyproject.toml</p>
+<ul class="simple">
+<li>Installation with new setuptools again possible</li>
+</ul>
+<p>Version 0.4: Move to setuptools</p>
+<ul class="simple">
+<li>Seems previous releases had versioning problems with pypi</li>
+</ul>
 <p>Version 0.3: Small fixes</p>
 <ul class="simple">
 <li>Compatibility with older protocol versions, thanks to Sampo Savolainen
 for the patch</li>
 <li>Fix band lookup if no QSO on band</li>
 </ul>
 <p>Version 0.2: Fix setup.py install_requires</p>
```

### Comparing `wsjtx_srv-0.4/README.rst` & `wsjtx_srv-0.5/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 before status.
 
 .. _WSJT-X: https://physics.princeton.edu/pulsar/k1jt/wsjtx.html
 
 Changes
 -------
 
+Version 0.5: Add pyproject.toml
+
+- Installation with new setuptools again possible
+
+Version 0.4: Move to setuptools
+
+- Seems previous releases had versioning problems with pypi
+
 Version 0.3: Small fixes
 
 - Compatibility with older protocol versions, thanks to Sampo Savolainen
   for the patch
 - Fix band lookup if no QSO on band
 
 Version 0.2: Fix setup.py install_requires
```

### Comparing `wsjtx_srv-0.4/setup.py` & `wsjtx_srv-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,20 +50,27 @@
     , license          = license
     , author           = "Ralf Schlatterbeck"
     , author_email     = "rsc@runtux.com"
     , install_requires = ['rsclib', 'hamradio']
     , packages         = ['wsjtx_srv']
     , platforms        = 'Any'
     , url              = "https://github.com/schlatterbeck/wsjtx-srv"
-    , scripts          = ['bin/wsjtx-srv', 'bin/wbf']
+    , entry_points     = dict
+        ( console_scripts =
+            [ 'wsjtx-srv=wsjtx_srv.wsjtx:main'
+            , 'wbf=wsjtx_srv.wsjtx:wbf'
+            ]
+        )
     , python_requires  = rq
     , classifiers      = \
         [ 'Development Status :: 5 - Production/Stable'
         , 'License :: OSI Approved :: ' + license
         , 'Operating System :: OS Independent'
         , 'Programming Language :: Python'
         , 'Intended Audience :: Developers'
         , 'Programming Language :: Python :: 3.7'
         , 'Programming Language :: Python :: 3.8'
         , 'Programming Language :: Python :: 3.9'
+        , 'Programming Language :: Python :: 3.10'
+        , 'Programming Language :: Python :: 3.11'
         ]
     )
```

### Comparing `wsjtx_srv-0.4/wsjtx_srv/wsjtx.py` & `wsjtx_srv-0.5/wsjtx_srv/wsjtx.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,227 +3,227 @@
 import sys
 import io
 import re
 import os
 import atexit
 from socket            import socket, AF_INET, SOCK_DGRAM
 from struct            import pack, unpack
-from argparse          import ArgumentParser
+from argparse          import ArgumentParser, Action as Argparse_Action
 from rsclib.autosuper  import autosuper
 from hamradio.adif     import ADIF
 from hamradio.cty      import CTY_DXCC
 from hamradio.bandplan import bandplan_austria
 from hamradio.dbimport import ADIF_Uploader, urlencode
 
-class Protocol_Element :
+class Protocol_Element:
     """ A single protocol element to be parsed from binary format or
         serialized to binary format.
     """
 
-    def __init__ (self, value) :
+    def __init__ (self, value):
         self.value = value
     # end def __init__
 
     @classmethod
-    def deserialize (cls, bytes, length = 0) :
+    def deserialize (cls, bytes, length = 0):
         raise NotImplementedError ("Needs to be define in sub-class")
     # end def deserialize
 
-    def serialize (self) :
+    def serialize (self):
         raise NotImplementedError ("Needs to be define in sub-class")
     # end def serialize
 
     @property
-    def serialization_size (self) :
+    def serialization_size (self):
         raise NotImplementedError ("Needs to be define in sub-class")
     # end def serialization_size
 
 # end class Protocol_Element
 
-class UTF8_String (Protocol_Element) :
+class UTF8_String (Protocol_Element):
     """ An UTF-8 string consisting of a length and the string
         Special case is a null string (different from an empty string)
         which encodes the length as 0xffffffff
     >>> v = UTF8_String.deserialize (b'\\x00\\x00\\x00\\x04abcd')
     >>> v.value
     'abcd'
     >>> v.serialize ()
     b'\\x00\\x00\\x00\\x04abcd'
     >>> s = UTF8_String (None)
     >>> s.serialize ()
     b'\\xff\\xff\\xff\\xff'
     """
 
     @classmethod
-    def deserialize (cls, bytes, length = 0) :
+    def deserialize (cls, bytes, length = 0):
         offset = 4
         length = unpack ('!L', bytes [:offset]) [0]
         # Special case empty (None?) string
-        if length == 0xFFFFFFFF :
+        if length == 0xFFFFFFFF:
             value = None
             return cls (value)
         value  = unpack ('%ds' % length, bytes [offset:offset+length]) [0]
         return cls (value.decode ('utf-8'))
     # end def deserialize
 
-    def serialize (self) :
-        if self.value is None :
+    def serialize (self):
+        if self.value is None:
             return pack ('!L', 0xFFFFFFFF)
         length = len (self.value)
         value  = self.value.encode ('utf-8')
         return pack ('!L', length) + pack ('%ds' % length, value)
     # end def serialize
 
     @property
-    def serialization_size (self) :
-        if self.value is None :
+    def serialization_size (self):
+        if self.value is None:
             return 4
         return 4 + len (self.value.encode ('utf-8'))
     # end def serialization_size
 
 # end class UTF8_String
 
-class Optional_Quint (Protocol_Element) :
+class Optional_Quint (Protocol_Element):
     """ A quint which is optional, length in deserialize is used
         We encode a missing value as None
     """
 
     formats = dict \
         (( (1, '!B')
         ,  (4, '!L')
         ,  (8, '!Q')
         ))
 
     @classmethod
-    def deserialize (cls, bytes, length = 1) :
-        if len (bytes) == 0 :
+    def deserialize (cls, bytes, length = 1):
+        if len (bytes) == 0:
             value = None
-        else :
+        else:
             value = unpack (self.formats [length], bytes) [0]
         object = cls (value)
         object.size = length
-        if value is None :
+        if value is None:
             object.size = 0
         return object
     # end def deserialize
 
-    def serialize (self) :
-        if self.value is None :
+    def serialize (self):
+        if self.value is None:
             return b''
         return pack (self.formats [self.size], self.value)
     # end def serialize
 
     @property
-    def serialization_size (self) :
-        if self.value is None :
+    def serialization_size (self):
+        if self.value is None:
             return 0
         return self.size
     # end def serialization_size
 
 # end class Optional_Quint
 
-class QDateTime (Protocol_Element) :
+class QDateTime (Protocol_Element):
     """ A QT DateTime object
         The case with a timezone is not used
     """
 
-    def __init__ (self, date, time, timespec, offset = None) :
+    def __init__ (self, date, time, timespec, offset = None):
         self.date     = date
         self.time     = time
         self.timespec = timespec
         self.offset   = offset
         assert self.offset is None or self.timespec == 2
-        if self.timespec == 2 and self.offset is not None :
+        if self.timespec == 2 and self.offset is not None:
             raise ValueError ("Offset required when timespec=2")
     # end def __init__
 
     @classmethod
-    def deserialize (cls, bytes, length = 0) :
+    def deserialize (cls, bytes, length = 0):
         date, time, timespec = unpack ('!qLB', bytes [:13])
         offset = None
-        if timespec == 2 :
+        if timespec == 2:
             offset = unpack ('!l', bytes [13:17]) [0]
         return cls (date, time, timespec, offset)
     # end def deserialize
 
-    def serialize (self) :
+    def serialize (self):
         r = [pack ('!qLB', self.date, self.time, self.timespec)]
-        if self.offset is not None :
+        if self.offset is not None:
             r.append (pack ('!l', self.offset))
         return b''.join (r)
     # end def serialize
 
     @property
-    def serialization_size (self) :
-        if self.offset is None :
+    def serialization_size (self):
+        if self.offset is None:
             return 13
         return 13 + 4
     # end def serialization_size
 
     @property
-    def value (self) :
+    def value (self):
         return self
     # end def value
 
-    def __str__ (self) :
+    def __str__ (self):
         s = ( 'QDatTime(date=%(date)s time=%(time)s '
             + 'timespec=%(timespec)s offset=%(offset)s)'
             )
         return s % self.__dict__
     # end def __str__
     __repr__ = __str__
 
 # end class QDateTime
 
-class QColor (Protocol_Element) :
+class QColor (Protocol_Element):
     """ A QT color object
         We support only RGB type or invalid
     """
 
     fmt          = '!BHHHHH'
     spec_rgb     = 1
     spec_invalid = 0
     cmax         = 0xFFFF
     serialization_size = 11
 
     def __init__ \
-        (self, red = 0, green = 0, blue = 0, alpha = cmax, spec = spec_rgb) :
+        (self, red = 0, green = 0, blue = 0, alpha = cmax, spec = spec_rgb):
         self.spec     = spec
         self.red      = red
         self.green    = green
         self.blue     = blue
         self.alpha    = alpha
     # end def __init__
 
     @classmethod
-    def deserialize (cls, bytes, length = 0) :
+    def deserialize (cls, bytes, length = 0):
         b = bytes [:cls.serialization_size]
         s, a, r, g, b, dummy = unpack (cls.fmt, b)
         return cls (spec = s, alpha = a, red = r, green = g, blue = b)
     # end def deserialize
 
-    def serialize (self) :
+    def serialize (self):
         return pack \
             ( self.fmt
             , self.spec
             , self.alpha
             , self.red
             , self.green
             , self.blue
             , 0
             )
     # end def serialize
 
     @property
-    def value (self) :
+    def value (self):
         return self
     # end def value
 
-    def __str__ (self) :
-        if self.spec != self.spec_rgb :
+    def __str__ (self):
+        if self.spec != self.spec_rgb:
             return 'QColor(Invalid)'
         s = ( 'QColor(alpha=%(alpha)s, red=%(red)s, '
             + 'green=%(green)s, blue=%(blue)s)'
             )
         return s % self.__dict__
     # end def __str__
     __repr__ = __str__
@@ -264,15 +264,15 @@
 qtime      = quint32
 qdatetime  = (QDateTime, 0)
 qcolor     = (QColor, 0)
 
 statusmsg = b'\xad\xbc\xcb\xda\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x14WSJT-X - TS590S-klbg\x00\x00\x00\x00\x00k\xf0\xd0\x00\x00\x00\x03FT8\x00\x00\x00\x06XAMPLE\x00\x00\x00\x02-2\x00\x00\x00\x03FT8\x00\x00\x01\x00\x00\x02\xcb\x00\x00\x04n\x00\x00\x00\x06OE3RSU\x00\x00\x00\x06JN88DG\x00\x00\x00\x04JO21\x00\xff\xff\xff\xff\x00\x00\xff\xff\xff\xff\xff\xff\xff\xff\x00\x00\x00\x0bTS590S-klbg\x00\x00\x00%XAMPLE OE3RSU 73                     '
 clearmsg = b'\xad\xbc\xcb\xda\x00\x00\x00\x03\x00\x00\x00\x03\x00\x00\x00\x14WSJT-X - TS590S-klbg'
 
-class WSJTX_Telegram (autosuper) :
+class WSJTX_Telegram (autosuper):
     """ Base class of WSJTX Telegram
         Note that we a list of (name, format, len) tuples as the format
         specification. The name is the name of the variable, the format
         is either a struct.pack compatible format specifier or an
         instance of Protocol_Element which knows how to deserialize (or
         serialize) itself. The len is the length to parse from the
         string. If 0 the Protocol_Element will know its serialization
@@ -294,94 +294,94 @@
         ]
     defaults = dict (magic = magic, version_number = 3, id = 'wsjt-server')
     suppress = dict.fromkeys (('magic', 'version_number', 'id', 'type'))
 
     # Individual telegrams register here:
     type_registry = {}
 
-    def __init__ (self, **kw) :
+    def __init__ (self, **kw):
         params = {}
         params.update (self.defaults)
         params.update (kw)
-        if 'type' not in params :
+        if 'type' not in params:
             params ['type'] = self.type
         assert params ['magic'] == self.magic
         assert self.schema_version_number >= params ['version_number']
         # Thats for sub-classes, they have their own format
-        for name, (a, b) in self.format :
+        for name, (a, b) in self.format:
             setattr (self, name, params [name])
-        if self.__class__.type is not None :
+        if self.__class__.type is not None:
             assert self.__class__.type == self.type
         self.__super.__init__ (** params)
     # end def __init__
 
     @classmethod
-    def from_bytes (cls, bytes) :
+    def from_bytes (cls, bytes):
         kw   = cls.deserialize (bytes)
         type = kw ['type']
         self = cls (** kw)
-        if type in cls.type_registry :
+        if type in cls.type_registry:
             c = cls.type_registry [type]
             kw.update (c.deserialize (bytes))
             return c (** kw)
-        else :
+        else:
             return self
     # end def from_bytes
 
     @classmethod
-    def deserialize (cls, bytes) :
+    def deserialize (cls, bytes):
         b  = bytes
         kw = {}
-        for name, (format, length) in cls.format :
+        for name, (format, length) in cls.format:
             # Due to compatibility reasons new message fields are added to
             # the end of the messsage. The buffer is empty when the message
             # is older format and a field is missing.
             if (len(b) == 0):
                 kw[name] = None
                 continue
-            if isinstance (format, type ('')) :
+            if isinstance (format, type ('')):
                 kw [name] = unpack (format, b [:length]) [0]
                 b = b [length:]
-            else :
+            else:
                 value = format.deserialize (b, length)
                 b = b [value.serialization_size:]
                 kw [name] = value.value
         return kw
     # end def deserialize
 
-    def as_bytes (self) :
+    def as_bytes (self):
         r = []
-        for name, (fmt, length) in self.format :
+        for name, (fmt, length) in self.format:
             v = getattr (self, name)
-            if isinstance (v, Protocol_Element) :
+            if isinstance (v, Protocol_Element):
                 r.append (v.serialize ())
-            elif isinstance (fmt, type ('')) :
+            elif isinstance (fmt, type ('')):
                 r.append (pack (fmt, v))
-            else :
+            else:
                 r.append (fmt (v).serialize ())
         return b''.join (r)
     # end def as_bytes
 
-    def __str__ (self) :
+    def __str__ (self):
         r = [self.__class__.__name__.split ('_', 1) [-1]]
-        for n, (fmt, length) in self.format :
-            if n not in self.suppress :
+        for n, (fmt, length) in self.format:
+            if n not in self.suppress:
                 r.append ('%s=%s' % (n, getattr (self, n)))
         return ' '.join (r)
     # end def __str__
     __repr__ = __str__
 
     @property
-    def serialization_size (self) :
+    def serialization_size (self):
         return 16 + len (self.id.encode ('utf-8'))
     # end def serialization_size
 
 # end class WSJTX_Telegram
 
-class WSJTX_Heartbeat (WSJTX_Telegram) :
+class WSJTX_Heartbeat (WSJTX_Telegram):
 
     type   = 0
 
     format = WSJTX_Telegram.format + \
         [ ('max_schema',     quint32)
         , ('version',        qutf8)
         , ('revision',       qutf8)
@@ -391,15 +391,15 @@
         , version    = ''
         , revision   = ''
         , ** WSJTX_Telegram.defaults
         )
 # end class WSJTX_Heartbeat
 WSJTX_Telegram.type_registry [WSJTX_Heartbeat.type] = WSJTX_Heartbeat
 
-class WSJTX_Status (WSJTX_Telegram) :
+class WSJTX_Status (WSJTX_Telegram):
 
     type   = 1
     format = WSJTX_Telegram.format + \
         [ ('dial_frq',       quint64)
         , ('mode',           qutf8)
         , ('dx_call',        qutf8)
         , ('report',         qutf8)
@@ -421,15 +421,15 @@
         , ('config_name',    qutf8)
         , ('tx_message',     qutf8)
         ]
 
 # end class WSJTX_Status
 WSJTX_Telegram.type_registry [WSJTX_Status.type] = WSJTX_Status
 
-class WSJTX_Decode (WSJTX_Telegram) :
+class WSJTX_Decode (WSJTX_Telegram):
 
     type   = 2
     format = WSJTX_Telegram.format + \
         [ ('is_new',         qbool)
         , ('time',           qtime)
         , ('snr',            qint32)
         , ('delta_t',        qdouble)
@@ -439,24 +439,24 @@
         , ('low_confidence', qbool)
         , ('off_air',        qbool)
         ]
 
 # end class WSJTX_Decode
 WSJTX_Telegram.type_registry [WSJTX_Decode.type] = WSJTX_Decode
 
-class WSJTX_Clear (WSJTX_Telegram) :
+class WSJTX_Clear (WSJTX_Telegram):
 
     type     = 3
     format   = WSJTX_Telegram.format + [('window', opt_quint8)]
     defaults = dict (window = None, **WSJTX_Telegram.defaults)
 
 # end class WSJTX_Clear
 WSJTX_Telegram.type_registry [WSJTX_Clear.type] = WSJTX_Clear
 
-class WSJTX_Reply (WSJTX_Telegram) :
+class WSJTX_Reply (WSJTX_Telegram):
 
     type   = 4
     format = WSJTX_Telegram.format + \
         [ ('time',           qtime)
         , ('snr',            qint32)
         , ('delta_t',        qdouble)
         , ('delta_f',        quint32)
@@ -465,15 +465,15 @@
         , ('low_confidence', qbool)
         , ('modifiers',      quint8)
         ]
 
 # end class WSJTX_Reply
 WSJTX_Telegram.type_registry [WSJTX_Reply.type] = WSJTX_Reply
 
-class WSJTX_QSO_Logged (WSJTX_Telegram) :
+class WSJTX_QSO_Logged (WSJTX_Telegram):
 
     type   = 5
     format = WSJTX_Telegram.format + \
         [ ('time_off',       qdatetime)
         , ('dx_call',        qutf8)
         , ('dx_grid',        qutf8)
         , ('tx_frq',         quint64)
@@ -491,49 +491,49 @@
         , ('exchange_recv',  qutf8)
         , ('adif_propmode',  qutf8)
         ]
 
 # end class WSJTX_QSO_Logged
 WSJTX_Telegram.type_registry [WSJTX_QSO_Logged.type] = WSJTX_QSO_Logged
 
-class WSJTX_Close (WSJTX_Telegram) :
+class WSJTX_Close (WSJTX_Telegram):
 
     type   = 6
 
 # end class WSJTX_Close
 WSJTX_Telegram.type_registry [WSJTX_Close.type] = WSJTX_Close
 
-class WSJTX_Replay (WSJTX_Telegram) :
+class WSJTX_Replay (WSJTX_Telegram):
 
     type   = 7
 
 # end class WSJTX_Replay
 WSJTX_Telegram.type_registry [WSJTX_Replay.type] = WSJTX_Replay
 
-class WSJTX_Halt_TX (WSJTX_Telegram) :
+class WSJTX_Halt_TX (WSJTX_Telegram):
 
     type   = 8
     format = WSJTX_Telegram.format + [('auto_tx_only', qbool)]
 
 # end class WSJTX_Halt_TX
 WSJTX_Telegram.type_registry [WSJTX_Halt_TX.type] = WSJTX_Halt_TX
 
-class WSJTX_Free_Text (WSJTX_Telegram) :
+class WSJTX_Free_Text (WSJTX_Telegram):
 
     type   = 9
     format = WSJTX_Telegram.format + \
         [ ('text',   qutf8)
         , ('send',   qbool)
         ]
     defaults = dict (send = False, **WSJTX_Telegram.defaults)
 
 # end class WSJTX_Free_Text
 WSJTX_Telegram.type_registry [WSJTX_Free_Text.type] = WSJTX_Free_Text
 
-class WSJTX_WSPR_Decode (WSJTX_Telegram) :
+class WSJTX_WSPR_Decode (WSJTX_Telegram):
 
     type   = 10
     format = WSJTX_Telegram.format + \
         [ ('is_new',         qbool)
         , ('time',           qtime)
         , ('snr',            qint32)
         , ('delta_t',        qdouble)
@@ -544,31 +544,31 @@
         , ('power',          qint32)
         , ('off_air',        qbool)
         ]
 
 # end class WSJTX_WSPR_Decode
 WSJTX_Telegram.type_registry [WSJTX_WSPR_Decode.type] = WSJTX_WSPR_Decode
 
-class WSJTX_Location (WSJTX_Telegram) :
+class WSJTX_Location (WSJTX_Telegram):
 
     type   = 11
     format = WSJTX_Telegram.format + [('location', qutf8)]
 
 # end class WSJTX_Location
 WSJTX_Telegram.type_registry [WSJTX_Location.type] = WSJTX_Location
 
-class WSJTX_Logged_ADIF (WSJTX_Telegram) :
+class WSJTX_Logged_ADIF (WSJTX_Telegram):
 
     type   = 12
     format = WSJTX_Telegram.format + [('adif_txt', qutf8)]
 
 # end class WSJTX_Logged_ADIF
 WSJTX_Telegram.type_registry [WSJTX_Logged_ADIF.type] = WSJTX_Logged_ADIF
 
-class WSJTX_Highlight_Call (WSJTX_Telegram) :
+class WSJTX_Highlight_Call (WSJTX_Telegram):
     """ Highlight a callsign in WSJTX
     >>> kw = dict (id = 'test', version_number = 2)
     >>> whc = WSJTX_Highlight_Call \\
     ...     ( callsign = 'OE3RSU'
     ...     , bg_color = color_white
     ...     , fg_color = color_red
     ...     , highlight_last = 1
@@ -592,23 +592,23 @@
         , highlight_last = False
         , ** WSJTX_Telegram.defaults
         )
 
 # end class WSJTX_Highlight_Call
 WSJTX_Telegram.type_registry [WSJTX_Highlight_Call.type] = WSJTX_Highlight_Call
 
-class WSJTX_Switch_Config (WSJTX_Telegram) :
+class WSJTX_Switch_Config (WSJTX_Telegram):
 
     type   = 14
     format = WSJTX_Telegram.format + [('adif_txt', qutf8)]
 
 # end class WSJTX_Switch_Config
 WSJTX_Telegram.type_registry [WSJTX_Switch_Config.type] = WSJTX_Switch_Config
 
-class WSJTX_Configure (WSJTX_Telegram) :
+class WSJTX_Configure (WSJTX_Telegram):
 
     type   = 15
     format = WSJTX_Telegram.format + \
         [ ('mode',           qutf8)
         , ('frq_tolerance',  quint32)
         , ('sub_mode',       qutf8)
         , ('fast_mode',      qbool)
@@ -618,155 +618,155 @@
         , ('dx_grid',        qutf8)
         , ('gen_messages',   qbool)
         ]
 
 # end class WSJTX_Configure
 WSJTX_Telegram.type_registry [WSJTX_Configure.type] = WSJTX_Configure
 
-class UDP_Connector :
+class UDP_Connector:
 
-    def __init__ (self, wbf, ip = '127.0.0.1', port = 2237, id = None) :
+    def __init__ (self, wbf, ip = '127.0.0.1', port = 2237, id = None):
         self.band    = None
         self.ip      = ip
         self.port    = port
         self.socket  = socket (AF_INET, SOCK_DGRAM)
         self.wbf     = wbf
         self.args    = getattr (wbf, 'args', None)
         self.peer    = {}
         self.adr     = None
         self.id      = id
         self.dx_call = None
         self.socket.bind ((self.ip, self.port))
-        if id is None :
+        if id is None:
             self.id = WSJTX_Telegram.defaults ['id']
         self.heartbeat_seen = False
         self.color_by_call  = {}
         self.pending_color  = {}
         # Register atexit handler for cleanup
         atexit.register (self.cleanup)
     # end def __init__
 
-    def cleanup (self) :
+    def cleanup (self):
         self.decolor ()
         self.perform_pending_changes ()
     # end def cleanup
 
-    def color (self, callsign, **kw) :
+    def color (self, callsign, **kw):
         tel = WSJTX_Highlight_Call (callsign = callsign, **kw)
         self.socket.sendto (tel.as_bytes (), self.adr)
     # end def color
 
-    def decolor (self) :
+    def decolor (self):
         """ Remove all coloring
             Needed on band change and when exiting
             Note that this only schedules the changes.
         """
-        for call in self.color_by_call :
+        for call in self.color_by_call:
             # Can save some time not considering uncolored calls
-            if self.color_by_call [call] != ctuple_invalid :
+            if self.color_by_call [call] != ctuple_invalid:
                 self.pending_color [call] = ctuple_invalid
         self.color_by_call = {}
     # end def decolor
 
-    def handle (self, tel) :
+    def handle (self, tel):
         """ Handle given telegram.
             We send a heartbeat whenever we receive one.
             In addition we parse Decode messages, extract the call sign
             and determine worked-before and coloring.
         """
-        if not self.heartbeat_seen or isinstance (tel, WSJTX_Heartbeat) :
+        if not self.heartbeat_seen or isinstance (tel, WSJTX_Heartbeat):
             self.heartbeat ()
-        if isinstance (tel, WSJTX_Status) :
+        if isinstance (tel, WSJTX_Status):
             self.handle_status (tel)
-        if isinstance (tel, WSJTX_Decode) :
+        if isinstance (tel, WSJTX_Decode):
             self.handle_decode (tel)
-        if isinstance (tel, WSJTX_Logged_ADIF) :
+        if isinstance (tel, WSJTX_Logged_ADIF):
             self.handle_logged (tel)
-        if isinstance (tel, WSJTX_Close) :
+        if isinstance (tel, WSJTX_Close):
             self.handle_close (tel)
     # end def handle
 
-    def handle_close (self, tel) :
+    def handle_close (self, tel):
         """ Just exit when wsjtx exits
         """
         assert self.peer [tel.id] == self.adr
         sys.exit (0)
     # end def handle_close
 
-    def handle_decode (self, tel) :
-        if tel.off_air or not tel.is_new :
+    def handle_decode (self, tel):
+        if tel.off_air or not tel.is_new:
             return
         call  = self.parse_message (tel) or ''
         call  = call.lstrip ('<').rstrip ('>')
-        if not call or call == '...' :
+        if not call or call == '...':
             return
         color = self.wbf.lookup_color (self.band, call)
-        if call in self.color_by_call :
-            if self.color_by_call [call] != color :
+        if call in self.color_by_call:
+            if self.color_by_call [call] != color:
                 self.update_color (call, color)
-        else :
+        else:
             self.update_color (call, color)
     # end def handle_decode
 
-    def handle_logged (self, tel) :
+    def handle_logged (self, tel):
         """ Handle a Log event when a QSO is logged.
             We directly receive ADIF from WSJTX
         """
         adif = ADIF (io.StringIO (tel.adif_txt))
         assert len (adif.records) == 1
         rec = adif.records [0]
         self.wbf.add_entry (rec)
     # end def handle_logged
 
-    def handle_status (self, tel) :
+    def handle_status (self, tel):
         """ Handle pending coloring
         """
         band = bandplan_austria.lookup (tel.dial_frq)
-        if self.band != band.name :
+        if self.band != band.name:
             self.band = band.name
             # Invalidate all colors on band change
             self.decolor ()
-        if self.dx_call != tel.dx_call :
+        if self.dx_call != tel.dx_call:
             self.dx_call = tel.dx_call
-            if self.args.set_locator_msg :
+            if self.args.set_locator_msg:
                 t = '<%s> <%s> 597373 %s' \
                   % (self.dx_call, self.args.callsign, self.args.locator)
                 stel = WSJTX_Free_Text (text = t)
                 self.socket.sendto (stel.as_bytes (), self.adr)
                 print ('Set free text to "%s"' % t)
-        if not tel.decoding :
+        if not tel.decoding:
             self.perform_pending_changes ()
     # end def handle_status
 
-    def heartbeat (self, **kw) :
+    def heartbeat (self, **kw):
         tel = WSJTX_Heartbeat (version = '4711', **kw)
         self.socket.sendto (tel.as_bytes (), self.adr)
     # end def heartbeat
 
     # Some regexes for matching
     re_report = re.compile (r'[R]?[-+][0-9]{2}')
     re_loc    = re.compile (r'[A-Z]{2}[0-9]{2}')
     re_call   = re.compile \
         (r'(([A-Z])|([A-Z][A-Z0-9])|([0-9][A-Z]))[0-9][A-Z]{1,3}')
 
-    def is_locator (self, s) :
+    def is_locator (self, s):
         """ Check if s is a locator
         >>> u = UDP_Connector (port = 4711, wbf = None)
         >>> u.is_locator ('-2')
         False
         >>> u.is_locator ('JN88')
         True
         >>> u.is_locator ('kk77')
         False
         >>> u.socket.close ()
         """
         return bool (self.re_loc.match (s))
     # end def is_locator
 
-    def is_report (self, s) :
+    def is_report (self, s):
         """ Check if s is a report
         >>> u = UDP_Connector (port = 4711, wbf = None)
         >>> u.is_report ('-2')
         False
         >>> u.is_report ('-02')
         True
         >>> u.is_report ('+20')
@@ -774,34 +774,34 @@
         >>> u.is_report ('R+20')
         True
         >>> u.socket.close ()
         """
         return bool (self.re_report.match (s))
     # end def is_locator
 
-    def is_stdcall (self, s) :
+    def is_stdcall (self, s):
         """ Check if s is a standard callsign
         >>> u = UDP_Connector (port = 4711, wbf = None)
         >>> u.is_stdcall ('D1X')
         True
         >>> u.is_stdcall ('JN88')
         False
         >>> u.is_stdcall ('OE3RSU')
         True
         >>> u.socket.close ()
         """
         return bool (self.re_call.match (s))
     # end def is_stdcall
 
-    def parse_message (self, tel) :
+    def parse_message (self, tel):
         """ Parse the message property of a decode which includes the
             callsign(s). Note that we try to use only the second
             (sender) callsign.
         >>> u = UDP_Connector (port = 4711, wbf = None)
-        >>> class t :
+        >>> class t:
         ...     message = None
         >>> t.message = 'JA1XXX YL2XXX R-18'
         >>> u.parse_message (t)
         'YL2XXX'
         >>> t.message = 'UB9XXX OH1XXX KP20'
         >>> u.parse_message (t)
         'OH1XXX'
@@ -857,110 +857,115 @@
         >>> u.parse_message (t)
         Unknown message: OZ1XXX 0
         >>> t.message = '9H1XX EA8XX IL18'
         >>> u.parse_message (t)
         'EA8XX'
         >>> u.socket.close ()
         """
-        if not tel.message :
+        if not tel.message:
             print ("Empty message: %s" % tel)
             return None
-        if ';' in tel.message :
+        if ';' in tel.message:
             print ("Unknown message: %s" % tel.message)
             return None
         l = tel.message.split ()
         # Strip off marginal decode info
-        if l [-1].startswith ('a') :
+        if l [-1].startswith ('a'):
             l = l [:-1]
-        if l [-1] == '?' :
+        if l [-1] == '?':
             l = l [:-1]
-        if l [0] in ('CQ', 'QRZ') :
+        if l [0] in ('CQ', 'QRZ'):
             # CQ DX or similar
-            if len (l) == 4 and len (l [2]) >= 3 :
+            if len (l) == 4 and len (l [2]) >= 3:
                 return l [2]
             # CQ DX or something without locator
-            if len (l) == 3 and len (l [2]) != 4 and len (l [1]) <= 4 :
-                if len (l [2]) >= 3 :
+            if len (l) == 3 and len (l [2]) != 4 and len (l [1]) <= 4:
+                if len (l [2]) >= 3:
                     return l [2]
-            if len (l [1]) >= 3 :
+            if len (l [1]) >= 3:
                 return l [1]
-        if len (l) == 2 and len (l [1]) >= 3 :
+        if len (l) == 2 and len (l [1]) >= 3:
             return l [1]
-        if len (l) < 2 :
+        if len (l) < 2:
             print ("Unknown message: %s" % tel.message)
             return None
-        if len (l) == 4 and l [2] == 'R' and len (l [1]) >= 3 :
+        if len (l) == 4 and l [2] == 'R' and len (l [1]) >= 3:
             return l [1]
-        if len (l) == 3 and len (l [1]) >= 3 :
+        if len (l) == 3 and len (l [1]) >= 3:
             if len (l [1]) > 3 or self.is_stdcall (l [1]):
                 return l [1]
-            if self.is_locator (l [2]) :
+            if self.is_locator (l [2]):
                 return l [1]
-            if self.is_report (l [2]) :
+            if self.is_report (l [2]):
                 return l [1]
         print ("Unknown message: %s" % tel.message)
         return None
     # end def parse_message
 
-    def perform_pending_changes (self) :
-        for call in self.pending_color :
+    def perform_pending_changes (self):
+        for call in self.pending_color:
             fg = self.pending_color [call][0]
             bg = self.pending_color [call][1]
             self.color (call, fg_color = fg, bg_color = bg)
         self.pending_color = {}
     # end def perform_pending_changes
 
-    def receive (self) :
+    def receive (self):
         bytes, address = self.socket.recvfrom (4096)
         tel = WSJTX_Telegram.from_bytes (bytes)
-        if tel.id not in self.peer :
+        if tel.id not in self.peer:
             self.peer [tel.id] = address
-        if not self.adr :
+        if not self.adr:
             self.adr = address
         # Only handle messages from preferred peer for now
-        if self.adr == address :
+        if self.adr == address:
             self.handle (tel)
         return tel
     # end def receive
 
-    def set_peer (self, peername) :
-        if peername in self.peer :
+    def set_peer (self, peername):
+        if peername in self.peer:
             self.adr = self.peer [peername]
     # end def set_peer
 
-    def update_color (self, call, color) :
+    def update_color (self, call, color):
         self.color_by_call [call] = color
         self.pending_color [call] = color
     # end def update_color
 
 # end class UDP_Connector
 
-class WBF (autosuper) :
+class WBF (autosuper):
     """ Worked before info
+        This applies to the given band.
+        It is initialized with all calls for this band, in the end
+        self.wbf contains counters for all dxccs we have seen.
     """
 
-    def __init__ (self, band, always_match = False) :
+    def __init__ (self, band, always_match = False):
         self.band         = band
         self.wbf          = {}
         self.always_match = always_match
     # end def __init__
 
-    def add_item (self, item, record = 1) :
-        self.wbf [item] = record
+    def add_item (self, item):
+        if item not in self.wbf:
+            self.wbf [item] = 0
+        self.wbf [item] += 1
     # end def add_item
 
-    def lookup (self, item) :
-        if self.always_match :
+    def lookup (self, item):
+        if self.always_match:
             return None
         return self.wbf.get (item, None)
     # end def lookup
 
 # end class WBF
 
-class Worked_Before (autosuper) :
+class Worked_Before (autosuper):
     """ This parses an ADIF log file and extracts worked-before info
         This can then be used by the UDP_Connector to color calls by
         parsing calls from incoming Decode packets.
         We have a WBF per band and a WBF per known DXCC.
         if we cannot determine the dxcc info for a record (unfortunately
         not provided by wsjtx currently) all records will be colored
         only in the color for "new call" or "new call on band".
@@ -973,70 +978,70 @@
     ctuple_wbf           = ctuple_invalid
     ctuple_dxcc          = ctuple_dxcc
     ctuple_dxcc_band     = ctuple_dxcc_band
     ctuple_new_call      = ctuple_new_call
     ctuple_new_call_band = ctuple_new_call_band
     ctuple_highlight     = ctuple_highlight
 
-    def __init__ (self, adif = None, args = None, **kw) :
+    def __init__ (self, adif = None, args = None, **kw):
         # Color override
-        for k in kw :
-            if k.startswith ('ctuple_') :
+        for k in kw:
+            if k.startswith ('ctuple_'):
                 setattr (self, k, kw [k])
         self.args      = args
         self.cty_dxcc  = CTY_DXCC ()
-        self.band_info = {}
+        self.band_info = {} # by callsign
         self.dxcc_info = {} # by dxcc number
         self.band_info ['ALL'] = WBF ('ALL')
         self.dxcc_info ['ALL'] = WBF ('ALL')
-        if adif :
-            with io.open (adif, 'r', encoding = args.encoding) as f :
+        if adif:
+            with io.open (adif, 'r', encoding = args.encoding) as f:
                 adif = ADIF (f)
-                for rec in adif :
-                    if not rec.band :
+                for rec in adif:
+                    if not rec.band:
                         continue
                     self.add_entry (rec)
     # end def __init__
 
-    def fuzzy_match_dxcc (self, call, use_dxcc = False) :
+    def fuzzy_match_dxcc (self, call, use_dxcc = False):
         lookup = self.cty_dxcc.callsign_lookup
-        if use_dxcc :
+        if use_dxcc:
             lookup = self.cty_dxcc.dxcc.callsign_lookup
         entities = lookup (call)
         return entities
     # end def fuzzy_match_dxcc
 
-    def fuzzy_match_dxcc_code (self, call, only_one = False) :
+    def fuzzy_match_dxcc_code (self, call, only_one = False):
         """ Use prefix info from dxcc list to fuzzy match the call
         >>> w = Worked_Before ()
         >>> w.fuzzy_match_dxcc_code ('OE3RSU')
         ['206']
         >>> w.fuzzy_match_dxcc_code ('OE3RSU', only_one = True)
         '206'
         >>> w.fuzzy_match_dxcc_code ('RK3LG', only_one = True)
         '054'
         >>> w.fuzzy_match_dxcc_code ('RK3LG')
         ['054']
         """
         entities = self.fuzzy_match_dxcc (call)
-        if entities :
-            if only_one and len (entities) == 1 :
+        if entities:
+            if only_one and len (entities) == 1:
                 return entities [0].code
-            elif not only_one :
+            elif not only_one:
                 return [e.code for e in entities]
     # end def fuzzy_match_dxcc_code
 
-    def add_call_entry (self, rec) :
-        if rec.band not in self.band_info :
+    def add_call_entry (self, rec):
+        if rec.band not in self.band_info:
             self.band_info [rec.band] = WBF (rec.band)
-        self.band_info [rec.band].add_item (rec.call, rec)
-        self.band_info ['ALL'].   add_item (rec.call, rec)
+        self.band_info [rec.band].add_item (rec.call)
+        self.band_info ['ALL'].   add_item (rec.call)
     # end def add_call_entry
 
-    def add_dxcc_entry (self, rec) :
+    def add_dxcc_entry (self, rec):
         """ Match the dxcc for this adif record
             Note that we're using the standard ADIF DXCC entity code in
             the ADIF field DXCC *or* the COUNTRY field (in ASCII) or the
             COUNTRY_INTL field (in utf-8). Since all entity names are in
             english, all the COUNTRY_INTL should be in ASCII (a subset
             of utf-8) anyway. We match country to code and vice-versa
             via the ARRL dxcc list. If all this fails we do a fuzzy
@@ -1045,63 +1050,63 @@
             Note that you may want to code your own dxcc lookup for
             calls: You may want to treat dxcc entities for which you
             worked someone but do not have a QSL (or no LOTW QSL) as not
             worked before. So in that case you can override this
             routine.
         """
         dxcc_code = None
-        if getattr (rec, 'dxcc', None) :
+        if getattr (rec, 'dxcc', None):
             dxcc_code = '%03d' % int (rec.dxcc, 10)
-        elif getattr (rec, 'country', None) :
+        elif getattr (rec, 'country', None):
             dxcc = self.cty_dxcc.dxcc.by_name [rec.country]
             dxcc_code = dxcc.code
-        elif getattr (rec, 'country_intl', None) :
+        elif getattr (rec, 'country_intl', None):
             dxcc = self.cty_dxcc.dxcc.by_name [rec.country_intl]
             dxcc_code = dxcc.code
-        else :
+        else:
             dxcc_code = self.fuzzy_match_dxcc_code (rec.call, only_one = 1)
-        if dxcc_code :
-            if rec.band not in self.dxcc_info :
+        if dxcc_code:
+            if rec.band not in self.dxcc_info:
                 self.dxcc_info [rec.band] = WBF (rec.band)
             self.dxcc_info [rec.band].add_item (dxcc_code)
             self.dxcc_info ['ALL'].   add_item (dxcc_code)
     # end def add_dxcc_entry
 
-    def add_entry (self, rec) :
+    def add_entry (self, rec):
         self.add_call_entry (rec)
         self.add_dxcc_entry (rec)
     # end def add_entry
 
-    def lookup_new_call (self, call) :
+    def lookup_new_call (self, call):
         """ Look up a call and decide if new on band or global
         >>> w = Worked_Before ()
         >>> w.lookup_new_call ('SX4711TEST')
         'new_call'
         """
         r = self.band_info ['ALL'].lookup (call)
-        if r :
+        if r:
             return 'new_call_band'
         return 'new_call'
     # end def lookup_new_call
 
-    def lookup (self, band, call) :
+    def lookup (self, band, call):
         """ Look up the status for this call for this band
             Involves checking of a new DXCC (on band or globally)
             and the check of a new call (on band or globally)
             The following test looks up RK0 which matches both, European
             Russia and Asiatic Russia.
         >>> w = Worked_Before ()
         >>> w.band_info ['40m'] = WBF ('40m')
         >>> w.band_info ['17m'] = WBF ('40m')
         >>> w.band_info ['10m'] = WBF ('40m')
         >>> w.dxcc_info ['40m'] = WBF ('40m')
         >>> w.dxcc_info ['17m'] = WBF ('17m')
         >>> w.dxcc_info ['10m'] = WBF ('17m')
         >>> w.dxcc_info ['ALL'] = WBF ('ALL')
-        >>> for code in ('054', '015', '236', '279') :
+        >>> for code in ('054', '015', '236', '279'):
         ...     w.dxcc_info ['40m'].add_item (code)
         ...     w.dxcc_info ['ALL'].add_item (code)
         >>> w.lookup ('40m', 'RK0')
         'new_call'
         >>> w.lookup ('40m', 'SX4711TEST')
         'new_call'
 
@@ -1109,171 +1114,201 @@
         >>> w.lookup ('17m', 'GM0XXX')
         'new_dxcc_band'
 
         # Nothing worked for this DXCC
         >>> w.lookup ('10m', 'GG7XXX')
         'new_dxcc'
         """
-        if band not in self.band_info :
-            return 'new_dxcc'
+        if band not in self.band_info:
+            self.band_info [band] = WBF (band)
         r = self.band_info [band].lookup (call)
-        if r :
+        if r:
             return 'wbf'
         dxccs = self.fuzzy_match_dxcc_code (call)
-        if not dxccs :
+        if not dxccs:
             return 'new_dxcc'
         r2 = 1
-        for dxcc in dxccs :
+        m  = 0
+        for dxcc in dxccs:
             if band not in self.dxcc_info:
                 self.dxcc_info [band] = WBF (band)
             r2 = r2 and self.dxcc_info [band].lookup (dxcc)
+            if r2 and self.dxcc_info [band].lookup (dxcc) > m:
+                m = self.dxcc_info [band].lookup (dxcc)
         # Matched for *all* dxccs; not new dxcc on this (and any) band
-        if r2 :
-            for dxcc in dxccs :
-                if dxcc in self.args.highlight_dxcc :
-                    return 'highlight'
+        if r2:
+            for dxcc in dxccs:
+                if dxcc in self.args.highlight_dxcc:
+                    if not self.args.highlight_dxcc [dxcc]:
+                        return 'highlight'
+                    else:
+                        if self.args.highlight_dxcc [dxcc] > m:
+                            return 'highlight'
             return self.lookup_new_call (call)
         r3 = 1
-        for dxcc in dxccs :
+        for dxcc in dxccs:
             r3 = r3 and self.dxcc_info ['ALL'].lookup (dxcc)
         # Matched for *all* dxccs; not new dxcc on this band
-        if r3 :
+        if r3:
             return 'new_dxcc_band'
         return 'new_dxcc'
     # end def lookup
 
     color_lookup_table = dict \
         (( ('new_dxcc',      ('New DXCC',         'ctuple_dxcc'))
         ,  ('new_dxcc_band', ('New DXCC on Band', 'ctuple_dxcc_band'))
         ,  ('new_call',      ('New Call',         'ctuple_new_call'))
         ,  ('new_call_band', ('New Call on Band', 'ctuple_new_call_band'))
         ,  ('wbf',           ('Worked before',    'ctuple_wbf'))
         ,  ('highlight',     ('Highlight',        'ctuple_highlight'))
         ))
 
-    def lookup_verbose (self, band, call) :
+    def lookup_verbose (self, band, call):
         """ Look up the verbose description of worked-before status for
             this call for this band
         """
         status = self.lookup (band, call)
         return self.color_lookup_table [status][0]
     # end def lookup_verbose
 
-    def lookup_color (self, band, call) :
+    def lookup_color (self, band, call):
         """ Look up the color for this call for this band
             We to a simple lookup and map the result to a color.
             Involves checking of a new DXCC (on band or globally)
             and the check of a new call (on band or globally)
             The following test looks up RK0 which matches both, European
             Russia and Asiatic Russia.
         >>> w = Worked_Before ()
         >>> w.band_info ['40m'] = WBF ('40m')
         >>> w.dxcc_info ['40m'] = WBF ('40m')
         >>> w.dxcc_info ['ALL'] = WBF ('ALL')
-        >>> for code in ('054', '015') :
+        >>> for code in ('054', '015'):
         ...     w.dxcc_info ['40m'].add_item (code)
         ...     w.dxcc_info ['ALL'].add_item (code)
         >>> w.lookup_color ('40m', 'RK0') [1]
         QColor(alpha=65535, red=0, green=65535, blue=65535)
         """
         status = self.lookup (band, call)
         return getattr (self, self.color_lookup_table [status][1])
     # end def lookup_color
 
 # end class Worked_Before
 
-class QSO_Database_Worked_Before (Worked_Before) :
+class QSO_Database_Worked_Before (Worked_Before):
     """ Get DXCC data from QSO database
         This only gets a dxcc if the qso is *confirmed* in LOTW.
     """
 
     def __init__ \
         ( self, url, username, locator
         , adif = None
         , args = None
         , password = None
         , **kw
-        ) :
+        ):
         d = dict \
             ( url      = url
             , username = username
             , password = password
             , dry_run  = True
             )
-        if 'verbose' in kw :
+        if 'verbose' in kw:
             d.update (verbose = kw ['verbose'])
         self.au = ADIF_Uploader (** d)
         self.__super.__init__ (adif, args, **kw)
         self.locator = locator
         self.add_dxccs ()
     # end def __init__
 
-    def add_dxccs (self) :
+    def add_dxccs (self):
         # determine ham_call from locator
         d  = dict (gridsquare = self.locator)
         hc = self.au.get ('ham_call?' + urlencode (d))['data']['collection']
-        if len (hc) != 1 :
+        if len (hc) != 1:
             raise ValueError \
                 ("Ham Call with Loc=%s: Got %d entries"
                 % (self.locator, len (hc))
                 )
         d = dict (qsl_type = 'LOTW')
         d ['qso.owner'] = hc [0]['id']
         d ['@fields'] = 'qso.dxcc_entity.code,qso.band.name'
         d ['@sort']   = 'qso.band.name'
         qsls = self.au.get ('qsl?' + urlencode (d))['data']['collection']
-        for qsl in qsls :
+        for qsl in qsls:
             band = qsl ['qso.band.name']
             dxcc_code = qsl ['qso.dxcc_entity.code']
-            if band not in self.dxcc_info :
+            if band not in self.dxcc_info:
                 self.dxcc_info [band] = WBF (band)
             self.dxcc_info [band]. add_item (dxcc_code)
             self.dxcc_info ['ALL'].add_item (dxcc_code)
     # end def add_dxccs
 
-    def add_dxcc_entry (self, rec) :
+    def add_dxcc_entry (self, rec):
         """ Do nothing here: We update the DXCC map in add_dxccs
             and we do *not* mark newly-worked calls in the DXCC map:
             We only want LOTW-confirmed entries.
         """
         return
     # end def add_dxcc_entry
 
 # end class QSO_Database_Worked_Before
 
-def get_defaults () :
+def get_defaults ():
     home  = os.environ.get ('HOME', '')
     d     = {}
     d.update (adif_path = os.environ.get 
         ('WBF_PATH', os.path.join (home, '.local/share/WSJTX/wsjtx_log.adi')))
     d.update (call  = os.environ.get ('WBF_CALL',      'OE3RSU'))
     d.update (loc   = os.environ.get ('WBF_LOC',       'JN88dg'))
     d.update (user  = os.environ.get ('WBF_USER',      None))
     d.update (dburl = os.environ.get ('WBF_DBURL',     None))
     hl = [x.strip () for x in os.environ.get ('WBF_HIGHLIGHT', '').split (',')]
-    if hl :
-        d.update (highlight = hl)
+    if hl:
+        hd = {}
+        for h in hl:
+            try:
+                k, v = h.split (':')
+                hd [k] = int (v)
+            except ValueError:
+                hd [h] = None
+        d.update (highlight = hd)
     return d
 # end def get_defaults
 
-def default_cmd (defaults = None) :
-    if defaults is None :
+def default_cmd (defaults = None):
+    if defaults is None:
         defaults = get_defaults ()
+
+    class Dict_Append (Argparse_Action):
+        def __call__ (self, parser, namespace, values, option_string = None):
+            import pdb; pdb.set_trace ()
+            dst = getattr (namespace, self.dest)
+            try:
+                k, v = values.split (':')
+                dst.update (k, int (v))
+            except ValueError:
+                dst.update (values, None)
+        # end def __call__
+    # end class Dict_Append
+
     cmd = ArgumentParser ()
     cmd.add_argument \
         ( '-a', '--adif'
         , help    = 'ADIF file to parse, default=%(default)s'
         , default = defaults ['adif_path']
         )
     cmd.add_argument \
         ( "-d", "--highlight-dxcc"
         , help    = 'DXCC to highlight even if only new call on band'
-                    ' may be specified multiple times'
+                    ' may be specified multiple times, optionally this'
+                    ' can be NNN:count where NNN is the DXCC number and'
+                    ' count is the number of contacts for this dxcc, after'
+                    ' number has been reached no highlighting is performed'
         , default = defaults ['highlight']
-        , action  = 'append'
+        , action  = Dict_Append
         )
     cmd.add_argument \
         ( "-e", "--encoding"
         , help    = 'ADIF file character encoding, default=%(default)s'
         , default = 'utf-8'
         )
     cmd.add_argument \
@@ -1294,69 +1329,102 @@
         ( "-u", "--dbuser"
         , help    = 'User of qso tracker, default=%(default)s'
         , default = defaults ['user']
         )
     return cmd
 # end def default_cmd
 
-def get_wbf (cmd = None, defaults = None) :
-    if defaults is None :
+def get_wbf (cmd = None, defaults = None):
+    if defaults is None:
         defaults = get_defaults ()
-    if cmd is None :
+    if cmd is None:
         cmd = default_cmd (defaults)
         cmd.add_argument \
             ( "-c", "--callsign"
             , help    = 'Callsign of user of wsjtx, default=%(default)s'
             , default = defaults ['call']
             )
         cmd.add_argument \
             ( "-L", "--set-locator-msg"
             , help    = 'Set free-text message to locator message with '
                         '<dx-call> <own-call> report locator using EU-VHF '
                         'message'
             , action  = 'store_true'
             )
     args = cmd.parse_args ()
-    if args.dburl and args.dbuser :
+    if args.dburl and args.dbuser:
         wbf = QSO_Database_Worked_Before \
             ( url      = args.dburl
             , username = args.dbuser
             , password = args.password
             , locator  = args.locator
             , adif     = args.adif
             , args     = args
             )
-    else :
+    else:
         wbf = Worked_Before (args = args, adif = args.adif)
     return wbf
 # end def get_wbf
 
-def main (get_wbf = get_wbf) :
+def main (get_wbf = get_wbf):
     wbf  = get_wbf ()
     uc   = UDP_Connector (wbf)
     args = wbf.args
     weedout = \
         ( WSJTX_Decode, WSJTX_Status, WSJTX_Heartbeat, WSJTX_QSO_Logged
         , WSJTX_Logged_ADIF
         )
-    while 1 :
+    while 1:
         tel = uc.receive ()
         if not isinstance (tel, weedout):
             print (tel)
 # end def main
 
+def wbf (argv = None):
+    cmd = default_cmd ()
+    cmd.add_argument \
+        ( 'callsign'
+        , help    = 'Callsign(s) to look up'
+        , nargs   = '+'
+        )
+    cmd.add_argument \
+        ( '-b', '--band'
+        , help    = 'Band to do lookup for, default=%(default)s'
+        , default = '40m'
+        )
+    cmd.add_argument \
+        ( '-D', '--use-dxcc'
+        , help    = 'If specified, use dxcc list for call lookup'
+        , action  = 'store_true'
+        )
+
+    wbf  = get_wbf (cmd)
+    args = wbf.args
+    for callsign in args.callsign :
+        print (callsign, end = ': ')
+        entities = wbf.fuzzy_match_dxcc (callsign, use_dxcc = args.use_dxcc)
+        if entities :
+            print \
+                ( "Entities: %s"
+                % ', '.join ('%s (%s)' % (e.name, e.code) for e in entities)
+                )
+        else :
+            print ("No DXCC Entities found for this call")
+        print ('     WBF-Status: %s' % wbf.lookup_verbose (args.band, callsign))
+# end def wbf
+
 __all__ = [ "main", "QDateTime", "QColor", "color_red", "color_green"
           , "color_blue", "color_white", "color_black"
           , "color_cyan", "color_cyan1", "color_pink", "color_pink1"
           , "ctuple_invalid"
           , "WSJTX_Heartbeat", "WSJTX_Status", "WSJTX_Decode"
           , "WSJTX_Clear", "WSJTX_Reply", "WSJTX_QSO_Logged"
           , "WSJTX_Close", "WSJTX_Replay", "WSJTX_Halt_TX"
           , "WSJTX_Free_Text", "WSJTX_WSPR_Decode", "WSJTX_Location"
           , "WSJTX_Logged_ADIF", "WSJTX_Highlight_Call"
           , "WSJTX_Switch_Config", "WSJTX_Configure", "UDP_Connector"
           , "WBF", "Worked_Before", "get_defaults", "default_cmd"
           , "get_wbf"
           ]
 
-if __name__ == '__main__' :
+if __name__ == '__main__':
     main ()
```

### Comparing `wsjtx_srv-0.4/wsjtx_srv.egg-info/PKG-INFO` & `wsjtx_srv-0.5/wsjtx_srv.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 Metadata-Version: 2.1
 Name: wsjtx-srv
-Version: 0.4
+Version: 0.5
 Summary: Library implementation of WSJTX companion program
 Home-page: https://github.com/schlatterbeck/wsjtx-srv
 Author: Ralf Schlatterbeck
-Author-email: rsc@runtux.com
+Author-email: Ralf Schlatterbeck <rsc@runtux.com>
 License: BSD License
-Description: wsjtx-srv: Library for WSJT-X server implementation
-        ===================================================
-        
-        :Author: Ralf Schlatterbeck <rsc@runtux.com>
-        
-        This implements a simple UDP server that binds to the WSJT-X_ UDP message
-        protocol port. It also provides everything for parsing and/or generating
-        WSJT-X_ telegrams.
-        
-        By default calling ``wsjtx-srv`` will provide a simple server that
-        colors all callsigns not in the ADIF file for the current band. It uses
-        the ADIF logfile from WSJT-X_ with a default path to that file. You can
-        specify the correct path for your installation either via
-        command-line (call ``wsjtx-srv`` with the ``--help`` option) or in the
-        environment variable ``WBF_PATH``. It has also an implementation that
-        looks up DXCC-entities in my log database, but only those that have been
-        confirmed via LOTW.
-        
-        The implementation of ``wsjtx-srv`` should give a rough idea of how to use
-        this in your own projects.
-        
-        There is a companion-program ``wbf`` standing for *worked before* that
-        takes a number of callsigns on the command-line and tells you the worked
-        before status.
-        
-        .. _WSJT-X: https://physics.princeton.edu/pulsar/k1jt/wsjtx.html
-        
-        Changes
-        -------
-        
-        Version 0.3: Small fixes
-        
-        - Compatibility with older protocol versions, thanks to Sampo Savolainen
-          for the patch
-        - Fix band lookup if no QSO on band
-        
-        Version 0.2: Fix setup.py install_requires
-        
-        Version 0.1: Initial implementation
-        
-        - Implement serialization and deserialization of WSJT-X_ telegrams and a
-          simple server
-        - First Release
-        
-        
+Project-URL: Homepage, https://github.com/schlatterbeck/wsjtx-srv
+Project-URL: Bug Tracker, https://github.com/schlatterbeck/wsjtx-srv/issues
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+wsjtx-srv: Library for WSJT-X server implementation
+===================================================
+
+:Author: Ralf Schlatterbeck <rsc@runtux.com>
+
+This implements a simple UDP server that binds to the WSJT-X_ UDP message
+protocol port. It also provides everything for parsing and/or generating
+WSJT-X_ telegrams.
+
+By default calling ``wsjtx-srv`` will provide a simple server that
+colors all callsigns not in the ADIF file for the current band. It uses
+the ADIF logfile from WSJT-X_ with a default path to that file. You can
+specify the correct path for your installation either via
+command-line (call ``wsjtx-srv`` with the ``--help`` option) or in the
+environment variable ``WBF_PATH``. It has also an implementation that
+looks up DXCC-entities in my log database, but only those that have been
+confirmed via LOTW.
+
+The implementation of ``wsjtx-srv`` should give a rough idea of how to use
+this in your own projects.
+
+There is a companion-program ``wbf`` standing for *worked before* that
+takes a number of callsigns on the command-line and tells you the worked
+before status.
+
+.. _WSJT-X: https://physics.princeton.edu/pulsar/k1jt/wsjtx.html
+
+Changes
+-------
+
+Version 0.5: Add pyproject.toml
+
+- Installation with new setuptools again possible
+
+Version 0.4: Move to setuptools
+
+- Seems previous releases had versioning problems with pypi
+
+Version 0.3: Small fixes
+
+- Compatibility with older protocol versions, thanks to Sampo Savolainen
+  for the patch
+- Fix band lookup if no QSO on band
+
+Version 0.2: Fix setup.py install_requires
+
+Version 0.1: Initial implementation
+
+- Implement serialization and deserialization of WSJT-X_ telegrams and a
+  simple server
+- First Release
+
```

