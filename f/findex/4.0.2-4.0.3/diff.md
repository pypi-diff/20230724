# Comparing `tmp/findex-4.0.2-cp37-abi3-win_amd64.whl.zip` & `tmp/findex-4.0.3-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1932078 bytes, number of entries: 8
--rw-r--r--  4.6 unx      533 b- defN 23-Jul-17 11:22 findex-4.0.2.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-17 11:22 findex-4.0.2.dist-info/WHEEL
--rw-r--r--  4.6 unx    32275 b- defN 23-Jul-17 11:22 findex-4.0.2.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx     6630 b- defN 23-Jul-17 11:22 cloudproof_findex/__init__.pyi
--rw-r--r--  4.6 unx       27 b- defN 23-Jul-17 11:22 cloudproof_findex/py.typed
--rw-r--r--  4.6 unx      462 b- defN 23-Jul-17 11:22 cloudproof_findex/__init__.py
--rwxr-xr-x  4.6 unx  3817984 b- defN 23-Jul-17 11:22 cloudproof_findex/cloudproof_findex.pyd
--rw-r--r--  4.6 unx      659 b- defN 23-Jul-17 11:22 findex-4.0.2.dist-info/RECORD
-8 files, 3858664 bytes uncompressed, 1930930 bytes compressed:  50.0%
+Zip file size: 1934323 bytes, number of entries: 8
+-rw-r--r--  4.6 unx      533 b- defN 23-Jul-24 09:30 findex-4.0.3.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-24 09:30 findex-4.0.3.dist-info/WHEEL
+-rw-r--r--  4.6 unx    32275 b- defN 23-Jul-24 09:30 findex-4.0.3.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     6630 b- defN 23-Jul-24 09:30 cloudproof_findex/__init__.pyi
+-rw-r--r--  4.6 unx      462 b- defN 23-Jul-24 09:30 cloudproof_findex/__init__.py
+-rw-r--r--  4.6 unx       27 b- defN 23-Jul-24 09:30 cloudproof_findex/py.typed
+-rwxr-xr-x  4.6 unx  3827200 b- defN 23-Jul-24 09:30 cloudproof_findex/cloudproof_findex.pyd
+-rw-r--r--  4.6 unx      659 b- defN 23-Jul-24 09:30 findex-4.0.3.dist-info/RECORD
+8 files, 3867880 bytes uncompressed, 1933175 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: findex-4.0.2.dist-info/METADATA
+Filename: findex-4.0.3.dist-info/METADATA
 Comment: 
 
-Filename: findex-4.0.2.dist-info/WHEEL
+Filename: findex-4.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: findex-4.0.2.dist-info/license_files/LICENSE.md
+Filename: findex-4.0.3.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: cloudproof_findex/__init__.pyi
 Comment: 
 
-Filename: cloudproof_findex/py.typed
+Filename: cloudproof_findex/__init__.py
 Comment: 
 
-Filename: cloudproof_findex/__init__.py
+Filename: cloudproof_findex/py.typed
 Comment: 
 
 Filename: cloudproof_findex/cloudproof_findex.pyd
 Comment: 
 
-Filename: findex-4.0.2.dist-info/RECORD
+Filename: findex-4.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `findex-4.0.2.dist-info/METADATA` & `findex-4.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findex
-Version: 4.0.2
+Version: 4.0.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: cffi
 License-File: LICENSE.md
 Summary: Cosmian Findex Cloudproof library
 Author: Théophile Brézot<theophile.brezot@cosmian.com>
```

## Comparing `findex-4.0.2.dist-info/license_files/LICENSE.md` & `findex-4.0.3.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

## Comparing `findex-4.0.2.dist-info/RECORD` & `findex-4.0.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-findex-4.0.2.dist-info/METADATA,sha256=DrszezIS4geRaBKqWYjOmAMjGsYYmkoioxIyntez6t8,533
-findex-4.0.2.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
-findex-4.0.2.dist-info/license_files/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
+findex-4.0.3.dist-info/METADATA,sha256=8FqYgOVbtCAuyE48GI1p_9sWHL6O9UETED4AZFRKiTM,533
+findex-4.0.3.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
+findex-4.0.3.dist-info/license_files/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
 cloudproof_findex/__init__.pyi,sha256=s4cLBzc0_qzzX67jtRAOxuwD67t2Iwei8dsGVxDMlMw,6630
-cloudproof_findex/py.typed,sha256=bWew9mHgMy8LqMu7RuqQXFXLBxh2CRx0dUbSx-3wE48,27
 cloudproof_findex/__init__.py,sha256=woy5cZfk_uN-PjUlPNLnr-Hy3U2u3_6YJACHQWExrMc,462
-cloudproof_findex/cloudproof_findex.pyd,sha256=hrnFBpdpNhzJfd0_G1ohj4txHpxWswv57iqJ75VFtqU,3817984
-findex-4.0.2.dist-info/RECORD,,
+cloudproof_findex/py.typed,sha256=bWew9mHgMy8LqMu7RuqQXFXLBxh2CRx0dUbSx-3wE48,27
+cloudproof_findex/cloudproof_findex.pyd,sha256=e_sWV1VmPM-TTca5PlGHQ4xv_j_RaRar8ULr69eKzww,3827200
+findex-4.0.3.dist-info/RECORD,,
```

