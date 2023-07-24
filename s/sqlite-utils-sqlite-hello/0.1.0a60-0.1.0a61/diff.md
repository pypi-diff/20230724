# Comparing `tmp/sqlite_utils_sqlite_hello-0.1.0a60-py3-none-any.whl.zip` & `tmp/sqlite_utils_sqlite_hello-0.1.0a61-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2244 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-24 00:58 sqlite_utils_sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:58 sqlite_utils_sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      540 b- defN 23-Jul-24 01:00 sqlite_utils_sqlite_hello-0.1.0a60.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 01:00 sqlite_utils_sqlite_hello-0.1.0a60.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       56 b- defN 23-Jul-24 01:00 sqlite_utils_sqlite_hello-0.1.0a60.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jul-24 01:00 sqlite_utils_sqlite_hello-0.1.0a60.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      681 b- defN 23-Jul-24 01:00 sqlite_utils_sqlite_hello-0.1.0a60.dist-info/RECORD
-7 files, 1764 bytes uncompressed, 998 bytes compressed:  43.4%
+Zip file size: 2234 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      276 b- defN 23-Jul-24 01:14 sqlite_utils_sqlite_hello/__init__.py
+-rw-r--r--  2.0 unx       80 b- defN 23-Jul-24 01:14 sqlite_utils_sqlite_hello/version.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      681 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/RECORD
+7 files, 1735 bytes uncompressed, 988 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sqlite_utils_sqlite_hello/__init__.py
 Comment: 
 
 Filename: sqlite_utils_sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a60.dist-info/METADATA
+Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a60.dist-info/WHEEL
+Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a60.dist-info/entry_points.txt
+Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a60.dist-info/top_level.txt
+Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a60.dist-info/RECORD
+Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_utils_sqlite_hello/__init__.py

 * *Ordering differences only*

```diff
@@ -1,11 +1,11 @@
-from sqlite_utils import hookimpl
-import sqlite_hello
-
-from sqlite_utils_sqlite_hello.version import __version_info__, __version__
-
-
-@hookimpl
-def prepare_connection(conn):
-    conn.enable_load_extension(True)
-    sqlite_hello.load(conn)
-    conn.enable_load_extension(False)
+from sqlite_utils import hookimpl
+import sqlite_hello
+
+from sqlite_utils_sqlite_hello.version import __version_info__, __version__
+
+
+@hookimpl
+def prepare_connection(conn):
+    conn.enable_load_extension(True)
+    sqlite_hello.load(conn)
+    conn.enable_load_extension(False)
```

## sqlite_utils_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.60"
-__version_info__ = tuple(__version__.split("."))
+__version__ = "0.1.0-alpha.61"
+__version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_utils_sqlite_hello-0.1.0a60.dist-info/METADATA` & `sqlite_utils_sqlite_hello-0.1.0a61.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: sqlite-utils-sqlite-hello
-Version: 0.1.0a60
-Summary: TODO
-Author: Alex Garcia
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/asg017/sqlite-hello
-Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
-Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
-Description-Content-Type: text/markdown
-Requires-Dist: sqlite-utils
-Requires-Dist: sqlite-hello
-
-# `sqlite-utils-sqlite-hello`
-
-A `sqlite-utils` plugin that registers the `sqlite-hello` extension.
+Metadata-Version: 2.1
+Name: sqlite-utils-sqlite-hello
+Version: 0.1.0a61
+Summary: TODO
+Author: Alex Garcia
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/asg017/sqlite-hello
+Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
+Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
+Description-Content-Type: text/markdown
+Requires-Dist: sqlite-utils
+Requires-Dist: sqlite-hello
+
+# `sqlite-utils-sqlite-hello`
+
+A `sqlite-utils` plugin that registers the `sqlite-hello` extension.
```

## Comparing `sqlite_utils_sqlite_hello-0.1.0a60.dist-info/RECORD` & `sqlite_utils_sqlite_hello-0.1.0a61.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-sqlite_utils_sqlite_hello/__init__.py,sha256=zoA1iTPrfoKOJRViB3aMEgtlGDQjUefmBEiPLE55Tes,287
-sqlite_utils_sqlite_hello/version.py,sha256=HlUiuzrv6zTP1AdX8bGiIbzFdycLI__qMH7FaxjqjAA,82
-sqlite_utils_sqlite_hello-0.1.0a60.dist-info/METADATA,sha256=LvsYbNXCDDTuabTaslWg2-30c4yn0t1XqhugZ_X9R30,540
-sqlite_utils_sqlite_hello-0.1.0a60.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-sqlite_utils_sqlite_hello-0.1.0a60.dist-info/entry_points.txt,sha256=GkeiI1YN1zuw1rIf-3BWSz_aKo03ttq1AAbPMv7Z5Wc,56
-sqlite_utils_sqlite_hello-0.1.0a60.dist-info/top_level.txt,sha256=RDXX67SyuHEZi7qGbD-6OKES0y-shx1CMoviTs_KLjM,26
-sqlite_utils_sqlite_hello-0.1.0a60.dist-info/RECORD,,
+sqlite_utils_sqlite_hello/__init__.py,sha256=1kBGZZAQRzS0XkdUqDVFeze5gh1w8HkN_Sdc6Q6GNMg,276
+sqlite_utils_sqlite_hello/version.py,sha256=GUVYGCmBwrxEaVh-nxq-MZfYW9gEDDfShgRKT9RRMi8,80
+sqlite_utils_sqlite_hello-0.1.0a61.dist-info/METADATA,sha256=KI55MRaIKGpHaq0G5j7fa8NKh6NVM9xDrfjtC3xgatE,524
+sqlite_utils_sqlite_hello-0.1.0a61.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+sqlite_utils_sqlite_hello-0.1.0a61.dist-info/entry_points.txt,sha256=GkeiI1YN1zuw1rIf-3BWSz_aKo03ttq1AAbPMv7Z5Wc,56
+sqlite_utils_sqlite_hello-0.1.0a61.dist-info/top_level.txt,sha256=RDXX67SyuHEZi7qGbD-6OKES0y-shx1CMoviTs_KLjM,26
+sqlite_utils_sqlite_hello-0.1.0a61.dist-info/RECORD,,
```

