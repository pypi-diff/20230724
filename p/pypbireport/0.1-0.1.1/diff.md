# Comparing `tmp/pypbireport-0.1.tar.gz` & `tmp/pypbireport-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypbireport-0.1.tar", last modified: Fri Jul 21 20:42:07 2023, max compression
+gzip compressed data, was "pypbireport-0.1.1.tar", last modified: Mon Jul 24 19:28:39 2023, max compression
```

## Comparing `pypbireport-0.1.tar` & `pypbireport-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 20:42:07.570924 pypbireport-0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-16 11:12:28.000000 pypbireport-0.1/LICENSE
--rw-rw-rw-   0        0        0     7831 2023-07-21 20:42:07.569922 pypbireport-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7427 2023-07-21 20:25:26.000000 pypbireport-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 20:42:07.556467 pypbireport-0.1/pypbireport/
--rw-rw-rw-   0        0        0      815 2023-07-21 19:43:52.000000 pypbireport-0.1/pypbireport/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:42:07.565919 pypbireport-0.1/pypbireport/constants/
--rw-rw-rw-   0        0        0       99 2023-07-18 20:18:03.000000 pypbireport-0.1/pypbireport/constants/bookmarks.py
--rw-rw-rw-   0        0        0      644 2023-07-18 20:18:10.000000 pypbireport-0.1/pypbireport/constants/charts.py
--rw-rw-rw-   0        0        0       85 2023-07-18 20:18:18.000000 pypbireport-0.1/pypbireport/constants/shapes.py
--rw-rw-rw-   0        0        0     2940 2023-07-18 20:18:21.000000 pypbireport-0.1/pypbireport/constants/structures.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:42:07.566923 pypbireport-0.1/pypbireport/functions/
--rw-rw-rw-   0        0        0      531 2023-07-16 09:16:07.000000 pypbireport-0.1/pypbireport/functions/functions.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:42:07.568921 pypbireport-0.1/pypbireport/pbi/
--rw-rw-rw-   0        0        0     4185 2023-07-21 19:39:15.000000 pypbireport-0.1/pypbireport/pbi/pbifile.py
--rw-rw-rw-   0        0        0    28954 2023-07-21 19:57:44.000000 pypbireport-0.1/pypbireport/pbi/pbireport.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:42:07.561920 pypbireport-0.1/pypbireport.egg-info/
--rw-rw-rw-   0        0        0     7831 2023-07-21 20:42:07.000000 pypbireport-0.1/pypbireport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-21 20:42:07.000000 pypbireport-0.1/pypbireport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:42:07.000000 pypbireport-0.1/pypbireport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-21 20:42:07.000000 pypbireport-0.1/pypbireport.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-21 20:42:07.000000 pypbireport-0.1/pypbireport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-07-18 20:14:31.000000 pypbireport-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 20:42:07.571434 pypbireport-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 19:28:39.324298 pypbireport-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-07-16 11:12:28.000000 pypbireport-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7946 2023-07-24 19:28:39.323297 pypbireport-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7538 2023-07-24 19:25:24.000000 pypbireport-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 19:28:39.308297 pypbireport-0.1.1/pypbireport/
+-rw-rw-rw-   0        0        0      815 2023-07-21 19:43:52.000000 pypbireport-0.1.1/pypbireport/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:28:39.319296 pypbireport-0.1.1/pypbireport/constants/
+-rw-rw-rw-   0        0        0       99 2023-07-18 20:18:03.000000 pypbireport-0.1.1/pypbireport/constants/bookmarks.py
+-rw-rw-rw-   0        0        0      644 2023-07-18 20:18:10.000000 pypbireport-0.1.1/pypbireport/constants/charts.py
+-rw-rw-rw-   0        0        0       85 2023-07-18 20:18:18.000000 pypbireport-0.1.1/pypbireport/constants/shapes.py
+-rw-rw-rw-   0        0        0     2940 2023-07-18 20:18:21.000000 pypbireport-0.1.1/pypbireport/constants/structures.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:28:39.320295 pypbireport-0.1.1/pypbireport/functions/
+-rw-rw-rw-   0        0        0      531 2023-07-16 09:16:07.000000 pypbireport-0.1.1/pypbireport/functions/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:28:39.322296 pypbireport-0.1.1/pypbireport/pbi/
+-rw-rw-rw-   0        0        0     4185 2023-07-21 19:39:15.000000 pypbireport-0.1.1/pypbireport/pbi/pbifile.py
+-rw-rw-rw-   0        0        0    29219 2023-07-24 19:24:55.000000 pypbireport-0.1.1/pypbireport/pbi/pbireport.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:28:39.314296 pypbireport-0.1.1/pypbireport.egg-info/
+-rw-rw-rw-   0        0        0     7946 2023-07-24 19:28:39.000000 pypbireport-0.1.1/pypbireport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-24 19:28:39.000000 pypbireport-0.1.1/pypbireport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 19:28:39.000000 pypbireport-0.1.1/pypbireport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-24 19:28:39.000000 pypbireport-0.1.1/pypbireport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-24 19:28:39.000000 pypbireport-0.1.1/pypbireport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      559 2023-07-24 19:25:52.000000 pypbireport-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 19:28:39.324298 pypbireport-0.1.1/setup.cfg
```

### Comparing `pypbireport-0.1/LICENSE` & `pypbireport-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypbireport-0.1/PKG-INFO` & `pypbireport-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypbireport
-Version: 0.1
+Version: 0.1.1
 Summary: Package to manipulate Power BI reports
 Author-email: Ismael Miranda <ismaelmiranda11@hotmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 
 - [Coding Power BI Report Layout with Python](#coding-power-bi-report-layout-with-python)
   - [Installation and use](#installation-and-use)
   - [Why?](#why)
   - [Features](#features)
   - [Use case](#use-case)
   - [Licensing and Author](#licensing-and-author)
+  - [Versions](#versions)
 
 
 ## Installation and use
 
 To use this module in Python, just install it with pip in the command line.
 
 ```
@@ -157,7 +158,12 @@
 
 ## Licensing and Author 
 
 Be free to use this module in your Power BI development and don't hesitate to contact me.
 
 Ismael Miranda  
 <ismaelmiranda11@hotmail.com>
+
+## Versions
+
+0.1 - Release
+0.1.1 - Bug fix in create_bookmark_slicer() function
```

### Comparing `pypbireport-0.1/README.md` & `pypbireport-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 - [Coding Power BI Report Layout with Python](#coding-power-bi-report-layout-with-python)
   - [Installation and use](#installation-and-use)
   - [Why?](#why)
   - [Features](#features)
   - [Use case](#use-case)
   - [Licensing and Author](#licensing-and-author)
+  - [Versions](#versions)
 
 
 ## Installation and use
 
 To use this module in Python, just install it with pip in the command line.
 
 ```
@@ -145,7 +146,12 @@
 
 ## Licensing and Author 
 
 Be free to use this module in your Power BI development and don't hesitate to contact me.
 
 Ismael Miranda  
 <ismaelmiranda11@hotmail.com>
+
+## Versions
+
+0.1 - Release
+0.1.1 - Bug fix in create_bookmark_slicer() function
```

### Comparing `pypbireport-0.1/pypbireport/__init__.py` & `pypbireport-0.1.1/pypbireport/__init__.py`

 * *Files identical despite different names*

### Comparing `pypbireport-0.1/pypbireport/constants/charts.py` & `pypbireport-0.1.1/pypbireport/constants/charts.py`

 * *Files identical despite different names*

### Comparing `pypbireport-0.1/pypbireport/constants/structures.py` & `pypbireport-0.1.1/pypbireport/constants/structures.py`

 * *Files identical despite different names*

### Comparing `pypbireport-0.1/pypbireport/functions/functions.py` & `pypbireport-0.1.1/pypbireport/functions/functions.py`

 * *Files identical despite different names*

### Comparing `pypbireport-0.1/pypbireport/pbi/pbifile.py` & `pypbireport-0.1.1/pypbireport/pbi/pbifile.py`

 * *Files identical despite different names*

### Comparing `pypbireport-0.1/pypbireport/pbi/pbireport.py` & `pypbireport-0.1.1/pypbireport/pbi/pbireport.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,20 +669,31 @@
             _id_ (str): A hexadecimal value for created bookmark slicer.
             _dict_ (dict): The dict of bookmark slicer.
 
         Description:
             For a bookmark group created, this create a bookmark slicer or 
             bookmark navigator for report. 
         '''
-        bookmark_slicer_dict = BOOKMARK_SLICER_DICT
+        bookmark_slicer_dict = copy.deepcopy(BOOKMARK_SLICER_DICT)
         
         # 1. Assemble the dict
         _visual_id = hex_code()
 
-        bookmark_slice_config_dict = BOOKMARK_SLICER_CONFIG_DICT
+        bookmark_slice_config_dict = copy.deepcopy(BOOKMARK_SLICER_CONFIG_DICT)
+        
+        # Name
+        (
+            bookmark_slice_config_dict
+            .update(
+                {
+                    'name':_visual_id
+                }
+            )
+        )
+        # Layout
         (
             bookmark_slice_config_dict
             .get('layouts',[{}])
             [0]
             .get('position',{})
             .update(
                 {
@@ -691,15 +702,15 @@
                     "z": bookmark_slicer_dict.get('z'),
                     "width":  bookmark_slicer_dict.get('width'),
                     "height": bookmark_slicer_dict.get('height'),
                     "tabOrder":  bookmark_slicer_dict.get('tabOrder')
                 }
             )
         )
-        
+        # Bookmarkgroup
         (
             bookmark_slice_config_dict
             .get('singleVisual',{})
             .get('objects',{})
             .get('bookmarks',[])
             [0]
             .get('properties',{})
```

### Comparing `pypbireport-0.1/pypbireport.egg-info/PKG-INFO` & `pypbireport-0.1.1/pypbireport.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypbireport
-Version: 0.1
+Version: 0.1.1
 Summary: Package to manipulate Power BI reports
 Author-email: Ismael Miranda <ismaelmiranda11@hotmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 
 - [Coding Power BI Report Layout with Python](#coding-power-bi-report-layout-with-python)
   - [Installation and use](#installation-and-use)
   - [Why?](#why)
   - [Features](#features)
   - [Use case](#use-case)
   - [Licensing and Author](#licensing-and-author)
+  - [Versions](#versions)
 
 
 ## Installation and use
 
 To use this module in Python, just install it with pip in the command line.
 
 ```
@@ -157,7 +158,12 @@
 
 ## Licensing and Author 
 
 Be free to use this module in your Power BI development and don't hesitate to contact me.
 
 Ismael Miranda  
 <ismaelmiranda11@hotmail.com>
+
+## Versions
+
+0.1 - Release
+0.1.1 - Bug fix in create_bookmark_slicer() function
```

### Comparing `pypbireport-0.1/pyproject.toml` & `pypbireport-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-sytem]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pypbireport'
-version = '0.1'
+version = '0.1.1'
 authors = [
     {name='Ismael Miranda', email='ismaelmiranda11@hotmail.com'}
 ]
 description = 'Package to manipulate Power BI reports'
 readme = 'README.md'
 requires-python = '>=3.9'
 classifiers = [
```

