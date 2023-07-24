# Comparing `tmp/agent-bdi-1.1.5.tar.gz` & `tmp/agent-bdi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-bdi-1.1.5.tar", last modified: Mon Jan 23 18:06:49 2023, max compression
+gzip compressed data, was "agent-bdi-1.2.0.tar", last modified: Mon Jul 24 11:33:26 2023, max compression
```

## Comparing `agent-bdi-1.1.5.tar` & `agent-bdi-1.2.0.tar`

### file list

```diff
@@ -1,64 +1,27 @@
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.627250 agent-bdi-1.1.5/
--rw-r--r--   0 xumingfang   (501) staff       (20)     1799 2023-01-10 18:22:34.000000 agent-bdi-1.1.5/.gitignore
--rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:56:07.000000 agent-bdi-1.1.5/CHANGES.md
--rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:55:55.000000 agent-bdi-1.1.5/LICENSE.md
--rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:56:20.000000 agent-bdi-1.1.5/MANIFEST.in
--rw-r--r--   0 xumingfang   (501) staff       (20)     3149 2023-01-23 18:06:49.627332 agent-bdi-1.1.5/PKG-INFO
--rw-r--r--   0 xumingfang   (501) staff       (20)     2612 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/README.md
--rw-r--r--   0 xumingfang   (501) staff       (20)       60 2023-01-10 18:24:03.000000 agent-bdi-1.1.5/agent-bdi.code-workspace
--rw-r--r--   0 xumingfang   (501) staff       (20)      241 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/requirements.txt
--rw-r--r--   0 xumingfang   (501) staff       (20)      659 2023-01-23 18:06:49.627668 agent-bdi-1.1.5/setup.cfg
--rw-r--r--   0 xumingfang   (501) staff       (20)      856 2023-01-23 18:06:43.000000 agent-bdi-1.1.5/setup.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.618186 agent-bdi-1.1.5/src/
--rw-r--r--   0 xumingfang   (501) staff       (20)     1097 2023-01-10 19:28:15.000000 agent-bdi-1.1.5/src/Helper.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.618903 agent-bdi-1.1.5/src/agent_bdi.egg-info/
--rw-r--r--   0 xumingfang   (501) staff       (20)     3149 2023-01-23 18:06:49.000000 agent-bdi-1.1.5/src/agent_bdi.egg-info/PKG-INFO
--rw-r--r--   0 xumingfang   (501) staff       (20)     1283 2023-01-23 18:06:49.000000 agent-bdi-1.1.5/src/agent_bdi.egg-info/SOURCES.txt
--rw-r--r--   0 xumingfang   (501) staff       (20)        1 2023-01-23 18:06:49.000000 agent-bdi-1.1.5/src/agent_bdi.egg-info/dependency_links.txt
--rw-r--r--   0 xumingfang   (501) staff       (20)       11 2023-01-23 18:06:49.000000 agent-bdi-1.1.5/src/agent_bdi.egg-info/top_level.txt
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.620299 agent-bdi-1.1.5/src/core/
--rw-r--r--   0 xumingfang   (501) staff       (20)      301 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/src/core/Agent.py
--rw-r--r--   0 xumingfang   (501) staff       (20)       56 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/src/core/Belief.py
--rw-r--r--   0 xumingfang   (501) staff       (20)       50 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/src/core/Desire.py
--rw-r--r--   0 xumingfang   (501) staff       (20)       53 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/src/core/Intention.py
--rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:54:43.000000 agent-bdi-1.1.5/src/core/__init__.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.621811 agent-bdi-1.1.5/src/holon/
--rw-r--r--   0 xumingfang   (501) staff       (20)      111 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/src/holon/Blackboard.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      429 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/src/holon/Heart.py
--rw-r--r--   0 xumingfang   (501) staff       (20)     1097 2023-01-10 19:35:33.000000 agent-bdi-1.1.5/src/holon/Helper.py
--rw-r--r--   0 xumingfang   (501) staff       (20)     3508 2023-01-23 18:06:31.000000 agent-bdi-1.1.5/src/holon/HolonicAgent.py
--rw-r--r--   0 xumingfang   (501) staff       (20)       69 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/src/holon/HolonicDesire.py
--rw-r--r--   0 xumingfang   (501) staff       (20)       81 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/src/holon/HolonicIntention.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      193 2023-01-10 19:29:11.000000 agent-bdi-1.1.5/src/holon/__init__.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.622281 agent-bdi-1.1.5/tests/
--rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:55:02.000000 agent-bdi-1.1.5/tests/__init__.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.623090 agent-bdi-1.1.5/tests/guide/
--rw-r--r--   0 xumingfang   (501) staff       (20)      640 2023-01-23 16:59:41.000000 agent-bdi-1.1.5/tests/guide/GuideMain.py
--rw-r--r--   0 xumingfang   (501) staff       (20)        0 2023-01-10 17:54:54.000000 agent-bdi-1.1.5/tests/guide/__init__.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      155 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/config.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.624044 agent-bdi-1.1.5/tests/guide/dialog/
--rw-r--r--   0 xumingfang   (501) staff       (20)      129 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/dialog/AudioInput.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      130 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/dialog/AudioOutput.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      384 2023-01-10 19:23:21.000000 agent-bdi-1.1.5/tests/guide/dialog/DialogSystem.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      122 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/dialog/Nlu.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.624773 agent-bdi-1.1.5/tests/guide/hearing/
--rw-r--r--   0 xumingfang   (501) staff       (20)      138 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/hearing/BackgroundDenoising.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      329 2023-01-10 19:23:36.000000 agent-bdi-1.1.5/tests/guide/hearing/Hearing.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      129 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/hearing/Microphone.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.625334 agent-bdi-1.1.5/tests/guide/navi/
--rw-r--r--   0 xumingfang   (501) staff       (20)      388 2023-01-10 19:23:55.000000 agent-bdi-1.1.5/tests/guide/navi/NaviSystem.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      172 2023-01-10 19:23:59.000000 agent-bdi-1.1.5/tests/guide/navi/RouteFind.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      174 2023-01-10 19:24:04.000000 agent-bdi-1.1.5/tests/guide/navi/VisualInput.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.625983 agent-bdi-1.1.5/tests/guide/navi/walk/
--rw-r--r--   0 xumingfang   (501) staff       (20)      132 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/navi/walk/KanbanDetect.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      130 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/navi/walk/RoadDetect.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      315 2023-01-10 19:23:48.000000 agent-bdi-1.1.5/tests/guide/navi/walk/WalkGuide.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      238 2023-01-23 04:30:07.000000 agent-bdi-1.1.5/tests/guide/start.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.626537 agent-bdi-1.1.5/tests/guide/visual/
--rw-r--r--   0 xumingfang   (501) staff       (20)      125 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/visual/Camera.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      137 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/visual/ImagePreprocessing.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      311 2023-01-10 19:24:17.000000 agent-bdi-1.1.5/tests/guide/visual/Visual.py
-drwxr-xr-x   0 xumingfang   (501) staff       (20)        0 2023-01-23 18:06:49.627061 agent-bdi-1.1.5/tests/guide/voice/
--rw-r--r--   0 xumingfang   (501) staff       (20)      126 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/voice/Speaker.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      133 2023-01-10 11:54:29.000000 agent-bdi-1.1.5/tests/guide/voice/ToneProcessing.py
--rw-r--r--   0 xumingfang   (501) staff       (20)      299 2023-01-10 19:24:28.000000 agent-bdi-1.1.5/tests/guide/voice/Voice.py
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.496457 agent-bdi-1.2.0/
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/LICENSE.md
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/MANIFEST.in
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     3149 2023-07-24 11:33:26.496457 agent-bdi-1.2.0/PKG-INFO
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     2612 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/README.md
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      659 2023-07-24 11:33:26.496457 agent-bdi-1.2.0/setup.cfg
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      856 2023-07-24 11:26:34.000000 agent-bdi-1.2.0/setup.py
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.495457 agent-bdi-1.2.0/src/
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.495457 agent-bdi-1.2.0/src/agent_bdi.egg-info/
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     3149 2023-07-24 11:33:26.000000 agent-bdi-1.2.0/src/agent_bdi.egg-info/PKG-INFO
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      466 2023-07-24 11:33:26.000000 agent-bdi-1.2.0/src/agent_bdi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        1 2023-07-24 11:33:26.000000 agent-bdi-1.2.0/src/agent_bdi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       11 2023-07-24 11:33:26.000000 agent-bdi-1.2.0/src/agent_bdi.egg-info/top_level.txt
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.495457 agent-bdi-1.2.0/src/core/
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      302 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/Agent.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       56 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/Belief.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       50 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/Desire.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       53 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/Intention.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/__init__.py
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.496457 agent-bdi-1.2.0/src/holon/
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      111 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/holon/Blackboard.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      436 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/holon/Heart.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     1896 2023-07-05 09:54:01.000000 agent-bdi-1.2.0/src/holon/Helper.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     4974 2023-07-11 18:17:19.000000 agent-bdi-1.2.0/src/holon/HolonicAgent.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       69 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/holon/HolonicDesire.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       81 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/holon/HolonicIntention.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      377 2023-07-05 10:07:40.000000 agent-bdi-1.2.0/src/holon/__init__.py
```

### Comparing `agent-bdi-1.1.5/PKG-INFO` & `agent-bdi-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 1.1.5
+Version: 1.2.0
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-1.1.5/README.md` & `agent-bdi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `agent-bdi-1.1.5/setup.cfg` & `agent-bdi-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `agent-bdi-1.1.5/setup.py` & `agent-bdi-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "agent-bdi",
-    version = "1.1.5",
+    version = "1.2.0",
     author = "Ming Fang Shiu",
     author_email='avatar.xu@gmail.com',
     description='Agent BDI framework',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mfshiu/abdi.git",
     project_urls = {
```

### Comparing `agent-bdi-1.1.5/src/agent_bdi.egg-info/PKG-INFO` & `agent-bdi-1.2.0/src/agent_bdi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 1.1.5
+Version: 1.2.0
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-1.1.5/src/holon/HolonicAgent.py` & `agent-bdi-1.2.0/src/holon/HolonicAgent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import logging
 import inspect
+import logging
 from multiprocessing import Process
 import os
 import signal
 import sys
 import threading
 import time 
 
@@ -15,110 +15,152 @@
 from holon import Helper
 from core.Agent import Agent
 from holon.Blackboard import Blackboard
 from holon.HolonicDesire import HolonicDesire
 from holon.HolonicIntention import HolonicIntention
 from holon import config
 
+logger = logging.getLogger('ABDI')
+
 class HolonicAgent(Agent) :
-    def __init__(self, b:Blackboard=None, d:HolonicDesire=None, i: HolonicIntention=None):
+    def __init__(self, cfg:config=None, b:Blackboard=None, d:HolonicDesire=None, i: HolonicIntention=None):
         b = b or Blackboard()
         d = d or HolonicDesire()
         i = i or HolonicIntention()
         super().__init__(b, d, i)
         self.head_agents = []
         self.body_agents = []
-        self.mqtt_client = None
         self.run_interval_seconds = 1
-        self.is_running = False
+        self._mqtt_client = None
+        self._agent_proc = None
+        self._config = cfg if cfg else config()
+        self.name = f'<{self.__class__.__name__}>'
+
+
+    def start(self):
+        self._agent_proc = Process(target=self._run, args=(self._config,))
+        self._agent_proc.start()
+
+        for a in self.head_agents:
+            a.start()
+        for a in self.body_agents:
+            a.start()
+
+# ===================================
+# |            Process              |
+# ===================================
+
+
+    def is_running(self):
+        return not self._terminate_lock.is_set()
 
     def _on_connect(self, client, userdata, flags, rc):
-        logging.info(f"MQTT is connected with result code {str(rc)}")
+        logger.info(f"{self.name} result code:{str(rc)}")
         client.subscribe("echo")
         client.subscribe("terminate")
 
         self._on_connected()
 
 
     def _on_connected(self):
         pass
 
 
     def _on_message(self, client, db, msg):
         data = msg.payload.decode('utf-8', 'ignore')
-
-        if "terminate" == msg.topic:
-            self._terminate_lock.set()
-
         self._on_topic(msg.topic, data)
+        # try:
+        #     self._on_topic(msg.topic, data)
+        # except Exception as ex:
+        #     logging.exception(f'{ex}')
 
 
     def _on_topic(self, topic, data):
-        logging.debug("topic: %s, data: %s" % (topic, data))
+        # logging.debug(f"{self.name} topic:{topic}, data:{data}")
+
+        if "terminate" == topic:
+            if data:
+                if type(self).__name__ == data:
+                    self.terminate()
+            else:
+                self.terminate()
 
 
     def _run_begin(self):
-        Helper.init_logging()
-        logging.info(f"_run_begin: {self.__class__.__name__}")
+        #Helper.init_logging(self._config.log_dir, self._config.log_level)
+        logger.debug(f"{self.name} ...")
+        
+        def signal_handler(signal, frame):
+            logger.warning(f"{self.name} Ctrl-C: {self.__class__.__name__}")
+            self.terminate()
+        signal.signal(signal.SIGINT, signal_handler)
 
         self._terminate_lock = threading.Event()
         self._start_mqtt()
         threading.Thread(target=self.__interval_loop).start()
         
-        def signal_handler(signal, frame):
-            self._terminate_lock.set()
-        signal.signal(signal.SIGINT, signal_handler)
-        
-        self.is_running = True
+        # self.is_running = True
         # Helper.write_log("_run_begin 2")
 
     def __interval_loop(self):
         while not self._terminate_lock.is_set():
             self._run_interval()
             time.sleep(self.run_interval_seconds)
 
     def _run_interval(self):
         pass
 
     def _running(self):
-        logging.debug("running")
+        logger.debug(f"{self.name} ...")
 
-    def _run(self):
+    def _run(self, cfg:config):
+        self._config = cfg
         self._run_begin()
         self._running()
         self._run_end()
     
     def _run_end(self):
-        logging.warn(f"_run_end: {self.__class__.__name__}")
-        self.is_running = False
-        self._terminate_lock.wait()
+        logger.debug(f"{self.name} ...")
+        # self.is_running = False
+        # self._terminate_lock.wait()
+        while not self._terminate_lock.is_set():
+            self._terminate_lock.wait(1)
         self._stop_mqtt()
 
+
     def _start_mqtt(self):
-        logging.info("Starting...")
-        self.mqtt_client = mqtt.Client()
-        self.mqtt_client.on_connect = self._on_connect
-        self.mqtt_client.on_message = self._on_message
-        if config.mqtt_username:
-            self.mqtt_client.username_pw_set(config.mqtt_username, config.mqtt_password)
-        self.mqtt_client.connect(config.mqtt_address, config.mqtt_port, config.mqtt_keepalive)
-        self.mqtt_client.loop_start()
+        logger.debug(f"{self.name} ...")
+        self._mqtt_client = mqtt.Client()
+        self._mqtt_client.on_connect = self._on_connect
+        self._mqtt_client.on_message = self._on_message
+        cfg = self._config
+        if cfg.mqtt_username:
+            self._mqtt_client.username_pw_set(cfg.mqtt_username, cfg.mqtt_password)
+        logger.debug(f"addr:{cfg.mqtt_address} port:{cfg.mqtt_port} keep:{cfg.mqtt_keepalive}")
+        self._mqtt_client.connect(cfg.mqtt_address, cfg.mqtt_port, cfg.mqtt_keepalive)
+        self._mqtt_client.loop_start()
+
 
     def _stop_mqtt(self):
-        logging.warn("_stop_mqtt")
-        self.mqtt_client.disconnect()
-        self.mqtt_client.loop_stop()
-        
-    def start(self):
-        p = Process(target=self._run)
-        p.start()
+        logger.debug(f"{self.name} ...")
+        self._mqtt_client.disconnect()
+        self._mqtt_client.loop_stop()
 
-        for a in self.head_agents:
-            logging.info(f"head: {a.__module__} start")
-            a.start()
-        for a in self.body_agents:
-            logging.info(f"body: {a.__module__} start")
-            a.start()
+
+    def publish(self, topic, payload=None):
+        # logging.debug(f'{str(self._mqtt_client.socket())}, topic:{topic}, payload:{payload}')
+        ret = self._mqtt_client.publish(topic, payload)
+        # logging.debug(f'ret: {str(ret)}')
         
 
+    def terminate(self):
+        logger.warn(f"{self.name}.")
+
+        for a in self.head_agents:
+            name = a.__class__.__name__
+            self.publish(topic='terminate', payload=name)
 
+        for a in self.body_agents:
+            name = a.__class__.__name__
+            self.publish(topic='terminate', payload=name)
 
+        self._terminate_lock.set()
```

