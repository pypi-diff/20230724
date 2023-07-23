# Comparing `tmp/djangondor-1.0.0.tar.gz` & `tmp/djangondor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangondor-1.0.0.tar", last modified: Sun Jul 23 22:13:43 2023, max compression
+gzip compressed data, was "djangondor-1.0.1.tar", last modified: Sun Jul 23 22:25:54 2023, max compression
```

## Comparing `djangondor-1.0.0.tar` & `djangondor-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.0.0/LICENSE
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1169 2023-07-23 22:13:43.625484 djangondor-1.0.0/PKG-INFO
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      285 2023-07-23 22:13:38.000000 djangondor-1.0.0/README.rst
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/djangondor/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/admin.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/apps.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      645 2023-07-23 12:18:10.000000 djangondor-1.0.0/djangondor/collections.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/djangondor/migrations/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/migrations/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       57 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/models.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     2800 2023-07-21 07:32:44.000000 djangondor-1.0.0/djangondor/requests.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/djangondor/templatetags/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.0.0/djangondor/templatetags/__init__.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.0.0/djangondor/templatetags/djangondor_collection_tags.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.0.0/djangondor/templatetags/djangondor_path_tags.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/tests.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.0.0/djangondor/time.py
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.0/djangondor/views.py
-drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:13:43.625484 djangondor-1.0.0/djangondor.egg-info/
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1169 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/PKG-INFO
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      584 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/SOURCES.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/dependency_links.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/requires.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-23 22:13:43.000000 djangondor-1.0.0/djangondor.egg-info/top_level.txt
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.0.0/pyproject.toml
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      894 2023-07-23 22:13:43.629484 djangondor-1.0.0/setup.cfg
--rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       38 2023-07-23 21:11:32.000000 djangondor-1.0.0/setup.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.900786 djangondor-1.0.1/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1103 2023-07-21 07:05:22.000000 djangondor-1.0.1/LICENSE
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1279 2023-07-23 22:25:54.900786 djangondor-1.0.1/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      394 2023-07-23 22:23:20.000000 djangondor-1.0.1/README.rst
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.896787 djangondor-1.0.1/djangondor/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/admin.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      152 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/apps.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      645 2023-07-23 12:18:10.000000 djangondor-1.0.1/djangondor/collections.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.900786 djangondor-1.0.1/djangondor/migrations/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/migrations/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       57 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/models.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     2800 2023-07-21 07:32:44.000000 djangondor-1.0.1/djangondor/requests.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.900786 djangondor-1.0.1/djangondor/templatetags/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 11:24:34.000000 djangondor-1.0.1/djangondor/templatetags/__init__.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      410 2023-07-23 11:25:18.000000 djangondor-1.0.1/djangondor/templatetags/djangondor_collection_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1601 2023-07-23 11:22:38.000000 djangondor-1.0.1/djangondor/templatetags/djangondor_path_tags.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       60 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/tests.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      909 2023-07-21 07:30:17.000000 djangondor-1.0.1/djangondor/time.py
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       63 2023-07-23 20:57:03.000000 djangondor-1.0.1/djangondor/views.py
+drwxrwxr-x   0 dalitso   (1000) dalitso   (1000)        0 2023-07-23 22:25:54.900786 djangondor-1.0.1/djangondor.egg-info/
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)     1279 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/PKG-INFO
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      584 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)        1 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       12 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/requires.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       11 2023-07-23 22:25:54.000000 djangondor-1.0.1/djangondor.egg-info/top_level.txt
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       89 2023-07-23 21:09:19.000000 djangondor-1.0.1/pyproject.toml
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)      894 2023-07-23 22:25:54.900786 djangondor-1.0.1/setup.cfg
+-rw-rw-r--   0 dalitso   (1000) dalitso   (1000)       38 2023-07-23 21:11:32.000000 djangondor-1.0.1/setup.py
```

### Comparing `djangondor-1.0.0/LICENSE` & `djangondor-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.0/PKG-INFO` & `djangondor-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -35,7 +35,9 @@
 
 1. Add "djangondor" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
         ...,
         "djangondor",
     ]
+
+2. See the documentation at <https://github.com/DalitsoSakala/djangondor/blob/main/djangondor/docs/INDEX.md>
```

### Comparing `djangondor-1.0.0/djangondor/collections.py` & `djangondor-1.0.1/djangondor/collections.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.0/djangondor/requests.py` & `djangondor-1.0.1/djangondor/requests.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.0/djangondor/templatetags/djangondor_path_tags.py` & `djangondor-1.0.1/djangondor/templatetags/djangondor_path_tags.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.0/djangondor/time.py` & `djangondor-1.0.1/djangondor/time.py`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.0/djangondor.egg-info/PKG-INFO` & `djangondor-1.0.1/djangondor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of django utilities.
 Home-page: https://github.com/dalitsosakala/djangondor
 Author: Dalitso Sakala
 Author-email: dalitso.1sc@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -35,7 +35,9 @@
 
 1. Add "djangondor" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
         ...,
         "djangondor",
     ]
+
+2. See the documentation at <https://github.com/DalitsoSakala/djangondor/blob/main/djangondor/docs/INDEX.md>
```

### Comparing `djangondor-1.0.0/djangondor.egg-info/SOURCES.txt` & `djangondor-1.0.1/djangondor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangondor-1.0.0/setup.cfg` & `djangondor-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangondor
-version = 1.0.0
+version = 1.0.1
 description = A collection of django utilities.
 long_description = file: README.rst
 url = https://github.com/dalitsosakala/djangondor
 author = Dalitso Sakala
 author_email = dalitso.1sc@gmail.com
 license = MIT License
 classifiers =
```

