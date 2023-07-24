# Comparing `tmp/sbom2dot-0.2.1-py2.py3-none-any.whl.zip` & `tmp/sbom2dot-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6289 bytes, number of entries: 9
+Zip file size: 6290 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:05 sbom2dot/__init__.py
 -rw-r--r--  2.0 unx     2482 b- defN 23-Feb-15 10:04 sbom2dot/cli.py
 -rw-r--r--  2.0 unx     3693 b- defN 23-Mar-23 23:05 sbom2dot/dotgenerator.py
--rw-r--r--  2.0 unx      100 b- defN 23-Mar-23 21:03 sbom2dot/version.py
--rw-r--r--  2.0 unx     7904 b- defN 23-Mar-27 14:14 sbom2dot-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-27 14:14 sbom2dot-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Mar-27 14:14 sbom2dot-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-27 14:14 sbom2dot-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      701 b- defN 23-Mar-27 14:14 sbom2dot-0.2.1.dist-info/RECORD
-9 files, 15122 bytes uncompressed, 5081 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 21:11 sbom2dot/version.py
+-rw-r--r--  2.0 unx     7904 b- defN 23-Jul-24 18:12 sbom2dot-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 18:12 sbom2dot-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-24 18:12 sbom2dot-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-24 18:12 sbom2dot-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      701 b- defN 23-Jul-24 18:12 sbom2dot-0.3.0.dist-info/RECORD
+9 files, 15122 bytes uncompressed, 5082 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sbom2dot/dotgenerator.py
 Comment: 
 
 Filename: sbom2dot/version.py
 Comment: 
 
-Filename: sbom2dot-0.2.1.dist-info/METADATA
+Filename: sbom2dot-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sbom2dot-0.2.1.dist-info/WHEEL
+Filename: sbom2dot-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sbom2dot-0.2.1.dist-info/entry_points.txt
+Filename: sbom2dot-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbom2dot-0.2.1.dist-info/top_level.txt
+Filename: sbom2dot-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sbom2dot-0.2.1.dist-info/RECORD
+Filename: sbom2dot-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbom2dot/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.2.1"
+VERSION: str = "0.3.0"
```

## Comparing `sbom2dot-0.2.1.dist-info/METADATA` & `sbom2dot-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbom2dot
-Version: 0.2.1
+Version: 0.3.0
 Summary: Create a dependency graph of the components within a SBOM
 Home-page: https://github.com/anthonyharrison/sbom2dot
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: lib4sbom (>=0.3.0)
+Requires-Dist: lib4sbom (>=0.4.0)
 
 # SBOM2DOT
 
 SBOM2DOT generates a dependency graph of the components within an SBOM (Software Bill of Materials). The format of the graph
 file is compatible with the [DOT language](https://graphviz.org/doc/info/lang.html) used by the
 [GraphViz](https://graphviz.org/) application. SBOMs are supported in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
```

## Comparing `sbom2dot-0.2.1.dist-info/RECORD` & `sbom2dot-0.3.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sbom2dot/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
 sbom2dot/cli.py,sha256=2M3674YJti3dwAaXDkYFpFPumatp53NvDbtkKnVOMek,2482
 sbom2dot/dotgenerator.py,sha256=ZBrcysOqxCFLkQP3eDDfe1jG15vCEyOvqbP5_V6PVWU,3693
-sbom2dot/version.py,sha256=Sf4YLFWUpG_pOy51nAMl86uP4c0l_zH7N9PSxWNRR6w,100
-sbom2dot-0.2.1.dist-info/METADATA,sha256=2GaSpnW9pbhzZKwWJa2JPX8AlVGjDeUBYH4CSuzeyEc,7904
-sbom2dot-0.2.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbom2dot-0.2.1.dist-info/entry_points.txt,sha256=NCoLNj-LIJCkkYH91B_3xexdWse4snrLlEFxwlNMzO0,47
-sbom2dot-0.2.1.dist-info/top_level.txt,sha256=_V_3qTiGX2c9tLPS7xbX51Dc4oWALXo693JqM7AMoJ4,9
-sbom2dot-0.2.1.dist-info/RECORD,,
+sbom2dot/version.py,sha256=_p-y2a7gEF6oU37vmbGAsqrCSIpyaZoCAugkrzEBDQI,100
+sbom2dot-0.3.0.dist-info/METADATA,sha256=VIYCP3ej0yMJne_VlTz_pVvBcEm3rS3v-gqKK5xn3KI,7904
+sbom2dot-0.3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbom2dot-0.3.0.dist-info/entry_points.txt,sha256=NCoLNj-LIJCkkYH91B_3xexdWse4snrLlEFxwlNMzO0,47
+sbom2dot-0.3.0.dist-info/top_level.txt,sha256=_V_3qTiGX2c9tLPS7xbX51Dc4oWALXo693JqM7AMoJ4,9
+sbom2dot-0.3.0.dist-info/RECORD,,
```

