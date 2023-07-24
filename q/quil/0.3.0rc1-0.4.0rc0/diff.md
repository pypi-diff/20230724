# Comparing `tmp/quil-0.3.0rc1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/quil-0.4.0rc0-cp310-cp310-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2074262 bytes, number of entries: 12
--rw-r--r--  4.6 unx     1048 b- defN 23-Jul-12 20:26 quil-0.3.0rc1.dist-info/METADATA
--rw-r--r--  4.6 unx      128 b- defN 23-Jul-12 20:26 quil-0.3.0rc1.dist-info/WHEEL
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-12 20:26 quil/py.typed
--rw-r--r--  4.6 unx     7308 b- defN 23-Jul-12 20:26 quil/program/__init__.pyi
--rw-r--r--  4.6 unx     6834 b- defN 23-Jul-12 20:26 quil/expression/__init__.pyi
--rw-r--r--  4.6 unx      439 b- defN 23-Jul-12 20:26 quil/validation/identifier.pyi
--rw-r--r--  4.6 unx       39 b- defN 23-Jul-12 20:26 quil/validation/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-12 20:26 quil/__init__.pyi
--rw-r--r--  4.6 unx       20 b- defN 23-Jul-12 20:26 quil/__init__.py
--rw-r--r--  4.6 unx    43714 b- defN 23-Jul-12 20:26 quil/instructions/__init__.pyi
--rwxr-xr-x  4.6 unx  6586176 b- defN 23-Jul-12 20:26 quil/quil.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      940 b- defN 23-Jul-12 20:26 quil-0.3.0rc1.dist-info/RECORD
-12 files, 6646646 bytes uncompressed, 2072692 bytes compressed:  68.8%
+Zip file size: 3399650 bytes, number of entries: 12
+-rw-r--r--  4.6 unx     1048 b- defN 23-Jul-24 19:13 quil-0.4.0rc0.dist-info/METADATA
+-rw-r--r--  4.6 unx      147 b- defN 23-Jul-24 19:13 quil-0.4.0rc0.dist-info/WHEEL
+-rw-r--r--  4.6 unx    43714 b- defN 23-Jul-24 19:13 quil/instructions/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-24 19:13 quil/__init__.pyi
+-rw-r--r--  4.6 unx       20 b- defN 23-Jul-24 19:13 quil/__init__.py
+-rw-r--r--  4.6 unx     7308 b- defN 23-Jul-24 19:13 quil/program/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-24 19:13 quil/py.typed
+-rw-r--r--  4.6 unx     6834 b- defN 23-Jul-24 19:13 quil/expression/__init__.pyi
+-rw-r--r--  4.6 unx       39 b- defN 23-Jul-24 19:13 quil/validation/__init__.pyi
+-rw-r--r--  4.6 unx      439 b- defN 23-Jul-24 19:13 quil/validation/identifier.pyi
+-rwxr-xr-x  4.6 unx 10181143 b- defN 23-Jul-24 19:13 quil/quil.cpython-310-darwin.so
+-rw-r--r--  4.6 unx      932 b- defN 23-Jul-24 19:13 quil-0.4.0rc0.dist-info/RECORD
+12 files, 10241624 bytes uncompressed, 3398098 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,37 +1,37 @@
-Filename: quil-0.3.0rc1.dist-info/METADATA
+Filename: quil-0.4.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: quil-0.3.0rc1.dist-info/WHEEL
+Filename: quil-0.4.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: quil/py.typed
+Filename: quil/instructions/__init__.pyi
 Comment: 
 
-Filename: quil/program/__init__.pyi
+Filename: quil/__init__.pyi
 Comment: 
 
-Filename: quil/expression/__init__.pyi
+Filename: quil/__init__.py
 Comment: 
 
-Filename: quil/validation/identifier.pyi
+Filename: quil/program/__init__.pyi
 Comment: 
 
-Filename: quil/validation/__init__.pyi
+Filename: quil/py.typed
 Comment: 
 
-Filename: quil/__init__.pyi
+Filename: quil/expression/__init__.pyi
 Comment: 
 
-Filename: quil/__init__.py
+Filename: quil/validation/__init__.pyi
 Comment: 
 
-Filename: quil/instructions/__init__.pyi
+Filename: quil/validation/identifier.pyi
 Comment: 
 
-Filename: quil/quil.cpython-39-x86_64-linux-gnu.so
+Filename: quil/quil.cpython-310-darwin.so
 Comment: 
 
-Filename: quil-0.3.0rc1.dist-info/RECORD
+Filename: quil-0.4.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `quil-0.3.0rc1.dist-info/METADATA` & `quil-0.4.0rc0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quil
-Version: 0.3.0rc1
+Version: 0.4.0rc0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Summary: A Python package for building and parsing Quil programs.
```

