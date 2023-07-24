# Comparing `tmp/authomize-rest-api-client-4.3.2.tar.gz` & `tmp/authomize-rest-api-client-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.3.2.tar", last modified: Sun Jul  2 12:26:14 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.3.tar", last modified: Mon Jul 24 16:47:56 2023, max compression
```

## Comparing `authomize-rest-api-client-4.3.2.tar` & `authomize-rest-api-client-4.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2619 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.623463 authomize-rest-api-client-4.3.2/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.623463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84645 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45351 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200535 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104842 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-02 12:25:55.000000 authomize-rest-api-client-4.3.2/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-02 12:26:14.000000 authomize-rest-api-client-4.3.2/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-02 12:26:14.000000 authomize-rest-api-client-4.3.2/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 12:26:14.000000 authomize-rest-api-client-4.3.2/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-02 12:26:14.000000 authomize-rest-api-client-4.3.2/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-02 12:26:14.000000 authomize-rest-api-client-4.3.2/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-02 12:26:14.627463 authomize-rest-api-client-4.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1117 2023-07-02 12:25:58.000000 authomize-rest-api-client-4.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84645 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49598 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   200535 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115884 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-24 16:47:38.000000 authomize-rest-api-client-4.3.3/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 16:47:56.000000 authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-24 16:47:56.569186 authomize-rest-api-client-4.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-24 16:47:42.000000 authomize-rest-api-client-4.3.3/setup.py
```

### Comparing `authomize-rest-api-client-4.3.2/LICENSE.txt` & `authomize-rest-api-client-4.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/README.md` & `authomize-rest-api-client-4.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,12 +66,17 @@
 ```
 curl https://apidev.authomize.com/openapi-platform.json | jq --indent 2 . > authomize/rest_api_client/openapi/external_rest_api/openapi.json
 ```
 2.
 ```
 datamodel-codegen --use-default-kwarg --encoding=utf-8 --input authomize/rest_api_client/openapi/external_rest_api/openapi.json --output authomize/rest_api_client/generated/external_rest_api
 ```
-The main schema then is created in an `__init__.py` file, and some missing schemas are created inside another file. Then:
-3. Replace the content of `authomize/rest_api_client/generated/external_rest_api/schema.py` from the newly created `__init__.py`
-4. Add the missing schemas from the other file to the end of `schema.py`
-5. Fix the imports / errors in `schema.py`
-6. Remove all the newly created files (leave only `schema.py`)
+The main schema then is created in an `__init__.py` file, and some missing schemas are created inside another file.  
+Then:
+3. Replace the content of `authomize/rest_api_client/generated/external_rest_api/schemas.py` from the newly created `__init__.py`  
+```
+ mv authomize/rest_api_client/generated/external_rest_api/__init__.py authomize/rest_api_client/generated/external_rest_api/schemas.py
+ touch authomize/rest_api_client/generated/external_rest_api/__init__.py
+```   
+4. Add the missing schemas from the other file to the end of `schemas.py`
+5. Fix the imports / errors in `schemas.py`
+6. Remove all the newly created files (leave only `schemas.py`)
```

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-07-02T11:49:06+00:00
+#   timestamp: 2023-07-24T16:36:38+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field, constr
+from pydantic import BaseModel, Extra, Field, conint, constr
+
+from .field_class__authomize.external_rest_api.app.routes_schema import inventory
 
 
 class AccessByType(Enum):
     account = 'account'
     grouping = 'grouping'
 
 
 class AccessToType(Enum):
     asset = 'asset'
     grouping = 'grouping'
 
 
+class AccountExpansion(Enum):
+    identity = 'identity'
+    sourceApp = 'sourceApp'
+    tags = 'tags'
+    riskScores = 'riskScores'
+
+
 class AccountRiskScore(BaseModel):
     blastRadiusRiskScore: Optional[int] = Field(
         default=None,
         description='Blast Radius Risk Score',
         title='Blastradiusriskscore',
     )
     takeoverRiskScore: Optional[int] = Field(
@@ -289,16 +298,16 @@
         default=None, description='Takeover Risk Score', title='Takeoverriskscore'
     )
     blastRadiusRiskScore: Optional[int] = Field(
         default=None,
         description='Blast Radius Risk Score',
         title='Blastradiusriskscore',
     )
-    summaryRiskScore: Optional[int] = Field(
-        default=None, description='Summary Risk Score', title='Summaryriskscore'
+    overallRiskScore: Optional[int] = Field(
+        default=None, description='Summary Risk Score', title='Overallriskscore'
     )
 
 
 class IncidentExpansion(Enum):
     policy = 'policy'
     assignee = 'assignee'
 
@@ -413,27 +422,31 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='4.3.0', description='**version**', title='Version'
+        default='4.3.2', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     data: CommentSchema = Field(..., description='Actual Data', title='Data')
 
 
+class OkResponse(BaseModel):
+    ok: Optional[bool] = Field(default=True, description='OK\n', title='Ok')
+
+
 class OriginIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[str]] = Field(
         default=[], alias='$in', description='In', title='$In'
     )
@@ -485,14 +498,62 @@
     inactive = 'inactive'
 
 
 class ReviewerExpansion(Enum):
     user = 'user'
 
 
+class RiskFactorIn(BaseModel):
+    type: str = Field(
+        ...,
+        description='Type should be unique for risk factors on the same account. Different accounts can have the same risk factor type.\n',
+        title='Type',
+    )
+    score: conint(ge=0) = Field(
+        ..., description='The factor non-negative risk score.\n', title='Score'
+    )
+    title: str = Field(
+        ...,
+        description='The title of the risk factor that should be displayed on the UI.\n',
+        title='Title',
+    )
+    description: str = Field(
+        ...,
+        description='A longer description of the risk factor that explains how it was calculated, how it works and so on.\n',
+        title='Description',
+    )
+    modifiedAt: Optional[datetime] = Field(
+        default=None,
+        description='Automatically set modification time. Automatically generated.\n',
+        title='Modifiedat',
+    )
+
+
+class SearchAccountsIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
+class SearchAccountsOriginIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[str]] = Field(
+        default=[], alias='$in', description='In', title='$In'
+    )
+
+
+class SearchAccountsSortFields(Enum):
+    account_name = 'account.name'
+
+
 class SearchAssetsSortFields(Enum):
     asset_name = 'asset.name'
 
 
 class SearchGroupsAppIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -554,15 +615,14 @@
 
 
 class SearchIncidentsSortFields(Enum):
     createdAt = 'createdAt'
     updatedAt = 'updatedAt'
     severity = 'severity'
     status = 'status'
-    isResolved = 'isResolved'
 
 
 class Selection(Enum):
     keep = 'keep'
     revoke = 'revoke'
     null = 'null'
 
@@ -589,14 +649,28 @@
     order: Optional[SortOrder] = Field(
         default='ASC',
         description='Sort by ascending or descending order (ascending is the default)',
         title='Order',
     )
 
 
+class SortSchemaSearchAccountsSortFields(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    fieldName: SearchAccountsSortFields = Field(
+        ..., description='Sort the results by field name', title='FieldName'
+    )
+    order: Optional[SortOrder] = Field(
+        default='ASC',
+        description='Sort by ascending or descending order (ascending is the default)',
+        title='Order',
+    )
+
+
 class SortSchemaSearchAssetsSortFields(BaseModel):
     class Config:
         extra = Extra.forbid
 
     fieldName: SearchAssetsSortFields = Field(
         ..., description='Sort the results by field name', title='FieldName'
     )
@@ -691,26 +765,51 @@
     severity: Optional[SeverityType] = Field(
         default=None,
         description='The severity of the incident (Low, Medium, High or Critical).',
     )
 
 
 class UserSchema(BaseModel):
-    userId: str = Field(..., description='Unique ID', title='Userid')
-    userFirstName: str = Field(..., description='First Name', title='Userfirstname')
-    userLastName: str = Field(..., description='Last Name', title='Userlastname')
-    userEmail: str = Field(..., description='Email', title='Useremail')
+    id: str = Field(..., description='Unique ID', title='Id')
+    firstName: Optional[str] = Field(
+        default=None, description='First Name', title='Firstname'
+    )
+    lastName: Optional[str] = Field(
+        default=None, description='Last Name', title='Lastname'
+    )
+    email: Optional[str] = Field(default=None, description='Email', title='Email')
+
+
+class UserStatus(Enum):
+    Deleted = 'Deleted'
+    Disabled = 'Disabled'
+    Enabled = 'Enabled'
+    Staged = 'Staged'
+    Suspended = 'Suspended'
+    Unknown = 'Unknown'
 
 
 class ValidationError(BaseModel):
     loc: List[str] = Field(..., title='Location')
     msg: str = Field(..., title='Message')
     type: str = Field(..., title='Error Type')
 
 
+class AddIdentityRisksRequestSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    filter: Optional[SearchIdentitiesFilterBody] = Field(
+        default=None, description='Search filter options', title='Filter'
+    )
+    risks: List[RiskFactorIn] = Field(
+        ..., description='List of risks to add to the identity', title='Risks'
+    )
+
+
 class AicpaTsc2017(BaseModel):
     values: List[AicpaTsc2017Standard] = Field(..., description='Values')
     id: Optional[str] = Field(
         default='aicpaTsc2017', description='UniqueID', title='Id'
     )
     name: Optional[str] = Field(
         default='SOC 2 (TSC 2017)', description='Name', title='Name'
@@ -738,15 +837,15 @@
         title='Sourceapp',
     )
     createdAt: Optional[datetime] = Field(
         default=None,
         description='The date (in ISO 8601 format) that the asset was created\n',
         title='Createdat',
     )
-    lastUsedAt: Optional[datetime] = Field(
+    lastUsedAt: Optional[str] = Field(
         default=None,
         description='The date (in ISO 8601 format) of the last time that the asset was in use.',
         title='Lastusedat',
     )
     href: Optional[str] = Field(
         default=None,
         description='A link to the asset in the source application',
@@ -878,14 +977,22 @@
         title='Originid',
     )
     uniqueId: Optional[str] = Field(
         default=None,
         description='The unique ID of the group (as provided by the connector)',
         title='Uniqueid',
     )
+    createdAt: Optional[str] = Field(
+        default=None,
+        description='Type of the group in source system.',
+        title='Createdat',
+    )
+    originType: Optional[str] = Field(
+        default=None, description='Date when group was created.', title='Origintype'
+    )
 
 
 class HTTPValidationError(BaseModel):
     detail: Optional[List[ValidationError]] = Field(default=None, title='Detail')
 
 
 class IncidentEntitiesSchema(BaseModel):
@@ -1001,14 +1108,29 @@
     incidentsCount: Optional[int] = Field(
         default=None,
         description='Number of associated incidents',
         title='Incidentscount',
     )
 
 
+class RemoveIdentityRisksRequestSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    filter: Optional[SearchIdentitiesFilterBody] = Field(
+        default=None, description='Search filter options', title='Filter'
+    )
+    since: datetime = Field(
+        ..., description='Only remove risks from before this timestamp', title='Since'
+    )
+    riskTypes: List[str] = Field(
+        ..., description='List of risks to add to the identity', title='Risktypes'
+    )
+
+
 class ReviewerSchema(BaseModel):
     userId: str = Field(..., description='User ID of the Reviewer', title='Userid')
     campaignId: str = Field(..., description='Campaign ID', title='Campaignid')
     lastNotifiedAt: datetime = Field(
         ..., description='Time of last notified', title='Lastnotifiedat'
     )
     lastActiveAt: datetime = Field(
@@ -1019,31 +1141,47 @@
     )
     id: str = Field(..., description='Unique ID', title='Id')
     user: Optional[UserSchema] = Field(
         default=None, description='User Schema of the reviewer', title='User'
     )
 
 
-class SearchAssetsFilterBody(BaseModel):
+class SearchAccountsFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    originId: Optional[OriginIdFilter] = Field(
-        default=None, description='Find assets by their origin ID', title='Originid'
+    originId: Optional[SearchAccountsOriginIdFilter] = Field(
+        default=None,
+        description='Find accounts by their ID in the source system',
+        title='Originid',
     )
-    appId: Optional[AppIdFilter] = Field(
-        default=None, description='Find assets by their app ID', title='Appid'
+    authomizeId: Optional[SearchAccountsIdFilter] = Field(
+        default=None,
+        description='Find accounts by their Authomize ID',
+        title='Authomizeid',
     )
-    uniqueId: Optional[UniqueIdFilter] = Field(
-        default=None, description='Find assets by their unique ID', title='Uniqueid'
+
+
+class SearchAccountsRequestSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    pagination: Optional[PaginationRequestSchema] = Field(
+        default=None, description='Pagination metadata', title='Pagination'
     )
-    authomizeId: Optional[AssetIdFilter] = Field(
+    expand: Optional[List[AccountExpansion]] = Field(
+        default=None, description='Expand Fields'
+    )
+    sort: Optional[List[SortSchemaSearchAccountsSortFields]] = Field(
         default=None,
-        description='Find assets by their Authomize ID',
-        title='Authomizeid',
+        description='Sort the results by account fields in ascending or descending order',
+        title='Sort',
+    )
+    filter: Optional[SearchAccountsFilterBody] = Field(
+        default=None, description='Search Accounts Filter', title='Filter'
     )
 
 
 class SearchAssetsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
@@ -1054,18 +1192,16 @@
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
     expand: Optional[List[AssetExpansion]] = Field(
         default=None, description='Expand fields (to show additional information)'
     )
-    filter: Optional[SearchAssetsFilterBody] = Field(
-        default=None,
-        description='Find assets by their ID on the source system',
-        title='Filter',
+    filter: Optional[inventory.SearchAssetsFilterBody] = Field(
+        default=None, description='Search Assets Filter', title='Filter'
     )
 
 
 class SearchCampaignPermissionsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
@@ -1096,53 +1232,31 @@
     sort: Optional[List[SortSchemaFieldName]] = Field(
         default=None,
         description='Sort the results by campaign fields in ascending or descending order',
         title='Sort',
     )
 
 
-class SearchGroupsFilterBody(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    uniqueId: Optional[SearchGroupsUniqueIdFilter] = Field(
-        default=None, description='Find groups by their unique ID', title='Uniqueid'
-    )
-    originId: Optional[SearchGroupsOriginIdFilter] = Field(
-        default=None, description='Find groups by their origin ID', title='Originid'
-    )
-    appId: Optional[SearchGroupsAppIdFilter] = Field(
-        default=None, description='Find groups by their app ID', title='Appid'
-    )
-    authomizeId: Optional[SearchGroupsIdFilter] = Field(
-        default=None,
-        description='Find groups by their Authomize ID',
-        title='Authomizeid',
-    )
-
-
 class SearchGroupsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchGroupsSortFields]] = Field(
         default=None,
-        description='Sort the results by identity name in ascending or descending order',
+        description="Sort the results by group's name in ascending or descending order",
         title='Sort',
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
     expand: Optional[List[GroupExpansion]] = Field(
         default=None, description='Expand fields (to show additional information)'
     )
-    filter: Optional[SearchGroupsFilterBody] = Field(
-        default=None,
-        description='Find groups by their ID on the source system',
-        title='Filter',
+    filter: Optional[inventory.SearchGroupsFilterBody] = Field(
+        default=None, description='Search Groups Filter', title='Filter'
     )
 
 
 class SearchIdentitiesRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
@@ -1207,15 +1321,17 @@
     )
     pagination: Optional[PaginationRequestSchema] = Field(
         default=None, description='Pagination metadata', title='Pagination'
     )
 
 
 class AccountSchema(BaseModel):
-    authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
+    authomizeId: str = Field(
+        ..., description='Authomize ID of the account', title='Authomizeid'
+    )
     originId: Optional[str] = Field(
         default=None,
         description='The identifier of the account from the source system.',
         title='Originid',
     )
     uniqueId: Optional[str] = Field(
         default=None,
@@ -1228,28 +1344,43 @@
     type: str = Field(..., description='Type of account', title='Type')
     isExternal: bool = Field(
         ..., description='Is account external (Yes or No)', title='Isexternal'
     )
     email: Optional[str] = Field(
         default=None, description='Email address of account', title='Email'
     )
-    identityId: Optional[str] = Field(
-        default=None, description='ID of identitiy', title='Identityid'
-    )
     identity: Optional[RawIdentitySchema] = Field(
         default=None, description='Associated Identity', title='Identity'
     )
     sourceApp: Optional[SourceAppSchema] = Field(
         default=None, description='Associated source app ', title='Sourceapp'
     )
+    firstName: Optional[str] = Field(
+        default=None, description='First name of account', title='Firstname'
+    )
+    lastName: Optional[str] = Field(
+        default=None, description='Last name of account', title='Lastname'
+    )
     isAdmin: Optional[bool] = Field(
         default=None,
         description='Is the account an admin account (Yes or No)',
         title='Isadmin',
     )
+    status: Optional[UserStatus] = Field(default=None, description='The account status')
+    description: Optional[str] = Field(
+        default=None, description='The account description', title='Description'
+    )
+    hasMfa: Optional[bool] = Field(
+        default=None,
+        description='Does the account have MFA enabled (Yes or No)',
+        title='Hasmfa',
+    )
+    lastLoginAt: Optional[str] = Field(
+        default=None, description='Account Last Logged date', title='Lastloginat'
+    )
     tags: Optional[List[TagSchema]] = Field(
         default=None, description='Tags associated with the account.', title='Tags'
     )
     riskScore: Optional[AccountRiskScore] = Field(
         default=None, description='Risk Scores for the Account.', title='Riskscore'
     )
 
@@ -1403,14 +1534,26 @@
 class NonPaginatedResponseSchemaReviewerSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     data: ReviewerSchema = Field(..., description='Actual Data', title='Data')
 
 
+class PaginatedResponseSchemaAccountSchema(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    pagination: Optional[PaginationResponseSchema] = Field(
+        default=None, description='Pagination Metadata', title='Pagination'
+    )
+    data: List[AccountSchema] = Field(
+        ..., description='List of Actual Data', title='Data'
+    )
+
+
 class PaginatedResponseSchemaCampaignsPermissionSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
@@ -1438,21 +1581,22 @@
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[IncidentSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
 
-
 class SearchAssetsFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
     originId: Optional[OriginIdFilter] = Field(
-        default=None, description='Find assets by their origin ID', title='Originid'
+        default=None,
+        description='Find assets by their ID in the source system',
+        title='Originid',
     )
     appId: Optional[AppIdFilter] = Field(
         default=None, description='Find assets by their app ID', title='Appid'
     )
     uniqueId: Optional[UniqueIdFilter] = Field(
         default=None, description='Find assets by their unique ID', title='Uniqueid'
     )
@@ -1467,15 +1611,17 @@
     class Config:
         extra = Extra.forbid
 
     uniqueId: Optional[SearchGroupsUniqueIdFilter] = Field(
         default=None, description='Find groups by their unique ID', title='Uniqueid'
     )
     originId: Optional[SearchGroupsOriginIdFilter] = Field(
-        default=None, description='Find groups by their origin ID', title='Originid'
+        default=None,
+        description='Find groups by their ID in the source system',
+        title='Originid',
     )
     appId: Optional[SearchGroupsAppIdFilter] = Field(
         default=None, description='Find groups by their app ID', title='Appid'
     )
     authomizeId: Optional[SearchGroupsIdFilter] = Field(
         default=None,
         description='Find groups by their Authomize ID',
```

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9713658754095761%*

 * *Differences: {"'components'": "{'schemas': {'AccountSchema': {'properties': {'authomizeId': {'description': "*

 * *                 "'Authomize ID of the account'}, 'firstName': OrderedDict([('title', "*

 * *                 "'Firstname'), ('type', 'string'), ('description', 'First name of account')]), "*

 * *                 "'lastName': OrderedDict([('title', 'Lastname'), ('type', 'string'), "*

 * *                 "('description', 'Last name of account')]), 'status': OrderedDict([('allOf', "*

 * *                 "[OrderedDict([('$ref', '#/c […]*

```diff
@@ -15,14 +15,25 @@
                 "enum": [
                     "asset",
                     "grouping"
                 ],
                 "title": "AccessToType",
                 "type": "string"
             },
+            "AccountExpansion": {
+                "description": "An enumeration.",
+                "enum": [
+                    "identity",
+                    "sourceApp",
+                    "tags",
+                    "riskScores"
+                ],
+                "title": "AccountExpansion",
+                "type": "string"
+            },
             "AccountRiskScore": {
                 "properties": {
                     "blastRadiusRiskScore": {
                         "description": "Blast Radius Risk Score",
                         "title": "Blastradiusriskscore",
                         "type": "integer"
                     },
@@ -39,47 +50,67 @@
                 },
                 "title": "AccountRiskScore",
                 "type": "object"
             },
             "AccountSchema": {
                 "properties": {
                     "authomizeId": {
-                        "description": "Unique ID",
+                        "description": "Authomize ID of the account",
                         "title": "Authomizeid",
                         "type": "string"
                     },
+                    "description": {
+                        "description": "The account description",
+                        "title": "Description",
+                        "type": "string"
+                    },
                     "email": {
                         "description": "Email address of account",
                         "title": "Email",
                         "type": "string"
                     },
+                    "firstName": {
+                        "description": "First name of account",
+                        "title": "Firstname",
+                        "type": "string"
+                    },
+                    "hasMfa": {
+                        "description": "Does the account have MFA enabled (Yes or No)",
+                        "title": "Hasmfa",
+                        "type": "boolean"
+                    },
                     "identity": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/RawIdentitySchema"
                             }
                         ],
                         "description": "Associated Identity",
                         "title": "Identity"
                     },
-                    "identityId": {
-                        "description": "ID of identitiy",
-                        "title": "Identityid",
-                        "type": "string"
-                    },
                     "isAdmin": {
                         "description": "Is the account an admin account (Yes or No)",
                         "title": "Isadmin",
                         "type": "boolean"
                     },
                     "isExternal": {
                         "description": "Is account external (Yes or No)",
                         "title": "Isexternal",
                         "type": "boolean"
                     },
+                    "lastLoginAt": {
+                        "description": "Account Last Logged date",
+                        "title": "Lastloginat",
+                        "type": "string"
+                    },
+                    "lastName": {
+                        "description": "Last name of account",
+                        "title": "Lastname",
+                        "type": "string"
+                    },
                     "name": {
                         "description": "Name of account",
                         "title": "Name",
                         "type": "string"
                     },
                     "originId": {
                         "description": "The identifier of the account from the source system.",
@@ -100,14 +131,22 @@
                             {
                                 "$ref": "#/components/schemas/SourceAppSchema"
                             }
                         ],
                         "description": "Associated source app ",
                         "title": "Sourceapp"
                     },
+                    "status": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/UserStatus"
+                            }
+                        ],
+                        "description": "The account status"
+                    },
                     "tags": {
                         "description": "Tags associated with the account.",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
@@ -127,14 +166,42 @@
                     "authomizeId",
                     "type",
                     "isExternal"
                 ],
                 "title": "AccountSchema",
                 "type": "object"
             },
+            "AddIdentityRisksRequestSchema": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "filter": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchIdentitiesFilterBody"
+                            }
+                        ],
+                        "description": "Search filter options",
+                        "title": "Filter"
+                    },
+                    "risks": {
+                        "description": "List of risks to add to the identity",
+                        "items": {
+                            "$ref": "#/components/schemas/RiskFactorIn"
+                        },
+                        "title": "Risks",
+                        "type": "array"
+                    }
+                },
+                "required": [
+                    "risks"
+                ],
+                "title": "AddIdentityRisksRequestSchema",
+                "type": "object"
+            },
             "AddIncidentCommentRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "content": {
                         "description": "Content of comment.",
                         "maxLength": 1025,
@@ -281,15 +348,14 @@
                     "incidentsCount": {
                         "description": "Number of associated incidents",
                         "title": "Incidentscount",
                         "type": "integer"
                     },
                     "lastUsedAt": {
                         "description": "The date (in ISO 8601 format) of the last time that the asset was in use.",
-                        "format": "date-time",
                         "title": "Lastusedat",
                         "type": "string"
                     },
                     "name": {
                         "description": "Name of the asset (for example, application, virtual machine, file, etc.)",
                         "title": "Name",
                         "type": "string"
@@ -848,14 +914,19 @@
             "GroupSchema": {
                 "properties": {
                     "authomizeId": {
                         "description": "Authomize ID of the Group.",
                         "title": "Authomizeid",
                         "type": "string"
                     },
+                    "createdAt": {
+                        "description": "Type of the group in source system.",
+                        "title": "Createdat",
+                        "type": "string"
+                    },
                     "incidentsCount": {
                         "description": "Number of incidents associated with the group.",
                         "title": "Incidentscount",
                         "type": "integer"
                     },
                     "members": {
                         "default": [],
@@ -872,14 +943,19 @@
                         "type": "string"
                     },
                     "originId": {
                         "description": "The ID of the group on the source system",
                         "title": "Originid",
                         "type": "string"
                     },
+                    "originType": {
+                        "description": "Date when group was created.",
+                        "title": "Origintype",
+                        "type": "string"
+                    },
                     "ownerId": {
                         "description": "Authomize ID of the Group Owner.",
                         "title": "Ownerid",
                         "type": "string"
                     },
                     "sourceApp": {
                         "allOf": [
@@ -956,17 +1032,17 @@
             "IdentityRiskScore": {
                 "properties": {
                     "blastRadiusRiskScore": {
                         "description": "Blast Radius Risk Score",
                         "title": "Blastradiusriskscore",
                         "type": "integer"
                     },
-                    "summaryRiskScore": {
+                    "overallRiskScore": {
                         "description": "Summary Risk Score",
-                        "title": "Summaryriskscore",
+                        "title": "Overallriskscore",
                         "type": "integer"
                     },
                     "takeoverRiskScore": {
                         "description": "Takeover Risk Score",
                         "title": "Takeoverriskscore",
                         "type": "integer"
                     }
@@ -1501,15 +1577,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "4.3.0",
+                        "default": "4.3.2",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1590,14 +1666,26 @@
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NonPaginatedResponseSchema[ReviewerSchema]",
                 "type": "object"
             },
+            "OkResponse": {
+                "properties": {
+                    "ok": {
+                        "default": true,
+                        "description": "OK\n",
+                        "title": "Ok",
+                        "type": "boolean"
+                    }
+                },
+                "title": "OkResponse",
+                "type": "object"
+            },
             "OriginIdFilter": {
                 "additionalProperties": false,
                 "properties": {
                     "$in": {
                         "default": [],
                         "description": "In",
                         "items": {
@@ -1606,14 +1694,41 @@
                         "title": "$In",
                         "type": "array"
                     }
                 },
                 "title": "OriginIdFilter",
                 "type": "object"
             },
+            "PaginatedResponseSchema_AccountSchema_": {
+                "additionalProperties": false,
+                "properties": {
+                    "data": {
+                        "description": "List of Actual Data",
+                        "items": {
+                            "$ref": "#/components/schemas/AccountSchema"
+                        },
+                        "title": "Data",
+                        "type": "array"
+                    },
+                    "pagination": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/PaginationResponseSchema"
+                            }
+                        ],
+                        "description": "Pagination Metadata",
+                        "title": "Pagination"
+                    }
+                },
+                "required": [
+                    "data"
+                ],
+                "title": "PaginatedResponseSchema[AccountSchema]",
+                "type": "object"
+            },
             "PaginatedResponseSchema_AssetSchema_": {
                 "additionalProperties": false,
                 "properties": {
                     "data": {
                         "description": "List of Actual Data",
                         "items": {
                             "$ref": "#/components/schemas/AssetSchema"
@@ -1909,14 +2024,49 @@
                 },
                 "required": [
                     "authomizeId"
                 ],
                 "title": "RawIdentitySchema",
                 "type": "object"
             },
+            "RemoveIdentityRisksRequestSchema": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "filter": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchIdentitiesFilterBody"
+                            }
+                        ],
+                        "description": "Search filter options",
+                        "title": "Filter"
+                    },
+                    "riskTypes": {
+                        "description": "List of risks to add to the identity",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Risktypes",
+                        "type": "array"
+                    },
+                    "since": {
+                        "description": "Only remove risks from before this timestamp",
+                        "format": "date-time",
+                        "title": "Since",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "since",
+                    "riskTypes"
+                ],
+                "title": "RemoveIdentityRisksRequestSchema",
+                "type": "object"
+            },
             "ReviewStatus": {
                 "description": "An enumeration.",
                 "enum": [
                     "pending",
                     "completed",
                     "reviewing",
                     "notified",
@@ -1990,14 +2140,160 @@
                     "lastActiveAt",
                     "reviewStatus",
                     "id"
                 ],
                 "title": "ReviewerSchema",
                 "type": "object"
             },
+            "RiskFactorIn": {
+                "properties": {
+                    "description": {
+                        "description": "A longer description of the risk factor that explains how it was calculated, how it works and so on.\n",
+                        "title": "Description",
+                        "type": "string"
+                    },
+                    "modifiedAt": {
+                        "description": "Automatically set modification time. Automatically generated.\n",
+                        "format": "date-time",
+                        "title": "Modifiedat",
+                        "type": "string"
+                    },
+                    "score": {
+                        "description": "The factor non-negative risk score.\n",
+                        "minimum": 0,
+                        "title": "Score",
+                        "type": "integer"
+                    },
+                    "title": {
+                        "description": "The title of the risk factor that should be displayed on the UI.\n",
+                        "title": "Title",
+                        "type": "string"
+                    },
+                    "type": {
+                        "description": "Type should be unique for risk factors on the same account. Different accounts can have the same risk factor type.\n",
+                        "title": "Type",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "type",
+                    "score",
+                    "title",
+                    "description"
+                ],
+                "title": "RiskFactorIn",
+                "type": "object"
+            },
+            "SearchAccountsFilterBody": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "authomizeId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchAccountsIdFilter"
+                            }
+                        ],
+                        "description": "Find accounts by their Authomize ID",
+                        "title": "Authomizeid"
+                    },
+                    "originId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchAccountsOriginIdFilter"
+                            }
+                        ],
+                        "description": "Find accounts by their ID in the source system",
+                        "title": "Originid"
+                    }
+                },
+                "title": "SearchAccountsFilterBody",
+                "type": "object"
+            },
+            "SearchAccountsIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchAccountsIdFilter",
+                "type": "object"
+            },
+            "SearchAccountsOriginIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "default": [],
+                        "description": "In",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "$In",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchAccountsOriginIdFilter",
+                "type": "object"
+            },
+            "SearchAccountsRequestSchema": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "expand": {
+                        "description": "Expand Fields",
+                        "items": {
+                            "$ref": "#/components/schemas/AccountExpansion"
+                        },
+                        "type": "array"
+                    },
+                    "filter": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchAccountsFilterBody"
+                            }
+                        ],
+                        "description": "Search Accounts Filter",
+                        "title": "Filter"
+                    },
+                    "pagination": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/PaginationRequestSchema"
+                            }
+                        ],
+                        "description": "Pagination metadata",
+                        "title": "Pagination"
+                    },
+                    "sort": {
+                        "description": "Sort the results by account fields in ascending or descending order",
+                        "items": {
+                            "$ref": "#/components/schemas/SortSchema_SearchAccountsSortFields_"
+                        },
+                        "title": "Sort",
+                        "type": "array"
+                    }
+                },
+                "title": "SearchAccountsRequestSchema",
+                "type": "object"
+            },
+            "SearchAccountsSortFields": {
+                "description": "An enumeration.",
+                "enum": [
+                    "account.name"
+                ],
+                "title": "SearchAccountsSortFields",
+                "type": "string"
+            },
             "SearchAssetsRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "expand": {
                         "description": "Expand fields (to show additional information)",
                         "items": {
@@ -2007,15 +2303,15 @@
                     },
                     "filter": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/_class__authomize.external_rest_api.app.routes_schema.inventory.SearchAssetsFilterBody__"
                             }
                         ],
-                        "description": "Find assets by their ID on the source system",
+                        "description": "Search Assets Filter",
                         "title": "Filter"
                     },
                     "pagination": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
@@ -2174,28 +2470,28 @@
                     },
                     "filter": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/_class__authomize.external_rest_api.app.routes_schema.inventory.SearchGroupsFilterBody__"
                             }
                         ],
-                        "description": "Find groups by their ID on the source system",
+                        "description": "Search Groups Filter",
                         "title": "Filter"
                     },
                     "pagination": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
                         "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort the results by identity name in ascending or descending order",
+                        "description": "Sort the results by group's name in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_SearchGroupsSortFields_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
@@ -2415,16 +2711,15 @@
             },
             "SearchIncidentsSortFields": {
                 "description": "An enumeration.",
                 "enum": [
                     "createdAt",
                     "updatedAt",
                     "severity",
-                    "status",
-                    "isResolved"
+                    "status"
                 ],
                 "title": "SearchIncidentsSortFields",
                 "type": "string"
             },
             "Selection": {
                 "description": "An enumeration.",
                 "enum": [
@@ -2478,14 +2773,43 @@
                 },
                 "required": [
                     "fieldName"
                 ],
                 "title": "SortSchema[FieldName]",
                 "type": "object"
             },
+            "SortSchema_SearchAccountsSortFields_": {
+                "additionalProperties": false,
+                "properties": {
+                    "fieldName": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchAccountsSortFields"
+                            }
+                        ],
+                        "description": "Sort the results by field name",
+                        "title": "FieldName"
+                    },
+                    "order": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SortOrder"
+                            }
+                        ],
+                        "default": "ASC",
+                        "description": "Sort by ascending or descending order (ascending is the default)",
+                        "title": "Order"
+                    }
+                },
+                "required": [
+                    "fieldName"
+                ],
+                "title": "SortSchema[SearchAccountsSortFields]",
+                "type": "object"
+            },
             "SortSchema_SearchAssetsSortFields_": {
                 "additionalProperties": false,
                 "properties": {
                     "fieldName": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchAssetsSortFields"
@@ -2686,44 +3010,54 @@
                     }
                 },
                 "title": "UpdateIncidentRequestSchema",
                 "type": "object"
             },
             "UserSchema": {
                 "properties": {
-                    "userEmail": {
+                    "email": {
                         "description": "Email",
-                        "title": "Useremail",
+                        "title": "Email",
                         "type": "string"
                     },
-                    "userFirstName": {
+                    "firstName": {
                         "description": "First Name",
-                        "title": "Userfirstname",
+                        "title": "Firstname",
                         "type": "string"
                     },
-                    "userId": {
+                    "id": {
                         "description": "Unique ID",
-                        "title": "Userid",
+                        "title": "Id",
                         "type": "string"
                     },
-                    "userLastName": {
+                    "lastName": {
                         "description": "Last Name",
-                        "title": "Userlastname",
+                        "title": "Lastname",
                         "type": "string"
                     }
                 },
                 "required": [
-                    "userId",
-                    "userFirstName",
-                    "userLastName",
-                    "userEmail"
+                    "id"
                 ],
                 "title": "UserSchema",
                 "type": "object"
             },
+            "UserStatus": {
+                "description": "An enumeration.",
+                "enum": [
+                    "Deleted",
+                    "Disabled",
+                    "Enabled",
+                    "Staged",
+                    "Suspended",
+                    "Unknown"
+                ],
+                "title": "UserStatus",
+                "type": "string"
+            },
             "ValidationError": {
                 "properties": {
                     "loc": {
                         "items": {
                             "type": "string"
                         },
                         "title": "Location",
@@ -2770,15 +3104,15 @@
                     },
                     "originId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/OriginIdFilter"
                             }
                         ],
-                        "description": "Find assets by their origin ID",
+                        "description": "Find assets by their ID in the source system",
                         "title": "Originid"
                     },
                     "uniqueId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/UniqueIdFilter"
                             }
@@ -2814,15 +3148,15 @@
                     },
                     "originId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchGroupsOriginIdFilter"
                             }
                         ],
-                        "description": "Find groups by their origin ID",
+                        "description": "Find groups by their ID in the source system",
                         "title": "Originid"
                     },
                     "uniqueId": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SearchGroupsUniqueIdFilter"
                             }
@@ -2842,15 +3176,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.3.0",
+        "version": "4.3.2",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -3409,14 +3743,61 @@
                 ],
                 "summary": "Retrieve Incidents Extended",
                 "tags": [
                     "Incident"
                 ]
             }
         },
+        "/v2/inventory/accounts/search": {
+            "post": {
+                "description": "Search Accounts",
+                "operationId": "search_accounts_v2_inventory_accounts_search_post",
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/SearchAccountsRequestSchema"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/PaginatedResponseSchema_AccountSchema_"
+                                }
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    }
+                },
+                "security": [
+                    {
+                        "APIKeyHeader": []
+                    }
+                ],
+                "summary": "Search Accounts",
+                "tags": [
+                    "Inventory"
+                ]
+            }
+        },
         "/v2/inventory/assets/search": {
             "post": {
                 "description": "Find specific assets on Authomize and get related data (as found on the asset\u2019s Single Entity page)",
                 "operationId": "search_assets_v2_inventory_assets_search_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
@@ -3503,14 +3884,106 @@
                 ],
                 "summary": "Search Groups",
                 "tags": [
                     "Inventory"
                 ]
             }
         },
+        "/v2/inventory/identities/risk": {
+            "delete": {
+                "description": "Add takeover risk factors to accounts in the identity",
+                "operationId": "remove_identity_risks_v2_inventory_identities_risk_delete",
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/RemoveIdentityRisksRequestSchema"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/OkResponse"
+                                }
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    }
+                },
+                "security": [
+                    {
+                        "APIKeyHeader": []
+                    }
+                ],
+                "summary": "Remove Identity Risks",
+                "tags": [
+                    "Inventory"
+                ]
+            },
+            "post": {
+                "description": "Add takeover risk factors to accounts in the identity",
+                "operationId": "add_identity_risks_v2_inventory_identities_risk_post",
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "$ref": "#/components/schemas/AddIdentityRisksRequestSchema"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/OkResponse"
+                                }
+                            }
+                        },
+                        "description": "Successful Response"
+                    },
+                    "422": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/HTTPValidationError"
+                                }
+                            }
+                        },
+                        "description": "Validation Error"
+                    }
+                },
+                "security": [
+                    {
+                        "APIKeyHeader": []
+                    }
+                ],
+                "summary": "Add Identity Risks",
+                "tags": [
+                    "Inventory"
+                ]
+            }
+        },
         "/v2/inventory/identities/search": {
             "post": {
                 "description": "Find specific identities on Authomize and get related data (as found on Identity Single Entity page). Search by email address or AuthomizeID.",
                 "operationId": "search_identities_v2_inventory_identities_search_post",
                 "requestBody": {
                     "content": {
                         "application/json": {
```

### Comparing `authomize-rest-api-client-4.3.2/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.3/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.2/setup.py` & `authomize-rest-api-client-4.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.3.2',
+        version='4.3.3',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

