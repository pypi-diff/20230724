# Comparing `tmp/datasette_sqlite_hello-0.1.0a57-py3-none-any.whl.zip` & `tmp/datasette_sqlite_hello-0.1.0a58-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2221 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-24 00:31 datasette_sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:31 datasette_sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-24 00:32 datasette_sqlite_hello-0.1.0a57.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:32 datasette_sqlite_hello-0.1.0a57.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-24 00:32 datasette_sqlite_hello-0.1.0a57.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 00:32 datasette_sqlite_hello-0.1.0a57.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      660 b- defN 23-Jul-24 00:32 datasette_sqlite_hello-0.1.0a57.dist-info/RECORD
-7 files, 1772 bytes uncompressed, 1017 bytes compressed:  42.6%
+Zip file size: 2219 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-24 00:38 datasette_sqlite_hello/__init__.py
+-rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:38 datasette_sqlite_hello/version.py
+-rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      660 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/RECORD
+7 files, 1772 bytes uncompressed, 1015 bytes compressed:  42.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_hello/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_hello/version.py
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a57.dist-info/METADATA
+Filename: datasette_sqlite_hello-0.1.0a58.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a57.dist-info/WHEEL
+Filename: datasette_sqlite_hello-0.1.0a58.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a57.dist-info/entry_points.txt
+Filename: datasette_sqlite_hello-0.1.0a58.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a57.dist-info/top_level.txt
+Filename: datasette_sqlite_hello-0.1.0a58.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a57.dist-info/RECORD
+Filename: datasette_sqlite_hello-0.1.0a58.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.57"
+__version__ = "0.1.0-alpha.58"
 __version_info__ = tuple(__version__.split("."))
```

