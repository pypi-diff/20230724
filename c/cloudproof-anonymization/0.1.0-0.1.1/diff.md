# Comparing `tmp/cloudproof_anonymization-0.1.0-cp37-abi3-win_amd64.whl.zip` & `tmp/cloudproof_anonymization-0.1.1-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 668821 bytes, number of entries: 7
--rw-r--r--  4.6 unx     3436 b- defN 23-Jun-02 13:11 cloudproof_anonymization-0.1.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jun-02 13:11 cloudproof_anonymization-0.1.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     9621 b- defN 23-Jun-02 13:11 cloudproof_anonymization/__init__.pyi
--rw-r--r--  4.6 unx       27 b- defN 23-Jun-02 13:11 cloudproof_anonymization/py.typed
--rw-r--r--  4.6 unx      204 b- defN 23-Jun-02 13:11 cloudproof_anonymization/__init__.py
--rwxr-xr-x  4.6 unx  1596928 b- defN 23-Jun-02 13:11 cloudproof_anonymization/cloudproof_anonymization.pyd
--rw-r--r--  4.6 unx      644 b- defN 23-Jun-02 13:11 cloudproof_anonymization-0.1.0.dist-info/RECORD
-7 files, 1610954 bytes uncompressed, 667665 bytes compressed:  58.6%
+Zip file size: 782700 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     3507 b- defN 23-Jul-24 09:26 cloudproof_anonymization-0.1.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-24 09:26 cloudproof_anonymization-0.1.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx    32275 b- defN 23-Jul-24 09:26 cloudproof_anonymization-0.1.1.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     9621 b- defN 23-Jul-24 09:26 cloudproof_anonymization/__init__.pyi
+-rw-r--r--  4.6 unx      204 b- defN 23-Jul-24 09:26 cloudproof_anonymization/__init__.py
+-rw-r--r--  4.6 unx       27 b- defN 23-Jul-24 09:26 cloudproof_anonymization/py.typed
+-rwxr-xr-x  4.6 unx  1840640 b- defN 23-Jul-24 09:26 cloudproof_anonymization/cloudproof_anonymization.pyd
+-rw-r--r--  4.6 unx      767 b- defN 23-Jul-24 09:26 cloudproof_anonymization-0.1.1.dist-info/RECORD
+8 files, 1887135 bytes uncompressed, 781338 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
-Filename: cloudproof_anonymization-0.1.0.dist-info/METADATA
+Filename: cloudproof_anonymization-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: cloudproof_anonymization-0.1.0.dist-info/WHEEL
+Filename: cloudproof_anonymization-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: cloudproof_anonymization/__init__.pyi
+Filename: cloudproof_anonymization-0.1.1.dist-info/license_files/LICENSE.md
 Comment: 
 
-Filename: cloudproof_anonymization/py.typed
+Filename: cloudproof_anonymization/__init__.pyi
 Comment: 
 
 Filename: cloudproof_anonymization/__init__.py
 Comment: 
 
+Filename: cloudproof_anonymization/py.typed
+Comment: 
+
 Filename: cloudproof_anonymization/cloudproof_anonymization.pyd
 Comment: 
 
-Filename: cloudproof_anonymization-0.1.0.dist-info/RECORD
+Filename: cloudproof_anonymization-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudproof_anonymization-0.1.0.dist-info/METADATA` & `cloudproof_anonymization-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: cloudproof_anonymization
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: cffi
+License-File: LICENSE.md
 Summary: Cosmian Cloudproof Anonymization library
 Author: Hugo Rosenkranz-costa<hugo.rosenkranz@cosmian.com>
 Author-email: Hugo Rosenkranz-costa<hugo.rosenkranz@cosmian.com>
-License: MIT/Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/cosmian/cloudproof_rust/
 
 # Data Anonymization
 
 `Data anonymization` is the process of transforming data in such a way that it can no longer be used to identify individuals without the use of additional information. This is often done to protect the privacy of individuals whose data is being collected or processed.
 
 Anonymization techniques can include removing identifying information such as names and addresses, replacing identifying information with pseudonyms, and aggregating data so that individual data points cannot be distinguished. It's important to note that while anonymization can reduce the risk of re-identification, it is not foolproof and must be used in conjunction with other security measures to fully protect personal data.
```

## Comparing `cloudproof_anonymization-0.1.0.dist-info/RECORD` & `cloudproof_anonymization-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-cloudproof_anonymization-0.1.0.dist-info/METADATA,sha256=1ce7k-tbtASfqi65DQaMTX-PKgxUPKJD9u0sZy9Yknc,3436
-cloudproof_anonymization-0.1.0.dist-info/WHEEL,sha256=lO8DhDEyNhXrOG0fb7degSdk7XyHtCDkr6WQEBfaH0A,94
+cloudproof_anonymization-0.1.1.dist-info/METADATA,sha256=C5dCXB7psglO7SHEO-IU29UU_XzR1Q_5ydsdT-UXH-E,3507
+cloudproof_anonymization-0.1.1.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
+cloudproof_anonymization-0.1.1.dist-info/license_files/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
 cloudproof_anonymization/__init__.pyi,sha256=Uo0woijQVXDuP7cA039rvkUKk1CYwEnQFwuDzRCNPG8,9621
-cloudproof_anonymization/py.typed,sha256=bWew9mHgMy8LqMu7RuqQXFXLBxh2CRx0dUbSx-3wE48,27
 cloudproof_anonymization/__init__.py,sha256=jMrSzNS4T-Ksav70PfzCjFUctNVGdzL4RvEBCpejLLs,204
-cloudproof_anonymization/cloudproof_anonymization.pyd,sha256=jPdD1Kxbez3FlXJogfMEGoGzcvNU-caytUsgHFhV9dU,1596928
-cloudproof_anonymization-0.1.0.dist-info/RECORD,,
+cloudproof_anonymization/py.typed,sha256=bWew9mHgMy8LqMu7RuqQXFXLBxh2CRx0dUbSx-3wE48,27
+cloudproof_anonymization/cloudproof_anonymization.pyd,sha256=NMviqlBKJiQTnC1ENa8Xpsdc5IYIJu6BZ2KK01sCrjg,1840640
+cloudproof_anonymization-0.1.1.dist-info/RECORD,,
```

