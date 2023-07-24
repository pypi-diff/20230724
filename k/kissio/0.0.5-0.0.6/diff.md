# Comparing `tmp/kissio-0.0.5.tar.gz` & `tmp/kissio-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kissio-0.0.5.tar", last modified: Mon Jul 24 10:50:20 2023, max compression
+gzip compressed data, was "kissio-0.0.6.tar", last modified: Mon Jul 24 11:10:12 2023, max compression
```

## Comparing `kissio-0.0.5.tar` & `kissio-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:20.117248 kissio-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 10:50:09.000000 kissio-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 10:50:20.117248 kissio-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 10:50:09.000000 kissio-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:20.117248 kissio-0.0.5/kissio/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 10:50:09.000000 kissio-0.0.5/kissio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-24 10:50:09.000000 kissio-0.0.5/kissio/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:20.117248 kissio-0.0.5/kissio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 10:50:20.000000 kissio-0.0.5/kissio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 10:50:20.000000 kissio-0.0.5/kissio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:50:20.000000 kissio-0.0.5/kissio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 10:50:20.000000 kissio-0.0.5/kissio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:50:20.117248 kissio-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 10:50:09.000000 kissio-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:50:20.117248 kissio-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-24 10:50:09.000000 kissio-0.0.5/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:10:12.006350 kissio-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 11:09:56.000000 kissio-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 11:10:12.006350 kissio-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 11:09:56.000000 kissio-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:10:12.002350 kissio-0.0.6/kissio/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 11:09:56.000000 kissio-0.0.6/kissio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-24 11:09:56.000000 kissio-0.0.6/kissio/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:10:12.002350 kissio-0.0.6/kissio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 11:10:11.000000 kissio-0.0.6/kissio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 11:10:11.000000 kissio-0.0.6/kissio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:10:11.000000 kissio-0.0.6/kissio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 11:10:11.000000 kissio-0.0.6/kissio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:10:12.006350 kissio-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 11:09:56.000000 kissio-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:10:12.006350 kissio-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-24 11:09:56.000000 kissio-0.0.6/test/test.py
```

### Comparing `kissio-0.0.5/LICENSE` & `kissio-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kissio-0.0.5/README.md` & `kissio-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kissio-0.0.5/kissio/pipe.py` & `kissio-0.0.6/kissio/pipe.py`

 * *Files identical despite different names*

### Comparing `kissio-0.0.5/test/test.py` & `kissio-0.0.6/test/test.py`

 * *Files identical despite different names*

