# Comparing `tmp/django-livesettings3-1.6.0.tar.gz` & `tmp/django-livesettings3-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-livesettings3-1.6.0.tar", last modified: Thu Jul 20 00:00:02 2023, max compression
+gzip compressed data, was "django-livesettings3-1.6.1.tar", last modified: Thu Jul 20 01:18:06 2023, max compression
```

## Comparing `django-livesettings3-1.6.0.tar` & `django-livesettings3-1.6.1.tar`

### file list

```diff
@@ -1,94 +1,89 @@
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.169468 django-livesettings3-1.6.0/
--rw-r--r--   0 evgeny     (501) staff       (20)       88 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/AUTHORS
--rw-r--r--   0 evgeny     (501) staff       (20)     1498 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/LICENSE
--rw-r--r--   0 evgeny     (501) staff       (20)      129 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/MANIFEST.in
--rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-20 00:00:02.169595 django-livesettings3-1.6.0/PKG-INFO
--rw-r--r--   0 evgeny     (501) staff       (20)     5906 2023-07-19 23:59:41.000000 django-livesettings3-1.6.0/README.md
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.143741 django-livesettings3-1.6.0/django_livesettings3.egg-info/
--rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-20 00:00:01.000000 django-livesettings3-1.6.0/django_livesettings3.egg-info/PKG-INFO
--rw-r--r--   0 evgeny     (501) staff       (20)     2301 2023-07-20 00:00:02.000000 django-livesettings3-1.6.0/django_livesettings3.egg-info/SOURCES.txt
--rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-20 00:00:01.000000 django-livesettings3-1.6.0/django_livesettings3.egg-info/dependency_links.txt
--rw-r--r--   0 evgeny     (501) staff       (20)       34 2023-07-20 00:00:01.000000 django-livesettings3-1.6.0/django_livesettings3.egg-info/requires.txt
--rw-r--r--   0 evgeny     (501) staff       (20)       13 2023-07-20 00:00:01.000000 django-livesettings3-1.6.0/django_livesettings3.egg-info/top_level.txt
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.152073 django-livesettings3-1.6.0/livesettings/
--rw-r--r--   0 evgeny     (501) staff       (20)      394 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/__init__.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1922 2023-07-14 19:51:10.000000 django-livesettings3-1.6.0/livesettings/forms.py
--rw-r--r--   0 evgeny     (501) staff       (20)     7684 2023-07-14 19:51:10.000000 django-livesettings3-1.6.0/livesettings/functions.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.138252 django-livesettings3-1.6.0/livesettings/locale/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.133575 django-livesettings3-1.6.0/livesettings/locale/de/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.153094 django-livesettings3-1.6.0/livesettings/locale/de/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)      706 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2982 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.134028 django-livesettings3-1.6.0/livesettings/locale/en/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.154159 django-livesettings3-1.6.0/livesettings/locale/en/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)      367 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2878 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.134539 django-livesettings3-1.6.0/livesettings/locale/es/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.154569 django-livesettings3-1.6.0/livesettings/locale/es/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.134956 django-livesettings3-1.6.0/livesettings/locale/fr/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.155403 django-livesettings3-1.6.0/livesettings/locale/fr/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1621 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3618 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.135475 django-livesettings3-1.6.0/livesettings/locale/he/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.156356 django-livesettings3-1.6.0/livesettings/locale/he/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1655 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2837 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.135884 django-livesettings3-1.6.0/livesettings/locale/it/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.157270 django-livesettings3-1.6.0/livesettings/locale/it/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1582 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3117 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.136325 django-livesettings3-1.6.0/livesettings/locale/ko/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.158152 django-livesettings3-1.6.0/livesettings/locale/ko/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1128 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3110 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.136738 django-livesettings3-1.6.0/livesettings/locale/pl/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.159003 django-livesettings3-1.6.0/livesettings/locale/pl/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2637 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.137276 django-livesettings3-1.6.0/livesettings/locale/pt_BR/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.159835 django-livesettings3-1.6.0/livesettings/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1208 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2645 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.137707 django-livesettings3-1.6.0/livesettings/locale/ru/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.160771 django-livesettings3-1.6.0/livesettings/locale/ru/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1178 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.138048 django-livesettings3-1.6.0/livesettings/locale/sv/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.161707 django-livesettings3-1.6.0/livesettings/locale/sv/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1481 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2598 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.138399 django-livesettings3-1.6.0/livesettings/locale/tr/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.162540 django-livesettings3-1.6.0/livesettings/locale/tr/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1242 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3243 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.163427 django-livesettings3-1.6.0/livesettings/migrations/
--rw-r--r--   0 evgeny     (501) staff       (20)     1684 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/migrations/0001_initial.py
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/migrations/__init__.py
--rw-r--r--   0 evgeny     (501) staff       (20)     7142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.0/livesettings/models.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1846 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/overrides.py
--rw-r--r--   0 evgeny     (501) staff       (20)       79 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/signals.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.138952 django-livesettings3-1.6.0/livesettings/templates/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.166048 django-livesettings3-1.6.0/livesettings/templates/livesettings/
--rw-r--r--   0 evgeny     (501) staff       (20)      437 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/templates/livesettings/_admin_site_views.html
--rw-r--r--   0 evgeny     (501) staff       (20)     4781 2023-07-19 23:59:41.000000 django-livesettings3-1.6.0/livesettings/templates/livesettings/group_settings.html
--rw-r--r--   0 evgeny     (501) staff       (20)      878 2023-07-17 19:18:52.000000 django-livesettings3-1.6.0/livesettings/templates/livesettings/groups_navbar.html
--rw-r--r--   0 evgeny     (501) staff       (20)     6159 2023-07-16 21:37:36.000000 django-livesettings3-1.6.0/livesettings/templates/livesettings/site_settings.html
--rw-r--r--   0 evgeny     (501) staff       (20)       41 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/templates/livesettings/text.txt
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.166736 django-livesettings3-1.6.0/livesettings/templatetags/
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/templatetags/__init__.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 00:00:02.168997 django-livesettings3-1.6.0/livesettings/templatetags/__pycache__/
--rw-r--r--   0 evgeny     (501) staff       (20)      168 2022-02-10 21:17:23.000000 django-livesettings3-1.6.0/livesettings/templatetags/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)      176 2023-07-14 21:20:54.000000 django-livesettings3-1.6.0/livesettings/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     2084 2022-02-10 21:17:23.000000 django-livesettings3-1.6.0/livesettings/templatetags/__pycache__/config_tags.cpython-36.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     2098 2023-07-14 21:20:54.000000 django-livesettings3-1.6.0/livesettings/templatetags/__pycache__/config_tags.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     2142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.0/livesettings/templatetags/config_tags.py
--rw-r--r--   0 evgeny     (501) staff       (20)      447 2023-07-16 19:44:06.000000 django-livesettings3-1.6.0/livesettings/test_urls.py
--rw-r--r--   0 evgeny     (501) staff       (20)    29460 2023-07-17 19:11:51.000000 django-livesettings3-1.6.0/livesettings/tests.py
--rw-r--r--   0 evgeny     (501) staff       (20)      392 2023-07-15 19:16:27.000000 django-livesettings3-1.6.0/livesettings/urls.py
--rw-r--r--   0 evgeny     (501) staff       (20)     2131 2022-02-10 21:13:39.000000 django-livesettings3-1.6.0/livesettings/utils.py
--rw-r--r--   0 evgeny     (501) staff       (20)    33758 2023-07-19 23:59:41.000000 django-livesettings3-1.6.0/livesettings/values.py
--rw-r--r--   0 evgeny     (501) staff       (20)     4706 2023-07-17 19:19:33.000000 django-livesettings3-1.6.0/livesettings/views.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1135 2023-07-19 23:59:41.000000 django-livesettings3-1.6.0/livesettings/widgets.py
--rw-r--r--   0 evgeny     (501) staff       (20)       79 2023-07-20 00:00:02.170080 django-livesettings3-1.6.0/setup.cfg
--rw-r--r--   0 evgeny     (501) staff       (20)     1277 2023-07-16 19:15:07.000000 django-livesettings3-1.6.0/setup.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.893473 django-livesettings3-1.6.1/
+-rw-r--r--   0 evgeny     (501) staff       (20)       88 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/AUTHORS
+-rw-r--r--   0 evgeny     (501) staff       (20)     1498 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/LICENSE
+-rw-r--r--   0 evgeny     (501) staff       (20)       93 2023-07-20 01:14:43.000000 django-livesettings3-1.6.1/MANIFEST.in
+-rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-20 01:18:06.893626 django-livesettings3-1.6.1/PKG-INFO
+-rw-r--r--   0 evgeny     (501) staff       (20)     5906 2023-07-19 23:59:41.000000 django-livesettings3-1.6.1/README.md
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.865051 django-livesettings3-1.6.1/django_livesettings3.egg-info/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/PKG-INFO
+-rw-r--r--   0 evgeny     (501) staff       (20)     2047 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)       34 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/requires.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)       13 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/top_level.txt
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.873976 django-livesettings3-1.6.1/livesettings/
+-rw-r--r--   0 evgeny     (501) staff       (20)      394 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/__init__.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1922 2023-07-14 19:51:10.000000 django-livesettings3-1.6.1/livesettings/forms.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     7684 2023-07-14 19:51:10.000000 django-livesettings3-1.6.1/livesettings/functions.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.859092 django-livesettings3-1.6.1/livesettings/locale/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.854882 django-livesettings3-1.6.1/livesettings/locale/de/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.874972 django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)      706 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2982 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.855238 django-livesettings3-1.6.1/livesettings/locale/en/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.876140 django-livesettings3-1.6.1/livesettings/locale/en/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)      367 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2878 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.855588 django-livesettings3-1.6.1/livesettings/locale/es/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.876586 django-livesettings3-1.6.1/livesettings/locale/es/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.855936 django-livesettings3-1.6.1/livesettings/locale/fr/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.877364 django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1621 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3618 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.856382 django-livesettings3-1.6.1/livesettings/locale/he/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.878250 django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1655 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2837 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.856786 django-livesettings3-1.6.1/livesettings/locale/it/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.879166 django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1582 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3117 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.857232 django-livesettings3-1.6.1/livesettings/locale/ko/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.880015 django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1128 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3110 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.857629 django-livesettings3-1.6.1/livesettings/locale/pl/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.881208 django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2637 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.858003 django-livesettings3-1.6.1/livesettings/locale/pt_BR/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.882661 django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1208 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2645 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.858373 django-livesettings3-1.6.1/livesettings/locale/ru/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.884125 django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1178 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.858743 django-livesettings3-1.6.1/livesettings/locale/sv/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.885533 django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1481 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2598 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.859254 django-livesettings3-1.6.1/livesettings/locale/tr/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.886945 django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1242 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3243 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.888294 django-livesettings3-1.6.1/livesettings/migrations/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1684 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/migrations/0001_initial.py
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/migrations/__init__.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     7142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.1/livesettings/models.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1846 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/overrides.py
+-rw-r--r--   0 evgeny     (501) staff       (20)       79 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/signals.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.859873 django-livesettings3-1.6.1/livesettings/templates/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.892094 django-livesettings3-1.6.1/livesettings/templates/livesettings/
+-rw-r--r--   0 evgeny     (501) staff       (20)      437 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/_admin_site_views.html
+-rw-r--r--   0 evgeny     (501) staff       (20)     4781 2023-07-19 23:59:41.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/group_settings.html
+-rw-r--r--   0 evgeny     (501) staff       (20)      878 2023-07-17 19:18:52.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/groups_navbar.html
+-rw-r--r--   0 evgeny     (501) staff       (20)     6159 2023-07-16 21:37:36.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/site_settings.html
+-rw-r--r--   0 evgeny     (501) staff       (20)       41 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/text.txt
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.893022 django-livesettings3-1.6.1/livesettings/templatetags/
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/templatetags/__init__.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     2142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.1/livesettings/templatetags/config_tags.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      447 2023-07-16 19:44:06.000000 django-livesettings3-1.6.1/livesettings/test_urls.py
+-rw-r--r--   0 evgeny     (501) staff       (20)    29460 2023-07-17 19:11:51.000000 django-livesettings3-1.6.1/livesettings/tests.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      392 2023-07-15 19:16:27.000000 django-livesettings3-1.6.1/livesettings/urls.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     2131 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/utils.py
+-rw-r--r--   0 evgeny     (501) staff       (20)    33758 2023-07-19 23:59:41.000000 django-livesettings3-1.6.1/livesettings/values.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     4706 2023-07-17 19:19:33.000000 django-livesettings3-1.6.1/livesettings/views.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1135 2023-07-19 23:59:41.000000 django-livesettings3-1.6.1/livesettings/widgets.py
+-rw-r--r--   0 evgeny     (501) staff       (20)       79 2023-07-20 01:18:06.894150 django-livesettings3-1.6.1/setup.cfg
+-rw-r--r--   0 evgeny     (501) staff       (20)     1277 2023-07-20 01:16:11.000000 django-livesettings3-1.6.1/setup.py
```

### Comparing `django-livesettings3-1.6.0/LICENSE` & `django-livesettings3-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/PKG-INFO` & `django-livesettings3-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-livesettings3
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python 3 port of django-livesettings
 Home-page: https://github.com/kunaldeo/django-livesettings3/
 Author: Kunal Deo
 Author-email: kunaldeo@gmail.com
 License: New BSD License
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-livesettings3-1.6.0/README.md` & `django-livesettings3-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/django_livesettings3.egg-info/PKG-INFO` & `django-livesettings3-1.6.1/django_livesettings3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-livesettings3
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python 3 port of django-livesettings
 Home-page: https://github.com/kunaldeo/django-livesettings3/
 Author: Kunal Deo
 Author-email: kunaldeo@gmail.com
 License: New BSD License
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-livesettings3-1.6.0/django_livesettings3.egg-info/SOURCES.txt` & `django-livesettings3-1.6.1/django_livesettings3.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -49,12 +49,8 @@
 livesettings/migrations/__init__.py
 livesettings/templates/livesettings/_admin_site_views.html
 livesettings/templates/livesettings/group_settings.html
 livesettings/templates/livesettings/groups_navbar.html
 livesettings/templates/livesettings/site_settings.html
 livesettings/templates/livesettings/text.txt
 livesettings/templatetags/__init__.py
-livesettings/templatetags/config_tags.py
-livesettings/templatetags/__pycache__/__init__.cpython-36.pyc
-livesettings/templatetags/__pycache__/__init__.cpython-39.pyc
-livesettings/templatetags/__pycache__/config_tags.cpython-36.pyc
-livesettings/templatetags/__pycache__/config_tags.cpython-39.pyc
+livesettings/templatetags/config_tags.py
```

### Comparing `django-livesettings3-1.6.0/livesettings/forms.py` & `django-livesettings3-1.6.1/livesettings/forms.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/functions.py` & `django-livesettings3-1.6.1/livesettings/functions.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/de/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/de/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/en/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/fr/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/fr/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/he/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/he/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/it/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/it/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/ko/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/ko/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/pl/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/pl/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/pt_BR/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/pt_BR/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/ru/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/ru/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/sv/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/sv/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/tr/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/locale/tr/LC_MESSAGES/django.po` & `django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/migrations/0001_initial.py` & `django-livesettings3-1.6.1/livesettings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/models.py` & `django-livesettings3-1.6.1/livesettings/models.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/overrides.py` & `django-livesettings3-1.6.1/livesettings/overrides.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/templates/livesettings/group_settings.html` & `django-livesettings3-1.6.1/livesettings/templates/livesettings/group_settings.html`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/templates/livesettings/groups_navbar.html` & `django-livesettings3-1.6.1/livesettings/templates/livesettings/groups_navbar.html`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/templates/livesettings/site_settings.html` & `django-livesettings3-1.6.1/livesettings/templates/livesettings/site_settings.html`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/templatetags/config_tags.py` & `django-livesettings3-1.6.1/livesettings/templatetags/config_tags.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/tests.py` & `django-livesettings3-1.6.1/livesettings/tests.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/utils.py` & `django-livesettings3-1.6.1/livesettings/utils.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/values.py` & `django-livesettings3-1.6.1/livesettings/values.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/views.py` & `django-livesettings3-1.6.1/livesettings/views.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/livesettings/widgets.py` & `django-livesettings3-1.6.1/livesettings/widgets.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.0/setup.py` & `django-livesettings3-1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-livesettings3',
-    version='1.6.0',
+    version='1.6.1',
     description="Python 3 port of django-livesettings",
     long_description="""Python 3 version of django live settings. It provides the ability to configure settings via an admin interface, rather than by editing "settings.py". Documentation avaiable at Github.""",
     author='Kunal Deo',
     author_email='kunaldeo@gmail.com',
     url='https://github.com/kunaldeo/django-livesettings3/',
     license='New BSD License',
     platforms=['any'],
@@ -18,10 +18,10 @@
                  'Programming Language :: Python',
                  'Programming Language :: Python :: 3 :: Only',
                  'Programming Language :: Python :: 3.8',
                  'Programming Language :: Python :: 3.9',
                  'Programming Language :: Python :: 3.10',
                  'Framework :: Django'],
     packages=find_packages(),
-    install_requires=['django>=1.8,<6', 'django-keyedcache3'],
+    install_requires=['django>=1.8,<5', 'django-keyedcache3'],
     include_package_data=True,
 )
```

