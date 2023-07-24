# Comparing `tmp/Shimarin-0.0.9.tar.gz` & `tmp/Shimarin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimarin-0.0.9.tar", last modified: Mon May 22 12:23:19 2023, max compression
+gzip compressed data, was "Shimarin-0.1.0.tar", last modified: Mon Jul 24 21:13:06 2023, max compression
```

## Comparing `Shimarin-0.0.9.tar` & `Shimarin-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.198397 Shimarin-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 12:23:19.198397 Shimarin-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 12:23:07.000000 Shimarin-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.194397 Shimarin-0.0.9/Shimarin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.198397 Shimarin-0.0.9/Shimarin/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/client/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.198397 Shimarin-0.0.9/Shimarin/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/server/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.194397 Shimarin-0.0.9/Shimarin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 12:23:07.000000 Shimarin-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-22 12:23:19.198397 Shimarin-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:06.679068 Shimarin-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-24 21:13:06.679068 Shimarin-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 21:12:53.000000 Shimarin-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:06.675068 Shimarin-0.1.0/Shimarin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:06.679068 Shimarin-0.1.0/Shimarin/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/client/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:06.675068 Shimarin-0.1.0/Shimarin/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:06.679068 Shimarin-0.1.0/Shimarin/plugins/flask_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/plugins/flask_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/plugins/flask_api/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:06.679068 Shimarin-0.1.0/Shimarin/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 21:12:53.000000 Shimarin-0.1.0/Shimarin/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:06.679068 Shimarin-0.1.0/Shimarin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-24 21:13:06.000000 Shimarin-0.1.0/Shimarin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-24 21:13:06.000000 Shimarin-0.1.0/Shimarin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:13:06.000000 Shimarin-0.1.0/Shimarin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:13:06.000000 Shimarin-0.1.0/Shimarin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 21:13:06.000000 Shimarin-0.1.0/Shimarin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 21:13:06.000000 Shimarin-0.1.0/Shimarin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-24 21:12:53.000000 Shimarin-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-24 21:13:06.679068 Shimarin-0.1.0/setup.cfg
```

### Comparing `Shimarin-0.0.9/PKG-INFO` & `Shimarin-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.9
+Version: 0.1.0
 Summary: asynchronous event-based communication between client and server
-Home-page: 
+Home-page: https://github.com/kamuridesu/Shimarin
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
+Provides-Extra: flask
 
 # Shimarin
 
 Asynchronous event-based communication between client and server.
 
 
 # How to use
```

### Comparing `Shimarin-0.0.9/Shimarin/client/events.py` & `Shimarin-0.1.0/Shimarin/client/events.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.0.9/Shimarin/client/networking.py` & `Shimarin-0.1.0/Shimarin/client/networking.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.0.9/Shimarin/server/events.py` & `Shimarin-0.1.0/Shimarin/server/events.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.0.9/Shimarin.egg-info/PKG-INFO` & `Shimarin-0.1.0/Shimarin.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.9
+Version: 0.1.0
 Summary: asynchronous event-based communication between client and server
-Home-page: 
+Home-page: https://github.com/kamuridesu/Shimarin
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
+Provides-Extra: flask
 
 # Shimarin
 
 Asynchronous event-based communication between client and server.
 
 
 # How to use
```

