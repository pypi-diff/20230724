# Comparing `tmp/tubular-0.3.8.tar.gz` & `tmp/tubular-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubular-0.3.8.tar", last modified: Mon Jul 10 16:13:10 2023, max compression
+gzip compressed data, was "tubular-1.0.0.tar", last modified: Mon Jul 24 13:13:41 2023, max compression
```

## Comparing `tubular-0.3.8.tar` & `tubular-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:13:10.090562 tubular-0.3.8/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1550 2023-07-10 16:08:48.000000 tubular-0.3.8/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4336 2023-07-10 16:13:10.086562 tubular-0.3.8/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3707 2023-07-10 16:08:48.000000 tubular-0.3.8/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-07-10 16:13:10.090562 tubular-0.3.8/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1519 2023-07-10 16:08:48.000000 tubular-0.3.8/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:13:10.074562 tubular-0.3.8/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:08:48.000000 tubular-0.3.8/tests/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14382 2023-07-10 16:08:48.000000 tubular-0.3.8/tests/test_data.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4983 2023-07-10 16:08:48.000000 tubular-0.3.8/tests/test_transformers.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:13:10.082563 tubular-0.3.8/tubular/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      175 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       22 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/_version.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15066 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/base.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20018 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/capping.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2063 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/comparison.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    41318 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/dates.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13415 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/imputers.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17169 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/mapping.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2003 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/misc.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42320 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/nominal.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    29859 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/numeric.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5981 2023-07-10 16:08:48.000000 tubular-0.3.8/tubular/strings.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-10 16:13:10.086562 tubular-0.3.8/tubular.egg-info/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4336 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      470 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       40 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       14 2023-07-10 16:13:09.000000 tubular-0.3.8/tubular.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-24 13:13:41.048693 tubular-1.0.0/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1550 2023-07-24 13:06:41.000000 tubular-1.0.0/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4336 2023-07-24 13:13:41.048693 tubular-1.0.0/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3707 2023-07-24 13:06:41.000000 tubular-1.0.0/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-07-24 13:13:41.048693 tubular-1.0.0/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1519 2023-07-24 13:06:41.000000 tubular-1.0.0/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-24 13:13:41.032693 tubular-1.0.0/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-07-24 13:06:41.000000 tubular-1.0.0/tests/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14382 2023-07-24 13:06:41.000000 tubular-1.0.0/tests/test_data.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4983 2023-07-24 13:06:41.000000 tubular-1.0.0/tests/test_transformers.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-24 13:13:41.040693 tubular-1.0.0/tubular/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      175 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       22 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/_version.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15066 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/base.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20018 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/capping.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2063 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/comparison.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    41038 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/dates.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13415 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/imputers.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17169 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/mapping.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2003 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/misc.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42320 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/nominal.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    29859 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/numeric.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5981 2023-07-24 13:06:41.000000 tubular-1.0.0/tubular/strings.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-24 13:13:41.048693 tubular-1.0.0/tubular.egg-info/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4336 2023-07-24 13:13:40.000000 tubular-1.0.0/tubular.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      470 2023-07-24 13:13:40.000000 tubular-1.0.0/tubular.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-07-24 13:13:40.000000 tubular-1.0.0/tubular.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       33 2023-07-24 13:13:40.000000 tubular-1.0.0/tubular.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       14 2023-07-24 13:13:40.000000 tubular-1.0.0/tubular.egg-info/top_level.txt
```

### Comparing `tubular-0.3.8/LICENSE` & `tubular-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/PKG-INFO` & `tubular-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.8
+Version: 1.0.0
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tubular-0.3.8/README.md` & `tubular-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/setup.py` & `tubular-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tests/test_data.py` & `tubular-1.0.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tests/test_transformers.py` & `tubular-1.0.0/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/base.py` & `tubular-1.0.0/tubular/base.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/capping.py` & `tubular-1.0.0/tubular/capping.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/comparison.py` & `tubular-1.0.0/tubular/comparison.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/dates.py` & `tubular-1.0.0/tubular/dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         Name of first date column, difference will be calculated as column_upper - column_lower
     column_upper : str
         Name of second date column, difference will be calculated as column_upper - column_lower
     new_column_name : str, default = None
         Name given to calculated datediff column. If None then {column_upper}_{column_lower}_datediff_{units}
         will be used.
     units : str, default = 'D'
-        Numpy datetime units, accepted values are 'Y', 'M', 'D', 'h', 'm', 's'
+        Numpy datetime units, accepted values are 'D', 'h', 'm', 's'
     copy : bool, default = True
         Should X be copied prior to transform?
     verbose: bool, default = False
     """
 
     def __init__(
         self,
@@ -207,33 +207,27 @@
         if type(column_upper) is not str:
             msg = f"{self.classname()}: column_upper must be a str"
             raise TypeError(msg)
 
         columns = [column_lower, column_upper]
 
         accepted_values_units = [
-            "Y",
-            "M",
             "D",
             "h",
             "m",
             "s",
         ]
 
         if type(units) is not str:
             msg = f"{self.classname()}: units must be a str"
             raise TypeError(msg)
 
         if units not in accepted_values_units:
             msg = f"{self.classname()}: units must be one of {accepted_values_units}, got {units}"
             raise ValueError(msg)
-        if units in ["Y", "M"]:
-            warnings.warn(
-                f"{self.classname()}: Y/M units will be changed or deprecated in a future version, consider using DateDiffLeapYearTransformer or D units instead",
-            )
 
         self.units = units
 
         if new_column_name is not None:
             if type(new_column_name) is not str:
                 msg = f"{self.classname()}: new_column_name must be a str"
                 raise TypeError(msg)
```

### Comparing `tubular-0.3.8/tubular/imputers.py` & `tubular-1.0.0/tubular/imputers.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/mapping.py` & `tubular-1.0.0/tubular/mapping.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/misc.py` & `tubular-1.0.0/tubular/misc.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/nominal.py` & `tubular-1.0.0/tubular/nominal.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/numeric.py` & `tubular-1.0.0/tubular/numeric.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular/strings.py` & `tubular-1.0.0/tubular/strings.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.8/tubular.egg-info/PKG-INFO` & `tubular-1.0.0/tubular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.8
+Version: 1.0.0
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

