# Comparing `tmp/sqlite_utils_sqlite_hello-0.1.0a57-py3-none-any.whl.zip` & `tmp/sqlite_utils_sqlite_hello-0.1.0a58-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2252 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      286 b- defN 23-Jul-24 00:31 sqlite_utils_sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:31 sqlite_utils_sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      540 b- defN 23-Jul-24 00:32 sqlite_utils_sqlite_hello-0.1.0a57.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:32 sqlite_utils_sqlite_hello-0.1.0a57.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       56 b- defN 23-Jul-24 00:32 sqlite_utils_sqlite_hello-0.1.0a57.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jul-24 00:32 sqlite_utils_sqlite_hello-0.1.0a57.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      681 b- defN 23-Jul-24 00:32 sqlite_utils_sqlite_hello-0.1.0a57.dist-info/RECORD
-7 files, 1763 bytes uncompressed, 1006 bytes compressed:  42.9%
+Zip file size: 2246 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-24 00:38 sqlite_utils_sqlite_hello/__init__.py
+-rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:38 sqlite_utils_sqlite_hello/version.py
+-rw-rw-rw-  2.0 fat      540 b- defN 23-Jul-24 00:39 sqlite_utils_sqlite_hello-0.1.0a58.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:39 sqlite_utils_sqlite_hello-0.1.0a58.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-Jul-24 00:39 sqlite_utils_sqlite_hello-0.1.0a58.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Jul-24 00:39 sqlite_utils_sqlite_hello-0.1.0a58.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      681 b- defN 23-Jul-24 00:39 sqlite_utils_sqlite_hello-0.1.0a58.dist-info/RECORD
+7 files, 1764 bytes uncompressed, 1000 bytes compressed:  43.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sqlite_utils_sqlite_hello/__init__.py
 Comment: 
 
 Filename: sqlite_utils_sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a57.dist-info/METADATA
+Filename: sqlite_utils_sqlite_hello-0.1.0a58.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a57.dist-info/WHEEL
+Filename: sqlite_utils_sqlite_hello-0.1.0a58.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a57.dist-info/entry_points.txt
+Filename: sqlite_utils_sqlite_hello-0.1.0a58.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a57.dist-info/top_level.txt
+Filename: sqlite_utils_sqlite_hello-0.1.0a58.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a57.dist-info/RECORD
+Filename: sqlite_utils_sqlite_hello-0.1.0a58.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_utils_sqlite_hello/__init__.py

```diff
@@ -1,11 +1,11 @@
 from sqlite_utils import hookimpl
 import sqlite_hello
 
-from sqite_utils_sqlite_hello.version import __version_info__, __version__
+from sqlite_utils_sqlite_hello.version import __version_info__, __version__
 
 
 @hookimpl
 def prepare_connection(conn):
     conn.enable_load_extension(True)
     sqlite_hello.load(conn)
     conn.enable_load_extension(False)
```

## sqlite_utils_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.57"
+__version__ = "0.1.0-alpha.58"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_utils_sqlite_hello-0.1.0a57.dist-info/METADATA` & `sqlite_utils_sqlite_hello-0.1.0a58.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-sqlite-hello
-Version: 0.1.0a57
+Version: 0.1.0a58
 Summary: TODO
 Author: Alex Garcia
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asg017/sqlite-hello
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Description-Content-Type: text/markdown
```

