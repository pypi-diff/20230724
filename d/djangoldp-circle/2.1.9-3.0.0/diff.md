# Comparing `tmp/djangoldp_circle-2.1.9.tar.gz` & `tmp/djangoldp_circle-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_circle-2.1.9.tar", last modified: Tue May 25 10:13:02 2021, max compression
+gzip compressed data, was "djangoldp_circle-3.0.0.tar", last modified: Mon Jul 24 21:44:53 2023, max compression
```

## Comparing `djangoldp_circle-2.1.9.tar` & `djangoldp_circle-3.0.0.tar`

### file list

```diff
@@ -1,71 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/
--rw-rw-rw-   0 root         (0) root         (0)      595 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/
--rw-rw-rw-   0 root         (0) root         (0)       32 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6192 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/models.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3764 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1660 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/views.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/xmpp.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     2905 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/
--rw-rw-rw-   0 root         (0) root         (0)    18326 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_save.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)     2348 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_view.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      464 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0002_auto_20191021_1357.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0019_auto_20200522_1516.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0015_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0024_auto_20200925_1108.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0010_auto_20200414_0908.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0027_circle_description.py
--rw-rw-rw-   0 root         (0) root         (0)      930 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0011_auto_20200426_1632.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0018_auto_20200512_1352.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0026_auto_20210115_1038.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0008_circlemember_is_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0009_auto_20200226_1742.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0005_auto_20191029_1227.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0007_auto_20191112_1251.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0020_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0023_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0017_auto_20200512_1348.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0025_remove_circle_team.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0016_merge_20200506_1904.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0012_auto_20200427_1047.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0028_auto_20210204_1904.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0030_merge_20210211_1453.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0029_auto_20210211_1244.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0003_auto_20191024_1604.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0014_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0013_auto_20200506_1503.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0029_auto_20210211_1440.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0014_auto_20200506_1517.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0004_auto_20191024_1831.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0013_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0006_circle_status.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      908 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/commands/mock_circle.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/filters.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2021-05-25 10:12:59.000000 djangoldp_circle-2.1.9/djangoldp_circle/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/setup.py
--rw-r--r--   0 root         (0) root         (0)      313 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-25 10:13:01.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2021-05-25 10:13:01.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-05-25 10:13:01.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2743 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      313 2021-05-25 10:13:01.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.060352 djangoldp_circle-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-24 21:44:53.060352 djangoldp_circle-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.052352 djangoldp_circle-3.0.0/djangoldp_circle/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-24 21:44:50.000000 djangoldp_circle-3.0.0/djangoldp_circle/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2905 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.052352 djangoldp_circle-3.0.0/djangoldp_circle/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.048351 djangoldp_circle-3.0.0/djangoldp_circle/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.052352 djangoldp_circle-3.0.0/djangoldp_circle/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.052352 djangoldp_circle-3.0.0/djangoldp_circle/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.052352 djangoldp_circle-3.0.0/djangoldp_circle/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2351 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.052352 djangoldp_circle-3.0.0/djangoldp_circle/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.056352 djangoldp_circle-3.0.0/djangoldp_circle/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      534 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.052352 djangoldp_circle-3.0.0/djangoldp_circle/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.056352 djangoldp_circle-3.0.0/djangoldp_circle/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.056352 djangoldp_circle-3.0.0/djangoldp_circle/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.056352 djangoldp_circle-3.0.0/djangoldp_circle/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/management/commands/mock_circle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.060352 djangoldp_circle-3.0.0/djangoldp_circle/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0002_auto_20191021_1357.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0003_auto_20191024_1604.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0004_auto_20191024_1831.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0005_auto_20191029_1227.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0006_circle_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0007_auto_20191112_1251.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0008_circlemember_is_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0009_auto_20200226_1742.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0010_auto_20200414_0908.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0011_auto_20200426_1632.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0012_auto_20200427_1047.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0013_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0013_auto_20200506_1503.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0014_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0014_auto_20200506_1517.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0015_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0016_merge_20200506_1904.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0017_auto_20200512_1348.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0018_auto_20200512_1352.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0019_auto_20200522_1516.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0020_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0023_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0024_auto_20200925_1108.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0025_remove_circle_team.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0026_auto_20210115_1038.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0027_circle_description.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0028_auto_20210204_1904.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0029_auto_20210211_1244.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0029_auto_20210211_1440.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0030_merge_20210211_1453.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0031_circle_parentcircle.py
+-rw-rw-rw-   0 root         (0) root         (0)     2323 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0032_auto_20220304_1046.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0033_auto_20220317_1915.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0034_auto_20220412_1337.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/0035_alter_circle_options_alter_circlemember_options.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15225 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.060352 djangoldp_circle-3.0.0/djangoldp_circle/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.060352 djangoldp_circle-3.0.0/djangoldp_circle/templates/accessrequests/
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/templates/accessrequests/access_requested.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/templates/accessrequests/access_resolved.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.060352 djangoldp_circle-3.0.0/djangoldp_circle/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)    21180 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_save.py
+-rw-rw-rw-   0 root         (0) root         (0)     3324 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_view.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6344 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/djangoldp_circle/xmpp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:44:53.052352 djangoldp_circle-3.0.0/djangoldp_circle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-24 21:44:52.000000 djangoldp_circle-3.0.0/djangoldp_circle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-07-24 21:44:53.000000 djangoldp_circle-3.0.0/djangoldp_circle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:44:52.000000 djangoldp_circle-3.0.0/djangoldp_circle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-24 21:44:52.000000 djangoldp_circle-3.0.0/djangoldp_circle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-24 21:44:52.000000 djangoldp_circle-3.0.0/djangoldp_circle.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-24 21:44:53.060352 djangoldp_circle-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 21:44:32.000000 djangoldp_circle-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_circle-2.1.9/setup.cfg` & `djangoldp_circle-3.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 author_email = nicolas@happy-dev.fr
 description = djangoldp package for circle data models
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp>=2.1
-	djangoldp_account>=2.1
+	djangoldp~=3.0
+	djangoldp_account~=3.0
+include_package_data = true
 
 [options.extras_require]
 dev = 
 	factory_boy>=2.11.0
+	djangoldp_notification>=3.0
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_circle/__init__.py:__version__
 commit_parser = commit_parser.parse
 
 [egg_info]
```

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/permissions.py` & `djangoldp_circle-3.0.0/djangoldp_circle/permissions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.conf import settings
 from django.db.models import QuerySet, Q
 
 from djangoldp.utils import is_authenticated_user
 from djangoldp.permissions import LDPPermissions, LDPObjectLevelPermissions
-from djangoldp_circle.filters import CircleFilterBackend, CircleMemberFilterBackend
+from djangoldp_circle.filters import CircleFilterBackend, CircleMemberFilterBackend, \
+    CircleAccessRequestFilterBackend
 from djangoldp_circle.xmpp import get_client_ip, XMPP_SERVERS
 
 
 class CirclePermissions(LDPPermissions):
     filter_backends = [CircleFilterBackend]
 
     def get_object_permissions(self, request, view, obj):
@@ -22,16 +23,21 @@
                 if obj.members.filter(user=user).get().is_admin:
                     perms = perms.union({'change', 'delete'})
 
         # permissions gained by the circle being public
         if obj.status == 'Public':
             perms = perms.union({'view'})
 
+            # I can join the public circle
             if is_authenticated_user(user):
                 perms = perms.union({'add'})
+        
+        # I can view - but not automatically join - restricted circles
+        elif obj.status == 'Restricted':
+            perms = perms.union({'view'})
 
         return perms
 
     def get_container_permissions(self, request, view, obj=None, bypass=False):
         if obj is None:
             perms = super().get_container_permissions(request, view, obj)
 
@@ -99,7 +105,25 @@
         return super().has_permission(request, view)
     
     def has_object_permission(self, request, view, obj):
         if get_client_ip(request) in XMPP_SERVERS:
             return True
 
         return super().has_object_permission(request, view, obj)
+
+
+class CircleAccessRequestPermissions(LDPPermissions):
+    filter_backends = [CircleAccessRequestFilterBackend]
+
+    def get_object_permissions(self, request, view, obj):
+        from djangoldp_circle.models import CircleMember
+
+        perms = super().get_object_permissions(request, view, obj)
+
+        user = request.user
+        if is_authenticated_user(user):
+            # I must be an admin of the circle referenced
+            member = obj.circle.members.filter(user=user)
+            if member.exists() and member.get().is_admin:
+                perms = perms.union({'view', 'change'})
+
+        return perms
```

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/factories.py` & `djangoldp_circle-3.0.0/djangoldp_circle/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/check_integrity.py` & `djangoldp_circle-3.0.0/djangoldp_circle/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/admin.py` & `djangoldp_circle-3.0.0/djangoldp_circle/admin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp.models import Model
-from .models import Circle, CircleMember
+from .models import Circle, CircleMember, CircleAccessRequest
 
 
+@admin.register(CircleMember)
 class EmptyAdmin(admin.ModelAdmin):
     def get_model_perms(self, request):
         return {}
 
 
 class TeamInline(admin.TabularInline):
     model = CircleMember
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
     extra = 0
 
 
+@admin.register(CircleAccessRequest)
+class CircleAccessRequestAdmin(DjangoLDPAdmin):
+    list_display = ('urlid', 'user', 'circle', 'status')
+    exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
+    search_fields = ['urlid', 'user__urlid', 'circle__urlid', 'circle__name']
+    ordering = ['urlid']
+
+
+class CircleAccessRequestInline(admin.TabularInline):
+    model = CircleAccessRequest
+    exclude = ('urlid', 'is_backlink', 'allow_create_backlink')
+    extra = 0
+
+
+@admin.register(Circle)
 class CircleAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'name', 'owner', 'status', 'jabberID')
     exclude = ('urlid', 'is_backlink', 'allow_create_backlink', 'jabberID', 'jabberRoom')
     search_fields = ['urlid', 'name', 'members__user__urlid', 'subtitle', 'description', 'status', 'owner__urlid']
     ordering = ['urlid']
-    inlines = [TeamInline]
+    inlines = [TeamInline, CircleAccessRequestInline]
 
     def get_queryset(self, request):
         # Hide distant circles
         queryset = super(CircleAdmin, self).get_queryset(request)
         internal_ids = [x.pk for x in queryset if not Model.is_external(x)]
         return queryset.filter(pk__in=internal_ids)
 
 
-admin.site.register(CircleMember, EmptyAdmin)
-admin.site.register(Circle, CircleAdmin)
```

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_permissions.py` & `djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime, timedelta
 
 from djangoldp.permissions import LDPPermissions
 
 from rest_framework.test import APITestCase, APIClient
 from guardian.shortcuts import assign_perm
 
-from djangoldp_circle.models import Circle, CircleMember
+from djangoldp_circle.models import Circle, CircleMember, CircleAccessRequest
 from djangoldp_circle.tests.utils import get_random_user
 
 
 class PermissionsTestCase(APITestCase):
     def setUp(self):
         self.client = APIClient()
 
@@ -88,18 +88,19 @@
     def test_list_circles(self):
         self.setUpLoggedInUser()
         # a public circle, a private circle I own and a private circle I'm not in
         another_user = get_random_user()
         public_circle = self._get_random_circle('Public', another_user)
         my_circle = self._get_random_circle('Private', self.user)
         private_circle = self._get_random_circle('Private', another_user)
+        restricted_circle = self._get_random_circle('Restricted', another_user)
 
         response = self.client.get('/circles/')
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(len(response.data['ldp:contains']), 2)
+        self.assertEqual(len(response.data['ldp:contains']), 3)
 
     # GET circle public
     def test_get_public_circle(self):
         self.setUpLoggedInUser()
         another_user = get_random_user()
         self.setUpCircle('Public', another_user)
 
@@ -457,7 +458,68 @@
 
         response = self.client.patch('/circles/{}/'.format(self.circle.pk),
                                      data=json.dumps(payload), content_type='application/ld+json')
         self.assertEqual(response.status_code, 200)
 
         circle = Circle.objects.get(pk=self.circle.pk)
         self.assertEqual(circle.owner.urlid, owner_id)
+    
+    def test_make_access_request(self):
+        self.setUpLoggedInUser()
+        self.setUpCircle('Restrict', get_random_user())
+        
+        payload = self._get_request_json(circle=self.circle.urlid)
+
+        response = self.client.post('/circles/{}/access_requests/'.format(self.circle.pk),
+                                    data=json.dumps(payload), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 201)
+        ar = CircleAccessRequest.objects.filter(user=self.user)[0]
+        self.assertEqual(ar.circle, self.circle)
+
+    def test_accept_access_request(self):
+        self.setUpLoggedInUser()
+        self.setUpCircle('Restrict', get_random_user())
+
+        CircleMember.objects.create(circle=self.circle, user=self.user, is_admin=True)
+        other_user = get_random_user()
+        ar = CircleAccessRequest.objects.create(circle=self.circle, user=other_user, status='Pending')
+        self.assertFalse(CircleMember.objects.filter(user=other_user, circle=self.circle).exists())
+
+        payload = self._get_request_json()
+        payload.update({
+            'status': 'Accepted'
+        })
+
+        response = self.client.patch('/circleaccessrequests/{}/'.format(ar.pk),
+                                     data=json.dumps(payload), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 200)
+        ar = self.circle.access_requests.all()[0]
+        self.assertEqual(ar.status, payload['status'])
+        self.assertTrue(CircleMember.objects.filter(user=other_user, circle=self.circle).exists())
+    
+    def test_respond_access_request_not_admin(self):
+        self.setUpLoggedInUser()
+        self.setUpCircle('Restrict', get_random_user())
+
+        CircleMember.objects.create(circle=self.circle, user=self.user, is_admin=False)
+        ar = CircleAccessRequest.objects.create(circle=self.circle, user=get_random_user(), status='Pending')
+
+        payload = self._get_request_json()
+        payload.update({
+            'status': 'Accepted'
+        })
+
+        response = self.client.patch('/circleaccessrequests/{}/'.format(ar.pk),
+                                     data=json.dumps(payload), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 404)
+    
+    def test_access_request_removed_when_user_removed(self):
+        self.setUpLoggedInUser()
+        self.setUpCircle('Restrict', self.user)
+
+        other_user = get_random_user()
+        ar = CircleAccessRequest.objects.create(circle=self.circle, user=other_user, status='Accepted')
+        cm = CircleMember.objects.get(circle=self.circle, user=other_user)
+
+        cm.delete()
+        ar = CircleAccessRequest.objects.filter(pk=ar.pk)
+        self.assertFalse(ar.exists())
```

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_save.py` & `djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_save.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/tests/runner.py` & `djangoldp_circle-3.0.0/djangoldp_circle/tests/runner.py`

 * *Files 17% similar despite different names*

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
-    'ldppackages': ['djangoldp_account', 'djangoldp_circle', 'djangoldp_circle.tests'],
+    'ldppackages': ['djangoldp_account', 'djangoldp_circle', 'djangoldp_circle.tests', 'djangoldp_notification'],
 
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
@@ -39,10 +40,11 @@
 
 failures = test_runner.run_tests([
     'djangoldp_circle.tests.tests_permissions',
     'djangoldp_circle.tests.tests_save',
     'djangoldp_circle.tests.tests_view',
     'djangoldp_circle.tests.tests_post',
     'djangoldp_circle.tests.tests_cache',
+    'djangoldp_circle.tests.tests_notifications',
 ])
 if failures:
     sys.exit(failures)
```

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_post.py` & `djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_cache.py` & `djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_view.py` & `djangoldp_circle-3.0.0/djangoldp_circle/tests/tests_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-import uuid
-import json
-from datetime import datetime, timedelta
-
-from djangoldp.permissions import LDPPermissions
-
 from rest_framework.test import APITestCase, APIClient
-from guardian.shortcuts import assign_perm
-
-from djangoldp_circle.models import Circle, CircleMember
+from djangoldp_circle.models import Circle
 from djangoldp_circle.tests.utils import get_random_user
 
 
 class ViewTestCase(APITestCase):
     def setUp(self):
         self.client = APIClient()
```

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0015_auto_20200505_1733.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0015_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0024_auto_20200925_1108.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0024_auto_20200925_1108.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0010_auto_20200414_0908.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0010_auto_20200414_0908.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0011_auto_20200426_1632.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0011_auto_20200426_1632.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0009_auto_20200226_1742.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0009_auto_20200226_1742.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0005_auto_20191029_1227.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0005_auto_20191029_1227.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0007_auto_20191112_1251.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0007_auto_20191112_1251.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0020_auto_20200610_1323.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0020_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0023_auto_20200617_1817.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0023_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0028_auto_20210204_1904.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0028_auto_20210204_1904.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0029_auto_20210211_1244.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0029_auto_20210211_1244.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0014_auto_20200501_1207.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0014_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0013_auto_20200506_1503.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0013_auto_20200506_1503.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0029_auto_20210211_1440.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0029_auto_20210211_1440.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0014_auto_20200506_1517.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0014_auto_20200506_1517.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0001_initial.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0013_auto_20200429_1346.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0013_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0006_circle_status.py` & `djangoldp_circle-3.0.0/djangoldp_circle/migrations/0006_circle_status.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/management/commands/mock_circle.py` & `djangoldp_circle-3.0.0/djangoldp_circle/management/commands/mock_circle.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle/filters.py` & `djangoldp_circle-3.0.0/djangoldp_circle/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         elif is_anonymous_user(request.user):
             return queryset.filter(status='Public')
         else:
             objects = super().filter_queryset(request, queryset, view).values_list('pk')
             return queryset.filter(
                 Q(members__user=request.user) |
                 Q(status='Public') |
+                Q(status='Restricted') |
                 Q(pk__in=objects)
             ).distinct()
 
 
 class CircleMemberFilterBackend(ObjectPermissionsFilter):
     def filter_queryset(self, request, queryset, view):
         if get_client_ip(request) in XMPP_SERVERS:
@@ -32,7 +33,27 @@
             objects = super().filter_queryset(request, queryset, view).values_list('pk')
             return queryset.filter(
                 Q(user=request.user) |
                 Q(circle__status='Public') |
                 Q(circle__members__user=request.user) |
                 Q(pk__in=objects)
             ).distinct()
+
+
+class CircleAccessRequestFilterBackend(ObjectPermissionsFilter):
+    def filter_queryset(self, request, queryset, view):
+        from djangoldp_circle.models import CircleMember
+
+        if get_client_ip(request) in XMPP_SERVERS:
+            return queryset
+        elif is_anonymous_user(request.user):
+            return view.model.objects.none()
+        else:
+            # objects which I have permissions on by grace of my superclass (e.g. object permissions)
+            objects = super().filter_queryset(request, queryset, view).values_list('pk', flat=True)
+            # unite it with the circles for which I am an administrator
+            objects = list(set(objects).union(CircleMember.objects.filter(user=request.user, is_admin=True).values_list('circle', flat=True)))
+
+            return queryset.filter(
+                Q(user=request.user) |
+                Q(circle__pk__in=objects)
+            ).distinct()
```

### Comparing `djangoldp_circle-2.1.9/README.md` & `djangoldp_circle-3.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+# Synopsis
+
+Circles represent groups of people, and can optionally support a chat mechanic in co-operation with XMPP
+
 # Permissions on Circles
 
-Circles can be **Public**, **Private** or **Archived**
+Standard Circles can be **Public**, **Private** or **Archived**
 
 Anonymous users can view public circles
 
 Authenticated users can view public circles and add to them. You can change this in the settings :
 ```
 # default value :
 USER_AUTHENTICATED_CIRCLE_PERMISSIONS=['view', 'add']
@@ -12,12 +16,18 @@
 USER_AUTHENTICATED_CIRCLE_PERMISSIONS=['view']
 ```
 
 If a user is a **member** of a private circle (they have been added by another member, or the circle's creator), then they can view the circle, and add to it
 
 If a member is an **admin** of a circle then they can change information about the circle and delete it. They can add other users as administrators, or delete members, but they can't delete other administrators, or delete themselves if they are the last administrator
 
+Circles can also be **Restricted**, which makes them Private circles which a user can request access to. When an administrator accepts their request, they will be added to the circle membership
+
 As with all DjangoLDP models, individual users may also be given permissions individually on circles
 
 ## Allow XMPP server to access private datas
 
 By default, our Prosody server is allowed to access any Circle information, for membership purpose. You can set it to your own server by adding `XMPP_SERVER_IP` to your packages.yml.
+
+## Changelog
+
+Now supports Django4.2 and Python3.11
```

### Comparing `djangoldp_circle-2.1.9/djangoldp_circle.egg-info/SOURCES.txt` & `djangoldp_circle-3.0.0/djangoldp_circle.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,37 @@
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 djangoldp_circle/__init__.py
 djangoldp_circle/admin.py
 djangoldp_circle/apps.py
 djangoldp_circle/check_integrity.py
 djangoldp_circle/djangoldp_urls.py
 djangoldp_circle/factories.py
 djangoldp_circle/filters.py
 djangoldp_circle/models.py
 djangoldp_circle/permissions.py
+djangoldp_circle/serializers.py
 djangoldp_circle/settings.py
 djangoldp_circle/views.py
 djangoldp_circle/xmpp.py
 djangoldp_circle.egg-info/PKG-INFO
 djangoldp_circle.egg-info/SOURCES.txt
 djangoldp_circle.egg-info/dependency_links.txt
 djangoldp_circle.egg-info/requires.txt
 djangoldp_circle.egg-info/top_level.txt
+djangoldp_circle/locale/de/LC_MESSAGES/django.mo
+djangoldp_circle/locale/de/LC_MESSAGES/django.po
+djangoldp_circle/locale/en/LC_MESSAGES/django.mo
+djangoldp_circle/locale/en/LC_MESSAGES/django.po
+djangoldp_circle/locale/es/LC_MESSAGES/django.mo
+djangoldp_circle/locale/es/LC_MESSAGES/django.po
+djangoldp_circle/locale/fr/LC_MESSAGES/django.mo
+djangoldp_circle/locale/fr/LC_MESSAGES/django.po
 djangoldp_circle/management/__init__.py
 djangoldp_circle/management/commands/__init__.py
 djangoldp_circle/management/commands/mock_circle.py
 djangoldp_circle/migrations/0001_initial.py
 djangoldp_circle/migrations/0002_auto_20191021_1357.py
 djangoldp_circle/migrations/0003_auto_20191024_1604.py
 djangoldp_circle/migrations/0004_auto_20191024_1831.py
@@ -48,16 +58,25 @@
 djangoldp_circle/migrations/0025_remove_circle_team.py
 djangoldp_circle/migrations/0026_auto_20210115_1038.py
 djangoldp_circle/migrations/0027_circle_description.py
 djangoldp_circle/migrations/0028_auto_20210204_1904.py
 djangoldp_circle/migrations/0029_auto_20210211_1244.py
 djangoldp_circle/migrations/0029_auto_20210211_1440.py
 djangoldp_circle/migrations/0030_merge_20210211_1453.py
+djangoldp_circle/migrations/0031_circle_parentcircle.py
+djangoldp_circle/migrations/0032_auto_20220304_1046.py
+djangoldp_circle/migrations/0033_auto_20220317_1915.py
+djangoldp_circle/migrations/0034_auto_20220412_1337.py
+djangoldp_circle/migrations/0035_alter_circle_options_alter_circlemember_options.py
 djangoldp_circle/migrations/__init__.py
+djangoldp_circle/templates/__init__.py
+djangoldp_circle/templates/accessrequests/access_requested.html
+djangoldp_circle/templates/accessrequests/access_resolved.html
 djangoldp_circle/tests/__init__.py
 djangoldp_circle/tests/runner.py
 djangoldp_circle/tests/tests_cache.py
+djangoldp_circle/tests/tests_notifications.py
 djangoldp_circle/tests/tests_permissions.py
 djangoldp_circle/tests/tests_post.py
 djangoldp_circle/tests/tests_save.py
 djangoldp_circle/tests/tests_view.py
 djangoldp_circle/tests/utils.py
```

