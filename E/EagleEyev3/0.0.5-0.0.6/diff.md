# Comparing `tmp/eagleeyev3-0.0.5.tar.gz` & `tmp/eagleeyev3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagleeyev3-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eagleeyev3-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eagleeyev3-0.0.5.tar` & `eagleeyev3-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      162 2023-07-20 15:43:05.663721 eagleeyev3-0.0.5/.gitignore
--rw-r--r--   0        0        0     1049 2023-07-18 18:55:59.571391 eagleeyev3-0.0.5/LICENSE
--rw-r--r--   0        0        0      375 2023-07-20 04:33:54.569165 eagleeyev3-0.0.5/README.md
--rw-r--r--   0        0        0      380 2023-07-20 15:33:42.589081 eagleeyev3-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    27534 2023-07-24 16:22:55.160633 eagleeyev3-0.0.5/src/EagleEyev3/__init__.py
--rw-r--r--   0        0        0      533 2023-07-11 02:17:41.899184 eagleeyev3-0.0.5/src/EagleEyev3/settings.py
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 eagleeyev3-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      162 2023-07-20 15:43:05.663721 eagleeyev3-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1049 2023-07-18 18:55:59.571391 eagleeyev3-0.0.6/LICENSE
+-rw-r--r--   0        0        0      375 2023-07-20 04:33:54.569165 eagleeyev3-0.0.6/README.md
+-rw-r--r--   0        0        0      380 2023-07-20 15:33:42.589081 eagleeyev3-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    27527 2023-07-24 20:58:26.689982 eagleeyev3-0.0.6/src/EagleEyev3/__init__.py
+-rw-r--r--   0        0        0      533 2023-07-11 02:17:41.899184 eagleeyev3-0.0.6/src/EagleEyev3/settings.py
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 eagleeyev3-0.0.6/PKG-INFO
```

### Comparing `eagleeyev3-0.0.5/LICENSE` & `eagleeyev3-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eagleeyev3-0.0.5/src/EagleEyev3/__init__.py` & `eagleeyev3-0.0.6/src/EagleEyev3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Python client for Eagle Eye Networks APIv3 """
-__version__ = "0.0.5"
+version = "0.0.6"
+__version__ = version
 
 
 import json
 import logging
 import requests
 from .settings import *
 
@@ -17,15 +18,15 @@
 
 
 class EagleEyev3():
     """
     Class representing the EagleEyev3 client.
     """
 
-    __version__ = "0.0.5"
+    __version__ = version
     __all__ = ['EagleEyev3', 'Device', 'Camera']
 
     def __init__(self, config=None):
         """
         Initializes the EagleEyev3 client object.
         """
         self.client_id = None
@@ -750,15 +751,16 @@
                 success = True
                 # filter events by type
                 [self.events['status'].append(i) for i in response.json()['results'] if i['type'] == 'een.deviceCloudStatusUpdateEvent.v1']
                 [self.events['motion'].append(i) for i in response.json()['results'] if i['type'] == 'een.motionDetectionEvent.v1']
 
                 # remove duplicates
                 seen = set()
-                self.events['status'] = [event for event in self.events['status'] if event['endTimestamp'] and event['id'] not in seen and not seen.add(event['id'])]
+                self.events['status'] = [event for event in self.events['status'] if event['id'] not in seen and not seen.add(event['id'])]
+
                 seen = set()
                 self.events['motion'] = [event for event in self.events['motion'] if event['id'] not in seen and not seen.add(event['id'])]
 
                 # sort by event startTimestamp descending
                 self.events['status'] = sorted(self.events['status'], key=lambda x: x['startTimestamp'], reverse=True)
                 self.events['motion'] = sorted(self.events['motion'], key=lambda x: x['startTimestamp'], reverse=True)
             else:
```

### Comparing `eagleeyev3-0.0.5/src/EagleEyev3/settings.py` & `eagleeyev3-0.0.6/src/EagleEyev3/settings.py`

 * *Files identical despite different names*

### Comparing `eagleeyev3-0.0.5/PKG-INFO` & `eagleeyev3-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EagleEyev3
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python client for Eagle Eye Networks APIv3 
 Author-email: mcotton <mcotton@mcottondesign.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://mcottondesign.com
 
 # EE-status-v3 #
```

