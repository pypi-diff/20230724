# Comparing `tmp/datasette_sqlite_hello-0.1.0a59-py3-none-any.whl.zip` & `tmp/datasette_sqlite_hello-0.1.0a60-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2219 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-24 00:48 datasette_sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:48 datasette_sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      660 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/RECORD
-7 files, 1772 bytes uncompressed, 1015 bytes compressed:  42.7%
+Zip file size: 2220 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-24 00:58 datasette_sqlite_hello/__init__.py
+-rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:58 datasette_sqlite_hello/version.py
+-rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      660 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/RECORD
+7 files, 1772 bytes uncompressed, 1016 bytes compressed:  42.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_hello/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_hello/version.py
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a59.dist-info/METADATA
+Filename: datasette_sqlite_hello-0.1.0a60.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a59.dist-info/WHEEL
+Filename: datasette_sqlite_hello-0.1.0a60.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a59.dist-info/entry_points.txt
+Filename: datasette_sqlite_hello-0.1.0a60.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a59.dist-info/top_level.txt
+Filename: datasette_sqlite_hello-0.1.0a60.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a59.dist-info/RECORD
+Filename: datasette_sqlite_hello-0.1.0a60.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.59"
+__version__ = "0.1.0-alpha.60"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_hello-0.1.0a59.dist-info/METADATA` & `datasette_sqlite_hello-0.1.0a60.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-hello
-Version: 0.1.0a59
+Version: 0.1.0a60
 Home-page: https://github.com/asg017/sqlite-hello
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Requires-Python: >=3.6
```

