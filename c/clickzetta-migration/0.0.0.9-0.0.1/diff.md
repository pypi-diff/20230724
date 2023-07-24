# Comparing `tmp/clickzetta-migration-0.0.0.9.tar.gz` & `tmp/clickzetta-migration-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-migration-0.0.0.9.tar", last modified: Wed Jul 19 11:39:37 2023, max compression
+gzip compressed data, was "clickzetta-migration-0.0.1.tar", last modified: Mon Jul 24 02:52:18 2023, max compression
```

## Comparing `clickzetta-migration-0.0.0.9.tar` & `clickzetta-migration-0.0.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.815464 clickzetta-migration-0.0.0.9/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.9/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 11:39:37.815306 clickzetta-migration-0.0.0.9/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.808188 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      141 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-19 11:39:37.000000 clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/top_level.txt
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.808563 clickzetta-migration-0.0.0.9/migration/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.9/migration/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809069 clickzetta-migration-0.0.0.9/migration/base/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.9/migration/base/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.9/migration/base/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.9/migration/base/status.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809273 clickzetta-migration-0.0.0.9/migration/connector/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.9/migration/connector/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809419 clickzetta-migration-0.0.0.9/migration/connector/destination/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809697 clickzetta-migration-0.0.0.9/migration/connector/destination/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/clickzetta/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.809975 clickzetta-migration-0.0.0.9/migration/connector/destination/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/connector/destination/doris/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.810576 clickzetta-migration-0.0.0.9/migration/connector/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.9/migration/connector/source/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.9/migration/connector/source/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.810867 clickzetta-migration-0.0.0.9/migration/connector/source/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.9/migration/connector/source/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7648 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.0.9/migration/connector/source/clickzetta/source.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.811145 clickzetta-migration-0.0.0.9/migration/connector/source/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.9/migration/connector/source/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/connector/source/doris/source.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.9/migration/connector/source/enum.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.811343 clickzetta-migration-0.0.0.9/migration/connector/source/hive/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.9/migration/connector/source/hive/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.811420 clickzetta-migration-0.0.0.9/migration/connector/source/odps/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.9/migration/connector/source/odps/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11946 2023-07-19 08:11:58.000000 clickzetta-migration-0.0.0.9/migration/migration.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.811922 clickzetta-migration-0.0.0.9/migration/scheduler/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.9/migration/scheduler/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.812215 clickzetta-migration-0.0.0.9/migration/scheduler/data_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.9/migration/scheduler/data_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.9/migration/scheduler/data_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.812498 clickzetta-migration-0.0.0.9/migration/scheduler/data_validation/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.9/migration/scheduler/data_validation/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2841 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.0.9/migration/scheduler/data_validation/validation.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.9/migration/scheduler/scheduler.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.812739 clickzetta-migration-0.0.0.9/migration/scheduler/schema_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.9/migration/scheduler/schema_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.9/migration/scheduler/schema_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.813852 clickzetta-migration-0.0.0.9/migration/scheduler/task/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/base_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/data_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/schema_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3741 2023-07-19 11:39:24.000000 clickzetta-migration-0.0.0.9/migration/scheduler/task/validation_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.9/migration/scheduler/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.814019 clickzetta-migration-0.0.0.9/migration/scheduler/unify_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.9/migration/scheduler/unify_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.9/migration/scheduler/unify_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.814303 clickzetta-migration-0.0.0.9/migration/test/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.9/migration/test/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2480 2023-07-19 08:31:48.000000 clickzetta-migration-0.0.0.9/migration/test/util_test.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 11:39:37.815048 clickzetta-migration-0.0.0.9/migration/util/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.9/migration/util/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7705 2023-07-19 08:16:46.000000 clickzetta-migration-0.0.0.9/migration/util/migration_tasks_status.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.9/migration/util/object_storage_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1787 2023-07-19 08:33:07.000000 clickzetta-migration-0.0.0.9/migration/util/script_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-19 11:39:36.000000 clickzetta-migration-0.0.0.9/migration/version.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-19 11:39:37.815506 clickzetta-migration-0.0.0.9/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1503 2023-07-19 08:35:49.000000 clickzetta-migration-0.0.0.9/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.817682 clickzetta-migration-0.0.1/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.1/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      257 2023-07-24 02:52:18.817546 clickzetta-migration-0.0.1/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.809203 clickzetta-migration-0.0.1/clickzetta_migration.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      257 2023-07-24 02:52:18.000000 clickzetta-migration-0.0.1/clickzetta_migration.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-24 02:52:18.000000 clickzetta-migration-0.0.1/clickzetta_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-24 02:52:18.000000 clickzetta-migration-0.0.1/clickzetta_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-24 02:52:18.000000 clickzetta-migration-0.0.1/clickzetta_migration.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-24 02:52:18.000000 clickzetta-migration-0.0.1/clickzetta_migration.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      141 2023-07-24 02:52:18.000000 clickzetta-migration-0.0.1/clickzetta_migration.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-24 02:52:18.000000 clickzetta-migration-0.0.1/clickzetta_migration.egg-info/top_level.txt
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.809615 clickzetta-migration-0.0.1/migration/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.1/migration/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.810335 clickzetta-migration-0.0.1/migration/base/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.1/migration/base/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.1/migration/base/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.1/migration/base/status.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.810599 clickzetta-migration-0.0.1/migration/connector/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.1/migration/connector/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.810794 clickzetta-migration-0.0.1/migration/connector/destination/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.1/migration/connector/destination/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.1/migration/connector/destination/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.811157 clickzetta-migration-0.0.1/migration/connector/destination/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.1/migration/connector/destination/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8253 2023-07-21 03:43:56.000000 clickzetta-migration-0.0.1/migration/connector/destination/clickzetta/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.811460 clickzetta-migration-0.0.1/migration/connector/destination/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.1/migration/connector/destination/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.1/migration/connector/destination/doris/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.812124 clickzetta-migration-0.0.1/migration/connector/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.1/migration/connector/source/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.1/migration/connector/source/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.812402 clickzetta-migration-0.0.1/migration/connector/source/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.1/migration/connector/source/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7648 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.1/migration/connector/source/clickzetta/source.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.812767 clickzetta-migration-0.0.1/migration/connector/source/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.1/migration/connector/source/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6819 2023-07-21 04:45:30.000000 clickzetta-migration-0.0.1/migration/connector/source/doris/source.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.1/migration/connector/source/enum.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.813015 clickzetta-migration-0.0.1/migration/connector/source/hive/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.1/migration/connector/source/hive/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.813092 clickzetta-migration-0.0.1/migration/connector/source/odps/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.1/migration/connector/source/odps/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    12391 2023-07-21 03:13:29.000000 clickzetta-migration-0.0.1/migration/migration.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.813719 clickzetta-migration-0.0.1/migration/scheduler/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.1/migration/scheduler/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.814014 clickzetta-migration-0.0.1/migration/scheduler/data_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.1/migration/scheduler/data_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.1/migration/scheduler/data_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.814296 clickzetta-migration-0.0.1/migration/scheduler/data_validation/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.1/migration/scheduler/data_validation/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2841 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.1/migration/scheduler/data_validation/validation.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.1/migration/scheduler/scheduler.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.814695 clickzetta-migration-0.0.1/migration/scheduler/schema_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.1/migration/scheduler/schema_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.1/migration/scheduler/schema_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.815866 clickzetta-migration-0.0.1/migration/scheduler/task/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.1/migration/scheduler/task/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.1/migration/scheduler/task/base_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.1/migration/scheduler/task/data_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.1/migration/scheduler/task/schema_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3747 2023-07-19 11:49:03.000000 clickzetta-migration-0.0.1/migration/scheduler/task/validation_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.1/migration/scheduler/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.816201 clickzetta-migration-0.0.1/migration/scheduler/unify_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.1/migration/scheduler/unify_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.1/migration/scheduler/unify_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.816507 clickzetta-migration-0.0.1/migration/test/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.1/migration/test/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2574 2023-07-19 11:49:03.000000 clickzetta-migration-0.0.1/migration/test/util_test.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-24 02:52:18.817266 clickzetta-migration-0.0.1/migration/util/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.1/migration/util/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7703 2023-07-20 03:36:13.000000 clickzetta-migration-0.0.1/migration/util/migration_tasks_status.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.1/migration/util/object_storage_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1787 2023-07-19 08:33:07.000000 clickzetta-migration-0.0.1/migration/util/script_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-07-24 02:52:16.000000 clickzetta-migration-0.0.1/migration/version.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-24 02:52:18.817724 clickzetta-migration-0.0.1/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1503 2023-07-19 08:35:49.000000 clickzetta-migration-0.0.1/setup.py
```

### Comparing `clickzetta-migration-0.0.0.9/clickzetta_migration.egg-info/SOURCES.txt` & `clickzetta-migration-0.0.1/clickzetta_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/base/exceptions.py` & `clickzetta-migration-0.0.1/migration/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/connector/destination/base.py` & `clickzetta-migration-0.0.1/migration/connector/destination/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/connector/destination/clickzetta/destination.py` & `clickzetta-migration-0.0.1/migration/connector/destination/doris/destination.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,135 @@
 import logging
 import os
+import random
+from datetime import datetime
+from time import sleep
+
+import pymysql
 
 from migration.connector.destination.base import Destination
 from clickzetta.dbapi.connection import Connection as ClickZettaConnection
 from clickzetta.client import Client
 from migration.base.exceptions import DestinationExecutionError, GrammarRestrictionsError
-import migration.util.script_util as script_utils
+from migration.base.status import Status
+import migration.util.object_storage_util as object_storage_util
 
 logger = logging.getLogger(__name__)
 
+MAX_GET_STATUS_TIMES = 100
+
 
-class ClickZettaDestination(Destination):
+class DorisDestination(Destination):
     def __init__(self, config: dict, meta_conf_path=None, storage_conf_path=None):
-        super().__init__('Clickzetta', config)
+        super().__init__('Doris', config)
         self.connection = None
-        self.instance_id = None
+        self.connection_params = self.get_connection_params()
         self.meta_conf_path = meta_conf_path
-        self.storage_config_path = storage_conf_path
+        self.storage_conf_path = storage_conf_path
 
     def get_connection_params(self):
-        assert self.config.get("service"), "service is required"
-        assert self.config.get("workspace"), "workspace is required"
-        assert self.config.get("instance"), "instance is required"
-        assert self.config.get("vcluster"), "vcluster is required"
-        assert self.config.get("username"), "username is required"
-        assert self.config.get("password"), "password is required"
-        assert self.config.get("instanceId"), "instanceId is required"
-        self.instance_id = self.config.get("instanceId")
+        assert self.config['fe_servers']
+        assert self.config['user']
+        assert self.config['password']
+
         return {
-            "service": self.config.get("service"),
-            "workspace": self.config.get("workspace"),
-            "instance": self.config.get("instance"),
-            "vcluster": self.config.get("vcluster"),
-            "username": self.config.get("username"),
-            "password": self.config.get("password"),
+            'host': self.config['fe_servers'][0].split(':')[0],
+            'port': int(self.config['fe_servers'][0].split(':')[1]),
+            'user': self.config['user'],
+            'password': self.config['password']
         }
 
     def connect(self):
         if self.connection is None:
-            connection_params = self.get_connection_params()
-            client = Client(
-                service=connection_params["service"],
-                workspace=connection_params["workspace"],
-                instance=connection_params["instance"],
-                vcluster=connection_params["vcluster"],
-                username=connection_params["username"],
-                password=connection_params["password"],
-            )
-            self.connection = ClickZettaConnection(client=client)
+            self.connection = pymysql.connect(**self.connection_params)
+            logger.info(f"Connect to Doris {self.connection_params['host']} successfully")
 
     def create_table(self, table_name, ddl: str):
         self.execute_sql(ddl)
         logger.info(f"Create table {table_name} successfully")
 
     def create_database(self, db_name):
-        self.execute_sql(f"CREATE SCHEMA IF NOT EXISTS {db_name}")
+        self.execute_sql(f"CREATE DATABASE IF NOT EXISTS {db_name}")
         logger.info(f"Create database {db_name} successfully")
 
     def execute_sql(self, sql, bind_params=None):
         try:
             self.connect()
-            cursor = self.connection.cursor()
-            cursor.execute(sql, bind_params)
-            return cursor.fetchall()
+            with self.connection.cursor() as cur:
+                cur.execute(sql, bind_params)
+                return cur.fetchall()
         except Exception as e:
             logger.error("migration Error running SQL: {}, error:{}", sql, e)
             raise DestinationExecutionError('migration Error running SQL: {}, error:{}'.format(sql, e))
 
     def close(self):
         self.connection.close()
 
     def load_external_data(self, file_path, schema_name, table_name):
-        meta_cmd_path = script_utils.get_meta_cmd_path()
-        meta_conf_path = os.path.abspath(os.path.join(os.getcwd(), "../../../../conf/meta_conf.json"))
+        object_storage = object_storage_util.get_object_storage_config(self.storage_conf_path)
+        label_name = f"{schema_name}_{table_name}_{datetime.now().day}_{random.randint(1, 100000000)}"
+        load_sql = f"use {schema_name};\n" \
+                   f"LOAD LABEL {label_name}\n" \
+                   f"(\n" \
+                   f"DATA INFILE(\"s3://{object_storage['bucket']}/{file_path}/*\")\n" \
+                   f"INTO TABLE {table_name}\n" \
+                   f"FORMAT AS \"parquet\"\n" \
+                   f")\n" \
+                   f"WITH S3\n" \
+                   f"(\n" \
+                   f"\"AWS_ENDPOINT\" = \"{object_storage['endpoint']}\",\n" \
+                   f"\"AWS_ACCESS_KEY\" = \"{object_storage['id']}\",\n" \
+                   f"\"AWS_SECRET_KEY\" = \"{object_storage['key']}\",\n" \
+                   f"\"AWS_REGION\" = \"{object_storage['region']}\"\n" \
+                   f");\n"
+        logger.info(f"Start to load data from {file_path} to {schema_name}.{table_name} with sql: {load_sql}")
+        self.execute_sql(load_sql)
+        current_times = 0
+        while current_times < MAX_GET_STATUS_TIMES:
+            if current_times == MAX_GET_STATUS_TIMES - 1:
+                raise DestinationExecutionError(
+                    f"doris load data from {file_path} to {schema_name}.{table_name}"
+                    f" failed, get result more than 100 times.")
+            check_state_sql = f"show load where Label = '{label_name}'"
+            state = self.execute_sql(check_state_sql)[0][2]
+            if state == 'FINISHED':
+                break
+            elif state == 'CANCELLED' or state == 'FAILED':
+                logger.error(f"doris load data from {file_path} to {schema_name}.{table_name} failed")
+                raise DestinationExecutionError(
+                    f"doris loading data from {file_path} to {schema_name}.{table_name} failed")
+            else:
+                logger.info(f"Waiting for doris S3 data loading, current state is {state}")
+            sleep(5)
+            current_times += 1
 
-        load_cmd = f"{meta_cmd_path} append-table -i {self.instance_id} -n {self.config.get('workspace')}" \
-                   f",{schema_name} -t {table_name} -r \"{file_path}\" -c {meta_conf_path}"
-        try:
-            os.popen(load_cmd)
-        except BaseException as e:
-            logger.error("migration Error loading external data: {}, error:{}", load_cmd, e)
-            raise DestinationExecutionError('migration Error loading external data: {}, error:{}'.format(load_cmd, e))
-
-        rewrite_table_sql = f"INSERT OVERWRITE {schema_name}.{table_name} SELECT * FROM {schema_name}.{table_name};"
-        self.execute_sql(rewrite_table_sql)
-        logger.info(f"Clickzetta Load external data {file_path} to {schema_name}.{table_name} successfully")
+        logger.info(f"Doirs Load data from {file_path} to {schema_name}.{table_name} successfully")
 
     def gen_destination_ddl(self, db_name, table_name, columns, primary_keys, cluster_info, partition_columns):
-        if primary_keys and cluster_info:
-            for primary_key, cluster_key in zip(primary_keys, cluster_info.cluster_keys):
-                if primary_key != cluster_key:
-                    logger.warning(f"Primary key {primary_key} is not in cluster key {cluster_info.cluster_keys}")
-                    raise GrammarRestrictionsError(f"Primary key {primary_key} is not in cluster key "
-                                                   f"{cluster_info.cluster_keys}")
         destination_ddl = 'CREATE TABLE IF NOT EXISTS {db}.{table} (\n'.format(db=db_name, table=table_name)
         for index, column in enumerate(columns):
             destination_ddl += '    {name} {type} {is_null} ' \
                 .format(name=column.name,
                         type=column.type,
                         is_null='' if column.is_null else 'NOT NULL')
             # if column.default_value:
             #     destination_ddl += "   DEFAULT {default_value}".format(default_value=column.default_value)
             if index != len(columns) - 1:
                 destination_ddl += ',\n'
             else:
                 destination_ddl += '\n'
 
         if primary_keys:
-            destination_ddl += '    PRIMARY KEY ({primary_keys}),\n'.format(primary_keys=','.join(primary_keys))
+            destination_ddl += '    UNIQUE KEY ({primary_keys}),\n'.format(primary_keys=','.join(primary_keys))
         destination_ddl += ') \n'
+        if partition_columns:
+            destination_ddl += 'PARTITIONED BY ({partitioned_by})\n'.format(partitioned_by=','.join(partition_columns))
         if cluster_info:
             destination_ddl += 'CLUSTERED BY ({clustered_by})\n'.format(
                 clustered_by=','.join(cluster_info.cluster_keys))
             destination_ddl += 'SORTED BY ({clustered_by})\n'.format(clustered_by=','.join(cluster_info.cluster_keys))
             if cluster_info.bucket_num:
                 destination_ddl += 'INTO {buckets} BUCKETS\n'.format(buckets=cluster_info.bucket_num)
             else:
                 destination_ddl += 'INTO 32 BUCKETS\n'
-
-        if partition_columns:
-            destination_ddl += 'PARTITIONED BY ({partitioned_by})\n'.format(partitioned_by=','.join(partition_columns))
         self.create_database(db_name)
         return destination_ddl
-
```

### Comparing `clickzetta-migration-0.0.0.9/migration/connector/destination/doris/destination.py` & `clickzetta-migration-0.0.1/migration/connector/source/doris/source.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import logging
-import os
-import random
-from datetime import datetime
-from time import sleep
+import re
 
 import pymysql
+import sqlparse
 
-from migration.connector.destination.base import Destination
-from clickzetta.dbapi.connection import Connection as ClickZettaConnection
-from clickzetta.client import Client
-from migration.base.exceptions import DestinationExecutionError, GrammarRestrictionsError
-from migration.base.status import Status
+from migration.connector.source.base import Source
+from migration.base.exceptions import SourceExecutionError
+from migration.connector.source.enum import Column, ClusterInfo
 import migration.util.object_storage_util as object_storage_util
 
 logger = logging.getLogger(__name__)
 
-MAX_GET_STATUS_TIMES = 100
 
-
-class DorisDestination(Destination):
+class DorisSource(Source):
     def __init__(self, config: dict, meta_conf_path=None, storage_conf_path=None):
         super().__init__('Doris', config)
-        self.connection = None
         self.connection_params = self.get_connection_params()
         self.meta_conf_path = meta_conf_path
-        self.storage_conf_path = storage_conf_path
+        self.storage_config_path = storage_conf_path
+
+    """
+    Doris connection parameters is a dict including following keys:
+    1. host: host of Doris
+    2. port: port for mysql client, default is 9030
+    3. database: database name
+    4. user: user name
+    5. passwd: password
+    """
 
     def get_connection_params(self):
         assert self.config['fe_servers']
         assert self.config['user']
         assert self.config['password']
 
         return {
@@ -39,97 +41,116 @@
         }
 
     def connect(self):
         if self.connection is None:
             self.connection = pymysql.connect(**self.connection_params)
             logger.info(f"Connect to Doris {self.connection_params['host']} successfully")
 
-    def create_table(self, table_name, ddl: str):
-        self.execute_sql(ddl)
-        logger.info(f"Create table {table_name} successfully")
-
-    def create_database(self, db_name):
-        self.execute_sql(f"CREATE DATABASE IF NOT EXISTS {db_name}")
-        logger.info(f"Create database {db_name} successfully")
+    def get_database_names(self):
+        result = self.execute_sql("show databases")
+        return [row[0] for row in result]
+
+    def get_table_names(self, database_name):
+        result = self.execute_sql(f"show tables from {database_name}")
+        return [row[0] for row in result]
+
+    def get_ddl_sql(self, database_name, table_name):
+        return self.execute_sql(f"show create table {database_name}.{table_name}")[0][1]
+
+    def get_table_cluster_info(self, database_name, table_name):
+        ddl_sql = self.get_ddl_sql(database_name, table_name)
+        cluster_columns = []
+        ddl_format_sql = sqlparse.format(ddl_sql, reindent=True, keyword_case='upper')
+        match_result = re.match(r'(.*)DISTRIBUTED(.*)BY(.*?)\((.*?)\)(.*)BUCKETS(.*?)(\d+).*', ddl_format_sql, re.S)
+        if match_result:
+            for cluster_column in match_result.group(4).strip().split(','):
+                cluster_columns.append(cluster_column.replace('`', '').strip())
+            return ClusterInfo(int(match_result.group(7).strip()), cluster_columns)
+
+        return None
+
+    def get_table_partition_columns(self, database_name, table_name):
+        ddl_sql = self.get_ddl_sql(database_name, table_name)
+        partition_columns = []
+        ddl_format_sql = sqlparse.format(ddl_sql, reindent=True, keyword_case='upper')
+        match_result = re.match(r'(.*?)PARTITION(.*?)BY(.*?)\((.*?)\).*', ddl_format_sql, re.S)
+        if match_result:
+            for partition_column in match_result.group(4).strip().split(','):
+                partition_columns.append(partition_column.replace('`', '').strip())
+            return partition_columns
+        return None
+
+    def get_primary_key(self, database_name, table_name):
+        ddl_sql = self.get_ddl_sql(database_name, table_name)
+        primary_keys = []
+        ddl_format_sql = sqlparse.format(ddl_sql, reindent=True, keyword_case='upper')
+        match_result = re.match(r'(.*?)UNIQUE(.*?)KEY(.*?)\((.*?)\).*', ddl_format_sql, re.S)
+        if match_result:
+            for primary_key in match_result.group(4).strip().split(','):
+                primary_keys.append(primary_key.replace('`', '').strip())
+            return primary_keys
+        return None
+
+    def get_table_columns(self, database_name, table_name) -> list[Column]:
+        result = self.execute_sql(f"desc {database_name}.{table_name}")
+        table_columns = []
+        for row in result:
+            table_columns.append(Column(name=row[0], type=row[1].upper(),
+                                        is_null=True if row[2].strip() == 'Yes' else False,
+                                        default_value=row[4]))
+        return table_columns
 
     def execute_sql(self, sql, bind_params=None):
         try:
             self.connect()
             with self.connection.cursor() as cur:
                 cur.execute(sql, bind_params)
                 return cur.fetchall()
-        except Exception as e:
-            logger.error("migration Error running SQL: {}, error:{}", sql, e)
-            raise DestinationExecutionError('migration Error running SQL: {}, error:{}'.format(sql, e))
 
-    def close(self):
-        self.connection.close()
+        except SourceExecutionError as e:
+            logger.error(f"Doris connector execute sql {sql} failed, error: {e}")
+            raise f"Doris connector execute sql {sql} failed, error: {e}"
+
+    def type_mapping(self):
+        return {
+            'DATETIME': 'TIMESTAMP',
+        }
 
-    def load_external_data(self, file_path, schema_name, table_name):
-        object_storage = object_storage_util.get_object_storage_config(self.storage_conf_path)
-        label_name = f"{schema_name}_{table_name}_{datetime.now().day}_{random.randint(1, 100000000)}"
-        load_sql = f"use {schema_name};\n" \
-                   f"LOAD LABEL {label_name}\n" \
-                   f"(\n" \
-                   f"DATA INFILE(\"s3://{object_storage['bucket']}/{file_path}/*\")\n" \
-                   f"INTO TABLE {table_name}\n" \
-                   f"FORMAT AS \"parquet\"\n" \
-                   f")\n" \
-                   f"WITH S3\n" \
-                   f"(\n" \
-                   f"\"AWS_ENDPOINT\" = \"{object_storage['endpoint']}\",\n" \
-                   f"\"AWS_ACCESS_KEY\" = \"{object_storage['id']}\",\n" \
-                   f"\"AWS_SECRET_KEY\" = \"{object_storage['key']}\",\n" \
-                   f"\"AWS_REGION\" = \"{object_storage['region']}\"\n" \
-                   f");\n"
-        logger.info(f"Start to load data from {file_path} to {schema_name}.{table_name} with sql: {load_sql}")
-        self.execute_sql(load_sql)
-        current_times = 0
-        while current_times < MAX_GET_STATUS_TIMES:
-            if current_times == MAX_GET_STATUS_TIMES - 1:
-                raise DestinationExecutionError(
-                    f"doris load data from {file_path} to {schema_name}.{table_name}"
-                    f" failed, get result more than 100 times.")
-            check_state_sql = f"show load where Label = '{label_name}'"
-            state = self.execute_sql(check_state_sql)[0][2]
-            if state == 'FINISHED':
-                break
-            elif state == 'CANCELLED' or state == 'FAILED':
-                logger.error(f"doris load data from {file_path} to {schema_name}.{table_name} failed")
-                raise DestinationExecutionError(
-                    f"doris loading data from {file_path} to {schema_name}.{table_name} failed")
-            else:
-                logger.info(f"Waiting for doris S3 data loading, current state is {state}")
-            sleep(5)
-            current_times += 1
-
-        logger.info(f"Doirs Load data from {file_path} to {schema_name}.{table_name} successfully")
-
-    def gen_destination_ddl(self, db_name, table_name, columns, primary_keys, cluster_info, partition_columns):
-        destination_ddl = 'CREATE TABLE IF NOT EXISTS {db}.{table} (\n'.format(db=db_name, table=table_name)
-        for index, column in enumerate(columns):
-            destination_ddl += '    {name} {type} {is_null} ' \
-                .format(name=column.name,
-                        type=column.type,
-                        is_null='' if column.is_null else 'NOT NULL')
-            # if column.default_value:
-            #     destination_ddl += "   DEFAULT {default_value}".format(default_value=column.default_value)
-            if index != len(columns) - 1:
-                destination_ddl += ',\n'
-            else:
-                destination_ddl += '\n'
-
-        if primary_keys:
-            destination_ddl += '    UNIQUE KEY ({primary_keys}),\n'.format(primary_keys=','.join(primary_keys))
-        destination_ddl += ') \n'
-        if partition_columns:
-            destination_ddl += 'PARTITIONED BY ({partitioned_by})\n'.format(partitioned_by=','.join(partition_columns))
-        if cluster_info:
-            destination_ddl += 'CLUSTERED BY ({clustered_by})\n'.format(
-                clustered_by=','.join(cluster_info.cluster_keys))
-            destination_ddl += 'SORTED BY ({clustered_by})\n'.format(clustered_by=','.join(cluster_info.cluster_keys))
-            if cluster_info.bucket_num:
-                destination_ddl += 'INTO {buckets} BUCKETS\n'.format(buckets=cluster_info.bucket_num)
-            else:
-                destination_ddl += 'INTO 32 BUCKETS\n'
-        self.create_database(db_name)
-        return destination_ddl
+    def close(self):
+        if self.connection is not None:
+            self.connection.close()
+            self.connection = None
+            logger.info(f"Close connection to Doris {self.connection_params['host']} successfully")
+
+    def unload_data(self, task):
+        logger.info(f"Begin to unload data from Doris table {task.name} to object storage")
+        file_path = f"{task.project_id}/{task.id}/{task.name.split('.')[1]}/"
+        object_storage_conf = object_storage_util.get_object_storage_config(self.storage_config_path)
+        partitions = ''
+        if hasattr(task, 'transform_partitions') and task.transform_partitions:
+            partitions = ' PARTITION ( '
+            values = task.transform_partitions[0]
+            for index, value in enumerate(values):
+                if index == 0:
+                    partitions += value
+                else:
+                    partitions += f",{value}"
+            partitions += ' ) '
+
+        unload_sql = f"EXPORT TABLE {task.name}\n" \
+                     f"{partitions}\n " \
+                     f"TO \"s3://{object_storage_conf['bucket']}/{file_path}\" \n" \
+                     f"WITH S3\n" \
+                     f"(\n" \
+                     f"\"AWS_ENDPOINT\"=\"{object_storage_conf['endpoint']}\",\n" \
+                     f"\"AWS_ACCESS_KEY\"=\"{object_storage_conf['id']}\",\n" \
+                     f"\"AWS_SECRET_KEY\"=\"{object_storage_conf['key']}\",\n" \
+                     f"\"AWS_REGION\"=\"{object_storage_conf['region']}\"\n" \
+                     f");"
+        logger.info(f"Unload data from Doris {self.connection_params['host']} with sql: {unload_sql}")
+        try:
+            self.execute_sql(unload_sql)
+        except BaseException as e:
+            logger.error(f"Unload data from Doris {self.connection_params['host']} failed, error: {e}")
+            raise BaseException(f"Unload data from Doris {self.connection_params['host']} failed, error: {e}")
+        logger.info(f"Unload data from Doris {self.connection_params['host']} to path {file_path} successfully")
+        return [file_path]
```

### Comparing `clickzetta-migration-0.0.0.9/migration/connector/source/base.py` & `clickzetta-migration-0.0.1/migration/connector/source/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/connector/source/clickzetta/source.py` & `clickzetta-migration-0.0.1/migration/connector/source/clickzetta/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/migration.py` & `clickzetta-migration-0.0.1/migration/migration.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,16 @@
     cz-migration run -p <profile_path> --meta_conf <meta_conf> --storage_conf <storage_conf> [--table_list_file <external_table_list_file>][migrate schema and data from source to destination, including validation]
     cz-migration status -p <profile_path> [check migration status]
     cz-migration resume -p <profile_path> [resume migration]
     cz-migration report -p <profile_path> [generate migration report]
 """
 import logging
 import os.path
-
 import docopt
 import yaml
-
 from migration.connector.destination.base import Destination
 from migration.connector.destination.clickzetta.destination import ClickZettaDestination
 from migration.connector.destination.doris.destination import DorisDestination
 from migration.connector.source import Source
 from migration.connector.source.clickzetta.source import ClickzettaSource
 from migration.connector.source.doris.source import DorisSource
 from migration.scheduler.data_transformer.transformer import DataTransformer
@@ -48,15 +46,14 @@
     with open(out_path, 'w') as f:
         for db in dbs:
             if db.startswith("__") or db.startswith("information_schema"):
                 continue
             tables = source.get_table_names(db)
             for table in tables:
                 f.write(f"{db}.{table}\n")
-    logger.info(f"Generating meta from source {source} to {out_path} successfully!")
 
 
 def schema(source: Source, destination: Destination, db_list: list, config_table_list: list, external_table_list: list,
            project_name: str, concurrency: int, quit_if_fail: bool):
     logger.info(f"Transforming schema from source {source} to destination {destination}")
     print(f"Transforming schema from source {source} to destination {destination}")
     SchemaTransformer(source, destination, project_name, db_list, config_table_list, external_table_list, concurrency,
@@ -112,15 +109,14 @@
     meta_conf_path = None
     storage_conf_path = None
     if not args['-p']:
         print("Please specify profile path!")
         logger.error("Please specify profile path!")
     profile_path = args['<profile_path>']
     print(f"Using profile {profile_path}")
-
     with open(profile_path, 'r') as f:
         profile = yaml.safe_load(f)['config']
     project_name = profile['name']
     print(f"Using project name  {project_name}")
     project_version = profile['version']
     print(f"Using project version  {project_version}")
     project_desc = profile['description']
@@ -136,22 +132,21 @@
     config_table_list = []
     external_table_list = []
     transform_partitions = {}
     if source_config['type'].strip() == 'doris':
         config = {'fe_servers': source_config['fe_servers'], 'user': source_config['username'],
                   'password': source_config['password']}
         logger.info(f"migration source {config}")
-        if source_config['transform_partitions']:
+        if 'transform_partitions' in source_config and source_config['transform_partitions']:
             tables = source_config['transform_partitions']['tables']
-            columns = source_config['transform_partitions']['columns']
             values = source_config['transform_partitions']['values']
-            if not len(columns) == len(values) == len(tables):
+            if not len(values) == len(tables):
                 raise Exception("transform_partitions columns, values and tables should have same length")
-            for i in range(len(columns)):
-                transform_partitions[tables[i]] = [columns[i], values[i]]
+            for i in range(len(tables)):
+                transform_partitions[tables[i]] = [values[i]]
         print(f"migration source {config}")
         source = DorisSource(config, meta_conf_path, storage_conf_path)
         if args['--table_list_file']:
             with open(args['<external_table_list_file>'], 'r') as f:
                 lines = f.readlines()
                 for line in lines:
                     external_table_list.append(line.strip())
@@ -165,14 +160,22 @@
                 db_list = source_config['migration_dbs']
     elif source_config['type'].strip() == 'clickzetta':
         config = {'service': source_config['service'], 'username': source_config['username'],
                   'workspace': source_config['workspace'], 'password': source_config['password'],
                   'instance': source_config['instance'], 'vcluster': source_config['vcluster'],
                   'instanceId': source_config['instanceId']}
         logger.info(f"migration source {config}")
+        if 'transform_partitions' in source_config and source_config['transform_partitions']:
+            tables = source_config['transform_partitions']['tables']
+            columns = source_config['transform_partitions']['columns']
+            values = source_config['transform_partitions']['values']
+            if not len(columns) == len(values) == len(tables):
+                raise Exception("transform_partitions columns, values and tables should have same length")
+            for i in range(len(columns)):
+                transform_partitions[tables[i]] = [columns[i], values[i]]
         print(f"migration source {config}")
         source = ClickzettaSource(config, meta_conf_path, storage_conf_path)
         if args['--table_list_file']:
             with open(args['<external_table_list_file>'], 'r') as f:
                 lines = f.readlines()
                 for line in lines:
                     external_table_list.append(line.strip())
```

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/data_transformer/transformer.py` & `clickzetta-migration-0.0.1/migration/scheduler/data_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/data_validation/validation.py` & `clickzetta-migration-0.0.1/migration/scheduler/data_validation/validation.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/scheduler.py` & `clickzetta-migration-0.0.1/migration/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/schema_transformer/transformer.py` & `clickzetta-migration-0.0.1/migration/scheduler/schema_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/task/base_task.py` & `clickzetta-migration-0.0.1/migration/scheduler/task/base_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/task/data_task.py` & `clickzetta-migration-0.0.1/migration/scheduler/task/data_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/task/schema_task.py` & `clickzetta-migration-0.0.1/migration/scheduler/task/schema_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/task/validation_task.py` & `clickzetta-migration-0.0.1/migration/scheduler/task/validation_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 
     def check_number_type_statistics(self):
         type_mapping = self.source.type_mapping()
         table_columns = self.source.get_table_columns(self.name.split('.')[0], self.name.split('.')[1])
         for column in table_columns:
             if self.is_number_type(column, type_mapping):
                 sql = f"select min({column.name}), max({column.name}), avg({column.name}) from {self.name}"
-                source_result = self.source.execute_sql(sql)
+                source_result = self.source.execute_sql(sql)[0]
                 logger.info(f"source table: {self.name} column: {column.name} statistics: {source_result}")
-                destination_result = self.destination.execute_sql(sql)
+                destination_result = self.destination.execute_sql(sql)[0]
                 logger.info(f"destination table: {self.name} column: {column.name} statistics: {destination_result}")
                 if source_result != destination_result:
                     self.status = TaskStatus.FAILED
                     self.end_time = datetime.now()
                     migration_tasks_status.update_task_status(self.destination, self)
                     logger.error(
                         f'ValidationTask {self.name} failed to run, error: number type statistics not equal, retry times: {self.retry_times}')
```

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/transformer.py` & `clickzetta-migration-0.0.1/migration/scheduler/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/scheduler/unify_transformer/transformer.py` & `clickzetta-migration-0.0.1/migration/scheduler/unify_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/test/util_test.py` & `clickzetta-migration-0.0.1/migration/test/util_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,7 +63,10 @@
         PK_TABLE_DML_HINT = {'hints': {'cz.sql.allow.insert.table.with.pk': 'true'}}
         config = {'service': 'poc-ap-shanghai-tencentcloud.api.clickzetta.com', 'username': 'changean',
                   'workspace': 'quickStart_WS',
                   'password': 'Achangean123!', 'instance': '1fdbc4a7', 'vcluster': 'DEFAULT', "instanceId": 32}
         destination = ClickZettaDestination(config)
         print(destination.execute_sql('show schemas;'))
         print(os.path.join(os.path.abspath(os.path.dirname(os.path.dirname(__file__))), 'scripts/linux/meta_cmd'))
+        list_1 = (8, 8, 8.0)
+        list_2 = (8.0, 8.0, 8.0)
+        print(list_1 == list_2)
```

### Comparing `clickzetta-migration-0.0.0.9/migration/util/migration_tasks_status.py` & `clickzetta-migration-0.0.1/migration/util/migration_tasks_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 def init_task_status(destination: Destination, task: Task):
     sql = None
     global INCREMENTAL_INDEX
     if destination.name.lower() == "clickzetta":
         sql = f"""
         INSERT INTO {STATUS_SCHEMA}.{task.project_id} (id, task_id, task_name, prject_id, task_status, task_type, task_start_time, task_end_time) 
-        values ('{INCREMENTAL_INDEX}','{task.id}', '{task.name}','{task.project_id}','{task.status.value}', '{task.task_type.value}', cast('{task.start_time}' as timestamp), null)
+        values ({INCREMENTAL_INDEX},'{task.id}', '{task.name}','{task.project_id}','{task.status.value}', '{task.task_type.value}', cast('{task.start_time}' as timestamp), null)
         """
         destination.execute_sql(sql, PK_TABLE_DML_HINT)
     elif destination.name.lower() == "doris":
         sql = f"""
         INSERT INTO {STATUS_SCHEMA}.{task.project_id} (id, task_id, task_name, prject_id, task_status, task_type, task_start_time, task_end_time) 
         values ('{INCREMENTAL_INDEX}','{task.id}', '{task.name}','{task.project_id}','{task.status.value}', '{task.task_type.value}', cast('{task.start_time}' as datetime), null)
         """
```

### Comparing `clickzetta-migration-0.0.0.9/migration/util/object_storage_util.py` & `clickzetta-migration-0.0.1/migration/util/object_storage_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/migration/util/script_util.py` & `clickzetta-migration-0.0.1/migration/util/script_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.9/setup.py` & `clickzetta-migration-0.0.1/setup.py`

 * *Files identical despite different names*

