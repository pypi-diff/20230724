# Comparing `tmp/django-simple-sso.naudit-1.2.1.tar.gz` & `tmp/django-simple-sso.naudit-1.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-sso.naudit-1.2.1.tar", last modified: Wed Jul 19 15:09:01 2023, max compression
+gzip compressed data, was "django-simple-sso.naudit-1.2.1.1.tar", last modified: Mon Jul 24 09:47:37 2023, max compression
```

## Comparing `django-simple-sso.naudit-1.2.1.tar` & `django-simple-sso.naudit-1.2.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10335 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8967 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.710353 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10335 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-19 15:09:01.000000 django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.710353 django-simple-sso.naudit-1.2.1/simple_sso/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.710353 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_client/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.710353 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0002_consumer_name_max_length.py
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0003_token_redirect_to_max_length.py
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0003_token_session.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2289 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8499 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/sso_server/server.py
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/simple_sso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:09:01.714353 django-simple-sso.naudit-1.2.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-07-19 15:08:50.000000 django-simple-sso.naudit-1.2.1/tests/utils/context_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:37.918296 django-simple-sso.naudit-1.2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10337 2023-07-24 09:47:37.918296 django-simple-sso.naudit-1.2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8967 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:37.910296 django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10337 2023-07-24 09:47:37.000000 django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-07-24 09:47:37.000000 django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 09:47:37.000000 django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 09:47:37.000000 django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-24 09:47:37.000000 django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-24 09:47:37.000000 django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-24 09:47:37.918296 django-simple-sso.naudit-1.2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:37.910296 django-simple-sso.naudit-1.2.1.1/simple_sso/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:37.910296 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_client/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_client/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_client/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:37.914296 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:37.914296 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1833 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/migrations/0002_consumer_name_max_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/migrations/0003_token_redirect_to_max_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/migrations/0004_token_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2289 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8499 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/simple_sso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:37.914296 django-simple-sso.naudit-1.2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:37.918296 django-simple-sso.naudit-1.2.1.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-07-24 09:47:28.000000 django-simple-sso.naudit-1.2.1.1/tests/utils/context_managers.py
```

### Comparing `django-simple-sso.naudit-1.2.1/LICENSE` & `django-simple-sso.naudit-1.2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/PKG-INFO` & `django-simple-sso.naudit-1.2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-sso.naudit
-Version: 1.2.1
+Version: 1.2.1.1
 Summary: Simple SSO for Django
 Home-page: http://github.com/naudit/django-simple-sso
 Author: Rafael Leira
 Author-email: rafael.leira@naudit.es
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-simple-sso.naudit-1.2.1/README.rst` & `django-simple-sso.naudit-1.2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/PKG-INFO` & `django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-sso.naudit
-Version: 1.2.1
+Version: 1.2.1.1
 Summary: Simple SSO for Django
 Home-page: http://github.com/naudit/django-simple-sso
 Author: Rafael Leira
 Author-email: rafael.leira@naudit.es
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-simple-sso.naudit-1.2.1/django_simple_sso.naudit.egg-info/SOURCES.txt` & `django-simple-sso.naudit-1.2.1.1/django_simple_sso.naudit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 simple_sso/sso_server/__init__.py
 simple_sso/sso_server/apps.py
 simple_sso/sso_server/models.py
 simple_sso/sso_server/server.py
 simple_sso/sso_server/migrations/0001_initial.py
 simple_sso/sso_server/migrations/0002_consumer_name_max_length.py
 simple_sso/sso_server/migrations/0003_token_redirect_to_max_length.py
-simple_sso/sso_server/migrations/0003_token_session.py
+simple_sso/sso_server/migrations/0004_token_session.py
 simple_sso/sso_server/migrations/__init__.py
 tests/__init__.py
 tests/settings.py
 tests/test_core.py
 tests/test_migrations.py
 tests/urls.py
 tests/utils/__init__.py
```

### Comparing `django-simple-sso.naudit-1.2.1/setup.py` & `django-simple-sso.naudit-1.2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/simple_sso/signals.py` & `django-simple-sso.naudit-1.2.1.1/simple_sso/signals.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/simple_sso/sso_client/client.py` & `django-simple-sso.naudit-1.2.1.1/simple_sso/sso_client/client.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/simple_sso/sso_client/middleware.py` & `django-simple-sso.naudit-1.2.1.1/simple_sso/sso_client/middleware.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0001_initial.py` & `django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/simple_sso/sso_server/migrations/0003_token_session.py` & `django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/migrations/0004_token_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('sessions', '0001_initial'),
-        ('sso_server', '0002_consumer_name_max_length'),
+        ('sso_server', '0003_token_redirect_to_max_length'),
     ]
 
     operations = [
         migrations.AddField(
             model_name='token',
             name='session',
             field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='sessions.session'),
```

### Comparing `django-simple-sso.naudit-1.2.1/simple_sso/sso_server/models.py` & `django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/models.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/simple_sso/sso_server/server.py` & `django-simple-sso.naudit-1.2.1.1/simple_sso/sso_server/server.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/tests/settings.py` & `django-simple-sso.naudit-1.2.1.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/tests/test_core.py` & `django-simple-sso.naudit-1.2.1.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/tests/test_migrations.py` & `django-simple-sso.naudit-1.2.1.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/tests/urls.py` & `django-simple-sso.naudit-1.2.1.1/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-simple-sso.naudit-1.2.1/tests/utils/context_managers.py` & `django-simple-sso.naudit-1.2.1.1/tests/utils/context_managers.py`

 * *Files identical despite different names*

