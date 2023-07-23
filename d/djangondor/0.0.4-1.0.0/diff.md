# Comparing `tmp/djangondor-0.0.4.tar.gz` & `tmp/djangondor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "djangondor-1.0.0.tar", last modified: Sun Jul 23 22:13:43 2023, max compression
```

## Comparing `djangondor-0.0.4.tar` & `djangondor-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,29 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 djangondor-0.0.4/src/djangondor/__about__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 djangondor-0.0.4/src/djangondor/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 djangondor-0.0.4/src/djangondor/collections.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 djangondor-0.0.4/src/djangondor/requests.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 djangondor-0.0.4/src/djangondor/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangondor-0.0.4/src/djangondor/templatetags/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 djangondor-0.0.4/src/djangondor/templatetags/djangondor_collection_tags.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 djangondor-0.0.4/src/djangondor/templatetags/djangondor_path_tags.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 djangondor-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 djangondor-0.0.4/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 djangondor-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 djangondor-0.0.4/README.md
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 djangondor-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 djangondor-0.0.4/PKG-INFO
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.0.0/LICENSE
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1169 2023-07-23 22:13:43.625484 djangondor-1.0.0/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      285 2023-07-23 22:13:38.000000 djangondor-1.0.0/README.rst
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/djangondor/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/admin.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/apps.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      645 2023-07-23 12:18:10.000000 djangondor-1.0.0/djangondor/collections.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/djangondor/migrations/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/migrations/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       57 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/models.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     2800 2023-07-21 07:32:44.000000 djangondor-1.0.0/djangondor/requests.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/djangondor/templatetags/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.0.0/djangondor/templatetags/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.0.0/djangondor/templatetags/djangondor_collection_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.0.0/djangondor/templatetags/djangondor_path_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/tests.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.0.0/djangondor/time.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/views.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/djangondor.egg-info/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1169 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      584 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/requires.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/top_level.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.0.0/pyproject.toml
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      894 2023-07-23 22:13:43.629484 djangondor-1.0.0/setup.cfg
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       38 2023-07-23 21:11:32.000000 djangondor-1.0.0/setup.py
```

### Comparing `djangondor-0.0.4/src/djangondor/collections.py` & `djangondor-1.0.0/djangondor/collections.py`

 * *Files identical despite different names*

### Comparing `djangondor-0.0.4/src/djangondor/requests.py` & `djangondor-1.0.0/djangondor/requests.py`

 * *Files identical despite different names*

### Comparing `djangondor-0.0.4/src/djangondor/time.py` & `djangondor-1.0.0/djangondor/time.py`

 * *Files identical despite different names*

### Comparing `djangondor-0.0.4/src/djangondor/templatetags/djangondor_path_tags.py` & `djangondor-1.0.0/djangondor/templatetags/djangondor_path_tags.py`

 * *Files identical despite different names*

### Comparing `djangondor-0.0.4/LICENSE.txt` & `djangondor-1.0.0/LICENSE`

 * *Files identical despite different names*

