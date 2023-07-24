# Comparing `tmp/pyne_script_utilities-1.0.4.tar.gz` & `tmp/pyne_script_utilities-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyne_script_utilities-1.0.4.tar", last modified: Mon Jul 24 19:41:31 2023, max compression
+gzip compressed data, was "pyne_script_utilities-1.0.5.tar", last modified: Mon Jul 24 20:24:05 2023, max compression
```

## Comparing `pyne_script_utilities-1.0.4.tar` & `pyne_script_utilities-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 19:41:31.530767 pyne_script_utilities-1.0.4/
--rw-r--r--   0 krijn     (1000) krijn     (1000)    35148 2023-07-06 09:11:48.000000 pyne_script_utilities-1.0.4/LICENSE
--rw-r--r--   0 krijn     (1000) krijn     (1000)     1149 2023-07-24 19:41:31.530767 pyne_script_utilities-1.0.4/PKG-INFO
--rw-r--r--   0 krijn     (1000) krijn     (1000)      613 2023-07-19 19:47:36.000000 pyne_script_utilities-1.0.4/README.md
--rw-r--r--   0 krijn     (1000) krijn     (1000)      727 2023-07-24 19:14:02.000000 pyne_script_utilities-1.0.4/pyproject.toml
--rw-r--r--   0 krijn     (1000) krijn     (1000)       38 2023-07-24 19:41:31.530767 pyne_script_utilities-1.0.4/setup.cfg
-drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 19:41:31.530767 pyne_script_utilities-1.0.4/src/
-drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 19:41:31.530767 pyne_script_utilities-1.0.4/src/pyne_script/
--rw-r--r--   0 krijn     (1000) krijn     (1000)       38 2023-07-22 13:56:07.000000 pyne_script_utilities-1.0.4/src/pyne_script/__init__.py
--rw-r--r--   0 krijn     (1000) krijn     (1000)    23208 2023-07-24 19:28:20.000000 pyne_script_utilities-1.0.4/src/pyne_script/series.py
-drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 19:41:31.530767 pyne_script_utilities-1.0.4/src/pyne_script_utilities.egg-info/
--rw-r--r--   0 krijn     (1000) krijn     (1000)     1149 2023-07-24 19:41:31.000000 pyne_script_utilities-1.0.4/src/pyne_script_utilities.egg-info/PKG-INFO
--rw-r--r--   0 krijn     (1000) krijn     (1000)      330 2023-07-24 19:41:31.000000 pyne_script_utilities-1.0.4/src/pyne_script_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 krijn     (1000) krijn     (1000)        1 2023-07-24 19:41:31.000000 pyne_script_utilities-1.0.4/src/pyne_script_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 krijn     (1000) krijn     (1000)        6 2023-07-24 19:41:31.000000 pyne_script_utilities-1.0.4/src/pyne_script_utilities.egg-info/requires.txt
--rw-r--r--   0 krijn     (1000) krijn     (1000)       12 2023-07-24 19:41:31.000000 pyne_script_utilities-1.0.4/src/pyne_script_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 20:24:05.670053 pyne_script_utilities-1.0.5/
+-rw-r--r--   0 krijn     (1000) krijn     (1000)    35148 2023-07-06 09:11:48.000000 pyne_script_utilities-1.0.5/LICENSE
+-rw-r--r--   0 krijn     (1000) krijn     (1000)     1149 2023-07-24 20:24:05.670053 pyne_script_utilities-1.0.5/PKG-INFO
+-rw-r--r--   0 krijn     (1000) krijn     (1000)      613 2023-07-19 19:47:36.000000 pyne_script_utilities-1.0.5/README.md
+-rw-r--r--   0 krijn     (1000) krijn     (1000)      727 2023-07-24 20:20:28.000000 pyne_script_utilities-1.0.5/pyproject.toml
+-rw-r--r--   0 krijn     (1000) krijn     (1000)       38 2023-07-24 20:24:05.670053 pyne_script_utilities-1.0.5/setup.cfg
+drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 20:24:05.670053 pyne_script_utilities-1.0.5/src/
+drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 20:24:05.670053 pyne_script_utilities-1.0.5/src/pyne_script/
+-rw-r--r--   0 krijn     (1000) krijn     (1000)       38 2023-07-22 13:56:07.000000 pyne_script_utilities-1.0.5/src/pyne_script/__init__.py
+-rw-r--r--   0 krijn     (1000) krijn     (1000)    23220 2023-07-24 20:21:24.000000 pyne_script_utilities-1.0.5/src/pyne_script/series.py
+drwxr-xr-x   0 krijn     (1000) krijn     (1000)        0 2023-07-24 20:24:05.670053 pyne_script_utilities-1.0.5/src/pyne_script_utilities.egg-info/
+-rw-r--r--   0 krijn     (1000) krijn     (1000)     1149 2023-07-24 20:24:05.000000 pyne_script_utilities-1.0.5/src/pyne_script_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 krijn     (1000) krijn     (1000)      330 2023-07-24 20:24:05.000000 pyne_script_utilities-1.0.5/src/pyne_script_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 krijn     (1000) krijn     (1000)        1 2023-07-24 20:24:05.000000 pyne_script_utilities-1.0.5/src/pyne_script_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 krijn     (1000) krijn     (1000)        6 2023-07-24 20:24:05.000000 pyne_script_utilities-1.0.5/src/pyne_script_utilities.egg-info/requires.txt
+-rw-r--r--   0 krijn     (1000) krijn     (1000)       12 2023-07-24 20:24:05.000000 pyne_script_utilities-1.0.5/src/pyne_script_utilities.egg-info/top_level.txt
```

### Comparing `pyne_script_utilities-1.0.4/LICENSE` & `pyne_script_utilities-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyne_script_utilities-1.0.4/PKG-INFO` & `pyne_script_utilities-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyne_script_utilities
-Version: 1.0.4
+Version: 1.0.5
 Summary: A set of utility sub-modules that allow for code structure similar to pinescript in python
 Author: 80sVectorz
 Project-URL: Homepage, https://github.com/80sVectorz/pyne_script
 Project-URL: Bug Tracker, https://github.com/80sVectorz/pyne_script/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
```

### Comparing `pyne_script_utilities-1.0.4/README.md` & `pyne_script_utilities-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyne_script_utilities-1.0.4/pyproject.toml` & `pyne_script_utilities-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["pyne_script*"]
 namespaces = false
 
 [project]
 name = "pyne_script_utilities"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="80sVectorz"},
 ]
 description = "A set of utility sub-modules that allow for code structure similar to pinescript in python"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["numpy"]
```

### Comparing `pyne_script_utilities-1.0.4/src/pyne_script/series.py` & `pyne_script_utilities-1.0.5/src/pyne_script/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
                 elif len(data) == 0:
                     raise SeriesInvalidKeyValuePairs_Zero()
                 if length_ticker == -1:
                     length_ticker = len(data)
                 elif len(data) != length_ticker:
                     raise SeriesInvalidKeyValuePairs_Length()
                 for element in data:
-                    if not isinstance(element, int | float):
+                    if not isinstance(element, int | float | np.number):
                         raise SeriesInvalidKeyValuePairs_Numeric(key)
 
                 self.series_types[key] = series_type
 
                 if series_type == int and int not in self.heads.keys():
                     self.heads[int] = np.zeros(
                         len(key_value_pairs.values()), dtype=dtypes[int]
```

### Comparing `pyne_script_utilities-1.0.4/src/pyne_script_utilities.egg-info/PKG-INFO` & `pyne_script_utilities-1.0.5/src/pyne_script_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyne-script-utilities
-Version: 1.0.4
+Version: 1.0.5
 Summary: A set of utility sub-modules that allow for code structure similar to pinescript in python
 Author: 80sVectorz
 Project-URL: Homepage, https://github.com/80sVectorz/pyne_script
 Project-URL: Bug Tracker, https://github.com/80sVectorz/pyne_script/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
```

