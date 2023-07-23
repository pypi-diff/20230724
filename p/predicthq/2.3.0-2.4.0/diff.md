# Comparing `tmp/predicthq-2.3.0.tar.gz` & `tmp/predicthq-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predicthq-2.3.0.tar", last modified: Thu Apr 27 21:15:33 2023, max compression
+gzip compressed data, was "predicthq-2.4.0.tar", last modified: Sun Jul 23 22:24:34 2023, max compression
```

## Comparing `predicthq-2.3.0.tar` & `predicthq-2.4.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 21:15:23.000000 predicthq-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-27 21:15:23.000000 predicthq-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-04-27 21:15:33.252367 predicthq-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-04-27 21:15:23.000000 predicthq-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/oauth2/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/oauth2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/accounts/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/accounts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/events/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/events/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/events/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/features/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/features/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/features/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/places/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/places/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/places/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/places/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/radius/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/radius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/radius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/radius/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 21:15:33.256367 predicthq-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-27 21:15:23.000000 predicthq-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-27 21:15:23.000000 predicthq-2.3.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-27 21:15:23.000000 predicthq-2.3.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.477751 predicthq-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-23 22:24:26.000000 predicthq-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-23 22:24:26.000000 predicthq-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-23 22:24:34.477751 predicthq-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-23 22:24:26.000000 predicthq-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.465751 predicthq-2.4.0/predicthq/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.469751 predicthq-2.4.0/predicthq/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.469751 predicthq-2.4.0/predicthq/endpoints/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/oauth2/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/oauth2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.469751 predicthq-2.4.0/predicthq/endpoints/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.473751 predicthq-2.4.0/predicthq/endpoints/v1/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/accounts/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/accounts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.473751 predicthq-2.4.0/predicthq/endpoints/v1/broadcasts/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/broadcasts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/broadcasts/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/broadcasts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.473751 predicthq-2.4.0/predicthq/endpoints/v1/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/events/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/events/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.473751 predicthq-2.4.0/predicthq/endpoints/v1/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/features/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/features/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.477751 predicthq-2.4.0/predicthq/endpoints/v1/places/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/places/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/places/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/places/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.477751 predicthq-2.4.0/predicthq/endpoints/v1/radius/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/radius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/radius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/endpoints/v1/radius/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-23 22:24:26.000000 predicthq-2.4.0/predicthq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.469751 predicthq-2.4.0/predicthq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-23 22:24:34.000000 predicthq-2.4.0/predicthq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-23 22:24:34.000000 predicthq-2.4.0/predicthq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:24:34.000000 predicthq-2.4.0/predicthq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-23 22:24:34.000000 predicthq-2.4.0/predicthq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-23 22:24:34.000000 predicthq-2.4.0/predicthq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-23 22:24:34.477751 predicthq-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-23 22:24:26.000000 predicthq-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:24:34.477751 predicthq-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-23 22:24:26.000000 predicthq-2.4.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-23 22:24:26.000000 predicthq-2.4.0/tests/test_config.py
```

### Comparing `predicthq-2.3.0/LICENSE` & `predicthq-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/PKG-INFO` & `predicthq-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predicthq
-Version: 2.3.0
+Version: 2.4.0
 Summary: PredictHQ Event Intelligence
 Home-page: https://github.com/predicthq/sdk-py
 Author: PredictHQ
 Author-email: developers@predicthq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `predicthq-2.3.0/README.md` & `predicthq-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/client.py` & `predicthq-2.4.0/predicthq/client.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/config.py` & `predicthq-2.4.0/predicthq/config.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/base.py` & `predicthq-2.4.0/predicthq/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/decorators.py` & `predicthq-2.4.0/predicthq/endpoints/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,24 +12,33 @@
     params = {}
     for key, value in data.items():
         if isinstance(value, bool):
             params[key] = 1 if value else 0
         elif isinstance(value, list):
             params[key] = separator.join(map(str, value))
         elif isinstance(value, dict):
-            for subkey, subvalue in value.items():
-                if isinstance(subvalue, list):
-                    params[glue.join((key, subkey))] = separator.join(map(str, subvalue))
-                else:
-                    params[glue.join((key, subkey))] = subvalue
+            params.update(_flatten_dict(value, glue, separator, parent_key=key))
         else:
             params[key] = value
     return params
 
 
+def _flatten_dict(d, glue, separator, parent_key=""):
+    flat_dict = {}
+    for k, v in d.items():
+        if isinstance(v, dict):
+            flat_dict.update(_flatten_dict(v, glue, separator, f"{parent_key}{glue}{k}" if parent_key else k))
+            continue
+        if isinstance(v, list):
+            flat_dict.update({f"{parent_key}{glue}{k}" if parent_key else k: separator.join(map(str, v))})
+            continue
+        flat_dict.update({f"{parent_key}{glue}{k}" if parent_key else k: v})
+    return flat_dict
+
+
 def _process_kwargs(kwargs, separator="__"):
     data = defaultdict(dict)
     for key, value in kwargs.items():
         if separator in key:
             k, subk = key.split(separator)
             data[k][subk] = value
         else:
```

### Comparing `predicthq-2.3.0/predicthq/endpoints/oauth2/endpoint.py` & `predicthq-2.4.0/predicthq/endpoints/oauth2/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/oauth2/schemas.py` & `predicthq-2.4.0/predicthq/endpoints/oauth2/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/schemas.py` & `predicthq-2.4.0/predicthq/endpoints/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 
     import_format = r"@(?P<latitude>-?\d+(\.\d+)?),(?P<longitude>-?\d+(\.\d+)?)"
     export_format = "@{latitude},{longitude}"
 
     latitude = FloatType(required=True)
     longitude = FloatType(required=True)
 
+
 # see https://github.com/predicthq/sdk-py/pull/84#discussion_r1163399743
 # ParentType requires either the value to be a boolean value or an enum value
 # therefore, we need to create a custom type that allows both
 class BooleanOrEnumType(BooleanType):
     def __init__(self, *args, **kwargs):
         self.enum_values = kwargs.pop("choices")
         super().__init__(*args, **kwargs)
@@ -244,14 +245,23 @@
 class Entity(Model):
     class Options:
         serialize_when_none = False
 
     id = StringType()
 
 
+class PredictedEventSpendIndustry(Model):
+    class Options:
+        serialize_when_none = False
+
+    accommodation = ModelType(IntRange)
+    hospitality = ModelType(IntRange)
+    transportation = ModelType(IntRange)
+
+
 class LimitMixin(Model):
 
     limit = IntType(min_value=1)
 
 
 class OffsetMixin(Model):
```

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/endpoint.py` & `predicthq-2.4.0/predicthq/endpoints/v1/broadcasts/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/schemas.py` & `predicthq-2.4.0/predicthq/endpoints/v1/broadcasts/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/events/endpoint.py` & `predicthq-2.4.0/predicthq/endpoints/v1/events/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/events/schemas.py` & `predicthq-2.4.0/predicthq/endpoints/v1/events/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     PolyModelType,
     ResultSet,
     ResultType,
     SortableMixin,
     StringListType,
     StringModelType,
     StringType,
+    PredictedEventSpendIndustry,
 )
 from schematics.common import NONEMPTY
 
 
 class SearchParams(PaginatedMixin, SortableMixin, ConfigMixin, Model):
     class Options:
         serialize_when_none = False
@@ -66,14 +67,16 @@
     entity = ModelType(Entity)
     local_rank = ModelType(IntRange)
     local_rank_level = ListType(IntType(min_value=1, max_value=5))
     phq_attendance = ModelType(IntRange)
     predicted_end = ModelType(DateTimeRange)
     rank = ModelType(IntRange)
     rank_level = ListType(IntType(min_value=1, max_value=5))
+    predicted_event_spend = ModelType(IntRange)
+    predicted_event_spend_industry = ModelType(PredictedEventSpendIndustry)
 
 
 class Entities(Model):
     class Options:
         serialize_when_none = True
 
     entity_id = StringType()
@@ -124,14 +127,20 @@
 
 class Geo(Model):
 
     geometry = PolyModelType(model_spec=[Point, MultiPoint, Polygon, MultiPolygon])
     placekey = StringType()
 
 
+class PredictedEventSpendIndustries(Model):
+    accommodation = IntType()
+    hospitality = IntType()
+    transportation = IntType()
+
+
 class ParentEvent(Model):
 
     parent_event_id = StringType()
 
 
 class ImpactPatternImpacts(Model):
 
@@ -181,14 +190,16 @@
     brand_safe = BooleanType()
     entities = ListType(ModelType(Entities))  # Venues and addresses add-on
     local_rank = IntType()  # Local Rank add-on
     phq_attendance = IntType()  # PHQ Attendance add-on
     predicted_end = DateTimeType()
     private = BooleanType()  # Loop add-on
     rank = IntType()  # PHQ Rank add-on
+    predicted_event_spend = IntType()  # Predicted Event Spend add-on
+    predicted_event_spend_industries = ModelType(PredictedEventSpendIndustries)
 
 
 class EventResultSet(ResultSet):
 
     overflow = BooleanType()
 
     results = ResultType(Event)
```

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/features/endpoint.py` & `predicthq-2.4.0/predicthq/endpoints/v1/features/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/features/schemas.py` & `predicthq-2.4.0/predicthq/endpoints/v1/features/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/places/schemas.py` & `predicthq-2.4.0/predicthq/endpoints/v1/places/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/radius/endpoint.py` & `predicthq-2.4.0/predicthq/endpoints/v1/radius/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq/endpoints/v1/radius/schemas.py` & `predicthq-2.4.0/predicthq/endpoints/v1/radius/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/predicthq.egg-info/PKG-INFO` & `predicthq-2.4.0/predicthq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predicthq
-Version: 2.3.0
+Version: 2.4.0
 Summary: PredictHQ Event Intelligence
 Home-page: https://github.com/predicthq/sdk-py
 Author: PredictHQ
 Author-email: developers@predicthq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `predicthq-2.3.0/predicthq.egg-info/SOURCES.txt` & `predicthq-2.4.0/predicthq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/setup.py` & `predicthq-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/tests/test_client.py` & `predicthq-2.4.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.3.0/tests/test_config.py` & `predicthq-2.4.0/tests/test_config.py`

 * *Files identical despite different names*

