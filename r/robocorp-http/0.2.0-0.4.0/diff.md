# Comparing `tmp/robocorp_http-0.2.0.tar.gz` & `tmp/robocorp_http-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_http-0.2.0.tar", max compression
+gzip compressed data, was "robocorp_http-0.4.0.tar", max compression
```

## Comparing `robocorp_http-0.2.0.tar` & `robocorp_http-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       24 2023-04-04 11:49:45.062599 robocorp_http-0.2.0/README.md
--rw-r--r--   0        0        0      545 2023-04-25 10:41:01.008843 robocorp_http-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-25 10:39:03.647640 robocorp_http-0.2.0/src/robocorp/http/__init__.py
--rw-r--r--   0        0        0     1339 2023-04-25 10:39:03.647870 robocorp_http-0.2.0/src/robocorp/http/_http.py
--rw-r--r--   0        0        0      598 2023-04-25 10:39:03.647969 robocorp_http-0.2.0/src/robocorp/http/_types.py
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 robocorp_http-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      633 2023-07-24 11:47:43.170943 robocorp_http-0.4.0/docs/README.md
+-rw-r--r--   0        0        0      763 2023-07-24 11:47:43.170943 robocorp_http-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-07-24 11:47:43.170943 robocorp_http-0.4.0/src/robocorp/http/__init__.py
+-rw-r--r--   0        0        0     2199 2023-07-24 11:47:43.170943 robocorp_http-0.4.0/src/robocorp/http/_http.py
+-rw-r--r--   0        0        0        0 2023-07-24 11:47:43.170943 robocorp_http-0.4.0/src/robocorp/http/py.typed
+-rw-r--r--   0        0        0     1268 1970-01-01 00:00:00.000000 robocorp_http-0.4.0/PKG-INFO
```

### Comparing `robocorp_http-0.2.0/pyproject.toml` & `robocorp_http-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 [tool.poetry]
 name = "robocorp-http"
-version = "0.2.0"
-description = "Robocorp HTTP automation library"
+version = "0.4.0"
+description = "Robocorp HTTP library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
-	"Kerkko P. <kerkko@robocorp.com>",
-    "Antero V. <antero@robocorp.com>",
+	"Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
+repository = "https://github.com/robocorp/robo/"
+license = "Apache-2.0"
 packages = [{include = "robocorp", from="src"}]
 
+[tool.black]
+skip-string-normalization = false
+skip-magic-trailing-comma = false
+
+[tool.isort]
+profile = "black"
+
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.28.2"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
-libs-devdeps = {path = ".."}
+robocorp-devutils = {path = "../devutils/", develop = true}
+types-requests = "^2.31.0.1"
+responses = "^0.23.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_http-0.2.0/src/robocorp/http/_http.py` & `robocorp_http-0.4.0/src/robocorp/http/_http.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,76 @@
+import re
 from pathlib import Path
-import requests
-from urllib.parse import urlparse
+from typing import Optional, Union
+from urllib.parse import unquote, urlparse
 
-from typing import Any, Optional
-from robocorp.http._types import PathType
+import requests
 
+PathLike = Union[str, Path]
 
-def _create_or_overwrite_target_file(
-    path: PathType,
-    response: Any,
-    overwrite: bool,
-) -> Path:
-    CHUNK_SIZE = 32768
-    path = Path(path)
-    path.parent.mkdir(parents=True, exist_ok=True)
-    file_exists = path.is_file()
-    if not file_exists or (file_exists and overwrite):
-        with open(path, "wb") as f:
-            for chunk in response.iter_content(CHUNK_SIZE):
-                if chunk:  # filter out keep-alive new chunks
-                    f.write(chunk)
-    return path
+CHUNK_SIZE = 32768
 
 
 def download(
     url: str,
-    target_file: Optional[PathType] = None,
+    path: Optional[PathLike] = None,
     overwrite: bool = False,
-    stream=True,
 ) -> Path:
-    dirname = Path()
-    filename = None
+    """Download a file from the given URL.
 
-    if target_file is not None:
-        target = Path(target_file)
-        if target.is_dir():
-            dirname = target
+    If the `path` argument is not given, the file is downloaded to the
+    current working directory. The filename is automatically selected
+    based on either the response headers or the URL.
+
+    Params:
+        url: URL to download
+        path: Path to destination file
+        overwrite: Overwrite file if it already exists
+
+    Returns:
+        Path to created file
+    """
+    if path is not None:
+        path = Path(path)
+        if path.is_dir():
+            dirname = path
+            filename = None
         else:
-            dirname = target.parent
-            filename = target.name
+            dirname = path.parent
+            filename = path.name
+    else:
+        dirname = Path.cwd()
+        filename = None
 
-    if filename is None:
-        filename = urlparse(url).path.rsplit("/", 1)[-1] or "downloaded.html"
-
-    with requests.get(url, stream=stream) as response:
+    with requests.get(url, stream=True) as response:
         response.raise_for_status()
-        path = _create_or_overwrite_target_file(dirname / filename, response, overwrite)
 
-    return path
+        # Try to resolve filename from response headers
+        if filename is None:
+            if content_disposition := response.headers.get("Content-Disposition"):
+                if match := re.search(r"filename=\"(.+)\"", content_disposition):
+                    filename = match.group(1)
+
+        # Try to parse filename from download URL
+        if filename is None:
+            parts = urlparse(url).path.split("/")
+            for part in reversed(parts):
+                part = unquote(part)
+                if part.strip():
+                    filename = part
+                    break
+
+        # Fallback value (unlikely)
+        if filename is None:
+            filename = "unknown"
+
+        output = dirname / filename
+        if output.exists() and not overwrite:
+            raise FileExistsError(f"File already exists: {output}")
+
+        dirname.mkdir(parents=True, exist_ok=True)
+        with open(output, "wb") as fd:
+            for chunk in response.iter_content(CHUNK_SIZE):
+                if chunk:  # Filter out keep-alive new chunks
+                    fd.write(chunk)
+
+        return output
```

