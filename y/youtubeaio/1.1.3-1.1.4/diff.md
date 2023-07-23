# Comparing `tmp/youtubeaio-1.1.3.tar.gz` & `tmp/youtubeaio-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubeaio-1.1.3.tar", max compression
+gzip compressed data, was "youtubeaio-1.1.4.tar", max compression
```

## Comparing `youtubeaio-1.1.3.tar` & `youtubeaio-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/LICENSE.md
--rw-r--r--   0        0        0     4864 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/README.md
--rw-r--r--   0        0        0     3873 2023-07-23 20:40:50.976369 youtubeaio-1.1.3/pyproject.toml
--rw-r--r--   0        0        0       57 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/src/youtubeaio/__init__.py
--rw-r--r--   0        0        0      831 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/src/youtubeaio/const.py
--rw-r--r--   0        0        0     3149 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/src/youtubeaio/helper.py
--rw-r--r--   0        0        0     7429 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/src/youtubeaio/models.py
--rw-r--r--   0        0        0     1772 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/src/youtubeaio/oauth.py
--rw-r--r--   0        0        0        0 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/src/youtubeaio/py.typed
--rw-r--r--   0        0        0     2139 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/src/youtubeaio/types.py
--rw-r--r--   0        0        0     9483 2023-07-23 20:40:32.208353 youtubeaio-1.1.3/src/youtubeaio/youtube.py
--rw-r--r--   0        0        0     6115 1970-01-01 00:00:00.000000 youtubeaio-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/LICENSE.md
+-rw-r--r--   0        0        0     4864 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/README.md
+-rw-r--r--   0        0        0     3873 2023-07-23 22:58:53.330885 youtubeaio-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/src/youtubeaio/__init__.py
+-rw-r--r--   0        0        0      831 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/src/youtubeaio/const.py
+-rw-r--r--   0        0        0     3149 2023-07-23 22:58:35.710301 youtubeaio-1.1.4/src/youtubeaio/helper.py
+-rw-r--r--   0        0        0     7429 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/models.py
+-rw-r--r--   0        0        0     1772 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/oauth.py
+-rw-r--r--   0        0        0        0 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/py.typed
+-rw-r--r--   0        0        0     2139 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/types.py
+-rw-r--r--   0        0        0     9711 2023-07-23 22:58:35.714301 youtubeaio-1.1.4/src/youtubeaio/youtube.py
+-rw-r--r--   0        0        0     6115 1970-01-01 00:00:00.000000 youtubeaio-1.1.4/PKG-INFO
```

### Comparing `youtubeaio-1.1.3/LICENSE.md` & `youtubeaio-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.3/README.md` & `youtubeaio-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.3/pyproject.toml` & `youtubeaio-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "youtubeaio"
-version = "1.1.3"
+version = "1.1.4"
 description = "Asynchronous Python client for YouTube V3 API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-youtube"
 repository = "https://github.com/joostlek/python-youtube"
```

### Comparing `youtubeaio-1.1.3/src/youtubeaio/const.py` & `youtubeaio-1.1.4/src/youtubeaio/const.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.3/src/youtubeaio/helper.py` & `youtubeaio-1.1.4/src/youtubeaio/helper.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.3/src/youtubeaio/models.py` & `youtubeaio-1.1.4/src/youtubeaio/models.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.3/src/youtubeaio/oauth.py` & `youtubeaio-1.1.4/src/youtubeaio/oauth.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.3/src/youtubeaio/types.py` & `youtubeaio-1.1.4/src/youtubeaio/types.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.1.3/src/youtubeaio/youtube.py` & `youtubeaio-1.1.4/src/youtubeaio/youtube.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     YouTubeChannel,
     YouTubePlaylistItem,
     YouTubeSubscription,
     YouTubeVideo,
 )
 from youtubeaio.types import (
     AuthScope,
+    ForbiddenError,
     MissingScopeError,
     UnauthorizedError,
     YouTubeAPIError,
     YouTubeBackendError,
     YouTubeResourceNotFoundError,
 )
 
@@ -82,14 +83,18 @@
             raise YouTubeAPIError(
                 "Bad Request" + ("" if msg is None else f" - {msg!s}"),
             )
         if response.status == 404:
             raise YouTubeResourceNotFoundError
         if response.status == 401:
             raise UnauthorizedError
+        if response.status == 403:
+            response_json = await response.json()
+            error_message = response_json["error"]["errors"][0]["message"]
+            raise ForbiddenError(error_message)
         if 400 <= response.status < 500:
             try:
                 response.raise_for_status()
             except ClientError as exc:
                 raise YouTubeAPIError from exc
         return response
```

### Comparing `youtubeaio-1.1.3/PKG-INFO` & `youtubeaio-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtubeaio
-Version: 1.1.3
+Version: 1.1.4
 Summary: Asynchronous Python client for YouTube V3 API.
 Home-page: https://github.com/joostlek/python-youtube
 License: MIT
 Keywords: youtube,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
```

