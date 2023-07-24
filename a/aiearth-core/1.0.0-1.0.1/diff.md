# Comparing `tmp/aiearth-core-1.0.0.tar.gz` & `tmp/aiearth-core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiearth-core-1.0.0.tar", last modified: Thu Jun  8 05:54:37 2023, max compression
+gzip compressed data, was "aiearth-core-1.0.1.tar", last modified: Mon Jul 24 05:54:43 2023, max compression
```

## Comparing `aiearth-core-1.0.0.tar` & `aiearth-core-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 05:54:37.536851 aiearth-core-1.0.0/
--rw-r--r--   0 songci     (502) staff       (20)    11357 2023-05-24 03:51:09.000000 aiearth-core-1.0.0/LICENSE
--rw-r--r--   0 songci     (502) staff       (20)      396 2023-06-08 05:54:37.537041 aiearth-core-1.0.0/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)       55 2023-05-17 11:31:12.000000 aiearth-core-1.0.0/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 05:54:37.485275 aiearth-core-1.0.0/aiearth/
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 05:54:37.529338 aiearth-core-1.0.0/aiearth/core/
--rw-r--r--   0 songci     (502) staff       (20)      120 2023-06-06 06:47:03.000000 aiearth-core-1.0.0/aiearth/core/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     4150 2023-05-24 03:36:40.000000 aiearth-core-1.0.0/aiearth/core/auth.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 05:54:37.531939 aiearth-core-1.0.0/aiearth/core/client/
--rw-r--r--   0 songci     (502) staff       (20)       80 2023-05-17 11:32:17.000000 aiearth-core-1.0.0/aiearth/core/client/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     3812 2023-05-15 07:24:04.000000 aiearth-core-1.0.0/aiearth/core/client/client.py
--rw-r--r--   0 songci     (502) staff       (20)      775 2022-11-21 06:06:45.000000 aiearth-core-1.0.0/aiearth/core/client/constants.py
--rw-r--r--   0 songci     (502) staff       (20)     1652 2023-05-18 12:58:40.000000 aiearth-core-1.0.0/aiearth/core/client/endpoints.py
--rw-r--r--   0 songci     (502) staff       (20)      191 2023-05-15 07:24:04.000000 aiearth-core-1.0.0/aiearth/core/env.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 05:54:37.533167 aiearth-core-1.0.0/aiearth/core/error/
--rw-r--r--   0 songci     (502) staff       (20)      115 2022-11-21 06:06:45.000000 aiearth-core-1.0.0/aiearth/core/error/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)      849 2022-11-21 06:06:45.000000 aiearth-core-1.0.0/aiearth/core/error/aie_error.py
--rw-r--r--   0 songci     (502) staff       (20)      904 2023-05-15 05:43:26.000000 aiearth-core-1.0.0/aiearth/core/g_var.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 05:54:37.536415 aiearth-core-1.0.0/aiearth_core.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      396 2023-06-08 05:54:37.000000 aiearth-core-1.0.0/aiearth_core.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      494 2023-06-08 05:54:37.000000 aiearth-core-1.0.0/aiearth_core.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-06-08 05:54:37.000000 aiearth-core-1.0.0/aiearth_core.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)       43 2023-06-08 05:54:37.000000 aiearth-core-1.0.0/aiearth_core.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        8 2023-06-08 05:54:37.000000 aiearth-core-1.0.0/aiearth_core.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       74 2023-06-08 05:54:37.537693 aiearth-core-1.0.0/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)     1117 2023-05-26 05:53:58.000000 aiearth-core-1.0.0/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-24 05:54:43.573696 aiearth-core-1.0.1/
+-rw-r--r--   0 songci     (502) staff       (20)    11357 2023-05-24 03:51:09.000000 aiearth-core-1.0.1/LICENSE
+-rw-r--r--   0 songci     (502) staff       (20)      396 2023-07-24 05:54:43.573876 aiearth-core-1.0.1/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)       55 2023-05-17 11:31:12.000000 aiearth-core-1.0.1/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-24 05:54:43.560456 aiearth-core-1.0.1/aiearth/
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-24 05:54:43.566453 aiearth-core-1.0.1/aiearth/core/
+-rw-r--r--   0 songci     (502) staff       (20)      120 2023-07-24 02:16:19.000000 aiearth-core-1.0.1/aiearth/core/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     4150 2023-05-24 03:36:40.000000 aiearth-core-1.0.1/aiearth/core/auth.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-24 05:54:43.568824 aiearth-core-1.0.1/aiearth/core/client/
+-rw-r--r--   0 songci     (502) staff       (20)       80 2023-05-17 11:32:17.000000 aiearth-core-1.0.1/aiearth/core/client/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     3812 2023-05-15 07:24:04.000000 aiearth-core-1.0.1/aiearth/core/client/client.py
+-rw-r--r--   0 songci     (502) staff       (20)      775 2022-11-21 06:06:45.000000 aiearth-core-1.0.1/aiearth/core/client/constants.py
+-rw-r--r--   0 songci     (502) staff       (20)     1652 2023-05-18 12:58:40.000000 aiearth-core-1.0.1/aiearth/core/client/endpoints.py
+-rw-r--r--   0 songci     (502) staff       (20)      314 2023-07-24 02:16:05.000000 aiearth-core-1.0.1/aiearth/core/env.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-24 05:54:43.570209 aiearth-core-1.0.1/aiearth/core/error/
+-rw-r--r--   0 songci     (502) staff       (20)      115 2022-11-21 06:06:45.000000 aiearth-core-1.0.1/aiearth/core/error/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)      849 2022-11-21 06:06:45.000000 aiearth-core-1.0.1/aiearth/core/error/aie_error.py
+-rw-r--r--   0 songci     (502) staff       (20)      904 2023-05-15 05:43:26.000000 aiearth-core-1.0.1/aiearth/core/g_var.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-24 05:54:43.573250 aiearth-core-1.0.1/aiearth_core.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      396 2023-07-24 05:54:43.000000 aiearth-core-1.0.1/aiearth_core.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      494 2023-07-24 05:54:43.000000 aiearth-core-1.0.1/aiearth_core.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-07-24 05:54:43.000000 aiearth-core-1.0.1/aiearth_core.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)       43 2023-07-24 05:54:43.000000 aiearth-core-1.0.1/aiearth_core.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        8 2023-07-24 05:54:43.000000 aiearth-core-1.0.1/aiearth_core.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       74 2023-07-24 05:54:43.574526 aiearth-core-1.0.1/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)     1117 2023-05-26 05:53:58.000000 aiearth-core-1.0.1/setup.py
```

### Comparing `aiearth-core-1.0.0/LICENSE` & `aiearth-core-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiearth-core-1.0.0/aiearth/core/auth.py` & `aiearth-core-1.0.1/aiearth/core/auth.py`

 * *Files identical despite different names*

### Comparing `aiearth-core-1.0.0/aiearth/core/client/client.py` & `aiearth-core-1.0.1/aiearth/core/client/client.py`

 * *Files identical despite different names*

### Comparing `aiearth-core-1.0.0/aiearth/core/client/constants.py` & `aiearth-core-1.0.1/aiearth/core/client/constants.py`

 * *Files identical despite different names*

### Comparing `aiearth-core-1.0.0/aiearth/core/client/endpoints.py` & `aiearth-core-1.0.1/aiearth/core/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `aiearth-core-1.0.0/aiearth/core/error/aie_error.py` & `aiearth-core-1.0.1/aiearth/core/error/aie_error.py`

 * *Files identical despite different names*

### Comparing `aiearth-core-1.0.0/aiearth/core/g_var.py` & `aiearth-core-1.0.1/aiearth/core/g_var.py`

 * *Files identical despite different names*

### Comparing `aiearth-core-1.0.0/setup.py` & `aiearth-core-1.0.1/setup.py`

 * *Files identical despite different names*

