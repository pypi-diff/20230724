# Comparing `tmp/datasette_sqlite_hello-0.1.0a55-py3-none-any.whl.zip` & `tmp/datasette_sqlite_hello-0.1.0a56-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2219 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-23 19:42 datasette_sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-23 19:42 datasette_sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-23 19:43 datasette_sqlite_hello-0.1.0a55.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-23 19:43 datasette_sqlite_hello-0.1.0a55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-23 19:43 datasette_sqlite_hello-0.1.0a55.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-23 19:43 datasette_sqlite_hello-0.1.0a55.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      660 b- defN 23-Jul-23 19:43 datasette_sqlite_hello-0.1.0a55.dist-info/RECORD
-7 files, 1772 bytes uncompressed, 1015 bytes compressed:  42.7%
+Zip file size: 2220 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-24 00:28 datasette_sqlite_hello/__init__.py
+-rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:28 datasette_sqlite_hello/version.py
+-rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-24 00:29 datasette_sqlite_hello-0.1.0a56.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:29 datasette_sqlite_hello-0.1.0a56.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-24 00:29 datasette_sqlite_hello-0.1.0a56.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 00:29 datasette_sqlite_hello-0.1.0a56.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      660 b- defN 23-Jul-24 00:29 datasette_sqlite_hello-0.1.0a56.dist-info/RECORD
+7 files, 1772 bytes uncompressed, 1016 bytes compressed:  42.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_hello/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_hello/version.py
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a55.dist-info/METADATA
+Filename: datasette_sqlite_hello-0.1.0a56.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a55.dist-info/WHEEL
+Filename: datasette_sqlite_hello-0.1.0a56.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a55.dist-info/entry_points.txt
+Filename: datasette_sqlite_hello-0.1.0a56.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a55.dist-info/top_level.txt
+Filename: datasette_sqlite_hello-0.1.0a56.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a55.dist-info/RECORD
+Filename: datasette_sqlite_hello-0.1.0a56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.55"
+__version__ = "0.1.0-alpha.56"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_hello-0.1.0a55.dist-info/METADATA` & `datasette_sqlite_hello-0.1.0a56.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-hello
-Version: 0.1.0a55
+Version: 0.1.0a56
 Home-page: https://github.com/asg017/sqlite-hello
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Requires-Python: >=3.6
```

## Comparing `datasette_sqlite_hello-0.1.0a55.dist-info/RECORD` & `datasette_sqlite_hello-0.1.0a56.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_hello/__init__.py,sha256=_bTDo2EMxavW_7jeQuin3Zjfcbjf_EWPBejF3967Zlw,279
-datasette_sqlite_hello/version.py,sha256=D1ohCmf7mGH5dOtHOjABGeSG_fY-JdpjpeCo734mcEw,82
-datasette_sqlite_hello-0.1.0a55.dist-info/METADATA,sha256=8u2Dcejaquns8lPqVJESonzqJL7oo8tGWSTvOBaSKtE,586
-datasette_sqlite_hello-0.1.0a55.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-datasette_sqlite_hello-0.1.0a55.dist-info/entry_points.txt,sha256=X0FnrOoDf3sGgQlWdM3s86QQSGuAZRKfOVfLJcXocpI,50
-datasette_sqlite_hello-0.1.0a55.dist-info/top_level.txt,sha256=klX1wE-1onKhiIgleurv_OT4mMGfe2GmHvNwpSMuYic,23
-datasette_sqlite_hello-0.1.0a55.dist-info/RECORD,,
+datasette_sqlite_hello/version.py,sha256=Uwv8aq5HcgAJrdh8JNdLXTtBEkUC32FyRn3uwtczObQ,82
+datasette_sqlite_hello-0.1.0a56.dist-info/METADATA,sha256=KHiDmmTSANdHSsT562uF8dScufhqcY-ndEc4jCtyhMM,586
+datasette_sqlite_hello-0.1.0a56.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+datasette_sqlite_hello-0.1.0a56.dist-info/entry_points.txt,sha256=X0FnrOoDf3sGgQlWdM3s86QQSGuAZRKfOVfLJcXocpI,50
+datasette_sqlite_hello-0.1.0a56.dist-info/top_level.txt,sha256=klX1wE-1onKhiIgleurv_OT4mMGfe2GmHvNwpSMuYic,23
+datasette_sqlite_hello-0.1.0a56.dist-info/RECORD,,
```

