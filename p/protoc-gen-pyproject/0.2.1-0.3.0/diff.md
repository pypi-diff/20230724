# Comparing `tmp/protoc-gen-pyproject-0.2.1.tar.gz` & `tmp/protoc-gen-pyproject-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protoc-gen-pyproject-0.2.1.tar", last modified: Fri Nov 11 09:53:50 2022, max compression
+gzip compressed data, was "protoc-gen-pyproject-0.3.0.tar", last modified: Mon Jul 24 13:42:29 2023, max compression
```

## Comparing `protoc-gen-pyproject-0.2.1.tar` & `protoc-gen-pyproject-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 john      (1000) users      (100)        0 2022-11-11 09:53:50.748653 protoc-gen-pyproject-0.2.1/
--rw-r--r--   0 john      (1000) users      (100)    11357 2022-10-21 11:11:45.000000 protoc-gen-pyproject-0.2.1/LICENSE
--rw-r--r--   0 john      (1000) users      (100)      108 2022-11-11 09:53:50.748653 protoc-gen-pyproject-0.2.1/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      547 2022-10-21 11:11:45.000000 protoc-gen-pyproject-0.2.1/README.md
-drwxr-xr-x   0 john      (1000) users      (100)        0 2022-11-11 09:53:50.748653 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject/
--rw-r--r--   0 john      (1000) users      (100)       23 2022-10-21 11:11:45.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject/__init__.py
--rw-r--r--   0 john      (1000) users      (100)       32 2022-10-21 11:11:45.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject/__main__.py
--rw-r--r--   0 john      (1000) users      (100)      552 2022-10-21 11:11:45.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject/main.py
--rw-r--r--   0 john      (1000) users      (100)     2491 2022-11-11 09:48:59.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject/parser.py
-drwxr-xr-x   0 john      (1000) users      (100)        0 2022-11-11 09:53:50.748653 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject.egg-info/
--rw-r--r--   0 john      (1000) users      (100)      108 2022-11-11 09:53:50.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      424 2022-11-11 09:53:50.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) users      (100)        1 2022-11-11 09:53:50.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) users      (100)       67 2022-11-11 09:53:50.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) users      (100)       21 2022-11-11 09:53:50.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject.egg-info/requires.txt
--rw-r--r--   0 john      (1000) users      (100)       21 2022-11-11 09:53:50.000000 protoc-gen-pyproject-0.2.1/protoc_gen_pyproject.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) users      (100)      233 2022-11-11 09:52:16.000000 protoc-gen-pyproject-0.2.1/pyproject.toml
--rw-r--r--   0 john      (1000) users      (100)       38 2022-11-11 09:53:50.749653 protoc-gen-pyproject-0.2.1/setup.cfg
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 13:42:29.004672 protoc-gen-pyproject-0.3.0/
+-rw-r--r--   0 john      (1000) users      (100)    11357 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/LICENSE
+-rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 13:42:29.004672 protoc-gen-pyproject-0.3.0/PKG-INFO
+-rw-r--r--   0 john      (1000) users      (100)      547 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/README.md
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 13:42:29.003672 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/
+-rw-r--r--   0 john      (1000) users      (100)       23 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/__init__.py
+-rw-r--r--   0 john      (1000) users      (100)       32 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/__main__.py
+-rw-r--r--   0 john      (1000) users      (100)      552 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/main.py
+-rw-r--r--   0 john      (1000) users      (100)     2847 2023-07-24 13:37:54.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/parser.py
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 13:42:29.004672 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/
+-rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) users      (100)      424 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) users      (100)        1 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) users      (100)       67 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) users      (100)       45 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) users      (100)       21 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/top_level.txt
+-rw-r--r--   0 john      (1000) users      (100)      267 2023-07-24 13:35:58.000000 protoc-gen-pyproject-0.3.0/pyproject.toml
+-rw-r--r--   0 john      (1000) users      (100)       38 2023-07-24 13:42:29.004672 protoc-gen-pyproject-0.3.0/setup.cfg
```

### Comparing `protoc-gen-pyproject-0.2.1/LICENSE` & `protoc-gen-pyproject-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.2.1/README.md` & `protoc-gen-pyproject-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.2.1/protoc_gen_pyproject/main.py` & `protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/main.py`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.2.1/protoc_gen_pyproject/parser.py` & `protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os.path
 import re
 from pathlib import Path
-from typing import TypedDict, cast
+from typing import TypedDict
 
+import toml
+import dunamai
 from betterproto.lib.google.protobuf.compiler import (
     CodeGeneratorRequest,
     CodeGeneratorResponse,
     CodeGeneratorResponseFile,
 )
 
 PARAM_REGEX = re.compile(
@@ -60,14 +62,21 @@
     if not os.path.exists(file_path):
         return CodeGeneratorResponse(error=f"No project file found at '{file_path}'")
 
     file_content = None
     with open(file=file_path) as f:
         file_content = f.read()
 
+    # Automatically set package version if configured to do so.
+    set_version_from_vcs = params.get("set_version_from_vcs")
+    if set_version_from_vcs is not None:
+        pyproject_toml = toml.loads(file_content)
+        pyproject_toml["version"] = dunamai.Version.from_any_vcs()
+        file_content = toml.dumps(pyproject_toml)
+
     files = [CodeGeneratorResponseFile(name="pyproject.toml", content=file_content)]
 
     include_py_typed = params.get("include_py_typed")
     if include_py_typed is None or (
         include_py_typed is not None and include_py_typed["key"] != "False"
     ):
         package_name = params.get("package_name")
```

