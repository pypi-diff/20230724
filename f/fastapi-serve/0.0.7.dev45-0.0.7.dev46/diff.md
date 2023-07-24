# Comparing `tmp/fastapi-serve-0.0.7.dev45.tar.gz` & `tmp/fastapi-serve-0.0.7.dev46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.7.dev45.tar", last modified: Fri Jul 21 10:21:34 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.7.dev46.tar", last modified: Mon Jul 24 14:48:45 2023, max compression
```

## Comparing `fastapi-serve-0.0.7.dev45.tar` & `fastapi-serve-0.0.7.dev46.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.251269 fastapi-serve-0.0.7.dev45/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 10:21:33.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.251269 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/blob/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.251269 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:48:45.892480 fastapi-serve-0.0.7.dev46/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-24 14:48:45.892480 fastapi-serve-0.0.7.dev46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:48:45.888480 fastapi-serve-0.0.7.dev46/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-24 14:48:45.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:48:45.888480 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:48:45.892480 fastapi-serve-0.0.7.dev46/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:48:45.892480 fastapi-serve-0.0.7.dev46/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:48:45.892480 fastapi-serve-0.0.7.dev46/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:48:45.888480 fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-24 14:48:45.000000 fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-24 14:48:45.000000 fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:48:45.000000 fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 14:48:45.000000 fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:48:45.000000 fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 14:48:45.000000 fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 14:48:45.000000 fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:48:45.892480 fastapi-serve-0.0.7.dev46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-24 14:48:37.000000 fastapi-serve-0.0.7.dev46/setup.py
```

### Comparing `fastapi-serve-0.0.7.dev45/LICENSE` & `fastapi-serve-0.0.7.dev46/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/PKG-INFO` & `fastapi-serve-0.0.7.dev46/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.7.dev45
+Version: 0.0.7.dev46
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -79,15 +79,15 @@
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
     - 🧱 [Deploy a simple FastAPI application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
     - ⚙️ [Understanding configuration and pricing on Jina AI Cloud](docs/CONFIG.MD)
     - 🔄 [Upgrade your FastAPI applications with zero downtime](docs/upgrades/)
-    - 🏢 Managing Larger Applications with Complex Directory Structure (Documentation in progress 🚧)
+    - 🕸️ [Managing Larger Applications with Complex Directory Structure](docs/larger/project1)
 - ↕️ **Scaling**
     - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
     - 📉 [Serverless (scale-to-zero) deployments based on RPS](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
     - 🌍 [Leverage environment variables for app configuration](docs/envs/)
     - 🗝️ [Use secrets for Redis-powered rate limiting](docs/rate_limit/)
 - 💾 **Storage**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.7.dev45 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.7.dev46 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -48,17 +48,17 @@
 FastAPI application: ```bash fastapi-serve deploy jcloud main:app ``` You'll
 get a URL to access your newly deployed application along with the Swagger UI.
 ## ð Documentation Dive into understanding `fastapi-serve` through our
 comprehensive documentation and examples: - ð **Getting Started** - ð§±
 [Deploy a simple FastAPI application](docs/simple/) - ð¥ï¸ [Dig deep into
 the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding configuration and
 pricing on Jina AI Cloud](docs/CONFIG.MD) - ð [Upgrade your FastAPI
-applications with zero downtime](docs/upgrades/) - ð¢ Managing Larger
-Applications with Complex Directory Structure (Documentation in progress ð§)
-- âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
+applications with zero downtime](docs/upgrades/) - ð¸ï¸ [Managing Larger
+Applications with Complex Directory Structure](docs/larger/project1) - âï¸
+**Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
 autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments based on RPS]
 (docs/autoscaling/serverless/) - ð§© **Config & Credentials** - ð [Leverage
 environment variables for app configuration](docs/envs/) - ðï¸ [Use secrets
 for Redis-powered rate limiting](docs/rate_limit/) - ð¾ **Storage** - ð
 [Manage file uploads and downloads with built-in blob storage](docs/
 file_handling/) - ð Network storage for persisting and securely accessing
 app data (Documentation in progress ð§) - ð **Security** - ð®ââï¸
```

### Comparing `fastapi-serve-0.0.7.dev45/README.md` & `fastapi-serve-0.0.7.dev46/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
     - 🧱 [Deploy a simple FastAPI application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
     - ⚙️ [Understanding configuration and pricing on Jina AI Cloud](docs/CONFIG.MD)
     - 🔄 [Upgrade your FastAPI applications with zero downtime](docs/upgrades/)
-    - 🏢 Managing Larger Applications with Complex Directory Structure (Documentation in progress 🚧)
+    - 🕸️ [Managing Larger Applications with Complex Directory Structure](docs/larger/project1)
 - ↕️ **Scaling**
     - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
     - 📉 [Serverless (scale-to-zero) deployments based on RPS](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
     - 🌍 [Leverage environment variables for app configuration](docs/envs/)
     - 🗝️ [Use secrets for Redis-powered rate limiting](docs/rate_limit/)
 - 💾 **Storage**
```

#### html2text {}

```diff
@@ -31,17 +31,17 @@
 FastAPI application: ```bash fastapi-serve deploy jcloud main:app ``` You'll
 get a URL to access your newly deployed application along with the Swagger UI.
 ## ð Documentation Dive into understanding `fastapi-serve` through our
 comprehensive documentation and examples: - ð **Getting Started** - ð§±
 [Deploy a simple FastAPI application](docs/simple/) - ð¥ï¸ [Dig deep into
 the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding configuration and
 pricing on Jina AI Cloud](docs/CONFIG.MD) - ð [Upgrade your FastAPI
-applications with zero downtime](docs/upgrades/) - ð¢ Managing Larger
-Applications with Complex Directory Structure (Documentation in progress ð§)
-- âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
+applications with zero downtime](docs/upgrades/) - ð¸ï¸ [Managing Larger
+Applications with Complex Directory Structure](docs/larger/project1) - âï¸
+**Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
 autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments based on RPS]
 (docs/autoscaling/serverless/) - ð§© **Config & Credentials** - ð [Leverage
 environment variables for app configuration](docs/envs/) - ðï¸ [Use secrets
 for Redis-powered rate limiting](docs/rate_limit/) - ð¾ **Storage** - ð
 [Manage file uploads and downloads with built-in blob storage](docs/
 file_handling/) - ð Network storage for persisting and securely accessing
 app data (Documentation in progress ð§) - ð **Security** - ð®ââï¸
```

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/__main__.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/export.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/export.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/cloud/options.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/helper.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/utils/auth.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/utils/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/utils/blob/storage.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/utils/blob/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve/utils/helper.py` & `fastapi-serve-0.0.7.dev46/fastapi_serve/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.7.dev45
+Version: 0.0.7.dev46
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -79,15 +79,15 @@
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
     - 🧱 [Deploy a simple FastAPI application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
     - ⚙️ [Understanding configuration and pricing on Jina AI Cloud](docs/CONFIG.MD)
     - 🔄 [Upgrade your FastAPI applications with zero downtime](docs/upgrades/)
-    - 🏢 Managing Larger Applications with Complex Directory Structure (Documentation in progress 🚧)
+    - 🕸️ [Managing Larger Applications with Complex Directory Structure](docs/larger/project1)
 - ↕️ **Scaling**
     - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
     - 📉 [Serverless (scale-to-zero) deployments based on RPS](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
     - 🌍 [Leverage environment variables for app configuration](docs/envs/)
     - 🗝️ [Use secrets for Redis-powered rate limiting](docs/rate_limit/)
 - 💾 **Storage**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.7.dev45 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.7.dev46 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -48,17 +48,17 @@
 FastAPI application: ```bash fastapi-serve deploy jcloud main:app ``` You'll
 get a URL to access your newly deployed application along with the Swagger UI.
 ## ð Documentation Dive into understanding `fastapi-serve` through our
 comprehensive documentation and examples: - ð **Getting Started** - ð§±
 [Deploy a simple FastAPI application](docs/simple/) - ð¥ï¸ [Dig deep into
 the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding configuration and
 pricing on Jina AI Cloud](docs/CONFIG.MD) - ð [Upgrade your FastAPI
-applications with zero downtime](docs/upgrades/) - ð¢ Managing Larger
-Applications with Complex Directory Structure (Documentation in progress ð§)
-- âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
+applications with zero downtime](docs/upgrades/) - ð¸ï¸ [Managing Larger
+Applications with Complex Directory Structure](docs/larger/project1) - âï¸
+**Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
 autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments based on RPS]
 (docs/autoscaling/serverless/) - ð§© **Config & Credentials** - ð [Leverage
 environment variables for app configuration](docs/envs/) - ðï¸ [Use secrets
 for Redis-powered rate limiting](docs/rate_limit/) - ð¾ **Storage** - ð
 [Manage file uploads and downloads with built-in blob storage](docs/
 file_handling/) - ð Network storage for persisting and securely accessing
 app data (Documentation in progress ð§) - ð **Security** - ð®ââï¸
```

### Comparing `fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.7.dev46/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.7.dev45/setup.py` & `fastapi-serve-0.0.7.dev46/setup.py`

 * *Files identical despite different names*

