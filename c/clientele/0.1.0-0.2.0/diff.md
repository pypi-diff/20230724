# Comparing `tmp/clientele-0.1.0.tar.gz` & `tmp/clientele-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clientele-0.1.0.tar", max compression
+gzip compressed data, was "clientele-0.2.0.tar", max compression
```

## Comparing `clientele-0.1.0.tar` & `clientele-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0     1120 2023-07-24 01:44:09.718982 clientele-0.1.0/README.md
--rw-r--r--   0        0        0      793 2023-07-24 01:49:32.488234 clientele-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 07:37:51.654393 clientele-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     1713 2023-07-24 01:40:29.741703 clientele-0.1.0/src/cli.py
--rw-r--r--   0        0        0    12832 2023-07-22 05:53:57.699601 clientele-0.1.0/src/generator.py
--rw-r--r--   0        0        0      109 2023-07-21 07:37:51.656574 clientele-0.1.0/src/settings.py
--rw-r--r--   0        0        0        0 2023-07-21 07:37:51.652078 clientele-0.1.0/src/template/__init__.py
--rw-r--r--   0        0        0      108 2023-07-21 07:37:51.651661 clientele-0.1.0/src/template/client.py
--rw-r--r--   0        0        0      854 2023-07-21 08:10:05.563681 clientele-0.1.0/src/template/http.py
--rw-r--r--   0        0        0       91 2023-07-21 07:37:51.653295 clientele-0.1.0/src/template/schemas.py
--rw-r--r--   0        0        0      340 2023-07-21 07:37:51.657244 clientele-0.1.0/src/writer.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 clientele-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1607 2023-07-24 03:48:04.784855 clientele-0.2.0/README.md
+-rw-r--r--   0        0        0      872 2023-07-24 04:21:34.493850 clientele-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.2.0/src/__init__.py
+-rw-r--r--   0        0        0     1890 2023-07-24 03:57:17.660962 clientele-0.2.0/src/cli.py
+-rw-r--r--   0        0        0     1355 2023-07-24 02:58:52.770829 clientele-0.2.0/src/generator.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.2.0/src/generators/__init__.py
+-rw-r--r--   0        0        0     8426 2023-07-24 04:18:46.735999 clientele-0.2.0/src/generators/clients.py
+-rw-r--r--   0        0        0     3793 2023-07-24 03:51:19.613122 clientele-0.2.0/src/generators/http.py
+-rw-r--r--   0        0        0     3621 2023-07-24 04:14:37.896419 clientele-0.2.0/src/generators/schemas.py
+-rw-r--r--   0        0        0      109 2023-07-24 01:55:07.678461 clientele-0.2.0/src/settings.py
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.2.0/src/template/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-24 03:49:46.038745 clientele-0.2.0/src/template/client.py
+-rw-r--r--   0        0        0      697 2023-07-24 03:50:51.889574 clientele-0.2.0/src/template/http.py
+-rw-r--r--   0        0        0       91 2023-07-24 01:55:07.678461 clientele-0.2.0/src/template/schemas.py
+-rw-r--r--   0        0        0     1942 2023-07-24 04:16:31.046189 clientele-0.2.0/src/utils.py
+-rw-r--r--   0        0        0      446 2023-07-24 03:32:58.998660 clientele-0.2.0/src/writer.py
+-rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 clientele-0.2.0/setup.py
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 clientele-0.2.0/PKG-INFO
```

### Comparing `clientele-0.1.0/README.md` & `clientele-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 Plus - there is no complex boilerplate and the generated code is very small.
 
 ## Features
 
 * Fully typed API Client using Pydantic.
 * Minimalist and easy to use - the generated code is tiny.
 * Choose either sync (default) or async - we support both.
+* Generates authentication code for you (curently only supports HTTP Bearer auth)
 * Written entirely in Python - no need to install other languages to use OpenAPI.
 
 We're built on:
 
 * [Pydantic 2.0](https://docs.pydantic.dev/latest/)
 * [httpx](https://www.python-httpx.org/)
 * [openapi-core](https://openapi-core.readthedocs.io/en/latest/)
@@ -30,21 +31,37 @@
 ```
 
 ## Usage
 
 ### From URLs
 
 ```sh
-clientele generate -u URL_TO_OPEN_API.json -o output/
+clientele generate -u http://URL_TO_OPEN_API.json -o output/
 ```
 
 ### From files
 
 ```sh
 clientele generate -f path/to/file.json -o output/
 ```
 
 ### Async Client
 
 ```sh
-clientele generate -f path/to/file.json -o output/ --async t
-```
+clientele generate -f path/to/file.json -o output/ --asyncio t
+```
+
+## Authentication
+
+If your OpenAPI spec provides security information for the following authentication methods:
+
+* HTTP Bearer
+
+Then clientele will provide you information on the environment variables you need to set to
+make this work during the generation. For example:
+
+```sh
+Please set
+* MY_CLIENT_AUTH_USER_KEY
+* MY_CLIENT_AUTH_PASS_KEY
+environment variable to use basic authentication
+```
```

### Comparing `clientele-0.1.0/pyproject.toml` & `clientele-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "clientele"
-version = "0.1.0"
+version = "0.2.0"
 description = "Typed API Clients from OpenAPI specs"
 authors = ["Paul Hallett <paulandrewhallett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "src"}]
+homepage = "https://github.com/beckett-software/clientele"
 
 [tool.poetry.scripts]
 clientele = "src.cli:cli_group"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 httpx = "^0.24.1"
 click = "^8.1.3"
 structlog = "^23.1.0"
+ipython = "^8.14.0"
 pydantic = "^2.0.3"
 rich = "^13.4.2"
 openapi-core = "0.18.0"
 pyyaml = "^6.0.1"
 types-pyyaml = "^6.0.12.11"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `clientele-0.1.0/src/cli.py` & `clientele-0.2.0/src/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,27 @@
             # It's probably yaml
             data = yaml.safe_load(response.content)
         spec = Spec.from_dict(data)
     else:
         with open(file, "r") as f:
             spec = Spec.from_file(f)
     log.info(
-        f"Found API client for {spec['info']['title']} | version {spec['info']['version']}"
+        f"Found API specification for {spec['info']['title']} | version {spec['info']['version']}"
     )
     major, _, _ = spec["openapi"].split(".")
     if int(major) < 3:
         log.warning(
             f"clientele only supports OpenAPI version 3.0.0 and up, and you have {spec['openapi']}"
         )
         return
+    log.info(f"OpenAPI version {spec['openapi']}")
+    if asyncio:
+        log.info("Generating async client...")
+    else:
+        log.info("Generating sync client...")
     Generator(spec=spec, asyncio=asyncio, output_dir=output).generate(url=url)
 
 
 cli_group.add_command(generate)
 
 if __name__ == "__main__":
     cli_group()
```

### Comparing `clientele-0.1.0/src/template/http.py` & `clientele-0.2.0/src/template/http.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 import typing
+from os import environ  # noqa
 
-from httpx import Client, Response
+import httpx  # noqa
 from pydantic import ValidationError
 
-client = Client()
 
-
-def _get(url: str) -> Response:
-    return client.get(url)
-
-
-def _post(url: str, data: typing.Dict) -> Response:
-    return client.post(url, json=data)
-
-
-def _handle_response(func, response):
+def handle_response(func, response):
     """
     returns a response that matches the data neatly for a function
     """
     response.raise_for_status()
     response_data = response.json()
     response_types = typing.get_type_hints(func).get("return")
     if typing.get_origin(response_types) == typing.Union:
```

