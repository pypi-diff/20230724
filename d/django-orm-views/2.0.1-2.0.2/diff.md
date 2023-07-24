# Comparing `tmp/django-orm-views-2.0.1.tar.gz` & `tmp/django-orm-views-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-orm-views-2.0.1.tar", last modified: Fri Oct 21 14:42:46 2022, max compression
+gzip compressed data, was "django-orm-views-2.0.2.tar", last modified: Mon Jul 24 13:32:48 2023, max compression
```

## Comparing `django-orm-views-2.0.1.tar` & `django-orm-views-2.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 14:42:46.952351 django-orm-views-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7413 2022-10-21 14:42:46.952351 django-orm-views-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5693 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 14:42:46.952351 django-orm-views-2.0.1/django_orm_views/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 14:42:46.952351 django-orm-views-2.0.1/django_orm_views/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 14:42:46.952351 django-orm-views-2.0.1/django_orm_views/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/management/commands/sync_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/not_managed_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/register.py
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     6302 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/django_orm_views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 14:42:46.952351 django-orm-views-2.0.1/django_orm_views.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7413 2022-10-21 14:42:46.000000 django-orm-views-2.0.1/django_orm_views.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-10-21 14:42:46.000000 django-orm-views-2.0.1/django_orm_views.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 14:42:46.000000 django-orm-views-2.0.1/django_orm_views.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 14:42:46.000000 django-orm-views-2.0.1/django_orm_views.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-10-21 14:42:46.000000 django-orm-views-2.0.1/django_orm_views.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-21 14:42:46.000000 django-orm-views-2.0.1/django_orm_views.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 14:42:46.952351 django-orm-views-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-21 14:42:37.000000 django-orm-views-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:32:48.139250 django-orm-views-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-24 13:32:48.139250 django-orm-views-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:32:48.139250 django-orm-views-2.0.2/django_orm_views/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:32:48.139250 django-orm-views-2.0.2/django_orm_views/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:32:48.139250 django-orm-views-2.0.2/django_orm_views/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/management/commands/sync_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/not_managed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/django_orm_views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:32:48.139250 django-orm-views-2.0.2/django_orm_views.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-24 13:32:48.000000 django-orm-views-2.0.2/django_orm_views.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-24 13:32:48.000000 django-orm-views-2.0.2/django_orm_views.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:32:48.000000 django-orm-views-2.0.2/django_orm_views.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:32:47.000000 django-orm-views-2.0.2/django_orm_views.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 13:32:48.000000 django-orm-views-2.0.2/django_orm_views.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 13:32:48.000000 django-orm-views-2.0.2/django_orm_views.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:32:48.139250 django-orm-views-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 13:32:36.000000 django-orm-views-2.0.2/setup.py
```

### Comparing `django-orm-views-2.0.1/LICENSE` & `django-orm-views-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-orm-views-2.0.1/PKG-INFO` & `django-orm-views-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-orm-views
-Version: 2.0.1
+Version: 2.0.2
 Summary: A framework for managing database views based on Django, without the migrations
 Author: iwoca
 Author-email: Josh Dutton <j.dutton@iwoca.co.uk>
 License: Copyright 2022 iwoca Ltd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django-orm-views-2.0.1/README.md` & `django-orm-views-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-orm-views-2.0.1/django_orm_views/management/commands/sync_views.py` & `django-orm-views-2.0.2/django_orm_views/management/commands/sync_views.py`

 * *Files identical despite different names*

### Comparing `django-orm-views-2.0.1/django_orm_views/not_managed_model.py` & `django-orm-views-2.0.2/django_orm_views/not_managed_model.py`

 * *Files identical despite different names*

### Comparing `django-orm-views-2.0.1/django_orm_views/register.py` & `django-orm-views-2.0.2/django_orm_views/register.py`

 * *Files identical despite different names*

### Comparing `django-orm-views-2.0.1/django_orm_views/sync.py` & `django-orm-views-2.0.2/django_orm_views/sync.py`

 * *Files identical despite different names*

### Comparing `django-orm-views-2.0.1/django_orm_views/views.py` & `django-orm-views-2.0.2/django_orm_views/views.py`

 * *Files identical despite different names*

### Comparing `django-orm-views-2.0.1/django_orm_views.egg-info/PKG-INFO` & `django-orm-views-2.0.2/django_orm_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-orm-views
-Version: 2.0.1
+Version: 2.0.2
 Summary: A framework for managing database views based on Django, without the migrations
 Author: iwoca
 Author-email: Josh Dutton <j.dutton@iwoca.co.uk>
 License: Copyright 2022 iwoca Ltd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django-orm-views-2.0.1/django_orm_views.egg-info/SOURCES.txt` & `django-orm-views-2.0.2/django_orm_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-orm-views-2.0.1/pyproject.toml` & `django-orm-views-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-orm-views"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="Josh Dutton", email="j.dutton@iwoca.co.uk" },
 ]
 description = "A framework for managing database views based on Django, without the migrations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `django-orm-views-2.0.1/setup.py` & `django-orm-views-2.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='django_orm_views',
-    version='2.0.1',
+    version='2.0.2',
     description='Package to define manage Postgres views on a Django server',
     author='iwoca',
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     include_package_data=True,
     python_requires='>=3.6',
     install_requires=[
-        'django>=2.1,<4.1',
+        'django>=2.1,<4.2',
         'dataclasses>=0.7; python_version < "3.7.0"',
     ],
     extras_require={
         'test': [
             'psycopg2-binary==2.8.6'
         ]
     },
```

