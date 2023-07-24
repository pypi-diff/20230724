# Comparing `tmp/djangoldp_contact-2.1.4.tar.gz` & `tmp/djangoldp_contact-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_contact-2.1.4.tar", last modified: Tue Apr 27 15:42:33 2021, max compression
+gzip compressed data, was "djangoldp_contact-3.0.0.tar", last modified: Mon Jul 24 20:55:21 2023, max compression
```

## Comparing `djangoldp_contact-2.1.4.tar` & `djangoldp_contact-3.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:42:33.000000 djangoldp_contact-2.1.4/
--rw-rw-rw-   0 root         (0) root         (0)      579 2021-04-27 15:42:33.000000 djangoldp_contact-2.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       21 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:42:33.000000 djangoldp_contact-2.1.4/djangoldp_contact/
--rw-rw-rw-   0 root         (0) root         (0)       33 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1376 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/models.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:42:33.000000 djangoldp_contact-2.1.4/djangoldp_contact/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4307 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:42:33.000000 djangoldp_contact-2.1.4/djangoldp_contact/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      654 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/migrations/0002_auto_20201208_1157.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/migrations/0003_auto_20210218_1145.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/djangoldp_contact/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2021-04-27 15:42:31.000000 djangoldp_contact-2.1.4/djangoldp_contact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-04-27 15:42:13.000000 djangoldp_contact-2.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:42:33.000000 djangoldp_contact-2.1.4/djangoldp_contact.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-27 15:42:32.000000 djangoldp_contact-2.1.4/djangoldp_contact.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2021-04-27 15:42:32.000000 djangoldp_contact-2.1.4/djangoldp_contact.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2021-04-27 15:42:32.000000 djangoldp_contact-2.1.4/djangoldp_contact.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      750 2021-04-27 15:42:32.000000 djangoldp_contact-2.1.4/djangoldp_contact.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      300 2021-04-27 15:42:32.000000 djangoldp_contact-2.1.4/djangoldp_contact.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      300 2021-04-27 15:42:33.000000 djangoldp_contact-2.1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:55:21.774777 djangoldp_contact-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      261 2023-07-24 20:55:21.778777 djangoldp_contact-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:55:21.774777 djangoldp_contact-3.0.0/djangoldp_contact/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 20:55:19.000000 djangoldp_contact-3.0.0/djangoldp_contact/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/check_integrity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:55:21.774777 djangoldp_contact-3.0.0/djangoldp_contact/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/migrations/0002_auto_20201208_1157.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/migrations/0003_auto_20210218_1145.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:55:21.774777 djangoldp_contact-3.0.0/djangoldp_contact/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/djangoldp_contact/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:55:21.774777 djangoldp_contact-3.0.0/djangoldp_contact.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      261 2023-07-24 20:55:21.000000 djangoldp_contact-3.0.0/djangoldp_contact.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-24 20:55:21.000000 djangoldp_contact-3.0.0/djangoldp_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:55:21.000000 djangoldp_contact-3.0.0/djangoldp_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-24 20:55:21.000000 djangoldp_contact-3.0.0/djangoldp_contact.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 20:55:21.000000 djangoldp_contact-3.0.0/djangoldp_contact.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-24 20:55:21.778777 djangoldp_contact-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 20:55:01.000000 djangoldp_contact-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_contact-2.1.4/setup.cfg` & `djangoldp_contact-3.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 author_email = jbaptiste@startinblox.com
 description = djangoldp package for circle data models
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.1
-	djangoldp_account~=2.1
-	djangoldp_notification~=2.1
+	djangoldp~=3.0
+	djangoldp_account~=3.0
+	djangoldp_notification~=3.0
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_contact/__init__.py:__version__
 commit_parser = commit_parser.parse
 
 [egg_info]
```

### Comparing `djangoldp_contact-2.1.4/djangoldp_contact/models.py` & `djangoldp_contact-3.0.0/djangoldp_contact/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.db.models.signals import post_save
 from django.dispatch import receiver
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from djangoldp.fields import LDPUrlField
 from djangoldp.models import Model
 from djangoldp_contact.views import ContactViewSet
 from djangoldp_notification.models import Notification
 
 
 class Contact(Model):
```

### Comparing `djangoldp_contact-2.1.4/djangoldp_contact/check_integrity.py` & `djangoldp_contact-3.0.0/djangoldp_contact/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-2.1.4/djangoldp_contact/admin.py` & `djangoldp_contact-3.0.0/djangoldp_contact/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp.models import Model
 from .models import Contact
 
 
+@admin.register(Contact)
 class ContactAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'user', 'contact')
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     search_fields = ['urlid', 'user__urlid', 'contact__urlid']
     ordering = ['urlid']
 
     def get_queryset(self, request):
         # Hide distant contacts
         queryset = super(ContactAdmin, self).get_queryset(request)
         internal_ids = [x.pk for x in queryset if not Model.is_external(x)]
         return queryset.filter(pk__in=internal_ids)
 
 
-admin.site.register(Contact, ContactAdmin)
```

### Comparing `djangoldp_contact-2.1.4/djangoldp_contact/tests/tests_permissions.py` & `djangoldp_contact-3.0.0/djangoldp_contact/tests/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-2.1.4/djangoldp_contact/tests/runner.py` & `djangoldp_contact-3.0.0/djangoldp_contact/tests/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import sys
 import yaml
 
 import django
 from django.conf import settings as django_settings
 from djangoldp.conf.ldpsettings import LDPSettings
-from djangoldp.tests.settings_default import yaml_config
-
+from djangoldp.tests.server_settings import yaml_config
 # override config loading
 config = {
     # add the packages to the reference list
     'ldppackages': ['djangoldp_account', 'djangoldp_notification', 'djangoldp_contact', 'djangoldp_contact.tests'],
 
     # required values for server
     'server': {
+        'SECRET_KEY': "$r&)p-4k@h5b!1yrft6&q%j)_p$lxqh6#)jeeu0z1iag&y&wdu",
         'AUTH_USER_MODEL': 'djangoldp_account.LDPUser',
         'REST_FRAMEWORK': {
             'DEFAULT_PAGINATION_CLASS': 'djangoldp.pagination.LDPPagination',
             'PAGE_SIZE': 5
         },
         # map the config of the core settings (avoid asserts to fail)
         'SITE_URL': 'http://happy-dev.fr',
```

### Comparing `djangoldp_contact-2.1.4/djangoldp_contact/migrations/0002_auto_20201208_1157.py` & `djangoldp_contact-3.0.0/djangoldp_contact/migrations/0002_auto_20201208_1157.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-2.1.4/djangoldp_contact/migrations/0001_initial.py` & `djangoldp_contact-3.0.0/djangoldp_contact/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-2.1.4/djangoldp_contact.egg-info/SOURCES.txt` & `djangoldp_contact-3.0.0/djangoldp_contact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

