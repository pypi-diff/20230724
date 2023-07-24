# Comparing `tmp/sbom4files-0.2.2-py2.py3-none-any.whl.zip` & `tmp/sbom4files-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11999 bytes, number of entries: 11
+Zip file size: 12076 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:03 sbom4files/__init__.py
 -rw-r--r--  2.0 unx     5579 b- defN 23-Feb-21 14:56 sbom4files/cli.py
--rw-r--r--  2.0 unx     6782 b- defN 23-Apr-10 17:02 sbom4files/filescanner.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:28 sbom4files/version.py
+-rw-r--r--  2.0 unx     7050 b- defN 23-Jul-23 20:48 sbom4files/filescanner.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-23 20:59 sbom4files/version.py
 -rw-r--r--  2.0 unx      217 b- defN 23-Mar-02 18:44 sbom4files/filetypes/filetypes.txt
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5296 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      901 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/RECORD
-11 files, 30480 bytes uncompressed, 10469 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-24 17:38 sbom4files-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5354 b- defN 23-Jul-24 17:38 sbom4files-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 17:38 sbom4files-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Jul-24 17:38 sbom4files-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-24 17:38 sbom4files-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      901 b- defN 23-Jul-24 17:38 sbom4files-0.3.0.dist-info/RECORD
+11 files, 30806 bytes uncompressed, 10546 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: sbom4files/version.py
 Comment: 
 
 Filename: sbom4files/filetypes/filetypes.txt
 Comment: 
 
-Filename: sbom4files-0.2.2.dist-info/LICENSE
+Filename: sbom4files-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: sbom4files-0.2.2.dist-info/METADATA
+Filename: sbom4files-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sbom4files-0.2.2.dist-info/WHEEL
+Filename: sbom4files-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sbom4files-0.2.2.dist-info/entry_points.txt
+Filename: sbom4files-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbom4files-0.2.2.dist-info/top_level.txt
+Filename: sbom4files-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sbom4files-0.2.2.dist-info/RECORD
+Filename: sbom4files-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbom4files/filescanner.py

```diff
@@ -128,17 +128,22 @@
                 print(f"Processing {filename} {mimetype}")
             found_license, found_copyright, copyright_text = self._find_licence(
                 filename
             )
             if found_license is not None:
                 for license in found_license:
                     self.sbom_file.set_licenseinfoinfile(license)
-                    self.sbom_file.set_licensecomment(
+                    license_comment = (
                         "This information was automatically extracted from the file."
                     )
+                    if self.licensescanner.deprecated(license):
+                        license_comment = (
+                            f"{license_comment} {license} is now deprecated."
+                        )
+                    self.sbom_file.set_licensecomment(license_comment)
                 if len(found_license) == 1:
                     self.sbom_file.set_licenseconcluded(found_license[0])
                 else:
                     concluded_licence = " AND ".join(f for f in found_license)
                     self.sbom_file.set_licenseconcluded(concluded_licence)
             else:
                 # Default licence status
```

## sbom4files/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.2.2"
+VERSION: str = "0.3.0"
```

## Comparing `sbom4files-0.2.2.dist-info/LICENSE` & `sbom4files-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbom4files-0.2.2.dist-info/METADATA` & `sbom4files-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbom4files
-Version: 0.2.2
+Version: 0.3.0
 Summary: SBOM generator for files in a directory
 Home-page: https://github.com/anthonyharrison/sbom4files
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -20,16 +20,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lib4sbom (>=0.3.1)
+Requires-Dist: lib4sbom (>=0.4.0)
 Requires-Dist: python-magic
+Requires-Dist: python-magic-bin ; sys_platform == "win32"
 
 # SBOM4Files
 
 SBOM4Files generates a SBOM (Software Bill of Materials) for a directory in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
 It identifies all files within a directory and includes license and copyright information, where possible, for each file.
```

## Comparing `sbom4files-0.2.2.dist-info/RECORD` & `sbom4files-0.3.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 sbom4files/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
 sbom4files/cli.py,sha256=2sUdqMki4i2ABxUuKd0Pr6f775Dlnp8G7BwsmP9Y8Tg,5579
-sbom4files/filescanner.py,sha256=sKkvDr0mWZO8ZmgQbW3JWlebXwov5hM7UsUwW4a6T1g,6782
-sbom4files/version.py,sha256=VP4uRSuHmuKjzwIqMLUYkkWD0y-Vmwjp3767t3k7EKE,100
+sbom4files/filescanner.py,sha256=vu9pIPmbtULrkAfJgvSq1KdOJlbvmw2n_R97AbRXoNk,7050
+sbom4files/version.py,sha256=_p-y2a7gEF6oU37vmbGAsqrCSIpyaZoCAugkrzEBDQI,100
 sbom4files/filetypes/filetypes.txt,sha256=mFdRDlJg_vIWslpGQcEixVr1xRU902jfnMR0dkz7U4g,217
-sbom4files-0.2.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbom4files-0.2.2.dist-info/METADATA,sha256=QJRYSqLSujs9SRZwAR51G-KoREbiQpz7zPCFZfPovwI,5296
-sbom4files-0.2.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbom4files-0.2.2.dist-info/entry_points.txt,sha256=XlS7rP6kZ-HMnSqDDpYCWlEeYxMTU7O9uAsIGirYBcc,51
-sbom4files-0.2.2.dist-info/top_level.txt,sha256=S42h8aNeBI7n-q5AaLwoFesKPogNrCB2kQ9-XqbDa6w,11
-sbom4files-0.2.2.dist-info/RECORD,,
+sbom4files-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbom4files-0.3.0.dist-info/METADATA,sha256=fJse-xJ-o7BJIISqYIVp8bVIr4gtqESQX4HQ8btgc2E,5354
+sbom4files-0.3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbom4files-0.3.0.dist-info/entry_points.txt,sha256=XlS7rP6kZ-HMnSqDDpYCWlEeYxMTU7O9uAsIGirYBcc,51
+sbom4files-0.3.0.dist-info/top_level.txt,sha256=S42h8aNeBI7n-q5AaLwoFesKPogNrCB2kQ9-XqbDa6w,11
+sbom4files-0.3.0.dist-info/RECORD,,
```

