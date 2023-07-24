# Comparing `tmp/sqlite_utils_sqlite_url-0.1.0-py3-none-any.whl.zip` & `tmp/sqlite_utils_sqlite_url-0.1.0a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2142 bytes, number of entries: 7
--rw-r--r--  2.0 unx      270 b- defN 23-Jul-24 06:08 sqlite_utils_sqlite_url/__init__.py
--rw-r--r--  2.0 unx       71 b- defN 23-Jul-24 06:08 sqlite_utils_sqlite_url/version.py
--rw-r--r--  2.0 unx      507 b- defN 23-Jul-24 06:09 sqlite_utils_sqlite_url-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 06:09 sqlite_utils_sqlite_url-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-24 06:09 sqlite_utils_sqlite_url-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 23-Jul-24 06:09 sqlite_utils_sqlite_url-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      652 b- defN 23-Jul-24 06:09 sqlite_utils_sqlite_url-0.1.0.dist-info/RECORD
-7 files, 1668 bytes uncompressed, 954 bytes compressed:  42.8%
+Zip file size: 2173 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      270 b- defN 23-Jul-24 04:29 sqlite_utils_sqlite_url/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jul-24 04:29 sqlite_utils_sqlite_url/version.py
+-rw-r--r--  2.0 unx      509 b- defN 23-Jul-24 04:29 sqlite_utils_sqlite_url-0.1.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 04:29 sqlite_utils_sqlite_url-0.1.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-24 04:29 sqlite_utils_sqlite_url-0.1.0a8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-24 04:29 sqlite_utils_sqlite_url-0.1.0a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      662 b- defN 23-Jul-24 04:29 sqlite_utils_sqlite_url-0.1.0a8.dist-info/RECORD
+7 files, 1688 bytes uncompressed, 965 bytes compressed:  42.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sqlite_utils_sqlite_url/__init__.py
 Comment: 
 
 Filename: sqlite_utils_sqlite_url/version.py
 Comment: 
 
-Filename: sqlite_utils_sqlite_url-0.1.0.dist-info/METADATA
+Filename: sqlite_utils_sqlite_url-0.1.0a8.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_utils_sqlite_url-0.1.0.dist-info/WHEEL
+Filename: sqlite_utils_sqlite_url-0.1.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_utils_sqlite_url-0.1.0.dist-info/entry_points.txt
+Filename: sqlite_utils_sqlite_url-0.1.0a8.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_url-0.1.0.dist-info/top_level.txt
+Filename: sqlite_utils_sqlite_url-0.1.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_url-0.1.0.dist-info/RECORD
+Filename: sqlite_utils_sqlite_url-0.1.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_utils_sqlite_url/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0"
+__version__ = "0.1.0-alpha.8"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_utils_sqlite_url-0.1.0.dist-info/RECORD` & `sqlite_utils_sqlite_url-0.1.0a8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sqlite_utils_sqlite_url/__init__.py,sha256=8Qp1HZ7obNkoo5spKw5jcpqBzp2G7orDpUWaY4Cj-kQ,270
-sqlite_utils_sqlite_url/version.py,sha256=oCpXiISrUNZEvF5jF6FEL7MUTdIxhrYYtlvRuj56P98,71
-sqlite_utils_sqlite_url-0.1.0.dist-info/METADATA,sha256=I904OU9zv5y72yUYhZIeb8ojxhJCCHHA5KS92GJVVDA,507
-sqlite_utils_sqlite_url-0.1.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-sqlite_utils_sqlite_url-0.1.0.dist-info/entry_points.txt,sha256=YGv7v73_28wITaq991gsNj5upqjMlfxQA0yfrncdKjw,52
-sqlite_utils_sqlite_url-0.1.0.dist-info/top_level.txt,sha256=QWDQv-iAhRydh0st_oXJqhFPgZqarsLC4lsvRjRlZoA,24
-sqlite_utils_sqlite_url-0.1.0.dist-info/RECORD,,
+sqlite_utils_sqlite_url/version.py,sha256=I0ZUcRKO4eykIcOSGighZnoI2j-WP8IxOzhHnNZBhaw,79
+sqlite_utils_sqlite_url-0.1.0a8.dist-info/METADATA,sha256=WvA-5WzvipXRoczG9eVZCwf1YhaScAoauXg7FP5bF7k,509
+sqlite_utils_sqlite_url-0.1.0a8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+sqlite_utils_sqlite_url-0.1.0a8.dist-info/entry_points.txt,sha256=YGv7v73_28wITaq991gsNj5upqjMlfxQA0yfrncdKjw,52
+sqlite_utils_sqlite_url-0.1.0a8.dist-info/top_level.txt,sha256=QWDQv-iAhRydh0st_oXJqhFPgZqarsLC4lsvRjRlZoA,24
+sqlite_utils_sqlite_url-0.1.0a8.dist-info/RECORD,,
```

