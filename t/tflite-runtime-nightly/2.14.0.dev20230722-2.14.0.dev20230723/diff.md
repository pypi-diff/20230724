# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230722-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230723-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2407870 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Jul-23 05:01 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6846160 b- defN 23-Jul-23 05:03 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Jul-23 05:01 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Jul-23 05:01 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Jul-23 05:01 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1441 b- defN 23-Jul-23 05:03 tflite_runtime_nightly-2.14.0.dev20230722.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-Jul-23 05:03 tflite_runtime_nightly-2.14.0.dev20230722.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jul-23 05:03 tflite_runtime_nightly-2.14.0.dev20230722.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Jul-23 05:03 tflite_runtime_nightly-2.14.0.dev20230722.dist-info/RECORD
-9 files, 6891050 bytes uncompressed, 2406324 bytes compressed:  65.1%
+Zip file size: 2407871 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-24 05:06 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6846160 b- defN 23-Jul-24 05:08 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Jul-24 05:06 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Jul-24 05:06 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Jul-24 05:06 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1441 b- defN 23-Jul-24 05:08 tflite_runtime_nightly-2.14.0.dev20230723.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-Jul-24 05:08 tflite_runtime_nightly-2.14.0.dev20230723.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jul-24 05:08 tflite_runtime_nightly-2.14.0.dev20230723.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Jul-24 05:08 tflite_runtime_nightly-2.14.0.dev20230723.dist-info/RECORD
+9 files, 6891050 bytes uncompressed, 2406325 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230722.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230723.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230722.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230723.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230722.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230723.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230722.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230723.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230722'
-__git_version__ = '0.6.0-151025-g5430e5e238f'
+__version__ = '2.14.0dev20230723'
+__git_version__ = '0.6.0-151031-g7ce32a1a15c'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230722.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230723.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230722
+Version: 2.14.0.dev20230723
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230722.dist-info/RECORD` & `tflite_runtime_nightly-2.14.0.dev20230723.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=WKbyEVAK3Em3Q-Kaf89ocDW0VOgsk--84kmG8dI2m4w,80
+tflite_runtime/__init__.py,sha256=HiTul7RKf3iHzmhH3N9F2hp2SAU0HSK-3q6XJce0Dis,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=9Rz8CXD9ySUResZerUXOAICHPVIpwsevs3hHzXHWeKc,6846160
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.14.0.dev20230722.dist-info/METADATA,sha256=HYKYz1y4cj4dd_bgta_MJxKqCwQPlRB3eD3eGavsxIw,1441
-tflite_runtime_nightly-2.14.0.dev20230722.dist-info/WHEEL,sha256=bz3LNIts_Fx6FT4flbAhYt-b-go4FVoCtKM4eoP3Y9A,111
-tflite_runtime_nightly-2.14.0.dev20230722.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.14.0.dev20230722.dist-info/RECORD,,
+tflite_runtime_nightly-2.14.0.dev20230723.dist-info/METADATA,sha256=pmZrFNiXhkSXaIuFSZUH8i94WbVyDUSOIW4Ua7g0Z5w,1441
+tflite_runtime_nightly-2.14.0.dev20230723.dist-info/WHEEL,sha256=bz3LNIts_Fx6FT4flbAhYt-b-go4FVoCtKM4eoP3Y9A,111
+tflite_runtime_nightly-2.14.0.dev20230723.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.14.0.dev20230723.dist-info/RECORD,,
```

