# Comparing `tmp/proxy_cheap-0.0.2.tar.gz` & `tmp/proxy_cheap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy_cheap-0.0.2.tar", last modified: Mon Jul 24 12:10:15 2023, max compression
+gzip compressed data, was "proxy_cheap-0.0.3.tar", last modified: Mon Jul 24 12:49:15 2023, max compression
```

## Comparing `proxy_cheap-0.0.2.tar` & `proxy_cheap-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 12:10:15.752030 proxy_cheap-0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-07-24 11:40:03.000000 proxy_cheap-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      646 2023-07-24 12:10:15.751030 proxy_cheap-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-07-24 11:32:09.000000 proxy_cheap-0.0.2/README.md
--rw-rw-rw-   0        0        0      620 2023-07-24 12:08:45.000000 proxy_cheap-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 12:10:15.752030 proxy_cheap-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 12:10:15.742027 proxy_cheap-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:10:15.745032 proxy_cheap-0.0.2/src/proxy_cheap/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:03:50.000000 proxy_cheap-0.0.2/src/proxy_cheap/__init__.py
--rw-rw-rw-   0        0        0     3427 2023-07-24 11:52:11.000000 proxy_cheap-0.0.2/src/proxy_cheap/cheap.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:10:15.750030 proxy_cheap-0.0.2/src/proxy_cheap.egg-info/
--rw-rw-rw-   0        0        0      646 2023-07-24 12:10:15.000000 proxy_cheap-0.0.2/src/proxy_cheap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-24 12:10:15.000000 proxy_cheap-0.0.2/src/proxy_cheap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 12:10:15.000000 proxy_cheap-0.0.2/src/proxy_cheap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-24 12:10:15.000000 proxy_cheap-0.0.2/src/proxy_cheap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:15.008974 proxy_cheap-0.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-07-24 11:40:03.000000 proxy_cheap-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      646 2023-07-24 12:49:15.007977 proxy_cheap-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-07-24 11:32:09.000000 proxy_cheap-0.0.3/README.md
+-rw-rw-rw-   0        0        0      620 2023-07-24 12:48:31.000000 proxy_cheap-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 12:49:15.008974 proxy_cheap-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:14.994972 proxy_cheap-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:14.997974 proxy_cheap-0.0.3/src/proxy_cheap/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:03:50.000000 proxy_cheap-0.0.3/src/proxy_cheap/__init__.py
+-rw-rw-rw-   0        0        0     3429 2023-07-24 12:40:47.000000 proxy_cheap-0.0.3/src/proxy_cheap/cheap.py
+drwxrwxrwx   0        0        0        0 2023-07-24 12:49:15.007977 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/
+-rw-rw-rw-   0        0        0      646 2023-07-24 12:49:14.000000 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-24 12:49:14.000000 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 12:49:14.000000 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-24 12:49:14.000000 proxy_cheap-0.0.3/src/proxy_cheap.egg-info/top_level.txt
```

### Comparing `proxy_cheap-0.0.2/LICENSE` & `proxy_cheap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proxy_cheap-0.0.2/PKG-INFO` & `proxy_cheap-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: proxy_cheap
-Version: 0.0.2
+Version: 0.0.3
 Summary: proxy-cheap API python implementatione
 Author-email: lr2bmail <lr2b.com@gmail.com>
 Project-URL: Homepage, https://github.com/lr2bmail/proxy_cheap
 Project-URL: Bug Tracker, https://github.com/lr2bmail/proxy_cheap/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # proxy-cheap API python implementation
 
  proxy-cheap API python implementation for ordering and managing proxies
```

### Comparing `proxy_cheap-0.0.2/pyproject.toml` & `proxy_cheap-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0","requests"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxy_cheap"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="lr2bmail", email="lr2b.com@gmail.com" },
 ]
 description = "proxy-cheap API python implementatione"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=2.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 2",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lr2bmail/proxy_cheap"
 "Bug Tracker" = "https://github.com/lr2bmail/proxy_cheap/issues"
```

### Comparing `proxy_cheap-0.0.2/src/proxy_cheap/cheap.py` & `proxy_cheap-0.0.3/src/proxy_cheap/cheap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 
+
 class Cheap():
     def __init__(self, api_key, api_secret):
         self.url_base = "https://api.proxy-cheap.com"
         self.headers = {
             "X-Api-Key": api_key,
             "X-Api-Secret": api_secret,
             "accept": "application/json",
```

### Comparing `proxy_cheap-0.0.2/src/proxy_cheap.egg-info/PKG-INFO` & `proxy_cheap-0.0.3/src/proxy_cheap.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: proxy-cheap
-Version: 0.0.2
+Version: 0.0.3
 Summary: proxy-cheap API python implementatione
 Author-email: lr2bmail <lr2b.com@gmail.com>
 Project-URL: Homepage, https://github.com/lr2bmail/proxy_cheap
 Project-URL: Bug Tracker, https://github.com/lr2bmail/proxy_cheap/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # proxy-cheap API python implementation
 
  proxy-cheap API python implementation for ordering and managing proxies
```

