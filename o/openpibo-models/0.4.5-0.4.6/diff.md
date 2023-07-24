# Comparing `tmp/openpibo_models-0.4.5-py3-none-any.whl.zip` & `tmp/openpibo_models-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 476589 bytes, number of entries: 10
--rw-r--r--  2.0 unx      151 b- defN 23-Jan-30 21:20 openpibo_models/__init__.py
--rw-r--r--  2.0 unx   723640 b- defN 23-Jan-30 21:19 openpibo_models/models/KDL.ttf
--rw-r--r--  2.0 unx   341687 b- defN 23-Jan-30 21:17 openpibo_models/models/dialog.csv
--rw-r--r--  2.0 unx   341661 b- defN 23-Jan-30 21:17 openpibo_models/models/dialog1.csv
--rw-r--r--  2.0 unx    74794 b- defN 23-Jan-30 21:17 openpibo_models/models/motion_db.json
--rw-r--r--  2.0 unx      199 b- defN 23-Jan-30 21:17 openpibo_models/models/sample_db.json
--rw-r--r--  2.0 unx      754 b- defN 23-Jan-30 21:21 openpibo_models-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-30 21:21 openpibo_models-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jan-30 21:21 openpibo_models-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      874 b- defN 23-Jan-30 21:21 openpibo_models-0.4.5.dist-info/RECORD
-10 files, 1483868 bytes uncompressed, 475091 bytes compressed:  68.0%
+Zip file size: 475698 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-24 08:21 openpibo_models/__init__.py
+-rw-r--r--  2.0 unx   723640 b- defN 23-Jul-24 07:47 openpibo_models/models/KDL.ttf
+-rw-r--r--  2.0 unx   341687 b- defN 23-Jul-24 07:47 openpibo_models/models/dialog.csv
+-rw-r--r--  2.0 unx   313743 b- defN 23-Jul-24 07:50 openpibo_models/models/dialog_en.csv
+-rw-r--r--  2.0 unx    74794 b- defN 23-Jul-24 07:47 openpibo_models/models/motion_db.json
+-rw-r--r--  2.0 unx      199 b- defN 23-Jul-24 07:47 openpibo_models/models/sample_db.json
+-rw-r--r--  2.0 unx      754 b- defN 23-Jul-24 08:22 openpibo_models-0.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:22 openpibo_models-0.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-24 08:22 openpibo_models-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      876 b- defN 23-Jul-24 08:22 openpibo_models-0.4.6.dist-info/RECORD
+10 files, 1455952 bytes uncompressed, 474196 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: openpibo_models/models/KDL.ttf
 Comment: 
 
 Filename: openpibo_models/models/dialog.csv
 Comment: 
 
-Filename: openpibo_models/models/dialog1.csv
+Filename: openpibo_models/models/dialog_en.csv
 Comment: 
 
 Filename: openpibo_models/models/motion_db.json
 Comment: 
 
 Filename: openpibo_models/models/sample_db.json
 Comment: 
 
-Filename: openpibo_models-0.4.5.dist-info/METADATA
+Filename: openpibo_models-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: openpibo_models-0.4.5.dist-info/WHEEL
+Filename: openpibo_models-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: openpibo_models-0.4.5.dist-info/top_level.txt
+Filename: openpibo_models-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: openpibo_models-0.4.5.dist-info/RECORD
+Filename: openpibo_models-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openpibo_models/__init__.py

```diff
@@ -1,6 +1,6 @@
 from pkg_resources import resource_filename
 
-__version__ = '0.4.5'
+__version__ = '0.4.6'
 
 def filepath(filename):
   return resource_filename(__name__, f'models/{filename}')
```

## Comparing `openpibo_models-0.4.5.dist-info/METADATA` & `openpibo_models-0.4.6.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpibo-models
-Version: 0.4.5
+Version: 0.4.6
 Summary: Models used by the openpibo-python package.
 Home-page: https://github.com/themakerrobot/openpibo_models
 Author: circulus
 Author-email: leeyunjai@circul.us
 License: UNKNOWN
 Keywords: openpibo
 Platform: UNKNOWN
```

