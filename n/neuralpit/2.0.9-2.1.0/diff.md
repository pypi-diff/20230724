# Comparing `tmp/neuralpit-2.0.9.tar.gz` & `tmp/neuralpit-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-2.0.9.tar", last modified: Thu Jul 20 06:03:37 2023, max compression
+gzip compressed data, was "neuralpit-2.1.0.tar", last modified: Mon Jul 24 17:34:04 2023, max compression
```

## Comparing `neuralpit-2.0.9.tar` & `neuralpit-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 06:03:37.973272 neuralpit-2.0.9/
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 06:03:05.000000 neuralpit-2.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-20 06:03:37.973272 neuralpit-2.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-20 06:03:05.000000 neuralpit-2.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-20 06:03:05.000000 neuralpit-2.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 06:03:37.973272 neuralpit-2.0.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 06:03:37.969272 neuralpit-2.0.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 06:03:37.969272 neuralpit-2.0.9/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      586 2023-07-20 06:03:05.000000 neuralpit-2.0.9/src/neuralpit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 06:03:37.973272 neuralpit-2.0.9/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 06:03:05.000000 neuralpit-2.0.9/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3353 2023-07-20 06:03:05.000000 neuralpit-2.0.9/src/neuralpit/services/conversation.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-20 06:03:05.000000 neuralpit-2.0.9/src/neuralpit/services/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 06:03:37.973272 neuralpit-2.0.9/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-20 06:03:37.000000 neuralpit-2.0.9/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-20 06:03:37.000000 neuralpit-2.0.9/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 06:03:37.000000 neuralpit-2.0.9/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-20 06:03:37.000000 neuralpit-2.0.9/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-20 06:03:37.000000 neuralpit-2.0.9/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 06:03:37.973272 neuralpit-2.0.9/test/
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-20 06:03:05.000000 neuralpit-2.0.9/test/testCreateConversation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:34:04.040292 neuralpit-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 17:33:33.000000 neuralpit-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-24 17:34:04.040292 neuralpit-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-24 17:33:33.000000 neuralpit-2.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-24 17:33:33.000000 neuralpit-2.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 17:34:04.040292 neuralpit-2.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:34:04.036292 neuralpit-2.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:34:04.036292 neuralpit-2.1.0/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-07-24 17:33:33.000000 neuralpit-2.1.0/src/neuralpit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:34:04.036292 neuralpit-2.1.0/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 17:33:33.000000 neuralpit-2.1.0/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-07-24 17:33:33.000000 neuralpit-2.1.0/src/neuralpit/services/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-24 17:33:33.000000 neuralpit-2.1.0/src/neuralpit/services/conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:34:04.040292 neuralpit-2.1.0/src/neuralpit/utils/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-24 17:33:33.000000 neuralpit-2.1.0/src/neuralpit/utils/streamer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:34:04.036292 neuralpit-2.1.0/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-24 17:34:04.000000 neuralpit-2.1.0/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-24 17:34:04.000000 neuralpit-2.1.0/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 17:34:04.000000 neuralpit-2.1.0/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-24 17:34:04.000000 neuralpit-2.1.0/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 17:34:04.000000 neuralpit-2.1.0/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:34:04.040292 neuralpit-2.1.0/test/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-07-24 17:33:33.000000 neuralpit-2.1.0/test/testCreateConversation.py
```

### Comparing `neuralpit-2.0.9/PKG-INFO` & `neuralpit-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.0.9
+Version: 2.1.0
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `neuralpit-2.0.9/pyproject.toml` & `neuralpit-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "2.0.9"
+version = "2.1.0"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-2.0.9/src/neuralpit/__init__.py` & `neuralpit-2.1.0/src/neuralpit/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,7 +16,8 @@
         if cls._instance is None:
             cls._instance = cls.__new__(cls)
             # Put any initialization here.
             cls._instance.api_endpoint = api_endpoint
             cls._instance.api_key = api_key
         return cls._instance
 
+STREAM_DELIMITER = '@@NEURALPIT@@'
```

### Comparing `neuralpit-2.0.9/src/neuralpit/services/conversation.py` & `neuralpit-2.1.0/src/neuralpit/services/conversation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 from typing import List
 import json
 from requests.compat import urljoin
-from neuralpit import NeuralPitSDK
+from neuralpit import NeuralPitSDK, STREAM_DELIMITER
+from neuralpit.utils.streamer import Streamer
 
 class ConversationService():
 
     def __init__(self) -> None:
         super().__init__()
         sdk = NeuralPitSDK.instance()
         self.api_key = sdk.api_key
@@ -50,19 +51,33 @@
     def listConversationHistory(self, conversation_id):
         get_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/history')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         get_call = requests.get(get_url, headers = headers)
         resp =  json.loads(get_call.content)
         return resp
     
+    def clearConversationHistory(self, conversation_id):
+        delete_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/history')
+        headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
+        delete_call = requests.delete(delete_url, headers = headers)
+        return True
+    
     def queryConversation(self, conversation_id, question, debug=False):
         post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/query')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         post_call = requests.post(post_url, headers = headers, json = {'question': question, 'debug': debug})
         resp =  json.loads(post_call.content)
         return resp
     
     def summarizeDocument(self, conversation_id, document_id, debug=False):
         get_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/document/{document_id}/summarize')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         post_call = requests.get(get_url, headers = headers, json = {'debug': debug})
         return post_call.content
+    
+    def queryConversationStream(self, conversation_id, question, debug=False, chunk_size=1024):
+        post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/query_stream')
+        headers = {'x-api-key':self.api_key}
+        with requests.post(post_url, headers = headers, json = {'question': question, 'debug': debug}, stream=True) as r:
+            streamer = Streamer(r.iter_content(chunk_size))
+            for item in streamer.iter_item():
+                yield item
```

### Comparing `neuralpit-2.0.9/src/neuralpit/services/conversion.py` & `neuralpit-2.1.0/src/neuralpit/services/conversion.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.0.9/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-2.1.0/src/neuralpit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.0.9
+Version: 2.1.0
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

