# Comparing `tmp/pymoebot-0.2.2.tar.gz` & `tmp/pymoebot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoebot-0.2.2.tar", last modified: Sun Jul 16 11:07:22 2023, max compression
+gzip compressed data, was "pymoebot-0.2.3.tar", last modified: Mon Jul 24 11:57:39 2023, max compression
```

## Comparing `pymoebot-0.2.2.tar` & `pymoebot-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:07:22.043352 pymoebot-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-16 11:07:22.043352 pymoebot-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-16 11:07:03.000000 pymoebot-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:07:22.043352 pymoebot-0.2.2/pymoebot/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-16 11:07:03.000000 pymoebot-0.2.2/pymoebot/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-16 11:07:03.000000 pymoebot-0.2.2/pymoebot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:07:22.043352 pymoebot-0.2.2/pymoebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-16 11:07:22.000000 pymoebot-0.2.2/pymoebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-16 11:07:22.000000 pymoebot-0.2.2/pymoebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:07:22.000000 pymoebot-0.2.2/pymoebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 11:07:22.000000 pymoebot-0.2.2/pymoebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 11:07:22.000000 pymoebot-0.2.2/pymoebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:07:22.043352 pymoebot-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-16 11:07:03.000000 pymoebot-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:07:22.043352 pymoebot-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 11:07:03.000000 pymoebot-0.2.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-16 11:07:03.000000 pymoebot-0.2.2/test/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:39.703800 pymoebot-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-24 11:57:39.703800 pymoebot-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-24 11:57:28.000000 pymoebot-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:39.699800 pymoebot-0.2.3/pymoebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 11:57:28.000000 pymoebot-0.2.3/pymoebot/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-24 11:57:28.000000 pymoebot-0.2.3/pymoebot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:39.703800 pymoebot-0.2.3/pymoebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 11:57:39.000000 pymoebot-0.2.3/pymoebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:57:39.703800 pymoebot-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 11:57:28.000000 pymoebot-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:39.703800 pymoebot-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:57:28.000000 pymoebot-0.2.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-24 11:57:28.000000 pymoebot-0.2.3/test/model_test.py
```

### Comparing `pymoebot-0.2.2/PKG-INFO` & `pymoebot-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymoebot
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library intended to monitor and control MoeBot robotic lawn mowers.
 Home-page: https://github.com/Whytey/pymoebot
 Author: David Whyte
 Author-email: David@Whyte.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pymoebot-0.2.2/README.md` & `pymoebot-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pymoebot-0.2.2/pymoebot/__init__.py` & `pymoebot-0.2.3/pymoebot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     def __init__(self, device_id: str, device_ip: str, local_key: str) -> None:
         self.__id = device_id
         self.__ip = device_ip
         self.__key = local_key
 
         self.__device = tinytuya.Device(self.__id, self.__ip, self.__key)
 
+        self.__listeners = []
+
         self.__tuya_version = self.__do_proto_check()
         self.__device.set_version(self.__tuya_version)
 
         self.__thread = None
         self.__shutdown = threading.Event()
         self.__shutdown.set()  # The thread should be flagged as not running
 
-        self.__listeners = []
-
         self.__battery = None
         self.__state = None
         self.__emergency_state = None
         self.__mow_in_rain = None
         self.__mow_time = None
         self.__work_mode = None
         self.__online = False
@@ -62,14 +62,16 @@
         if '104' in dps:
             self.__mow_in_rain = dps['104']
         if '105' in dps:
             self.__mow_time = dps['105']
         if '114' in dps:
             self.__work_mode = dps['114']
 
+        for listener in self.__listeners:
+            listener(data)
         return True
 
     def poll(self):
         result = self.__device.status()
         self.__parse_payload(result)
 
     def __loop(self):
@@ -84,16 +86,14 @@
                 break
             # See if any data is available
             data = self.__device.receive()
             if data is not None:
                 _log.debug("Received Payload: %r", data)
 
                 self.__parse_payload(data)
-                for listener in self.__listeners:
-                    listener(data)
 
             # Send keepalive heartbeat
             payload = self.__device.generate_payload(tinytuya.HEART_BEAT)
             self.__device.send(payload)
 
     def listen(self):
         if self.__shutdown.is_set():
```

### Comparing `pymoebot-0.2.2/pymoebot.egg-info/PKG-INFO` & `pymoebot-0.2.3/pymoebot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymoebot
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library intended to monitor and control MoeBot robotic lawn mowers.
 Home-page: https://github.com/Whytey/pymoebot
 Author: David Whyte
 Author-email: David@Whyte.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pymoebot-0.2.2/setup.py` & `pymoebot-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pymoebot-0.2.2/test/model_test.py` & `pymoebot-0.2.3/test/model_test.py`

 * *Files identical despite different names*

