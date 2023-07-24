# Comparing `tmp/sbomaudit-0.1.2-py2.py3-none-any.whl.zip` & `tmp/sbomaudit-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 14807 bytes, number of entries: 10
+Zip file size: 14838 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:08 sbomaudit/__init__.py
--rw-r--r--  2.0 unx    21953 b- defN 23-Apr-10 17:31 sbomaudit/audit.py
+-rw-r--r--  2.0 unx    22617 b- defN 23-Jul-23 21:42 sbomaudit/audit.py
 -rw-r--r--  2.0 unx     4416 b- defN 23-Mar-02 17:59 sbomaudit/cli.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:36 sbomaudit/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    14069 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      797 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/RECORD
-10 files, 52937 bytes uncompressed, 13453 bytes compressed:  74.6%
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 21:10 sbomaudit/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-24 18:04 sbomaudit-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14074 b- defN 23-Jul-24 18:04 sbomaudit-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 18:04 sbomaudit-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Jul-24 18:04 sbomaudit-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-24 18:04 sbomaudit-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      797 b- defN 23-Jul-24 18:04 sbomaudit-0.2.0.dist-info/RECORD
+10 files, 53606 bytes uncompressed, 13484 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: sbomaudit/cli.py
 Comment: 
 
 Filename: sbomaudit/version.py
 Comment: 
 
-Filename: sbomaudit-0.1.2.dist-info/LICENSE
+Filename: sbomaudit-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: sbomaudit-0.1.2.dist-info/METADATA
+Filename: sbomaudit-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: sbomaudit-0.1.2.dist-info/WHEEL
+Filename: sbomaudit-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: sbomaudit-0.1.2.dist-info/entry_points.txt
+Filename: sbomaudit-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbomaudit-0.1.2.dist-info/top_level.txt
+Filename: sbomaudit-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sbomaudit-0.1.2.dist-info/RECORD
+Filename: sbomaudit-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbomaudit/audit.py

```diff
@@ -154,15 +154,15 @@
                     "Up to date SPDX Version",
                     ["SPDX-2.2", "SPDX-2.3"],
                     document.get_version(),
                 )
             else:
                 self._check_value(
                     "Up to date CycloneDX Version",
-                    ["1.3", "1.4"],
+                    ["1.3", "1.4", "1.5"],
                     document.get_version(),
                 )
             creation_time = document.get_created() is not None
             creator_identified = len(document.get_creator()) > 0
             relationships_valid = len(relationships) > 0
             self._check("SBOM Creator identified", creator_identified)
             self._check("SBOM Creation time defined", creation_time)
@@ -223,14 +223,18 @@
                                 spdx_license,
                                 failure_text=f"{license}",
                             )
                             self._check(
                                 f"OSI Approved license for {name}",
                                 self.license_scanner.osi_approved(license),
                             )
+                            self._check(
+                                f"Non-deprecated license for {name}",
+                                not self.license_scanner.deprecated(license),
+                            )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for {name}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
                             )
                         if deny_licenses is not None:
@@ -260,14 +264,18 @@
                                 spdx_license,
                                 failure_text=f"{license}",
                             )
                             self._check(
                                 f"OSI Approved license for {id}",
                                 self.license_scanner.osi_approved(license),
                             )
+                            self._check(
+                                f"Non-deprecated license for {name}",
+                                not self.license_scanner.deprecated(license),
+                            )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for {id}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
                             )
                         if deny_licenses is not None:
@@ -377,14 +385,18 @@
                                 spdx_license,
                                 failure_text=f"{license}",
                             )
                             self._check(
                                 f"OSI Approved license for {name}",
                                 self.license_scanner.osi_approved(license),
                             )
+                            self._check(
+                                f"Non-deprecated license for {name}",
+                                not self.license_scanner.deprecated(license),
+                            )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for package {name}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
                             )
                         if deny_licenses is not None:
```

## sbomaudit/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.1.2"
+VERSION: str = "0.2.0"
```

## Comparing `sbomaudit-0.1.2.dist-info/LICENSE` & `sbomaudit-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbomaudit-0.1.2.dist-info/METADATA` & `sbomaudit-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbomaudit
-Version: 0.1.2
+Version: 0.2.0
 Summary: Audit SBOM contents
 Home-page: https://github.com/anthonyharrison/sbomaudit
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -20,20 +20,20 @@
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
 Requires-Dist: requests
 Requires-Dist: packageurl-python
 
-# SBOMAUIDT
+# SBOMAUDIT
 
 SBOMAUDIT reports on the quality of the contents of an SBOM (Software Bill of Materials) by performing a number of checks. SBOMs are supported in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
 
 ## Installation
 
 To install use the following command:
@@ -128,15 +128,15 @@
 
 The following section identifies the checks which are performed.
 
 ### SBOM Format
 
 The following checks are performed:
 
-- Check that the version of the SBOM is either version 2.2 or 2.3 (SPDX) or version 1.3 or 1.4 (CycloneDX).
+- Check that the version of the SBOM is either version 2.2 or 2.3 (SPDX) or version 1.3, 1.4 or 1.5 (CycloneDX).
 
 - Check that a creator is defined.
 
 - Check that the time that the SBOM is created is defined.
 
 ### Files
```

## Comparing `sbomaudit-0.1.2.dist-info/RECORD` & `sbomaudit-0.2.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 sbomaudit/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-sbomaudit/audit.py,sha256=wBEpEOwLeS4NzsZtIR0HqlrCVNJMQZE98ChQlv1NuSY,21953
+sbomaudit/audit.py,sha256=4Qwo-pCO84ix2cGDuNWe9ONB10NV26Uzhe2yP0SmhXk,22617
 sbomaudit/cli.py,sha256=i29SeCOa4HtQ4p6GNkJhskEdGht9OjhNN7s1O8-dH3k,4416
-sbomaudit/version.py,sha256=hrPdaOLNANEcNndLBVrZaUWgb423W5Fht_jiswwp470,100
-sbomaudit-0.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbomaudit-0.1.2.dist-info/METADATA,sha256=Ma9trFDpQwf5ZTJhc1OUgIplSoYBTtZydVpRmwygoWw,14069
-sbomaudit-0.1.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbomaudit-0.1.2.dist-info/entry_points.txt,sha256=f8Rv8KaNsOGMapJwNvfQYJUoc8O8S2Ce49e3-Qa6n-I,49
-sbomaudit-0.1.2.dist-info/top_level.txt,sha256=8U0fCtvt4EJsO7B5XDwiiuBa7CsDVbcPJOJfWWJWcp0,10
-sbomaudit-0.1.2.dist-info/RECORD,,
+sbomaudit/version.py,sha256=Mustbl9r6LIU5iErNlnCJ7lyI7PZQHJcJDUDLTkW-p8,100
+sbomaudit-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbomaudit-0.2.0.dist-info/METADATA,sha256=nOtDWOTF4dlCgQPC9x0moPb-gr3MKTSG0G8pJAGOTDE,14074
+sbomaudit-0.2.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbomaudit-0.2.0.dist-info/entry_points.txt,sha256=f8Rv8KaNsOGMapJwNvfQYJUoc8O8S2Ce49e3-Qa6n-I,49
+sbomaudit-0.2.0.dist-info/top_level.txt,sha256=8U0fCtvt4EJsO7B5XDwiiuBa7CsDVbcPJOJfWWJWcp0,10
+sbomaudit-0.2.0.dist-info/RECORD,,
```

