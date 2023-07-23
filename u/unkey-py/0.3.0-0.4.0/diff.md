# Comparing `tmp/unkey_py-0.3.0.tar.gz` & `tmp/unkey_py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unkey_py-0.3.0.tar", max compression
+gzip compressed data, was "unkey_py-0.4.0.tar", max compression
```

## Comparing `unkey_py-0.3.0.tar` & `unkey_py-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-07-16 16:38:10.043501 unkey_py-0.3.0/LICENSE
--rw-r--r--   0        0        0     1851 2023-07-16 16:38:10.043501 unkey_py-0.3.0/README.md
--rw-r--r--   0        0        0     2311 2023-07-16 16:38:10.043501 unkey_py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1416 2023-07-16 16:38:10.155500 unkey_py-0.3.0/unkey/__init__.py
--rw-r--r--   0        0        0      643 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/__main__.py
--rw-r--r--   0        0        0     2492 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/client.py
--rw-r--r--   0        0        0      332 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/constants.py
--rw-r--r--   0        0        0      436 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/errors.py
--rw-r--r--   0        0        0      291 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/__init__.py
--rw-r--r--   0        0        0      729 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/apis.py
--rw-r--r--   0        0        0     1615 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/base.py
--rw-r--r--   0        0        0      840 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/http.py
--rw-r--r--   0        0        0     2897 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/models/keys.py
--rw-r--r--   0        0        0        0 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/py.typed
--rw-r--r--   0        0        0     2230 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/result.py
--rw-r--r--   0        0        0     2089 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/routes.py
--rw-r--r--   0        0        0     3581 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/serializer.py
--rw-r--r--   0        0        0      151 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/__init__.py
--rw-r--r--   0        0        0     2353 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/apis.py
--rw-r--r--   0        0        0     1229 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/base.py
--rw-r--r--   0        0        0     4388 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/http.py
--rw-r--r--   0        0        0     3970 2023-07-16 16:38:10.047501 unkey_py-0.3.0/unkey/services/keys.py
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 unkey_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-23 21:57:29.160836 unkey_py-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1851 2023-07-23 21:57:29.160836 unkey_py-0.4.0/README.md
+-rw-r--r--   0        0        0     2311 2023-07-23 21:57:29.160836 unkey_py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1572 2023-07-23 21:57:29.256838 unkey_py-0.4.0/unkey/__init__.py
+-rw-r--r--   0        0        0      643 2023-07-23 21:57:29.160836 unkey_py-0.4.0/unkey/__main__.py
+-rw-r--r--   0        0        0     2492 2023-07-23 21:57:29.160836 unkey_py-0.4.0/unkey/client.py
+-rw-r--r--   0        0        0      332 2023-07-23 21:57:29.160836 unkey_py-0.4.0/unkey/constants.py
+-rw-r--r--   0        0        0      656 2023-07-23 21:57:29.160836 unkey_py-0.4.0/unkey/errors.py
+-rw-r--r--   0        0        0      291 2023-07-23 21:57:29.160836 unkey_py-0.4.0/unkey/models/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-23 21:57:29.160836 unkey_py-0.4.0/unkey/models/apis.py
+-rw-r--r--   0        0        0     1615 2023-07-23 21:57:29.160836 unkey_py-0.4.0/unkey/models/base.py
+-rw-r--r--   0        0        0      840 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/models/http.py
+-rw-r--r--   0        0        0     2897 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/models/keys.py
+-rw-r--r--   0        0        0        0 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/py.typed
+-rw-r--r--   0        0        0     2230 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/result.py
+-rw-r--r--   0        0        0     2143 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/routes.py
+-rw-r--r--   0        0        0     3581 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/serializer.py
+-rw-r--r--   0        0        0      151 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/services/__init__.py
+-rw-r--r--   0        0        0     2448 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/services/apis.py
+-rw-r--r--   0        0        0     1304 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/services/base.py
+-rw-r--r--   0        0        0     4388 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/services/http.py
+-rw-r--r--   0        0        0     6408 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/services/keys.py
+-rw-r--r--   0        0        0     1029 2023-07-23 21:57:29.164837 unkey_py-0.4.0/unkey/undefined.py
+-rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 unkey_py-0.4.0/PKG-INFO
```

### Comparing `unkey_py-0.3.0/LICENSE` & `unkey_py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/README.md` & `unkey_py-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/pyproject.toml` & `unkey_py-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unkey.py"
-version = "0.3.0"
+version = "0.4.0"
 description = "An asynchronous Python SDK for unkey.dev."
 authors = ["Jonxslays"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/unkey.py"
 repository = "https://github.com/Jonxslays/unkey.py"
 packages = [
```

### Comparing `unkey_py-0.3.0/unkey/__init__.py` & `unkey_py-0.4.0/unkey/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 from __future__ import annotations
 
 from typing import Final
 
 __packagename__: Final[str] = "unkey.py"
-__version__: Final[str] = "0.3.0"
+__version__: Final[str] = "0.4.0"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous Python SDK for unkey.dev."
 __url__: Final[str] = "https://github.com/Jonxslays/unkey.py"
 __docs__: Final[str] = "https://jonxslays.github.io/unkey.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "GPL-3.0"
-__git_sha__: Final[str] = "[3c333fd]"
+__git_sha__: Final[str] = "[c6002d9]"
 
 from . import client
 from . import constants
 from . import errors
 from . import models
 from . import result
 from . import routes
 from . import serializer
 from . import services
+from . import undefined
 from .client import *
 from .errors import *
 from .models import *
 from .result import *
 from .routes import *
 from .serializer import *
 from .services import *
+from .undefined import *
 
 __all__ = (
     "client",
     "constants",
     "errors",
     "models",
     "result",
     "routes",
     "serializer",
     "services",
+    "undefined",
     "Api",
     "ApiKey",
     "ApiKeyList",
     "ApiKeyMeta",
     "ApiKeyVerification",
     "ApiService",
     "BaseEnum",
@@ -51,15 +54,19 @@
     "Client",
     "CompiledRoute",
     "Err",
     "ErrorCode",
     "HttpResponse",
     "HttpService",
     "KeyService",
+    "MissingRequiredArgument",
     "Ok",
     "Ratelimit",
     "RatelimitType",
     "Result",
     "Route",
     "Serializer",
+    "UndefinedNoneOr",
+    "UndefinedOr",
     "UnwrapError",
+    "UNDEFINED",
 )
```

### Comparing `unkey_py-0.3.0/unkey/__main__.py` & `unkey_py-0.4.0/unkey/__main__.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/unkey/client.py` & `unkey_py-0.4.0/unkey/client.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/unkey/models/apis.py` & `unkey_py-0.4.0/unkey/models/apis.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/unkey/models/base.py` & `unkey_py-0.4.0/unkey/models/base.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/unkey/models/http.py` & `unkey_py-0.4.0/unkey/models/http.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/unkey/models/keys.py` & `unkey_py-0.4.0/unkey/models/keys.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/unkey/result.py` & `unkey_py-0.4.0/unkey/result.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/unkey/routes.py` & `unkey_py-0.4.0/unkey/routes.py`

 * *Files 14% similar despite different names*

```diff
@@ -79,11 +79,12 @@
         return compiled
 
 
 # Keys
 CREATE_KEY: t.Final[Route] = Route(c.POST, "/keys")
 VERIFY_KEY: t.Final[Route] = Route(c.POST, "/keys/verify")
 REVOKE_KEY: t.Final[Route] = Route(c.DELETE, "/keys/{}")
+UPDATE_KEY: t.Final[Route] = Route(c.PUT, "/keys/{}")
 
 # Apis
 GET_API: t.Final[Route] = Route(c.GET, "/apis/{}")
 GET_KEYS: t.Final[Route] = Route(c.GET, "/apis/{}/keys")
```

### Comparing `unkey_py-0.3.0/unkey/serializer.py` & `unkey_py-0.4.0/unkey/serializer.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/unkey/services/apis.py` & `unkey_py-0.4.0/unkey/services/apis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import typing as t
 
 from unkey import models
 from unkey import result
 from unkey import routes
+from unkey import undefined
 
 from . import BaseService
 
 __all__ = ("ApiService",)
 
 T = t.TypeVar("T")
 ResultT = result.Result[T, models.HttpResponse]
@@ -42,15 +43,20 @@
                     models.ErrorCode.from_str_maybe(data.get("code", "unknown")),
                 )
             )
 
         return result.Ok(self._serializer.to_api(data))
 
     async def list_keys(
-        self, api_id: str, *, owner_id: t.Optional[str] = None, limit: int = 100, offset: int = 0
+        self,
+        api_id: str,
+        *,
+        owner_id: undefined.UndefinedOr[str] = undefined.UNDEFINED,
+        limit: int = 100,
+        offset: int = 0,
     ) -> ResultT[models.ApiKeyList]:
         """Gets a paginated list of keys for the given api.
 
         Args:
             api_id: The id of the api.
 
         Keyword Args:
```

### Comparing `unkey_py-0.3.0/unkey/services/http.py` & `unkey_py-0.4.0/unkey/services/http.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.3.0/PKG-INFO` & `unkey_py-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unkey-py
-Version: 0.3.0
+Version: 0.4.0
 Summary: An asynchronous Python SDK for unkey.dev.
 Home-page: https://github.com/Jonxslays/unkey.py
 License: GPL-3.0-only
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

