# Comparing `tmp/empack-3.0.1.tar.gz` & `tmp/empack-3.1.0.tar.gz`

## Comparing `empack-3.0.1.tar` & `empack-3.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 empack-3.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.0.1/ci_env.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.0.1/setup.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 empack-3.0.1/config/empack_config.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.0.1/empack/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 empack-3.0.1/empack/file_patterns.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 empack-3.0.1/empack/filter_env.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.0.1/empack/micromamba_wrapper.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 empack-3.0.1/empack/pack.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.0.1/empack/repodata.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.0.1/empack/tar_utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.0.1/empack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/app.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/err.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/main.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/pack.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/repodata.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.0.1/tests/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.0.1/tests/conftest.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.0.1/tests/empack_test_config.yaml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.0.1/tests/empack_test_extra_config.yaml
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 empack-3.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 empack-3.0.1/tests/test_filter.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.0.1/tests/test_integration.py
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 empack-3.0.1/tests/test_pack.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.0.1/LICENSE
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.0.1/README.md
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 empack-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 empack-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 empack-3.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.1.0/ci_env.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.1.0/setup.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 empack-3.1.0/config/empack_config.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.1.0/empack/__init__.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 empack-3.1.0/empack/file_patterns.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 empack-3.1.0/empack/filter_env.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.1.0/empack/micromamba_wrapper.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 empack-3.1.0/empack/pack.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.1.0/empack/repodata.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.1.0/empack/tar_utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.1.0/empack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/app.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/err.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/main.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/pack.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/repodata.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.1.0/tests/empack_test_config.yaml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.1.0/tests/empack_test_extra_config.yaml
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 empack-3.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 empack-3.1.0/tests/test_filter.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.1.0/tests/test_integration.py
+-rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 empack-3.1.0/tests/test_pack.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.1.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.1.0/LICENSE
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.1.0/README.md
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 empack-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 empack-3.1.0/PKG-INFO
```

### Comparing `empack-3.0.1/.pre-commit-config.yaml` & `empack-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/config/empack_config.yaml` & `empack-3.1.0/config/empack_config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/empack/file_patterns.py` & `empack-3.1.0/empack/file_patterns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import fnmatch
 import re
-from typing import Optional
+from typing import Optional, Union
 
 import yaml
 from pydantic import BaseModel, Field, PrivateAttr, RootModel
 
 
 class FilePatternsModelBase(BaseModel, extra="forbid"):
     pass
@@ -27,15 +27,15 @@
     pattern: str
 
     def match(self, path):
         return fnmatch.fnmatch(path, self.pattern)
 
 
 class FilePattern(RootModel, extra="forbid"):
-    root: RegexPattern | UnixPattern
+    root: Union[RegexPattern, UnixPattern]
 
     def match(self, path):
         return self.root.match(path)
 
 
 class FileFilter(BaseModel, extra="forbid"):
     include_patterns: list[FilePattern] = Field(default_factory=list)
@@ -51,15 +51,15 @@
                 if ep.match(path):
                     return False
 
         return include
 
 
 class PkgFileFilter(BaseModel, extra="forbid"):
-    packages: dict[str, FileFilter | list[FileFilter]]
+    packages: dict[str, Union[FileFilter, list[FileFilter]]]
     default: FileFilter
 
     def get_filter_for_pkg(self, pkg_name):
         return self.packages.get(pkg_name, self.default)
 
     def get_filters_for_pkg(self, pkg_name):
         matchers = self.get_filter_for_pkg(pkg_name)
@@ -76,15 +76,15 @@
                 self.packages[pkg_name] = filters
 
 
 # when multiple config files are provided, the default
 # must be optional for the additional configs, otherwise
 # the would always overwrite the main default config
 class AdditionalPkgFileFilter(BaseModel, extra="forbid"):
-    packages: dict[str, FileFilter | list[FileFilter]]
+    packages: dict[str, Union[FileFilter, list[FileFilter]]]
     default: Optional[FileFilter] = None
 
 
 def pkg_file_filter_from_yaml(path, *extra_path):
     with open(path) as pack_config_file:
         pack_config = yaml.safe_load(pack_config_file)
         pkg_file_filter = PkgFileFilter.model_validate(pack_config)
```

### Comparing `empack-3.0.1/empack/filter_env.py` & `empack-3.1.0/empack/filter_env.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,78 @@
+import csv
 import glob
 import json
 import os
 import shutil
 from pathlib import Path
 
 
+def iterate_pip_pkg_record(env_prefix):
+    # Find all RECORD files for .dist-info folders for which INSTALLER is "pip"
+    # Resolve site-packages directory, ignoring the python3.1/ symlink
+    site_packages = [
+        site_package
+        for site_package in Path(env_prefix).resolve().glob("lib/python*/site-packages")
+        if "python3.1" not in site_package.parts
+    ]
+    if not site_packages:
+        return []
+    site_packages = site_packages[0]
+    relative_site_packages = site_packages.relative_to(env_prefix)
+
+    packages_dist_info = Path(site_packages).resolve().glob("*.dist-info")
+
+    for dist_info in packages_dist_info:
+        if not (dist_info / "INSTALLER").exists():
+            continue
+
+        # Continue if package not installed with pip
+        with open(dist_info / "INSTALLER") as installer:
+            if installer.read().strip() != "pip":
+                continue
+
+        # Fetch package name
+        package_name, package_version = dist_info.name.removesuffix(".dist-info").split("-")
+
+        # Find all files
+        with open(dist_info / "RECORD") as record:
+            files = csv.reader(record)
+            all_files = [_file[0] for _file in files]
+            all_files_paths = [
+                relative_site_packages / _file
+                for _file in all_files
+                # Excluding .dist-info files
+                if ".dist-info" not in _file
+            ]
+
+        yield dict(
+            name=package_name,
+            version=package_version,
+            files=all_files_paths,
+            # Some hugly hacks to make it work...
+            fn=f"{package_name}-{package_version}",
+            build="pip",
+            build_number=0,
+            depends=[],
+        )
+
+
 def iterate_env_pkg_meta(env_prefix):
     meta_dir = os.path.join(env_prefix, "conda-meta")
     pkg_meta_files = glob.glob(os.path.join(meta_dir, "*.json"))
+
     for p in pkg_meta_files:
         with open(p) as pkg_meta_file:
             pkg_meta = json.load(pkg_meta_file)
             yield pkg_meta
 
+    # Iterate through pip installed packages and get mock pkg_meta
+    for pkg_meta in iterate_pip_pkg_record(env_prefix):
+        yield pkg_meta
+
 
 def write_minimal_conda_meta(pkg_meta, env_prefix):
     content = {k: pkg_meta[k] for k in ["name", "version", "build", "build_number"]}
     conda_meta_dir = Path(env_prefix) / "conda-meta"
     conda_meta_dir.mkdir(parents=True, exist_ok=True)
 
     filename = f"{pkg_meta['name']}-{pkg_meta['version']}-{pkg_meta['build']}.json"
```

### Comparing `empack-3.0.1/empack/micromamba_wrapper.py` & `empack-3.1.0/empack/micromamba_wrapper.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/empack/pack.py` & `empack-3.1.0/empack/pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/empack/repodata.py` & `empack-3.1.0/empack/repodata.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/empack/tar_utils.py` & `empack-3.1.0/empack/tar_utils.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/empack/cli/pack.py` & `empack-3.1.0/empack/cli/pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/empack/cli/repodata.py` & `empack-3.1.0/empack/cli/repodata.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/tests/conftest.py` & `empack-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/tests/empack_test_config.yaml` & `empack-3.1.0/tests/empack_test_config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/tests/test_cli.py` & `empack-3.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/tests/test_filter.py` & `empack-3.1.0/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/tests/test_integration.py` & `empack-3.1.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/tests/test_pack.py` & `empack-3.1.0/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/.gitignore` & `empack-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/LICENSE` & `empack-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/README.md` & `empack-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/pyproject.toml` & `empack-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empack-3.0.1/PKG-INFO` & `empack-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empack
-Version: 3.0.1
+Version: 3.1.0
 Summary: empack emscripten+boa
 Project-URL: Homepage, https://github.com/emscripten-forge/empack
 Author-email: Thorsten Beier <derthorstenbeier@gmail.com>
 License: 
         MIT License
         
         Copyright (c) 2022, Thorsten Beier
```

