# Comparing `tmp/protoc-gen-pyproject-0.3.0.tar.gz` & `tmp/protoc-gen-pyproject-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protoc-gen-pyproject-0.3.0.tar", last modified: Mon Jul 24 13:42:29 2023, max compression
+gzip compressed data, was "protoc-gen-pyproject-0.3.1.tar", last modified: Mon Jul 24 14:00:57 2023, max compression
```

## Comparing `protoc-gen-pyproject-0.3.0.tar` & `protoc-gen-pyproject-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 13:42:29.004672 protoc-gen-pyproject-0.3.0/
--rw-r--r--   0 john      (1000) users      (100)    11357 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/LICENSE
--rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 13:42:29.004672 protoc-gen-pyproject-0.3.0/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      547 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/README.md
-drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 13:42:29.003672 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/
--rw-r--r--   0 john      (1000) users      (100)       23 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/__init__.py
--rw-r--r--   0 john      (1000) users      (100)       32 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/__main__.py
--rw-r--r--   0 john      (1000) users      (100)      552 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/main.py
--rw-r--r--   0 john      (1000) users      (100)     2847 2023-07-24 13:37:54.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/parser.py
-drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 13:42:29.004672 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/
--rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      424 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) users      (100)        1 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) users      (100)       67 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) users      (100)       45 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/requires.txt
--rw-r--r--   0 john      (1000) users      (100)       21 2023-07-24 13:42:29.000000 protoc-gen-pyproject-0.3.0/protoc_gen_pyproject.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) users      (100)      267 2023-07-24 13:35:58.000000 protoc-gen-pyproject-0.3.0/pyproject.toml
--rw-r--r--   0 john      (1000) users      (100)       38 2023-07-24 13:42:29.004672 protoc-gen-pyproject-0.3.0/setup.cfg
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:00:57.442136 protoc-gen-pyproject-0.3.1/
+-rw-r--r--   0 john      (1000) users      (100)    11357 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/LICENSE
+-rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 14:00:57.442136 protoc-gen-pyproject-0.3.1/PKG-INFO
+-rw-r--r--   0 john      (1000) users      (100)      547 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/README.md
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:00:57.441136 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/
+-rw-r--r--   0 john      (1000) users      (100)       23 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/__init__.py
+-rw-r--r--   0 john      (1000) users      (100)       32 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/__main__.py
+-rw-r--r--   0 john      (1000) users      (100)      552 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/main.py
+-rw-r--r--   0 john      (1000) users      (100)     3024 2023-07-24 13:58:56.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/parser.py
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:00:57.441136 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/
+-rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) users      (100)      424 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) users      (100)        1 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) users      (100)       67 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) users      (100)       45 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) users      (100)       21 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/top_level.txt
+-rw-r--r--   0 john      (1000) users      (100)      267 2023-07-24 13:59:24.000000 protoc-gen-pyproject-0.3.1/pyproject.toml
+-rw-r--r--   0 john      (1000) users      (100)       38 2023-07-24 14:00:57.442136 protoc-gen-pyproject-0.3.1/setup.cfg
```

### Comparing `protoc-gen-pyproject-0.3.0/LICENSE` & `protoc-gen-pyproject-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.3.0/README.md` & `protoc-gen-pyproject-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/main.py` & `protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/main.py`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.3.0/protoc_gen_pyproject/parser.py` & `protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import TypedDict
 
 import toml
 import dunamai
 from betterproto.lib.google.protobuf.compiler import (
     CodeGeneratorRequest,
     CodeGeneratorResponse,
+    CodeGeneratorResponseFeature,
     CodeGeneratorResponseFile,
 )
 
 PARAM_REGEX = re.compile(
     r"(?:(?P<param>[^,=]+)(?:=(?P<key>[^,=]+)(?:=(?P<value>(?:[^,\\]|\\,|\\\\)+))?)?)"
 )
 
@@ -48,48 +49,51 @@
 
 def generate_code(request: CodeGeneratorRequest) -> CodeGeneratorResponse:
     """Create a response to generate the project file.
 
     Will look at the `gen_project` parameter if set to decide which
     file to use.
     """
+    response = CodeGeneratorResponse()
+    response.supported_features = CodeGeneratorResponseFeature.FEATURE_PROTO3_OPTIONAL
+
     params = parse_params(request.parameter)
 
     file_path = "pyproject.toml"
     generate_pyproject_param = params.get("gen_pyproject")
     if generate_pyproject_param is not None:
         file_path = generate_pyproject_param["key"]
 
     if not os.path.exists(file_path):
-        return CodeGeneratorResponse(error=f"No project file found at '{file_path}'")
+        response.error = f"No project file found at '{file_path}'"
+        return response
 
     file_content = None
     with open(file=file_path) as f:
         file_content = f.read()
 
     # Automatically set package version if configured to do so.
     set_version_from_vcs = params.get("set_version_from_vcs")
-    if set_version_from_vcs is not None:
+    if set_version_from_vcs is not None and set_version_from_vcs["key"] == "True":
         pyproject_toml = toml.loads(file_content)
-        pyproject_toml["version"] = dunamai.Version.from_any_vcs()
+        pyproject_toml["version"] = dunamai.Version.from_any_vcs().serialize()
         file_content = toml.dumps(pyproject_toml)
 
     files = [CodeGeneratorResponseFile(name="pyproject.toml", content=file_content)]
 
     include_py_typed = params.get("include_py_typed")
     if include_py_typed is None or (
         include_py_typed is not None and include_py_typed["key"] != "False"
     ):
         package_name = params.get("package_name")
         if package_name is None:
-            return CodeGeneratorResponse(
-                error=f"package_name must be set if `include_py_typed` is True."
-            )
+            response.error = f"package_name must be set if `include_py_typed` is True."
+            return response
 
         files.append(
             CodeGeneratorResponseFile(
                 name=str(Path(package_name["key"]) / "py.typed"), content=""
             )
         )
 
-    response = CodeGeneratorResponse(file=files)
+    response.files = files
     return response
```

