# Comparing `tmp/fastapi_dynamic_routers-0.1.tar.gz` & `tmp/fastapi_dynamic_routers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_dynamic_routers-0.1.tar", last modified: Mon Jul 24 07:14:06 2023, max compression
+gzip compressed data, was "fastapi_dynamic_routers-0.1.1.tar", last modified: Mon Jul 24 07:51:22 2023, max compression
```

## Comparing `fastapi_dynamic_routers-0.1.tar` & `fastapi_dynamic_routers-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 07:14:06.024340 fastapi_dynamic_routers-0.1/
--rw-rw-rw-   0        0        0      246 2023-07-24 07:14:06.021328 fastapi_dynamic_routers-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-07-24 07:02:01.000000 fastapi_dynamic_routers-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 07:14:05.947681 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers/
--rw-rw-rw-   0        0        0       82 2023-07-24 07:02:01.000000 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers/__init__.py
--rw-rw-rw-   0        0        0     1052 2023-07-24 07:02:01.000000 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers/dynamic_routes_includer.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:14:06.018326 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers.egg-info/
--rw-rw-rw-   0        0        0      246 2023-07-24 07:14:05.000000 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-24 07:14:05.000000 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 07:14:05.000000 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 07:14:05.000000 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-24 07:14:05.000000 fastapi_dynamic_routers-0.1/fastapi_dynamic_routers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 07:14:06.027328 fastapi_dynamic_routers-0.1/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-07-24 07:13:32.000000 fastapi_dynamic_routers-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:51:22.905495 fastapi_dynamic_routers-0.1.1/
+-rw-rw-rw-   0        0        0     1543 2023-07-24 07:51:22.898493 fastapi_dynamic_routers-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      575 2023-07-24 07:46:56.000000 fastapi_dynamic_routers-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 07:51:22.817495 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers/
+-rw-rw-rw-   0        0        0       82 2023-07-24 07:02:01.000000 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers/__init__.py
+-rw-rw-rw-   0        0        0     1052 2023-07-24 07:02:01.000000 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers/dynamic_routes_includer.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:51:22.888494 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers.egg-info/
+-rw-rw-rw-   0        0        0     1543 2023-07-24 07:51:22.000000 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-24 07:51:22.000000 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 07:51:22.000000 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 07:51:22.000000 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-24 07:51:22.000000 fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 07:51:22.906494 fastapi_dynamic_routers-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2022 2023-07-24 07:51:18.000000 fastapi_dynamic_routers-0.1.1/setup.py
```

### Comparing `fastapi_dynamic_routers-0.1/README.md` & `fastapi_dynamic_routers-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# fastapi_dynamic_routes
+# fastapi_dynamic_routers
 
-fastapi_dynamic_routes is a Python library that provides a dynamic routes includer for FastAPI. It allows you to register routes dynamically and keep your codebase clean and organized.
+fastapi_dynamic_routers is a Python library that provides a dynamic routes includer for FastAPI. It allows you to register routes dynamically and keep your codebase clean and organized.
 
 ## Installation
 
-You can install fastapi_dynamic_routes using pip:
+You can install fastapi_dynamic_routers using pip:
 
 ```bash
-pip install fastapi_dynamic_routes
+pip install fastapi_dynamic_routers
 ```
 
 
 ## Usage
 
 ```python
 from fastapi import FastAPI
-from fastapi_dynamic_routes import Routers
+from fastapi_dynamic_routers import Routers
 
 app = FastAPI()
 
 URLS = [
     'path.to.APIRouter.instantiate',
     '...'
 ]
```

### Comparing `fastapi_dynamic_routers-0.1/fastapi_dynamic_routers/dynamic_routes_includer.py` & `fastapi_dynamic_routers-0.1.1/fastapi_dynamic_routers/dynamic_routes_includer.py`

 * *Files identical despite different names*

