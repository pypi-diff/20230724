# Comparing `tmp/flict-1.1.0.tar.gz` & `tmp/flict-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flict-1.1.0.tar", last modified: Tue Jul 18 06:26:57 2023, max compression
+gzip compressed data, was "flict-1.1.1.tar", last modified: Mon Jul 24 03:51:13 2023, max compression
```

## Comparing `flict-1.1.0.tar` & `flict-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 06:26:33.000000 flict-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 06:26:33.000000 flict-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-18 06:26:57.326307 flict-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-18 06:26:33.000000 flict-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 06:26:33.000000 flict-1.1.0/flict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-07-18 06:26:33.000000 flict-1.1.0/flict/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/flictlib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-18 06:26:57.000000 flict-1.1.0/flict/flictlib/flict_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/flictlib/format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/dot_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/json_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/markdown_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/text_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/lic_comp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/license_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/flictlib/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/project/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-18 06:26:33.000000 flict-1.1.0/flict/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/var/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-18 06:26:33.000000 flict-1.1.0/flict/var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-18 06:26:33.000000 flict-1.1.0/flict/var/alias.json
--rw-r--r--   0 runner    (1001) docker     (123)   457966 2023-07-18 06:26:33.000000 flict-1.1.0/flict/var/scancode-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-18 06:26:33.000000 flict-1.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 06:26:33.000000 flict-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 06:26:57.330307 flict-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-18 06:26:33.000000 flict-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:51:13.678804 flict-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 03:50:51.000000 flict-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-24 03:50:51.000000 flict-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-24 03:51:13.678804 flict-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-24 03:50:51.000000 flict-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:51:13.674804 flict-1.1.1/flict/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 03:50:51.000000 flict-1.1.1/flict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-07-24 03:50:51.000000 flict-1.1.1/flict/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:51:13.678804 flict-1.1.1/flict/flictlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-24 03:51:13.000000 flict-1.1.1/flict/flictlib/flict_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:51:13.678804 flict-1.1.1/flict/flictlib/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/format/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/format/dot_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/format/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/format/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/format/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/format/markdown_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/format/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/lic_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/license_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:51:13.678804 flict-1.1.1/flict/flictlib/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/project/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-24 03:50:51.000000 flict-1.1.1/flict/flictlib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-24 03:50:51.000000 flict-1.1.1/flict/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:51:13.678804 flict-1.1.1/flict/var/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-24 03:50:51.000000 flict-1.1.1/flict/var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-24 03:50:51.000000 flict-1.1.1/flict/var/alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)   457966 2023-07-24 03:50:51.000000 flict-1.1.1/flict/var/scancode-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:51:13.674804 flict-1.1.1/flict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-24 03:51:13.000000 flict-1.1.1/flict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-24 03:51:13.000000 flict-1.1.1/flict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:51:13.000000 flict-1.1.1/flict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 03:51:13.000000 flict-1.1.1/flict.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-24 03:51:13.000000 flict-1.1.1/flict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 03:51:13.000000 flict-1.1.1/flict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 03:50:51.000000 flict-1.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 03:50:51.000000 flict-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-24 03:51:13.678804 flict-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-24 03:50:51.000000 flict-1.1.1/setup.py
```

### Comparing `flict-1.1.0/LICENSE` & `flict-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/PKG-INFO` & `flict-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flict
-Version: 1.1.0
+Version: 1.1.1
 Summary: FOSS License Compatibility Tool
 Home-page: https://github.com/vinland-technology/flict
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flict-1.1.0/README.md` & `flict-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/__main__.py` & `flict-1.1.1/flict/__main__.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/alias.py` & `flict-1.1.1/flict/flictlib/alias.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/arbiter.py` & `flict-1.1.1/flict/flictlib/arbiter.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/compatibility.py` & `flict-1.1.1/flict/flictlib/compatibility.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/flict_config.py` & `flict-1.1.1/flict/flictlib/flict_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         except Exception:  # noqa: S110 - it's okay ignore all errors here
             pass
     return {}
 
 
 _userconfig = read_user_config()
 
-flict_version = "1.1.0"
+flict_version = "1.1.1"
 
 SCRIPT_DIR = os.path.realpath(os.path.join(os.path.dirname(os.path.realpath(__file__)), "../"))
 
 VAR_DIR = os.path.join(SCRIPT_DIR, "var")
 
 BUILTIN_ALIAS_FILE = os.path.join(VAR_DIR, "alias.json")
 DEFAULT_FLICT_ALIAS_FILE = os.path.join(VAR_DIR, BUILTIN_ALIAS_FILE)
```

### Comparing `flict-1.1.0/flict/flictlib/format/common.py` & `flict-1.1.1/flict/flictlib/format/common.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/format/dot_format.py` & `flict-1.1.1/flict/flictlib/format/dot_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/format/factory.py` & `flict-1.1.1/flict/flictlib/format/factory.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/format/format.py` & `flict-1.1.1/flict/flictlib/format/format.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/format/json_format.py` & `flict-1.1.1/flict/flictlib/format/json_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/format/markdown_format.py` & `flict-1.1.1/flict/flictlib/format/markdown_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/format/text_format.py` & `flict-1.1.1/flict/flictlib/format/text_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/lic_comp.py` & `flict-1.1.1/flict/flictlib/lic_comp.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/license.py` & `flict-1.1.1/flict/flictlib/license.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/license_parser.py` & `flict-1.1.1/flict/flictlib/license_parser.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/logger.py` & `flict-1.1.1/flict/flictlib/logger.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/project/reader.py` & `flict-1.1.1/flict/flictlib/project/reader.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/return_codes.py` & `flict-1.1.1/flict/flictlib/return_codes.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/flictlib/utils.py` & `flict-1.1.1/flict/flictlib/utils.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/impl.py` & `flict-1.1.1/flict/impl.py`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/var/alias.json` & `flict-1.1.1/flict/var/alias.json`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict/var/scancode-licenses.json` & `flict-1.1.1/flict/var/scancode-licenses.json`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict.egg-info/PKG-INFO` & `flict-1.1.1/flict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flict
-Version: 1.1.0
+Version: 1.1.1
 Summary: FOSS License Compatibility Tool
 Home-page: https://github.com/vinland-technology/flict
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flict-1.1.0/flict.egg-info/SOURCES.txt` & `flict-1.1.1/flict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flict-1.1.0/flict.egg-info/requires.txt` & `flict-1.1.1/flict.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 license-expression~=30.1
 osadl-matrix==2023.6.23.30625
-wheel~=0.40
+wheel~=0.41
 
 [dev]
 bump2version~=1.0
 dataclasses~=0.6
 dlint~=0.14
 flake8-2020~=1.8
 flake8-bandit~=4.1
@@ -35,9 +35,9 @@
 pytest-forked~=1.6
 pytest-icdiff~=0.6
 pytest-random-order~=1.1
 pytest-socket~=0.6
 pytest-sugar~=0.9
 pytest-tldr~=0.2
 pytest~=7.4
-reuse~=1.1
+reuse~=2.1
 twine~=4.0
```

### Comparing `flict-1.1.0/requirements-dev.txt` & `flict-1.1.1/requirements-dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 pytest-forked ~= 1.6
 pytest-icdiff ~= 0.6
 pytest-random-order ~= 1.1
 pytest-socket ~= 0.6
 pytest-sugar ~= 0.9
 pytest-tldr ~= 0.2
 twine ~= 4.0
-reuse ~= 1.1
+reuse ~= 2.1
```

### Comparing `flict-1.1.0/setup.py` & `flict-1.1.1/setup.py`

 * *Files identical despite different names*

