# Comparing `tmp/djangoldp_notification-2.2.9.tar.gz` & `tmp/djangoldp_notification-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_notification-2.2.9.tar", last modified: Tue May  4 11:51:49 2021, max compression
+gzip compressed data, was "djangoldp_notification-3.0.0.tar", last modified: Mon Jul 24 20:37:50 2023, max compression
```

## Comparing `djangoldp_notification-2.2.9.tar` & `djangoldp_notification-3.0.0.tar`

### file list

```diff
@@ -1,54 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/
--rw-rw-rw-   0 root         (0) root         (0)      667 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5598 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       72 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification/
--rw-rw-rw-   0 root         (0) root         (0)       76 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    12478 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/models.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/views.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     3526 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/middlewares.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1541 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     4093 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/tests/test_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification/tests/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1879 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/tests/scripts/generate_inbox_fixture.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      717 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0007_auto_20200604_1055.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0009_auto_20200619_0802.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0003_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)      694 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0002_auto_20190917_1107.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0006_subscription_parent.py
--rw-rw-rw-   0 root         (0) root         (0)     1659 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0010_notificationsetting.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0011_auto_20210218_1145.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0004_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0008_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)     1832 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/0005_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     1582 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/management/commands/suppress_old_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/management/commands/mock_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/management/commands/create_subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification/templates/
--rw-rw-rw-   0 root         (0) root         (0)      565 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/templates/email.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2021-05-04 11:51:46.000000 djangoldp_notification-2.2.9/djangoldp_notification/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/djangoldp_notification/djangoldp_settings.py
--rw-rw-rw-   0 root         (0) root         (0)       92 2021-05-04 11:51:22.000000 djangoldp_notification-2.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1986 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      380 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/djangoldp_notification.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      380 2021-05-04 11:51:48.000000 djangoldp_notification-2.2.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.133130 djangoldp_notification-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-24 20:37:50.133130 djangoldp_notification-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5940 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.129130 djangoldp_notification-3.0.0/djangoldp_notification/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-24 20:37:47.000000 djangoldp_notification-3.0.0/djangoldp_notification/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3526 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.125130 djangoldp_notification-3.0.0/djangoldp_notification/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.125130 djangoldp_notification-3.0.0/djangoldp_notification/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.129130 djangoldp_notification-3.0.0/djangoldp_notification/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.125130 djangoldp_notification-3.0.0/djangoldp_notification/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.129130 djangoldp_notification-3.0.0/djangoldp_notification/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.125130 djangoldp_notification-3.0.0/djangoldp_notification/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.129130 djangoldp_notification-3.0.0/djangoldp_notification/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.125130 djangoldp_notification-3.0.0/djangoldp_notification/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.129130 djangoldp_notification-3.0.0/djangoldp_notification/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2352 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/management/commands/create_subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/management/commands/mock_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1582 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/management/commands/suppress_old_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.133130 djangoldp_notification-3.0.0/djangoldp_notification/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      694 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0002_auto_20190917_1107.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0003_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0004_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0005_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0006_subscription_parent.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0007_auto_20200604_1055.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0008_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0009_auto_20200619_0802.py
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0010_notificationsetting.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0011_auto_20210218_1145.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0012_auto_20210729_1912.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0013_auto_20211016_1203.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0014_subscription_disable_automatic_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/0015_alter_subscription_options.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13848 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.133130 djangoldp_notification-3.0.0/djangoldp_notification/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/templates/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.133130 djangoldp_notification-3.0.0/djangoldp_notification/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/tests/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.133130 djangoldp_notification-3.0.0/djangoldp_notification/tests/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/tests/scripts/generate_inbox_fixture.py
+-rw-rw-rw-   0 root         (0) root         (0)     4093 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/tests/test_subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/djangoldp_notification/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:37:50.129130 djangoldp_notification-3.0.0/djangoldp_notification.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-24 20:37:50.000000 djangoldp_notification-3.0.0/djangoldp_notification.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-07-24 20:37:50.000000 djangoldp_notification-3.0.0/djangoldp_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:37:50.000000 djangoldp_notification-3.0.0/djangoldp_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-24 20:37:50.000000 djangoldp_notification-3.0.0/djangoldp_notification.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-24 20:37:50.000000 djangoldp_notification-3.0.0/djangoldp_notification.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-07-24 20:37:50.133130 djangoldp_notification-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-07-24 20:37:30.000000 djangoldp_notification-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_notification-2.2.9/setup.cfg` & `djangoldp_notification-3.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 author_email = matthieu@happy-dev.fr
 description = djangoldp package for notifications data models
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.1.0
-	djangoldp_account~=2.1
+	djangoldp~=3.0
+	djangoldp_account>=3.0
 
 [options.extras_require]
 include_package_data = True
 dev = 
 	factory_boy>=2.12.0
 
 [semantic_release]
```

### Comparing `djangoldp_notification-2.2.9/README.md` & `djangoldp_notification-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 An object allowing a User to be notified of any change on a resource or a container. A subscription has the following fields:
 
 | Field    | Type       | Default | Description                                                  |
 | -------- | ---------- | ------- | ------------------------------------------------------------ |
 | `object` | `URLField` |         | ID of the resource or the container to watch                 |
 | `inbox`  | `URLField` |         | ID of the inbox to notify when the resource or the container change |
 | `field`  | `CharField` |         | (optional) if set, then object['field'] will be sent in the notification, not object |
+| `disable_automatic_notifications`  | `BooleanField` |   `False`   | By default, notifications will be sent to this inbox everytime the target object/container is updated. Setting this flag to true prevents this behaviour, meaning that notifications will have to be triggered manually |
 
 For convenience, when you create a subscription on an object, DjangoLDP-Notification will parse the object for any one-to-many nested field relations. It will then create nested-subscriptions, i.e. a subscription on the nested field which sends an update to the same inbox, passing the parent model. If this behaviour is undesired you can delete the `Subscription` instance
 
 You can automatically create required subscriptions based on your settings.py with this management command:
 
 ```bash
 ./manage.py create_subscriptions
@@ -124,7 +125,12 @@
 Then run this command to send notifications:
 
 ```bash
 ./manage.py check_integrity --send-subscription-notifications
 ```
 
 Notice that you may have to restart your ActivityQueue or your DjangoLDP server, depending on [how you configured the ActivityQueueService](https://git.startinblox.com/djangoldp-packages/djangoldp/blob/master/djangoldp/conf/server_template/server/wsgi.py-tpl#L21-24)
+
+
+## Changelog
+
+Now supports Django4.2 and Python3.11
```

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/models.py` & `djangoldp_notification-3.0.0/djangoldp_notification/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 from django.core.mail import send_mail
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models.signals import post_save, post_delete
 from django.dispatch import receiver
 from django.template import loader
 from django.urls import NoReverseMatch, get_resolver, reverse
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from djangoldp.fields import LDPUrlField
 from djangoldp.models import Model
 from djangoldp.views import LDPViewSet
 from djangoldp.activities.services import ActivityQueueService, ActivityPubService, activity_sending_finished
 from djangoldp_notification.middlewares import MODEL_MODIFICATION_USER_FIELD
 from djangoldp_notification.permissions import InboxPermissions, SubscriptionsPermissions
 from djangoldp_notification.views import LDPNotificationsViewSet
 import logging
 
 
 logger = logging.getLogger('djangoldp')
 
 
 class Notification(Model):
-    user = models.ForeignKey(settings.AUTH_USER_MODEL, related_name='inbox', on_delete=models.deletion.CASCADE)
-    author = LDPUrlField()
-    object = LDPUrlField()
+    user = models.ForeignKey(settings.AUTH_USER_MODEL, related_name='inbox', on_delete=models.deletion.CASCADE, help_text='the recipient of the notification')
+    author = LDPUrlField(help_text='the sender of the notification')
+    object = LDPUrlField(help_text='the urlid of the saved object being transmitted by the notification')
     type = models.CharField(max_length=255)
-    summary = models.TextField()
+    summary = models.TextField(blank=True, default='')
     date = models.DateTimeField(auto_now_add=True)
-    unread = models.BooleanField(default=True)
+    unread = models.BooleanField(default=True, help_text='set to False after the user has seen the notification')
 
     class Meta(Model.Meta):
         owner_field = 'user'
         ordering = ['-date']
         permission_classes = [InboxPermissions]
         anonymous_perms = ['add']
         authenticated_perms = ['inherit']
@@ -72,15 +72,15 @@
             if author == self.user:
                 return
 
         super(Notification, self).save(*args, **kwargs)
 
 class NotificationSetting(Model):
     user = models.OneToOneField(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, related_name="settings")
-    receiveMail = models.BooleanField(default=True)
+    receiveMail = models.BooleanField(default=True, help_text='if set to True the user will receive an email on notification receipt')
 
     class Meta:
         auto_author = 'user'
         owner_field = 'user'
         anonymous_perms = []
         authenticated_perms = []
         owner_perms = ['view', 'change']
@@ -88,23 +88,26 @@
         serializer_fields = ['@id', 'receiveMail']
         rdf_type = 'sib:usersettings'
 
     def __str__(self):
         return '{} ({})'.format(self.user.get_full_name(), self.user.urlid)
 
 class Subscription(Model):
-    object = models.URLField()
-    inbox = models.URLField()
+    object = models.URLField(help_text='the urlid of the object being subscribed')
+    inbox = models.URLField(help_text='the inbox of the recipient of the notification')
     field = models.CharField(max_length=255, blank=True, null=True,
                              help_text='if set to a field name on the object model, the field will be passed instead of the object instance')
+    disable_automatic_notifications = models.BooleanField(default=False,
+                             help_text='By default, notifications will be sent to this inbox everytime the target object/container is updated. Setting this flag to true prevents this behaviour, meaning that notifications will have to be triggered manually')
 
     def __str__(self):
         return '{}'.format(self.object)
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         anonymous_perms = []
         authenticated_perms = ["add", "view", "delete"]
         permission_classes = [SubscriptionsPermissions]
 
 
 @receiver(post_save, sender=Subscription, dispatch_uid="nested_subscriber_check")
 def create_nested_subscribers(sender, instance, created, **kwargs):
@@ -161,15 +164,15 @@
             try:
                 url_container = settings.BASE_URL + Model.container_id(instance)
                 url_resource = settings.BASE_URL + Model.resource_id(instance)
             except NoReverseMatch:
                 return
 
             # dispatch a notification for every Subscription on this resource
-            for subscription in Subscription.objects.filter(models.Q(object=url_resource) | models.Q(object=url_container)):
+            for subscription in Subscription.objects.filter(models.Q(disable_automatic_notifications=False) & (models.Q(object=url_resource) | models.Q(object=url_container))):
                 if subscription.inbox not in recipients and (not subscription.is_backlink or not kwargs.get("created")):
                     # I may have configured to send the subscription to a foreign key
                     if subscription.field is not None and len(subscription.field) > 1:
                         try:
                             if kwargs.get("created"):
                                 continue
 
@@ -218,66 +221,89 @@
             "object": object_iri,
             "author": author,
             "type": request_type
         }
         ActivityQueueService.send_activity(target, json)
 
 
+def get_default_email_sender_djangoldp_instance():
+    '''
+    :return: the configured email host if it can find one, or None
+    '''
+    email_from = (getattr(settings, 'DEFAULT_FROM_EMAIL', False) or getattr(settings, 'EMAIL_HOST_USER', False))
+    
+    if not email_from:
+        jabber_host = getattr(settings, 'JABBER_DEFAULT_HOST', False)
+
+        if jabber_host:
+            return "noreply@" + jabber_host
+        return None
+
+    return email_from
+
 @receiver(post_save, sender=Notification)
 def send_email_on_notification(sender, instance, created, **kwargs):
-    if created and instance.summary and getattr(settings,'JABBER_DEFAULT_HOST',False) and instance.user.email:
+    if created \
+            and instance.summary \
+            and instance.user.email \
+            and instance.type in ('Message', 'Mention'):
+
+        email_from = get_default_email_sender_djangoldp_instance()
+
+        if email_from is None or not instance.user.settings.receiveMail:
+            return
+
         # get author name, and store in who
         try:
             # local author
             if instance.author.startswith(settings.SITE_URL):
                 who = str(Model.resolve_id(instance.author.replace(settings.SITE_URL, '')).get_full_name())
             # external author
             else:
                 who = requests.get(instance.author).json()['name']
         except:
-            who = "Quelqu'un"
+            who = _("Quelqu'un")
 
         # get identifier for resource triggering notification, and store in where
         try:
             if instance.object.startswith(settings.SITE_URL):
                 if hasattr(Model.resolve_id(instance.object.replace(settings.SITE_URL, '')), 'get_full_name'):
                     where = Model.resolve_id(instance.object.replace(settings.SITE_URL, '')).get_full_name()
                 else:
                     where = str(Model.resolve_id(instance.object.replace(settings.SITE_URL, '')).name)
             else:
                 where = requests.get(instance.object).json()['name']
         except:
-            where = "le chat"
+            where = _("le chat")
 
         if who == where:
-            where = "t'a envoyé un message privé"
+            where = _("t'a envoyé un message privé")
         else:
-            where = "t'a mentionné sur " + where
+            where = _("t'a mentionné sur ") + where
 
         on = (getattr(settings, 'INSTANCE_DEFAULT_CLIENT', False) or settings.JABBER_DEFAULT_HOST)
 
         html_message = loader.render_to_string(
             'email.html',
             {
                 'on': on,
                 'instance': instance,
                 'author': who,
                 'object': where
             }
         )
 
-        if instance.user.settings.receiveMail:
-            send_mail(
-                'Notification sur ' + on,
-                instance.summary,
-                (getattr(settings, 'EMAIL_HOST_USER', False) or "noreply@" + settings.JABBER_DEFAULT_HOST),
-                [instance.user.email],
-                fail_silently=True,
-                html_message=html_message
-            )
+        send_mail(
+            _('Notification sur ') + on,
+            instance.summary,
+            email_from,
+            [instance.user.email],
+            fail_silently=True,
+            html_message=html_message
+        )
 
 @receiver(post_save, sender=settings.AUTH_USER_MODEL)
 def create_user_settings(sender, instance, created, **kwargs):
     try:
         if created and instance.urlid.startswith(settings.SITE_URL):
             NotificationSetting.objects.create(user=instance)
     except:
```

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/permissions.py` & `djangoldp_notification-3.0.0/djangoldp_notification/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/factories.py` & `djangoldp_notification-3.0.0/djangoldp_notification/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/check_integrity.py` & `djangoldp_notification-3.0.0/djangoldp_notification/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/middlewares.py` & `djangoldp_notification-3.0.0/djangoldp_notification/middlewares.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/admin.py` & `djangoldp_notification-3.0.0/djangoldp_notification/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp.models import Model
 from .models import Notification, NotificationSetting, Subscription
 
 
+@admin.register(Notification)
 class NotificationAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'user', 'author', 'type', 'object', 'unread')
-    exclude = ('urlid', 'is_backlink', 'allow_create_backlink', 'user')
+    exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     search_fields = ['urlid', 'user__urlid', 'author', 'object', 'type', 'summary']
     ordering = ['-urlid']
 
     def get_queryset(self, request):
         # Hide distant notification
         queryset = super(NotificationAdmin, self).get_queryset(request)
         internal_ids = [x.pk for x in queryset if not Model.is_external(x)]
         return queryset.filter(pk__in=internal_ids)
 
 
+@admin.register(Subscription)
 class SubscriptionAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'object', 'inbox', 'field')
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     search_fields = ['urlid', 'object', 'inbox', 'field']
     ordering = ['urlid']
 
 
+@admin.register(NotificationSetting)
 class NotificationSettingAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'user', 'receiveMail')
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     search_fields = ['urlid', 'user', 'receiveMail']
     ordering = ['urlid']
 
 
-admin.site.register(Notification, NotificationAdmin)
-admin.site.register(Subscription, SubscriptionAdmin)
-admin.site.register(NotificationSetting, NotificationSettingAdmin)
```

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/tests/runner.py` & `djangoldp_notification-3.0.0/djangoldp_notification/tests/runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import sys
 import yaml
 
 import django
 from django.conf import settings as django_settings
 from djangoldp.conf.ldpsettings import LDPSettings
-from djangoldp.tests.settings_default import yaml_config
+from djangoldp.tests.server_settings import yaml_config
 
 # override config loading
 config = {
     # add the packages to the reference list
     'ldppackages': ['djangoldp_account', 'djangoldp_notification', 'djangoldp_notification.tests'],
 
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
@@ -39,11 +40,12 @@
 django.setup()
 from django.test.runner import DiscoverRunner
 
 test_runner = DiscoverRunner(verbosity=1)
 
 failures = test_runner.run_tests([
     'djangoldp_notification.tests.test_models',
+    'djangoldp_notification.tests.test_subscriptions',
     'djangoldp_notification.tests.test_cache',
 ])
 if failures:
     sys.exit(failures)
```

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/tests/test_cache.py` & `djangoldp_notification-3.0.0/djangoldp_notification/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/tests/scripts/generate_inbox_fixture.py` & `djangoldp_notification-3.0.0/djangoldp_notification/tests/scripts/generate_inbox_fixture.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/tests/test_models.py` & `djangoldp_notification-3.0.0/djangoldp_notification/tests/test_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 from rest_framework.test import APITestCase, APIClient
 
 from djangoldp_account.models import LDPUser
 from djangoldp_notification.models import Subscription
 
 
-class TestSubscription(APITestCase):
+class TestModel(APITestCase):
     circle_user1_url = "http://localhost:8000/circles/1/"
     circle_user2_url = "http://localhost:8000/circles/2/"
 
     def _get_random_user(self):
         return LDPUser.objects.create(email='{}@test.co.uk'.format(str(uuid.uuid4())), first_name='Test',
                                       last_name='Test', username=str(uuid.uuid4()))
 
@@ -37,9 +37,10 @@
     def test_logged_in_succeeds(self):
         self._auth_as_user(self.user2)
         response = self.client.get("/subscriptions/").data.get("ldp:contains")
         self.assertEqual(len(response), 2)
         response = response[1]
         self.assertEqual(response["object"], self.circle_user2_url)
         self.assertEqual(response["inbox"], "http://testserver/users/piotr_kropotkine/inbox/")
-        self.assertIn({'mode': {'@type': 'view'}}, response["permissions"])
-        self.assertIn({'mode': {'@type': 'delete'}}, response["permissions"])
+        # No more permissions serialised on users
+        # self.assertIn({'mode': {'@type': 'view'}}, response["permissions"])
+        # self.assertIn({'mode': {'@type': 'delete'}}, response["permissions"])
```

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0007_auto_20200604_1055.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0007_auto_20200604_1055.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0009_auto_20200619_0802.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0009_auto_20200619_0802.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0003_auto_20200429_1346.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0003_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0002_auto_20190917_1107.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0002_auto_20190917_1107.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0006_subscription_parent.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0006_subscription_parent.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0010_notificationsetting.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0010_notificationsetting.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0011_auto_20210218_1145.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0011_auto_20210218_1145.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0004_auto_20200501_1207.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0004_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0008_auto_20200610_1323.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0008_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0001_initial.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/migrations/0005_auto_20200505_1733.py` & `djangoldp_notification-3.0.0/djangoldp_notification/migrations/0005_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/management/commands/suppress_old_notifications.py` & `djangoldp_notification-3.0.0/djangoldp_notification/management/commands/suppress_old_notifications.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/management/commands/create_subscriptions.py` & `djangoldp_notification-3.0.0/djangoldp_notification/management/commands/create_subscriptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,17 +6,43 @@
   help = 'Create required subscriptions'
 
   def handle(self, *args, **options):
     host = getattr(settings, 'SITE_URL')
     jabber_host = getattr(settings, 'JABBER_DEFAULT_HOST')
     xmpp = getattr(settings, 'PROSODY_HTTP_URL')
 
-    Subscription.objects.get_or_create(object=host+"/circles/", inbox=xmpp + "/conference." + jabber_host + "/happydev_muc_admin", field=None)
-    Subscription.objects.get_or_create(object=host+"/circle-members/", inbox=xmpp + "/conference." + jabber_host + "/happydev_muc_admin", field="circle")
-    Subscription.objects.get_or_create(object=host+"/projects/", inbox=xmpp + "/conference." + jabber_host + "/happydev_muc_admin", field=None)
-    Subscription.objects.get_or_create(object=host+"/project-members/", inbox=xmpp + "/conference." + jabber_host + "/happydev_muc_admin", field="project")
+    try:
+        sub = Subscription.objects.get(object="{}/circles/".format(host))
+        sub.delete()
+    except Subscription.DoesNotExist:
+        pass
+
+    try:
+        sub = Subscription.objects.get(object="{}/projects/".format(host))
+        sub.delete()
+    except Subscription.DoesNotExist:
+        pass
+
+    try:
+        sub = Subscription.objects.get(object="{}/circle-members/".format(host))
+        sub.delete()
+    except Subscription.DoesNotExist:
+        pass
+
+    try:
+        sub = Subscription.objects.get(object="{}/project-members/".format(host))
+        sub.delete()
+    except Subscription.DoesNotExist:
+        pass
+
+    Subscription.objects.get_or_create(object=host+"/circles/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_muc_admin", field=None)
+    Subscription.objects.get_or_create(object=host+"/projects/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_muc_admin", field=None)
+    
     Subscription.objects.get_or_create(object=host+"/users/", inbox=xmpp + "/" + jabber_host + "/happydev_user_admin", field=None)
     Subscription.objects.get_or_create(object=host+"/profiles/", inbox=xmpp + "/" + jabber_host + "/happydev_user_admin", field="user")
     Subscription.objects.get_or_create(object=host+"/chatprofiles/", inbox=xmpp + "/" + jabber_host + "/happydev_user_admin", field="user")
     Subscription.objects.get_or_create(object=host+"/accounts/", inbox=xmpp + "/" + jabber_host + "/happydev_user_admin", field="user")
 
+    Subscription.objects.get_or_create(object=host+"/circle-members/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_muc_members_admin", field=None)
+    Subscription.objects.get_or_create(object=host+"/project-members/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_muc_members_admin", field=None)
+
     self.stdout.write(self.style.SUCCESS("Successfully  created subscriptions\nhost: "+host+"\nxmpp server: "+xmpp+"\njabber host: "+jabber_host))
```

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/filters.py` & `djangoldp_notification-3.0.0/djangoldp_notification/filters.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification/templates/email.html` & `djangoldp_notification-3.0.0/djangoldp_notification/templates/email.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+{% load i18n %}
 <!DOCTYPE html>
 <html>
     <head>
     </head>
     <body>
         <div>
-            <p style='font-style:italic;color:#777'><b>{{ author }}</b> {{ object }} de {{ on }}</p>
+            <p style='font-style:italic;color:#777'><b>{{ author }}</b> {{ object }} {% trans "de" %} {{ on }}</p>
             <p>{{ instance.summary }}</p>
         </div>
         <div style='margin-top:10px;'>
             <p style='font-size:small;color:#777'>
                 --
                 <br>
-                Ne réponds pas directement à cet e-mail, à la place rends-toi sur <a href='{{ on }}' target='_blank'>{{ on }}</a>.
+                {% trans "Ne réponds pas directement à cet e-mail, à la place rends-toi sur" %} <a href='{{ on }}' target='_blank'>{{ on }}</a>.
                 <br>
             </p>
         </div>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,6 @@
-{{ author }} {{ object }} de {{ on }}
+{% load i18n %}
+{{ author }} {{ object }} {% trans "de" %} {{ on }}
 {{ instance.summary }}
 --
-Ne rÃ©ponds pas directement Ã  cet e-mail, Ã  la place rends-toi sur {{_on_}}.
+{% trans "Ne rÃ©ponds pas directement Ã  cet e-mail, Ã  la place rends-toi sur"
+%} {{_on_}}.
```

### Comparing `djangoldp_notification-2.2.9/djangoldp_notification.egg-info/SOURCES.txt` & `djangoldp_notification-3.0.0/djangoldp_notification.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 djangoldp_notification/settings.py
 djangoldp_notification/views.py
 djangoldp_notification.egg-info/PKG-INFO
 djangoldp_notification.egg-info/SOURCES.txt
 djangoldp_notification.egg-info/dependency_links.txt
 djangoldp_notification.egg-info/requires.txt
 djangoldp_notification.egg-info/top_level.txt
+djangoldp_notification/locale/en/LC_MESSAGES/django.mo
+djangoldp_notification/locale/en/LC_MESSAGES/django.po
+djangoldp_notification/locale/es/LC_MESSAGES/django.mo
+djangoldp_notification/locale/es/LC_MESSAGES/django.po
+djangoldp_notification/locale/fr/LC_MESSAGES/django.mo
+djangoldp_notification/locale/fr/LC_MESSAGES/django.po
 djangoldp_notification/management/commands/__init__.py
 djangoldp_notification/management/commands/create_subscriptions.py
 djangoldp_notification/management/commands/mock_notification.py
 djangoldp_notification/management/commands/suppress_old_notifications.py
 djangoldp_notification/migrations/0001_initial.py
 djangoldp_notification/migrations/0002_auto_20190917_1107.py
 djangoldp_notification/migrations/0003_auto_20200429_1346.py
@@ -30,15 +36,20 @@
 djangoldp_notification/migrations/0005_auto_20200505_1733.py
 djangoldp_notification/migrations/0006_subscription_parent.py
 djangoldp_notification/migrations/0007_auto_20200604_1055.py
 djangoldp_notification/migrations/0008_auto_20200610_1323.py
 djangoldp_notification/migrations/0009_auto_20200619_0802.py
 djangoldp_notification/migrations/0010_notificationsetting.py
 djangoldp_notification/migrations/0011_auto_20210218_1145.py
+djangoldp_notification/migrations/0012_auto_20210729_1912.py
+djangoldp_notification/migrations/0013_auto_20211016_1203.py
+djangoldp_notification/migrations/0014_subscription_disable_automatic_notifications.py
+djangoldp_notification/migrations/0015_alter_subscription_options.py
 djangoldp_notification/migrations/__init__.py
 djangoldp_notification/templates/__init__.py
 djangoldp_notification/templates/email.html
 djangoldp_notification/tests/__init__.py
 djangoldp_notification/tests/runner.py
 djangoldp_notification/tests/test_cache.py
 djangoldp_notification/tests/test_models.py
+djangoldp_notification/tests/test_subscriptions.py
 djangoldp_notification/tests/scripts/generate_inbox_fixture.py
```

