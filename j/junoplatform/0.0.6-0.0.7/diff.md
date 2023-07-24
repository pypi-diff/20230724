# Comparing `tmp/junoplatform-0.0.6.tar.gz` & `tmp/junoplatform-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junoplatform-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "junoplatform-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `junoplatform-0.0.6.tar` & `junoplatform-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0       31 2023-07-12 03:20:16.720150 junoplatform-0.0.6/.gitignore
--rw-r--r--   0        0        0        0 2023-07-10 07:45:23.535265 junoplatform-0.0.6/README.md
--rw-r--r--   0        0        0      859 2023-07-18 03:26:45.512854 junoplatform-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 08:03:40.679259 junoplatform-0.0.6/src/junoplatform/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-17 07:58:35.111276 junoplatform-0.0.6/src/junoplatform/io/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 11:17:07.122874 junoplatform-0.0.6/src/junoplatform/io/_input/__init__.py
--rw-r--r--   0        0        0      408 2023-07-14 01:45:21.929460 junoplatform-0.0.6/src/junoplatform/io/_input/clickhouse.py
--rw-r--r--   0        0        0      237 2023-07-10 09:06:31.429958 junoplatform-0.0.6/src/junoplatform/io/_input/reader.py
--rw-r--r--   0        0        0      816 2023-07-13 12:43:43.305443 junoplatform-0.0.6/src/junoplatform/io/_output/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 02:04:06.922936 junoplatform-0.0.6/src/junoplatform/meta/__init__.py
--rw-r--r--   0        0        0     2142 2023-07-17 09:03:42.085651 junoplatform-0.0.6/src/junoplatform/meta/decorators.py
--rw-r--r--   0        0        0      866 2023-07-17 09:07:03.410699 junoplatform-0.0.6/src/junoplatform/templates/main.py
--rw-r--r--   0        0        0        0 2023-07-10 08:39:47.775803 junoplatform-0.0.6/src/junoplatform/tools/__init__.py
--rw-r--r--   0        0        0     3470 2023-07-18 03:18:44.190852 junoplatform-0.0.6/src/junoplatform/tools/cmd.py
--rw-r--r--   0        0        0      163 2023-07-13 05:56:20.979580 junoplatform-0.0.6/tests/fputs.egg-info/PKG-INFO
--rw-r--r--   0        0        0      138 2023-07-13 05:56:20.999580 junoplatform-0.0.6/tests/fputs.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-07-13 05:56:20.979580 junoplatform-0.0.6/tests/fputs.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        6 2023-07-13 05:56:20.979580 junoplatform-0.0.6/tests/fputs.egg-info/top_level.txt
--rw-r--r--   0        0        0       76 2023-07-17 08:32:09.175206 junoplatform-0.0.6/tests/input.json
--rw-r--r--   0        0        0      363 2023-07-13 05:55:54.568005 junoplatform-0.0.6/tests/setup.py
--rw-r--r--   0        0        0      866 2023-07-17 09:02:41.334545 junoplatform-0.0.6/tests/test.py
--rw-r--r--   0        0        0      782 2023-07-17 09:02:02.959111 junoplatform-0.0.6/tests/test_module.c
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 junoplatform-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       31 2023-07-12 03:20:16.720150 junoplatform-0.0.7/.gitignore
+-rw-r--r--   0        0        0      507 2023-07-19 05:36:13.410996 junoplatform-0.0.7/README.md
+-rw-r--r--   0        0        0      872 2023-07-24 08:10:28.782194 junoplatform-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 08:03:40.679259 junoplatform-0.0.7/src/junoplatform/__init__.py
+-rw-r--r--   0        0        0     2180 2023-07-24 07:19:22.526970 junoplatform-0.0.7/src/junoplatform/io/__init__.py
+-rw-r--r--   0        0        0     6770 2023-07-24 07:24:03.365887 junoplatform-0.0.7/src/junoplatform/io/_driver.py
+-rw-r--r--   0        0        0     2712 2023-07-24 07:31:48.238244 junoplatform-0.0.7/src/junoplatform/io/utils.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:04:06.922936 junoplatform-0.0.7/src/junoplatform/meta/__init__.py
+-rw-r--r--   0        0        0     2490 2023-07-24 06:40:22.971935 junoplatform-0.0.7/src/junoplatform/meta/decorators.py
+-rw-r--r--   0        0        0     1015 2023-07-24 07:20:51.249308 junoplatform-0.0.7/src/junoplatform/templates/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:39:47.775803 junoplatform-0.0.7/src/junoplatform/tools/__init__.py
+-rw-r--r--   0        0        0     6831 2023-07-24 08:02:10.605013 junoplatform-0.0.7/src/junoplatform/tools/cmd.py
+-rw-r--r--   0        0        0      163 2023-07-13 05:56:20.979580 junoplatform-0.0.7/tests/fputs.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      138 2023-07-13 05:56:20.999580 junoplatform-0.0.7/tests/fputs.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-07-13 05:56:20.979580 junoplatform-0.0.7/tests/fputs.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        6 2023-07-13 05:56:20.979580 junoplatform-0.0.7/tests/fputs.egg-info/top_level.txt
+-rw-r--r--   0        0        0       76 2023-07-17 08:32:09.175206 junoplatform-0.0.7/tests/input.json
+-rw-r--r--   0        0        0      363 2023-07-13 05:55:54.568005 junoplatform-0.0.7/tests/setup.py
+-rw-r--r--   0        0        0      202 2023-07-24 07:10:54.672586 junoplatform-0.0.7/tests/test.py
+-rw-r--r--   0        0        0      782 2023-07-17 09:02:02.959111 junoplatform-0.0.7/tests/test_module.c
+-rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 junoplatform-0.0.7/PKG-INFO
```

### Comparing `junoplatform-0.0.6/pyproject.toml` & `junoplatform-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project.scripts]
 junocli = "junoplatform.tools.cmd:main"
 
 [project]
 name = "junoplatform"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Bruce.Lu", email="lzbgt@icloud.com" },
 ]
 description = "juno AI platform lib"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -28,12 +28,13 @@
     "pyyaml",
     "clickhouse-connect",
     "pymongo",
     "questdb",
     "postgres",
     "cryptography",
     "bcrypt",
+    "redis",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lzbgt/sampleproject"
 "Bug Tracker" = "https://github.com/lzbgt/sampleproject/issues"
```

### Comparing `junoplatform-0.0.6/src/junoplatform/meta/decorators.py` & `junoplatform-0.0.7/src/junoplatform/meta/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 import numpy as np
 from threading import Thread
-from junoplatform.io import InputConfig
+from junoplatform.io import InputConfig, Storage
 from functools import wraps
 import datetime
 import time
 import logging
 import os
 import json
 
 logging.basicConfig(level=logging.INFO,
                     format='%(asctime)s %(levelname)s - %(message)s')
 class EntryPoint:
     def __init__(self, cfg_in: str|InputConfig, detached: bool = False):
         super(EntryPoint, self).__init__()
         self.cfg_in: InputConfig
         self.detached = detached
+        self.storage = Storage()
         if isinstance(cfg_in, str):
-            self.cfg_in = InputConfig(**json.load(open(cfg_in)))
+            logging.info(f"loading input spec from file: {cfg_in}")
+            try:
+                self.cfg_in = InputConfig(**json.load(open(cfg_in)))
+            except Exception as e:
+                msg = f"error in input.json: {e}"
+                logging.error(msg)
+                exit(1)
         elif isinstance(self.cfg_in, InputConfig):
+            logging.info(f"loading input spec from class: {cfg_in}")
             self.cfg_in = cfg_in
         else:
             raise Exception(f"cfg_in must be type of InputConfig or string, but provides: {type(self.cfg_in)}")
 
     def __call__(self, func):
         def thread():
            while True:
               # TODO: prepare data for func
               # mock data
               ts = datetime.datetime.now().timestamp()
               row = len(self.cfg_in.tags)
               col = self.cfg_in.items
               
               data = np.zeros((row, col)) # type: ignore
-              func(data)
+              func(data, self.storage)
               # TODO: output
               te = datetime.datetime.now().timestamp()
 
               delay = self.cfg_in.interval - (te -ts) - 0.003
               logging.info(f"delay: {delay}")
               if delay < 0: 
                  delay = 0
@@ -44,16 +52,14 @@
               
         th = Thread(target=thread)
         if self.detached:
             th.daemon = True
         th.start()
         if not self.detached:
             th.join()
-        
-
 
 def auth(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         if not os.path.exists(args[0].juno_dir) or not os.path.exists(args[0].juno_file):
             # TODO: auth token
             logging.error(f"user not authenticationd.")
```

### Comparing `junoplatform-0.0.6/src/junoplatform/templates/main.py` & `junoplatform-0.0.7/src/junoplatform/templates/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from junoplatform.meta.decorators import EntryPoint
 from junoplatform.io import *
 import logging
 import random
 
 #@EntryPoint(InputConfig(tags=["OPC_TAG1", "OPC_TAG2"], items=1440, interval=5), detached=False)
 @EntryPoint("input.json", detached=False)
-def any_algo_entry_func(data):
+def any_algo_entry_func(data, storage:Storage):
     '''
     data: numpy.ndarray
       it is automatically provided by the junoplatform framework, and its content is specified by `InputConfig` above
     '''
 
     # TODO: algo processing with input data here
     logging.info(f"processing data: {data.shape}")
     
     # TODO: construct results as dict
     opc_data = {"OPC_TAG1": random.randint(1,10), "OPC_TAG2": random.randint(1,10)}
     probe1 = {"out":random.randint(1,10)}
+    state1 = {'s1': 1}
 
     # TODO: algo oputput results
     logging.info("data processed, writing outputs:")
-    MongoOutput.write(probe1, "probe1")
-    OPCOutput.write(opc_data)
+    storage.cloud.write("probe1", probe1)
+    storage.opc.write(opc_data)
+    storage.local.write('state1', state1)
+    data = storage.local.read('state1')
+    logging.info(data)
```

### Comparing `junoplatform-0.0.6/tests/test_module.c` & `junoplatform-0.0.7/tests/test_module.c`

 * *Files identical despite different names*

