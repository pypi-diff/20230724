# Comparing `tmp/biggo_pms_api_python-1.0.0.tar.gz` & `tmp/biggo_pms_api_python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biggo_pms_api_python-1.0.0.tar", last modified: Mon Jul 24 05:21:16 2023, max compression
+gzip compressed data, was "biggo_pms_api_python-1.0.1.tar", last modified: Mon Jul 24 05:25:33 2023, max compression
```

## Comparing `biggo_pms_api_python-1.0.0.tar` & `biggo_pms_api_python-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:21:16.041884 biggo_pms_api_python-1.0.0/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1069 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.0.0/LICENSE
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 05:21:16.041884 biggo_pms_api_python-1.0.0/PKG-INFO
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1823 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.0.0/README.md
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:21:16.041884 biggo_pms_api_python-1.0.0/biggo_pms_api_python/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)        0 2023-07-24 02:38:22.000000 biggo_pms_api_python-1.0.0/biggo_pms_api_python/__init__.py
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      451 2023-07-24 01:44:32.000000 biggo_pms_api_python-1.0.0/biggo_pms_api_python/error.py
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     7414 2023-07-24 02:43:54.000000 biggo_pms_api_python-1.0.0/biggo_pms_api_python/index.py
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:21:16.041884 biggo_pms_api_python-1.0.0/biggo_pms_api_python.egg-info/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 05:21:16.000000 biggo_pms_api_python-1.0.0/biggo_pms_api_python.egg-info/PKG-INFO
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 05:21:16.000000 biggo_pms_api_python-1.0.0/biggo_pms_api_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 05:21:16.000000 biggo_pms_api_python-1.0.0/biggo_pms_api_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)       21 2023-07-24 05:21:16.000000 biggo_pms_api_python-1.0.0/biggo_pms_api_python.egg-info/top_level.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)       38 2023-07-24 05:21:16.041884 biggo_pms_api_python-1.0.0/setup.cfg
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      304 2023-07-24 05:21:03.000000 biggo_pms_api_python-1.0.0/setup.py
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1069 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.0.1/LICENSE
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      261 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/PKG-INFO
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1823 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.0.1/README.md
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/biggo_pms_api_python/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)        0 2023-07-24 02:38:22.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python/__init__.py
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      451 2023-07-24 01:44:32.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python/error.py
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     7422 2023-07-24 05:25:20.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python/index.py
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      261 2023-07-24 05:25:33.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 05:25:33.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 05:25:33.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       21 2023-07-24 05:25:33.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/top_level.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       38 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/setup.cfg
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      284 2023-07-24 05:24:55.000000 biggo_pms_api_python-1.0.1/setup.py
```

### Comparing `biggo_pms_api_python-1.0.0/LICENSE` & `biggo_pms_api_python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biggo_pms_api_python-1.0.0/README.md` & `biggo_pms_api_python-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `biggo_pms_api_python-1.0.0/biggo_pms_api_python/index.py` & `biggo_pms_api_python-1.0.1/biggo_pms_api_python/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import os
 import requests
 import base64
 import time
 from datetime import datetime
-from error import BigGoAuthError, BigGoError
-import asyncio
+from biggo_pms_api_python.error import BigGoAuthError, BigGoError
 
 class BiggoAPIPMS:
     def __init__(self, clientID: str, clientSecret: str):
         self.clientID = clientID
         self.clientSecret = clientSecret
         self.accessToken = ''
         self.tokenType = 'Bearer'
@@ -31,18 +30,18 @@
         return self
 
     def is_token_expired(self) -> bool:
         return self.accessToken == '' or self.expiresAt < int(time.time())
 
     async def get_token(self):
         if not self.accessToken or self.is_token_expired():
-            await self.renew_token()
+            await self._renew_token()
         return self.accessToken
 
-    async def renew_token(self):
+    async def _renew_token(self):
         self.accessToken = ''
         self.tokenType = 'Bearer'
         self.expiresAt = 0
         basic_auth_header = f"Basic {base64.b64encode(f'{self.clientID}:{self.clientSecret}'.encode()).decode()}"
 
         try:
             response = requests.post('https://api.biggo.com/auth/v1/token', data={
```

