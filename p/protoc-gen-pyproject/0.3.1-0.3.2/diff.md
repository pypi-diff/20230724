# Comparing `tmp/protoc-gen-pyproject-0.3.1.tar.gz` & `tmp/protoc-gen-pyproject-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protoc-gen-pyproject-0.3.1.tar", last modified: Mon Jul 24 14:00:57 2023, max compression
+gzip compressed data, was "protoc-gen-pyproject-0.3.2.tar", last modified: Mon Jul 24 14:18:04 2023, max compression
```

## Comparing `protoc-gen-pyproject-0.3.1.tar` & `protoc-gen-pyproject-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:00:57.442136 protoc-gen-pyproject-0.3.1/
--rw-r--r--   0 john      (1000) users      (100)    11357 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/LICENSE
--rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 14:00:57.442136 protoc-gen-pyproject-0.3.1/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      547 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/README.md
-drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:00:57.441136 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/
--rw-r--r--   0 john      (1000) users      (100)       23 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/__init__.py
--rw-r--r--   0 john      (1000) users      (100)       32 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/__main__.py
--rw-r--r--   0 john      (1000) users      (100)      552 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/main.py
--rw-r--r--   0 john      (1000) users      (100)     3024 2023-07-24 13:58:56.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/parser.py
-drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:00:57.441136 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/
--rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      424 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) users      (100)        1 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) users      (100)       67 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) users      (100)       45 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/requires.txt
--rw-r--r--   0 john      (1000) users      (100)       21 2023-07-24 14:00:57.000000 protoc-gen-pyproject-0.3.1/protoc_gen_pyproject.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) users      (100)      267 2023-07-24 13:59:24.000000 protoc-gen-pyproject-0.3.1/pyproject.toml
--rw-r--r--   0 john      (1000) users      (100)       38 2023-07-24 14:00:57.442136 protoc-gen-pyproject-0.3.1/setup.cfg
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:18:04.582641 protoc-gen-pyproject-0.3.2/
+-rw-r--r--   0 john      (1000) users      (100)    11357 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.2/LICENSE
+-rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 14:18:04.582641 protoc-gen-pyproject-0.3.2/PKG-INFO
+-rw-r--r--   0 john      (1000) users      (100)      547 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.2/README.md
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:18:04.582641 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject/
+-rw-r--r--   0 john      (1000) users      (100)       23 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject/__init__.py
+-rw-r--r--   0 john      (1000) users      (100)       32 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject/__main__.py
+-rw-r--r--   0 john      (1000) users      (100)      552 2023-07-24 13:30:52.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject/main.py
+-rw-r--r--   0 john      (1000) users      (100)     3023 2023-07-24 14:16:40.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject/parser.py
+drwxr-xr-x   0 john      (1000) users      (100)        0 2023-07-24 14:18:04.582641 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject.egg-info/
+-rw-r--r--   0 john      (1000) users      (100)      108 2023-07-24 14:18:04.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) users      (100)      424 2023-07-24 14:18:04.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) users      (100)        1 2023-07-24 14:18:04.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) users      (100)       67 2023-07-24 14:18:04.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) users      (100)       45 2023-07-24 14:18:04.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) users      (100)       21 2023-07-24 14:18:04.000000 protoc-gen-pyproject-0.3.2/protoc_gen_pyproject.egg-info/top_level.txt
+-rw-r--r--   0 john      (1000) users      (100)      267 2023-07-24 14:17:14.000000 protoc-gen-pyproject-0.3.2/pyproject.toml
+-rw-r--r--   0 john      (1000) users      (100)       38 2023-07-24 14:18:04.582641 protoc-gen-pyproject-0.3.2/setup.cfg
```

### Comparing `protoc-gen-pyproject-0.3.1/LICENSE` & `protoc-gen-pyproject-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.3.1/README.md` & `protoc-gen-pyproject-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/main.py` & `protoc-gen-pyproject-0.3.2/protoc_gen_pyproject/main.py`

 * *Files identical despite different names*

### Comparing `protoc-gen-pyproject-0.3.1/protoc_gen_pyproject/parser.py` & `protoc-gen-pyproject-0.3.2/protoc_gen_pyproject/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,9 +91,9 @@
 
         files.append(
             CodeGeneratorResponseFile(
                 name=str(Path(package_name["key"]) / "py.typed"), content=""
             )
         )
 
-    response.files = files
+    response.file = files
     return response
```

