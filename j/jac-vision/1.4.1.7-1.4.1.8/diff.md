# Comparing `tmp/jac_vision-1.4.1.7.tar.gz` & `tmp/jac_vision-1.4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_vision-1.4.1.7.tar", last modified: Thu Jul 20 04:00:53 2023, max compression
+gzip compressed data, was "jac_vision-1.4.1.8.tar", last modified: Mon Jul 24 16:59:14 2023, max compression
```

## Comparing `jac_vision-1.4.1.7.tar` & `jac_vision-1.4.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:53.374370 jac_vision-1.4.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-20 04:00:53.374370 jac_vision-1.4.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:53.370370 jac_vision-1.4.1.7/jac_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:53.370370 jac_vision-1.4.1.7/jac_vision/detr/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/detr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/detr/detr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/detr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/detr/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:53.374370 jac_vision-1.4.1.7/jac_vision/dpt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/dpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/dpt/dpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/dpt/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/dpt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:53.374370 jac_vision-1.4.1.7/jac_vision/rftm/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/rftm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/rftm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/rftm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/rftm/rftm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:53.374370 jac_vision-1.4.1.7/jac_vision/yolos/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/yolos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/yolos/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/yolos/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/jac_vision/yolos/yolos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:53.370370 jac_vision-1.4.1.7/jac_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-20 04:00:53.000000 jac_vision-1.4.1.7/jac_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-20 04:00:53.000000 jac_vision-1.4.1.7/jac_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:00:53.000000 jac_vision-1.4.1.7/jac_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-20 04:00:53.000000 jac_vision-1.4.1.7/jac_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 04:00:53.000000 jac_vision-1.4.1.7/jac_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:00:53.374370 jac_vision-1.4.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 04:00:37.000000 jac_vision-1.4.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:14.363707 jac_vision-1.4.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-24 16:59:14.363707 jac_vision-1.4.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:14.355707 jac_vision-1.4.1.8/jac_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:14.359707 jac_vision-1.4.1.8/jac_vision/detr/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/detr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/detr/detr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/detr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/detr/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:14.359707 jac_vision-1.4.1.8/jac_vision/dpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/dpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/dpt/dpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/dpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/dpt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:14.363707 jac_vision-1.4.1.8/jac_vision/rftm/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/rftm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/rftm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/rftm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/rftm/rftm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:14.363707 jac_vision-1.4.1.8/jac_vision/yolos/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/yolos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/yolos/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/yolos/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/jac_vision/yolos/yolos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:14.355707 jac_vision-1.4.1.8/jac_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-24 16:59:14.000000 jac_vision-1.4.1.8/jac_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 16:59:14.000000 jac_vision-1.4.1.8/jac_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:59:14.000000 jac_vision-1.4.1.8/jac_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-24 16:59:14.000000 jac_vision-1.4.1.8/jac_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 16:59:14.000000 jac_vision-1.4.1.8/jac_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:59:14.363707 jac_vision-1.4.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-24 16:58:51.000000 jac_vision-1.4.1.8/setup.py
```

### Comparing `jac_vision-1.4.1.7/jac_vision/detr/detr.py` & `jac_vision-1.4.1.8/jac_vision/detr/detr.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/jac_vision/detr/model.py` & `jac_vision-1.4.1.8/jac_vision/detr/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/jac_vision/dpt/dpt.py` & `jac_vision-1.4.1.8/jac_vision/dpt/dpt.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/jac_vision/dpt/model.py` & `jac_vision-1.4.1.8/jac_vision/dpt/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/jac_vision/rftm/model.py` & `jac_vision-1.4.1.8/jac_vision/rftm/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/jac_vision/rftm/rftm.py` & `jac_vision-1.4.1.8/jac_vision/rftm/rftm.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/jac_vision/yolos/model.py` & `jac_vision-1.4.1.8/jac_vision/yolos/model.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/jac_vision/yolos/yolos.py` & `jac_vision-1.4.1.8/jac_vision/yolos/yolos.py`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/jac_vision.egg-info/SOURCES.txt` & `jac_vision-1.4.1.8/jac_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jac_vision-1.4.1.7/setup.py` & `jac_vision-1.4.1.8/setup.py`

 * *Files identical despite different names*

