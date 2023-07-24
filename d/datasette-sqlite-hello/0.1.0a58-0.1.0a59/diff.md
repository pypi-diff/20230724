# Comparing `tmp/datasette_sqlite_hello-0.1.0a58-py3-none-any.whl.zip` & `tmp/datasette_sqlite_hello-0.1.0a59-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2219 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-24 00:38 datasette_sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:38 datasette_sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      660 b- defN 23-Jul-24 00:39 datasette_sqlite_hello-0.1.0a58.dist-info/RECORD
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-24 00:48 datasette_sqlite_hello/__init__.py
+-rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:48 datasette_sqlite_hello/version.py
+-rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      660 b- defN 23-Jul-24 00:49 datasette_sqlite_hello-0.1.0a59.dist-info/RECORD
 7 files, 1772 bytes uncompressed, 1015 bytes compressed:  42.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_hello/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_hello/version.py
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a58.dist-info/METADATA
+Filename: datasette_sqlite_hello-0.1.0a59.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a58.dist-info/WHEEL
+Filename: datasette_sqlite_hello-0.1.0a59.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a58.dist-info/entry_points.txt
+Filename: datasette_sqlite_hello-0.1.0a59.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a58.dist-info/top_level.txt
+Filename: datasette_sqlite_hello-0.1.0a59.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a58.dist-info/RECORD
+Filename: datasette_sqlite_hello-0.1.0a59.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.58"
+__version__ = "0.1.0-alpha.59"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_hello-0.1.0a58.dist-info/METADATA` & `datasette_sqlite_hello-0.1.0a59.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-hello
-Version: 0.1.0a58
+Version: 0.1.0a59
 Home-page: https://github.com/asg017/sqlite-hello
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Requires-Python: >=3.6
```

## Comparing `datasette_sqlite_hello-0.1.0a58.dist-info/RECORD` & `datasette_sqlite_hello-0.1.0a59.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_hello/__init__.py,sha256=_bTDo2EMxavW_7jeQuin3Zjfcbjf_EWPBejF3967Zlw,279
-datasette_sqlite_hello/version.py,sha256=6IntCGtmBlcNg4ngDhckASIJjXoq9FCbqfAL0unH5Gg,82
-datasette_sqlite_hello-0.1.0a58.dist-info/METADATA,sha256=MSGDcC906PJnqyNIaHxUiGqiRIQBQiappfk_RU0jj_o,586
-datasette_sqlite_hello-0.1.0a58.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-datasette_sqlite_hello-0.1.0a58.dist-info/entry_points.txt,sha256=X0FnrOoDf3sGgQlWdM3s86QQSGuAZRKfOVfLJcXocpI,50
-datasette_sqlite_hello-0.1.0a58.dist-info/top_level.txt,sha256=klX1wE-1onKhiIgleurv_OT4mMGfe2GmHvNwpSMuYic,23
-datasette_sqlite_hello-0.1.0a58.dist-info/RECORD,,
+datasette_sqlite_hello/version.py,sha256=wF9CIDO6azTIM8rIAUwLJDbL3HpElKZ2AlW6q-0DMcI,82
+datasette_sqlite_hello-0.1.0a59.dist-info/METADATA,sha256=wQSCXc6Wc2j2TqXxxFXkxEXnKQ9_jn6LG54lwoE59Eg,586
+datasette_sqlite_hello-0.1.0a59.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+datasette_sqlite_hello-0.1.0a59.dist-info/entry_points.txt,sha256=X0FnrOoDf3sGgQlWdM3s86QQSGuAZRKfOVfLJcXocpI,50
+datasette_sqlite_hello-0.1.0a59.dist-info/top_level.txt,sha256=klX1wE-1onKhiIgleurv_OT4mMGfe2GmHvNwpSMuYic,23
+datasette_sqlite_hello-0.1.0a59.dist-info/RECORD,,
```

