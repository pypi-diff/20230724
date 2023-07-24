# Comparing `tmp/django-model-tracker-2.0.4b1.tar.gz` & `tmp/django-model-tracker-2.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-model-tracker-2.0.4b1.tar", last modified: Mon Jul 24 14:49:22 2023, max compression
+gzip compressed data, was "django-model-tracker-2.1.0b1.tar", last modified: Thu Jan  5 18:45:57 2023, max compression
```

## Comparing `django-model-tracker-2.0.4b1.tar` & `django-model-tracker-2.1.0b1.tar`

### file list

```diff
@@ -1,38 +1,71 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1085 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       82 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/MANIFEST.in
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/ModelTracker/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7640 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/ModelTracker/Tracker.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/ModelTracker/__init__.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/ModelTracker/management/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/ModelTracker/management/__init__.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/ModelTracker/management/commands/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/ModelTracker/management/commands/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1851 2022-02-15 13:46:15.000000 django-model-tracker-2.0.4b1/ModelTracker/management/commands/restoreObject.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      316 2023-07-24 14:49:11.000000 django-model-tracker-2.0.4b1/ModelTracker/middleware.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/ModelTracker/migrations/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1027 2022-12-19 11:52:41.000000 django-model-tracker-2.0.4b1/ModelTracker/migrations/0001_initial.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      576 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/ModelTracker/migrations/0002_auto_20160929_0517.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      718 2022-12-19 11:11:02.000000 django-model-tracker-2.0.4b1/ModelTracker/migrations/0003_history_related_objects.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/ModelTracker/migrations/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      730 2022-12-19 11:52:56.000000 django-model-tracker-2.0.4b1/ModelTracker/models.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.429233 django-model-tracker-2.0.4b1/ModelTracker/static/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/ModelTracker/static/ModelTracker/
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)   140427 2020-06-01 14:18:42.000000 django-model-tracker-2.0.4b1/ModelTracker/static/ModelTracker/bootstrap.min.css
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)    86663 2020-06-01 14:18:42.000000 django-model-tracker-2.0.4b1/ModelTracker/static/ModelTracker/jquery-3.2.1.min.js
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/ModelTracker/templates/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      797 2022-02-03 07:57:08.000000 django-model-tracker-2.0.4b1/ModelTracker/templates/changes.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2388 2022-02-15 13:28:58.000000 django-model-tracker-2.0.4b1/ModelTracker/templates/main.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      376 2022-12-19 10:55:53.000000 django-model-tracker-2.0.4b1/ModelTracker/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6875 2022-02-15 13:46:04.000000 django-model-tracker-2.0.4b1/ModelTracker/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4927 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3126 2022-12-19 10:32:18.000000 django-model-tracker-2.0.4b1/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/django_model_tracker.egg-info/
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)     4927 2023-07-24 14:49:22.000000 django-model-tracker-2.0.4b1/django_model_tracker.egg-info/PKG-INFO
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)      929 2023-07-24 14:49:22.000000 django-model-tracker-2.0.4b1/django_model_tracker.egg-info/SOURCES.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)        1 2023-07-24 14:49:22.000000 django-model-tracker-2.0.4b1/django_model_tracker.egg-info/dependency_links.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)        1 2020-07-06 07:49:50.000000 django-model-tracker-2.0.4b1/django_model_tracker.egg-info/not-zip-safe
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)       23 2023-07-24 14:49:22.000000 django-model-tracker-2.0.4b1/django_model_tracker.egg-info/requires.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)       13 2023-07-24 14:49:22.000000 django-model-tracker-2.0.4b1/django_model_tracker.egg-info/top_level.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-07-24 14:49:22.433233 django-model-tracker-2.0.4b1/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2645 2023-07-24 14:49:11.000000 django-model-tracker-2.0.4b1/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.173306 django-model-tracker-2.1.0b1/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1085 2016-06-13 12:01:36.000000 django-model-tracker-2.1.0b1/LICENSE
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       82 2020-06-01 14:18:42.000000 django-model-tracker-2.1.0b1/MANIFEST.in
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/ModelTracker/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     7640 2021-06-22 10:06:25.000000 django-model-tracker-2.1.0b1/ModelTracker/Tracker.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        0 2020-06-01 14:18:42.000000 django-model-tracker-2.1.0b1/ModelTracker/__init__.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/ModelTracker/management/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        0 2018-09-07 15:25:35.000000 django-model-tracker-2.1.0b1/ModelTracker/management/__init__.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/ModelTracker/management/commands/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        0 2018-09-07 15:25:35.000000 django-model-tracker-2.1.0b1/ModelTracker/management/commands/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1851 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/ModelTracker/management/commands/restoreObject.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      377 2023-01-05 18:28:50.000000 django-model-tracker-2.1.0b1/ModelTracker/middleware.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/ModelTracker/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1027 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/ModelTracker/migrations/0001_initial.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      576 2018-07-04 17:12:56.000000 django-model-tracker-2.1.0b1/ModelTracker/migrations/0002_auto_20160929_0517.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      718 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/ModelTracker/migrations/0003_history_related_objects.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      553 2023-01-05 18:41:12.000000 django-model-tracker-2.1.0b1/ModelTracker/migrations/0004_auto_20230105_1841.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2016-06-13 12:01:36.000000 django-model-tracker-2.1.0b1/ModelTracker/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      730 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/ModelTracker/models.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/ModelTracker/static/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/ModelTracker/static/ModelTracker/
+-rwxr-xr-x   0 mohamed   (1000) mohamed   (1000)   140427 2020-06-01 14:18:42.000000 django-model-tracker-2.1.0b1/ModelTracker/static/ModelTracker/bootstrap.min.css
+-rwxr-xr-x   0 mohamed   (1000) mohamed   (1000)    86663 2020-06-01 14:18:42.000000 django-model-tracker-2.1.0b1/ModelTracker/static/ModelTracker/jquery-3.2.1.min.js
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/ModelTracker/templates/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      797 2020-07-06 07:46:24.000000 django-model-tracker-2.1.0b1/ModelTracker/templates/changes.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2388 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/ModelTracker/templates/main.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      376 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/ModelTracker/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6875 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/ModelTracker/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4927 2023-01-05 18:45:57.173306 django-model-tracker-2.1.0b1/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3126 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/TestApp3/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     7640 2021-06-22 10:06:25.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/Tracker.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        0 2020-06-01 14:18:42.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/__init__.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/management/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        0 2018-09-07 15:25:35.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/management/__init__.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/management/commands/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        0 2018-09-07 15:25:35.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/management/commands/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1851 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/management/commands/restoreObject.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      377 2023-01-05 18:28:50.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/middleware.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.169306 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1027 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/migrations/0001_initial.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      576 2018-07-04 17:12:56.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/migrations/0002_auto_20160929_0517.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      718 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/migrations/0003_history_related_objects.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      553 2023-01-05 18:41:12.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/migrations/0004_auto_20230105_1841.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2016-06-13 12:01:36.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      730 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/models.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      376 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6875 2023-01-05 18:25:18.000000 django-model-tracker-2.1.0b1/TestApp3/ModelTracker/views.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.173306 django-model-tracker-2.1.0b1/TestApp3/TestApp3/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:35:59.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      393 2023-01-05 18:35:59.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/asgi.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.173306 django-model-tracker-2.1.0b1/TestApp3/TestApp3/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-01-05 18:41:40.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/migrations/0001_initial.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:40:59.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      220 2016-06-13 12:01:36.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/models.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3331 2023-01-05 18:38:24.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/settings.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      813 2023-01-05 18:39:28.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      350 2023-01-05 18:38:48.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      393 2023-01-05 18:35:59.000000 django-model-tracker-2.1.0b1/TestApp3/TestApp3/wsgi.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:41:29.000000 django-model-tracker-2.1.0b1/TestApp3/__init__.py
+-rwxrwxr-x   0 mohamed   (1000) mohamed   (1000)      664 2023-01-05 18:35:59.000000 django-model-tracker-2.1.0b1/TestApp3/manage.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-01-05 18:45:57.173306 django-model-tracker-2.1.0b1/django_model_tracker.egg-info/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     4927 2023-01-05 18:45:57.000000 django-model-tracker-2.1.0b1/django_model_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1932 2023-01-05 18:45:57.000000 django-model-tracker-2.1.0b1/django_model_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2023-01-05 18:45:57.000000 django-model-tracker-2.1.0b1/django_model_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2020-07-06 07:49:50.000000 django-model-tracker-2.1.0b1/django_model_tracker.egg-info/not-zip-safe
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       23 2023-01-05 18:45:57.000000 django-model-tracker-2.1.0b1/django_model_tracker.egg-info/requires.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       22 2023-01-05 18:45:57.000000 django-model-tracker-2.1.0b1/django_model_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-01-05 18:45:57.173306 django-model-tracker-2.1.0b1/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2645 2023-01-05 18:45:34.000000 django-model-tracker-2.1.0b1/setup.py
```

### Comparing `django-model-tracker-2.0.4b1/LICENSE` & `django-model-tracker-2.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/Tracker.py` & `django-model-tracker-2.1.0b1/ModelTracker/Tracker.py`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/management/commands/restoreObject.py` & `django-model-tracker-2.1.0b1/ModelTracker/management/commands/restoreObject.py`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/migrations/0001_initial.py` & `django-model-tracker-2.1.0b1/ModelTracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/migrations/0002_auto_20160929_0517.py` & `django-model-tracker-2.1.0b1/ModelTracker/migrations/0002_auto_20160929_0517.py`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/migrations/0003_history_related_objects.py` & `django-model-tracker-2.1.0b1/ModelTracker/migrations/0003_history_related_objects.py`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/models.py` & `django-model-tracker-2.1.0b1/ModelTracker/models.py`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/static/ModelTracker/bootstrap.min.css` & `django-model-tracker-2.1.0b1/ModelTracker/static/ModelTracker/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/static/ModelTracker/jquery-3.2.1.min.js` & `django-model-tracker-2.1.0b1/ModelTracker/static/ModelTracker/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/templates/changes.html` & `django-model-tracker-2.1.0b1/ModelTracker/templates/changes.html`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/templates/main.html` & `django-model-tracker-2.1.0b1/ModelTracker/templates/main.html`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/ModelTracker/views.py` & `django-model-tracker-2.1.0b1/ModelTracker/views.py`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/PKG-INFO` & `django-model-tracker-2.1.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-tracker
-Version: 2.0.4b1
+Version: 2.1.0b1
 Summary: Track Django Model Objects over time
 Home-page: https://github.com/mkalioby/ModelTracker/
 Download-URL: https://github.com/mkalioby/ModelTracker/
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-model-tracker-2.0.4b1/README.md` & `django-model-tracker-2.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `django-model-tracker-2.0.4b1/django_model_tracker.egg-info/PKG-INFO` & `django-model-tracker-2.1.0b1/django_model_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-tracker
-Version: 2.0.4b1
+Version: 2.1.0b1
 Summary: Track Django Model Objects over time
 Home-page: https://github.com/mkalioby/ModelTracker/
 Download-URL: https://github.com/mkalioby/ModelTracker/
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-model-tracker-2.0.4b1/setup.py` & `django-model-tracker-2.1.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 #    )
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-model-tracker',
-    version='2.0.4b1',
+    version='2.1.0b1',
     description='Track Django Model Objects over time',
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/ModelTracker/',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

