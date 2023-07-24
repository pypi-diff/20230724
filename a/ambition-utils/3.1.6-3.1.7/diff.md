# Comparing `tmp/ambition-utils-3.1.6.tar.gz` & `tmp/ambition-utils-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambition-utils-3.1.6.tar", last modified: Wed Jun 28 19:35:10 2023, max compression
+gzip compressed data, was "ambition-utils-3.1.7.tar", last modified: Mon Jul 24 13:58:37 2023, max compression
```

## Comparing `ambition-utils-3.1.6.tar` & `ambition-utils-3.1.7.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/LICENSE
--rw-rw-r--   0 wes       (1000) wes       (1000)       68 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/MANIFEST.in
--rw-rw-r--   0 wes       (1000) wes       (1000)     1975 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1114 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/README.rst
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/
--rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/activity/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/activity/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/activity/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     2231 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/activity/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1656 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/activity/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4446 2023-06-26 19:14:11.000000 ambition-utils-3.1.6/ambition_utils/activity/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2737 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/activity/tasks.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/activity/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/activity/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      229 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/activity/tests/model_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2794 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/activity/tests/task_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/anomaly/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/anomaly/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     9762 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/anomaly/models.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/anomaly/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/anomaly/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     6036 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/anomaly/tests/anomaly_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      202 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/anomaly/tests/apps.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/anomaly/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     2644 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/anomaly/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/anomaly/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      928 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/anomaly/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      138 2023-01-06 21:50:12.000000 ambition-utils-3.1.6/ambition_utils/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2545 2023-06-28 18:35:56.000000 ambition-utils-3.1.6/ambition_utils/fields.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    13636 2022-02-17 21:55:47.000000 ambition-utils-3.1.6/ambition_utils/forms.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/postgres_lock/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3782 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/lock.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/postgres_lock/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)      487 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      434 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      581 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      875 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/models.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils/postgres_lock/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4399 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/postgres_lock/tests/lock_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/ambition_utils/rrule/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/rrule/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      162 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/rrule/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      127 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/rrule/constants.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     9796 2023-06-26 21:32:04.000000 ambition-utils-3.1.6/ambition_utils/rrule/forms.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      389 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/rrule/handler.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/ambition_utils/rrule/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)      927 2023-06-28 19:28:24.000000 ambition-utils-3.1.6/ambition_utils/rrule/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      415 2023-06-28 19:28:24.000000 ambition-utils-3.1.6/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      936 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      486 2023-06-26 21:32:04.000000 ambition-utils-3.1.6/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/rrule/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    18825 2023-06-27 21:01:00.000000 ambition-utils-3.1.6/ambition_utils/rrule/models.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/ambition_utils/rrule/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/rrule/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      200 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/rrule/tests/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    17567 2023-06-26 21:32:04.000000 ambition-utils-3.1.6/ambition_utils/rrule/tests/form_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/ambition_utils/rrule/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1005 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/rrule/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/rrule/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    56586 2023-06-26 21:32:04.000000 ambition-utils-3.1.6/ambition_utils/rrule/tests/model_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      713 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/rrule/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7349 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/sql.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/ambition_utils/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      190 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/tests/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2556 2023-06-26 21:33:07.000000 ambition-utils-3.1.6/ambition_utils/tests/field_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    16249 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/tests/form_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/ambition_utils/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)      489 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      685 2023-06-28 19:28:24.000000 ambition-utils-3.1.6/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      364 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3144 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/tests/sql_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3435 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/tests/time_helper_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4765 2023-01-24 18:43:16.000000 ambition-utils-3.1.6/ambition_utils/time_helpers.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/ambition_utils/transaction/
--rw-rw-r--   0 wes       (1000) wes       (1000)       46 2022-02-17 21:55:47.000000 ambition-utils-3.1.6/ambition_utils/transaction/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2261 2022-02-17 21:55:47.000000 ambition-utils-3.1.6/ambition_utils/transaction/decorators.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/ambition_utils/transaction/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2022-02-17 21:55:47.000000 ambition-utils-3.1.6/ambition_utils/transaction/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2032 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/ambition_utils/transaction/tests/durable_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2666 2022-02-17 21:55:47.000000 ambition-utils-3.1.6/ambition_utils/transaction/utils.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/ambition_utils/urls.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-28 19:30:55.000000 ambition-utils-3.1.6/ambition_utils/version.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.017134 ambition-utils-3.1.6/ambition_utils.egg-info/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1975 2023-06-28 19:35:10.000000 ambition-utils-3.1.6/ambition_utils.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     3085 2023-06-28 19:35:10.000000 ambition-utils-3.1.6/ambition_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-28 19:35:10.000000 ambition-utils-3.1.6/ambition_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      262 2023-06-28 19:35:10.000000 ambition-utils-3.1.6/ambition_utils.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       15 2023-06-28 19:35:10.000000 ambition-utils-3.1.6/ambition_utils.egg-info/top_level.txt
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/requirements/
--rw-rw-r--   0 wes       (1000) wes       (1000)       31 2022-02-11 17:04:09.000000 ambition-utils-3.1.6/requirements/docs.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       96 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/requirements/requirements-testing.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      160 2023-06-26 21:33:07.000000 ambition-utils-3.1.6/requirements/requirements.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      252 2023-06-28 19:35:10.021134 ambition-utils-3.1.6/setup.cfg
--rw-rw-r--   0 wes       (1000) wes       (1000)     1914 2023-06-26 21:29:57.000000 ambition-utils-3.1.6/setup.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.592221 ambition-utils-3.1.7/
+-rw-r--r--   0 tneu       (501) staff       (20)     1075 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/LICENSE
+-rw-r--r--   0 tneu       (501) staff       (20)       68 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/MANIFEST.in
+-rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-07-24 13:58:37.592290 ambition-utils-3.1.7/PKG-INFO
+-rw-r--r--   0 tneu       (501) staff       (20)     1114 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/README.rst
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.579753 ambition-utils-3.1.7/ambition_utils/
+-rw-r--r--   0 tneu       (501) staff       (20)       48 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/__init__.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.580984 ambition-utils-3.1.7/ambition_utils/activity/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/activity/__init__.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.581583 ambition-utils-3.1.7/ambition_utils/activity/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     2231 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/activity/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)     1656 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/activity/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4446 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/activity/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2737 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/activity/tasks.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.581968 ambition-utils-3.1.7/ambition_utils/activity/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/activity/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      229 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/activity/tests/model_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2794 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/activity/tests/task_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.582242 ambition-utils-3.1.7/ambition_utils/anomaly/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/anomaly/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     9762 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/anomaly/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.582895 ambition-utils-3.1.7/ambition_utils/anomaly/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     6036 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/anomaly_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)      202 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/apps.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.583197 ambition-utils-3.1.7/ambition_utils/anomaly/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     2644 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      928 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/anomaly/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)      138 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2545 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/fields.py
+-rw-r--r--   0 tneu       (501) staff       (20)    13636 2023-01-26 16:48:58.000000 ambition-utils-3.1.7/ambition_utils/forms.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.583658 ambition-utils-3.1.7/ambition_utils/postgres_lock/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3782 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/lock.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.584403 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      487 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      434 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
+-rw-r--r--   0 tneu       (501) staff       (20)      581 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      875 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.584608 ambition-utils-3.1.7/ambition_utils/postgres_lock/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4399 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/postgres_lock/tests/lock_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.585744 ambition-utils-3.1.7/ambition_utils/rrule/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/rrule/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      162 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)      127 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/rrule/constants.py
+-rw-r--r--   0 tneu       (501) staff       (20)     9900 2023-07-20 18:18:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/forms.py
+-rw-r--r--   0 tneu       (501) staff       (20)      389 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/rrule/handler.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.587303 ambition-utils-3.1.7/ambition_utils/rrule/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      927 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      415 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
+-rw-r--r--   0 tneu       (501) staff       (20)      936 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
+-rw-r--r--   0 tneu       (501) staff       (20)      486 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/rrule/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)    18825 2023-07-20 21:45:03.000000 ambition-utils-3.1.7/ambition_utils/rrule/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.588442 ambition-utils-3.1.7/ambition_utils/rrule/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      200 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)    18459 2023-07-20 18:18:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/form_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.588755 ambition-utils-3.1.7/ambition_utils/rrule/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     1005 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)    56586 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/model_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)      713 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/rrule/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     7349 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/sql.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.590078 ambition-utils-3.1.7/ambition_utils/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      190 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2556 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/tests/field_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)    16249 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/tests/form_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.590676 ambition-utils-3.1.7/ambition_utils/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      489 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      685 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      364 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3144 2023-07-20 17:55:28.000000 ambition-utils-3.1.7/ambition_utils/tests/sql_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3435 2022-11-29 21:40:08.000000 ambition-utils-3.1.7/ambition_utils/tests/time_helper_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4765 2022-11-29 21:40:08.000000 ambition-utils-3.1.7/ambition_utils/time_helpers.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.591284 ambition-utils-3.1.7/ambition_utils/transaction/
+-rw-r--r--   0 tneu       (501) staff       (20)       46 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/transaction/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2261 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/transaction/decorators.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.591564 ambition-utils-3.1.7/ambition_utils/transaction/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/transaction/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2032 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/ambition_utils/transaction/tests/durable_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2666 2022-08-25 21:39:28.000000 ambition-utils-3.1.7/ambition_utils/transaction/utils.py
+-rw-r--r--   0 tneu       (501) staff       (20)       38 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/ambition_utils/urls.py
+-rw-r--r--   0 tneu       (501) staff       (20)       22 2023-07-20 21:59:50.000000 ambition-utils-3.1.7/ambition_utils/version.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.580468 ambition-utils-3.1.7/ambition_utils.egg-info/
+-rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/PKG-INFO
+-rw-r--r--   0 tneu       (501) staff       (20)     3085 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 tneu       (501) staff       (20)        1 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      262 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/requires.txt
+-rw-r--r--   0 tneu       (501) staff       (20)       15 2023-07-24 13:58:37.000000 ambition-utils-3.1.7/ambition_utils.egg-info/top_level.txt
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-07-24 13:58:37.592085 ambition-utils-3.1.7/requirements/
+-rw-r--r--   0 tneu       (501) staff       (20)       31 2022-08-25 20:38:52.000000 ambition-utils-3.1.7/requirements/docs.txt
+-rw-r--r--   0 tneu       (501) staff       (20)       96 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/requirements/requirements-testing.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      160 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/requirements/requirements.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      252 2023-07-24 13:58:37.592647 ambition-utils-3.1.7/setup.cfg
+-rw-r--r--   0 tneu       (501) staff       (20)     1914 2023-07-20 17:58:01.000000 ambition-utils-3.1.7/setup.py
```

### Comparing `ambition-utils-3.1.6/LICENSE` & `ambition-utils-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/PKG-INFO` & `ambition-utils-3.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.6
+Version: 3.1.7
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Keywords: django,database,query,sql,postgres,upsert
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -59,7 +60,9 @@
 If you need Python2 support, pin to `ambition-utils==0.4.0`
 
 Full documentation is available at http://ambition-utils.readthedocs.org
 
 License
 -------
 MIT License (see LICENSE)
+
+
```

### Comparing `ambition-utils-3.1.6/README.rst` & `ambition-utils-3.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/activity/migrations/0001_initial.py` & `ambition-utils-3.1.7/ambition_utils/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/activity/migrations/0002_auto_20180427_1819.py` & `ambition-utils-3.1.7/ambition_utils/activity/migrations/0002_auto_20180427_1819.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/activity/models.py` & `ambition-utils-3.1.7/ambition_utils/activity/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/activity/tasks.py` & `ambition-utils-3.1.7/ambition_utils/activity/tasks.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/activity/tests/task_tests.py` & `ambition-utils-3.1.7/ambition_utils/activity/tests/task_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/anomaly/models.py` & `ambition-utils-3.1.7/ambition_utils/anomaly/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/anomaly/tests/anomaly_tests.py` & `ambition-utils-3.1.7/ambition_utils/anomaly/tests/anomaly_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/anomaly/tests/migrations/0001_initial.py` & `ambition-utils-3.1.7/ambition_utils/anomaly/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/anomaly/tests/models.py` & `ambition-utils-3.1.7/ambition_utils/anomaly/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/fields.py` & `ambition-utils-3.1.7/ambition_utils/fields.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/forms.py` & `ambition-utils-3.1.7/ambition_utils/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/postgres_lock/lock.py` & `ambition-utils-3.1.7/ambition_utils/postgres_lock/lock.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py` & `ambition-utils-3.1.7/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/postgres_lock/models.py` & `ambition-utils-3.1.7/ambition_utils/postgres_lock/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/postgres_lock/tests/lock_tests.py` & `ambition-utils-3.1.7/ambition_utils/postgres_lock/tests/lock_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/rrule/forms.py` & `ambition-utils-3.1.7/ambition_utils/rrule/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,20 +246,21 @@
         return rrule_exclusion_form.get_rrule_params_from_cleaned_data()
 
     def save(self, **kwargs):
         """
         Saves the RRule model and returns it
         """
         # Keep track if this is an existing rrule that needs occurrence updated
-        need_to_refresh_next_recurrence = False
+        need_to_refresh_next_occurrence = False
 
         # Get the rrule model from the cleaned data
         rrule_model = self.cleaned_data.get('rrule')
         if rrule_model:
-            need_to_refresh_next_recurrence = True
+            # Refresh if the next occurrence is not expired.
+            need_to_refresh_next_occurrence = rrule_model.next_occurrence > datetime.utcnow()
         else:
             # Use the recurrence passed into save kwargs
             rrule_model = kwargs.get('recurrence') or RRule()
 
         # Create or update the rule
         rrule_model.rrule_params = self.get_rrule_params_from_cleaned_data()
         rrule_model.rrule_exclusion_params = self.cleaned_data.get('rrule_exclusion')
@@ -269,14 +270,14 @@
                 # This try except is because some field names might be reverse foreign key relationships
                 try:
                     setattr(rrule_model, key, value)
                 except TypeError:  # pragma: no cover
                     pass
 
         # Check if this was an existing model that needs to have its next occurrence updated
-        if need_to_refresh_next_recurrence:
+        if need_to_refresh_next_occurrence:
             rrule_model.refresh_next_occurrence()
 
         rrule_model.save()
 
         # Return the rule
         return rrule_model
```

### Comparing `ambition-utils-3.1.6/ambition_utils/rrule/migrations/0001_initial.py` & `ambition-utils-3.1.7/ambition_utils/rrule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py` & `ambition-utils-3.1.7/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/rrule/models.py` & `ambition-utils-3.1.7/ambition_utils/rrule/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/rrule/tests/form_tests.py` & `ambition-utils-3.1.7/ambition_utils/rrule/tests/form_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -446,54 +446,61 @@
         rrule_model = form.save(
             occurrence_handler_path='ambition_utils.rrule.handler.OccurrenceHandler',
             fake_recurrence=form
         )
 
         self.assertEqual(rrule_model.occurrence_handler_path, 'ambition_utils.rrule.handler.OccurrenceHandler')
 
-    @freeze_time(datetime.datetime(2017, 6, 4))
-    def test_update_from_id_field(self):
+    def test_update(self):
         """
-        Verifies that an existing rrule object will get updated from passing an id in the form data and that
-        the next recurrence is refreshed
+        Verifies an existing RRule object will be updated when the id of the RRule object is passed in the form data.
+        The next occurrence is refreshed when the occurrence is not expired to ensure the next occurrence is not
+        updated before its handler runs.
         """
-        data = {
-            'freq': rrule.DAILY,
-            'interval': 1,
-            'dtstart': '6/4/2017',
-            'byhour': '0',
-            'time_zone': 'UTC',
-            'ends': RecurrenceEnds.NEVER,
-        }
-        form = RecurrenceForm(data=data)
-        self.assertTrue(form.is_valid())
-        rrule_model = form.save(
-            occurrence_handler_path='ambition_utils.rrule.handler.OccurrenceHandler',
-        )
-        self.assertEqual(RRule.objects.count(), 1)
-        self.assertEqual(rrule_model.next_occurrence, datetime.datetime(2017, 6, 4))
+        # Create an object, update its next occurrence, and assert it changes.
+        with freeze_time(datetime.datetime(2017, 6, 4)):
+            data = {
+                'freq': rrule.DAILY,
+                'interval': 1,
+                'dtstart': '6/4/2017',
+                'byhour': '0',
+                'time_zone': 'UTC',
+                'ends': RecurrenceEnds.NEVER,
+            }
+            form = RecurrenceForm(data=data)
+            self.assertTrue(form.is_valid())
+            rrule_model = form.save(
+                occurrence_handler_path='ambition_utils.rrule.handler.OccurrenceHandler',
+            )
+            self.assertEqual(RRule.objects.count(), 1)
+            self.assertEqual(rrule_model.next_occurrence, datetime.datetime(2017, 6, 4))
 
-        # Handle update
-        data = {
-            'rrule': str(rrule_model.id),
-            'freq': rrule.DAILY,
-            'interval': 1,
-            'dtstart': '6/7/2017',
-            'byhour': '0',
-            'time_zone': 'UTC',
-            'ends': RecurrenceEnds.NEVER,
-        }
+            # Handle overdue and assert next day.
+            RRule.objects.update_next_occurrences([rrule_model])
+            self.assertEqual(rrule_model.next_occurrence, datetime.datetime(2017, 6, 5))
 
-        form = RecurrenceForm(data=data)
-        self.assertTrue(form.is_valid())
-        rrule_model = form.save(
-            occurrence_handler_path='ambition_utils.rrule.handler.OccurrenceHandler',
-        )
-        self.assertEqual(RRule.objects.count(), 1)
-        self.assertEqual(rrule_model.next_occurrence, datetime.datetime(2017, 6, 7))
+        # Next day. Update object's start date, by passing RRule.id along. Ensure next occurrence is not updated
+        # by the update since it's overdue.
+        with freeze_time(datetime.datetime(2017, 6, 5)):
+            data['rrule'] = str(rrule_model.id)
+            data['dtstart'] = '6/7/2017'
+
+            form = RecurrenceForm(data=data)
+            self.assertTrue(form.is_valid())
+            rrule_model = form.save(
+                occurrence_handler_path='ambition_utils.rrule.handler.OccurrenceHandler',
+            )
+            self.assertEqual(RRule.objects.count(), 1)
+
+            # Next occurrence should not be updated because it is expired and needs to be resolved by its handler.
+            self.assertEqual(rrule_model.next_occurrence, datetime.datetime(2017, 6, 5))
+
+            # Handle overdue and assert next occurrence now reflects the new start date instead of the next day, 6/6.
+            RRule.objects.update_next_occurrences([rrule_model])
+            self.assertEqual(rrule_model.next_occurrence, datetime.datetime(2017, 6, 7))
 
     def test_exclusion_rule(self):
         exclusion_data = {
             'freq': rrule.MONTHLY,
             'interval': 1,
             'dtstart': '6/1/2023',
             'byhour': '0',
```

### Comparing `ambition-utils-3.1.6/ambition_utils/rrule/tests/migrations/0001_initial.py` & `ambition-utils-3.1.7/ambition_utils/rrule/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/rrule/tests/model_tests.py` & `ambition-utils-3.1.7/ambition_utils/rrule/tests/model_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/rrule/tests/models.py` & `ambition-utils-3.1.7/ambition_utils/rrule/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/sql.py` & `ambition-utils-3.1.7/ambition_utils/sql.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/tests/field_tests.py` & `ambition-utils-3.1.7/ambition_utils/tests/field_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/tests/form_tests.py` & `ambition-utils-3.1.7/ambition_utils/tests/form_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/tests/migrations/0002_auto_20230124_1754.py` & `ambition-utils-3.1.7/ambition_utils/tests/migrations/0002_auto_20230124_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/tests/sql_tests.py` & `ambition-utils-3.1.7/ambition_utils/tests/sql_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/tests/time_helper_tests.py` & `ambition-utils-3.1.7/ambition_utils/tests/time_helper_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/time_helpers.py` & `ambition-utils-3.1.7/ambition_utils/time_helpers.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/transaction/decorators.py` & `ambition-utils-3.1.7/ambition_utils/transaction/decorators.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/transaction/tests/durable_tests.py` & `ambition-utils-3.1.7/ambition_utils/transaction/tests/durable_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils/transaction/utils.py` & `ambition-utils-3.1.7/ambition_utils/transaction/utils.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/ambition_utils.egg-info/PKG-INFO` & `ambition-utils-3.1.7/ambition_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.6
+Version: 3.1.7
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Keywords: django,database,query,sql,postgres,upsert
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -59,7 +60,9 @@
 If you need Python2 support, pin to `ambition-utils==0.4.0`
 
 Full documentation is available at http://ambition-utils.readthedocs.org
 
 License
 -------
 MIT License (see LICENSE)
+
+
```

### Comparing `ambition-utils-3.1.6/ambition_utils.egg-info/SOURCES.txt` & `ambition-utils-3.1.7/ambition_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.6/setup.py` & `ambition-utils-3.1.7/setup.py`

 * *Files identical despite different names*

