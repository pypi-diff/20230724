# Comparing `tmp/arq-django-admin-0.3.1.tar.gz` & `tmp/arq-django-admin-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arq-django-admin-0.3.1.tar", last modified: Tue Jul 11 10:21:22 2023, max compression
+gzip compressed data, was "arq-django-admin-0.3.2.tar", last modified: Mon Jul 24 08:04:49 2023, max compression
```

## Comparing `arq-django-admin-0.3.1.tar` & `arq-django-admin-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/arq_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.608548 arq-django-admin-0.3.1/arq_admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/arq_admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/job_abort.html
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/job_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/jobs.html
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/templates/arq_admin/queues.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/arq_admin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/arq_django_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:21:22.000000 arq-django-admin-0.3.1/arq_django_admin.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 10:21:22.612548 arq-django-admin-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-11 10:21:12.000000 arq-django-admin-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:49.482006 arq-django-admin-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-24 08:04:49.482006 arq-django-admin-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:49.478006 arq-django-admin-0.3.2/arq_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:49.478006 arq-django-admin-0.3.2/arq_admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:49.482006 arq-django-admin-0.3.2/arq_admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/templates/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:49.482006 arq-django-admin-0.3.2/arq_admin/templates/arq_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/templates/arq_admin/job_abort.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/templates/arq_admin/job_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/templates/arq_admin/jobs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/templates/arq_admin/queues.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/arq_admin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:49.482006 arq-django-admin-0.3.2/arq_django_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-24 08:04:49.000000 arq-django-admin-0.3.2/arq_django_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-24 08:04:49.000000 arq-django-admin-0.3.2/arq_django_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:04:49.000000 arq-django-admin-0.3.2/arq_django_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 08:04:49.000000 arq-django-admin-0.3.2/arq_django_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 08:04:49.000000 arq-django-admin-0.3.2/arq_django_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:04:49.000000 arq-django-admin-0.3.2/arq_django_admin.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 08:04:49.486006 arq-django-admin-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-24 08:04:34.000000 arq-django-admin-0.3.2/setup.py
```

### Comparing `arq-django-admin-0.3.1/LICENSE` & `arq-django-admin-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/PKG-INFO` & `arq-django-admin-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arq-django-admin
-Version: 0.3.1
+Version: 0.3.2
 Summary: An app that provides Django admin for ARQ
 Home-page: https://github.com/SlavaSkvortsov/arq-django-admin
 Author: Slava Skvortsov
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arq-django-admin-0.3.1/README.md` & `arq-django-admin-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/job.py` & `arq-django-admin-0.3.2/arq_admin/job.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/queue.py` & `arq-django-admin-0.3.2/arq_admin/queue.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/settings.py` & `arq-django-admin-0.3.2/arq_admin/settings.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/templates/arq_admin/job_abort.html` & `arq-django-admin-0.3.2/arq_admin/templates/arq_admin/job_abort.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/templates/arq_admin/job_detail.html` & `arq-django-admin-0.3.2/arq_admin/templates/arq_admin/job_detail.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/templates/arq_admin/jobs.html` & `arq-django-admin-0.3.2/arq_admin/templates/arq_admin/jobs.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/templates/arq_admin/queues.html` & `arq-django-admin-0.3.2/arq_admin/templates/arq_admin/queues.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/urls.py` & `arq-django-admin-0.3.2/arq_admin/urls.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_admin/views.py` & `arq-django-admin-0.3.2/arq_admin/views.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/arq_django_admin.egg-info/PKG-INFO` & `arq-django-admin-0.3.2/arq_django_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arq-django-admin
-Version: 0.3.1
+Version: 0.3.2
 Summary: An app that provides Django admin for ARQ
 Home-page: https://github.com/SlavaSkvortsov/arq-django-admin
 Author: Slava Skvortsov
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arq-django-admin-0.3.1/arq_django_admin.egg-info/SOURCES.txt` & `arq-django-admin-0.3.2/arq_django_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/setup.cfg` & `arq-django-admin-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.3.1/setup.py` & `arq-django-admin-0.3.2/setup.py`

 * *Files identical despite different names*

