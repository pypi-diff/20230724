# Comparing `tmp/distro2sbom-0.3.0-py2.py3-none-any.whl.zip` & `tmp/distro2sbom-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 20056 bytes, number of entries: 14
+Zip file size: 21206 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:04 distro2sbom/__init__.py
--rw-r--r--  2.0 unx     7510 b- defN 23-Apr-10 17:00 distro2sbom/cli.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:25 distro2sbom/version.py
+-rw-r--r--  2.0 unx     7791 b- defN 23-Jul-23 20:45 distro2sbom/cli.py
+-rw-r--r--  2.0 unx      462 b- defN 23-Jul-23 20:45 distro2sbom/test.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-13 17:46 distro2sbom/version.py
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:04 distro2sbom/distrobuilder/__init__.py
--rw-r--r--  2.0 unx     2582 b- defN 23-Apr-11 16:33 distro2sbom/distrobuilder/distrobuilder.py
--rw-r--r--  2.0 unx    12435 b- defN 23-Apr-13 13:17 distro2sbom/distrobuilder/dpkgbuilder.py
--rw-r--r--  2.0 unx    12251 b- defN 23-Apr-13 13:15 distro2sbom/distrobuilder/rpmbuilder.py
--rw-r--r--  2.0 unx     4421 b- defN 23-Mar-02 20:15 distro2sbom/distrobuilder/windowsbuilder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    10305 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1225 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/RECORD
-14 files, 62513 bytes uncompressed, 17996 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx     3110 b- defN 23-Jul-23 20:45 distro2sbom/distrobuilder/distrobuilder.py
+-rw-r--r--  2.0 unx    13415 b- defN 23-Jul-23 20:47 distro2sbom/distrobuilder/dpkgbuilder.py
+-rw-r--r--  2.0 unx    14043 b- defN 23-Jul-23 20:47 distro2sbom/distrobuilder/rpmbuilder.py
+-rw-r--r--  2.0 unx     4688 b- defN 23-Jul-23 20:45 distro2sbom/distrobuilder/windowsbuilder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-24 11:05 distro2sbom-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10573 b- defN 23-Jul-24 11:05 distro2sbom-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 11:05 distro2sbom-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 11:05 distro2sbom-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-24 11:05 distro2sbom-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1300 b- defN 23-Jul-24 11:05 distro2sbom-0.4.0.dist-info/RECORD
+15 files, 67166 bytes uncompressed, 19032 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: distro2sbom/__init__.py
 Comment: 
 
 Filename: distro2sbom/cli.py
 Comment: 
 
+Filename: distro2sbom/test.py
+Comment: 
+
 Filename: distro2sbom/version.py
 Comment: 
 
 Filename: distro2sbom/distrobuilder/__init__.py
 Comment: 
 
 Filename: distro2sbom/distrobuilder/distrobuilder.py
@@ -18,26 +21,26 @@
 
 Filename: distro2sbom/distrobuilder/rpmbuilder.py
 Comment: 
 
 Filename: distro2sbom/distrobuilder/windowsbuilder.py
 Comment: 
 
-Filename: distro2sbom-0.3.0.dist-info/LICENSE
+Filename: distro2sbom-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: distro2sbom-0.3.0.dist-info/METADATA
+Filename: distro2sbom-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: distro2sbom-0.3.0.dist-info/WHEEL
+Filename: distro2sbom-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: distro2sbom-0.3.0.dist-info/entry_points.txt
+Filename: distro2sbom-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: distro2sbom-0.3.0.dist-info/top_level.txt
+Filename: distro2sbom-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: distro2sbom-0.3.0.dist-info/RECORD
+Filename: distro2sbom-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## distro2sbom/cli.py

```diff
@@ -132,38 +132,41 @@
     defaults = {
         "distro": "",
         "input_file": "",
         "output_file": "",
         "sbom": "spdx",
         "debug": False,
         "format": "tag",
-        "name": "",
-        "release": "",
+        "name": None,
+        "release": None,
         "package": "",
         "system": False,
     }
 
     raw_args = parser.parse_args(argv[1:])
     args = {key: value for key, value in vars(raw_args).items() if value}
     args = ChainMap(args, defaults)
 
     # Validate CLI parameters
 
     if args["distro"] == "":
         print("[ERROR] distro type must be specified.")
         return -1
-    elif args["name"] == "":
-        print("[ERROR] distro name must be specified.")
-        return -1
-    elif args["release"] == "":
+    elif args["name"] is not None and args["release"] is None:
         print("[ERROR] distro release must be specified.")
         return -1
+    elif args["name"] is None and args["release"] is not None:
+        print("[ERROR] distro name must be specified.")
+        return -1
     elif args["input_file"] == "" and args["package"] == "" and not args["system"]:
         print("[ERROR] distro file or package name must be specified.")
         return -1
+    elif args["input_file"] != "" and args["name"] is None and args["release"] is None:
+        print("[ERROR] distro name and release must be specified.")
+        return -1
 
     # Ensure format is aligned with type of SBOM
     bom_format = args["format"]
     if args["sbom"] != "spdx" and bom_format in ["tag", "yaml"]:
         # Only json format valid for CycloneDX
         bom_format = "json"
 
@@ -237,15 +240,16 @@
         )
         sbom_gen.generate(
             project_name=sbom_build.get_parent(),
             sbom_data=distro_sbom.get_sbom(),
             filename=args["output_file"],
         )
     else:
-        print(f"[ERROR] Unable to locate package {args['package']}")
+        if args["package"] != "":
+            print(f"[ERROR] Unable to locate package {args['package']}")
         return -1
 
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

## distro2sbom/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.3.0"
+VERSION: str = "0.4.0"
```

## distro2sbom/distrobuilder/distrobuilder.py

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
 import re
 import subprocess
 import unicodedata
+from pathlib import Path
 
 
 class DistroBuilder:
     def __init__(self, debug=False):
         self.sbom_packages = {}
         self.sbom_relationships = []
         self.debug = debug
@@ -61,7 +62,21 @@
     def get_relationships(self):
         if self.debug:
             print(self.sbom_relationships)
         return self.sbom_relationships
 
     def get_parent(self):
         return self.parent
+
+    def get_system(self):
+        # Extract metadata from file
+        OS_FILE = "/etc/os-release"
+        metadata = {}
+        filePath = Path(OS_FILE)
+        # Check path exists and is a valid file
+        if filePath.exists() and filePath.is_file():
+            os_file = open(OS_FILE)
+            lines = os_file.readlines()
+            for line in lines:
+                data = line.split("=")
+                metadata[data[0].lower()] = data[1].replace('"', "").strip()
+        return metadata
```

## distro2sbom/distrobuilder/dpkgbuilder.py

```diff
@@ -14,16 +14,21 @@
 class DpkgBuilder(DistroBuilder):
     def __init__(self, name, release, debug=False):
         super().__init__(debug)
         self.sbom_package = SBOMPackage()
         self.sbom_relationship = SBOMRelationship()
         self.license = LicenseScanner()
         self.distro_packages = []
-        self.name = name.replace(" ", "-")
-        self.release = release
+        if name is None and release is None:
+            self.system_data = self.get_system()
+            self.name = self.system_data["name"].replace(" ", "-")
+            self.release = self.system_data["version_id"]
+        else:
+            self.name = name.replace(" ", "-")
+            self.release = release
         self.parent = f"Distro-{self.name}"
 
     def parse_data(self, filename):
         # Process file containing installed applications
         with open(filename) as dir_file:
             lines = dir_file.readlines()
         if len(lines) > 0:
@@ -33,15 +38,20 @@
             self.sbom_package.set_name(distro_root)
             self.sbom_package.set_version(self.release)
             self.sbom_package.set_type("operating-system")
             self.sbom_package.set_filesanalysis(False)
             license = "NOASSERTION"
             self.sbom_package.set_licensedeclared(license)
             self.sbom_package.set_licenseconcluded(license)
-            self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
+            if self.system_data.get("id") is not None:
+                self.sbom_package.set_supplier(
+                    "Organisation", self.system_data.get("id")
+                )
+            else:
+                self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             self.sbom_relationship.initialise()
             self.sbom_relationship.set_relationship(
                 self.parent, "DESCRIBES", distro_root
@@ -156,17 +166,21 @@
             if license != "NOASSERTION":
                 license_comment = (
                     "This information was automatically extracted from the package."
                 )
                 if license_text != "NOASSERTION" and license != license_text:
                     self.sbom_package.set_licensedeclared("NOASSERTION")
                     license_comment = f"{license_comment} {self.sbom_package.get_name()} declares {license_text} which is not currently a valid SPDX License identifier or expression."
+                if self.license.deprecated(license):
+                    license_comment = f"{license_comment} {license} is now deprecated."
                 self.sbom_package.set_licensecomments(license_comment)
             elif license_text != "NOASSERTION":
                 license_comment = f"{self.sbom_package.get_name()} declares {license_text} which is not currently a valid SPDX License identifier or expression."
+                if self.license.deprecated(license):
+                    license_comment = f"{license_comment} {license} is now deprecated."
                 self.sbom_package.set_licensecomments(license_comment)
             supplier = self.get("Maintainer")
             if len(supplier.split()) > 3:
                 self.sbom_package.set_supplier(
                     "Organization", self.format_supplier(supplier)
                 )
             elif len(supplier) > 1:
@@ -181,17 +195,15 @@
             if len(copyright) > 0:
                 self.sbom_package.set_copyrighttext(copyright)
             # External references
             self.sbom_package.set_externalreference(
                 "PACKAGE-MANAGER", "purl", f"pkg:deb/{package}@{version}"
             )
             if len(supplier) > 1:
-                component_supplier = self.format_supplier(
-                    supplier, include_email=False
-                )
+                component_supplier = self.format_supplier(supplier, include_email=False)
                 self.sbom_package.set_externalreference(
                     "SECURITY",
                     "cpe23Type",
                     f"cpe:2.3:a:{component_supplier.replace(' ', '_').lower()}:{package}:{version}:*:*:*:*:*:*:*",
                 )
             # Store package data
             self.sbom_packages[
@@ -233,24 +245,29 @@
         self.sbom_package.set_name(distro_root)
         self.sbom_package.set_version(self.release)
         self.sbom_package.set_type("operating-system")
         self.sbom_package.set_filesanalysis(False)
         license = "NOASSERTION"
         self.sbom_package.set_licensedeclared(license)
         self.sbom_package.set_licenseconcluded(license)
-        self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
+        if self.system_data.get("home_url") is not None:
+            self.sbom_package.set_homepage(self.system_data.get("home_url"))
+        if self.system_data.get("id") is not None:
+            self.sbom_package.set_supplier("Organisation", self.system_data.get("id"))
+        else:
+            self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
         # Store package data
         self.sbom_packages[
             (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
         ] = self.sbom_package.get_package()
         self.sbom_relationship.initialise()
         self.sbom_relationship.set_relationship(self.parent, "DESCRIBES", distro_root)
         self.sbom_relationships.append(self.sbom_relationship.get_relationship())
         # Get installed packages
-        out = self.run_program(f"dpkg -l")
+        out = self.run_program("dpkg -l")
         for line in out:
             if line[:2] == "ii":
                 # For each installed package
                 line_element = re.sub(" +", " ", line[2:].strip().rstrip("\n")).split(
                     " "
                 )
                 module_name = line_element[0]
```

## distro2sbom/distrobuilder/rpmbuilder.py

```diff
@@ -14,16 +14,21 @@
 class RpmBuilder(DistroBuilder):
     def __init__(self, name, release, debug=False):
         super().__init__(debug)
         self.sbom_package = SBOMPackage()
         self.sbom_relationship = SBOMRelationship()
         self.license = LicenseScanner()
         self.distro_packages = []
-        self.name = name.replace(" ", "-")
-        self.release = release
+        if name is None and release is None:
+            self.system_data = self.get_system()
+            self.name = self.system_data["name"].replace(" ", "-")
+            self.release = self.system_data["version_id"]
+        else:
+            self.name = name.replace(" ", "-")
+            self.release = release
         self.parent = f"Distro-{self.name}"
 
     def get_data(self):
         pass
 
     def parse_data(self, filename):
         # Process file containing installed applications
@@ -36,15 +41,20 @@
             self.sbom_package.set_name(distro_root)
             self.sbom_package.set_version(self.release)
             self.sbom_package.set_type("operating-system")
             self.sbom_package.set_filesanalysis(False)
             license = "NOASSERTION"
             self.sbom_package.set_licensedeclared(license)
             self.sbom_package.set_licenseconcluded(license)
-            self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
+            if self.system_data.get("id") is not None:
+                self.sbom_package.set_supplier(
+                    "Organisation", self.system_data.get("id")
+                )
+            else:
+                self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             self.sbom_relationship.initialise()
             self.sbom_relationship.set_relationship(
                 self.parent, "DESCRIBES", distro_root
@@ -148,27 +158,43 @@
             package = self.get("Name")
             version = self.get("Version")
             if parent == "-":
                 self.sbom_package.set_type("application")
             self.sbom_package.set_name(package)
             self.sbom_package.set_version(version)
             self.sbom_package.set_filesanalysis(False)
-            license = self.license.find_license(self.get("License"))
+            license_text = self.get("License")
+            license = self.license.find_license(license_text)
             # Report license as reported by metadata. If not valid SPDX, report NOASSERTION
-            if license != self.get("License"):
+            if license != license_text:
                 self.sbom_package.set_licensedeclared("NOASSERTION")
             else:
                 self.sbom_package.set_licensedeclared(license)
             # Report license if valid SPDX identifier
             self.sbom_package.set_licenseconcluded(license)
             # Add comment if metadata license was modified
-            if len(self.get("License")) > 0 and license != self.get("License"):
-                self.sbom_package.set_licensecomments(
-                    f"{self.get('Name')} declares {self.get('License')} which is not currently a valid SPDX License identifier or expression."
+            # if len(license_text) > 0 and license != license_text:
+            #    self.sbom_package.set_licensecomments(
+            #        f"{self.get('Name')} declares {license_text} which is not currently a valid SPDX License identifier or expression."
+            #    )
+
+            if license != "NOASSERTION":
+                license_comment = (
+                    "This information was automatically extracted from the package."
                 )
+                if license_text != "NOASSERTION" and license != license_text:
+                    license_comment = f"{license_comment} {self.sbom_package.get_name()} declares {license_text} which is not currently a valid SPDX License identifier or expression."
+                if self.license.deprecated(license):
+                    license_comment = f"{license_comment} {license} is now deprecated."
+                self.sbom_package.set_licensecomments(license_comment)
+            elif license_text != "NOASSERTION":
+                license_comment = f"{self.sbom_package.get_name()} declares {license_text} which is not currently a valid SPDX License identifier or expression."
+                if self.license.deprecated(license):
+                    license_comment = f"{license_comment} {license} is now deprecated."
+                self.sbom_package.set_licensecomments(license_comment)
             supplier = self.get("Packager")
             if len(supplier.split()) > 3:
                 self.sbom_package.set_supplier(
                     "Organization", self.format_supplier(supplier)
                 )
             elif len(supplier) > 1:
                 self.sbom_package.set_supplier("Person", self.format_supplier(supplier))
@@ -179,17 +205,15 @@
             if self.get("URL") != "":
                 self.sbom_package.set_homepage(self.get("URL"))
             # External references
             self.sbom_package.set_externalreference(
                 "PACKAGE-MANAGER", "purl", f"pkg:rpm/{package}@{version}"
             )
             if len(supplier) > 1:
-                component_supplier = self.format_supplier(
-                    supplier, include_email=False
-                )
+                component_supplier = self.format_supplier(supplier, include_email=False)
                 self.sbom_package.set_externalreference(
                     "SECURITY",
                     "cpe23Type",
                     f"cpe:2.3:a:{component_supplier.replace(' ', '_').lower()}:{package}:{version}:*:*:*:*:*:*:*",
                 )
             # Store package data
             self.sbom_packages[
@@ -229,24 +253,29 @@
         self.sbom_package.set_name(distro_root)
         self.sbom_package.set_version(self.release)
         self.sbom_package.set_type("operating-system")
         self.sbom_package.set_filesanalysis(False)
         license = "NOASSERTION"
         self.sbom_package.set_licensedeclared(license)
         self.sbom_package.set_licenseconcluded(license)
-        self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
+        if self.system_data.get("home_url") is not None:
+            self.sbom_package.set_homepage(self.system_data.get("home_url"))
+        if self.system_data.get("id") is not None:
+            self.sbom_package.set_supplier("Organisation", self.system_data.get("id"))
+        else:
+            self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
         # Store package data
         self.sbom_packages[
             (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
         ] = self.sbom_package.get_package()
         self.sbom_relationship.initialise()
         self.sbom_relationship.set_relationship(self.parent, "DESCRIBES", distro_root)
         self.sbom_relationships.append(self.sbom_relationship.get_relationship())
         # Get installed packages
-        out = self.run_program(f"rpm -qa")
+        out = self.run_program("rpm -qa")
         for line in out:
             # Parse line PRODUCT-VERSION[-Other]?. If pattern not followed ignore...
             item = os.path.splitext(os.path.basename(line.strip().rstrip("\n")))[
                 0
             ].lower()
             # Version assumed to start with digit.
             product_version = re.search(r"-\d[.\d]*[a-z0-9]*", item)
```

## distro2sbom/distrobuilder/windowsbuilder.py

```diff
@@ -1,26 +1,33 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
+import platform
 import re
 
 from lib4sbom.data.package import SBOMPackage
 from lib4sbom.data.relationship import SBOMRelationship
 
 from distro2sbom.distrobuilder.distrobuilder import DistroBuilder
 
 
 class WindowsBuilder(DistroBuilder):
     def __init__(self, name, release, debug=False):
         super().__init__(debug)
         self.sbom_package = SBOMPackage()
         self.sbom_relationship = SBOMRelationship()
         self.distro_packages = []
-        self.name = name.replace(" ", "-")
-        self.release = release
+        if name is not None:
+            self.name = name.replace(" ", "-")
+        else:
+            self.name = "Windows"
+        if release is not None:
+            self.release = release
+        else:
+            self.release = platform.version()
         self.parent = f"Distro-{self.name}"
 
     def get_data(self):
         pass
 
     def parse_data(self, filename):
         # Process product file
@@ -34,15 +41,15 @@
             self.sbom_package.initialise()
             self.sbom_package.set_name(distro_root)
             self.sbom_package.set_version(self.release)
             self.sbom_package.set_type("operating-system")
             self.sbom_package.set_filesanalysis(False)
             license = "NOASSERTION"
             self.sbom_package.set_licensedeclared(license)
-            self.sbom_package.set_supplier("Organisaiton", "Microsoft Corporation")
+            self.sbom_package.set_supplier("Organisation", "Microsoft Corporation")
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             distro_id = self.sbom_package.get_value("id")
             self.sbom_relationship.initialise()
             self.sbom_relationship.set_relationship(
@@ -91,7 +98,10 @@
                         self.sbom_relationships.append(
                             self.sbom_relationship.get_relationship()
                         )
                     metadata = {}
 
     def process_distro_package(self, module_name):
         print("[ERROR] Feature not available")
+
+    def get_system(self):
+        print("[ERROR] Feature not available")
```

## Comparing `distro2sbom-0.3.0.dist-info/LICENSE` & `distro2sbom-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `distro2sbom-0.3.0.dist-info/METADATA` & `distro2sbom-0.4.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distro2sbom
-Version: 0.3.0
+Version: 0.4.0
 Summary: SBOM generator for system distribution
 Home-page: https://github.com/anthonyharrison/distro2sbom
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
 
 # DISTRO2SBOM
 
 The DISTRO2SBOM generates a
 SBOM (Software Bill of Materials) for either an installed application or a complete system installation in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
 An SBOM for an installed package will identify all of its dependent components.
@@ -88,15 +88,16 @@
 ```
 						
 ## Operation
 
 The `--distro` option is used to identify the type of distribution. The auto option attempts to determine the type of distribution by searching for the
 presence of key applications required by the tool. If none of the required applications are found, the tool terminates. This option is mandatory.
 
-The `--name` option and `--release` option is used to identify the name and release of the distribution. These options are both mandatory.
+The `--name` option and `--release` option is used to identify the name and release of the distribution. These options are mandatory if the `--input-file` option is specified otherwise
+they are optional but if they are specified, values for both options are required. If they are not specified, values for these options shall be obtained from system files installed on the system.
 
 The `--input-file` option is used to provide a filename containing the list of packages installed on the system. The format of the file is dependent on the specified `--distro` option.
 
 - deb. The file used is the output of the following command
     ```bash
     dpkg -l > [filename.out]
     ```
@@ -182,18 +183,18 @@
 distro2sbom --distro deb --name <distro name> --release <distro release> --input-file <distrofile> --sbom cyclonedx --output-file <distrooutfile>
 ```
 
 This will generate an SBOM in CycloneDX JSON value for a distribution file in dpkg format (indicated by the 'deb' option)
 
 ### SBOM for System
 
-To generate an SBOM for an installed system.
+To generate an SBOM for an installed system, obtaining the name and release of the system from installed system files.
 
 ```bash
-distro2sbom --distro rpm --name <distro name> --release <distro release> --system --format json --output-file <distrooutfile>
+distro2sbom --distro deb --system --format json --output-file <distrooutfile>
 ```
 
 This will generate an SBOM in SPDX JSON value for a distribution file in dpkg format (indicated by the 'deb' option)
 
 ## Licence
 
 Licenced under the Apache 2.0 Licence.
```

## Comparing `distro2sbom-0.3.0.dist-info/RECORD` & `distro2sbom-0.4.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 distro2sbom/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-distro2sbom/cli.py,sha256=S3prwgydyg56adp3FwA6xJDrGBn8pK2njbI-RlzjlnM,7510
-distro2sbom/version.py,sha256=_p-y2a7gEF6oU37vmbGAsqrCSIpyaZoCAugkrzEBDQI,100
+distro2sbom/cli.py,sha256=aFufBnuW3KlmstXthdU1OcdSdkzSURbrG6yatQKndsE,7791
+distro2sbom/test.py,sha256=m8yYYiZq9QUIqcNAKQOGPvboIvnZ8WrZUH2ELMm4c4E,462
+distro2sbom/version.py,sha256=7JpTeIdgA2tX24hrLXHM3T788cSCK36qgBVFqIuHxgo,100
 distro2sbom/distrobuilder/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-distro2sbom/distrobuilder/distrobuilder.py,sha256=PELdB9OP0hoZhSUr0XN5pIn31nwm04glPqoGBRNhGJ4,2582
-distro2sbom/distrobuilder/dpkgbuilder.py,sha256=w5-bA8BEHHVBXORHvTNy9XPt3kXp_reK4zp0aQlRwDE,12435
-distro2sbom/distrobuilder/rpmbuilder.py,sha256=73pXNBgJ7HhBci-0o72affoSv6yZNT0IAvRbS8eGIGk,12251
-distro2sbom/distrobuilder/windowsbuilder.py,sha256=4_qlVL3hD_KW42iEhKoP_N1YF6YL5UJ7uq6uXYwwk_0,4421
-distro2sbom-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-distro2sbom-0.3.0.dist-info/METADATA,sha256=6kkEOh6LywuQKpcLkOVAGy0nrQpItZ_YsrMUC_GOKqc,10305
-distro2sbom-0.3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-distro2sbom-0.3.0.dist-info/entry_points.txt,sha256=r5RioA3bp_Kbd1UJ5L1BTfSea9qEISrGmoSKSAHFBOU,53
-distro2sbom-0.3.0.dist-info/top_level.txt,sha256=wj3FBpfTya_uiJ4egUDQ4vv-BO5G5swycPOUc7qymJM,12
-distro2sbom-0.3.0.dist-info/RECORD,,
+distro2sbom/distrobuilder/distrobuilder.py,sha256=MS-GkWh7LQUrMbxhEtGaK8J8IEzWMfeOOjC2HhT6lak,3110
+distro2sbom/distrobuilder/dpkgbuilder.py,sha256=L4dk2gbsR6pBOXGNuJvFKStCI0nxNVVDXut56oQMm3A,13415
+distro2sbom/distrobuilder/rpmbuilder.py,sha256=GShGjAx_dqkhA-im8ic5mKPixtW9-Ax3KE7Z-cssDb8,14043
+distro2sbom/distrobuilder/windowsbuilder.py,sha256=P-1xTEqHZHTEGobkbycf_Wgfa2KhlPRx5MqKVcQPLFY,4688
+distro2sbom-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+distro2sbom-0.4.0.dist-info/METADATA,sha256=r6FdSn6SwC5pZT0DK7xZ6xxdlPac5GholPMSEwb072g,10573
+distro2sbom-0.4.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+distro2sbom-0.4.0.dist-info/entry_points.txt,sha256=r5RioA3bp_Kbd1UJ5L1BTfSea9qEISrGmoSKSAHFBOU,53
+distro2sbom-0.4.0.dist-info/top_level.txt,sha256=wj3FBpfTya_uiJ4egUDQ4vv-BO5G5swycPOUc7qymJM,12
+distro2sbom-0.4.0.dist-info/RECORD,,
```

