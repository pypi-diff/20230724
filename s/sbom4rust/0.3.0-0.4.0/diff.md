# Comparing `tmp/sbom4rust-0.3.0-py2.py3-none-any.whl.zip` & `tmp/sbom4rust-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10686 bytes, number of entries: 10
+Zip file size: 10696 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-23 13:05 sbom4rust/__init__.py
 -rw-r--r--  2.0 unx     3963 b- defN 23-Jan-30 12:33 sbom4rust/cli.py
 -rw-r--r--  2.0 unx     5442 b- defN 23-Jan-30 12:33 sbom4rust/scanner.py
--rw-r--r--  2.0 unx      100 b- defN 23-Jan-30 12:32 sbom4rust/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jan-30 15:47 sbom4rust-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4730 b- defN 23-Jan-30 15:47 sbom4rust-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jan-30 15:47 sbom4rust-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Jan-30 15:47 sbom4rust-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jan-30 15:47 sbom4rust-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      796 b- defN 23-Jan-30 15:47 sbom4rust-0.3.0.dist-info/RECORD
-10 files, 26557 bytes uncompressed, 9328 bytes compressed:  64.9%
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 21:11 sbom4rust/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-24 18:09 sbom4rust-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4740 b- defN 23-Jul-24 18:09 sbom4rust-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 18:09 sbom4rust-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Jul-24 18:09 sbom4rust-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-24 18:09 sbom4rust-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      796 b- defN 23-Jul-24 18:09 sbom4rust-0.4.0.dist-info/RECORD
+10 files, 26567 bytes uncompressed, 9338 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: sbom4rust/scanner.py
 Comment: 
 
 Filename: sbom4rust/version.py
 Comment: 
 
-Filename: sbom4rust-0.3.0.dist-info/LICENSE
+Filename: sbom4rust-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: sbom4rust-0.3.0.dist-info/METADATA
+Filename: sbom4rust-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: sbom4rust-0.3.0.dist-info/WHEEL
+Filename: sbom4rust-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: sbom4rust-0.3.0.dist-info/entry_points.txt
+Filename: sbom4rust-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbom4rust-0.3.0.dist-info/top_level.txt
+Filename: sbom4rust-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sbom4rust-0.3.0.dist-info/RECORD
+Filename: sbom4rust-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbom4rust/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.3.0"
+VERSION: str = "0.4.0"
```

## Comparing `sbom4rust-0.3.0.dist-info/LICENSE` & `sbom4rust-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbom4rust-0.3.0.dist-info/METADATA` & `sbom4rust-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbom4rust
-Version: 0.3.0
+Version: 0.4.0
 Summary: SBOM generator for Rust modules
 Home-page: https://github.com/anthonyharrison/sbom4rust
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lib4sbom
+Requires-Dist: lib4sbom (>=0.4.0)
 Requires-Dist: toml
 
 # SBOM4Rust
 
 SBOM4Rust generates a SBOM (Software Bill of Materials) for Rust application or library in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
 It identifies all the dependent components which are explicity defined in the `Cargo.lock` file and reports the relationships between the components.
```

## Comparing `sbom4rust-0.3.0.dist-info/RECORD` & `sbom4rust-0.4.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 sbom4rust/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sbom4rust/cli.py,sha256=SFzzogCy_PG-5yKRt3DIyELM1tkzurCkYpPRPZxOmdA,3963
 sbom4rust/scanner.py,sha256=Nvr_ONbZiz4J-8nX-aQEdhbtmN-VhS0AzAA9GwAyrX8,5442
-sbom4rust/version.py,sha256=_p-y2a7gEF6oU37vmbGAsqrCSIpyaZoCAugkrzEBDQI,100
-sbom4rust-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbom4rust-0.3.0.dist-info/METADATA,sha256=aRqEzKwyVkhIJaAI-iZHy7cx8BRTp4L0tJOXfCMmW74,4730
-sbom4rust-0.3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbom4rust-0.3.0.dist-info/entry_points.txt,sha256=Cb8-kb5f-hfjR9QVG1UHpZmjtXYEzPIrPYBJIFFPYqg,49
-sbom4rust-0.3.0.dist-info/top_level.txt,sha256=gLWI0YmrFGeHVxumrj0UKykTr6gdKtM9_FeEABm_ID8,10
-sbom4rust-0.3.0.dist-info/RECORD,,
+sbom4rust/version.py,sha256=7JpTeIdgA2tX24hrLXHM3T788cSCK36qgBVFqIuHxgo,100
+sbom4rust-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbom4rust-0.4.0.dist-info/METADATA,sha256=JComEx-FYdG5cmjSOCz5a7zcp3nt4lkCUVnQ_9iENHQ,4740
+sbom4rust-0.4.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbom4rust-0.4.0.dist-info/entry_points.txt,sha256=Cb8-kb5f-hfjR9QVG1UHpZmjtXYEzPIrPYBJIFFPYqg,49
+sbom4rust-0.4.0.dist-info/top_level.txt,sha256=gLWI0YmrFGeHVxumrj0UKykTr6gdKtM9_FeEABm_ID8,10
+sbom4rust-0.4.0.dist-info/RECORD,,
```

