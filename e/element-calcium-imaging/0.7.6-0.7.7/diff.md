# Comparing `tmp/element-calcium-imaging-0.7.6.tar.gz` & `tmp/element-calcium-imaging-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-calcium-imaging-0.7.6.tar", last modified: Fri Jun 30 21:14:49 2023, max compression
+gzip compressed data, was "element-calcium-imaging-0.7.7.tar", last modified: Mon Jul 24 18:14:23 2023, max compression
```

## Comparing `element-calcium-imaging-0.7.6.tar` & `element-calcium-imaging-0.7.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:49.780861 element-calcium-imaging-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-30 21:14:49.780861 element-calcium-imaging-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:49.776861 element-calcium-imaging-0.7.6/element_calcium_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    66550 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63748 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    74306 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:49.780861 element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/cell_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/element_calcium_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:14:49.776861 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 21:14:49.000000 element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:14:49.780861 element-calcium-imaging-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-30 21:14:45.000000 element-calcium-imaging-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:23.293047 element-calcium-imaging-0.7.7/element_calcium_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66550 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63748 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74306 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/cell_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/setup.py
```

### Comparing `element-calcium-imaging-0.7.6/LICENSE` & `element-calcium-imaging-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/PKG-INFO` & `element-calcium-imaging-0.7.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.6
+Version: 0.7.7
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
@@ -40,16 +40,17 @@
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
 + We have designed three variations of the pipeline to handle different use cases. 
 Displayed above is the default `imaging` schema.  Details on all of the `imaging` 
-schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/
-element-calcium-imaging/latest/pipeline/) documentation page.
+schemas can be found in the [Data 
+Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) 
+documentation page.
 
 ## Getting Started
 
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
```

### Comparing `element-calcium-imaging-0.7.6/README.md` & `element-calcium-imaging-0.7.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
 + We have designed three variations of the pipeline to handle different use cases. 
 Displayed above is the default `imaging` schema.  Details on all of the `imaging` 
-schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/
-element-calcium-imaging/latest/pipeline/) documentation page.
+schemas can be found in the [Data 
+Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) 
+documentation page.
 
 ## Getting Started
 
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
```

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging/analysis.py` & `element-calcium-imaging-0.7.7/element_calcium_imaging/analysis.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging/imaging.py` & `element-calcium-imaging-0.7.7/element_calcium_imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_no_curation.py` & `element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_no_curation.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_preprocess.py` & `element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_preprocess.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging/imaging_report.py` & `element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_report.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/cell_plot.py` & `element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/cell_plot.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging/plotting/widget.py` & `element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging/scan.py` & `element-calcium-imaging-0.7.7/element_calcium_imaging/scan.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/PKG-INFO` & `element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.6
+Version: 0.7.7
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
@@ -40,16 +40,17 @@
 
 ## Data Pipeline Diagram
 
 ![pipeline](https://raw.githubusercontent.com/datajoint/element-calcium-imaging/main/images/pipeline_imaging.svg)
 
 + We have designed three variations of the pipeline to handle different use cases. 
 Displayed above is the default `imaging` schema.  Details on all of the `imaging` 
-schemas can be found in the [Data Pipeline](https://datajoint.com/docs/elements/
-element-calcium-imaging/latest/pipeline/) documentation page.
+schemas can be found in the [Data 
+Pipeline](https://datajoint.com/docs/elements/element-calcium-imaging/latest/pipeline/) 
+documentation page.
 
 ## Getting Started
 
 + Install from PyPI
 
      ```bash
      pip install element-calcium-imaging
```

### Comparing `element-calcium-imaging-0.7.6/element_calcium_imaging.egg-info/SOURCES.txt` & `element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.6/setup.py` & `element-calcium-imaging-0.7.7/setup.py`

 * *Files identical despite different names*

