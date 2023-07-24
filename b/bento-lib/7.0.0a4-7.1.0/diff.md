# Comparing `tmp/bento_lib-7.0.0a4.tar.gz` & `tmp/bento_lib-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-7.0.0a4.tar", last modified: Thu Jun 15 18:42:59 2023, max compression
+gzip compressed data, was "bento_lib-7.1.0.tar", last modified: Mon Jul 24 20:34:43 2023, max compression
```

## Comparing `bento_lib-7.0.0a4.tar` & `bento_lib-7.1.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.055838 bento_lib-7.0.0a4/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.055838 bento_lib-7.0.0a4/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.059838 bento_lib-7.0.0a4/bento_lib/auth/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.059838 bento_lib-7.0.0a4/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.059838 bento_lib-7.0.0a4/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.059838 bento_lib-7.0.0a4/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/responses/fastapi_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/responses/flask_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/bento_ingest.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.055838 bento_lib-7.0.0a4/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.293377 bento_lib-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-24 20:34:33.000000 bento_lib-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 20:34:33.000000 bento_lib-7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-24 20:34:43.293377 bento_lib-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-24 20:34:33.000000 bento_lib-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/auth/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.293377 bento_lib-7.1.0/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/responses/fastapi_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/responses/flask_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.293377 bento_lib-7.1.0/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/bento_ingest.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.293377 bento_lib-7.1.0/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:34:43.293377 bento_lib-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 20:34:33.000000 bento_lib-7.1.0/setup.py
```

### Comparing `bento_lib-7.0.0a4/LICENSE` & `bento_lib-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/PKG-INFO` & `bento_lib-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento_lib
-Version: 7.0.0a4
+Version: 7.1.0
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.0.0a4/README.md` & `bento_lib-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/auth/middleware/base.py` & `bento_lib-7.1.0/bento_lib/auth/middleware/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         enabled: bool = True,
         logger: logging.Logger | None = None,
     ):
         self._debug: bool = debug_mode
         self._verify_ssl: bool = not debug_mode
 
         self._enabled: bool = enabled
-        self._logger = logger or logging.getLogger(__name__)
+        self._logger: logging.Logger | None = logger
 
         self._drs_compat: bool = drs_compat
         self._sr_compat: bool = sr_compat
 
         self._bento_authz_service_url: str = bento_authz_service_url
 
     @property
@@ -57,16 +57,20 @@
         if headers_getter:
             return headers_getter(request)
 
         tkn_header = self.get_authz_header_value(request)
         self.check_require_token(require_token, tkn_header)
         return {"Authorization": tkn_header} if tkn_header else {}
 
+    def _log_error(self, message: str):
+        if self._logger:
+            self._logger.error(message)
+
     def _gen_exc_non_200_error_from_authz(self, code: int, content: bytes):
-        self._logger.error(f"Got non-200 response from authorization service: {code} {content}")
+        self._log_error(f"Got non-200 response from authorization service: {code} {content}")
         # Generic error - don't leak errors from authz service!
         raise BentoAuthException("Error from authz service", status_code=500)
 
     def authz_post(
         self,
         request: Any,
         path: str,
```

### Comparing `bento_lib-7.0.0a4/bento_lib/auth/middleware/django.py` & `bento_lib-7.1.0/bento_lib/auth/middleware/django.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+import logging
+
 from asgiref.sync import iscoroutinefunction, markcoroutinefunction
 from django.http import JsonResponse, HttpRequest, HttpResponse
 from typing import Awaitable, Callable
 
 from bento_lib.responses.errors import http_error
 from bento_lib.auth.exceptions import BentoAuthException
 from bento_lib.auth.middleware.base import BaseAuthMiddleware
 
 __all__ = [
     "DjangoAuthMiddleware",
 ]
 
 
 class DjangoAuthMiddleware(BaseAuthMiddleware):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # If no logger was passed, create a new logger
+        if self._logger is None:
+            self._logger = logging.getLogger(__name__)
+
     def get_authz_header_value(self, request: HttpRequest) -> str | None:
         return request.headers.get("Authorization")
 
     @staticmethod
     def mark_authz_done(request: HttpRequest):
         request.bento_determined_authz = True
```

### Comparing `bento_lib-7.0.0a4/bento_lib/auth/middleware/fastapi.py` & `bento_lib-7.1.0/bento_lib/auth/middleware/fastapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from fastapi import Depends, FastAPI, Request, Response, status
 from fastapi.responses import JSONResponse
 from typing import Awaitable, Callable
 
 from bento_lib.responses.errors import http_error
 from bento_lib.auth.exceptions import BentoAuthException
 from bento_lib.auth.middleware.base import BaseAuthMiddleware
@@ -14,16 +16,22 @@
 
 class FastApiAuthMiddleware(BaseAuthMiddleware):
     def attach(self, app: FastAPI):
         """
         Attach the middleware to an application. Must be called in order for requests to be checked.
         :param app: A FastAPI application.
         """
+
+        # Attach our instance's dispatch method to the FastAPI instance as a middleware function
         app.middleware("http")(self.dispatch)
 
+        # If no logger was passed, create a new logger
+        if self._logger is None:
+            self._logger = logging.getLogger(__name__)
+
     async def dispatch(self, request: Request, call_next: Callable[[Request], Awaitable[Response]]) -> Response:
         if not self.enabled or request.method == "OPTIONS":
             # - Skip checks if the authorization middleware is disabled
             # - Allow pre-flight responses through
             return await call_next(request)
 
         # Set flag saying the request hasn't had its permissions determined yet.
```

### Comparing `bento_lib-7.0.0a4/bento_lib/auth/middleware/flask.py` & `bento_lib-7.1.0/bento_lib/auth/middleware/flask.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 
 class FlaskAuthMiddleware(BaseAuthMiddleware):
     def attach(self, app: Flask):
         """
         Attach the middleware to an application. Must be called in order for requests to be checked.
         :param app: A Flask application.
         """
+
         app.before_request(self.middleware_pre)
         app.after_request(self.middleware_post)
 
+        if self._logger is None:
+            self._logger = app.logger
+
     def middleware_pre(self) -> None:
         if self.enabled:
             g.bento_determined_authz = False
 
     def _make_auth_error(self, e: BentoAuthException) -> Response:
         # returning an error, so mark authz flow as 'done' (rejecting in one way or another):
         self.mark_authz_done(request)
```

### Comparing `bento_lib-7.0.0a4/bento_lib/drs/utils.py` & `bento_lib-7.1.0/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/events/_event_bus.py` & `bento_lib-7.1.0/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/events/notifications.py` & `bento_lib-7.1.0/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/events/types.py` & `bento_lib-7.1.0/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/responses/errors.py` & `bento_lib-7.1.0/bento_lib/responses/errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/responses/fastapi_errors.py` & `bento_lib-7.1.0/bento_lib/responses/fastapi_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/responses/flask_errors.py` & `bento_lib-7.1.0/bento_lib/responses/flask_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-7.1.0/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/schemas/bento_ingest.schema.json` & `bento_lib-7.1.0/bento_lib/schemas/bento_ingest.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-7.1.0/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/search/data_structure.py` & `bento_lib-7.1.0/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/search/operations.py` & `bento_lib-7.1.0/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/search/postgres.py` & `bento_lib-7.1.0/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/search/queries.py` & `bento_lib-7.1.0/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/types.py` & `bento_lib-7.1.0/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib/workflows.py` & `bento_lib-7.1.0/bento_lib/workflows.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/bento_lib.egg-info/PKG-INFO` & `bento_lib-7.1.0/bento_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-lib
-Version: 7.0.0a4
+Version: 7.1.0
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.0.0a4/bento_lib.egg-info/SOURCES.txt` & `bento_lib-7.1.0/bento_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a4/setup.py` & `bento_lib-7.1.0/setup.py`

 * *Files identical despite different names*

