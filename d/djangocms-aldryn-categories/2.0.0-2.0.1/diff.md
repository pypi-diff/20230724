# Comparing `tmp/djangocms-aldryn-categories-2.0.0.tar.gz` & `tmp/djangocms-aldryn-categories-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-aldryn-categories-2.0.0.tar", last modified: Wed Jul 19 08:53:19 2023, max compression
+gzip compressed data, was "djangocms-aldryn-categories-2.0.1.tar", last modified: Mon Jul 24 09:26:33 2023, max compression
```

## Comparing `djangocms-aldryn-categories-2.0.0.tar` & `djangocms-aldryn-categories-2.0.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.212684 djangocms-aldryn-categories-2.0.0/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1485 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/LICENSE
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      141 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/MANIFEST.in
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3277 2023-07-19 08:53:19.212684 djangocms-aldryn-categories-2.0.0/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2145 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/README.rst
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       87 2023-07-19 08:53:02.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      971 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/admin.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      199 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/apps.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1064 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/cms_wizards.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3785 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/fields.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      291 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/forms.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/de/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      966 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1303 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/en/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/en/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      880 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1212 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/es/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      417 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1102 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/fr/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      924 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1327 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/it/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      417 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1102 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2045 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/0001_initial.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      513 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/0002_auto_20150109_1415.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      690 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/0003_auto_20150128_1359.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      637 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/0004_auto_20150623_0859.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2923 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/models.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       55 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1513 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/base.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      999 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/test_admin.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4549 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/test_fields.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6241 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/test_models.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 08:53:19.208684 djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3277 2023-07-19 08:53:19.000000 djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1490 2023-07-19 08:53:19.000000 djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/SOURCES.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-19 08:53:19.000000 djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/dependency_links.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-18 14:10:41.000000 djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/not-zip-safe
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       35 2023-07-19 08:53:19.000000 djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/requires.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       18 2023-07-19 08:53:19.000000 djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/top_level.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      119 2023-07-19 08:53:19.212684 djangocms-aldryn-categories-2.0.0/setup.cfg
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1466 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.0/setup.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.790017 djangocms-aldryn-categories-2.0.1/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1485 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/LICENSE
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      141 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/MANIFEST.in
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3277 2023-07-24 09:26:33.790017 djangocms-aldryn-categories-2.0.1/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2145 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/README.rst
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.786017 djangocms-aldryn-categories-2.0.1/aldryn_categories/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       87 2023-07-24 09:26:06.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      971 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/admin.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      199 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/apps.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1064 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/cms_wizards.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3785 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/fields.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      291 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/forms.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.782017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.782017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/de/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.786017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      966 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1303 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.782017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/en/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.786017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      880 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1212 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.782017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/es/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.786017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      417 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1102 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.782017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/fr/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.786017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      924 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1327 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.782017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/it/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.786017 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      417 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1102 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.786017 djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2045 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0001_initial.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      513 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0002_auto_20150109_1415.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      690 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0003_auto_20150128_1359.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      637 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0004_auto_20150623_0859.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1192 2023-07-24 09:09:56.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0005_alter_category_id_alter_categorytranslation_id_and_more.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-06-19 07:27:36.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2923 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/models.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.790017 djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       55 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1513 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/base.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      999 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/test_admin.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4549 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/test_fields.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6241 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/test_models.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 09:26:33.790017 djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3277 2023-07-24 09:26:33.000000 djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1583 2023-07-24 09:26:33.000000 djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/SOURCES.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-24 09:26:33.000000 djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/dependency_links.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-24 09:26:33.000000 djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/not-zip-safe
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       35 2023-07-24 09:26:33.000000 djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/requires.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       18 2023-07-24 09:26:33.000000 djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/top_level.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      119 2023-07-24 09:26:33.790017 djangocms-aldryn-categories-2.0.1/setup.cfg
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1466 2023-07-19 08:52:30.000000 djangocms-aldryn-categories-2.0.1/setup.py
```

### Comparing `djangocms-aldryn-categories-2.0.0/LICENSE` & `djangocms-aldryn-categories-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/PKG-INFO` & `djangocms-aldryn-categories-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-categories
-Version: 2.0.0
+Version: 2.0.1
 Summary: Hierarchical categories/taxonomies for your Django project.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-categories
 Author: Divio AG
 Author-email: info@divio.ch
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangocms-aldryn-categories-2.0.0/README.rst` & `djangocms-aldryn-categories-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/admin.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/cms_wizards.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/cms_wizards.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/fields.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/de/LC_MESSAGES/django.mo` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/de/LC_MESSAGES/django.po` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/en/LC_MESSAGES/django.mo` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/en/LC_MESSAGES/django.po` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/es/LC_MESSAGES/django.po` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/fr/LC_MESSAGES/django.mo` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/fr/LC_MESSAGES/django.po` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/locale/it/LC_MESSAGES/django.po` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/0001_initial.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/0002_auto_20150109_1415.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0002_auto_20150109_1415.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/0003_auto_20150128_1359.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0003_auto_20150128_1359.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/migrations/0004_auto_20150623_0859.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/migrations/0004_auto_20150623_0859.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/models.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/base.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/test_admin.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/test_fields.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/aldryn_categories/tests/test_models.py` & `djangocms-aldryn-categories-2.0.1/aldryn_categories/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/PKG-INFO` & `djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-categories
-Version: 2.0.0
+Version: 2.0.1
 Summary: Hierarchical categories/taxonomies for your Django project.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-categories
 Author: Divio AG
 Author-email: info@divio.ch
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangocms-aldryn-categories-2.0.0/djangocms_aldryn_categories.egg-info/SOURCES.txt` & `djangocms-aldryn-categories-2.0.1/djangocms_aldryn_categories.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 aldryn_categories/locale/fr/LC_MESSAGES/django.po
 aldryn_categories/locale/it/LC_MESSAGES/django.mo
 aldryn_categories/locale/it/LC_MESSAGES/django.po
 aldryn_categories/migrations/0001_initial.py
 aldryn_categories/migrations/0002_auto_20150109_1415.py
 aldryn_categories/migrations/0003_auto_20150128_1359.py
 aldryn_categories/migrations/0004_auto_20150623_0859.py
+aldryn_categories/migrations/0005_alter_category_id_alter_categorytranslation_id_and_more.py
 aldryn_categories/migrations/__init__.py
 aldryn_categories/tests/__init__.py
 aldryn_categories/tests/base.py
 aldryn_categories/tests/test_admin.py
 aldryn_categories/tests/test_fields.py
 aldryn_categories/tests/test_models.py
 djangocms_aldryn_categories.egg-info/PKG-INFO
```

### Comparing `djangocms-aldryn-categories-2.0.0/setup.py` & `djangocms-aldryn-categories-2.0.1/setup.py`

 * *Files identical despite different names*

