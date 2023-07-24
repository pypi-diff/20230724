# Comparing `tmp/pyvalidata-0.1.2-py3-none-any.whl.zip` & `tmp/pyvalidata-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6976 bytes, number of entries: 7
--rw-r--r--  2.0 unx     9572 b- defN 23-Jul-23 23:26 pyvalidata/__init__.py
+Zip file size: 6978 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     9573 b- defN 23-Jul-24 08:17 pyvalidata/__init__.py
 -rw-r--r--  2.0 unx     3699 b- defN 23-Jul-23 21:49 pyvalidata/validators.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Jul-23 23:26 pyvalidata-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2096 b- defN 23-Jul-23 23:26 pyvalidata-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-23 23:26 pyvalidata-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-23 23:26 pyvalidata-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      561 b- defN 23-Jul-23 23:26 pyvalidata-0.1.2.dist-info/RECORD
-7 files, 17105 bytes uncompressed, 5982 bytes compressed:  65.0%
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jul-24 08:28 pyvalidata-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2096 b- defN 23-Jul-24 08:28 pyvalidata-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:28 pyvalidata-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-24 08:28 pyvalidata-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      561 b- defN 23-Jul-24 08:28 pyvalidata-0.1.3.dist-info/RECORD
+7 files, 17106 bytes uncompressed, 5984 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pyvalidata/__init__.py
 Comment: 
 
 Filename: pyvalidata/validators.py
 Comment: 
 
-Filename: pyvalidata-0.1.2.dist-info/LICENSE
+Filename: pyvalidata-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyvalidata-0.1.2.dist-info/METADATA
+Filename: pyvalidata-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pyvalidata-0.1.2.dist-info/WHEEL
+Filename: pyvalidata-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyvalidata-0.1.2.dist-info/top_level.txt
+Filename: pyvalidata-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyvalidata-0.1.2.dist-info/RECORD
+Filename: pyvalidata-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyvalidata/__init__.py

```diff
@@ -1,8 +1,8 @@
-from validators import *
+from .validators import *
 
 def pyvalidatahelp():
     """Prints the detailed documentation and usage examples for PyValidata."""
     help_text = """
     PyValidata - Python Data Validation Package
 
     PyValidata is a Python package designed for easy and comprehelnsive data validation. It provides a colection of functions to validate data types, ranges, string lengths, and more. Ensure the integrity and quality of your data with PyValidata, a reliable data guardian for Python developers.
```

## Comparing `pyvalidata-0.1.2.dist-info/LICENSE` & `pyvalidata-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyvalidata-0.1.2.dist-info/METADATA` & `pyvalidata-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalidata
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for data validation
 Home-page: https://github.com/EklavyaT/pyvalidata
 Author: Eklavya Tomar
 Author-email: eklavyaprogramming@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

