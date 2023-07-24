# Comparing `tmp/datasette_sqlite_vss-0.1.1a9-py3-none-any.whl.zip` & `tmp/datasette_sqlite_vss-0.1.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2125 bytes, number of entries: 7
--rw-r--r--  2.0 unx      190 b- defN 23-May-23 18:38 datasette_sqlite_vss/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-May-28 18:24 datasette_sqlite_vss/version.py
--rw-r--r--  2.0 unx      557 b- defN 23-May-28 18:28 datasette_sqlite_vss-0.1.1a9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-28 18:28 datasette_sqlite_vss-0.1.1a9.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-May-28 18:28 datasette_sqlite_vss-0.1.1a9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-28 18:28 datasette_sqlite_vss-0.1.1a9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 23-May-28 18:28 datasette_sqlite_vss-0.1.1a9.dist-info/RECORD
-7 files, 1626 bytes uncompressed, 959 bytes compressed:  41.0%
+Zip file size: 2124 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      190 b- defN 23-May-30 17:56 datasette_sqlite_vss/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jul-24 20:19 datasette_sqlite_vss/version.py
+-rw-r--r--  2.0 unx      557 b- defN 23-Jul-24 20:28 datasette_sqlite_vss-0.1.2a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 20:28 datasette_sqlite_vss-0.1.2a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-24 20:28 datasette_sqlite_vss-0.1.2a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-24 20:28 datasette_sqlite_vss-0.1.2a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      641 b- defN 23-Jul-24 20:28 datasette_sqlite_vss-0.1.2a1.dist-info/RECORD
+7 files, 1626 bytes uncompressed, 958 bytes compressed:  41.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_vss/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_vss/version.py
 Comment: 
 
-Filename: datasette_sqlite_vss-0.1.1a9.dist-info/METADATA
+Filename: datasette_sqlite_vss-0.1.2a1.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_vss-0.1.1a9.dist-info/WHEEL
+Filename: datasette_sqlite_vss-0.1.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_vss-0.1.1a9.dist-info/entry_points.txt
+Filename: datasette_sqlite_vss-0.1.2a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_vss-0.1.1a9.dist-info/top_level.txt
+Filename: datasette_sqlite_vss-0.1.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_vss-0.1.1a9.dist-info/RECORD
+Filename: datasette_sqlite_vss-0.1.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_vss/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.1-alpha.9"
+__version__ = "0.1.2-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_vss-0.1.1a9.dist-info/METADATA` & `datasette_sqlite_vss-0.1.2a1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-vss
-Version: 0.1.1a9
+Version: 0.1.2a1
 Home-page: https://github.com/asg017/sqlite-vss
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-vss/issues
 Project-URL: CI, https://github.com/asg017/sqlite-vss/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-vss/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_vss-0.1.1a9.dist-info/RECORD` & `datasette_sqlite_vss-0.1.2a1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_vss/__init__.py,sha256=1LCY-tIpHYiF1CGp5tVBgnPCn78QmwrvJqYyXm9l6Lg,190
-datasette_sqlite_vss/version.py,sha256=IUnWpzE4hq4KWYTwXnfdMIV8srBC1nx5XDnY7ujW5N8,79
-datasette_sqlite_vss-0.1.1a9.dist-info/METADATA,sha256=v5u1RABiJeajU0lGqnD3HLL81rrGmCSX9d1y1VEAT4A,557
-datasette_sqlite_vss-0.1.1a9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_vss-0.1.1a9.dist-info/entry_points.txt,sha256=g6SBQV6Ze7DSQV75d0uxi0GSY9DKaGFreDJOoEHFU9o,46
-datasette_sqlite_vss-0.1.1a9.dist-info/top_level.txt,sha256=8_4ggvGdXsDCGTgnJVyL91drVfMloM7dakkdf2EPRcw,21
-datasette_sqlite_vss-0.1.1a9.dist-info/RECORD,,
+datasette_sqlite_vss/version.py,sha256=LIFb65E0T0yHeQVGZcN4wSLz1eEKKtCai-0Jh74gqQQ,79
+datasette_sqlite_vss-0.1.2a1.dist-info/METADATA,sha256=fAcfSciWfpuwFm7JzysMsRwHCH5uSasePRL4B9RybWo,557
+datasette_sqlite_vss-0.1.2a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_vss-0.1.2a1.dist-info/entry_points.txt,sha256=g6SBQV6Ze7DSQV75d0uxi0GSY9DKaGFreDJOoEHFU9o,46
+datasette_sqlite_vss-0.1.2a1.dist-info/top_level.txt,sha256=8_4ggvGdXsDCGTgnJVyL91drVfMloM7dakkdf2EPRcw,21
+datasette_sqlite_vss-0.1.2a1.dist-info/RECORD,,
```

