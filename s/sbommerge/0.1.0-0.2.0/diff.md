# Comparing `tmp/sbommerge-0.1.0-py2.py3-none-any.whl.zip` & `tmp/sbommerge-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 25263 bytes, number of entries: 18
+Zip file size: 25271 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-06 10:15 sbommerge/__init__.py
 -rw-r--r--  2.0 unx    14141 b- defN 23-Apr-13 17:11 sbommerge/cli.py
 -rw-r--r--  2.0 unx     5540 b- defN 22-Nov-11 12:58 sbommerge/cyclonedx_parser.py
 -rw-r--r--  2.0 unx     9736 b- defN 22-Oct-20 08:04 sbommerge/cyclonedxgenerator.py
 -rw-r--r--  2.0 unx     2449 b- defN 22-Nov-11 17:41 sbommerge/file.py
 -rw-r--r--  2.0 unx     4004 b- defN 22-Nov-11 17:59 sbommerge/generator.py
 -rw-r--r--  2.0 unx     2234 b- defN 22-Nov-13 15:03 sbommerge/output.py
 -rw-r--r--  2.0 unx     3322 b- defN 22-Oct-20 08:04 sbommerge/package.py
 -rw-r--r--  2.0 unx      758 b- defN 22-Oct-17 13:38 sbommerge/relationship.py
 -rw-r--r--  2.0 unx    17728 b- defN 22-Nov-11 17:32 sbommerge/spdx_parser.py
 -rw-r--r--  2.0 unx    18037 b- defN 22-Nov-13 10:38 sbommerge/spdxgenerator.py
--rw-r--r--  2.0 unx      100 b- defN 22-Oct-06 10:17 sbommerge/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbommerge-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4896 b- defN 23-Apr-14 15:13 sbommerge-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbommerge-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-14 15:13 sbommerge-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-14 15:13 sbommerge-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1447 b- defN 23-Apr-14 15:13 sbommerge-0.1.0.dist-info/RECORD
-18 files, 95918 bytes uncompressed, 22911 bytes compressed:  76.1%
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 21:10 sbommerge/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-24 18:07 sbommerge-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4955 b- defN 23-Jul-24 18:07 sbommerge-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 18:07 sbommerge-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Jul-24 18:07 sbommerge-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-24 18:07 sbommerge-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1447 b- defN 23-Jul-24 18:07 sbommerge-0.2.0.dist-info/RECORD
+18 files, 95977 bytes uncompressed, 22919 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sbommerge/spdxgenerator.py
 Comment: 
 
 Filename: sbommerge/version.py
 Comment: 
 
-Filename: sbommerge-0.1.0.dist-info/LICENSE
+Filename: sbommerge-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: sbommerge-0.1.0.dist-info/METADATA
+Filename: sbommerge-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: sbommerge-0.1.0.dist-info/WHEEL
+Filename: sbommerge-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: sbommerge-0.1.0.dist-info/entry_points.txt
+Filename: sbommerge-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbommerge-0.1.0.dist-info/top_level.txt
+Filename: sbommerge-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sbommerge-0.1.0.dist-info/RECORD
+Filename: sbommerge-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbommerge/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2022 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.1.0"
+VERSION: str = "0.2.0"
```

## Comparing `sbommerge-0.1.0.dist-info/LICENSE` & `sbommerge-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbommerge-0.1.0.dist-info/METADATA` & `sbommerge-0.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbommerge
-Version: 0.1.0
+Version: 0.2.0
 Summary: Software Bill of Material (SBOM) merge tool
 Home-page: https://github.com/anthonyharrison/sbommerge
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
-Requires-Dist: lib4sbom (>=0.3.1)
+Requires-Dist: lib4sbom (>=0.4.0)
 
 # SBOMMerge
 
 SBOMMerge merges two Software Bill of Materials (SBOMs) documents together. It supports SBOMs created in both
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org) formats.
 
 ## Installation
@@ -81,14 +81,15 @@
 | SBOM Type | Version   | Extension      |Format         |
 | --------- | --------- | ---------------|---------------|
 | SPDX      | 2.3       | .spdx          | TagValue      |
 | SPDX      | 2.3       | .spdx.json     | JSON          |
 | SPDX      | 2.3       | .spdx.yml      | YAML          |
 | SPDX      | 2.3       | .spdx.yaml     | YAML          |
 | CycloneDX | 1.4       | .json          | JSON          |
+| CycloneDX | 1.5       | .json          | JSON          |
 
 Details of the formats for each of the supported SBOM formats are available for
 [SPDX](https://spdx.dev/) and [CycloneDX](https://cyclonedx.org/).
 
 For SPDX SBOM files, it is assumed that the name of a Package precedes the version information for the package.
 Only modules with a package name and associated version information shall be processed.
```

## Comparing `sbommerge-0.1.0.dist-info/RECORD` & `sbommerge-0.2.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 sbommerge/file.py,sha256=UobKzzQUl_CGvIE60Dh9SepkcrquHBSeWQ_X3U7eNxs,2449
 sbommerge/generator.py,sha256=MCquKYLI8fjKSSinA3v7rH08ujNieqEnveeRVdyXYFI,4004
 sbommerge/output.py,sha256=iYGyAG6EaBHMWNzXlsI-60l4j0y2l_ggdPDY4-frHYI,2234
 sbommerge/package.py,sha256=XtYbzPoXFV825wz3WHGVoWNV0hm5wVmnksRiDywcutY,3322
 sbommerge/relationship.py,sha256=1TM_Omfz6VpE7DnjXH3cjEsdZPgaoNBzISQAWrG0XIk,758
 sbommerge/spdx_parser.py,sha256=plSqiJ6nWmGDrqBaWo2a_o3cBSVA9CyI6wWYtAJ7jiA,17728
 sbommerge/spdxgenerator.py,sha256=H2INyOGW4793SkSvlbh37I5-lsinED3JiMuSs_mOExo,18037
-sbommerge/version.py,sha256=UElp1S4vflxjj9NWNXktWralI0iCvF7tALLpAhTFJ28,100
-sbommerge-0.1.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbommerge-0.1.0.dist-info/METADATA,sha256=ELPGuLOQValSbXw2p-Vq8w7_28RJeR2aLXs9l6S9HE8,4896
-sbommerge-0.1.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbommerge-0.1.0.dist-info/entry_points.txt,sha256=NHQLHvxk0L7r2H_OWPXbcMdLvJ_sB-PhhbJCTZh_sB0,49
-sbommerge-0.1.0.dist-info/top_level.txt,sha256=9VnXQdMhfr8LmjXrn-arM935Y-2CzZwgsoQaYz8n2Mo,10
-sbommerge-0.1.0.dist-info/RECORD,,
+sbommerge/version.py,sha256=y4e1Q64VDcNdLST0o5gHkHdLoGtNPxbRS5XphRYvjWM,100
+sbommerge-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbommerge-0.2.0.dist-info/METADATA,sha256=yL72tXljeduT9kuZkfhbX0aStb0H41kfoCSIyYWKghA,4955
+sbommerge-0.2.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbommerge-0.2.0.dist-info/entry_points.txt,sha256=NHQLHvxk0L7r2H_OWPXbcMdLvJ_sB-PhhbJCTZh_sB0,49
+sbommerge-0.2.0.dist-info/top_level.txt,sha256=9VnXQdMhfr8LmjXrn-arM935Y-2CzZwgsoQaYz8n2Mo,10
+sbommerge-0.2.0.dist-info/RECORD,,
```

