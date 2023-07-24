# Comparing `tmp/globus-automate-client-0.6.tar.gz` & `tmp/globus-automate-client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-automate-client-0.6.tar", last modified: Mon Oct 14 19:10:11 2019, max compression
+gzip compressed data, was "globus-automate-client-0.7.0.tar", last modified: Thu Jul 16 15:45:42 2020, max compression
```

## Comparing `globus-automate-client-0.6.tar` & `globus-automate-client-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1314 2019-10-14 18:43:03.817737 globus-automate-client-0.6/README.rst
--rw-r--r--   0        0        0      492 2019-10-14 18:43:03.817737 globus-automate-client-0.6/globus_automate_client/__init__.py
--rw-r--r--   0        0        0     1844 2019-10-14 18:43:03.817737 globus-automate-client-0.6/globus_automate_client/action_client.py
--rw-r--r--   0        0        0     6222 2019-10-14 18:43:03.821737 globus-automate-client-0.6/globus_automate_client/flows_client.py
--rw-r--r--   0        0        0     3267 2019-10-14 18:43:03.821737 globus-automate-client-0.6/globus_automate_client/graphviz_rendering.py
--rw-r--r--   0        0        0     1549 2019-10-14 18:43:03.821737 globus-automate-client-0.6/globus_automate_client/helpers.py
--rw-r--r--   0        0        0    19476 2019-10-14 19:04:18.308771 globus-automate-client-0.6/globus_automate_client/main.py
--rw-r--r--   0        0        0     4990 2019-10-14 19:04:18.308771 globus-automate-client-0.6/globus_automate_client/queues_client.py
--rw-r--r--   0        0        0     2742 2019-10-14 18:43:03.821737 globus-automate-client-0.6/globus_automate_client/sync_and_identifier.json
--rw-r--r--   0        0        0     5029 2019-10-14 18:43:03.821737 globus-automate-client-0.6/globus_automate_client/token_management.py
--rw-r--r--   0        0        0     1318 2019-10-14 19:10:01.134201 globus-automate-client-0.6/pyproject.toml
--rw-r--r--   0        0        0     2103 1970-01-01 00:00:00.000000 globus-automate-client-0.6/setup.py
--rw-r--r--   0        0        0     2198 1970-01-01 00:00:00.000000 globus-automate-client-0.6/PKG-INFO
+-rw-r--r--   0        0        0    37351 2020-07-13 23:15:26.126721 globus-automate-client-0.7.0/README.rst
+-rw-r--r--   0        0        0      531 2020-07-16 15:44:48.415704 globus-automate-client-0.7.0/globus_automate_client/__init__.py
+-rw-r--r--   0        0        0     2136 2020-07-16 15:10:22.277354 globus-automate-client-0.7.0/globus_automate_client/action_client.py
+-rw-r--r--   0        0        0     4691 2020-07-16 15:10:22.278437 globus-automate-client-0.7.0/globus_automate_client/cli/actions.py
+-rw-r--r--   0        0        0     3870 2020-07-16 15:10:22.279517 globus-automate-client-0.7.0/globus_automate_client/cli/callbacks.py
+-rw-r--r--   0        0        0    12401 2020-07-16 15:10:22.280232 globus-automate-client-0.7.0/globus_automate_client/cli/flows.py
+-rw-r--r--   0        0        0     2491 2020-07-16 15:10:22.280981 globus-automate-client-0.7.0/globus_automate_client/cli/helpers.py
+-rw-r--r--   0        0        0      730 2020-07-16 15:44:48.416087 globus-automate-client-0.7.0/globus_automate_client/cli/main.py
+-rw-r--r--   0        0        0     4932 2020-07-16 15:10:22.282417 globus-automate-client-0.7.0/globus_automate_client/cli/queues.py
+-rw-r--r--   0        0        0     6071 2020-07-16 15:10:22.283111 globus-automate-client-0.7.0/globus_automate_client/flows_client.py
+-rw-r--r--   0        0        0     3267 2020-07-13 22:36:32.910472 globus-automate-client-0.7.0/globus_automate_client/graphviz_rendering.py
+-rw-r--r--   0        0        0     4990 2020-07-13 22:36:30.198538 globus-automate-client-0.7.0/globus_automate_client/queues_client.py
+-rw-r--r--   0        0        0     5030 2020-07-16 15:10:22.286134 globus-automate-client-0.7.0/globus_automate_client/token_management.py
+-rw-r--r--   0        0        0     1477 2020-07-16 15:44:48.417009 globus-automate-client-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    38641 2020-07-16 15:45:42.516987 globus-automate-client-0.7.0/setup.py
+-rw-r--r--   0        0        0    38330 2020-07-16 15:45:42.519397 globus-automate-client-0.7.0/PKG-INFO
```

### Comparing `globus-automate-client-0.6/globus_automate_client/action_client.py` & `globus-automate-client-0.7.0/globus_automate_client/action_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,34 @@
     AccessTokenAuthorizer,
     ClientCredentialsAuthorizer,
     GlobusHTTPResponse,
     RefreshTokenAuthorizer,
 )
 from globus_sdk.base import BaseClient
 
+CLIENT_ID = "e6c75d97-532a-4c88-b031-8584a319fa3e"
+
 
 class ActionClient(BaseClient):
     allowed_authorizer_types = (
         AccessTokenAuthorizer,
         RefreshTokenAuthorizer,
         ClientCredentialsAuthorizer,
     )
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
+    @property
+    def action_scope(self) -> str:
+        if not hasattr(self, "_action_scope"):
+            resp = self.introspect()
+            self._action_scope = resp.data.get("globus_auth_scope", "")
+        return self._action_scope
+
     def introspect(self, **kwargs) -> GlobusHTTPResponse:
         headers: Dict = {}
         if self.authorizer is not None:
             self.authorizer.set_authorization_header(headers)
         resp = requests.get(self.base_url, headers=headers)
         return self.default_response_class(resp, client=self)
```

### Comparing `globus-automate-client-0.6/globus_automate_client/flows_client.py` & `globus-automate-client-0.7.0/globus_automate_client/flows_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import uuid
 from typing import Any, Dict, List, Mapping, Optional
 
 from globus_sdk import (
     AccessTokenAuthorizer,
     ClientCredentialsAuthorizer,
     GlobusHTTPResponse,
     RefreshTokenAuthorizer,
 )
 from globus_sdk.base import BaseClient
 
 from .token_management import get_access_token_for_scope, get_access_tokens_for_scopes
 
-_prod_flows_base_url = "https://flows.automate.globus.org"
+PROD_FLOWS_BASE_URL = "https://flows.globus.org"
 
 MANAGE_FLOWS_SCOPE = (
     "https://auth.globus.org/scopes/eec9b274-0c81-4334-bdc2-54e90e689b9a/manage_flows"
 )
 VIEW_FLOWS_SCOPE = (
     "https://auth.globus.org/scopes/eec9b274-0c81-4334-bdc2-54e90e689b9a/view_flows"
 )
@@ -142,22 +141,20 @@
         flow_token = get_access_token_for_scope(flow_scope, self.client_id)
         self.authorizer = AccessTokenAuthorizer(flow_token)
         params = {"reverse_order": reverse_order, "limit": limit}
         return self.get(
             f"/flows/{flow_id}/{flow_action_id}/log", params=params, **kwargs
         )
 
-    def delete_flow(self, flow_id: str, flow_scope: Optional[str], **kwargs):
-        if flow_scope is None:
-            flow_scope = self._scope_for_flow(flow_id)
+    def delete_flow(self, flow_id: str, **kwargs):
         return self.delete(f"/flows/{flow_id}", **kwargs)
 
 
 def create_flows_client(
-    client_id: str, base_url: str = "https://flows.automate.globus.org"
+    client_id: str, base_url: str = PROD_FLOWS_BASE_URL
 ) -> FlowsClient:
     access_tokens = get_access_tokens_for_scopes(ALL_FLOW_SCOPES, client_id)
     temp_access_token = access_tokens.get(MANAGE_FLOWS_SCOPE)
     authorizer = AccessTokenAuthorizer(temp_access_token)
     return FlowsClient(
         access_tokens,
         client_id,
```

### Comparing `globus-automate-client-0.6/globus_automate_client/graphviz_rendering.py` & `globus-automate-client-0.7.0/globus_automate_client/graphviz_rendering.py`

 * *Files identical despite different names*

### Comparing `globus-automate-client-0.6/globus_automate_client/queues_client.py` & `globus-automate-client-0.7.0/globus_automate_client/queues_client.py`

 * *Files identical despite different names*

### Comparing `globus-automate-client-0.6/globus_automate_client/token_management.py` & `globus-automate-client-0.7.0/globus_automate_client/token_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from time import time
-from globus_sdk import NativeAppAuthClient
 import json
 from os import path
+from time import time
 from typing import Any, Dict, List, Optional, Tuple
 
+from globus_sdk import NativeAppAuthClient
 
 # python2/3 safe simple input reading
 get_input = getattr(__builtins__, "raw_input", input)
 
 _token_cache_filename = path.join(path.expanduser("~"), ".globus_token_cache")
 
 
@@ -29,15 +29,15 @@
             cache = json.load(f)
             return cache
     except FileNotFoundError:
         return {}
 
 
 def get_cached_tokens(
-    scopes: List[str]
+    scopes: List[str],
 ) -> Dict[str, Tuple[Optional[str], Optional[str]]]:
     token_cache = _load_cache()
     access_token = None
     refresh_token = None
     ret_tokens: Dict[str, Tuple[Optional[str], Optional[str]]] = {}
     for scope in scopes:
         if scope in token_cache:
```

