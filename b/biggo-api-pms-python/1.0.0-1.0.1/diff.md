# Comparing `tmp/biggo-api-pms-python-1.0.0.tar.gz` & `tmp/biggo-api-pms-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biggo-api-pms-python-1.0.0.tar", last modified: Mon Jul 24 04:00:03 2023, max compression
+gzip compressed data, was "biggo-api-pms-python-1.0.1.tar", last modified: Mon Jul 24 04:04:05 2023, max compression
```

## Comparing `biggo-api-pms-python-1.0.0.tar` & `biggo-api-pms-python-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 04:00:03.952479 biggo-api-pms-python-1.0.0/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1069 2023-07-24 01:23:02.000000 biggo-api-pms-python-1.0.0/LICENSE
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 04:00:03.952479 biggo-api-pms-python-1.0.0/PKG-INFO
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1823 2023-07-24 01:23:02.000000 biggo-api-pms-python-1.0.0/README.md
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 04:00:03.952479 biggo-api-pms-python-1.0.0/biggo_api_pms_python.egg-info/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 04:00:03.000000 biggo-api-pms-python-1.0.0/biggo_api_pms_python.egg-info/PKG-INFO
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      202 2023-07-24 04:00:03.000000 biggo-api-pms-python-1.0.0/biggo_api_pms_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 04:00:03.000000 biggo-api-pms-python-1.0.0/biggo_api_pms_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 04:00:03.000000 biggo-api-pms-python-1.0.0/biggo_api_pms_python.egg-info/top_level.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)       38 2023-07-24 04:00:03.952479 biggo-api-pms-python-1.0.0/setup.cfg
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      304 2023-07-24 03:59:47.000000 biggo-api-pms-python-1.0.0/setup.py
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 04:04:05.152952 biggo-api-pms-python-1.0.1/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1069 2023-07-24 01:23:02.000000 biggo-api-pms-python-1.0.1/LICENSE
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 04:04:05.152952 biggo-api-pms-python-1.0.1/PKG-INFO
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1823 2023-07-24 01:23:02.000000 biggo-api-pms-python-1.0.1/README.md
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 04:04:05.152952 biggo-api-pms-python-1.0.1/biggo-api-python-pms/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)        0 2023-07-24 02:38:22.000000 biggo-api-pms-python-1.0.1/biggo-api-python-pms/__init__.py
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      451 2023-07-24 01:44:32.000000 biggo-api-pms-python-1.0.1/biggo-api-python-pms/error.py
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     7414 2023-07-24 02:43:54.000000 biggo-api-pms-python-1.0.1/biggo-api-python-pms/index.py
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 04:04:05.152952 biggo-api-pms-python-1.0.1/biggo_api_pms_python.egg-info/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 04:04:05.000000 biggo-api-pms-python-1.0.1/biggo_api_pms_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 04:04:05.000000 biggo-api-pms-python-1.0.1/biggo_api_pms_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 04:04:05.000000 biggo-api-pms-python-1.0.1/biggo_api_pms_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       21 2023-07-24 04:04:05.000000 biggo-api-pms-python-1.0.1/biggo_api_pms_python.egg-info/top_level.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       38 2023-07-24 04:04:05.152952 biggo-api-pms-python-1.0.1/setup.cfg
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      304 2023-07-24 04:04:02.000000 biggo-api-pms-python-1.0.1/setup.py
```

### Comparing `biggo-api-pms-python-1.0.0/LICENSE` & `biggo-api-pms-python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biggo-api-pms-python-1.0.0/README.md` & `biggo-api-pms-python-1.0.1/README.md`

 * *Files identical despite different names*

