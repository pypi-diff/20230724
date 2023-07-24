# Comparing `tmp/django-tabular-permissions-2.9.1.tar.gz` & `tmp/django-tabular-permissions-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tabular-permissions-2.9.1.tar", last modified: Tue Jun  7 06:43:48 2022, max compression
+gzip compressed data, was "django-tabular-permissions-2.9.2.tar", last modified: Mon Jul 24 20:10:29 2023, max compression
```

## Comparing `django-tabular-permissions-2.9.1.tar` & `django-tabular-permissions-2.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     1296 2015-12-09 21:00:08.000000 django-tabular-permissions-2.9.1/LICENSE
--rw-r--r--   0 ramez     (1000) ramez     (1000)      179 2018-10-08 05:14:58.000000 django-tabular-permissions-2.9.1/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8846 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7720 2022-06-07 06:39:22.000000 django-tabular-permissions-2.9.1/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/django_tabular_permissions.egg-info/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     8846 2022-06-07 06:43:47.000000 django-tabular-permissions-2.9.1/django_tabular_permissions.egg-info/PKG-INFO
--rw-r--r--   0 ramez     (1000) ramez     (1000)      653 2022-06-07 06:43:48.000000 django-tabular-permissions-2.9.1/django_tabular_permissions.egg-info/SOURCES.txt
--rw-r--r--   0 ramez     (1000) ramez     (1000)        1 2022-06-07 06:43:47.000000 django-tabular-permissions-2.9.1/django_tabular_permissions.egg-info/dependency_links.txt
--rw-r--r--   0 ramez     (1000) ramez     (1000)       20 2022-06-07 06:43:48.000000 django-tabular-permissions-2.9.1/django_tabular_permissions.egg-info/top_level.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       38 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1481 2022-06-07 06:41:28.000000 django-tabular-permissions-2.9.1/setup.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2022-06-07 06:38:07.000000 django-tabular-permissions-2.9.1/tabular_permissions/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2134 2022-06-07 06:36:24.000000 django-tabular-permissions-2.9.1/tabular_permissions/admin.py
--rw-r--r--   0 ramez     (1000) ramez     (1000)     2101 2020-09-15 11:02:36.000000 django-tabular-permissions-2.9.1/tabular_permissions/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1344 2022-06-07 06:36:24.000000 django-tabular-permissions-2.9.1/tabular_permissions/helpers.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/locale/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/locale/ar/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/locale/ar/LC_MESSAGES/
--rw-r--r--   0 ramez     (1000) ramez     (1000)      642 2018-06-30 16:09:27.000000 django-tabular-permissions-2.9.1/tabular_permissions/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 ramez     (1000) ramez     (1000)     1039 2018-06-30 16:09:27.000000 django-tabular-permissions-2.9.1/tabular_permissions/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/static/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/static/tabular_permissions/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2404 2019-07-25 12:41:51.000000 django-tabular-permissions-2.9.1/tabular_permissions/static/tabular_permissions/tabular_permissions.js
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/templates/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/templates/tabular_permissions/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2022-06-07 06:43:48.314442 django-tabular-permissions-2.9.1/tabular_permissions/templates/tabular_permissions/admin/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     7041 2020-02-01 07:47:30.000000 django-tabular-permissions-2.9.1/tabular_permissions/templates/tabular_permissions/admin/tabular_permissions.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8512 2022-06-07 06:36:24.000000 django-tabular-permissions-2.9.1/tabular_permissions/widgets.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.136889 django-tabular-permissions-2.9.2/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     1296 2015-12-09 21:00:08.000000 django-tabular-permissions-2.9.2/LICENSE
+-rw-r--r--   0 ramez     (1000) ramez     (1000)      179 2018-10-08 05:14:58.000000 django-tabular-permissions-2.9.2/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8938 2023-07-24 20:10:29.136889 django-tabular-permissions-2.9.2/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7680 2023-07-24 19:50:21.000000 django-tabular-permissions-2.9.2/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     8938 2023-07-24 20:10:29.000000 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/PKG-INFO
+-rw-r--r--   0 ramez     (1000) ramez     (1000)      653 2023-07-24 20:10:29.000000 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/SOURCES.txt
+-rw-r--r--   0 ramez     (1000) ramez     (1000)        1 2023-07-24 20:10:29.000000 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/dependency_links.txt
+-rw-r--r--   0 ramez     (1000) ramez     (1000)       20 2023-07-24 20:10:29.000000 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/top_level.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       38 2023-07-24 20:10:29.136889 django-tabular-permissions-2.9.2/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1630 2023-07-24 20:10:27.000000 django-tabular-permissions-2.9.2/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-07-24 19:34:42.000000 django-tabular-permissions-2.9.2/tabular_permissions/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2261 2023-07-24 13:22:48.000000 django-tabular-permissions-2.9.2/tabular_permissions/admin.py
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     2101 2020-09-15 11:02:36.000000 django-tabular-permissions-2.9.2/tabular_permissions/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1344 2022-06-07 06:36:24.000000 django-tabular-permissions-2.9.2/tabular_permissions/helpers.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/locale/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)      642 2018-06-30 16:09:27.000000 django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     1039 2018-06-30 16:09:27.000000 django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/static/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/static/tabular_permissions/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2404 2019-07-25 12:41:51.000000 django-tabular-permissions-2.9.2/tabular_permissions/static/tabular_permissions/tabular_permissions.js
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/templates/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/templates/tabular_permissions/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.136889 django-tabular-permissions-2.9.2/tabular_permissions/templates/tabular_permissions/admin/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     7041 2020-02-01 07:47:30.000000 django-tabular-permissions-2.9.2/tabular_permissions/templates/tabular_permissions/admin/tabular_permissions.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8512 2022-06-07 06:36:24.000000 django-tabular-permissions-2.9.2/tabular_permissions/widgets.py
```

### Comparing `django-tabular-permissions-2.9.1/LICENSE` & `django-tabular-permissions-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.1/PKG-INFO` & `django-tabular-permissions-2.9.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,46 @@
-Metadata-Version: 2.1
-Name: django-tabular-permissions
-Version: 2.9.1
-Summary: Display django permissions in a tabular format that is user friendly, and highly customisable
-Home-page: https://github.com/RamezIssac/django-tabular-permissions
-Author: Ramez Ashraf
-Author-email: ramez@rasystems.io
-License: BSD License
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-License-File: LICENSE
 
 django-tabular-permissions
 ##########################
-Display model permissions in a tabular widget that is user friendly, translatable and customizable.
-*Scroll down for screen shots*
+Display django permissions in a user friendly, translatable and customizable widget .
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_1.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_1.png
+    :alt: Basic demo
+
+RTL and localized
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
+    :alt: RTL and localized
+
+With Custom permission behaviour
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
+    :alt: With Custom permission
+
 
 Version
 -------
 2.9.1 (June 7 2022)
 
 Features:
 ---------
 * Permissions and their relevant app and models names are displayed in the active language.
 * Permissions are displayed in a table that contain the default model permissions **plus** any custom permissions.
 * Supports view permission (started with Django 2).
 * Customize which apps, models to show in the permissions table. You can also set a exclude function for high-end customization.
 * RTL ready, Bootstrap ready.
 * Easy customize-able look.
-* Python 2.7, 3.6, 3.7 & 3.8. Django 1.11, 2.1, 2.2, 3.0, 3.1, 3.2 , 4.0 .
+* Python 2.7, 3.6, 3.7, 3.8, 3.9 , 3.10. Django 1.11, 2.1, 2.2, 3.0, 3.1, 3.2 , 4.0, 4.1, 4.2
 * Default `FilteredSelectMultiple` widget will appear only if you have custom permissions that are not model related (ie directly created by code or hand)
 
 
 
-.. image:: https://travis-ci.org/RamezIssac/django-tabular-permissions.svg?branch=master
-    :target: https://travis-ci.org/RamezIssac/django-tabular-permissions
-
-
 Installation
 ------------
 You can install `django-tabular-permissions` via Pypi::
 
     pip install django-tabular-permissions
 
 
@@ -71,15 +57,15 @@
     python manage.py collectstatic
 
 
 then navigate to User and/or Group change form to see `tabular_permissions` in action.
 
 Configuration:
 --------------
-Tabular_permissions possible configurations and their default::
+Tabular permissions possible configurations and their default::
 
     TABULAR_PERMISSIONS_CONFIG = {
         'template': 'tabular_permissions/admin/tabular_permissions.html',
         'exclude': {
             'override': False,
             'apps': [],
             'models': [],
@@ -147,59 +133,48 @@
 
 1. Upon form submit, the checked permissions in the table are dynamically appended to the form default permission input so the backend can carry on its functionality normally and correctly.
 2. Add handlers for column and row `select-all` checkboxes.
 
 
 Compatibility:
 --------------
-Version >= 2.0  only supports Django >= 1.11
-For earlier versions of django use django-tabular-permissions 1.0.9.
-
-
-Screenshots:
-------------
-Basic Demo
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_1.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_1.png
-    :alt: Basic demo
-
-RTL and localized
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
-    :alt: RTL and localized
-
-With Custom permission behaviour
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
-    :alt: With Custom permission
-
--------
+Current version support from Python 2.7 and up to Python 3.10, and Django from 1.11 to 4.1
+For Django < 1.11, use django-tabular-permissions 1.0.9.
 
 Demo:
 -----
 
 To run the demo project in the repo on your local you need
 
 1. Clone the repo;
 2. Create a virtualenv
 3. `pip install django-tabular-permissions`
 4. `python manage.py migrate`
 5. `python manage.py runserver`
 
-Enjoy and feel free to report any bugs or make pull requests.
 
-Cheers ;-)
+Tests
+-----
+
+To run the tests, you need to install the test requirements::
+
+    cd tests
+    pip install -r requirements.txt
+
+Then run::
+
+    python runtests.py
+
+With Coverage ::
+
+        coverage run runtests.py
+        coverage html
+
 
 Cross Reference
 ---------------
 
 If you like this package, chances are you may like those packages too!
 
 `Django Slick Reporting <https://github.com/ra-systems/django-slick-reporting>`_ Powerful and Efficient reporting engine with Charting capabilities.
 
 `Django Ra ERP Framework <https://github.com/ra-systems/RA>`_ A framework to build business solutions with ease.
-
-
-
```

### Comparing `django-tabular-permissions-2.9.1/README.rst` & `django-tabular-permissions-2.9.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,75 @@
+Metadata-Version: 2.1
+Name: django-tabular-permissions
+Version: 2.9.2
+Summary: Display django permissions in a tabular format that is user friendly, and highly customisable
+Home-page: https://github.com/RamezIssac/django-tabular-permissions
+Author: Ramez Ashraf
+Author-email: ramez@rasystems.io
+License: BSD License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+
 django-tabular-permissions
 ##########################
-Display model permissions in a tabular widget that is user friendly, translatable and customizable.
-*Scroll down for screen shots*
+Display django permissions in a user friendly, translatable and customizable widget .
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_1.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_1.png
+    :alt: Basic demo
+
+RTL and localized
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
+    :alt: RTL and localized
+
+With Custom permission behaviour
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
+    :alt: With Custom permission
+
 
 Version
 -------
 2.9.1 (June 7 2022)
 
 Features:
 ---------
 * Permissions and their relevant app and models names are displayed in the active language.
 * Permissions are displayed in a table that contain the default model permissions **plus** any custom permissions.
 * Supports view permission (started with Django 2).
 * Customize which apps, models to show in the permissions table. You can also set a exclude function for high-end customization.
 * RTL ready, Bootstrap ready.
 * Easy customize-able look.
-* Python 2.7, 3.6, 3.7 & 3.8. Django 1.11, 2.1, 2.2, 3.0, 3.1, 3.2 , 4.0 .
+* Python 2.7, 3.6, 3.7, 3.8, 3.9 , 3.10. Django 1.11, 2.1, 2.2, 3.0, 3.1, 3.2 , 4.0, 4.1, 4.2
 * Default `FilteredSelectMultiple` widget will appear only if you have custom permissions that are not model related (ie directly created by code or hand)
 
 
 
-.. image:: https://travis-ci.org/RamezIssac/django-tabular-permissions.svg?branch=master
-    :target: https://travis-ci.org/RamezIssac/django-tabular-permissions
-
-
 Installation
 ------------
 You can install `django-tabular-permissions` via Pypi::
 
     pip install django-tabular-permissions
 
 
@@ -44,15 +86,15 @@
     python manage.py collectstatic
 
 
 then navigate to User and/or Group change form to see `tabular_permissions` in action.
 
 Configuration:
 --------------
-Tabular_permissions possible configurations and their default::
+Tabular permissions possible configurations and their default::
 
     TABULAR_PERMISSIONS_CONFIG = {
         'template': 'tabular_permissions/admin/tabular_permissions.html',
         'exclude': {
             'override': False,
             'apps': [],
             'models': [],
@@ -120,57 +162,48 @@
 
 1. Upon form submit, the checked permissions in the table are dynamically appended to the form default permission input so the backend can carry on its functionality normally and correctly.
 2. Add handlers for column and row `select-all` checkboxes.
 
 
 Compatibility:
 --------------
-Version >= 2.0  only supports Django >= 1.11
-For earlier versions of django use django-tabular-permissions 1.0.9.
-
-
-Screenshots:
-------------
-Basic Demo
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_1.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_1.png
-    :alt: Basic demo
-
-RTL and localized
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
-    :alt: RTL and localized
-
-With Custom permission behaviour
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
-    :alt: With Custom permission
-
--------
+Current version support from Python 2.7 and up to Python 3.10, and Django from 1.11 to 4.1
+For Django < 1.11, use django-tabular-permissions 1.0.9.
 
 Demo:
 -----
 
 To run the demo project in the repo on your local you need
 
 1. Clone the repo;
 2. Create a virtualenv
 3. `pip install django-tabular-permissions`
 4. `python manage.py migrate`
 5. `python manage.py runserver`
 
-Enjoy and feel free to report any bugs or make pull requests.
 
-Cheers ;-)
+Tests
+-----
+
+To run the tests, you need to install the test requirements::
+
+    cd tests
+    pip install -r requirements.txt
+
+Then run::
+
+    python runtests.py
+
+With Coverage ::
+
+        coverage run runtests.py
+        coverage html
+
 
 Cross Reference
 ---------------
 
 If you like this package, chances are you may like those packages too!
 
 `Django Slick Reporting <https://github.com/ra-systems/django-slick-reporting>`_ Powerful and Efficient reporting engine with Charting capabilities.
 
 `Django Ra ERP Framework <https://github.com/ra-systems/RA>`_ A framework to build business solutions with ease.
-
```

### Comparing `django-tabular-permissions-2.9.1/django_tabular_permissions.egg-info/PKG-INFO` & `django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,75 @@
 Metadata-Version: 2.1
 Name: django-tabular-permissions
-Version: 2.9.1
+Version: 2.9.2
 Summary: Display django permissions in a tabular format that is user friendly, and highly customisable
 Home-page: https://github.com/RamezIssac/django-tabular-permissions
 Author: Ramez Ashraf
 Author-email: ramez@rasystems.io
 License: BSD License
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE
 
+
 django-tabular-permissions
 ##########################
-Display model permissions in a tabular widget that is user friendly, translatable and customizable.
-*Scroll down for screen shots*
+Display django permissions in a user friendly, translatable and customizable widget .
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_1.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_1.png
+    :alt: Basic demo
+
+RTL and localized
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
+    :alt: RTL and localized
+
+With Custom permission behaviour
+
+.. image:: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
+    :target: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
+    :alt: With Custom permission
+
 
 Version
 -------
 2.9.1 (June 7 2022)
 
 Features:
 ---------
 * Permissions and their relevant app and models names are displayed in the active language.
 * Permissions are displayed in a table that contain the default model permissions **plus** any custom permissions.
 * Supports view permission (started with Django 2).
 * Customize which apps, models to show in the permissions table. You can also set a exclude function for high-end customization.
 * RTL ready, Bootstrap ready.
 * Easy customize-able look.
-* Python 2.7, 3.6, 3.7 & 3.8. Django 1.11, 2.1, 2.2, 3.0, 3.1, 3.2 , 4.0 .
+* Python 2.7, 3.6, 3.7, 3.8, 3.9 , 3.10. Django 1.11, 2.1, 2.2, 3.0, 3.1, 3.2 , 4.0, 4.1, 4.2
 * Default `FilteredSelectMultiple` widget will appear only if you have custom permissions that are not model related (ie directly created by code or hand)
 
 
 
-.. image:: https://travis-ci.org/RamezIssac/django-tabular-permissions.svg?branch=master
-    :target: https://travis-ci.org/RamezIssac/django-tabular-permissions
-
-
 Installation
 ------------
 You can install `django-tabular-permissions` via Pypi::
 
     pip install django-tabular-permissions
 
 
@@ -71,15 +86,15 @@
     python manage.py collectstatic
 
 
 then navigate to User and/or Group change form to see `tabular_permissions` in action.
 
 Configuration:
 --------------
-Tabular_permissions possible configurations and their default::
+Tabular permissions possible configurations and their default::
 
     TABULAR_PERMISSIONS_CONFIG = {
         'template': 'tabular_permissions/admin/tabular_permissions.html',
         'exclude': {
             'override': False,
             'apps': [],
             'models': [],
@@ -147,59 +162,48 @@
 
 1. Upon form submit, the checked permissions in the table are dynamically appended to the form default permission input so the backend can carry on its functionality normally and correctly.
 2. Add handlers for column and row `select-all` checkboxes.
 
 
 Compatibility:
 --------------
-Version >= 2.0  only supports Django >= 1.11
-For earlier versions of django use django-tabular-permissions 1.0.9.
-
-
-Screenshots:
-------------
-Basic Demo
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_1.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_1.png
-    :alt: Basic demo
-
-RTL and localized
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_ar.png
-    :alt: RTL and localized
-
-With Custom permission behaviour
-
-.. image:: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
-    :target: https://rasystems.io/static/images/tabular_permissions/tp_extra.png
-    :alt: With Custom permission
-
--------
+Current version support from Python 2.7 and up to Python 3.10, and Django from 1.11 to 4.1
+For Django < 1.11, use django-tabular-permissions 1.0.9.
 
 Demo:
 -----
 
 To run the demo project in the repo on your local you need
 
 1. Clone the repo;
 2. Create a virtualenv
 3. `pip install django-tabular-permissions`
 4. `python manage.py migrate`
 5. `python manage.py runserver`
 
-Enjoy and feel free to report any bugs or make pull requests.
 
-Cheers ;-)
+Tests
+-----
+
+To run the tests, you need to install the test requirements::
+
+    cd tests
+    pip install -r requirements.txt
+
+Then run::
+
+    python runtests.py
+
+With Coverage ::
+
+        coverage run runtests.py
+        coverage html
+
 
 Cross Reference
 ---------------
 
 If you like this package, chances are you may like those packages too!
 
 `Django Slick Reporting <https://github.com/ra-systems/django-slick-reporting>`_ Powerful and Efficient reporting engine with Charting capabilities.
 
 `Django Ra ERP Framework <https://github.com/ra-systems/RA>`_ A framework to build business solutions with ease.
-
-
-
```

### Comparing `django-tabular-permissions-2.9.1/django_tabular_permissions.egg-info/SOURCES.txt` & `django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.1/setup.py` & `django-tabular-permissions-2.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-tabular-permissions',
-    version='2.9.1',
+    version='2.9.2',
     packages=['tabular_permissions'],
     include_package_data=True,
     license='BSD License',
     description='Display django permissions in a tabular format that is user friendly, and highly customisable',
     long_description=README,
     url='https://github.com/RamezIssac/django-tabular-permissions',
     author='Ramez Ashraf',
@@ -29,11 +29,14 @@
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
 )
```

### Comparing `django-tabular-permissions-2.9.1/tabular_permissions/admin.py` & `django-tabular-permissions-2.9.2/tabular_permissions/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,20 @@
                                                     'permissions')
             field.help_text = ''
         return field
 
 
 try:
     UserAdminModel = admin.site._registry[User].__class__
-except:
+except:  # pragma: no cover
     UserAdminModel = DjUserAdmin
 
 try:
     GroupAdminModel = admin.site._registry[Group].__class__
-except:
+except:  # pragma: no cover
     GroupAdminModel = DjGroupAdmin
 
 
 class TabularPermissionsUserAdmin(UserTabularPermissionsMixin, UserAdminModel):
     pass
 
 
@@ -51,9 +51,10 @@
     try:
         admin.site.unregister(User)
         admin.site.register(User, TabularPermissionsUserAdmin)
         admin.site.unregister(Group)
         admin.site.register(Group, TabularPermissionsGroupAdmin)
 
     except:
-        raise ImproperlyConfigured('Please make sure that django.contrib.auth '
-                                   'comes before tabular_permissions in INSTALLED_APPS')
+        raise ImproperlyConfigured(
+            'Please make sure that django.contrib.auth (Or the app containing your custom User model) '
+            'comes before tabular_permissions in INSTALLED_APPS; Or set AUTO_IMPLEMENT to False in your settings.')
```

### Comparing `django-tabular-permissions-2.9.1/tabular_permissions/app_settings.py` & `django-tabular-permissions-2.9.2/tabular_permissions/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.1/tabular_permissions/helpers.py` & `django-tabular-permissions-2.9.2/tabular_permissions/helpers.py`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.1/tabular_permissions/locale/ar/LC_MESSAGES/django.mo` & `django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.1/tabular_permissions/locale/ar/LC_MESSAGES/django.po` & `django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.1/tabular_permissions/static/tabular_permissions/tabular_permissions.js` & `django-tabular-permissions-2.9.2/tabular_permissions/static/tabular_permissions/tabular_permissions.js`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.1/tabular_permissions/templates/tabular_permissions/admin/tabular_permissions.html` & `django-tabular-permissions-2.9.2/tabular_permissions/templates/tabular_permissions/admin/tabular_permissions.html`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.1/tabular_permissions/widgets.py` & `django-tabular-permissions-2.9.2/tabular_permissions/widgets.py`

 * *Files identical despite different names*

