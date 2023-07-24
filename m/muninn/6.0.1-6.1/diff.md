# Comparing `tmp/muninn-6.0.1.tar.gz` & `tmp/muninn-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/muninn-6.0.1.tar", last modified: Tue Nov 22 08:58:35 2022, max compression
+gzip compressed data, was "dist/muninn-6.1.tar", last modified: Mon Jul 24 14:43:23 2023, max compression
```

## Comparing `muninn-6.0.1.tar` & `muninn-6.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/
--rw-r--r--   0 sander     (501) staff       (20)      880 2022-11-22 08:58:35.000000 muninn-6.0.1/PKG-INFO
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/test/
--rw-r--r--   0 sander     (501) staff       (20)    70112 2022-11-16 12:12:19.000000 muninn-6.0.1/test/test.py
--rw-r--r--   0 sander     (501) staff       (20)     4076 2022-08-16 07:53:04.000000 muninn-6.0.1/test/product_type.py.template
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/test/data/
--rw-r--r--   0 sander     (501) staff       (20)     1015 2022-03-17 08:49:39.000000 muninn-6.0.1/test/data/pi.txt
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/test/data/multi/
--rw-r--r--   0 sander     (501) staff       (20)      229 2022-03-17 08:49:39.000000 muninn-6.0.1/test/data/multi/2.txt
--rw-r--r--   0 sander     (501) staff       (20)      209 2022-03-17 08:49:39.000000 muninn-6.0.1/test/data/multi/1.txt
--rw-r--r--   0 sander     (501) staff       (20)     1508 2022-03-23 13:34:50.000000 muninn-6.0.1/test/data/README
--rwxr-xr-x   0 sander     (501) staff       (20)       75 2022-03-31 07:35:25.000000 muninn-6.0.1/test/coverage.sh
--rw-r--r--   0 sander     (501) staff       (20)    24897 2022-11-17 13:11:39.000000 muninn-6.0.1/CHANGES
--rw-r--r--   0 sander     (501) staff       (20)      229 2022-06-07 12:48:22.000000 muninn-6.0.1/MANIFEST.in
--rw-r--r--   0 sander     (501) staff       (20)     1593 2022-10-28 15:16:38.000000 muninn-6.0.1/DEVELOPER.md
--rw-r--r--   0 sander     (501) staff       (20)     1180 2022-06-07 12:48:22.000000 muninn-6.0.1/README.md
--rw-r--r--   0 sander     (501) staff       (20)     2837 2022-11-17 13:06:04.000000 muninn-6.0.1/setup.py
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn/
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn/database/
--rw-r--r--   0 sander     (501) staff       (20)    42893 2022-10-18 11:58:34.000000 muninn-6.0.1/muninn/database/postgresql.py
--rw-r--r--   0 sander     (501) staff       (20)     7471 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/database/blobgeometry.py
--rw-r--r--   0 sander     (501) staff       (20)       54 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/database/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)     6928 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/database/ewkb.py
--rw-r--r--   0 sander     (501) staff       (20)    40975 2022-10-18 11:58:50.000000 muninn-6.0.1/muninn/database/sqlite.py
--rw-r--r--   0 sander     (501) staff       (20)    32310 2022-10-18 11:47:04.000000 muninn-6.0.1/muninn/database/sql.py
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn/tools/
--rw-r--r--   0 sander     (501) staff       (20)     4474 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/update.py
--rw-r--r--   0 sander     (501) staff       (20)     6891 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/ingest.py
--rw-r--r--   0 sander     (501) staff       (20)     2157 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/pull.py
--rw-r--r--   0 sander     (501) staff       (20)     2014 2022-03-31 07:35:25.000000 muninn-6.0.1/muninn/tools/destroy.py
--rw-r--r--   0 sander     (501) staff       (20)     1468 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/untag.py
--rw-r--r--   0 sander     (501) staff       (20)     1797 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/remove.py
--rw-r--r--   0 sander     (501) staff       (20)     4897 2022-10-18 11:56:57.000000 muninn-6.0.1/muninn/tools/attach.py
--rw-r--r--   0 sander     (501) staff       (20)       54 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/tools/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)     2743 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/export.py
--rw-r--r--   0 sander     (501) staff       (20)     2945 2022-10-18 11:56:39.000000 muninn-6.0.1/muninn/tools/hash.py
--rw-r--r--   0 sander     (501) staff       (20)     9571 2022-10-18 11:57:48.000000 muninn-6.0.1/muninn/tools/summary.py
--rw-r--r--   0 sander     (501) staff       (20)     4604 2022-10-18 11:47:25.000000 muninn-6.0.1/muninn/tools/utils.py
--rw-r--r--   0 sander     (501) staff       (20)     1852 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/retrieve.py
--rw-r--r--   0 sander     (501) staff       (20)    10134 2022-10-18 11:57:04.000000 muninn-6.0.1/muninn/tools/search.py
--rw-r--r--   0 sander     (501) staff       (20)      977 2022-03-31 07:35:25.000000 muninn-6.0.1/muninn/tools/list_tags.py
--rw-r--r--   0 sander     (501) staff       (20)     1625 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/strip.py
--rw-r--r--   0 sander     (501) staff       (20)     1455 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/tools/info.py
--rw-r--r--   0 sander     (501) staff       (20)     1375 2022-03-31 07:35:25.000000 muninn-6.0.1/muninn/tools/prepare.py
--rw-r--r--   0 sander     (501) staff       (20)     1214 2022-07-15 11:54:00.000000 muninn-6.0.1/muninn/tools/tag.py
--rw-r--r--   0 sander     (501) staff       (20)     2898 2022-03-31 07:35:25.000000 muninn-6.0.1/muninn/config.py
--rw-r--r--   0 sander     (501) staff       (20)     9600 2022-10-18 11:48:29.000000 muninn-6.0.1/muninn/remote.py
--rw-r--r--   0 sander     (501) staff       (20)    10771 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/util.py
--rw-r--r--   0 sander     (501) staff       (20)     2283 2022-11-17 13:04:05.000000 muninn-6.0.1/muninn/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)     1807 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/core.py
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn/storage/
--rw-r--r--   0 sander     (501) staff       (20)        0 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/storage/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)    11036 2022-11-14 14:16:22.000000 muninn-6.0.1/muninn/storage/fs.py
--rw-r--r--   0 sander     (501) staff       (20)     7751 2022-11-16 11:52:39.000000 muninn-6.0.1/muninn/storage/swift.py
--rw-r--r--   0 sander     (501) staff       (20)    10813 2022-11-16 11:52:39.000000 muninn-6.0.1/muninn/storage/s3.py
--rw-r--r--   0 sander     (501) staff       (20)     2736 2022-08-22 11:56:38.000000 muninn-6.0.1/muninn/storage/base.py
--rw-r--r--   0 sander     (501) staff       (20)     1206 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/visitor.py
--rw-r--r--   0 sander     (501) staff       (20)      273 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/extension.py
--rw-r--r--   0 sander     (501) staff       (20)     7040 2022-03-31 07:35:25.000000 muninn-6.0.1/muninn/geometry.py
--rw-r--r--   0 sander     (501) staff       (20)    31466 2022-09-08 09:35:41.000000 muninn-6.0.1/muninn/language.py
--rw-r--r--   0 sander     (501) staff       (20)    77435 2022-10-28 11:56:38.000000 muninn-6.0.1/muninn/archive.py
--rw-r--r--   0 sander     (501) staff       (20)      342 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/exceptions.py
--rw-r--r--   0 sander     (501) staff       (20)     1010 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/enum.py
--rw-r--r--   0 sander     (501) staff       (20)     1446 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/_compat.py
--rw-r--r--   0 sander     (501) staff       (20)     3749 2022-03-17 08:49:39.000000 muninn-6.0.1/muninn/function.py
--rw-r--r--   0 sander     (501) staff       (20)     1685 2022-07-11 12:24:22.000000 muninn-6.0.1/muninn/struct.py
--rw-r--r--   0 sander     (501) staff       (20)     6499 2022-07-11 12:24:22.000000 muninn-6.0.1/muninn/schema.py
--rw-r--r--   0 sander     (501) staff       (20)       38 2022-11-22 08:58:35.000000 muninn-6.0.1/setup.cfg
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn.egg-info/
--rw-r--r--   0 sander     (501) staff       (20)      880 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn.egg-info/PKG-INFO
--rw-r--r--   0 sander     (501) staff       (20)     1340 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn.egg-info/SOURCES.txt
--rw-r--r--   0 sander     (501) staff       (20)      710 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn.egg-info/entry_points.txt
--rw-r--r--   0 sander     (501) staff       (20)        7 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn.egg-info/top_level.txt
--rw-r--r--   0 sander     (501) staff       (20)        1 2022-11-22 08:58:35.000000 muninn-6.0.1/muninn.egg-info/dependency_links.txt
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/
+-rw-r--r--   0 sander     (501) staff       (20)      878 2023-07-24 14:43:23.000000 muninn-6.1/PKG-INFO
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/test/
+-rw-r--r--   0 sander     (501) staff       (20)    72234 2023-07-21 09:55:52.000000 muninn-6.1/test/test.py
+-rw-r--r--   0 sander     (501) staff       (20)     4076 2022-08-16 07:53:04.000000 muninn-6.1/test/product_type.py.template
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/test/data/
+-rw-r--r--   0 sander     (501) staff       (20)     1015 2022-03-17 08:49:39.000000 muninn-6.1/test/data/pi.txt
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/test/data/multi/
+-rw-r--r--   0 sander     (501) staff       (20)      229 2022-03-17 08:49:39.000000 muninn-6.1/test/data/multi/2.txt
+-rw-r--r--   0 sander     (501) staff       (20)      209 2022-03-17 08:49:39.000000 muninn-6.1/test/data/multi/1.txt
+-rw-r--r--   0 sander     (501) staff       (20)     1508 2022-03-23 13:34:50.000000 muninn-6.1/test/data/README
+-rwxr-xr-x   0 sander     (501) staff       (20)       75 2022-03-31 07:35:25.000000 muninn-6.1/test/coverage.sh
+-rw-r--r--   0 sander     (501) staff       (20)    26029 2023-07-24 14:30:27.000000 muninn-6.1/CHANGES
+-rw-r--r--   0 sander     (501) staff       (20)      229 2022-06-07 12:48:22.000000 muninn-6.1/MANIFEST.in
+-rw-r--r--   0 sander     (501) staff       (20)     1593 2022-10-28 15:16:38.000000 muninn-6.1/DEVELOPER.md
+-rw-r--r--   0 sander     (501) staff       (20)     1180 2023-01-10 15:30:19.000000 muninn-6.1/README.md
+-rw-r--r--   0 sander     (501) staff       (20)     2835 2023-07-24 14:33:23.000000 muninn-6.1/setup.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn/
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn/database/
+-rw-r--r--   0 sander     (501) staff       (20)    42950 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/postgresql.py
+-rw-r--r--   0 sander     (501) staff       (20)     7471 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/blobgeometry.py
+-rw-r--r--   0 sander     (501) staff       (20)       54 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)     6928 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/ewkb.py
+-rw-r--r--   0 sander     (501) staff       (20)    40989 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/sqlite.py
+-rw-r--r--   0 sander     (501) staff       (20)    32428 2023-07-24 14:34:27.000000 muninn-6.1/muninn/database/sql.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn/tools/
+-rw-r--r--   0 sander     (501) staff       (20)     4516 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/update.py
+-rw-r--r--   0 sander     (501) staff       (20)     6891 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/ingest.py
+-rw-r--r--   0 sander     (501) staff       (20)     2157 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/pull.py
+-rw-r--r--   0 sander     (501) staff       (20)     2014 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/destroy.py
+-rw-r--r--   0 sander     (501) staff       (20)     1468 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/untag.py
+-rw-r--r--   0 sander     (501) staff       (20)     1797 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/remove.py
+-rw-r--r--   0 sander     (501) staff       (20)     4897 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/attach.py
+-rw-r--r--   0 sander     (501) staff       (20)       54 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)     2743 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/export.py
+-rw-r--r--   0 sander     (501) staff       (20)     2945 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/hash.py
+-rw-r--r--   0 sander     (501) staff       (20)     9571 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/summary.py
+-rw-r--r--   0 sander     (501) staff       (20)     4646 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/utils.py
+-rw-r--r--   0 sander     (501) staff       (20)     2040 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/retrieve.py
+-rw-r--r--   0 sander     (501) staff       (20)    10134 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/search.py
+-rw-r--r--   0 sander     (501) staff       (20)      977 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/list_tags.py
+-rw-r--r--   0 sander     (501) staff       (20)     1625 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/strip.py
+-rw-r--r--   0 sander     (501) staff       (20)     1455 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/info.py
+-rw-r--r--   0 sander     (501) staff       (20)     1388 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/prepare.py
+-rw-r--r--   0 sander     (501) staff       (20)     1214 2023-07-24 14:34:27.000000 muninn-6.1/muninn/tools/tag.py
+-rw-r--r--   0 sander     (501) staff       (20)     2898 2023-07-24 14:34:27.000000 muninn-6.1/muninn/config.py
+-rw-r--r--   0 sander     (501) staff       (20)    10760 2023-07-24 14:34:27.000000 muninn-6.1/muninn/remote.py
+-rw-r--r--   0 sander     (501) staff       (20)    10771 2023-07-24 14:34:27.000000 muninn-6.1/muninn/util.py
+-rw-r--r--   0 sander     (501) staff       (20)     2281 2023-07-24 14:34:27.000000 muninn-6.1/muninn/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)     1807 2023-07-24 14:34:27.000000 muninn-6.1/muninn/core.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn/storage/
+-rw-r--r--   0 sander     (501) staff       (20)        0 2022-03-17 08:49:39.000000 muninn-6.1/muninn/storage/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)    11566 2023-07-18 12:06:32.000000 muninn-6.1/muninn/storage/fs.py
+-rw-r--r--   0 sander     (501) staff       (20)     8008 2023-07-18 12:06:32.000000 muninn-6.1/muninn/storage/swift.py
+-rw-r--r--   0 sander     (501) staff       (20)    11064 2023-07-18 12:06:32.000000 muninn-6.1/muninn/storage/s3.py
+-rw-r--r--   0 sander     (501) staff       (20)     2524 2023-07-24 07:50:10.000000 muninn-6.1/muninn/storage/base.py
+-rw-r--r--   0 sander     (501) staff       (20)     1206 2023-07-24 14:34:27.000000 muninn-6.1/muninn/visitor.py
+-rw-r--r--   0 sander     (501) staff       (20)      273 2023-07-24 14:34:27.000000 muninn-6.1/muninn/extension.py
+-rw-r--r--   0 sander     (501) staff       (20)     7040 2023-07-24 14:34:27.000000 muninn-6.1/muninn/geometry.py
+-rw-r--r--   0 sander     (501) staff       (20)    31474 2023-07-24 14:34:27.000000 muninn-6.1/muninn/language.py
+-rw-r--r--   0 sander     (501) staff       (20)    77997 2023-07-24 14:34:27.000000 muninn-6.1/muninn/archive.py
+-rw-r--r--   0 sander     (501) staff       (20)      342 2023-07-24 14:34:27.000000 muninn-6.1/muninn/exceptions.py
+-rw-r--r--   0 sander     (501) staff       (20)     1010 2023-07-24 14:34:27.000000 muninn-6.1/muninn/enum.py
+-rw-r--r--   0 sander     (501) staff       (20)     1446 2022-03-17 08:49:39.000000 muninn-6.1/muninn/_compat.py
+-rw-r--r--   0 sander     (501) staff       (20)     3749 2023-07-24 14:34:27.000000 muninn-6.1/muninn/function.py
+-rw-r--r--   0 sander     (501) staff       (20)     1685 2023-07-24 14:34:27.000000 muninn-6.1/muninn/struct.py
+-rw-r--r--   0 sander     (501) staff       (20)     6499 2023-07-24 14:34:27.000000 muninn-6.1/muninn/schema.py
+-rw-r--r--   0 sander     (501) staff       (20)       38 2023-07-24 14:43:23.000000 muninn-6.1/setup.cfg
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/
+-rw-r--r--   0 sander     (501) staff       (20)      878 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/PKG-INFO
+-rw-r--r--   0 sander     (501) staff       (20)     1340 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/SOURCES.txt
+-rw-r--r--   0 sander     (501) staff       (20)      710 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/entry_points.txt
+-rw-r--r--   0 sander     (501) staff       (20)        7 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/top_level.txt
+-rw-r--r--   0 sander     (501) staff       (20)        1 2023-07-24 14:43:23.000000 muninn-6.1/muninn.egg-info/dependency_links.txt
```

### Comparing `muninn-6.0.1/PKG-INFO` & `muninn-6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: muninn
-Version: 6.0.1
+Version: 6.1
 Summary: Data product catalogue and archive system
 Home-page: https://github.com/stcorp/muninn
 Author: S[&]T
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `muninn-6.0.1/test/test.py` & `muninn-6.1/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 import shutil
 
 from muninn.geometry import Polygon, LinearRing, Point
 from muninn.extension import CascadeRule
 
 CFG = ConfigParser()
-CFG.read(u'test.cfg')
+CFG.read(os.environ.get('MUNINN_TEST_CFG', 'test.cfg'))
 
 STORAGE_BACKENDS = [s.strip() for s in CFG.get('DEFAULT', 'storage').split(',')]
 DATABASE_BACKENDS = [s.strip() for s in CFG.get('DEFAULT', 'database').split(',')]
 REMOTE_BACKENDS = [s.strip() for s in CFG.get('DEFAULT', 'remote_backends').split(',')]
 ARCHIVE_PATHS = [s.strip() for s in CFG.get('DEFAULT', 'archive_path').split(',')]
 USE_ENCLOSING_DIR = [s.strip() == 'true' for s in CFG.get('DEFAULT', 'use_enclosing_dir').split(',')]
 
@@ -76,16 +76,21 @@
     def __init__(self, *args, **kwargs):
         super(FSChecker, self).__init__(*args, **kwargs)
         self.root = self.parser.get('fs', 'root')
 
     def exists(self, path, size=None):
         path = os.path.join(self.root, path)
 
-        if not os.path.isfile(path):
-            return False
+        if path.endswith('/'):
+            if not os.path.isdir(path[:-1]):
+                return False
+        else:
+            if not os.path.isfile(path):
+                return False
+
         if size is not None and os.path.getsize(path) != size:
             return False
 
         return True
 
 
 class S3Checker(BaseChecker):
@@ -872,27 +877,39 @@
 
     def test_retrieve_file(self, archive):
         props = self._ingest_file(archive)
 
         name = 'pi.txt'
         size = os.path.getsize('data/pi.txt')
 
-        # copy
+        # copy (query)
         with muninn.util.TemporaryDirectory() as tmp_path:
-            archive.retrieve(target_path=tmp_path)
+            result = archive.retrieve(target_path=tmp_path)
+
+            if archive._params['use_enclosing_directory']:
+                assert result == [[os.path.join(tmp_path, name)]]
+            else:
+                assert result == [os.path.join(tmp_path, name)]
 
             path = os.path.join(tmp_path, name)
             assert os.path.isfile(path)
             assert os.path.getsize(path) == size
 
-            archive.retrieve(props.core.uuid, target_path=tmp_path)
+        # copy (uuid)
+        with muninn.util.TemporaryDirectory() as tmp_path:
+            result = archive.retrieve(props.core.uuid, target_path=tmp_path)
 
-            with pytest.raises(muninn.exceptions.Error) as excinfo:
-                archive.retrieve(uuid.uuid4())
-            assert 'No product found' in str(excinfo)
+            if archive._params['use_enclosing_directory']:
+                assert result == [os.path.join(tmp_path, name)]
+            else:
+                assert result == os.path.join(tmp_path, name)
+
+            path = os.path.join(tmp_path, name)
+            assert os.path.isfile(path)
+            assert os.path.getsize(path) == size
 
         # symlink
         if archive._params['storage'] == 'fs':
             with muninn.util.TemporaryDirectory() as tmp_path:
                 archive.retrieve(target_path=tmp_path, use_symlinks=True)
 
                 path = os.path.join(tmp_path, name)
@@ -912,27 +929,51 @@
                 assert os.readlink(path) == target_path
         else:
             with pytest.raises(muninn.exceptions.Error) as excinfo:
                 with muninn.util.TemporaryDirectory() as tmp_path:
                     archive.retrieve(target_path=tmp_path, use_symlinks=True)
             assert 'storage backend does not support symlinks' in str(excinfo)
 
+        # error
+        with muninn.util.TemporaryDirectory() as tmp_path:
+            with pytest.raises(muninn.exceptions.Error) as excinfo:
+                archive.retrieve(uuid.uuid4())
+            assert 'No product found' in str(excinfo)
+
+
     def test_retrieve_multi_file(self, archive):
         if archive._params['use_enclosing_directory'] is True:
-            self._ingest_multi_file(archive)
+            props = self._ingest_multi_file(archive)
 
-            # copy
+            # copy (query)
             with muninn.util.TemporaryDirectory() as tmp_path:
-                archive.retrieve(target_path=tmp_path)
+                result = archive.retrieve(target_path=tmp_path)
 
                 for name in ('1.txt', '2.txt'):
                     path = os.path.join(tmp_path, name)
                     assert os.path.isfile(path)
                     assert os.path.getsize(path) == os.path.getsize('data/multi/%s' % name)
 
+                assert len(result) == 1
+                assert os.path.join(tmp_path, '1.txt') in result[0]
+                assert os.path.join(tmp_path, '2.txt') in result[0]
+
+            # copy (uuid)
+            with muninn.util.TemporaryDirectory() as tmp_path:
+                result = archive.retrieve(props.core.uuid, target_path=tmp_path)
+
+                assert os.path.join(tmp_path, '1.txt') in result
+                assert os.path.join(tmp_path, '2.txt') in result
+
+            # copy to '.'
+            archive.retrieve(target_path='.')
+            for name in ('1.txt', '2.txt'):
+                assert os.path.isfile(name)
+                assert os.path.getsize(name) == os.path.getsize('data/multi/%s' % name)
+
             # symlink
             if archive._params['storage'] == 'fs':
                 with muninn.util.TemporaryDirectory() as tmp_path:
                     archive.retrieve(target_path=tmp_path, use_symlinks=True)
 
                     for name in ('1.txt', '2.txt'):
                         path = os.path.join(tmp_path, name)
@@ -1084,14 +1125,17 @@
             for name in names:
                 path = os.path.join(
                     'bicycle/multi',
                     name
                 )
                 assert archive._checker.exists(path)
 
+            assert archive._checker.exists('bicycle/multi/emptydir/')
+            assert archive._checker.exists('bicycle/multi/dir/emptydir/')
+
             for name in names:
                 oldpath = os.path.join(
                     archive._params['archive_path'],
                     'multi',
                     name
                 )
                 assert not archive._checker.exists(oldpath)
@@ -1648,14 +1692,18 @@
             s = archive.search('size in')
         assert 'unexpected end of input' in str(excinfo)
 
         with pytest.raises(muninn.exceptions.Error) as excinfo:
             s = archive.search('size in [] xyz')
         assert 'extra characters after expression' in str(excinfo)
 
+        with pytest.raises(muninn.exceptions.Error) as excinfo:
+            s = archive.search('covers(core.footprint, POINT (1.0, 3.0))')
+        assert 'char 34: expected one of: INTEGER, REAL, got ","' in str(excinfo)
+
 class TestTools:  # TODO more result checking, preferrably using tools
     def _run(self, tool, args='', action='', archive='my_arch', should_fail=False):
         python_path = 'PYTHONPATH=%s:.:$PYTHONPATH' % PARENT_DIR
         cmd = '%s python%s ../muninn/tools/%s.py %s %s %s 2>&1' % \
               (python_path, '3' if PY3 else '', tool, action, archive, args)
 
         returncode, output, errs = safe_popen(cmd, join=True)
@@ -1766,24 +1814,26 @@
         self._run('destroy', '-y')
         self._run('prepare')
         output = self._run('search', '"" -c')
         assert output == ['0']
 
     def test_summary(self, archive):
         output = self._run('ingest', 'data/pi.txt')
+        output = self._run('summary', '"" -g physical_name')
+        assert len(output) == 3
         output = self._run('summary', '"" -f csv -H')
         assert len(output) == 2
         assert output[1].split(',')[0] == '"1"'
         output = self._run('summary', '"" -f psv')
         assert len(output) == 2
 
     def test_retrieve(self, archive):  # TODO nprocesses setting & fixture?
         with muninn.util.TemporaryDirectory() as tmp_path:
             output = self._run('ingest', 'data/pi.txt')
-            output = self._run('retrieve', '"" -d %s' % tmp_path)
+            output = self._run('retrieve', '"" -d %s --verify-hash' % tmp_path)
             assert os.listdir(tmp_path) == ['pi.txt']
         archive.remove()
 
         # parallel
         with muninn.util.TemporaryDirectory() as tmp_path:
             output = self._run('ingest', '--parallel data/a.txt data/b.txt data/c.txt')
             output = self._run('retrieve', '"" --parallel -d %s' % tmp_path)
```

### Comparing `muninn-6.0.1/test/product_type.py.template` & `muninn-6.1/test/product_type.py.template`

 * *Files identical despite different names*

### Comparing `muninn-6.0.1/test/data/pi.txt` & `muninn-6.1/test/data/pi.txt`

 * *Files identical despite different names*

### Comparing `muninn-6.0.1/test/data/README` & `muninn-6.1/test/data/README`

 * *Files identical despite different names*

### Comparing `muninn-6.0.1/CHANGES` & `muninn-6.1/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+6.1 2023-07-24
+~~~~~~~~~~~~~~
+
+* The S3 bucket prefix is now created as a 'directory object' so its existence
+  can be explicitly checked.
+
+* muninn-pull for http/https will now retry once in case of a timeout error.
+
+* muninn-prepare --dry-run now adds a ';' at the end of each line.
+
+* Added --verify-hash option to muninn-retrieve.
+
+* Command line tools no longer show a progress bar if there is no tty.
+
+* Fixed issue where failing to set/unset a tag did not result in an error.
+
+* Fixed issue with relocating products in an S3 archive when the product
+  contained an empty subdirectory.
+
+* Fixed issue where muninn-summary could not group by core.physical_name or
+  core.archive_path.
+
+* Fixed issue where muninn was incorrectly using subdirectories in the
+  temporary directory if the 'tempdir' archive configuration option was set.
+
+* Fixed issue where archive.retrieve() and archive.export() were returning a
+  list if a single properties Struct was given as parameter and
+  `use_enclosing_directory` was not set. Additionally, each entry for a
+  product where `use_enclosing_directory` _is_ set will now always be a list.
+
 6.0.1 2022-11-17
 ~~~~~~~~~~~~~~~~
 
 * Fixed python 2 issues and updated documentation that python>=2.7 is required.
 
 6.0 2022-10-28
 ~~~~~~~~~~~~~~
```

### Comparing `muninn-6.0.1/DEVELOPER.md` & `muninn-6.1/DEVELOPER.md`

 * *Files identical despite different names*

### Comparing `muninn-6.0.1/README.md` & `muninn-6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 
 Muninn uses the concept of namespaces to group different sets of properties
 for a product together within the catalogue. Muninn itself provides a 'core'
 namespace that covers the most common properties for data products.
 Support for additional namespaces are handled through external plug-ins
 (see [Extensions](https://stcorp.github.io/muninn/extensions/)).
 
-In Norse mythology, Muninn is a raven that, together with another raven called
-Huggin, gather information for the god Odin. Muninn is Old Norse for "memory".
+In Norse mythology, Muninn is a raven who, together with another raven called
+Huginn, gathers information for the god Odin. Muninn is Old Norse for "memory".
 
 # Documentation
 
 See the [online documentation](https://stcorp.github.io/muninn/).
```

### Comparing `muninn-6.0.1/setup.py` & `muninn-6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     sys.exit("Python 2.7 (or newer) or 3.6 (or newer) is required to use this package.")
 
 
 requirements = []
 
 setup(
     name="muninn",
-    version="6.0.1",
+    version="6.1",
     description="Data product catalogue and archive system",
     url="https://github.com/stcorp/muninn",
     author="S[&]T",
     license="BSD",
     packages=["muninn", "muninn.tools", "muninn.database", "muninn.storage"],
     entry_points={"console_scripts": [
         "muninn-attach = muninn.tools.attach:main",
```

### Comparing `muninn-6.0.1/muninn/database/postgresql.py` & `muninn-6.1/muninn/database/postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 from muninn._compat import dictkeys, dictvalues, is_python2_unicode
 
 import re
@@ -299,76 +299,76 @@
         self._sql_builder = sql.SQLBuilder({}, sql.TypeMap(), {}, self._table_name, self._placeholder,
                                            self._placeholder, self._rewriter_property)
 
     def _create_tables_sql(self):
         result = []
         # Create the table for the core namespace.
         result.append(self._sql_builder.build_create_table_query("core"))
-        result.append("ALTER TABLE %s ADD PRIMARY KEY (uuid)" % self._core_table_name)
-        result.append("ALTER TABLE %s ADD CONSTRAINT %s_archive_path_uniq UNIQUE (archive_path, physical_name)" %
+        result.append("ALTER TABLE %s ADD PRIMARY KEY (uuid);" % self._core_table_name)
+        result.append("ALTER TABLE %s ADD CONSTRAINT %s_archive_path_uniq UNIQUE (archive_path, physical_name);" %
                       (self._core_table_name, self._core_table_name))
-        result.append("ALTER TABLE %s ADD CONSTRAINT %s_product_name_uniq UNIQUE (product_type, product_name)" %
+        result.append("ALTER TABLE %s ADD CONSTRAINT %s_product_name_uniq UNIQUE (product_type, product_name);" %
                       (self._core_table_name, self._core_table_name))
 
         schema = self._namespace_schema("core")
         for name in schema:
             if schema.has_index(name):
                 if schema[name] == Geometry:
                     # For the geospatial footprint we need to use a special GIST index
-                    result.append("CREATE INDEX idx_%s_%s ON %s USING GIST (%s)" %
+                    result.append("CREATE INDEX idx_%s_%s ON %s USING GIST (%s);" %
                                   (self._core_table_name, name, self._core_table_name, name))
                 else:
-                    result.append("CREATE INDEX idx_%s_%s ON %s (%s)" %
+                    result.append("CREATE INDEX idx_%s_%s ON %s (%s);" %
                                   (self._core_table_name, name, self._core_table_name, name))
 
         # Create the tables for all non-core namespaces.
         for namespace in self._namespace_schemas:
             if namespace == "core":
                 continue
 
             result.append(self._sql_builder.build_create_table_query(namespace))
 
-            result.append("ALTER TABLE %s ADD COLUMN uuid UUID PRIMARY KEY" % self._table_name(namespace))
+            result.append("ALTER TABLE %s ADD COLUMN uuid UUID PRIMARY KEY;" % self._table_name(namespace))
             result.append("ALTER TABLE %s ADD CONSTRAINT %s_uuid_fkey FOREIGN KEY (uuid) REFERENCES %s (uuid) ON "
-                          "DELETE CASCADE" % (self._table_name(namespace), self._table_name(namespace),
+                          "DELETE CASCADE;" % (self._table_name(namespace), self._table_name(namespace),
                                               self._core_table_name))
 
             schema = self._namespace_schema(namespace)
             for name in schema:
                 if schema.has_index(name):
                     if schema[name] == Geometry:
-                        result.append("CREATE INDEX idx_%s_%s ON %s USING GIST (%s)" %
+                        result.append("CREATE INDEX idx_%s_%s ON %s USING GIST (%s);" %
                                       (self._table_name(namespace), name, self._table_name(namespace), name))
                     else:
-                        result.append("CREATE INDEX idx_%s_%s ON %s (%s)" %
+                        result.append("CREATE INDEX idx_%s_%s ON %s (%s);" %
                                       (self._table_name(namespace), name, self._table_name(namespace), name))
 
         # We use explicit 'id' primary keys for the links and tags tables so the entries can be managed using
         # other front-ends that may not support tuples as primary keys.
 
         # Create the table for links.
-        result.append("CREATE TABLE %s (id SERIAL PRIMARY KEY, uuid UUID NOT NULL, source_uuid UUID NOT NULL)" %
+        result.append("CREATE TABLE %s (id SERIAL PRIMARY KEY, uuid UUID NOT NULL, source_uuid UUID NOT NULL);" %
                       self._link_table_name)
-        result.append("ALTER TABLE %s ADD CONSTRAINT %s_link_uuid_source_uuid_uniq UNIQUE (uuid, source_uuid)" %
+        result.append("ALTER TABLE %s ADD CONSTRAINT %s_link_uuid_source_uuid_uniq UNIQUE (uuid, source_uuid);" %
                       (self._link_table_name, self._link_table_name))
         result.append("ALTER TABLE %s ADD CONSTRAINT %s_uuid_fkey FOREIGN KEY (uuid) REFERENCES %s (uuid) ON "
-                      "DELETE CASCADE" % (self._link_table_name, self._link_table_name, self._core_table_name))
-        result.append("CREATE INDEX idx_%s_uuid ON %s (uuid)" % (self._link_table_name, self._link_table_name))
-        result.append("CREATE INDEX idx_%s_source_uuid ON %s (source_uuid)" %
+                      "DELETE CASCADE;" % (self._link_table_name, self._link_table_name, self._core_table_name))
+        result.append("CREATE INDEX idx_%s_uuid ON %s (uuid);" % (self._link_table_name, self._link_table_name))
+        result.append("CREATE INDEX idx_%s_source_uuid ON %s (source_uuid);" %
                       (self._link_table_name, self._link_table_name))
 
         # Create the table for tags.
-        result.append("CREATE TABLE %s (id SERIAL PRIMARY KEY, uuid UUID NOT NULL, tag TEXT NOT NULL)" %
+        result.append("CREATE TABLE %s (id SERIAL PRIMARY KEY, uuid UUID NOT NULL, tag TEXT NOT NULL);" %
                       self._tag_table_name)
-        result.append("ALTER TABLE %s ADD CONSTRAINT %s_tag_uuid_tag_uniq UNIQUE (uuid, tag)" %
+        result.append("ALTER TABLE %s ADD CONSTRAINT %s_tag_uuid_tag_uniq UNIQUE (uuid, tag);" %
                       (self._tag_table_name, self._tag_table_name))
         result.append("ALTER TABLE %s ADD CONSTRAINT %s_uuid_fkey FOREIGN KEY (uuid) REFERENCES %s (uuid) ON "
-                      "DELETE CASCADE" % (self._tag_table_name, self._tag_table_name, self._core_table_name))
-        result.append("CREATE INDEX idx_%s_uuid ON %s (uuid)" % (self._tag_table_name, self._tag_table_name))
-        result.append("CREATE INDEX idx_%s_tag ON %s (tag)" % (self._tag_table_name, self._tag_table_name))
+                      "DELETE CASCADE;" % (self._tag_table_name, self._tag_table_name, self._core_table_name))
+        result.append("CREATE INDEX idx_%s_uuid ON %s (uuid);" % (self._tag_table_name, self._tag_table_name))
+        result.append("CREATE INDEX idx_%s_tag ON %s (tag);" % (self._tag_table_name, self._tag_table_name))
         return result
 
     def _delete_product_properties(self, uuid):
         cursor = self._connection.cursor()
         try:
             cursor.execute("DELETE FROM %s WHERE source_uuid = %s" % (self._link_table_name, self._placeholder()),
                            (uuid,))
@@ -676,15 +676,16 @@
                                                                                     self._placeholder())
         for tag in tags:
             with self._connection:
                 cursor = self._connection.cursor()
                 try:
                     cursor.execute(query, (uuid, tag, uuid, tag))
                 except self._connection._backend.Error as _error:
-                    self._swallow_unique_violation(_error)
+                    if not self._swallow_unique_violation(_error):
+                        raise
                 finally:
                     cursor.close()
 
     def _tags(self, uuid):
         query = "SELECT tag FROM %s WHERE uuid = %s ORDER BY tag" % (self._tag_table_name, self._placeholder())
         parameters = (uuid,)
```

### Comparing `muninn-6.0.1/muninn/database/blobgeometry.py` & `muninn-6.1/muninn/database/blobgeometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import sys
 import struct
```

### Comparing `muninn-6.0.1/muninn/database/ewkb.py` & `muninn-6.1/muninn/database/ewkb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import codecs
 import struct
```

### Comparing `muninn-6.0.1/muninn/database/sqlite.py` & `muninn-6.1/muninn/database/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 from muninn._compat import dictkeys, dictvalues
 import os
 import re
@@ -245,26 +245,26 @@
                 sql = name + " " + type_name
                 if not schema.is_optional(name):
                     sql = sql + " " + "NOT NULL"
                 column_sql.append(sql)
         column_sql.append("PRIMARY KEY (uuid)")
         column_sql.append("UNIQUE (archive_path, physical_name)")
         column_sql.append("UNIQUE (product_type, product_name)")
-        result.append("CREATE TABLE %s (%s)" % (self._core_table_name, ", ".join(column_sql)))
+        result.append("CREATE TABLE %s (%s);" % (self._core_table_name, ", ".join(column_sql)))
         for name in schema:
             if self._type_map()[schema[name]] == "GEOMETRY":
-                result.append("SELECT AddGeometryColumn('%s', '%s', 4326, 'GEOMETRY', 2)" %
+                result.append("SELECT AddGeometryColumn('%s', '%s', 4326, 'GEOMETRY', 2);" %
                               (self._core_table_name, name,))
         for name in schema:
             if schema.has_index(name):
                 if schema[name] == Geometry:
                     # For the geospatial footprint we need to use a special spatial index
-                    result.append("SELECT CreateSpatialIndex('%s', '%s')" % (self._core_table_name, name))
+                    result.append("SELECT CreateSpatialIndex('%s', '%s');" % (self._core_table_name, name))
                 else:
-                    result.append("CREATE INDEX idx_%s_%s ON %s (%s)" %
+                    result.append("CREATE INDEX idx_%s_%s ON %s (%s);" %
                                   (self._core_table_name, name, self._core_table_name, name))
 
         # Create the tables for all non-core namespaces.
         for namespace in self._namespace_schemas:
             if namespace == "core":
                 continue
 
@@ -275,45 +275,45 @@
                 if type_name != "GEOMETRY":
                     sql = name + " " + type_name
                     if not schema.is_optional(name):
                         sql = sql + " " + "NOT NULL"
                     column_sql.append(sql)
             column_sql.append("uuid UUID PRIMARY KEY REFERENCES %s(uuid) ON DELETE CASCADE" %
                               self._core_table_name)
-            result.append("CREATE TABLE %s (%s)" % (self._table_name(namespace), ", ".join(column_sql)))
+            result.append("CREATE TABLE %s (%s);" % (self._table_name(namespace), ", ".join(column_sql)))
             for name in schema:
                 if self._type_map()[schema[name]] == "GEOMETRY":
-                    result.append("SELECT AddGeometryColumn('%s', '%s', 4326, 'GEOMETRY', 2)" %
+                    result.append("SELECT AddGeometryColumn('%s', '%s', 4326, 'GEOMETRY', 2);" %
                                   (self._table_name(namespace), name))
             for name in schema:
                 if schema.has_index(name):
                     if schema[name] == Geometry:
-                        result.append("SELECT CreateSpatialIndex('%s', '%s')" % (self._table_name(namespace), name))
+                        result.append("SELECT CreateSpatialIndex('%s', '%s');" % (self._table_name(namespace), name))
                     else:
-                        result.append("CREATE INDEX idx_%s_%s ON %s (%s)" %
+                        result.append("CREATE INDEX idx_%s_%s ON %s (%s);" %
                                       (self._table_name(namespace), name, self._table_name(namespace), name))
 
         # We use explicit 'id' primary keys for the links and tags tables so the entries can be managed using
         # other front-ends that may not support tuples as primary keys.
 
         # Create the table for links.
         result.append("CREATE TABLE %s (id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL, "
                       "uuid UUID REFERENCES %s(uuid) ON DELETE CASCADE, "
-                      "source_uuid UUID NOT NULL, UNIQUE (uuid, source_uuid))" %
+                      "source_uuid UUID NOT NULL, UNIQUE (uuid, source_uuid));" %
                       (self._link_table_name, self._core_table_name))
-        result.append("CREATE INDEX idx_%s_uuid ON %s (uuid)" % (self._link_table_name, self._link_table_name))
-        result.append("CREATE INDEX idx_%s_source_uuid ON %s (source_uuid)" %
+        result.append("CREATE INDEX idx_%s_uuid ON %s (uuid);" % (self._link_table_name, self._link_table_name))
+        result.append("CREATE INDEX idx_%s_source_uuid ON %s (source_uuid);" %
                       (self._link_table_name, self._link_table_name))
 
         # Create the table for tags.
         result.append("CREATE TABLE %s (id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL, "
                       "uuid UUID REFERENCES %s(uuid) ON DELETE CASCADE, "
-                      "tag TEXT NOT NULL, UNIQUE (uuid, tag))" % (self._tag_table_name, self._core_table_name))
-        result.append("CREATE INDEX idx_%s_uuid ON %s (uuid)" % (self._tag_table_name, self._tag_table_name))
-        result.append("CREATE INDEX idx_%s_tag ON %s (tag)" % (self._tag_table_name, self._tag_table_name))
+                      "tag TEXT NOT NULL, UNIQUE (uuid, tag));" % (self._tag_table_name, self._core_table_name))
+        result.append("CREATE INDEX idx_%s_uuid ON %s (uuid);" % (self._tag_table_name, self._tag_table_name))
+        result.append("CREATE INDEX idx_%s_tag ON %s (tag);" % (self._tag_table_name, self._tag_table_name))
         return result
 
     def _delete_product_properties(self, uuid):
         cursor = self._connection.cursor()
         try:
             cursor.execute("DELETE FROM %s WHERE source_uuid = %s" % (self._link_table_name, self._placeholder()),
                            (uuid,))
```

### Comparing `muninn-6.0.1/muninn/database/sql.py` & `muninn-6.1/muninn/database/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import collections
 
 try:
@@ -14,14 +14,15 @@
 import inspect
 
 from muninn.exceptions import *
 from muninn.function import Prototype
 from muninn.language import parse_and_analyze, Literal, Name, Identifier
 from muninn.schema import *
 from muninn.visitor import Visitor
+from muninn.core import Basename, ArchivePath
 
 
 AGGREGATE_FUNCTIONS = collections.OrderedDict([
     (Long, ['min', 'max', 'sum', 'avg']),
     (Integer, ['min', 'max', 'sum', 'avg']),
     (Real, ['min', 'max', 'sum', 'avg']),
     # (Boolean, []),
@@ -34,14 +35,16 @@
 
 GROUP_BY_FUNCTIONS = collections.OrderedDict([
     (Long, [None, ]),
     (Integer, [None, ]),
     # (Real, []),
     (Boolean, [None, ]),
     (Text, [None, 'length']),
+    (Basename, [None, 'length']),
+    (ArchivePath, [None, 'length']),
     (Timestamp, ['year', 'month', 'yearmonth', 'date', 'day', 'hour', 'minute', 'second', 'time']),
     # (UUID, []),
     # (Geometry, []),
 ])
 
 
 class TypeMap(MutableMapping):
@@ -409,15 +412,15 @@
         schema = self._namespace_schema(namespace)
         for identifier in schema:
             sql = identifier + " " + self._type(schema[identifier])
             if not schema.is_optional(identifier):
                 sql = sql + " " + "NOT NULL"
             column_sql.append(sql)
 
-        return "CREATE TABLE %s (%s)" % (self._table_name(namespace), ", ".join(column_sql))
+        return "CREATE TABLE %s (%s);" % (self._table_name(namespace), ", ".join(column_sql))
 
     def build_count_query(self, where="", parameters={}):
         join_set = set()
 
         # Parse the where clause.
         where_clause, where_parameters = "", {}
         if where:
```

### Comparing `muninn-6.0.1/muninn/tools/update.py` & `muninn-6.1/muninn/tools/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import logging
 import multiprocessing
 import sys
 
 try:
     from tqdm import tqdm as bar
 except ImportError:
-    def bar(range, total=None):
+    def bar(range, total=None, disable=None):
         return range
 
 import muninn
 from muninn.struct import Struct
 
 from muninn.tools.utils import Processor, create_parser, parse_args_and_run
 
@@ -81,19 +81,19 @@
         else:
             products = archive.search(expression, namespaces=archive.namespaces())
         if args.parallel:
             if args.processes is not None:
                 pool = multiprocessing.Pool(args.processes)
             else:
                 pool = multiprocessing.Pool()
-            list(bar(pool.imap(processor, products), total=len(products)))
+            list(bar(pool.imap(processor, products), total=len(products), disable=None))
             pool.close()
             pool.join()
         else:
-            for product in bar(products):
+            for product in bar(products, disable=None):
                 processor.perform_operation(archive, product)
 
     return 0
 
 
 def main():
     parser = create_parser(description="""Updates properties of existing products.
```

### Comparing `muninn-6.0.1/muninn/tools/ingest.py` & `muninn-6.1/muninn/tools/ingest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import argparse
 import fnmatch
 import glob
```

### Comparing `muninn-6.0.1/muninn/tools/pull.py` & `muninn-6.1/muninn/tools/pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import logging
 
 import muninn
```

### Comparing `muninn-6.0.1/muninn/tools/destroy.py` & `muninn-6.1/muninn/tools/destroy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 from muninn._compat import input
 import muninn
```

### Comparing `muninn-6.0.1/muninn/tools/untag.py` & `muninn-6.1/muninn/tools/untag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import muninn
 
 from muninn.tools.utils import Processor, create_parser, parse_args_and_run
```

### Comparing `muninn-6.0.1/muninn/tools/remove.py` & `muninn-6.1/muninn/tools/remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import muninn
 
 from muninn.tools.utils import Processor, create_parser, parse_args_and_run
```

### Comparing `muninn-6.0.1/muninn/tools/attach.py` & `muninn-6.1/muninn/tools/attach.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import logging
 import sys
 import os
```

### Comparing `muninn-6.0.1/muninn/tools/export.py` & `muninn-6.1/muninn/tools/export.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import argparse
 import logging
 import os
```

### Comparing `muninn-6.0.1/muninn/tools/hash.py` & `muninn-6.1/muninn/tools/hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import logging
 import sys
```

### Comparing `muninn-6.0.1/muninn/tools/summary.py` & `muninn-6.1/muninn/tools/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import re
 from datetime import timedelta
 import argparse
```

### Comparing `muninn-6.0.1/muninn/tools/utils.py` & `muninn-6.1/muninn/tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import argparse
 import logging
 import multiprocessing
@@ -11,15 +11,15 @@
 import sys
 
 try:
     from tqdm import tqdm as bar
     from multiprocessing import RLock
     RLock()  # fork off resource tracker before tqdm does it (with multiple threads running)
 except ImportError:
-    def bar(range, total=None):
+    def bar(range, total=None, disable=None):
         return range
 
 import muninn
 
 
 # This is a base class for operations on a list of items that can be performed in parallel using multiprocessing.
 # If you use the processor object as a callable then it is assumed that the operation is performed using subprocesses.
@@ -53,20 +53,20 @@
             pass
 
     def process(self, archive, args, items):
         total = len(items)
         num_success = 0
 
         if args.parallel:
-            num_success = sum(list(bar(_POOL.imap(self, items), total=total)))
+            num_success = sum(list(bar(_POOL.imap(self, items), total=total, disable=None)))
             _POOL.close()
             _POOL.join()
 
         elif total > 1:
-            for item in bar(items):
+            for item in bar(items, disable=None):
                 num_success += self.perform_operation(archive, item)
 
         elif total == 1:
             # don't show progress bar if we ingest just one item
             num_success = self.perform_operation(archive, items[0])
 
         return 0 if num_success == total else 1
```

### Comparing `muninn-6.0.1/muninn/tools/retrieve.py` & `muninn-6.1/muninn/tools/strip.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,43 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
-import os
-import argparse
-
 import muninn
 
 from muninn.tools.utils import Processor, create_parser, parse_args_and_run
 
 
-def directory(text):
-    if not os.path.isdir(text):
-        raise argparse.ArgumentTypeError("no such directory: %r" % text)
-
-    return text
-
-
-class RetrieveProcessor(Processor):
-    def __init__(self, args, target_path):
-        super(RetrieveProcessor, self).__init__(args)
+class StripProcessor(Processor):
+    def __init__(self, args):
+        super(StripProcessor, self).__init__(args)
         self.args = args
-        self.target_path = target_path
 
     def perform_operation(self, archive, product):
-        archive.retrieve(product.core.uuid, target_path=self.target_path, use_symlinks=self.args.link)
+        archive.strip(product.core.uuid, force=self.args.force, cascade=False)
         return 1
 
 
-def retrieve(args):
-    target_path = os.getcwd() if args.directory is None else args.directory
-    processor = RetrieveProcessor(args, target_path)
-
+def strip(args):
+    processor = StripProcessor(args)
     with muninn.open(args.archive) as archive:
         products = archive.search(where=args.expression, property_names=['uuid'])
-        return processor.process(archive, args, products)
+        returncode = processor.process(archive, args, products)
+        archive.cleanup_derived_products()
+        return returncode
 
 
 def main():
-    parser = create_parser(description="Retrieve products from a muninn archive.", parallel=True)
-    parser.add_argument("-d", "--directory", type=directory, help="directory in which retrieved products will be"
-                        " stored; by default, retrieved products will be stored in the current working directory")
-    parser.add_argument("-l", "--link", action="store_true", help="retrieve using symbolic links instead of copy")
+    parser = create_parser(description="Strip products contained in a muninn archive (i.e. remove "
+                           "products from disk, but don't remove the corresponding entries from the product "
+                           "catalogue)", parallel=True)
+    parser.add_argument("-f", "--force", action="store_true", help="also strip partially ingested products; note"
+                        " that this can cause product files to be removed while in the process of being ingested")
     parser.add_argument("archive", metavar="ARCHIVE", help="identifier of the archive to use")
-    parser.add_argument("expression", metavar="EXPRESSION", help="expression used to search for products to retrieve")
-    return parse_args_and_run(parser, retrieve)
+    parser.add_argument("expression", metavar="EXPRESSION", help="expression used to search for products to remove")
+    return parse_args_and_run(parser, strip)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `muninn-6.0.1/muninn/tools/search.py` & `muninn-6.1/muninn/tools/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import argparse
 import logging
```

### Comparing `muninn-6.0.1/muninn/tools/list_tags.py` & `muninn-6.1/muninn/tools/list_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import muninn
 
 from muninn.tools.utils import create_parser, parse_args_and_run
```

### Comparing `muninn-6.0.1/muninn/tools/info.py` & `muninn-6.1/muninn/tools/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import muninn
 
 from .utils import create_parser, parse_args_and_run
```

### Comparing `muninn-6.0.1/muninn/tools/prepare.py` & `muninn-6.1/muninn/tools/prepare.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import muninn
 
 from muninn.tools.utils import create_parser, parse_args_and_run
 
 
 def prepare(args):
     with muninn.open(args.archive) as archive:
         if args.dry_run:
             print("The following SQL statements would be executed:")
+            print()
             for sql in archive.prepare_catalogue(dry_run=True):
-                print("  " + sql)
+                print(sql)
         elif args.catalogue_only:
             archive.prepare_catalogue()
         else:
             archive.prepare(force=args.force)
     return 0
```

### Comparing `muninn-6.0.1/muninn/tools/tag.py` & `muninn-6.1/muninn/tools/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import muninn
 
 from muninn.tools.utils import Processor, create_parser, parse_args_and_run
```

### Comparing `muninn-6.0.1/muninn/config.py` & `muninn-6.1/muninn/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 from muninn._compat import string_types as basestring
 
 from muninn.schema import *
```

### Comparing `muninn-6.0.1/muninn/remote.py` & `muninn-6.1/muninn/remote.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 from __future__ import absolute_import, division, print_function
 
 import logging
 import os
 import re
 import json
@@ -31,55 +31,74 @@
         hostname = urlparse(url).hostname
         if hostname in credentials:
             return credentials[hostname]
     return None
 
 
 def download_http_oath2(url, target_dir, credentials, timeout=60):
+    import requests
     from requests_oauthlib import OAuth2Session
     from oauthlib.oauth2 import LegacyApplicationClient
 
     assert credentials['grant_type'] == "ResourceOwnerPasswordCredentialsGrant"
 
     session = OAuth2Session(client=LegacyApplicationClient(client_id=credentials['client_id']))
     session.fetch_token(token_url=credentials['token_url'], username=credentials['username'],
                         password=credentials['password'], client_id=credentials['client_id'],
                         client_secret=credentials['client_secret'])
     try:
-        r = session.get(url, timeout=timeout, stream=True)
-        r.raise_for_status()
-        local_file = os.path.join(target_dir, os.path.basename(urlparse(r.url).path))
-        if "content-disposition" in [k.lower() for k in r.headers.keys()]:
-            matches = re.findall("filename=\"?([^\"]+)\"?", r.headers["content-disposition"])
-            if len(matches) > 0:
-                local_file = os.path.join(target_dir, matches[-1])
-        with open(local_file, 'wb') as output:
-            for block in r.iter_content(1048576):  # use 1MB blocks
-                output.write(block)
+        retry = 1
+        while True:
+            try:
+                r = session.get(url, timeout=timeout, stream=True)
+                r.raise_for_status()
+                local_file = os.path.join(target_dir, os.path.basename(urlparse(r.url).path))
+                if "content-disposition" in [k.lower() for k in r.headers.keys()]:
+                    matches = re.findall("filename=\"?([^\"]+)\"?", r.headers["content-disposition"])
+                    if len(matches) > 0:
+                        local_file = os.path.join(target_dir, matches[-1])
+                with open(local_file, 'wb') as output:
+                    for block in r.iter_content(1048576):  # use 1MB blocks
+                        output.write(block)
+            except requests.exceptions.ReadTimeout:
+                if retry <= 0:
+                    raise
+                retry -= 1
+            else:
+                break
     except Exception as e:
         raise DownloadError('Error downloading %s (Reason: %s)' % (url, e))
     return local_file
 
 
 def download_http(url, target_dir, credentials=None, timeout=60):
     import requests
     auth = None
     if credentials is not None:
         auth = (credentials['username'], credentials['password'])
     try:
-        r = requests.get(url, timeout=timeout, stream=True, auth=auth)
-        r.raise_for_status()
-        local_file = os.path.join(target_dir, os.path.basename(urlparse(r.url).path))
-        if "content-disposition" in [k.lower() for k in r.headers.keys()]:
-            matches = re.findall("filename=\"?([^\"]+)\"?", r.headers["content-disposition"])
-            if len(matches) > 0:
-                local_file = os.path.join(target_dir, matches[-1])
-        with open(local_file, 'wb') as output:
-            for block in r.iter_content(1048576):  # use 1MB blocks
-                output.write(block)
+        retry = 1
+        while True:
+            try:
+                r = requests.get(url, timeout=timeout, stream=True, auth=auth)
+                r.raise_for_status()
+                local_file = os.path.join(target_dir, os.path.basename(urlparse(r.url).path))
+                if "content-disposition" in [k.lower() for k in r.headers.keys()]:
+                    matches = re.findall("filename=\"?([^\"]+)\"?", r.headers["content-disposition"])
+                    if len(matches) > 0:
+                        local_file = os.path.join(target_dir, matches[-1])
+                with open(local_file, 'wb') as output:
+                    for block in r.iter_content(1048576):  # use 1MB blocks
+                        output.write(block)
+            except requests.exceptions.ReadTimeout:
+                if retry <= 0:
+                    raise
+                retry -= 1
+            else:
+                break
     except Exception as e:
         raise DownloadError('Error downloading %s (Reason: %s)' % (url, e))
     return local_file
 
 
 def download_ftp(url, target_dir, credentials=None, timeout=60):
     url = urlparse(url)
@@ -157,17 +176,24 @@
                 util.remove_path(file_path)
                 return paths
 
         tar_extensions = [".tar", ".tgz", ".tar.gz", ".txz", ".tar.xz", ".tbz", ".tb2", "tar.bz2"]
         tar_extensions += [extension.upper() for extension in tar_extensions]
         for extension in tar_extensions:
             if filename == product.core.physical_name + extension:
+                absdirname = os.path.abspath(dirname)
                 with tarfile.open(file_path) as tararchive:
-                    tararchive.extractall(dirname)
-                    paths = set([path.split('/', 1)[0] for path in tararchive.getnames()])
+                    paths = []
+                    for member in tararchive.getmembers():
+                        # CVE-2007-4559: only extract tar members that end up inside the extraction target directory
+                        member_path = os.path.abspath(os.path.join(dirname, member.name))
+                        if os.path.commonprefix([absdirname, member_path]) == absdirname:
+                            paths += [os.path.relpath(member_path, dirname)]
+                            tararchive.extract(member, dirname)
+                    paths = set([path.split('/', 1)[0] for path in paths])
                     paths = [os.path.join(dirname, path) for path in sorted(paths)]
                 util.remove_path(file_path)
                 return paths
 
         return [file_path]
 
 
@@ -234,13 +260,13 @@
         if verify_hash_download and stored_hash is not None:
             hash_type = archive._extract_hash_type(stored_hash)
             if hash_type is None:
                 stored_hash = 'sha1:' + stored_hash
                 hash_type = 'sha1'
             calc_hash = util.product_hash(paths, hash_type=hash_type)
             if calc_hash != stored_hash:
-                raise DownloadError("hash mismatch when pulling product '%s' (%s)" %
+                raise DownloadError("hash mismatch when retrieving product '%s' (%s)" %
                                     (product.core.product_name, product.core.uuid))
 
         return paths
 
     return retrieve_files
```

### Comparing `muninn-6.0.1/muninn/util.py` & `muninn-6.1/muninn/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import errno
 import hashlib
 import os
```

### Comparing `muninn-6.0.1/muninn/__init__.py` & `muninn-6.1/muninn/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
-__version__ = "6.0.1"
-__copyright__ = "Copyright (C) 2014-2022 S[&]T, The Netherlands."
+__version__ = "6.1"
+__copyright__ = "Copyright (C) 2014-2023 S[&]T, The Netherlands."
 
 __all__ = ["Error", "InternalError", "Struct", "Archive", "open", "config_path"]
 
 import os as _os
 
 from muninn.archive import Archive
 from muninn.exceptions import *
```

### Comparing `muninn-6.0.1/muninn/core.py` & `muninn-6.1/muninn/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import os
 
 from muninn.schema import *
```

### Comparing `muninn-6.0.1/muninn/storage/fs.py` & `muninn-6.1/muninn/storage/fs.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     return FilesystemStorageBackend(tempdir=tempdir, **options)
 
 
 class FilesystemStorageBackend(StorageBackend):
     def __init__(self, root, use_symlinks=None, tempdir=None):
         super(FilesystemStorageBackend, self).__init__(tempdir)
 
+        self.global_prefix = root
         self._root = os.path.realpath(root)
         self._use_symlinks = use_symlinks or False
         self.supports_symlinks = True
 
     def prepare(self):
         # Create the archive root path.
         try:
@@ -39,15 +40,15 @@
     # tempdirs must be on the same file system for moves (below) to be atomic!
     def get_tmp_root(self, product):
         tmp_root = os.path.join(self._root, product.core.archive_path)
         util.make_path(tmp_root)
         return tmp_root
 
     def run_for_product(self, product, fn, use_enclosing_directory):
-        product_path = self.product_path(product)
+        product_path = os.path.join(self._root, product.core.archive_path, product.core.physical_name)
         if use_enclosing_directory:
             paths = [os.path.join(product_path, basename) for basename in os.listdir(product_path)]
         else:
             paths = [product_path]
         return fn(paths)
 
     def exists(self):
@@ -56,17 +57,14 @@
     def destroy(self):
         if self.exists():
             try:
                 util.remove_path(self._root)
             except EnvironmentError as _error:
                 raise Error("unable to remove archive root path '%s' [%s]" % (self._root, _error))
 
-    def product_path(self, product):
-        return os.path.join(self._root, product.core.archive_path, product.core.physical_name)
-
     def current_archive_path(self, paths, properties):
         for path in paths:
             if not util.is_sub_path(os.path.realpath(path), self._root, allow_equal=True):
                 raise Error("cannot ingest a file in-place if it is not inside the muninn archive root")
 
         abs_archive_path = os.path.dirname(os.path.realpath(paths[0]))
 
@@ -165,41 +163,52 @@
                     # Run optional function on result
                     if run_for_product is not None:
                         self.run_for_product(properties, run_for_product, use_enclosing_directory)
 
             except Exception as e:
                 raise StorageError(e, anything_stored)
 
-    # TODO product_path follows from product
-    def get(self, product, product_path, target_path, use_enclosing_directory, use_symlinks=None):
+    def get(self, product, target_path, use_enclosing_directory, use_symlinks=None):
+        paths = []
+
         if use_symlinks is None:
             use_symlinks = self._use_symlinks
 
+        product_path = os.path.join(self._root, product.core.archive_path, product.core.physical_name)
+        product_basename = os.path.basename(product_path)
+
         try:
             if use_symlinks:
                 if use_enclosing_directory:
                     for basename in os.listdir(product_path):
                         os.symlink(os.path.join(product_path, basename), os.path.join(target_path, basename))
+                        paths.append(os.path.join(target_path, basename))
                 else:
-                    os.symlink(product_path, os.path.join(target_path, os.path.basename(product_path)))
+                    os.symlink(product_path, os.path.join(target_path, product_basename))
+                    paths.append(os.path.join(target_path, product_basename))
             else:
                 if use_enclosing_directory:
                     for basename in os.listdir(product_path):
                         util.copy_path(os.path.join(product_path, basename), target_path, resolve_root=True)
+                        paths.append(os.path.join(target_path, basename))
                 else:
                     util.copy_path(product_path, target_path, resolve_root=True)
+                    paths.append(os.path.join(target_path, product_basename))
 
         except EnvironmentError as _error:
             raise Error("unable to retrieve product '%s' (%s) [%s]" % (product.core.product_name, product.core.uuid,
                                                                        _error))
 
+        return paths
+
     def size(self, product_path):
-        return util.product_size(product_path)
+        return util.product_size(os.path.join(self._root, product_path))
 
     def delete(self, product_path, properties):
+        product_path = os.path.join(self._root, product_path)
         if not os.path.lexists(product_path):
             # If the product does not exist, do not consider this an error.
             return
 
         try:
             tmp_root = self.get_tmp_root(properties)
             with util.TemporaryDirectory(prefix=".remove-", suffix="-%s" % properties.core.uuid.hex,
@@ -220,15 +229,15 @@
             return paths
 
         # Make target archive path
         abs_archive_path = os.path.realpath(os.path.join(self._root, archive_path))
         util.make_path(abs_archive_path)
 
         # Move files there
-        product_path = self.product_path(product)
+        product_path = os.path.join(self._root, product.core.archive_path, product.core.physical_name)
         os.rename(product_path, os.path.join(abs_archive_path, product.core.physical_name))
 
         # Optionally rewrite (local) paths
         if paths is not None:
             paths = [os.path.join(self._root, archive_path,
                                   os.path.relpath(path, os.path.join(self._root, product.core.archive_path)))
                      for path in paths]
```

### Comparing `muninn-6.0.1/muninn/storage/swift.py` & `muninn-6.1/muninn/storage/swift.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,14 @@
 
     def destroy(self):  # TODO individually deleting objects
         if self.exists():
             for data in self._conn.get_container(self.container)[1]:
                 self._conn.delete_object(self.container, data['name'])
             self._conn.delete_container(self.container)
 
-    def product_path(self, product):  # TODO needed?
-        return os.path.join(product.core.archive_path, product.core.physical_name)
-
     def current_archive_path(self, paths, properties):
         raise Error("Swift storage backend does not support ingesting already archived products")
 
     def put(self, paths, properties, use_enclosing_directory, use_symlinks=None,
             retrieve_files=None, run_for_product=None):
 
         if use_symlinks:
@@ -141,36 +138,44 @@
 
                 if run_for_product is not None:
                     run_for_product(paths)
 
         except Exception as e:
             raise StorageError(e, anything_stored)
 
-    def get(self, product, product_path, target_path, use_enclosing_directory, use_symlinks=None):
+    def get(self, product, target_path, use_enclosing_directory, use_symlinks=None):
+        paths = []
+
         if use_symlinks:
             raise Error("Swift storage backend does not support symlinks")
 
         archive_path = product.core.archive_path
+        product_path = os.path.join(archive_path, product.core.physical_name)
 
         keys = self._object_keys(product_path)
         if not keys:
             raise Error("no data for product '%s' (%s)" % (product.core.product_name, product.core.uuid))
 
         for key in keys:
             rel_path = os.path.relpath(key, archive_path)
             if use_enclosing_directory:
                 rel_path = '/'.join(rel_path.split('/')[1:])
             target = os.path.normpath(os.path.join(target_path, rel_path))
             if key.endswith('/'):
                 util.make_path(target)
             else:
-                util.make_path(os.path.dirname(target))
+                dirname = os.path.dirname(target)
+                if dirname != '':
+                    util.make_path(dirname)
                 binary = self._conn.get_object(self.container, key)[1]
                 with open(target, 'wb') as f:
                     f.write(binary)
+                paths.append(target)
+
+        return paths
 
     def delete(self, product_path, properties):
         for key in self._object_keys(product_path):
             self._conn.delete_object(self.container, key)
 
     def size(self, product_path):
         total = 0
@@ -179,20 +184,24 @@
         return total
 
     def move(self, product, archive_path, paths=None):
         # Ignore if product already there
         if product.core.archive_path == archive_path:
             return paths
 
-        product_path = self.product_path(product)
+        product_path = os.path.join(product.core.archive_path, product.core.physical_name)
         new_product_path = os.path.join(archive_path, product.core.physical_name)
 
         keys = self._object_keys(product_path)
         if not keys:
             raise Error("no data for product '%s' (%s)" % (product.core.product_name, product.core.uuid))
 
         for key in keys:
             new_key = os.path.normpath(os.path.join(new_product_path, os.path.relpath(key, product_path)))
-            self._conn.copy_object(self.container, key, os.path.join(self.container, new_key))
+            if key.endswith('/'):
+                self._conn.put_object(self.container, new_key+'/', contents=b'')
+            else:
+                self._conn.copy_object(self.container, key, os.path.join(self.container, new_key))
+
             self._conn.delete_object(self.container, key)
 
         return paths
```

### Comparing `muninn-6.0.1/muninn/storage/s3.py` & `muninn-6.1/muninn/storage/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,50 +112,49 @@
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == "404":
                 return False
             else:
                 raise
 
     def _prefix_exists(self):
-        if self._prefix:  # TODO created but still empty archive
+        if self._prefix:
             objs = list(self._resource.Bucket(self.bucket).objects.limit(count=1).filter(Prefix=self._prefix))
             return len(objs) == 1
         else:
             return True
 
     def prepare(self):
         if not self._bucket_exists():
             self._resource.create_bucket(Bucket=self.bucket)
+        if not self._prefix_exists():
+            self._create_dir(self._prefix)
 
     def exists(self):
         return self._bucket_exists() and self._prefix_exists()
 
     def destroy(self):
         if self._prefix:
             self._resource.Bucket(self.bucket).objects.filter(Prefix=self._prefix).delete()
         elif self._bucket_exists():
             bucket = self._resource.Bucket(self.bucket)
             bucket.objects.all().delete()
             bucket.delete()
 
-    def product_path(self, product):  # TODO needed?
-        return os.path.join(product.core.archive_path, product.core.physical_name)
-
     def current_archive_path(self, paths, properties):
         raise Error("S3 storage backend does not support ingesting already archived products")
 
     def _upload_file(self, key, path):
         obj = self._resource.Object(self.bucket, key)
-        if os.path.getsize(path) == 0:  # TODO otherwise upload_file hangs sometimes!?
+        if os.path.getsize(path) == 0:  # upload_file can hang on empty files
             self._resource.Object(self.bucket, key).put()
         else:
             obj.upload_file(path, ExtraArgs=self._upload_args, Config=self._transfer_config)
 
     def _create_dir(self, key):
-        # using put, as upload_file/upload_fileobj do not like the trailish slash
+        # using put, as upload_file/upload_fileobj do not like the trailing slash
         self._resource.Object(self.bucket, key+'/').put()
 
     def put(self, paths, properties, use_enclosing_directory, use_symlinks=None,
             retrieve_files=None, run_for_product=None):
 
         if use_symlinks:
             raise Error("S3 storage backend does not support symlinks")
@@ -207,19 +206,22 @@
 
                 if run_for_product is not None:
                     run_for_product(paths)
 
         except Exception as e:
             raise StorageError(e, anything_stored)
 
-    def get(self, product, product_path, target_path, use_enclosing_directory, use_symlinks=None):
+    def get(self, product, target_path, use_enclosing_directory, use_symlinks=None):
+        paths = []
+
         if use_symlinks:
             raise Error("S3 storage backend does not support symlinks")
 
         archive_path = product.core.archive_path
+        product_path = os.path.join(archive_path, product.core.physical_name)
         prefix = self._prefix + product_path
 
         objs = list(self._resource.Bucket(self.bucket).objects.filter(Prefix=prefix))
         if not objs:
             raise Error("no data for product '%s' (%s)" % (product.core.product_name, product.core.uuid))
 
         for obj in objs:
@@ -227,17 +229,22 @@
             if use_enclosing_directory:
                 rel_path = '/'.join(rel_path.split('/')[1:])
             target = os.path.normpath(os.path.join(target_path, rel_path))
 
             if obj.key.endswith('/'):
                 util.make_path(target)
             else:
-                util.make_path(os.path.dirname(target))
+                dirname = os.path.dirname(target)
+                if dirname != '':
+                    util.make_path(dirname)
                 self._resource.Object(self.bucket, obj.key).download_file(target, ExtraArgs=self._download_args,
                                                                           Config=self._transfer_config)
+                paths.append(target)
+
+        return paths
 
     def delete(self, product_path, properties):
         prefix = self._prefix + product_path
         for obj in self._resource.Bucket(self.bucket).objects.filter(Prefix=prefix):
             obj.delete()
 
     def size(self, product_path):
@@ -248,21 +255,24 @@
         return total
 
     def move(self, product, archive_path, paths=None):
         # Ignore if product already there
         if product.core.archive_path == archive_path:
             return paths
 
-        product_path = self._prefix + self.product_path(product)
-        new_product_path = self._prefix + os.path.join(archive_path, product.core.physical_name)
+        product_path = os.path.join(self._prefix, product.core.archive_path, product.core.physical_name)
+        new_product_path = os.path.join(self._prefix, archive_path, product.core.physical_name)
 
         objs = list(self._resource.Bucket(self.bucket).objects.filter(Prefix=product_path))
         if not objs:
             raise Error("no data for product '%s' (%s)" % (product.core.product_name, product.core.uuid))
 
         for obj in objs:
             new_key = os.path.normpath(os.path.join(new_product_path, os.path.relpath(obj.key, product_path)))
-            self._resource.Object(self.bucket, new_key).copy(CopySource={'Bucket': self.bucket, 'Key': obj.key},
+            if obj.key.endswith('/'):
+                self._create_dir(new_key)
+            else:
+                self._resource.Object(self.bucket, new_key).copy(CopySource={'Bucket': self.bucket, 'Key': obj.key},
                                                              ExtraArgs=self._copy_args, Config=self._transfer_config)
             self._resource.Object(self.bucket, obj.key).delete()
 
         return paths
```

### Comparing `muninn-6.0.1/muninn/storage/base.py` & `muninn-6.1/muninn/storage/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,24 +13,23 @@
             util.make_path(tmp_root)
             self._tmp_root = tmp_root
         else:
             self._tmp_root = None
 
     def get_tmp_root(self, product):
         if self._tmp_root is not None:
-            tmp_root = os.path.join(self._tmp_root, product.core.archive_path)
-            util.make_path(tmp_root)
-            return tmp_root
+            util.make_path(self._tmp_root)
+            return self._tmp_root
 
     def run_for_product(self, product, fn, use_enclosing_directory):
         tmp_root = self.get_tmp_root(product)
-        product_path = self.product_path(product)
+        product_path = os.path.join(product.core.archive_path, product.core.physical_name)
         with util.TemporaryDirectory(dir=tmp_root, prefix=".run_for_product-",
                                      suffix="-%s" % product.core.uuid.hex) as tmp_path:
-            self.get(product, product_path, tmp_path, use_enclosing_directory)
+            self.get(product, tmp_path, use_enclosing_directory)
             paths = [os.path.join(tmp_path, basename) for basename in os.listdir(tmp_path)]
             return fn(paths)
 
     def prepare(self):  # pragma: no cover
         # Prepare storage for use.
         raise NotImplementedError()
 
@@ -42,25 +41,20 @@
         # Initialize storage.
         raise NotImplementedError()
 
     def destroy(self):  # pragma: no cover
         # Destroy storage
         raise NotImplementedError()
 
-    # TODO refactor away?
-    def product_path(self, product):  # pragma: no cover
-        # Product path within storage
-        raise NotImplementedError()
-
     def put(self, paths, properties, use_enclosing_directory, use_symlinks=None,
             retrieve_files=None, run_for_product=None):  # pragma: no cover
         # Place product file(s) into storage
         raise NotImplementedError()
 
-    def get(self, product, product_path, target_path, use_enclosing_directory, use_symlinks=None):  # pragma: no cover
+    def get(self, product, target_path, use_enclosing_directory, use_symlinks=None):  # pragma: no cover
         # Retrieve product file(s) from storage
         raise NotImplementedError()
 
     def size(self, product_path):  # pragma: no cover
         # Return product storage size
         raise NotImplementedError()
```

### Comparing `muninn-6.0.1/muninn/visitor.py` & `muninn-6.1/muninn/visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import inspect
```

### Comparing `muninn-6.0.1/muninn/geometry.py` & `muninn-6.1/muninn/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 try:
     from collections.abc import MutableSequence
 except ImportError:
```

### Comparing `muninn-6.0.1/muninn/language.py` & `muninn-6.1/muninn/language.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 from muninn._compat import string_types as basestring
 
 import copy
@@ -268,15 +268,15 @@
 
         token = self.token
         self.next()
         return token
 
     def _types_to_string(self, types):
         try:
-            strings = map(TokenType.to_string, types)
+            strings = [TokenType.to_string(t) for t in types]
         except TypeError:
             return TokenType.to_string(types)
 
         return "%s%s" % ("" if len(strings) == 1 else "one of: ", ", ".join(strings))
 
     def _values_to_string(self, values):
         if isinstance(values, basestring):
```

### Comparing `muninn-6.0.1/muninn/archive.py` & `muninn-6.1/muninn/archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 from muninn._compat import string_types as basestring
 
 import collections
 import copy
@@ -422,17 +422,15 @@
             assert len(products) == 1
             return products[0]
 
     def _get_products(self, where, parameters=None, namespaces=None, property_names=None):  # TODO generator?
         if isinstance(where, basestring):
             return self.search(where, parameters=parameters, namespaces=namespaces, property_names=property_names)
 
-        if isinstance(where, UUID):
-            where = [where]
-        elif isinstance(where, Struct):
+        if isinstance(where, (UUID, Struct)):
             where = [where]
         else:
             try:
                 where = list(where)
             except Exception:
                 raise Error('Invalid product selection')
 
@@ -464,15 +462,15 @@
         else:
             return 'md5'  # default after use_hash deprecation
 
     def _product_path(self, product):
         if self._storage is None or getattr(product.core, 'archive_path', None) is None:
             return None
 
-        return self._storage.product_path(product)
+        return os.path.join(product.core.archive_path, product.core.physical_name)
 
     def _purge(self, product):
         # get full product
         product = self._get_product(product.core.uuid)
 
         # Remove the product from the product catalogue.
         self._database.delete_product_properties(product.core.uuid)
@@ -508,35 +506,42 @@
         product_path = self._product_path(product)
         if product_path is None:
             return
 
         # Remove the data associated with the product from storage.
         self._storage.delete(product_path, product)
 
-    def _retrieve(self, product, target_path, use_symlinks=False):
+    def _retrieve(self, product, target_path, use_symlinks=False, verify_hash=False):
         if 'archive_path' in product.core:
             # Determine the path of the product in storage.
             product_path = self._product_path(product)
 
             # Get the product type specific plugin.
             plugin = self.product_type_plugin(product.core.product_type)
             use_enclosing_directory = plugin.use_enclosing_directory
 
             # Symbolic link or copy the product at or to the specified target directory.
-            self._storage.get(product, product_path, target_path, use_enclosing_directory, use_symlinks)
+            paths = self._storage.get(product, target_path, use_enclosing_directory, use_symlinks)
 
-            return os.path.join(target_path, os.path.basename(product_path))
+            if verify_hash and 'hash' in product.core and not self._verify_hash(product, paths):
+                raise Error("retrieved product '%s' (%s) has incorrect hash" %
+                            (product.core.product_name, product.core.uuid))
+
+            if not use_enclosing_directory:
+                paths = paths[0]
 
         elif 'remote_url' in product.core:
-            retrieve_files = remote.retrieve_function(self, product, True)
-            retrieve_files(target_path)
+            retrieve_files = remote.retrieve_function(self, product, verify_hash)
+            paths = retrieve_files(target_path)
 
         else:
             raise Error("product '%s' (%s) not available" % (product.core.product_name, product.core.uuid))
 
+        return paths
+
     def _run_hooks(self, hook_name, properties, reverse=False, paths=None):
         plugins = list(self._hook_extensions.values())
         plugin = self._product_type_plugins.get(properties.core.product_type)
         if plugin is not None:
             plugins.insert(0, plugin)
 
         if reverse:
@@ -954,15 +959,15 @@
                 raise Error("export format '%s' not supported for product '%s' (%s)" %
                             (format, product.core.product_name, product.core.uuid))
 
             else:
                 exported_path = self._retrieve(product, target_path, False)
                 result.append(exported_path)
 
-        if isinstance(where, UUID):
+        if isinstance(where, (UUID, Struct)):
             return result[0]
         else:
             return result
 
     def export_formats(self):
         """Return a list of supported alternative export formats."""
         return list(self._export_formats)
@@ -1221,15 +1226,15 @@
                                             property_names=property_names)
             else:
                 product = self._get_product(uuid_or_properties.core.uuid,
                                             property_names=property_names)
 
         archive_path = getattr(product.core, 'archive_path', None)
         remote_url = getattr(product.core, 'remote_url', None)
-        if archive_path is not None:
+        if archive_path is not None and self._storage is not None:
             product_path = self._product_path(product)
             return os.path.join(self._storage.global_prefix, product_path)
         elif remote_url is not None:
             return remote_url
 
     def pull(self, where="", parameters={}, verify_hash=False, verify_hash_download=False):
         """Pull one or more remote products into the archive.
@@ -1466,41 +1471,43 @@
 
         # Remove (or strip) derived products if necessary.
         if cascade and len(products) > 0:
             self.cleanup_derived_products()
 
         return len(products)
 
-    def retrieve(self, where="", parameters={}, target_path=os.path.curdir, use_symlinks=False):
+    def retrieve(self, where="", parameters={}, target_path=os.path.curdir, use_symlinks=False, verify_hash=False):
         """Retrieve one or more products from the archive.
 
         Arguments:
         where           --  Search expression or one or more product uuid(s) or properties.
         parameters      --  Parameters referenced in the search expression.
         target_path     --  Directory under which the retrieved products will be stored.
         use_symlinks    --  If set to True, products will be retrieved as symbolic links to the original products kept
                             in the archive. If set to False, products will retrieved as copies of the original products.
                             By default, products will be retrieved as copies.
+        verify_hash     --  If set to True then, after the retrieval, the product will be matched against the hash
+                            from the metadata (only if the metadata contained a hash).
 
         Returns:
         Either a list containing the target paths for the
         retrieved products (when a search expression or multiple
         properties/uuids were passed), or a single target path.
 
         """
         products = self._get_products(where, parameters, property_names=_CORE_PROP_NAMES + ['remote_url'])
 
         result = []
         for product in products:
             if product.core.active and ('archive_path' in product.core or 'remote_url' in product.core):
-                result.append(self._retrieve(product, target_path, use_symlinks))
+                result.append(self._retrieve(product, target_path, use_symlinks, verify_hash))
             else:
                 raise Error("product '%s' (%s) not available" % (product.core.product_name, product.core.uuid))
 
-        if isinstance(where, UUID):
+        if isinstance(where, (UUID, Struct)):
             return result[0]
         else:
             return result
 
     def retrieve_properties(self, uuid, namespaces=[], property_names=[]):
         """Return properties for the specified product.
 
@@ -1688,15 +1695,15 @@
         separately.
 
         This function allows any property to be changed with the exception of the product UUID, and therefore needs to
         be used with care. The recommended way to update product properties is to first retrieve them using either
         retrieve_properties() or search(), change the properties, and then use this function to update the product
         catalogue.
 
-        Argument:
+        Arguments:
         properties         -- Product properties
         uuid               -- UUID of the product to update. By default, the UUID will be taken from the "core.uuid"
                               property.
         create_namespaces  -- Test if all namespaces are already defined for the product, and create them if needed.
         """
         if create_namespaces:
             if 'core' in properties and 'uuid' in properties.core:
```

### Comparing `muninn-6.0.1/muninn/enum.py` & `muninn-6.1/muninn/enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 
 class MetaEnum(type):
     def __new__(meta, name, bases, dct):
```

### Comparing `muninn-6.0.1/muninn/_compat.py` & `muninn-6.1/muninn/_compat.py`

 * *Files identical despite different names*

### Comparing `muninn-6.0.1/muninn/function.py` & `muninn-6.1/muninn/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 from muninn._compat import itervalues, imap, izip
 
 try:
     from collections.abc import MutableSet
```

### Comparing `muninn-6.0.1/muninn/struct.py` & `muninn-6.1/muninn/struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 from muninn.exceptions import Error
```

### Comparing `muninn-6.0.1/muninn/schema.py` & `muninn-6.1/muninn/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2022 S[&]T, The Netherlands.
+# Copyright (C) 2014-2023 S[&]T, The Netherlands.
 #
 
 from __future__ import absolute_import, division, print_function
 
 import datetime
 from muninn._compat import long
 from muninn._compat import string_types as basestring
```

### Comparing `muninn-6.0.1/muninn.egg-info/PKG-INFO` & `muninn-6.1/muninn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: muninn
-Version: 6.0.1
+Version: 6.1
 Summary: Data product catalogue and archive system
 Home-page: https://github.com/stcorp/muninn
 Author: S[&]T
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `muninn-6.0.1/muninn.egg-info/SOURCES.txt` & `muninn-6.1/muninn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `muninn-6.0.1/muninn.egg-info/entry_points.txt` & `muninn-6.1/muninn.egg-info/entry_points.txt`

 * *Files identical despite different names*

