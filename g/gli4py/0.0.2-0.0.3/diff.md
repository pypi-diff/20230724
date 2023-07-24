# Comparing `tmp/gli4py-0.0.2.tar.gz` & `tmp/gli4py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gli4py-0.0.2.tar", max compression
+gzip compressed data, was "gli4py-0.0.3.tar", max compression
```

## Comparing `gli4py-0.0.2.tar` & `gli4py-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0    35823 2023-07-24 11:22:10.017150 gli4py-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     1435 2023-07-24 11:24:15.317553 gli4py-0.0.2/README.md
--rwxr-xr-x   0        0        0      103 2023-07-24 11:24:13.483975 gli4py-0.0.2/gli4py/__init__.py
--rwxr-xr-x   0        0        0      289 2023-07-24 11:22:10.044154 gli4py-0.0.2/gli4py/error_codes.json
--rwxr-xr-x   0        0        0     1915 2023-07-24 14:30:52.939794 gli4py-0.0.2/gli4py/error_handling.py
--rwxr-xr-x   0        0        0     7597 2023-07-24 16:19:56.069991 gli4py-0.0.2/gli4py/glinet.py
--rwxr-xr-x   0        0        0      657 2023-07-24 16:20:41.747562 gli4py-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 gli4py-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0    35823 2023-07-24 11:22:10.017150 gli4py-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     1435 2023-07-24 11:24:15.317553 gli4py-0.0.3/README.md
+-rwxr-xr-x   0        0        0      103 2023-07-24 11:24:13.483975 gli4py-0.0.3/gli4py/__init__.py
+-rwxr-xr-x   0        0        0      289 2023-07-24 11:22:10.044154 gli4py-0.0.3/gli4py/error_codes.json
+-rwxr-xr-x   0        0        0     1915 2023-07-24 14:30:52.939794 gli4py-0.0.3/gli4py/error_handling.py
+-rwxr-xr-x   0        0        0     7606 2023-07-24 16:23:12.620105 gli4py-0.0.3/gli4py/glinet.py
+-rwxr-xr-x   0        0        0      657 2023-07-24 16:23:22.699290 gli4py-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 gli4py-0.0.3/PKG-INFO
```

### Comparing `gli4py-0.0.2/LICENSE` & `gli4py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gli4py-0.0.2/README.md` & `gli4py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gli4py-0.0.2/gli4py/error_handling.py` & `gli4py-0.0.3/gli4py/error_handling.py`

 * *Files identical despite different names*

### Comparing `gli4py-0.0.2/gli4py/glinet.py` & `gli4py-0.0.3/gli4py/glinet.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             {
                 'username': username,
                 'hash': hash
             }
             )
         return await self._request(login_data)
     
-    async def router_reachable(self, username:str) -> bool:
+    async def router_reachable(self, username:str = 'root') -> bool:
         try:
             res = await self._challenge(username)
             if res:
                 return True
         except:
             return False
         return False
```

### Comparing `gli4py-0.0.2/pyproject.toml` & `gli4py-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gli4py"
-version = "0.0.2"
+version = "0.0.3"
 description = "A python 3 API wrapper for GL-inet routers for consumption by Home Assistant"
 authors = ["HarvsG <doctor@codingdoctor.co.uk>"]
 license = "GNU GENERAL PUBLIC LICENSE"
 readme = "README.md"
 packages = [{include = "gli4py"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gli4py-0.0.2/PKG-INFO` & `gli4py-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gli4py
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python 3 API wrapper for GL-inet routers for consumption by Home Assistant
 License: GNU GENERAL PUBLIC LICENSE
 Author: HarvsG
 Author-email: doctor@codingdoctor.co.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

