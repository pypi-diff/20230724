# Comparing `tmp/djangoldp_circle-2.1.8.tar.gz` & `tmp/djangoldp_circle-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_circle-2.1.8.tar", last modified: Tue Apr 27 15:46:57 2021, max compression
+gzip compressed data, was "dist/djangoldp_circle-2.1.9.tar", last modified: Tue May 25 10:13:02 2021, max compression
```

## Comparing `djangoldp_circle-2.1.8.tar` & `djangoldp_circle-2.1.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      595 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle/
--rw-rw-rw-   0 root         (0) root         (0)       32 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     5929 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/models.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3764 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1660 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/views.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/xmpp.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     2905 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/
--rw-rw-rw-   0 root         (0) root         (0)    18326 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_save.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)     2348 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_view.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      464 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0002_auto_20191021_1357.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0019_auto_20200522_1516.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0015_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0024_auto_20200925_1108.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0010_auto_20200414_0908.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0027_circle_description.py
--rw-rw-rw-   0 root         (0) root         (0)      930 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0011_auto_20200426_1632.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0018_auto_20200512_1352.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0026_auto_20210115_1038.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0008_circlemember_is_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0009_auto_20200226_1742.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0005_auto_20191029_1227.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0007_auto_20191112_1251.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0020_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0023_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0017_auto_20200512_1348.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0025_remove_circle_team.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0016_merge_20200506_1904.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0012_auto_20200427_1047.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0028_auto_20210204_1904.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0030_merge_20210211_1453.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0029_auto_20210211_1244.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0003_auto_20191024_1604.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0014_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0013_auto_20200506_1503.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0029_auto_20210211_1440.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0014_auto_20200506_1517.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0004_auto_20191024_1831.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0013_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/0006_circle_status.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      908 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/management/commands/mock_circle.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/djangoldp_circle/filters.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2021-04-27 15:46:55.000000 djangoldp_circle-2.1.8/djangoldp_circle/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-04-27 15:46:43.000000 djangoldp_circle-2.1.8/setup.py
--rw-r--r--   0 root         (0) root         (0)      313 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2743 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      313 2021-04-27 15:46:57.000000 djangoldp_circle-2.1.8/djangoldp_circle.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6192 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3764 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1660 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/xmpp.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     2905 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    18326 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_save.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_view.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0002_auto_20191021_1357.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0019_auto_20200522_1516.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0015_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0024_auto_20200925_1108.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0010_auto_20200414_0908.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0027_circle_description.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0011_auto_20200426_1632.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0018_auto_20200512_1352.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0026_auto_20210115_1038.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0008_circlemember_is_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0009_auto_20200226_1742.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0005_auto_20191029_1227.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0007_auto_20191112_1251.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0020_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0023_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0017_auto_20200512_1348.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0025_remove_circle_team.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0016_merge_20200506_1904.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0012_auto_20200427_1047.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0028_auto_20210204_1904.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0030_merge_20210211_1453.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0029_auto_20210211_1244.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0003_auto_20191024_1604.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0014_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0013_auto_20200506_1503.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0029_auto_20210211_1440.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0014_auto_20200506_1517.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0004_auto_20191024_1831.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0013_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/0006_circle_status.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      908 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/commands/mock_circle.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/management/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/djangoldp_circle/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2021-05-25 10:12:59.000000 djangoldp_circle-2.1.9/djangoldp_circle/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2021-05-25 10:12:46.000000 djangoldp_circle-2.1.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)      313 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2021-05-25 10:13:01.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2021-05-25 10:13:01.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2021-05-25 10:13:01.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2743 2021-05-25 10:13:02.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      313 2021-05-25 10:13:01.000000 djangoldp_circle-2.1.9/djangoldp_circle.egg-info/PKG-INFO
```

### Comparing `djangoldp_circle-2.1.8/setup.cfg` & `djangoldp_circle-2.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/models.py` & `djangoldp_circle-2.1.9/djangoldp_circle/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,14 +20,23 @@
     ('Archived', 'Archived'),
 ]
 
 circle_fields = ["@id", "name", "subtitle", "description", "creationDate", "status", "owner", "jabberID", "jabberRoom", "members"]
 if 'djangoldp_community' in settings.DJANGOLDP_PACKAGES:
     circle_fields += ['community']
 
+if 'djangoldp_polls' in settings.DJANGOLDP_PACKAGES:
+    circle_fields += ['polls']
+
+if 'djangoldp_resource' in settings.DJANGOLDP_PACKAGES:
+    circle_fields += ['resources']
+
+if 'djangoldp_event' in settings.DJANGOLDP_PACKAGES:
+    circle_fields += ['events']
+
 
 class Circle(Model):
     name = models.CharField(max_length=255, blank=True, null=True, default='')
     subtitle = models.CharField(max_length=255, blank=True, null=True, default='')
     description = models.TextField(blank=True, null=True, default='')
     creationDate = models.DateField(auto_now_add=True)
     status = models.CharField(max_length=8, choices=STATUS_CHOICES, default='Public')
```

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/permissions.py` & `djangoldp_circle-2.1.9/djangoldp_circle/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/djangoldp_urls.py` & `djangoldp_circle-2.1.9/djangoldp_circle/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/views.py` & `djangoldp_circle-2.1.9/djangoldp_circle/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/factories.py` & `djangoldp_circle-2.1.9/djangoldp_circle/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/check_integrity.py` & `djangoldp_circle-2.1.9/djangoldp_circle/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/admin.py` & `djangoldp_circle-2.1.9/djangoldp_circle/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_permissions.py` & `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_save.py` & `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_save.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/tests/runner.py` & `djangoldp_circle-2.1.9/djangoldp_circle/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_post.py` & `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_cache.py` & `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/tests/tests_view.py` & `djangoldp_circle-2.1.9/djangoldp_circle/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0015_auto_20200505_1733.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0015_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0024_auto_20200925_1108.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0024_auto_20200925_1108.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0010_auto_20200414_0908.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0010_auto_20200414_0908.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0011_auto_20200426_1632.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0011_auto_20200426_1632.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0009_auto_20200226_1742.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0009_auto_20200226_1742.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0005_auto_20191029_1227.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0005_auto_20191029_1227.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0007_auto_20191112_1251.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0007_auto_20191112_1251.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0020_auto_20200610_1323.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0020_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0023_auto_20200617_1817.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0023_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0028_auto_20210204_1904.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0028_auto_20210204_1904.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0029_auto_20210211_1244.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0029_auto_20210211_1244.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0014_auto_20200501_1207.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0014_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0013_auto_20200506_1503.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0013_auto_20200506_1503.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0029_auto_20210211_1440.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0029_auto_20210211_1440.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0014_auto_20200506_1517.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0014_auto_20200506_1517.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0001_initial.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0013_auto_20200429_1346.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0013_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/migrations/0006_circle_status.py` & `djangoldp_circle-2.1.9/djangoldp_circle/migrations/0006_circle_status.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/management/commands/mock_circle.py` & `djangoldp_circle-2.1.9/djangoldp_circle/management/commands/mock_circle.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle/filters.py` & `djangoldp_circle-2.1.9/djangoldp_circle/filters.py`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/README.md` & `djangoldp_circle-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_circle-2.1.8/djangoldp_circle.egg-info/SOURCES.txt` & `djangoldp_circle-2.1.9/djangoldp_circle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

