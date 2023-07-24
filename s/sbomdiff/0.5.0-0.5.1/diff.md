# Comparing `tmp/sbomdiff-0.5.0-py2.py3-none-any.whl.zip` & `tmp/sbomdiff-0.5.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14236 bytes, number of entries: 12
+Zip file size: 14233 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-02 07:31 sbomdiff/__init__.py
 -rw-r--r--  2.0 unx     8734 b- defN 23-May-15 21:10 sbomdiff/cli.py
 -rw-r--r--  2.0 unx     4470 b- defN 23-Mar-28 20:15 sbomdiff/cyclonedx_parser.py
 -rw-r--r--  2.0 unx     1298 b- defN 22-Oct-20 16:02 sbomdiff/output.py
 -rw-r--r--  2.0 unx     7841 b- defN 23-Apr-13 20:22 sbomdiff/spdx_parser.py
--rw-r--r--  2.0 unx      100 b- defN 23-May-15 21:02 sbomdiff/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7573 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      949 b- defN 23-May-15 21:18 sbomdiff-0.5.0.dist-info/RECORD
-12 files, 42488 bytes uncompressed, 12646 bytes compressed:  70.2%
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 21:03 sbomdiff/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-24 17:45 sbomdiff-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7573 b- defN 23-Jul-24 17:45 sbomdiff-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 17:45 sbomdiff-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-24 17:45 sbomdiff-0.5.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-24 17:45 sbomdiff-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      949 b- defN 23-Jul-24 17:45 sbomdiff-0.5.1.dist-info/RECORD
+12 files, 42488 bytes uncompressed, 12643 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: sbomdiff/spdx_parser.py
 Comment: 
 
 Filename: sbomdiff/version.py
 Comment: 
 
-Filename: sbomdiff-0.5.0.dist-info/LICENSE
+Filename: sbomdiff-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: sbomdiff-0.5.0.dist-info/METADATA
+Filename: sbomdiff-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: sbomdiff-0.5.0.dist-info/WHEEL
+Filename: sbomdiff-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: sbomdiff-0.5.0.dist-info/entry_points.txt
+Filename: sbomdiff-0.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbomdiff-0.5.0.dist-info/top_level.txt
+Filename: sbomdiff-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sbomdiff-0.5.0.dist-info/RECORD
+Filename: sbomdiff-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbomdiff/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2022 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.5.0"
+VERSION: str = "0.5.1"
```

## Comparing `sbomdiff-0.5.0.dist-info/LICENSE` & `sbomdiff-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbomdiff-0.5.0.dist-info/METADATA` & `sbomdiff-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbomdiff
-Version: 0.5.0
+Version: 0.5.1
 Summary: Software Bill of Material (SBOM) difference tool
 Home-page: https://github.com/anthonyharrison/sbomdiff
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: defusedxml
 Requires-Dist: pyyaml (>=5.4)
-Requires-Dist: lib4sbom (>=0.3.1)
+Requires-Dist: lib4sbom (>=0.4.0)
 
 # SBOMDiff
 
 SBOMDiff is a tool to compare two Software Bill of Materials (SBOM) files and
 reports the differences. It supports SBOMs created in both
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org) formats.
```

## Comparing `sbomdiff-0.5.0.dist-info/RECORD` & `sbomdiff-0.5.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 sbomdiff/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sbomdiff/cli.py,sha256=Nq9kZ0qLGn0txXBSIxCo23A-Tb5loq2N_la_lFoaHtY,8734
 sbomdiff/cyclonedx_parser.py,sha256=lBp9SvYnVNxqlznYajTQWVIcTB-rn6bCTs5Ji9bFm0g,4470
 sbomdiff/output.py,sha256=G9tbsqlbCapnTyPgo6ROnSXVoVM2c4Hp1QfhvvvcQcQ,1298
 sbomdiff/spdx_parser.py,sha256=Wtpjg8PhL_6BS7l5GQvNlMMfMo0_Z59vMl13FBP0F5s,7841
-sbomdiff/version.py,sha256=Jpb0I-mkqELebity9eHVTcRu5I4Sjc_mXpT39iSYqWU,100
-sbomdiff-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbomdiff-0.5.0.dist-info/METADATA,sha256=agnhvvlLD04dXvlbTnyg2u6K-z4BG4DwymRJB7SqLpA,7573
-sbomdiff-0.5.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbomdiff-0.5.0.dist-info/entry_points.txt,sha256=fcONsvnGhylyVE47AbBD9yrXj47ScGZbVyJ7jGRcx9o,47
-sbomdiff-0.5.0.dist-info/top_level.txt,sha256=vt1EhODe3hHuS5SesbQue8uX-pOojrBfdtCwYdbEUgg,9
-sbomdiff-0.5.0.dist-info/RECORD,,
+sbomdiff/version.py,sha256=XnY4io6ySDm4EfY-yjs87ZMI2PjSUzm93dJjhBbPWjs,100
+sbomdiff-0.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbomdiff-0.5.1.dist-info/METADATA,sha256=cKqWwwnS59hJWJV15o_zp5Cmvws7djLgJcIjrKcUW34,7573
+sbomdiff-0.5.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbomdiff-0.5.1.dist-info/entry_points.txt,sha256=fcONsvnGhylyVE47AbBD9yrXj47ScGZbVyJ7jGRcx9o,47
+sbomdiff-0.5.1.dist-info/top_level.txt,sha256=vt1EhODe3hHuS5SesbQue8uX-pOojrBfdtCwYdbEUgg,9
+sbomdiff-0.5.1.dist-info/RECORD,,
```

