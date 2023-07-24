# Comparing `tmp/sqlite_utils_sqlite_ulid-0.2.1-py3-none-any.whl.zip` & `tmp/sqlite_utils_sqlite_ulid-0.2.1a19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2168 bytes, number of entries: 7
--rw-r--r--  2.0 unx      273 b- defN 23-Jul-24 06:07 sqlite_utils_sqlite_ulid/__init__.py
--rw-r--r--  2.0 unx       71 b- defN 23-Jul-24 06:07 sqlite_utils_sqlite_ulid/version.py
--rw-r--r--  2.0 unx      514 b- defN 23-Jul-24 06:08 sqlite_utils_sqlite_ulid-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 06:08 sqlite_utils_sqlite_ulid-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-Jul-24 06:08 sqlite_utils_sqlite_ulid-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-24 06:08 sqlite_utils_sqlite_ulid-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      659 b- defN 23-Jul-24 06:08 sqlite_utils_sqlite_ulid-0.2.1.dist-info/RECORD
-7 files, 1688 bytes uncompressed, 966 bytes compressed:  42.8%
+Zip file size: 2208 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      273 b- defN 23-Jul-24 04:42 sqlite_utils_sqlite_ulid/__init__.py
+-rw-r--r--  2.0 unx       80 b- defN 23-Jul-24 04:42 sqlite_utils_sqlite_ulid/version.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jul-24 04:42 sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 04:42 sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-Jul-24 04:42 sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-24 04:42 sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-24 04:42 sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/RECORD
+7 files, 1715 bytes uncompressed, 976 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sqlite_utils_sqlite_ulid/__init__.py
 Comment: 
 
 Filename: sqlite_utils_sqlite_ulid/version.py
 Comment: 
 
-Filename: sqlite_utils_sqlite_ulid-0.2.1.dist-info/METADATA
+Filename: sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_utils_sqlite_ulid-0.2.1.dist-info/WHEEL
+Filename: sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_utils_sqlite_ulid-0.2.1.dist-info/entry_points.txt
+Filename: sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_ulid-0.2.1.dist-info/top_level.txt
+Filename: sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_ulid-0.2.1.dist-info/RECORD
+Filename: sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_utils_sqlite_ulid/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.1"
+__version__ = "0.2.1-alpha.19"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_utils_sqlite_ulid-0.2.1.dist-info/METADATA` & `sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-sqlite-ulid
-Version: 0.2.1
+Version: 0.2.1a19
 Summary: TODO
 Author: Alex Garcia
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asg017/sqlite-ulid
 Project-URL: Changelog, https://github.com/asg017/sqlite-ulid/releases
 Project-URL: Issues, https://github.com/asg017/sqlite-ulid/issues
 Description-Content-Type: text/markdown
```

## Comparing `sqlite_utils_sqlite_ulid-0.2.1.dist-info/RECORD` & `sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sqlite_utils_sqlite_ulid/__init__.py,sha256=hT7C_-Tr5An0dNIMKdgUR3Eob6vNHCKkYMnX5fE0AXg,273
-sqlite_utils_sqlite_ulid/version.py,sha256=zzw85I4BZCxZg7xZswbOlQsELDeJjCwNYtkzgnJwqEc,71
-sqlite_utils_sqlite_ulid-0.2.1.dist-info/METADATA,sha256=x3KlMn-y0NOHQnpWr_0nwqXNdC3N_fX2Z_mj7FfxzVk,514
-sqlite_utils_sqlite_ulid-0.2.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-sqlite_utils_sqlite_ulid-0.2.1.dist-info/entry_points.txt,sha256=KYTNqZt1kjuyhslQr_340_inPQ8S7Ksyz69wXD2an5Y,54
-sqlite_utils_sqlite_ulid-0.2.1.dist-info/top_level.txt,sha256=ZmFFWb9QrmJo53fAY4PRdEDvwYa-AEF4XwfeCLGWHeo,25
-sqlite_utils_sqlite_ulid-0.2.1.dist-info/RECORD,,
+sqlite_utils_sqlite_ulid/version.py,sha256=3121XcPNSHyvcSSDURmwZbwNho3CBGy9euuwlEaMD9E,80
+sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/METADATA,sha256=F2R-wsI2YkUu59hsztg_ojhulfA1H_ckTu6FE9kBQ_E,517
+sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/entry_points.txt,sha256=KYTNqZt1kjuyhslQr_340_inPQ8S7Ksyz69wXD2an5Y,54
+sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/top_level.txt,sha256=ZmFFWb9QrmJo53fAY4PRdEDvwYa-AEF4XwfeCLGWHeo,25
+sqlite_utils_sqlite_ulid-0.2.1a19.dist-info/RECORD,,
```

