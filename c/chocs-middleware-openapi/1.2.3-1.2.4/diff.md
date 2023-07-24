# Comparing `tmp/chocs_middleware_openapi-1.2.3.tar.gz` & `tmp/chocs_middleware_openapi-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chocs_middleware_openapi-1.2.3.tar", max compression
+gzip compressed data, was "chocs_middleware_openapi-1.2.4.tar", max compression
```

## Comparing `chocs_middleware_openapi-1.2.3.tar` & `chocs_middleware_openapi-1.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/LICENSE
--rw-r--r--   0        0        0     4812 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/README.md
--rw-r--r--   0        0        0       42 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/__init__.py
--rw-r--r--   0        0        0     1108 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/error.py
--rw-r--r--   0        0        0     4407 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/middleware.py
--rw-r--r--   0        0        0     3923 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/validators.py
--rw-r--r--   0        0        0     1212 2023-07-19 13:59:31.539034 chocs_middleware_openapi-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 chocs_middleware_openapi-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-24 13:47:52.685497 chocs_middleware_openapi-1.2.4/LICENSE
+-rw-r--r--   0        0        0     4812 2023-07-24 13:47:52.685497 chocs_middleware_openapi-1.2.4/README.md
+-rw-r--r--   0        0        0       42 2023-07-24 13:47:52.685497 chocs_middleware_openapi-1.2.4/chocs_middleware/openapi/__init__.py
+-rw-r--r--   0        0        0     1108 2023-07-24 13:47:52.685497 chocs_middleware_openapi-1.2.4/chocs_middleware/openapi/error.py
+-rw-r--r--   0        0        0     4407 2023-07-24 13:47:52.685497 chocs_middleware_openapi-1.2.4/chocs_middleware/openapi/middleware.py
+-rw-r--r--   0        0        0     3923 2023-07-24 13:47:52.685497 chocs_middleware_openapi-1.2.4/chocs_middleware/openapi/validators.py
+-rw-r--r--   0        0        0     1212 2023-07-24 13:47:52.685497 chocs_middleware_openapi-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 chocs_middleware_openapi-1.2.4/PKG-INFO
```

### Comparing `chocs_middleware_openapi-1.2.3/LICENSE` & `chocs_middleware_openapi-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.3/README.md` & `chocs_middleware_openapi-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/error.py` & `chocs_middleware_openapi-1.2.4/chocs_middleware/openapi/error.py`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/middleware.py` & `chocs_middleware_openapi-1.2.4/chocs_middleware/openapi/middleware.py`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.3/chocs_middleware/openapi/validators.py` & `chocs_middleware_openapi-1.2.4/chocs_middleware/openapi/validators.py`

 * *Files identical despite different names*

### Comparing `chocs_middleware_openapi-1.2.3/pyproject.toml` & `chocs_middleware_openapi-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chocs_middleware.openapi"
-version = "1.2.3"
+version = "1.2.4"
 description = "Middleware to validate incoming requests with openapi spec."
 authors = [
     "Dawid Kraczkowski <dawid.kraczkowski@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 packages = [
```

### Comparing `chocs_middleware_openapi-1.2.3/PKG-INFO` & `chocs_middleware_openapi-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chocs-middleware-openapi
-Version: 1.2.3
+Version: 1.2.4
 Summary: Middleware to validate incoming requests with openapi spec.
 Home-page: https://github.com/kodemore/chocs-openapi
 License: MIT
 Keywords: openapi,json-schema,chocs,http,middleware
 Author: Dawid Kraczkowski
 Author-email: dawid.kraczkowski@gmail.com
 Requires-Python: >=3.8,<4.0
```

