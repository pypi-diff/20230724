# Comparing `tmp/sbom2doc-0.2.0-py2.py3-none-any.whl.zip` & `tmp/sbom2doc-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 16185 bytes, number of entries: 15
+Zip file size: 16222 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:05 sbom2doc/__init__.py
 -rw-r--r--  2.0 unx     2915 b- defN 23-Apr-04 15:57 sbom2doc/cli.py
--rw-r--r--  2.0 unx     7083 b- defN 23-Apr-10 17:29 sbom2doc/generator.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:35 sbom2doc/version.py
+-rw-r--r--  2.0 unx     7207 b- defN 23-Jul-15 16:34 sbom2doc/generator.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 21:09 sbom2doc/version.py
 -rw-r--r--  2.0 unx       76 b- defN 23-Apr-04 15:59 sbom2doc/docbuilder/__init__.py
 -rw-r--r--  2.0 unx     1367 b- defN 23-Apr-09 20:09 sbom2doc/docbuilder/consolebuilder.py
 -rw-r--r--  2.0 unx      481 b- defN 23-Apr-03 21:56 sbom2doc/docbuilder/docbuilder.py
 -rw-r--r--  2.0 unx     1107 b- defN 23-Apr-03 21:45 sbom2doc/docbuilder/markdownbuilder.py
 -rw-r--r--  2.0 unx     5818 b- defN 23-Apr-13 19:16 sbom2doc/docbuilder/pdfbuilder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    14054 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1243 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/RECORD
-15 files, 45843 bytes uncompressed, 14119 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-24 17:55 sbom2doc-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14054 b- defN 23-Jul-24 17:55 sbom2doc-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 17:55 sbom2doc-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-24 17:55 sbom2doc-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-24 17:55 sbom2doc-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1243 b- defN 23-Jul-24 17:55 sbom2doc-0.3.0.dist-info/RECORD
+15 files, 45967 bytes uncompressed, 14156 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: sbom2doc/docbuilder/markdownbuilder.py
 Comment: 
 
 Filename: sbom2doc/docbuilder/pdfbuilder.py
 Comment: 
 
-Filename: sbom2doc-0.2.0.dist-info/LICENSE
+Filename: sbom2doc-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: sbom2doc-0.2.0.dist-info/METADATA
+Filename: sbom2doc-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sbom2doc-0.2.0.dist-info/WHEEL
+Filename: sbom2doc-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sbom2doc-0.2.0.dist-info/entry_points.txt
+Filename: sbom2doc-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbom2doc-0.2.0.dist-info/top_level.txt
+Filename: sbom2doc-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sbom2doc-0.2.0.dist-info/RECORD
+Filename: sbom2doc-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbom2doc/generator.py

```diff
@@ -14,14 +14,15 @@
 def generate_document(format, sbom_parser, filename, outfile, include_license):
     # Get constituent components of the SBOM
     packages = sbom_parser.get_packages()
     files = sbom_parser.get_files()
     relationships = sbom_parser.get_relationships()
     document = SBOMDocument()
     document.copy_document(sbom_parser.get_document())
+    license_info = LicenseScanner()
 
     # Select document builder based on format
     if format == "markdown":
         sbom_document = MarkdownBuilder()
     elif format == "pdf":
         sbom_document = PDFBuilder()
     else:
@@ -81,14 +82,16 @@
         for package in packages:
             # Minimum elements are ID, Name, Version, Supplier
             id = package.get("id", None)
             name = package.get("name", None)
             version = package.get("version", None)
             supplier = package.get("supplier", None)
             license = package.get("licenseconcluded", "NOT KNOWN")
+            if license != "NOT KNOWN" and license_info.deprecated(license):
+                license = f"{license} (Deprecated)"
             sbom_licenses.append(license)
             sbom_document.addrow([name, version, supplier, license])
             if (
                 id is None
                 or name is None
                 or version is None
                 or supplier is None
@@ -151,15 +154,14 @@
         and relationships_valid
     )
     sbom_document.paragraph(f"NTIA conformant {valid_sbom}")
 
     if include_license:
         sbom_document.pagebreak()
         sbom_document.heading(1, "License Text")
-        license_info = LicenseScanner()
         for key, value in freq.items():
             # Ignore undefined licenses or expressions
             if key == "NOASSERTION" or license_info.license_expression(key):
                 continue
             license_url = f"https://spdx.org/licenses/{key}.json"
             try:
                 license_text = requests.get(license_url).json()
```

## sbom2doc/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.2.0"
+VERSION: str = "0.3.0"
```

## Comparing `sbom2doc-0.2.0.dist-info/LICENSE` & `sbom2doc-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbom2doc-0.2.0.dist-info/METADATA` & `sbom2doc-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbom2doc
-Version: 0.2.0
+Version: 0.3.0
 Summary: SBOM generator for Python modules
 Home-page: https://github.com/anthonyharrison/sbom2doc
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
 Requires-Dist: rich
 Requires-Dist: reportlab
 Requires-Dist: packageurl-python
 
 # SBOM2DOC
 
 SBOM2DOC documents and summarises the components within an SBOM (Software Bill of Materials). SBOMS are supported in a number of formats including
```

## Comparing `sbom2doc-0.2.0.dist-info/RECORD` & `sbom2doc-0.3.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 sbom2doc/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
 sbom2doc/cli.py,sha256=DmYEtaBzQ5qvLQg7alD-tC13mqXJNJ7Pr-WN54ofoY0,2915
-sbom2doc/generator.py,sha256=iMIL9V14oTxJ62mXQ7JL7ymK9xhy1PSD5TBE-peHa2k,7083
-sbom2doc/version.py,sha256=Mustbl9r6LIU5iErNlnCJ7lyI7PZQHJcJDUDLTkW-p8,100
+sbom2doc/generator.py,sha256=gVoUfkRUd5vOvvH60QLg8wre37W3A53q_MQZTdA6Nh0,7207
+sbom2doc/version.py,sha256=_p-y2a7gEF6oU37vmbGAsqrCSIpyaZoCAugkrzEBDQI,100
 sbom2doc/docbuilder/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
 sbom2doc/docbuilder/consolebuilder.py,sha256=QGFAcgk7q7eL2Y8141xPWFBUEwDiQ0XNwCRFbC7-BL8,1367
 sbom2doc/docbuilder/docbuilder.py,sha256=U8mvemVpbRg2a2NR0x-eaGAIpd6bY2bq_MZ3_IbcAi4,481
 sbom2doc/docbuilder/markdownbuilder.py,sha256=Io56grxZYX3yNnEBbFehty8zxq1V8XPEXANPPgtb8Ao,1107
 sbom2doc/docbuilder/pdfbuilder.py,sha256=I7sFtSW-Wrg3zDbPU1NKEGhARAZQr-zShe-yVbG_UCA,5818
-sbom2doc-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbom2doc-0.2.0.dist-info/METADATA,sha256=w5J7LYt8j_WRsglmISk5i7-a2wrdeEY3cib-e-GXMTU,14054
-sbom2doc-0.2.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbom2doc-0.2.0.dist-info/entry_points.txt,sha256=-bmvwIx9D5RZ0FGkoBtdSqwTXAE5wSiDHhY4jCsdCOk,47
-sbom2doc-0.2.0.dist-info/top_level.txt,sha256=SgNoJfZaHup5cF818Xlucq4NcZ-Ukxtm0E99YmxDc3c,9
-sbom2doc-0.2.0.dist-info/RECORD,,
+sbom2doc-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbom2doc-0.3.0.dist-info/METADATA,sha256=j1hg31QWPq4GLuzziPf8KUX-igeOD44IEib9q3C_el4,14054
+sbom2doc-0.3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbom2doc-0.3.0.dist-info/entry_points.txt,sha256=-bmvwIx9D5RZ0FGkoBtdSqwTXAE5wSiDHhY4jCsdCOk,47
+sbom2doc-0.3.0.dist-info/top_level.txt,sha256=SgNoJfZaHup5cF818Xlucq4NcZ-Ukxtm0E99YmxDc3c,9
+sbom2doc-0.3.0.dist-info/RECORD,,
```

