# Comparing `tmp/sdk-openapi-0.0.2.tar.gz` & `tmp/sdk-openapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk-openapi-0.0.2.tar", last modified: Mon Jul 24 06:59:54 2023, max compression
+gzip compressed data, was "sdk-openapi-0.0.3.tar", last modified: Mon Jul 24 07:04:15 2023, max compression
```

## Comparing `sdk-openapi-0.0.2.tar` & `sdk-openapi-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-24 06:59:54.331110 sdk-openapi-0.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      509 2023-07-24 06:59:54.331110 sdk-openapi-0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      265 2023-07-24 06:43:42.000000 sdk-openapi-0.0.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-24 06:59:54.327110 sdk-openapi-0.0.2/openapi/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      180 2023-07-24 06:39:07.000000 sdk-openapi-0.0.2/openapi/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-07-24 05:56:12.000000 sdk-openapi-0.0.2/openapi/constants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1300 2023-07-24 06:37:33.000000 sdk-openapi-0.0.2/openapi/core.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-24 06:59:54.331110 sdk-openapi-0.0.2/sdk_openapi.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      509 2023-07-24 06:59:54.000000 sdk-openapi-0.0.2/sdk_openapi.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-07-24 06:59:54.000000 sdk-openapi-0.0.2/sdk_openapi.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-24 06:59:54.000000 sdk-openapi-0.0.2/sdk_openapi.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-24 06:59:54.000000 sdk-openapi-0.0.2/sdk_openapi.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-07-24 06:59:54.000000 sdk-openapi-0.0.2/sdk_openapi.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-24 06:59:54.331110 sdk-openapi-0.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      753 2023-07-24 06:59:48.000000 sdk-openapi-0.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-24 07:04:15.243110 sdk-openapi-0.0.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      509 2023-07-24 07:04:15.243110 sdk-openapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      265 2023-07-24 06:43:42.000000 sdk-openapi-0.0.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-24 07:04:15.239110 sdk-openapi-0.0.3/openapi/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      180 2023-07-24 07:04:11.000000 sdk-openapi-0.0.3/openapi/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-07-24 05:56:12.000000 sdk-openapi-0.0.3/openapi/constants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1300 2023-07-24 06:37:33.000000 sdk-openapi-0.0.3/openapi/core.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-24 07:04:15.243110 sdk-openapi-0.0.3/sdk_openapi.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      509 2023-07-24 07:04:15.000000 sdk-openapi-0.0.3/sdk_openapi.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-07-24 07:04:15.000000 sdk-openapi-0.0.3/sdk_openapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-24 07:04:15.000000 sdk-openapi-0.0.3/sdk_openapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-24 07:04:15.000000 sdk-openapi-0.0.3/sdk_openapi.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-07-24 07:04:15.000000 sdk-openapi-0.0.3/sdk_openapi.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-24 07:04:15.243110 sdk-openapi-0.0.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2023-07-24 07:04:03.000000 sdk-openapi-0.0.3/setup.py
```

### Comparing `sdk-openapi-0.0.2/openapi/core.py` & `sdk-openapi-0.0.3/openapi/core.py`

 * *Files identical despite different names*

### Comparing `sdk-openapi-0.0.2/setup.py` & `sdk-openapi-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright 2023 Qewertyy, MIT License
 from setuptools import setup
 
 setup(
     name="sdk-openapi",
-    version="0.0.2",
+    version="0.0.3",
     author="Qewertyy",
     author_email="Qewertyy.irl@gmail.com",
     description="The python package for api.qewertyy.me",
     url="https://github.com/Qewertyy/Open-API",
     python_requires=">=3.8",
+    readme = "README.md",
     install_requires=[
         "requests",
         "aiohttp",
         "httpx[http2]",
         "asyncio"
     ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot, Image Generations, Latent Diffusion, State of Art",
```

