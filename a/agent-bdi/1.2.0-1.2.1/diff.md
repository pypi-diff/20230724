# Comparing `tmp/agent-bdi-1.2.0.tar.gz` & `tmp/agent-bdi-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-bdi-1.2.0.tar", last modified: Mon Jul 24 11:33:26 2023, max compression
+gzip compressed data, was "agent-bdi-1.2.1.tar", last modified: Mon Jul 24 13:15:55 2023, max compression
```

## Comparing `agent-bdi-1.2.0.tar` & `agent-bdi-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.496457 agent-bdi-1.2.0/
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/LICENSE.md
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/MANIFEST.in
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     3149 2023-07-24 11:33:26.496457 agent-bdi-1.2.0/PKG-INFO
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     2612 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/README.md
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      659 2023-07-24 11:33:26.496457 agent-bdi-1.2.0/setup.cfg
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      856 2023-07-24 11:26:34.000000 agent-bdi-1.2.0/setup.py
-drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.495457 agent-bdi-1.2.0/src/
-drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.495457 agent-bdi-1.2.0/src/agent_bdi.egg-info/
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     3149 2023-07-24 11:33:26.000000 agent-bdi-1.2.0/src/agent_bdi.egg-info/PKG-INFO
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      466 2023-07-24 11:33:26.000000 agent-bdi-1.2.0/src/agent_bdi.egg-info/SOURCES.txt
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        1 2023-07-24 11:33:26.000000 agent-bdi-1.2.0/src/agent_bdi.egg-info/dependency_links.txt
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       11 2023-07-24 11:33:26.000000 agent-bdi-1.2.0/src/agent_bdi.egg-info/top_level.txt
-drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.495457 agent-bdi-1.2.0/src/core/
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      302 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/Agent.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       56 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/Belief.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       50 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/Desire.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       53 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/Intention.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/core/__init__.py
-drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 11:33:26.496457 agent-bdi-1.2.0/src/holon/
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      111 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/holon/Blackboard.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      436 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/holon/Heart.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     1896 2023-07-05 09:54:01.000000 agent-bdi-1.2.0/src/holon/Helper.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     4974 2023-07-11 18:17:19.000000 agent-bdi-1.2.0/src/holon/HolonicAgent.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       69 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/holon/HolonicDesire.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       81 2023-07-03 13:41:25.000000 agent-bdi-1.2.0/src/holon/HolonicIntention.py
--rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      377 2023-07-05 10:07:40.000000 agent-bdi-1.2.0/src/holon/__init__.py
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 13:15:55.698435 agent-bdi-1.2.1/
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/LICENSE.md
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/MANIFEST.in
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     3149 2023-07-24 13:15:55.698435 agent-bdi-1.2.1/PKG-INFO
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     2612 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/README.md
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      659 2023-07-24 13:15:55.699436 agent-bdi-1.2.1/setup.cfg
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      856 2023-07-24 13:06:20.000000 agent-bdi-1.2.1/setup.py
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 13:15:55.697435 agent-bdi-1.2.1/src/
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 13:15:55.697435 agent-bdi-1.2.1/src/agent_bdi.egg-info/
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     3149 2023-07-24 13:15:55.000000 agent-bdi-1.2.1/src/agent_bdi.egg-info/PKG-INFO
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      446 2023-07-24 13:15:55.000000 agent-bdi-1.2.1/src/agent_bdi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        1 2023-07-24 13:15:55.000000 agent-bdi-1.2.1/src/agent_bdi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       11 2023-07-24 13:15:55.000000 agent-bdi-1.2.1/src/agent_bdi.egg-info/top_level.txt
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 13:15:55.698435 agent-bdi-1.2.1/src/core/
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      302 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/core/Agent.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       56 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/core/Belief.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       50 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/core/Desire.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       53 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/core/Intention.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)        0 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/core/__init__.py
+drwxrwxr-x   0 ericxu    (1001) ericxu    (1001)        0 2023-07-24 13:15:55.698435 agent-bdi-1.2.1/src/holon/
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      111 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/holon/Blackboard.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      436 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/holon/Heart.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)     4981 2023-07-24 12:58:34.000000 agent-bdi-1.2.1/src/holon/HolonicAgent.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       69 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/holon/HolonicDesire.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)       81 2023-07-03 13:41:25.000000 agent-bdi-1.2.1/src/holon/HolonicIntention.py
+-rw-rw-r--   0 ericxu    (1001) ericxu    (1001)      377 2023-07-05 10:07:40.000000 agent-bdi-1.2.1/src/holon/__init__.py
```

### Comparing `agent-bdi-1.2.0/PKG-INFO` & `agent-bdi-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 1.2.0
+Version: 1.2.1
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-1.2.0/README.md` & `agent-bdi-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `agent-bdi-1.2.0/setup.cfg` & `agent-bdi-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `agent-bdi-1.2.0/setup.py` & `agent-bdi-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "agent-bdi",
-    version = "1.2.0",
+    version = "1.2.1",
     author = "Ming Fang Shiu",
     author_email='avatar.xu@gmail.com',
     description='Agent BDI framework',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mfshiu/abdi.git",
     project_urls = {
```

### Comparing `agent-bdi-1.2.0/src/agent_bdi.egg-info/PKG-INFO` & `agent-bdi-1.2.1/src/agent_bdi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 1.2.0
+Version: 1.2.1
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-1.2.0/src/holon/HolonicAgent.py` & `agent-bdi-1.2.1/src/holon/HolonicAgent.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import time 
 
 import paho.mqtt.client as mqtt
 
 currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parentdir = os.path.dirname(currentdir)
 sys.path.insert(0, parentdir) 
-from holon import Helper
+#from tests.guide import Helper
 from core.Agent import Agent
 from holon.Blackboard import Blackboard
 from holon.HolonicDesire import HolonicDesire
 from holon.HolonicIntention import HolonicIntention
 from holon import config
 
 logger = logging.getLogger('ABDI')
```

