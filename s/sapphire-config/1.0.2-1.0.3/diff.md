# Comparing `tmp/sapphire_config-1.0.2.tar.gz` & `tmp/sapphire_config-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapphire_config-1.0.2.tar", last modified: Mon Jul 17 22:45:31 2023, max compression
+gzip compressed data, was "sapphire_config-1.0.3.tar", last modified: Mon Jul 24 19:57:33 2023, max compression
```

## Comparing `sapphire_config-1.0.2.tar` & `sapphire_config-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1070 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/LICENSE
--rw-rw-r--   0 valentic   (500) valentic   (500)       98 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/MANIFEST.in
--rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      199 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/README.md
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/examples/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/examples/components/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1042 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/examples/components/demo.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     2830 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/examples/components/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/examples/config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      982 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/examples/config/demo.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     4932 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/examples/config/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      996 2023-07-06 02:17:33.000000 sapphire_config-1.0.2/pyproject.toml
--rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/setup.cfg
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      251 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/src/sapphire_config/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5139 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/src/sapphire_config/component.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-17 22:41:43.000000 sapphire_config-1.0.2/src/sapphire_config/metadata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     9320 2023-07-17 22:43:44.000000 sapphire_config-1.0.2/src/sapphire_config/parser.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      588 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/SOURCES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/dependency_links.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       92 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/requires.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       16 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/top_level.txt
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/tests/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/tests/__pycache__/
--rw-rw-r--   0 valentic   (500) valentic   (500)    26765 2023-07-06 02:17:26.000000 sapphire_config-1.0.2/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc
--rw-rw-r--   0 valentic   (500) valentic   (500)    15474 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/tests/test_sapphireconfig.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1070 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/LICENSE
+-rw-rw-r--   0 valentic   (500) valentic   (500)       98 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/MANIFEST.in
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      199 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/README.md
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/examples/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/examples/components/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1042 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/examples/components/demo.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2830 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/examples/components/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/examples/config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      982 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/examples/config/demo.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     4932 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/examples/config/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      996 2023-07-06 02:17:33.000000 sapphire_config-1.0.3/pyproject.toml
+-rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/setup.cfg
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      251 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/src/sapphire_config/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5139 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/src/sapphire_config/component.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-24 18:36:09.000000 sapphire_config-1.0.3/src/sapphire_config/metadata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10027 2023-07-24 19:55:14.000000 sapphire_config-1.0.3/src/sapphire_config/parser.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      655 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       92 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/requires.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       16 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/top_level.txt
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/tests/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/tests/__pycache__/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    84897 2023-07-24 19:55:12.000000 sapphire_config-1.0.3/tests/__pycache__/test_sapphireconfig.cpython-311-pytest-7.4.0.pyc
+-rw-rw-r--   0 valentic   (500) valentic   (500)    26765 2023-07-06 02:17:26.000000 sapphire_config-1.0.3/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc
+-rw-rw-r--   0 valentic   (500) valentic   (500)    17175 2023-07-24 19:55:10.000000 sapphire_config-1.0.3/tests/test_sapphireconfig.py
```

### Comparing `sapphire_config-1.0.2/LICENSE` & `sapphire_config-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.2/PKG-INFO` & `sapphire_config-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapphire_config
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sapphire Configuration Parser
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Todd Valentic
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sapphire_config-1.0.2/examples/components/demo.conf` & `sapphire_config-1.0.3/examples/components/demo.conf`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.2/examples/components/demo.py` & `sapphire_config-1.0.3/examples/components/demo.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.2/examples/config/demo.conf` & `sapphire_config-1.0.3/examples/config/demo.conf`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.2/examples/config/demo.py` & `sapphire_config-1.0.3/examples/config/demo.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.2/pyproject.toml` & `sapphire_config-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.2/src/sapphire_config/component.py` & `sapphire_config-1.0.3/src/sapphire_config/component.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.2/src/sapphire_config/parser.py` & `sapphire_config-1.0.3/src/sapphire_config/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,27 @@
 #
 #   2023-06-17  Todd Valentic
 #               PEP8 compliance
 #
 #   2023-07-17  Todd Valentic
 #               Change Rate offset default to 0 from None
 #
+#   2023-07-24  Todd Valentic
+#               Add Rate.nexttime()
+#
 ##########################################################################
 
 import configparser as cp
 import datetime
 import importlib
 import pathlib
 import re
 
+from typing import Union
+
 from dateutil.relativedelta import relativedelta
 import dateutil.parser
 import humanfriendly
 import pytimeparse2 as pytimeparse
 
 # -------------------------------------------------------------------------
 #   Types
@@ -39,43 +44,61 @@
 
 
 class Rate:
     """Repeating event specification"""
 
     def __init__(
         self,
-        period: datetime.timedelta,
+        period: Union[int, float, datetime.timedelta],
         sync: bool = False,
-        offset: datetime.timedelta = 0,
+        offset: Union[int, float, datetime.timedelta] = 0,
         at_start: bool = False,
     ):
+        if isinstance(period, (float, int)):
+            period = datetime.timedelta(seconds=period)
+
+        if isinstance(offset, (float, int)):
+            offset = datetime.timedelta(seconds=offset)
+
         self.period = period
         self.sync = sync
         self.offset = offset
         self.at_start = at_start
 
     def __repr__(self):
         return (
             f"<Rate "
             f"period={self.period}, "
             f"sync={self.sync}, "
-            f"offset={self.period}, "
+            f"offset={self.offset}, "
             f"at_start={self.at_start}"
             f">"
         )
 
     def __eq__(self, other):
         return (
             self.period == other.period
             and self.sync == other.sync
             and self.offset == other.offset
             and self.at_start == other.at_start
         )
 
+    def nexttime(self, curtime: datetime.datetime):
+        """Seconds until next deadline""" 
+
+        period = self.period.total_seconds()
+
+        if self.sync:
+            timestamp = (curtime - self.offset).timestamp() 
+            wait = period - timestamp % period
+        else:
+            wait = period
 
+        return datetime.timedelta(seconds = wait)
+        
 # -------------------------------------------------------------------------
 #   Converters
 # -------------------------------------------------------------------------
 
 
 def as_datetime(value):
     """Convert to datetime"""
```

### Comparing `sapphire_config-1.0.2/src/sapphire_config.egg-info/PKG-INFO` & `sapphire_config-1.0.3/src/sapphire_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapphire-config
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sapphire Configuration Parser
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Todd Valentic
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sapphire_config-1.0.2/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc` & `sapphire_config-1.0.3/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.2/tests/test_sapphireconfig.py` & `sapphire_config-1.0.3/tests/test_sapphireconfig.py`

 * *Files 7% similar despite different names*

```diff
@@ -437,14 +437,74 @@
 
     period = datetime.timedelta(seconds=60)
     rate = sapphire.Rate(period)
 
     result = config['section'].get_rate('missing', fallback=rate)
     assert result == rate
 
+def test_rate_init_default():
+    rate = sapphire.Rate(0)
+
+    assert isinstance(rate.period, datetime.timedelta) 
+    assert isinstance(rate.offset, datetime.timedelta)
+    assert rate.period.total_seconds() == 0
+    assert rate.offset.total_seconds() == 0
+    assert rate.sync == False
+    assert rate.at_start == False
+
+def test_rate_init_timedelta():
+    period = datetime.timedelta(0)
+    offset = datetime.timedelta(0)
+    rate = sapphire.Rate(period, offset)
+
+    assert isinstance(rate.period, datetime.timedelta) 
+    assert isinstance(rate.offset, datetime.timedelta)
+    assert rate.period.total_seconds() == 0
+    assert rate.offset.total_seconds() == 0
+
+def test_rate_nexttime():
+    rate = sapphire.Rate(60, sync=False)
+
+    curtime = datetime.datetime(2001, 1, 1, 0, 0, 5)
+
+    wait = rate.nexttime(curtime)
+    assert wait.total_seconds() == 60 
+
+def test_rate_nexttime_sync():
+    rate = sapphire.Rate(60, sync=True)
+
+    curtime = datetime.datetime(2001, 1, 1, 0, 0, 5)
+
+    wait = rate.nexttime(curtime)
+    assert wait.total_seconds() == 55 
+
+def test_rate_nexttime_offset():
+    rate = sapphire.Rate(60, offset=10)
+
+    curtime = datetime.datetime(2001, 1, 1, 0, 0, 5)
+
+    wait = rate.nexttime(curtime)
+    assert wait.total_seconds() == 60 
+
+def test_rate_nexttime_offset_sync():
+    rate = sapphire.Rate(60, offset=10, sync=True)
+
+    curtime = datetime.datetime(2001, 1, 1, 0, 0, 5)
+
+    wait = rate.nexttime(curtime)
+    assert wait.total_seconds() == 5 
+
+def test_rate_nexttime_offset_sync2():
+    rate = sapphire.Rate(60, offset=10, sync=True)
+
+    curtime = datetime.datetime(2001, 1, 1, 0, 0, 15)
+
+    wait = rate.nexttime(curtime)
+    assert wait.total_seconds() == 55
+
 def test_get_components():
     config = sapphire.Parser()
     config['section'] = {}
     config['section']['components'] = 'a b'
 
     result = config.get_components('section', 'components', factory=Factory)
     assert isinstance(result, dict)
```

