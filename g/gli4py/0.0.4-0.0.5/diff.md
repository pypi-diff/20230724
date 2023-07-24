# Comparing `tmp/gli4py-0.0.4.tar.gz` & `tmp/gli4py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gli4py-0.0.4.tar", max compression
+gzip compressed data, was "gli4py-0.0.5.tar", max compression
```

## Comparing `gli4py-0.0.4.tar` & `gli4py-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0    35823 2023-07-24 11:22:10.017150 gli4py-0.0.4/LICENSE
--rwxr-xr-x   0        0        0     1435 2023-07-24 11:24:15.317553 gli4py-0.0.4/README.md
--rwxr-xr-x   0        0        0      103 2023-07-24 11:24:13.483975 gli4py-0.0.4/gli4py/__init__.py
--rwxr-xr-x   0        0        0      289 2023-07-24 11:22:10.044154 gli4py-0.0.4/gli4py/error_codes.json
--rwxr-xr-x   0        0        0     1915 2023-07-24 14:30:52.939794 gli4py-0.0.4/gli4py/error_handling.py
--rwxr-xr-x   0        0        0     7738 2023-07-24 17:59:03.447636 gli4py-0.0.4/gli4py/glinet.py
--rwxr-xr-x   0        0        0      657 2023-07-24 18:01:29.706729 gli4py-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 gli4py-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0    35823 2023-07-24 11:22:10.017150 gli4py-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0     1435 2023-07-24 11:24:15.317553 gli4py-0.0.5/README.md
+-rwxr-xr-x   0        0        0      103 2023-07-24 11:24:13.483975 gli4py-0.0.5/gli4py/__init__.py
+-rwxr-xr-x   0        0        0      289 2023-07-24 11:22:10.044154 gli4py-0.0.5/gli4py/error_codes.json
+-rwxr-xr-x   0        0        0     1915 2023-07-24 14:30:52.939794 gli4py-0.0.5/gli4py/error_handling.py
+-rwxr-xr-x   0        0        0     7692 2023-07-24 19:29:49.237337 gli4py-0.0.5/gli4py/glinet.py
+-rwxr-xr-x   0        0        0      657 2023-07-24 19:29:53.060397 gli4py-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 gli4py-0.0.5/PKG-INFO
```

### Comparing `gli4py-0.0.4/LICENSE` & `gli4py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gli4py-0.0.4/README.md` & `gli4py-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gli4py-0.0.4/gli4py/error_handling.py` & `gli4py-0.0.5/gli4py/error_handling.py`

 * *Files identical despite different names*

### Comparing `gli4py-0.0.4/gli4py/glinet.py` & `gli4py-0.0.5/gli4py/glinet.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             }
             )
         return await self._request(login_data)
     
     async def router_reachable(self, username:str = 'root') -> bool:
         try:
             res = await self._challenge(username)
+            print(res)
             if res:
                 return True
         except:
             return False
         return False
 
     async def login(self, username: str, password: str) -> None:
@@ -198,14 +199,14 @@
         status 0:not start 1:connected 2:connecting
         """
         return await self._request(self.gen_sid_payload('call', ['wg-client', 'get_status'], self.sid))
 
     async def wireguard_client_start(self, group_id: int, peer_id: int) -> dict:
         return await self._request(self.gen_sid_payload('call', ['wg-client', 'start', {"group_id":group_id,"peer_id":peer_id}], self.sid))
 
-    async def wireguard_client_stop(self, group_id: int, peer_id: int) -> dict:
-        return await self._request(self.gen_sid_payload('call', ['wg-client', 'stop', {"group_id":group_id,"peer_id":peer_id}], self.sid))
+    async def wireguard_client_stop(self) -> dict:
+        return await self._request(self.gen_sid_payload('call', ['wg-client', 'stop'], self.sid))
 
     @property
     def logged_in(self) -> bool:
         return self._logged_in
```

### Comparing `gli4py-0.0.4/pyproject.toml` & `gli4py-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gli4py"
-version = "0.0.4"
+version = "0.0.5"
 description = "A python 3 API wrapper for GL-inet routers for consumption by Home Assistant"
 authors = ["HarvsG <doctor@codingdoctor.co.uk>"]
 license = "GNU GENERAL PUBLIC LICENSE"
 readme = "README.md"
 packages = [{include = "gli4py"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gli4py-0.0.4/PKG-INFO` & `gli4py-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gli4py
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python 3 API wrapper for GL-inet routers for consumption by Home Assistant
 License: GNU GENERAL PUBLIC LICENSE
 Author: HarvsG
 Author-email: doctor@codingdoctor.co.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

