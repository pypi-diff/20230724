# Comparing `tmp/ezgpx-0.1.4.tar.gz` & `tmp/ezgpx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezgpx-0.1.4.tar", last modified: Thu Jul 20 13:03:02 2023, max compression
+gzip compressed data, was "ezgpx-0.1.5.tar", last modified: Mon Jul 24 14:29:50 2023, max compression
```

## Comparing `ezgpx-0.1.4.tar` & `ezgpx-0.1.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.621218 ezgpx-0.1.4/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    35149 2023-06-06 11:52:29.000000 ezgpx-0.1.4/LICENSE
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2158 2023-07-20 13:03:02.621218 ezgpx-0.1.4/PKG-INFO
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1179 2023-07-19 12:57:20.000000 ezgpx-0.1.4/README.md
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.617218 ezgpx-0.1.4/ezgpx/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       98 2023-06-08 09:27:44.000000 ezgpx-0.1.4/ezgpx/__init__.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.617218 ezgpx-0.1.4/ezgpx/gpx/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       18 2023-06-08 09:30:14.000000 ezgpx-0.1.4/ezgpx/gpx/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    25437 2023-07-20 12:51:00.000000 ezgpx-0.1.4/ezgpx/gpx/gpx.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.617218 ezgpx-0.1.4/ezgpx/gpx_elements/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      324 2023-07-03 09:39:46.000000 ezgpx-0.1.4/ezgpx/gpx_elements/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      892 2023-07-03 09:53:44.000000 ezgpx-0.1.4/ezgpx/gpx_elements/bounds.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      717 2023-07-03 09:49:36.000000 ezgpx-0.1.4/ezgpx/gpx_elements/copyright.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      553 2023-07-03 09:50:23.000000 ezgpx-0.1.4/ezgpx/gpx_elements/email.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2855 2023-07-03 09:50:51.000000 ezgpx-0.1.4/ezgpx/gpx_elements/extensions.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    16025 2023-07-14 14:04:08.000000 ezgpx-0.1.4/ezgpx/gpx_elements/gpx.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      680 2023-07-03 09:51:43.000000 ezgpx-0.1.4/ezgpx/gpx_elements/link.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1596 2023-07-03 09:52:07.000000 ezgpx-0.1.4/ezgpx/gpx_elements/metadata.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      730 2023-07-03 09:52:28.000000 ezgpx-0.1.4/ezgpx/gpx_elements/person.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1026 2023-07-03 12:48:14.000000 ezgpx-0.1.4/ezgpx/gpx_elements/point.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      504 2023-07-03 09:53:32.000000 ezgpx-0.1.4/ezgpx/gpx_elements/point_segment.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1545 2023-07-03 09:54:14.000000 ezgpx-0.1.4/ezgpx/gpx_elements/route.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1790 2023-07-14 14:04:26.000000 ezgpx-0.1.4/ezgpx/gpx_elements/track.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      938 2023-07-14 14:04:53.000000 ezgpx-0.1.4/ezgpx/gpx_elements/track_segment.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     3855 2023-07-14 14:32:30.000000 ezgpx-0.1.4/ezgpx/gpx_elements/way_point.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.617218 ezgpx-0.1.4/ezgpx/gpx_parser/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       21 2023-06-07 12:15:07.000000 ezgpx-0.1.4/ezgpx/gpx_parser/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    24179 2023-07-18 07:14:14.000000 ezgpx-0.1.4/ezgpx/gpx_parser/parser.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.621218 ezgpx-0.1.4/ezgpx/gpx_writer/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       21 2023-06-07 08:52:43.000000 ezgpx-0.1.4/ezgpx/gpx_writer/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    24207 2023-07-18 07:22:11.000000 ezgpx-0.1.4/ezgpx/gpx_writer/writer.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.621218 ezgpx-0.1.4/ezgpx/utils/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       76 2023-06-27 12:31:11.000000 ezgpx-0.1.4/ezgpx/utils/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1494 2023-06-28 13:57:41.000000 ezgpx-0.1.4/ezgpx/utils/algorithms.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2633 2023-07-18 15:26:00.000000 ezgpx-0.1.4/ezgpx/utils/distance.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2672 2023-07-14 14:27:06.000000 ezgpx-0.1.4/ezgpx/utils/projections.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.617218 ezgpx-0.1.4/ezgpx.egg-info/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2158 2023-07-20 13:03:02.000000 ezgpx-0.1.4/ezgpx.egg-info/PKG-INFO
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      978 2023-07-20 13:03:02.000000 ezgpx-0.1.4/ezgpx.egg-info/SOURCES.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2023-07-20 13:03:02.000000 ezgpx-0.1.4/ezgpx.egg-info/dependency_links.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       47 2023-07-20 13:03:02.000000 ezgpx-0.1.4/ezgpx.egg-info/requires.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       12 2023-07-20 13:03:02.000000 ezgpx-0.1.4/ezgpx.egg-info/top_level.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2023-07-20 13:03:02.621218 ezgpx-0.1.4/setup.cfg
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1727 2023-07-20 13:02:53.000000 ezgpx-0.1.4/setup.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.621218 ezgpx-0.1.4/tests/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        0 2023-06-07 13:13:09.000000 ezgpx-0.1.4/tests/__init__.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-20 13:03:02.621218 ezgpx-0.1.4/tests/dev_tests/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        0 2023-06-07 13:13:13.000000 ezgpx-0.1.4/tests/dev_tests/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     3193 2023-07-18 12:25:14.000000 ezgpx-0.1.4/tests/test_GPX.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1747 2023-07-18 12:27:24.000000 ezgpx-0.1.4/tests/test_utils.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.091924 ezgpx-0.1.5/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    35149 2023-06-06 11:52:29.000000 ezgpx-0.1.5/LICENSE
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2158 2023-07-24 14:29:50.091924 ezgpx-0.1.5/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1179 2023-07-19 12:57:20.000000 ezgpx-0.1.5/README.md
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.083924 ezgpx-0.1.5/ezgpx/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       98 2023-06-08 09:27:44.000000 ezgpx-0.1.5/ezgpx/__init__.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.083924 ezgpx-0.1.5/ezgpx/gpx/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       18 2023-06-08 09:30:14.000000 ezgpx-0.1.5/ezgpx/gpx/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    35639 2023-07-24 13:31:56.000000 ezgpx-0.1.5/ezgpx/gpx/gpx.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.087924 ezgpx-0.1.5/ezgpx/gpx_elements/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      324 2023-07-03 09:39:46.000000 ezgpx-0.1.5/ezgpx/gpx_elements/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      892 2023-07-03 09:53:44.000000 ezgpx-0.1.5/ezgpx/gpx_elements/bounds.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      717 2023-07-03 09:49:36.000000 ezgpx-0.1.5/ezgpx/gpx_elements/copyright.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      553 2023-07-03 09:50:23.000000 ezgpx-0.1.5/ezgpx/gpx_elements/email.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2855 2023-07-03 09:50:51.000000 ezgpx-0.1.5/ezgpx/gpx_elements/extensions.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    24767 2023-07-24 13:47:37.000000 ezgpx-0.1.5/ezgpx/gpx_elements/gpx.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      680 2023-07-03 09:51:43.000000 ezgpx-0.1.5/ezgpx/gpx_elements/link.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1596 2023-07-03 09:52:07.000000 ezgpx-0.1.5/ezgpx/gpx_elements/metadata.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      730 2023-07-03 09:52:28.000000 ezgpx-0.1.5/ezgpx/gpx_elements/person.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1026 2023-07-03 12:48:14.000000 ezgpx-0.1.5/ezgpx/gpx_elements/point.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      595 2023-07-23 14:49:38.000000 ezgpx-0.1.5/ezgpx/gpx_elements/point_segment.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1637 2023-07-23 14:50:06.000000 ezgpx-0.1.5/ezgpx/gpx_elements/route.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1892 2023-07-23 14:51:01.000000 ezgpx-0.1.5/ezgpx/gpx_elements/track.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1030 2023-07-23 14:50:40.000000 ezgpx-0.1.5/ezgpx/gpx_elements/track_segment.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     4143 2023-07-24 13:15:21.000000 ezgpx-0.1.5/ezgpx/gpx_elements/way_point.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.087924 ezgpx-0.1.5/ezgpx/gpx_parser/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       21 2023-06-07 12:15:07.000000 ezgpx-0.1.5/ezgpx/gpx_parser/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    24702 2023-07-23 14:46:38.000000 ezgpx-0.1.5/ezgpx/gpx_parser/parser.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.087924 ezgpx-0.1.5/ezgpx/gpx_writer/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       21 2023-06-07 08:52:43.000000 ezgpx-0.1.5/ezgpx/gpx_writer/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    24325 2023-07-22 13:28:10.000000 ezgpx-0.1.5/ezgpx/gpx_writer/writer.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.091924 ezgpx-0.1.5/ezgpx/utils/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       76 2023-06-27 12:31:11.000000 ezgpx-0.1.5/ezgpx/utils/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1494 2023-06-28 13:57:41.000000 ezgpx-0.1.5/ezgpx/utils/algorithms.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2633 2023-07-18 15:26:00.000000 ezgpx-0.1.5/ezgpx/utils/distance.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2672 2023-07-14 14:27:06.000000 ezgpx-0.1.5/ezgpx/utils/projections.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.083924 ezgpx-0.1.5/ezgpx.egg-info/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2158 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      978 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       47 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/requires.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       12 2023-07-24 14:29:49.000000 ezgpx-0.1.5/ezgpx.egg-info/top_level.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2023-07-24 14:29:50.091924 ezgpx-0.1.5/setup.cfg
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1727 2023-07-24 14:29:43.000000 ezgpx-0.1.5/setup.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.091924 ezgpx-0.1.5/tests/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        0 2023-06-07 13:13:09.000000 ezgpx-0.1.5/tests/__init__.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-24 14:29:50.091924 ezgpx-0.1.5/tests/dev_tests/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        0 2023-06-07 13:13:13.000000 ezgpx-0.1.5/tests/dev_tests/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     4634 2023-07-22 13:05:48.000000 ezgpx-0.1.5/tests/test_GPX.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1922 2023-07-24 13:53:40.000000 ezgpx-0.1.5/tests/test_utils.py
```

### Comparing `ezgpx-0.1.4/LICENSE` & `ezgpx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/PKG-INFO` & `ezgpx-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezgpx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy to use Python GPX library
 Home-page: https://pypi.org/project/ezgpx/
 Download-URL: https://github.com/FABallemand/ezGPX
 Author: Fabien ALLEMAND
 Author-email: allemand.fabien@orange.fr
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/FABallemand/ezGPX/issues
```

### Comparing `ezgpx-0.1.4/README.md` & `ezgpx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx/gpx.py` & `ezgpx-0.1.5/ezgpx/gpx/gpx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,78 @@
 import os
-from typing import Optional, Union
+from typing import Optional, Union, NewType
 import logging
 import webbrowser
 from datetime import datetime
 import pandas as pd
 from math import degrees
 
+from matplotlib.axes import Axes
 from matplotlib.figure import Figure
+import matplotlib.colors
 import matplotlib.pyplot as plt
 from mpl_toolkits.basemap import Basemap
 
 import gmplot
 
 import folium
 from folium.plugins import MiniMap
 from folium.features import DivIcon
 
 from ..gpx_elements import Gpx, WayPoint
 from ..gpx_parser import Parser
 from ..gpx_writer import Writer
 from ..utils import EARTH_RADIUS
 
+GPX = NewType("GPX", object) # GPX forward declaration for type hint
 
 class GPX():
     """
     High level GPX object.
     """
 
-    def __init__(self, file_path: str):
-        self.file_path: str = file_path
-        self.parser: Parser = Parser(file_path)
-        self.gpx: Gpx = self.parser.gpx
-        self.writer: Writer = Writer(
-            self.gpx, precisions=self.parser.precisions, time_format=self.parser.time_format)
+    def __init__(self, file_path: Optional[str] = None) -> None:
+        if file_path is not None:
+            self.file_path: str = file_path
+            self.parser: Parser = Parser(file_path)
+            self.gpx: Gpx = self.parser.gpx
+            self.writer: Writer = Writer(
+                self.gpx, precisions=self.parser.precisions, time_format=self.parser.time_format)
+        else:
+            pass
+
+    def __str__(self) -> str:
+        return f"file_path = {self.file_path}\nparser = {self.parser}\ngpx = {self.gpx}\nwriter = {self.writer}"
+        
+    def file_name(self) -> Union[str, None]:
+        """
+        Return .gpx file name.
+
+        Returns:
+            str: File name.
+        """
+        return os.path.basename(self.file_path)
 
     def name(self) -> str:
         """
         Return activity name.
 
         Returns:
             str: Activity name.
         """
         return self.gpx.name()
+    
+    def set_name(self, new_name: str) -> None:
+        """
+        Set name.
+
+        Args:
+            new_name (str): New name.
+        """
+        self.gpx.set_name(new_name)
 
     def nb_points(self) -> int:
         """
         Return the number of points in the GPX.
 
         Returns:
             int: Number of points in the GPX.
@@ -55,24 +82,24 @@
     def first_point(self) -> WayPoint:
         """
         Return GPX first point.
 
         Returns:
             WayPoint: First point.
         """
-        return self.gpx.tracks[0].trkseg[0].trkpt[0]
+        return self.gpx.first_point()
 
     def last_point(self) -> WayPoint:
         """
         Return GPX last point.
 
         Returns:
             WayPoint: Last point.
         """
-        return self.gpx.tracks[-1].trkseg[-1].trkpt[-1]
+        return self.gpx.last_point()
 
     def bounds(self) -> tuple[float, float, float, float]:
         """
         Find minimum and maximum latitude and longitude.
 
         Returns:
             tuple[float, float, float, float]: Min latitude, min longitude, max latitude, max longitude
@@ -110,14 +137,38 @@
         """
         Returns the descent (meters) of the tracks contained in the GPX.
 
         Returns:
             float: Descent (meters).
         """
         return self.gpx.descent()
+    
+    def compute_points_ascent_rate(self) -> None:
+        """
+        Compute ascent rate at each point.
+        """
+        self.gpx.compute_points_ascent_rate()
+
+    def min_ascent_rate(self) -> float:
+        """
+        Return activity minimum ascent rate.
+
+        Returns:
+            float: Minimum ascent rate.
+        """
+        return self.gpx.min_ascent_rate()
+    
+    def max_ascent_rate(self) -> float:
+        """
+        Return activity maximum ascent rate.
+
+        Returns:
+            float: Maximum ascent rate.
+        """
+        return self.gpx.max_ascent_rate()
 
     def min_elevation(self) -> float:
         """
         Returns the minimum elevation (meters) in the tracks contained in the GPX.
 
         Returns:
             float: Minimum elevation (meters).
@@ -191,19 +242,39 @@
         """
         Return average moving speed (kilometers per hour) during the activity.
 
         Returns:
             float: Average moving speed (kilometers per hour).
         """
         return self.gpx.avg_moving_speed()
+    
+    def compute_points_speed(self) -> None:
+        """
+        Compute speed (kilometers per hour) at each track point.
+        """
+        self.gpx.compute_points_speed()
+
+    def min_speed(self) -> float:
+        """
+        Return the minimum speed during the activity.
+
+        Returns:
+            float: Minimum speed.
+        """
+        return self.gpx.min_speed()
 
     def max_speed(self) -> float:
-        # TODO
-        pass
+        """
+        Return the maximum speed during the activity.
 
+        Returns:
+            float: Maximum speed.
+        """
+        return self.gpx.max_speed()
+    
     def avg_pace(self) -> float:
         """
         Return average pace (minutes per kilometer) during the activity.
 
         Returns:
             float: Average pace (minutes per kilometer).
         """
@@ -213,41 +284,44 @@
         """
         Return average moving pace (minutes per kilometer) during the activity.
 
         Returns:
             float: Average moving pace (minutes per kilometer).
         """
         return self.gpx.avg_moving_pace()
-
-    def to_string(self) -> str:
+    
+    def compute_points_pace(self) -> None:
         """
-        Convert the GPX object to a string.
-
-        Returns:
-            str: String representingth GPX object.
+        Compute pace at each track point.
         """
-        return self.writer.gpx_to_string(self.gpx)
+        self.gpx.compute_points_pace()
 
-    def to_gpx(self, path: str):
+    def min_pace(self) -> float:
         """
-        Write the GPX object to a .gpx file.
+        Return the minimum pace during the activity.
 
-        Args:
-            path (str): Path to the .gpx file.
+        Returns:
+            float: Minimum pace.
         """
-        self.writer.write(path)
+        return self.gpx.min_pace()
 
-    def to_dataframe(self) -> pd.DataFrame:
+    def max_pace(self) -> float:
         """
-        Convert GPX object to Pandas Dataframe.
+        Return the maximum pace during the activity.
 
         Returns:
-            pd.DataFrame: Dataframe containing position data from GPX.
+            float: Maximum pace.
+        """
+        return self.gpx.max_pace()
+    
+    def compute_points_ascent_speed(self) -> None:
         """
-        return self.gpx.to_dataframe()
+        Compute ascent speed (kilometers per hour) at each track point.
+        """
+        self.gpx.compute_points_ascent_speed()
 
     def remove_metadata(self):
         """
         Remove metadata (ie: metadata will not be written when saving the GPX object as a .gpx file).
         """
         self.writer.metadata = False
 
@@ -287,14 +361,114 @@
             tolerance (float, optional): Tolerance (meters). Corresponds to the
             minimum distance between the point and the track before the point
             is removed. Defaults to 2.
         """
         epsilon = degrees(tolerance/EARTH_RADIUS)
         self.gpx.simplify(epsilon)
 
+    def merge(self, gpx: GPX):
+        
+        if self.gpx.tag is None:
+            self.gpx.tag = gpx.gpx.tag
+        if self.gpx.creator is None:
+            self.gpx.creator = gpx.gpx.creator
+        if self.gpx.xmlns is None:
+            self.gpx.xmlns = gpx.gpx.xmlns
+        if self.gpx.version is None:
+            self.gpx.version = gpx.gpx.version
+        if self.gpx.xmlns_xsi is None:
+            self.gpx.xmlns_xsi = gpx.gpx.xmlns_xsi
+        self.gpx.xsi_schema_location.extend(gpx.gpx.xsi_schema_location)
+        if self.gpx.xmlns_gpxtpx is None:
+            self.gpx.xmlns_gpxtpx = gpx.gpx.xmlns_gpxtpx
+        if self.gpx.xmlns_gpxx is None:
+            self.gpx.xmlns_gpxx = gpx.gpx.xmlns_gpxx
+        if self.gpx.xmlns_gpxtrk is None:
+            self.gpx.xmlns_gpxtrk = gpx.gpx.xmlns_gpxtrk
+        if self.gpx.xmlns_wptx1 is None:
+            self.gpx.xmlns_wptx1 = gpx.gpx.xmlns_wptx1
+        if self.gpx.metadata is None:
+            self.gpx.metadata = gpx.gpx.metadata
+        self.gpx.wpt.extend(gpx.gpx.wpt)
+        self.gpx.rte.extend(gpx.gpx.rte)
+        self.gpx.tracks.extend(gpx.gpx.tracks)
+        if self.gpx.extensions is None:
+            self.gpx.extensions = gpx.gpx.extensions
+
+    def to_string(self) -> str:
+        """
+        Convert the GPX object to a string.
+
+        Returns:
+            str: String representingth GPX object.
+        """
+        return self.writer.gpx_to_string(self.gpx)
+    
+    def to_dataframe(
+            self,
+            projection: bool = False,
+            elevation: bool = True,
+            speed: bool = False,
+            pace: bool = False,
+            ascent_rate: bool = False,
+            ascent_speed: bool = False) -> pd.DataFrame:
+        """
+        Convert GPX object to Pandas Dataframe.
+
+        Args:
+            projection (bool, optional): Toggle projection. Defaults to False.
+            elevation (bool, optional): Toggle elevation. Defaults to True.
+            speed (bool, optional): Toggle speed. Defaults to False.
+            pace (bool, optional): Toggle pace. Defaults to False.
+            ascent_rate (bool, optional): Toggle ascent rate. Defaults to False.
+            ascent_speed (bool, optional): Toggle ascent speed. Defaults to False.
+
+        Returns:
+            pd.DataFrame: Dataframe containing data from GPX.
+        """
+        return self.gpx.to_dataframe(projection, elevation, speed, pace, ascent_rate, ascent_speed)
+
+    def to_gpx(self, path: str):
+        """
+        Write the GPX object to a .gpx file.
+
+        Args:
+            path (str): Path to the .gpx file.
+        """
+        self.writer.write(path)
+
+    def to_csv(
+            self,
+            projection: bool = False,
+            elevation: bool = True,
+            speed: bool = False,
+            pace: bool = False,
+            ascent_rate: bool = False,
+            ascent_speed: bool = False,
+            path: str = "unnamed.csv",
+            sep: str = ",",
+            header: bool = True,
+            index: bool = False):
+        """
+        Write the GPX object track coordinates to a .csv file.
+
+        Args:
+            projection (bool, optional): Toogle projected coordinates. Defaults to False.
+            elevation (bool, optional): Toggle elevation. Defaults to True.
+            speed (bool, optional): Toggle speed. Defaults to False.
+            pace (bool, optional): Toggle pace. Defaults to False.
+            ascent_rate (bool, optional): Toggle ascent rate. Defaults to False.
+            ascent_speed (bool, optional): Toggle ascent speed. Defaults to False.
+            path (str, optional): Path. Defaults to "unnamed.csv".
+            sep (str, optional): Separator. Defaults to ",".
+            header (bool, optional): Toggle header. Defaults to True.
+            index (bool, optional): Toggle index. Defaults to False.
+        """
+        self.to_dataframe(projection, elevation, speed, pace, ascent_rate, ascent_speed).to_csv(path, sep=sep, header=header, index=index)
+
     def _matplotlib_plot_text(
             self,
             fig: Figure,
             duration: Optional[tuple[float, float]] = (0, 0),
             distance: Optional[tuple[float, float]] = (0.5, 0),
             ascent: Optional[tuple[float, float]] = (1, 0),
             pace: Optional[tuple[float, float]] = (1, 0),
@@ -337,45 +511,91 @@
 
         elif speed is not None:
             plt.text(speed[0], speed[1],
                      f"Speed:\n{self.avg_speed():.2f} km/h", **text_parameters)
 
     def matplotlib_axes_plot(
             self,
-            axes,
+            axes: Axes,
             projection: Optional[str] = None,
-            base_color: str = "#101010",
-            elevation_color: bool = False,
+            color: str = "#101010",
+            colorbar: bool = False,
             start_stop_colors: Optional[tuple[str, str]] = None,
             way_points_color: Optional[str] = None,
             title: Optional[str] = None,
             duration: Optional[tuple[float, float]] = None,
             distance: Optional[tuple[float, float]] = None,
             ascent: Optional[tuple[float, float]] = None,
             pace: Optional[tuple[float, float]] = None,
-            speed: Optional[tuple[float, float]] = None,
-            file_path: Optional[str] = None):
+            speed: Optional[tuple[float, float]] = None):
+        """
+        Plot GPX on Matplotlib axes.
+
+        Args:
+            axes (matplotlib.axes.Axes): Axes to plot on.
+            projection (Optional[str], optional): Projection. Defaults to None.
+            color (str, optional): A color string (ie: "#FF0000" or "red") or a track attribute ("elevation", "speed", "pace", "vertical_drop", "ascent_rate", "ascent_speed") Defaults to "#101010".
+            colorbar (bool, optional): Colorbar toggle. Defaults to False.
+            elevation_color (bool, optional): Color track according to elevation. Defaults to False.
+            start_stop_colors (tuple[str, str], optional): Start and stop points colors. Defaults to False.
+            way_points_color (str, optional): Way point color. Defaults to False.
+            title (Optional[str], optional): Title. Defaults to None.
+            duration (Optional[tuple[float, float]], optional): Display duration. Defaults to None.
+            distance (Optional[tuple[float, float]], optional): Display distance. Defaults to None.
+            ascent (Optional[tuple[float, float]], optional): Display ascent. Defaults to None.
+            pace (Optional[tuple[float, float]], optional): Display pace. Defaults to None.
+            speed (Optional[tuple[float, float]], optional): Display pace. Defaults to None.
+        """
+        # Clear axes
+        axes.clear()
+
         # Handle projection (select dataframe columns to use and project if needed)
         if projection is None:
-            column_x = "longitude"
-            column_y = "latitude"
+            column_x = "lon"
+            column_y = "lat"
         else:
             column_x = "x"
             column_y = "y"
             self.gpx.project(projection)  # Project all track points
 
         # Create dataframe containing data from the GPX file
-        gpx_df = self.to_dataframe()
+        gpx_df = self.to_dataframe(projection=True, elevation=True, speed=True, pace=True, ascent_rate=True, ascent_speed=True)
 
         # Scatter all track points
-        if elevation_color:
-            axes.scatter(gpx_df[column_x], gpx_df[column_y],
-                        c=gpx_df["elevation"])
+        if color == "elevation":
+            cmap = matplotlib.colors.LinearSegmentedColormap.from_list("", ["green","blue"])
+            im = axes.scatter(gpx_df[column_x], gpx_df[column_y],
+                        c=gpx_df["ele"], cmap=cmap)
+        elif color == "speed":
+            # cmap = matplotlib.colors.LinearSegmentedColormap.from_list("", ["lightskyblue", "deepskyblue", "blue", "mediumblue", "midnightblue"])
+            cmap = matplotlib.colors.LinearSegmentedColormap.from_list("", ["lightskyblue", "mediumblue", "midnightblue"])
+            im = axes.scatter(gpx_df[column_x], gpx_df[column_y],
+                        c=gpx_df["speed"], cmap=cmap)
+        elif color == "pace":
+            cmap = matplotlib.colors.LinearSegmentedColormap.from_list("", ["lightskyblue", "midnightblue"])
+            im = axes.scatter(gpx_df[column_x], gpx_df[column_y],
+                        c=gpx_df["pace"], cmap=cmap)
+        elif color == "vertical_drop":
+            cmap = matplotlib.colors.LinearSegmentedColormap.from_list("", ["yellow", "orange", "red", "purple", "black"])
+            im = axes.scatter(gpx_df[column_x], gpx_df[column_y],
+                        c=abs(gpx_df["ascent_rate"]), cmap=cmap)
+        elif color == "ascent_rate":
+            cmap = matplotlib.colors.LinearSegmentedColormap.from_list("", ["darkgreen", "green", "yellow", "red", "black"])
+            im = axes.scatter(gpx_df[column_x], gpx_df[column_y],
+                        c=gpx_df["ascent_rate"], cmap=cmap)
+        elif color == "ascent_speed":
+            cmap = matplotlib.colors.LinearSegmentedColormap.from_list("", ["deeppink", "lightpink", "lightcoral", "red", "darkred"])
+            im = axes.scatter(gpx_df[column_x], gpx_df[column_y],
+                        c=gpx_df["ascent_speed"], cmap=cmap)
         else:
-            axes.scatter(gpx_df[column_x], gpx_df[column_y], color=base_color)
+            im = axes.scatter(gpx_df[column_x], gpx_df[column_y], color=color)
+        
+        # Colorbar
+        if colorbar:
+            plt.colorbar(im)
 
         # Scatter start and stop points with different color
         if start_stop_colors is not None:
             axes.scatter(gpx_df[column_x][0],
                         gpx_df[column_y][0], color=start_stop_colors[0])
             axes.scatter(gpx_df[column_x][len(gpx_df[column_x])-1],
                         gpx_df[column_y][len(gpx_df[column_x])-1], color=start_stop_colors[1])
@@ -387,15 +607,15 @@
                     way_point.project(projection)
                     axes.scatter(way_point._x, way_point._y, color=way_points_color)
                 else:
                     axes.scatter(way_point.lon, way_point.lat, color=way_points_color)
 
         # Add title
         if title is not None:
-            plt.title(title, size=20)
+            axes.set_title(title, size=20)
 
         # Add text elements
         self._matplotlib_plot_text(axes.get_figure(), duration, distance, ascent, pace, speed)
 
         # Add ticks
         axes.set_xticks([min(gpx_df[column_x]), max(gpx_df[column_x])])
         axes.set_yticks([min(gpx_df[column_y]), max(gpx_df[column_y])])
@@ -403,63 +623,78 @@
         # Add axis limits (useless??)
         if projection is not None:
             axes.set_xlim(left=min(gpx_df[column_x]),
                         right=max(gpx_df[column_x]))
             axes.set_ylim(bottom=min(gpx_df[column_y]),
                         top=max(gpx_df[column_y]))
 
-        # Save or display plot
-        if file_path is not None:
-            directory_path = os.path.dirname(os.path.realpath(file_path))
-            if not os.path.exists(directory_path):
-                logging.error("Provided path does not exist")
-                return
-            plt.savefig(file_path)
-        else:
-            plt.show()
-
     def matplotlib_plot(
         self,
         projection: Optional[str] = None,
-        base_color: str = "#101010",
-        elevation_color: bool = False,
+        color: str = "#101010",
+        colorbar: bool = False,
         start_stop_colors: Optional[tuple[str, str]] = None,
         way_points_color: Optional[str] = None,
         title: Optional[str] = None,
         duration: Optional[tuple[float, float]] = None,
         distance: Optional[tuple[float, float]] = None,
         ascent: Optional[tuple[float, float]] = None,
         pace: Optional[tuple[float, float]] = None,
         speed: Optional[tuple[float, float]] = None,
         file_path: Optional[str] = None):
+        """
+        plot GPX using Matplotlib.
 
+        Args:
+            projection (Optional[str], optional): Projection. Defaults to None.
+            color (str, optional): A color string (ie: "#FF0000" or "red") or a track attribute ("elevation", "speed", "pace", "vertical_drop", "ascent_rate", "ascent_speed") Defaults to "#101010".
+            colorbar (bool, optional): Colorbar toggle. Defaults to False.
+            start_stop_colors (tuple[str, str], optional): Start and stop points colors. Defaults to False.
+            way_points_color (str, optional): Way point color. Defaults to False.
+            title (Optional[str], optional): Title. Defaults to None.
+            duration (Optional[tuple[float, float]], optional): Display duration. Defaults to None.
+            distance (Optional[tuple[float, float]], optional): Display distance. Defaults to None.
+            ascent (Optional[tuple[float, float]], optional): Display ascent. Defaults to None.
+            pace (Optional[tuple[float, float]], optional): Display pace. Defaults to None.
+            speed (Optional[tuple[float, float]], optional): Display pace. Defaults to None.
+            file_path (Optional[str], optional): Path to save plot. Defaults to None.
+        """
         # Create figure with axes
         fig = plt.figure(figsize=(14, 8))
         fig.add_subplot(111)
 
         # Plot on axes
         self.matplotlib_axes_plot(fig.axes[0],
                                   projection,
-                                  base_color, 
-                                  elevation_color,
+                                  color,
+                                  colorbar,
                                   start_stop_colors,
                                   way_points_color,
                                   title,
                                   duration,
                                   distance,
                                   ascent,
                                   pace,
-                                  speed,
-                                  file_path)
+                                  speed)
+        
+        # Save or display plot
+        if file_path is not None:
+            directory_path = os.path.dirname(os.path.realpath(file_path))
+            if not os.path.exists(directory_path):
+                logging.error("Provided path does not exist")
+                return
+            plt.savefig(file_path)
+        else:
+            plt.show()
 
     def matplotlib_basemap_plot(
             self,
             projection: str = "cyl",
             service: str = "World_Shaded_Relief",
-            base_color: str = "#101010",
+            color: str = "#101010",
             start_stop_colors: Optional[tuple[str, str]] = None,
             way_points_color: Optional[str] = None,
             title: Optional[str] = None,
             duration: Optional[tuple[float, float]] = None,
             distance: Optional[tuple[float, float]] = None,
             ascent: Optional[tuple[float, float]] = None,
             pace: Optional[tuple[float, float]] = None,
@@ -467,15 +702,15 @@
             file_path: str = None):
         """
         Plot GPX using Matplotlib Basemap Toolkit.
 
         Args:
             projection (str, optional): Projection. Currently supported projections: cyl. Defaults to "cyl".
             service (str, optional): Service used to fetch map background. Currently supported services: "World_Shaded_Relief". Defaults to "World_Shaded_Relief".
-            base_color (str, optional): Track color. Defaults to "#101010".
+            color (str, optional): Track color. Defaults to "#101010".
             start_stop_colors (tuple[str, str], optional): Start and stop points colors. Defaults to False.
             way_points_color (str, optional): Way point color. Defaults to False.
             title (Optional[str], optional): Title. Defaults to None.
             duration (Optional[tuple[float, float]], optional): Display duration. Defaults to None.
             distance (Optional[tuple[float, float]], optional): Display distance. Defaults to None.
             ascent (Optional[tuple[float, float]], optional): Display ascent. Defaults to None.
             pace (Optional[tuple[float, float]], optional): Display pace. Defaults to None.
@@ -518,20 +753,20 @@
         map.arcgisimage(service=service,
                         xpixels=2000, dpi=200, verbose=True)
 
         # Create dataframe containing data from the GPX file
         gpx_df = self.to_dataframe()
 
         # Project track points
-        x, y = map(gpx_df["longitude"], gpx_df["latitude"])
+        x, y = map(gpx_df["lon"], gpx_df["lat"])
         
         # Plot track points on the map
         x = x.tolist()
         y = y.tolist()
-        map.plot(x, y, marker=None, color=base_color)
+        map.plot(x, y, marker=None, color=color)
 
         # Scatter start and stop points with different color
         if start_stop_colors:
             map.plot(x[0], y[0], marker="^", color=start_stop_colors[0])
             map.plot(x[-1], y[-1], marker="h", color=start_stop_colors[1])
 
         # Project and scatter way points with different color
@@ -556,28 +791,28 @@
                 return
             plt.savefig(file_path)
         else:
             plt.show()
 
     def gmplot_plot(
             self,
-            base_color: str = "#110000",
+            color: str = "#110000",
             start_stop_colors: Optional[tuple[str, str]] = None,
             way_points_color: Optional[str] = None,
             zoom: float = 10.0,
             title: Optional[str] = None,
             file_path: str = None,
             open: bool = True,
             scatter: bool = False,
             plot: bool = True):
         """
         Plot GPX using gmplot.
 
         Args:
-            base_color (str, optional): Track_color. Defaults to "#110000".
+            color (str, optional): Track_color. Defaults to "#110000".
             start_stop_colors (tuple[str, str], optional): Start and stop points colors. Defaults to False.
             way_points_color (str, optional): Way point color. Defaults to False.
             zoom (float, optional): Zoom. Defaults to 10.0.
             title (str, optional): Title. Defaults to None.
             file_path (str, optional): Path to save plot. Defaults to None.
             open (bool, optional): Open the plot in the default web browser. Defaults to True.
             scatter (bool, optional): Scatter track points. Defaults to False.
@@ -588,19 +823,19 @@
         map = gmplot.GoogleMapPlotter(center_lat, center_lon, zoom)
 
         # Create dataframe containing data from the GPX file
         gpx_df = self.to_dataframe()
 
         # Scatter track points
         if scatter:
-            map.scatter(gpx_df["latitude"], gpx_df["longitude"],
-                        base_color, size=5, marker=False)
+            map.scatter(gpx_df["lat"], gpx_df["lon"],
+                        color, size=5, marker=False)
         if plot:
-            map.plot(gpx_df["latitude"], gpx_df["longitude"],
-                     base_color, edge_width=2.5)
+            map.plot(gpx_df["lat"], gpx_df["lon"],
+                     color, edge_width=2.5)
         
         # Scatter start and stop points with different color
         if start_stop_colors:
             map.scatter([self.gpx.tracks[0].trkseg[0].trkpt[0].lat],
                         [self.gpx.tracks[0].trkseg[0].trkpt[0].lon],
                         start_stop_colors[0], size=5, marker=True)
             map.scatter([self.gpx.tracks[-1].trkseg[-1].trkpt[-1].lat],
@@ -623,15 +858,15 @@
         # Open map in web browser
         if open:
             webbrowser.open(file_path)
 
     def folium_plot(
             self,
             tiles: str = "OpenStreetMap",  # "OpenStreetMap", "Stamen Terrain", "Stamen Toner"
-            base_color: str = "#110000",
+            color: str = "#110000",
             start_stop_colors: Optional[tuple[str, str]] = None,
             way_points_color: Optional[str] = None,
             minimap: bool = False,
             coord_popup: bool = False,
             title: Optional[str] = None,
             zoom: float = 12.0,
             file_path: str = None,
@@ -657,15 +892,15 @@
                        tiles=tiles)
         
         # Plot track points
         gpx_df = self.to_dataframe()
         gpx_df["coordinates"] = list(
             zip(gpx_df.latitude, gpx_df.longitude))
         folium.PolyLine(gpx_df["coordinates"],
-                        tooltip=self.name(), color=base_color).add_to(m)
+                        tooltip=self.name(), color=color).add_to(m)
 
         # Scatter start and stop points with different color
         if start_stop_colors:
             folium.Marker([self.gpx.tracks[0].trkseg[0].trkpt[0].lat, self.gpx.tracks[0].trkseg[0].trkpt[0].lon],
                           popup="<b>Start</b>", tooltip="Start", icon=folium.Icon(color=start_stop_colors[0])).add_to(m)
             folium.Marker([self.gpx.tracks[-1].trkseg[-1].trkpt[-1].lat, self.gpx.tracks[-1].trkseg[-1].trkpt[-1].lon],
                           popup="<b>Stop</b>", tooltip="Stop", icon=folium.Icon(color=start_stop_colors[1])).add_to(m)
```

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/bounds.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/bounds.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/copyright.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/copyright.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/email.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/email.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/extensions.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/extensions.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/link.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/link.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/metadata.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/metadata.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/person.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/person.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/point.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/point.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/route.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/route.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,35 @@
             cmt: str = None,
             desc: str = None,
             src: str = None,
             link: Link = None,
             number: int = None, # non negative integer
             type: str = None,
             extensions: Extensions = None,
-            rtept: list[WayPoint] = []) -> None:
+            rtept: list[WayPoint] = None) -> None:
         """
         Initialize Route instance.
 
         Args:
             tag (str, optional): XML tag. Defaults to "rte".
             name (str, optional): Name. Defaults to None.
             cmt (str, optional): Comment. Defaults to None.
             desc (str, optional): Description. Defaults to None.
             src (str, optional): Source. Defaults to None.
             link (Link, optional): Link. Defaults to None.
             number (int, optional): Number. Defaults to None.
             extensions (Extensions, optional): Extensions. Defaults to None.
-            rtept (list[WayPoint], optional): Route points. Defaults to [].
+            rtept (list[WayPoint], optional): Route points. Defaults to None.
         """
         self.tag: str = tag
         self.name: str = name
         self.cmt: str = cmt
         self.desc: str = desc
         self.src: str = src
         self.link: Link = link
         self.number: int = number
         self.type: str = type
         self.extensions: Extensions = extensions
-        self.rtept: list[WayPoint] = rtept
+        if rtept is None:
+            self.rtept: list[WayPoint] = []
+        else:
+            self.rtept: list[WayPoint] = rtept
```

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/track.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,40 +14,43 @@
             cmt: str = None,
             desc: str = None,
             src: str = None,
             link: Link = None,
             number: int = None,
             type: str = None,
             extensions: Extensions = None,
-            trkseg: list[TrackSegment] = []):
+            trkseg: list[TrackSegment] = None):
         """
         Initialize Track instance.
 
         Args:
         tag (str, optional): XML tag. Defaults to "trk".
             name (str, optional): Name. Defaults to None.
             cmt (str, optional): Comment. Defaults to None.
             desc (str, optional): Description. Defaults to None.
             src (str, optional): Source. Defaults to None.
             link (Link, optional): Link. Defaults to None.
             number (int, optional): Number. Defaults to None.
             type (str, optional): Type. Defaults to None.
             extensions (Extensions, optional): Extensions. Defaults to None.
-            trkseg (list[TrackSegment], optional): List of track segments. Defaults to [].
+            trkseg (list[TrackSegment], optional): List of track segments. Defaults to None.
         """
         self.tag: str = tag
         self.name: str = name
         self.cmt: str = cmt
         self.desc: str = desc
         self.src: str = src
         self.link: Link = link
         self.number: int = number
         self.type: str = type
         self.extensions: Extensions = extensions
-        self.trkseg: list[TrackSegment] = trkseg
+        if trkseg is None:
+            self.trkseg: list[TrackSegment] = trkseg
+        else:
+            self.trkseg: list[TrackSegment] = trkseg
 
     def project(self, projection: str):
         """
         Project segments.
 
         Args:
             projection (str): Projection.
```

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/track_segment.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/track_segment.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,26 +5,29 @@
     """
     trksegType in GPX file.
     """
     
     def __init__(
             self,
             tag: str = "trkseg",
-            trkpt: list[WayPoint] = [],
+            trkpt: list[WayPoint] = None,
             extensions: Extensions = None) -> None:
         """
         Initialize TrackSegment instance.
 
         Args:
         tag (str, optional): XML tag. Defaults to "trkseg".
-            trkpt (list[WayPoint], optional): List of track points. Defaults to [].
+            trkpt (list[WayPoint], optional): List of track points. Defaults to None.
             extensions (Extensions, optional): Extensions. Defaults to None.
         """
         self.tag: str = tag
-        self.trkpt: list[WayPoint] = trkpt
+        if trkpt is None:
+            self.trkpt: list[WayPoint] = []
+        else:
+            self.trkpt: list[WayPoint] = trkpt
         self.extensions: Extensions = extensions
 
     def project(self, projection: str):
         """
         Project points.
 
         Args:
```

### Comparing `ezgpx-0.1.4/ezgpx/gpx_elements/way_point.py` & `ezgpx-0.1.5/ezgpx/gpx_elements/way_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,21 @@
         self.hdop: float = hdop
         self.vdop: float = vdop
         self.pdop: float = pdop
         self.age_of_gps_data: float = age_of_gps_data
         self.dgpsid: int = dgpsid
         self.extensions: Extensions = extensions
 
+        # Statistics (for map plotting: https://support.strava.com/hc/en-us/articles/360049869011-Personalized-Stat-Maps)
+        self.speed: float = None
+        self.pace: float = None
+        self.ascent_rate: float = None
+        self.ascent_speed: float = None
+
+        # Projection
         self._x: int = None
         self._y: int = None
 
     def project(self, projection: str):
         """
         Project point.
```

### Comparing `ezgpx-0.1.4/ezgpx/gpx_parser/parser.py` & `ezgpx-0.1.5/ezgpx/gpx_parser/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         try:
             time_ = datetime.strptime(element.find(sub_element, self.name_space).text, self.time_format)
         except:
             time_ = None
             logging.debug(f"{element} has no attribute {sub_element}.")
         return time_
 
-    def parse_bounds(self, bounds, tag: str ="bounds") -> Bounds:
+    def parse_bounds(self, bounds, tag: str ="bounds") -> Union[Bounds, None]:
         """
         Parse boundsType element from GPX file.
 
         Args:
             bounds (xml.etree.ElementTree.Element): Parsed bounds element.
             tag (str, Optional): XML tag. Defaults to "bounds".
 
@@ -277,15 +277,15 @@
         minlat = self.get_text(bounds, "minlat")
         minlon = self.get_text(bounds, "minlon")
         maxlat = self.get_text(bounds, "maxlat")
         maxlon = self.get_text(bounds, "maxlon")
 
         return Bounds(tag, minlat, minlon, maxlat, maxlon)
     
-    def parse_copyright(self, copyright, tag: str ="copyright") -> Copyright:
+    def parse_copyright(self, copyright, tag: str ="copyright") -> Union[Copyright, None]:
         """
         Parse copyrightType element from GPX file.
 
         Args:
             copyright (xml.etree.ElementTree.Element): Parsed copyright element.
             tag (str, Optional): XML tag. Defaults to "copyright".
 
@@ -297,15 +297,15 @@
         
         author = self.get_text(copyright, "author")
         year = self.find_text(copyright, "topo:year")
         licence = self.find_text(copyright, "topo:licence")
 
         return Copyright(tag, author, year, licence)
     
-    def parse_email(self, email, tag: str ="email") -> Email:
+    def parse_email(self, email, tag: str ="email") -> Union[Email, None]:
         """
         Parse emailType element from GPX file.
 
         Args:
             email (xml.etree.ElementTree.Element): Parsed email element.
             tag (str, Optional): XML tag. Defaults to "email".
 
@@ -316,47 +316,48 @@
             return None
         
         id = self.get_text(email, "id")
         domain = self.get_text(email, "domain")
 
         return Email(tag, id, domain)
     
-    def parse_extensions(self, extensions, tag: str ="extensions") -> Extensions:
+    def parse_extensions(self, extensions, tag: str ="extensions") -> Union[Extensions, None]:
         """
         Parse extensionsType element from GPX file.
 
         Args:
             extensions (xml.etree.ElementTree.Element): Parsed extensions element.
             tag (str, Optional): XML tag. Defaults to "extensions".
 
         Returns:
             Extensions: Extensions instance.
         """
         if extensions is None:
             return None
         
-        display_color = self.find_text(extensions, "topo:DisplayColor")
-        distance = self.find_text(extensions, "topo:Distance")
-        total_elapsed_time = self.find_text(extensions, "topo:TotalElapsedTime")
-        moving_time = self.find_text(extensions, "topo:MovingTime")
-        stopped_time = self.find_text(extensions, "topo:StoppedTime")
-        moving_speed = self.find_text(extensions, "topo:MovingSpeed")
-        max_speed = self.find_text(extensions, "topo:MaxSpeed")
-        max_elevation = self.find_text(extensions, "topo:MaxElevation")
-        min_elevation = self.find_text(extensions, "topo:MinElevation")
-        ascent = self.find_text(extensions, "topo:Ascent")
-        descent = self.find_text(extensions, "topo:Descent")
-        avg_ascent_rate = self.find_text(extensions, "topo:AvgAscentRate")
-        max_ascent_rate = self.find_text(extensions, "topo:MaxAscentRate")
-        avg_descent_rate = self.find_text(extensions, "topo:AvgDescentRate")
-        max_descent_rate = self.find_text(extensions, "topo:MaxDescentRate")
+        # display_color = self.find_text(extensions, "topo:DisplayColor")
+        # distance = self.find_text(extensions, "topo:Distance")
+        # total_elapsed_time = self.find_text(extensions, "topo:TotalElapsedTime")
+        # moving_time = self.find_text(extensions, "topo:MovingTime")
+        # stopped_time = self.find_text(extensions, "topo:StoppedTime")
+        # moving_speed = self.find_text(extensions, "topo:MovingSpeed")
+        # max_speed = self.find_text(extensions, "topo:MaxSpeed")
+        # max_elevation = self.find_text(extensions, "topo:MaxElevation")
+        # min_elevation = self.find_text(extensions, "topo:MinElevation")
+        # ascent = self.find_text(extensions, "topo:Ascent")
+        # descent = self.find_text(extensions, "topo:Descent")
+        # avg_ascent_rate = self.find_text(extensions, "topo:AvgAscentRate")
+        # max_ascent_rate = self.find_text(extensions, "topo:MaxAscentRate")
+        # avg_descent_rate = self.find_text(extensions, "topo:AvgDescentRate")
+        # max_descent_rate = self.find_text(extensions, "topo:MaxDescentRate")
 
-        return Extensions(tag, display_color, distance, total_elapsed_time, moving_time, stopped_time, moving_speed, max_speed, max_elevation, min_elevation, ascent, descent, avg_ascent_rate, max_ascent_rate, avg_descent_rate, max_descent_rate)
-
-    def parse_link(self, link, tag: str ="link") -> Link:
+        # return Extensions(tag, display_color, distance, total_elapsed_time, moving_time, stopped_time, moving_speed, max_speed, max_elevation, min_elevation, ascent, descent, avg_ascent_rate, max_ascent_rate, avg_descent_rate, max_descent_rate)
+        return None
+    
+    def parse_link(self, link, tag: str ="link") -> Union[Link, None]:
         """
         Parse linkType element from GPX file.
 
         Args:
             link (xml.etree.ElementTree.Element): Parsed link element.
             tag (str, Optional): XML tag. Defaults to "link".
 
@@ -368,15 +369,15 @@
         
         href = self.get_text(link, "href")
         text = self.find_text(link, "topo:text")
         type = self.find_text(link, "topo:type")
 
         return Link(tag, href, text, type)
     
-    def parse_metadata(self, metadata, tag: str = "metadata") -> Metadata:
+    def parse_metadata(self, metadata, tag: str = "metadata") -> Union[Metadata, None]:
         """
         Parse metadataType element from GPX file.
 
         Args:
             metadata (xml.etree.ElementTree.Element): Parsed metadata element.
             tag (str, Optional): XML tag. Defaults to "metadata".
 
@@ -394,15 +395,15 @@
         time = self.find_time(metadata, "topo:time")
         keywords = self.find_text(metadata, "topo:keywords")
         bounds = self.parse_bounds(metadata.find("topo:bounds", self.name_space))
         extensions = self.parse_extensions(metadata.find("topo:extensions", self.name_space))
 
         return Metadata(tag, name, desc, author, copyright, link, time, keywords, bounds, extensions)
 
-    def parse_person(self, person, tag: str ="person") -> Person:
+    def parse_person(self, person, tag: str ="person") -> Union[Person, None]:
         """
         Parse personType element from GPX file.
 
         Args:
             person (xml.etree.ElementTree.Element): Parsed person element.
             tag (str, Optional): XML tag. Defaults to "person".
 
@@ -417,15 +418,15 @@
         link = self.parse_link(person.find("topo:link", self.name_space))
 
         return Person(tag, name, email, link)
     
     def parse_point_segment(self, point_segment, tag: str = "ptseg") -> PointSegment:
         pass
 
-    def parse_point(self, point, tag: str = "pt") -> Point:
+    def parse_point(self, point, tag: str = "pt") -> Union[Point, None]:
         """
         Parse ptType element from GPX file.
 
         Args:
             point (xml.etree.ElementTree.Element): Parsed pt element.
             tag (str, Optional): XML tag. Defaults to "pt".
 
@@ -438,15 +439,15 @@
         lat = self.get_float(point, "lat")
         lon = self.get_float(point, "lon")
         ele = self.find_float(point, "topo:ele")
         time = self.find_time(point, "topo:time")
 
         return Point(tag, lat, lon, ele, time)
     
-    def parse_route(self, route, tag: str = "rte") -> Route:
+    def parse_route(self, route, tag: str = "rte") -> Union[Route, None]:
         """
         Parse rteType element from GPX file.
 
         Args:
             route (xml.etree.ElementTree.Element): Parsed rte element.
             tag (str, Optional): XML tag. Defaults to "rte".
 
@@ -468,15 +469,15 @@
         rtept = []
         way_points = route.findall("topo:rtept", self.name_space)
         for way_point in way_points:
             rtept.append(self.parse_way_point(way_point))
 
         return Route(tag, name, cmt, desc, src, link, number, type, extensions, rtept)
 
-    def parse_track_segment(self, track_segment, tag: str = "trkseg") -> TrackSegment:
+    def parse_track_segment(self, track_segment, tag: str = "trkseg") -> Union[TrackSegment, None]:
         """
         Parse trksegType element from GPX file.
 
         Args:
             track_segment (xml.etree.ElementTree.Element): Parsed trkseg element.
             tag (str, Optional): XML tag. Defaults to "trkseg".
 
@@ -493,15 +494,15 @@
             trkpt.append(self.parse_way_point(track_point, "trkpt"))
 
         # Extensions
         extensions = self.parse_extensions(track_segment.find("topo:extensions", self.name_space))
 
         return TrackSegment(tag, trkpt, extensions)
 
-    def parse_track(self, track, tag: str = "trk") -> Track:
+    def parse_track(self, track, tag: str = "trk") -> Union[Track, None]:
         """
         Parse trkType element from GPX file.
 
         Args:
             track (xml.etree.ElementTree.Element): Parsed trk element.
             tag (str, Optional): XML tag. Defaults to "trk".
 
@@ -523,15 +524,15 @@
         trkseg = []
         segments = track.findall("topo:trkseg", self.name_space)
         for segment in segments:
             trkseg.append(self.parse_track_segment(segment))
 
         return Track(tag, name, cmt, desc, src, link, number, type, extensions, trkseg)
     
-    def parse_way_point(self, way_point, tag: str = "wpt") -> WayPoint:
+    def parse_way_point(self, way_point, tag: str = "wpt") -> Union[WayPoint, None]:
         """
         Parse wptType element from GPX file.
 
         Args:
             way_point (xml.etree.ElementTree.Element): Parsed wpt element.
             tag (str, Optional): XML tag. Defaults to "person".
 
@@ -562,21 +563,29 @@
         pdop = self.find_float(way_point, "topo:pdop")
         age_of_gps_data = self.find_float(way_point, "topo:ageofgpsdata")
         dgpsid = self.find_float(way_point, "topo:dgpsid")
         extensions = self.parse_extensions(way_point.find("topo:extensions", self.name_space))
 
         return WayPoint(tag, lat, lon, ele, time, mag_var, geo_id_height, name, cmt, desc, src, link, sym, type, fix, sat, hdop, vdop, pdop, age_of_gps_data, dgpsid, extensions)
 
+    def find_xmlns_xsi(self) -> Union[str, None]:
+        schema_location = None
+        for elmt in list(self.gpx_root.attrib.keys()):
+            if elmt.endswith("schemaLocation"):
+                schema_location = elmt[1:-15]
+        return schema_location
+
     def parse_root_properties(self):
         """
         Parse XML properties from GPX file.
         """
         self.gpx.creator = self.gpx_root.attrib["creator"]
         self.gpx.version = self.gpx_root.attrib["version"]
         self.gpx.xmlns = self.gpx_root.tag[1:-4]
+        self.gpx.xmlns_xsi = self.find_xmlns_xsi()
         self.name_space["topo"] = self.gpx.xmlns
         name_spaces = self.gpx_root.get("{http://www.w3.org/2001/XMLSchema-instance}schemaLocation").split(" ")
         self.gpx.xsi_schema_location = [x for x in name_spaces if x != ""]
 
     def parse_root_metadata(self):
         """
         Parse metadataType elements from GPX file.
@@ -632,15 +641,15 @@
             return
 
         # Parse GPX file
         try:
             self.gpx_tree = ET.parse(self.file_path)
             self.gpx_root = self.gpx_tree.getroot()
         except Exception as err:
-            logging.exception(f"Unexpected {err=}, {type(err)=}.\nUnable to parse GPX file.")
+            logging.exception(f"Unexpected {err}, {type(err)}.\nUnable to parse GPX file.")
             raise
 
         # Parse properties
         try:
             self.parse_root_properties()
         except:
             logging.error("Unable to parse properties in GPX file.")
```

### Comparing `ezgpx-0.1.4/ezgpx/gpx_writer/writer.py` & `ezgpx-0.1.5/ezgpx/gpx_writer/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,20 +412,22 @@
         self.gpx_root.set("version", self.gpx.version)
         schema_location_string = ""
         for loc in self.gpx.xsi_schema_location:
             schema_location_string += loc
             schema_location_string += " "
         schema_location_string = schema_location_string[:len(schema_location_string)-1]
         self.gpx_root.set("xsi:schemaLocation", schema_location_string)
+        self.gpx_root.set("xmlns:xsi", self.gpx.xmlns_xsi)
     
     def add_properties_strava(self) -> None:
         """
         Add Strava style properties to the GPX root element.
         """
         self.gpx_root.set("creator", self.gpx.creator)
+        self.gpx_root.set("xmlns:xsi", self.gpx.xmlns_xsi)
         schema_location_string = ""
         for loc in self.gpx.xsi_schema_location:
             schema_location_string += loc
             schema_location_string += " "
         schema_location_string = schema_location_string[:len(schema_location_string)-1]
         self.gpx_root.set("xsi:schemaLocation", schema_location_string)
         self.gpx_root.set("version", self.gpx.version)
```

### Comparing `ezgpx-0.1.4/ezgpx/utils/algorithms.py` & `ezgpx-0.1.5/ezgpx/utils/algorithms.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/utils/distance.py` & `ezgpx-0.1.5/ezgpx/utils/distance.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx/utils/projections.py` & `ezgpx-0.1.5/ezgpx/utils/projections.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/ezgpx.egg-info/PKG-INFO` & `ezgpx-0.1.5/ezgpx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezgpx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy to use Python GPX library
 Home-page: https://pypi.org/project/ezgpx/
 Download-URL: https://github.com/FABallemand/ezGPX
 Author: Fabien ALLEMAND
 Author-email: allemand.fabien@orange.fr
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/FABallemand/ezGPX/issues
```

### Comparing `ezgpx-0.1.4/ezgpx.egg-info/SOURCES.txt` & `ezgpx-0.1.5/ezgpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.4/setup.py` & `ezgpx-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(os.path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ezgpx',
-    version='0.1.4',
+    version='0.1.5',
     description='Easy to use Python GPX library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['gpx', 'gpx-files', 'gpx-parser', 'gpx-reader', 'gpx-writer', 'gpx-data'],
     url='https://pypi.org/project/ezgpx/',
     download_url='https://github.com/FABallemand/ezGPX',
     project_urls={
```

### Comparing `ezgpx-0.1.4/tests/test_GPX.py` & `ezgpx-0.1.5/tests/test_GPX.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,79 +10,121 @@
 parent_folder = os.path.realpath(os.path.dirname(file_folder)) # ie: ezGPX
 
 os.chdir(file_folder)
 sys.path.append(parent_folder + "/ezgpx")
 
 from ezgpx import GPX
 
+FILES_DIRECTORY = "test_files/files/"
+REFERENCE_FILES_DIRECTORY = "test_files/reference_files/"
+
 class TestGPX():
 
+    #==== Init ===============================================================#
+
+    def test_init(self):
+
+        # Create temporary folder
+        rmtree("tmp", True)
+        os.makedirs(os.path.dirname(__file__) + "/tmp")
+
+    #==== Parsing/Writing ====================================================#
+
+    def test_parse_write(self, remove_tmp: bool = True):
+        
+        # Parse GPX file
+        self.test_gpx_1 = GPX(os.path.join(FILES_DIRECTORY, "strava_run_1.gpx"))
+
+        # Write GPX file
+        self.test_gpx_1.to_gpx("tmp/strava_run_1.gpx")
+
+        # Parse GPX file
+        self.test_gpx_2 = GPX("tmp/strava_run_1.gpx")
+
+    #==== Plots ==============================================================#
+
     def _test_matplotlib_plot_1(self):
         # Plot
         self.test_gpx.matplotlib_plot(start_stop_colors=None, elevation_color=False, title="Track", file_path="tmp/matplotlib_strava_run_1.png")
 
         # Load images
         test_img = plt.imread("tmp/matplotlib_strava_run_1.png")
-        ref_img = plt.imread("../tests/test_files/reference_files/matplotlib_strava_run_1.png")
+        ref_img = plt.imread(os.path.join(REFERENCE_FILES_DIRECTORY, "matplotlib_strava_run_1.png"))
 
         # Compare images
         return np.array_equal(test_img, ref_img)
     
     def _test_matplotlib_plot_2(self):
         # Plot
         self.test_gpx.matplotlib_plot(start_stop_colors=("#00FF00", "#FF0000"), elevation_color=False, title="Track", file_path="tmp/matplotlib_strava_run_1_start_stop.png")
 
         # Load images
         test_img = plt.imread("tmp/matplotlib_strava_run_1_start_stop.png")
-        ref_img = plt.imread("../tests/test_files/reference_files/matplotlib_strava_run_1_start_stop.png")
+        ref_img = plt.imread(os.path.join(REFERENCE_FILES_DIRECTORY, "matplotlib_strava_run_1_start_stop.png"))
 
         # Compare images
         return np.array_equal(test_img, ref_img)
     
     def _test_matplotlib_plot_3(self):
         # Plot
         self.test_gpx.matplotlib_plot(start_stop_colors=None, elevation_color=True, title="Track", file_path="tmp/matplotlib_strava_run_1_elevation.png")
 
         # Load images
         test_img = plt.imread("tmp/matplotlib_strava_run_1_elevation.png")
-        ref_img = plt.imread("../tests/test_files/reference_files/matplotlib_strava_run_1_elevation.png")
+        ref_img = plt.imread(os.path.join(REFERENCE_FILES_DIRECTORY, "matplotlib_strava_run_1_elevation.png"))
 
         # Compare images
         return np.array_equal(test_img, ref_img)
     
     def _test_matplotlib_plot_4(self):
         # Plot
         self.test_gpx.matplotlib_plot(start_stop_colors=("#00FF00", "#FF0000"), elevation_color=True, title="Track", file_path="tmp/matplotlib_strava_run_1_start_stop_elevation.png")
 
         # Load images
         test_img = plt.imread("tmp/matplotlib_strava_run_1_start_stop_elevation.png")
-        ref_img = plt.imread("../tests/test_files/reference_files/matplotlib_strava_run_1_start_stop_elevation.png")
+        ref_img = plt.imread(os.path.join(REFERENCE_FILES_DIRECTORY, "matplotlib_strava_run_1_start_stop_elevation.png"))
 
         # Compare images
         return np.array_equal(test_img, ref_img)
 
     def test_matplotlib_plot(self, remove_tmp: bool = True):
         """
         Test matplotlib_plot method.
 
         Args:
             remove_tmp (bool, optional): Remove temporary folder. Defaults to True.
         """
-        self.test_gpx = GPX("../tests/test_files/files/strava_run_1.gpx")
-
-        # Create temporary folder
-        rmtree("tmp", True)
-        os.makedirs(os.path.dirname(__file__) + "/tmp")
+        # Parse GPX file
+        self.test_gpx = GPX(os.path.join(FILES_DIRECTORY, "strava_run_1.gpx"))
 
         # Tests
         assert(self._test_matplotlib_plot_1())
         assert(self._test_matplotlib_plot_2())
         assert(self._test_matplotlib_plot_3())
         assert(self._test_matplotlib_plot_4())
+        # self._test_matplotlib_plot_1()
+        # self._test_matplotlib_plot_2()
+        # self._test_matplotlib_plot_3()
+        # self._test_matplotlib_plot_4()
 
+    #==== Destroy ============================================================#
+
+    def test_destroy(self, remove_tmp: bool = True):
         # Remove temporary folder
         if remove_tmp:
-            rmtree("tmp")
+            rmtree("tmp", True)
+
+    #==== Test ===============================================================#
 
     @pytest.mark.skip(reason="test") # https://docs.pytest.org/en/7.3.x/how-to/skipping.html
-    def test_test(self):
-        print("Testing...")
+    def test_test(self, remove_tmp: bool = True):
+
+         # Create temporary folder
+        rmtree("tmp", True)
+        os.makedirs(os.path.dirname(__file__) + "/tmp")
+
+        # Parse GPX file
+        self.test_gpx = GPX(os.path.join(FILES_DIRECTORY, "strava_run_1.gpx"))
+
+        # Remove temporary folder
+        if remove_tmp:
+            rmtree("tmp")
```

### Comparing `ezgpx-0.1.4/tests/test_utils.py` & `ezgpx-0.1.5/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 sys.path.append(parent_folder + "/ezgpx")
 
 from ezgpx import utils, WayPoint
 
 class TestUtils():
 
     def test_haversine_distance(self):
-        pass
+        point_1 = WayPoint("wpt", 48.0, 2.0)
+        point_2 = WayPoint("wpt", 43.0, 5.0)
+        assert math.isclose(utils.haversine_distance(point_1, point_2), 603020.0, abs_tol=1000.0)
 
     def _test_perpendicular_distance_horizontal_line(self):
         start = WayPoint("wpt", 0, 0)
         end = WayPoint("wpt", 0, 2)
         point = WayPoint("wpt", 1, 1)
         return math.isclose(utils.perpendicular_distance(start, end, point), 1)
```

