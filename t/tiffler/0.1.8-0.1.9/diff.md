# Comparing `tmp/tiffler-0.1.8.tar.gz` & `tmp/tiffler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiffler-0.1.8.tar", last modified: Mon Jul 24 05:00:51 2023, max compression
+gzip compressed data, was "tiffler-0.1.9.tar", last modified: Mon Jul 24 05:07:07 2023, max compression
```

## Comparing `tiffler-0.1.8.tar` & `tiffler-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:00:51.179825 tiffler-0.1.8/
--rw-r--r--   0 datnh      (501) staff       (20)     1319 2023-07-24 05:00:51.179705 tiffler-0.1.8/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)      896 2022-10-02 04:48:43.000000 tiffler-0.1.8/README.md
--rw-r--r--   0 datnh      (501) staff       (20)       38 2023-07-24 05:00:51.179923 tiffler-0.1.8/setup.cfg
--rw-r--r--   0 datnh      (501) staff       (20)     1250 2023-07-24 05:00:39.000000 tiffler-0.1.8/setup.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:00:51.178631 tiffler-0.1.8/tiffler/
--rw-r--r--   0 datnh      (501) staff       (20)       23 2022-10-02 04:48:43.000000 tiffler-0.1.8/tiffler/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     2893 2023-07-24 05:00:32.000000 tiffler-0.1.8/tiffler/tiffler.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:00:51.179420 tiffler-0.1.8/tiffler.egg-info/
--rw-r--r--   0 datnh      (501) staff       (20)     1319 2023-07-24 05:00:51.000000 tiffler-0.1.8/tiffler.egg-info/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)      181 2023-07-24 05:00:51.000000 tiffler-0.1.8/tiffler.egg-info/SOURCES.txt
--rw-r--r--   0 datnh      (501) staff       (20)        1 2023-07-24 05:00:51.000000 tiffler-0.1.8/tiffler.egg-info/dependency_links.txt
--rw-r--r--   0 datnh      (501) staff       (20)        8 2023-07-24 05:00:51.000000 tiffler-0.1.8/tiffler.egg-info/top_level.txt
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:07:07.796957 tiffler-0.1.9/
+-rw-r--r--   0 datnh      (501) staff       (20)     1319 2023-07-24 05:07:07.796839 tiffler-0.1.9/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)      896 2022-10-02 04:48:43.000000 tiffler-0.1.9/README.md
+-rw-r--r--   0 datnh      (501) staff       (20)       38 2023-07-24 05:07:07.797051 tiffler-0.1.9/setup.cfg
+-rw-r--r--   0 datnh      (501) staff       (20)     1250 2023-07-24 05:06:58.000000 tiffler-0.1.9/setup.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:07:07.795791 tiffler-0.1.9/tiffler/
+-rw-r--r--   0 datnh      (501) staff       (20)       23 2022-10-02 04:48:43.000000 tiffler-0.1.9/tiffler/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)     3252 2023-07-24 05:06:53.000000 tiffler-0.1.9/tiffler/tiffler.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-24 05:07:07.796569 tiffler-0.1.9/tiffler.egg-info/
+-rw-r--r--   0 datnh      (501) staff       (20)     1319 2023-07-24 05:07:07.000000 tiffler-0.1.9/tiffler.egg-info/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)      181 2023-07-24 05:07:07.000000 tiffler-0.1.9/tiffler.egg-info/SOURCES.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        1 2023-07-24 05:07:07.000000 tiffler-0.1.9/tiffler.egg-info/dependency_links.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        8 2023-07-24 05:07:07.000000 tiffler-0.1.9/tiffler.egg-info/top_level.txt
```

### Comparing `tiffler-0.1.8/PKG-INFO` & `tiffler-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiffler
-Version: 0.1.8
+Version: 0.1.9
 Summary: This Niffler finds shiny variables in text
 Home-page: UNKNOWN
 Author: nghoangdat
 Author-email: dat.nh.216@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tiffler-0.1.8/README.md` & `tiffler-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tiffler-0.1.8/setup.py` & `tiffler-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 extras_require = {}
 for path in glob("requirements.*.txt"):
     match = re.search("(?<=\.).+(?=\.)", path)
     if match:
         mode = match.group(0)
         extras_require[mode] = read_requirements(path)
 
-__VERSION__ = "0.1.8"
+__VERSION__ = "0.1.9"
 __DESCRIPTION__ = "This Niffler finds shiny variables in text"
 
 
 setuptools.setup(
     name="tiffler",
     packages=setuptools.find_packages(),
     version=__VERSION__,
```

### Comparing `tiffler-0.1.8/tiffler/tiffler.py` & `tiffler-0.1.9/tiffler/tiffler.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 SUPPORTED_TYPES = {
     "float": "[-+]?\d*\.\d+|\d+",
     "int": "[-+]?\d*\.\d+|\d+",
     "bool": "true|True|false|False|0|1",
     "str": ".+",
 }
 
+SUPPORTED_CONVERTERS = {
+    "int": lambda val: int(float(val)),
+    "bool": lambda val: {
+        "true": True,
+        "false": False,
+        "0": False,
+        "1": True,
+    }.get(val.lower(), bool(val)),
+}
+
 __all__ = ["Tiffler", "compile", "scan", "search"]
 
 
 class Tiffler:
     def __init__(self, template: str, case_sensitive: bool = True, **kwargs):
         self.case_sensitive = case_sensitive
         self.build(template)
@@ -34,16 +44,19 @@
 
                 if var_type is None:
                     var_type = "str"
 
                 if var_expr is None:
                     var_expr = SUPPORTED_TYPES.get(var_type, ".+")
 
-                assert var_type in SUPPORTED_TYPES, f"Type {var_type} is not supported"
-                var_type = eval(var_type)
+                if var_type in SUPPORTED_CONVERTERS:
+                    var_type = SUPPORTED_CONVERTERS[var_type]
+                else:
+                    assert var_type in SUPPORTED_TYPES, f"Type {var_type} is not supported"
+                    var_type = eval(var_type)
 
                 self.template += (
                     template[curr_idx : match.start() - 1] + rf"({var_expr})"
                 )
                 curr_idx = match.end() + 1
                 self.vars[var_name] = var_type
```

### Comparing `tiffler-0.1.8/tiffler.egg-info/PKG-INFO` & `tiffler-0.1.9/tiffler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiffler
-Version: 0.1.8
+Version: 0.1.9
 Summary: This Niffler finds shiny variables in text
 Home-page: UNKNOWN
 Author: nghoangdat
 Author-email: dat.nh.216@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

