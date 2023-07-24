# Comparing `tmp/djangoldp_joboffer-2.2.6.tar.gz` & `tmp/djangoldp_joboffer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_joboffer-2.2.6.tar", last modified: Wed Jan 26 18:52:23 2022, max compression
+gzip compressed data, was "djangoldp_joboffer-3.0.0.tar", last modified: Mon Jul 24 21:49:45 2023, max compression
```

## Comparing `djangoldp_joboffer-2.2.6.tar` & `djangoldp_joboffer-3.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/
--rw-rw-rw-   0 root         (0) root         (0)      739 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/
--rw-rw-rw-   0 root         (0) root         (0)     4566 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2360 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)     6379 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/tests_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     3814 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/tests_inbox.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     8254 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/templates/joboffer/
--rw-rw-rw-   0 root         (0) root         (0)      586 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/templates/joboffer/email.html
--rw-rw-rw-   0 root         (0) root         (0)     1178 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/management/commands/mock_joboffer.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-01-26 18:52:21.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1301 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0008_auto_20210326_1424.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0009_auto_20210531_1311.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0006_auto_20200804_1803.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0004_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0002_joboffer_urlid.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0005_auto_20200619_0815.py
--rw-rw-rw-   0 root         (0) root         (0)      933 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0007_auto_20200924_1937.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0003_auto_20200522_1521.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0010_joboffer_location.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2022-01-26 18:52:09.000000 djangoldp_joboffer-2.2.6/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      736 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      314 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 18:52:23.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2022-01-26 18:52:22.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 18:52:22.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1626 2022-01-26 18:52:22.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-01-26 18:52:22.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2022-01-26 18:52:22.000000 djangoldp_joboffer-2.2.6/djangoldp_joboffer.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      739 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.863922 djangoldp_joboffer-3.0.0/djangoldp_joboffer/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-24 21:49:43.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/djangoldp_joboffer/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/djangoldp_joboffer/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/management/commands/mock_joboffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0002_joboffer_urlid.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0003_auto_20200522_1521.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0004_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0005_auto_20200619_0815.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0006_auto_20200804_1803.py
+-rw-rw-rw-   0 root         (0) root         (0)      933 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0007_auto_20200924_1937.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0008_auto_20210326_1424.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0009_auto_20210531_1311.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0010_joboffer_location.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8253 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/djangoldp_joboffer/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/djangoldp_joboffer/templates/joboffer/
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/templates/joboffer/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3814 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/tests_inbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     6379 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/tests_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2360 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/djangoldp_joboffer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-24 21:49:45.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-07-24 21:49:45.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:49:45.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-24 21:49:45.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 21:49:45.000000 djangoldp_joboffer-3.0.0/djangoldp_joboffer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-07-24 21:49:45.867922 djangoldp_joboffer-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 21:49:27.000000 djangoldp_joboffer-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_joboffer-2.2.6/README.md` & `djangoldp_joboffer-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/views.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/tests_post.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/tests_notifications.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/tests_notifications.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/tests_inbox.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/tests_inbox.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/tests/runner.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/tests/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         'djangoldp_notification',
         'djangoldp_account',
         'djangoldp_joboffer',
         'djangoldp_joboffer.tests'],
 
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

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/models.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.db import models
 from django.contrib.auth import get_user_model
 from django.core.mail import send_mail
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 from django.template.loader import render_to_string
 from django.utils.html import strip_tags
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 import re
 
 from djangoldp.models import Model
 from djangoldp.activities import ActivityQueueService
 from djangoldp_skill.models import Skill
 from djangoldp_conversation.models import Conversation
 from djangoldp_notification.models import Notification, Subscription, get_default_email_sender_djangoldp_instance
```

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/templates/joboffer/email.html` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/templates/joboffer/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/admin.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp.models import Model
 from .models import JobOffer
 from .signals import post_save_joboffer_with_skills
 
 
+@admin.register(JobOffer)
 class JobOfferAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'title', 'author')
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     search_fields = ['urlid', 'title', 'author__urlid', 'skills__name', 'description']
     ordering = ['urlid']
 
     '''
@@ -22,8 +23,7 @@
     # when the JobOffer is saved and all related items attached,
     # send out notifications to users with matching skills
     def save_related(self, request, form, formsets, change):
         super().save_related(request, form, formsets, change)
         if isinstance(form.instance, JobOffer):
             post_save_joboffer_with_skills.send(sender=JobOffer, instance=form.instance, created=True)
 
-admin.site.register(JobOffer, JobOfferAdmin)
```

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/management/commands/mock_joboffer.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/management/commands/mock_joboffer.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/factories.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/notifications.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/notifications.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0001_initial.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0008_auto_20210326_1424.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0008_auto_20210326_1424.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0009_auto_20210531_1311.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0009_auto_20210531_1311.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0004_auto_20200610_1323.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0004_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0005_auto_20200619_0815.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0005_auto_20200619_0815.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0007_auto_20200924_1937.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0007_auto_20200924_1937.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer/migrations/0003_auto_20200522_1521.py` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer/migrations/0003_auto_20200522_1521.py`

 * *Files identical despite different names*

### Comparing `djangoldp_joboffer-2.2.6/setup.cfg` & `djangoldp_joboffer-3.0.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 description = djangoldp package for job offer data models
 license = MIT
 
 [options]
 include_package_data = True
 packages = find:
 install_requires = 
-	djangoldp_skill>=2.0
-	djangoldp>=2.1.27
-	djangoldp_notification>=2.2.12
+	djangoldp_skill~=3.0
+	djangoldp~=3.0
+	djangoldp_notification~=3.0
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
-	djangoldp_account>=2.1
+	djangoldp_account~=3.0
 	djangoldp_conversation
 	djangoldp_i18n
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_joboffer/__init__.py:__version__
 commit_parser = commit_parser.parse
```

### Comparing `djangoldp_joboffer-2.2.6/djangoldp_joboffer.egg-info/SOURCES.txt` & `djangoldp_joboffer-3.0.0/djangoldp_joboffer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

