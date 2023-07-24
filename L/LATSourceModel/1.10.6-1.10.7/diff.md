# Comparing `tmp/LATSourceModel-1.10.6.tar.gz` & `tmp/LATSourceModel-1.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LATSourceModel-1.10.6.tar", last modified: Tue Jul 18 17:14:51 2023, max compression
+gzip compressed data, was "LATSourceModel-1.10.7.tar", last modified: Mon Jul 24 12:37:01 2023, max compression
```

## Comparing `LATSourceModel-1.10.6.tar` & `LATSourceModel-1.10.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-07-18 17:14:51.265292 LATSourceModel-1.10.6/
--rw-r--r--   0 tyrelj     (501) staff       (20)    35129 2023-07-10 15:27:39.000000 LATSourceModel-1.10.6/LICENSE
--rw-r--r--   0 tyrelj     (501) staff       (20)     1594 2023-07-18 17:14:51.265180 LATSourceModel-1.10.6/PKG-INFO
--rw-r--r--   0 tyrelj     (501) staff       (20)     1078 2023-07-10 18:10:29.000000 LATSourceModel-1.10.6/README.md
--rw-r--r--   0 tyrelj     (501) staff       (20)      775 2023-07-16 19:02:17.000000 LATSourceModel-1.10.6/pyproject.toml
--rw-r--r--   0 tyrelj     (501) staff       (20)       38 2023-07-18 17:14:51.265326 LATSourceModel-1.10.6/setup.cfg
-drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-07-18 17:14:51.262786 LATSourceModel-1.10.6/src/
-drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-07-18 17:14:51.264273 LATSourceModel-1.10.6/src/LATSourceModel/
--rw-r--r--   0 tyrelj     (501) staff       (20)    48965 2023-07-18 17:10:18.000000 LATSourceModel-1.10.6/src/LATSourceModel/SourceList.py
--rw-r--r--   0 tyrelj     (501) staff       (20)      116 2023-07-16 19:02:17.000000 LATSourceModel-1.10.6/src/LATSourceModel/__init__.py
--rw-r--r--   0 tyrelj     (501) staff       (20)    10545 2023-07-16 19:02:17.000000 LATSourceModel-1.10.6/src/LATSourceModel/make4FGLxml.py
--rw-r--r--   0 tyrelj     (501) staff       (20)    74177 2023-07-18 17:10:18.000000 LATSourceModel-1.10.6/src/LATSourceModel/model_components.py
--rw-r--r--   0 tyrelj     (501) staff       (20)    11927 2023-07-18 17:10:18.000000 LATSourceModel-1.10.6/src/LATSourceModel/utilities.py
-drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-07-18 17:14:51.265025 LATSourceModel-1.10.6/src/LATSourceModel.egg-info/
--rw-r--r--   0 tyrelj     (501) staff       (20)     1594 2023-07-18 17:14:51.000000 LATSourceModel-1.10.6/src/LATSourceModel.egg-info/PKG-INFO
--rw-r--r--   0 tyrelj     (501) staff       (20)      455 2023-07-18 17:14:51.000000 LATSourceModel-1.10.6/src/LATSourceModel.egg-info/SOURCES.txt
--rw-r--r--   0 tyrelj     (501) staff       (20)        1 2023-07-18 17:14:51.000000 LATSourceModel-1.10.6/src/LATSourceModel.egg-info/dependency_links.txt
--rw-r--r--   0 tyrelj     (501) staff       (20)       63 2023-07-18 17:14:51.000000 LATSourceModel-1.10.6/src/LATSourceModel.egg-info/entry_points.txt
--rw-r--r--   0 tyrelj     (501) staff       (20)       21 2023-07-18 17:14:51.000000 LATSourceModel-1.10.6/src/LATSourceModel.egg-info/requires.txt
--rw-r--r--   0 tyrelj     (501) staff       (20)       15 2023-07-18 17:14:51.000000 LATSourceModel-1.10.6/src/LATSourceModel.egg-info/top_level.txt
+drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-07-24 12:37:01.837949 LATSourceModel-1.10.7/
+-rw-r--r--   0 tyrelj     (501) staff       (20)    35129 2023-07-10 15:27:39.000000 LATSourceModel-1.10.7/LICENSE
+-rw-r--r--   0 tyrelj     (501) staff       (20)     1731 2023-07-24 12:37:01.837839 LATSourceModel-1.10.7/PKG-INFO
+-rw-r--r--   0 tyrelj     (501) staff       (20)     1078 2023-07-10 18:10:29.000000 LATSourceModel-1.10.7/README.md
+-rw-r--r--   0 tyrelj     (501) staff       (20)      912 2023-07-24 12:36:23.000000 LATSourceModel-1.10.7/pyproject.toml
+-rw-r--r--   0 tyrelj     (501) staff       (20)       38 2023-07-24 12:37:01.837984 LATSourceModel-1.10.7/setup.cfg
+drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-07-24 12:37:01.835789 LATSourceModel-1.10.7/src/
+drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-07-24 12:37:01.836921 LATSourceModel-1.10.7/src/LATSourceModel/
+-rw-r--r--   0 tyrelj     (501) staff       (20)    48965 2023-07-18 17:10:18.000000 LATSourceModel-1.10.7/src/LATSourceModel/SourceList.py
+-rw-r--r--   0 tyrelj     (501) staff       (20)      116 2023-07-16 19:02:17.000000 LATSourceModel-1.10.7/src/LATSourceModel/__init__.py
+-rw-r--r--   0 tyrelj     (501) staff       (20)    10547 2023-07-24 12:30:24.000000 LATSourceModel-1.10.7/src/LATSourceModel/make4FGLxml.py
+-rw-r--r--   0 tyrelj     (501) staff       (20)    74177 2023-07-18 17:10:18.000000 LATSourceModel-1.10.7/src/LATSourceModel/model_components.py
+-rw-r--r--   0 tyrelj     (501) staff       (20)    11927 2023-07-18 17:10:18.000000 LATSourceModel-1.10.7/src/LATSourceModel/utilities.py
+drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-07-24 12:37:01.837682 LATSourceModel-1.10.7/src/LATSourceModel.egg-info/
+-rw-r--r--   0 tyrelj     (501) staff       (20)     1731 2023-07-24 12:37:01.000000 LATSourceModel-1.10.7/src/LATSourceModel.egg-info/PKG-INFO
+-rw-r--r--   0 tyrelj     (501) staff       (20)      455 2023-07-24 12:37:01.000000 LATSourceModel-1.10.7/src/LATSourceModel.egg-info/SOURCES.txt
+-rw-r--r--   0 tyrelj     (501) staff       (20)        1 2023-07-24 12:37:01.000000 LATSourceModel-1.10.7/src/LATSourceModel.egg-info/dependency_links.txt
+-rw-r--r--   0 tyrelj     (501) staff       (20)       63 2023-07-24 12:37:01.000000 LATSourceModel-1.10.7/src/LATSourceModel.egg-info/entry_points.txt
+-rw-r--r--   0 tyrelj     (501) staff       (20)       21 2023-07-24 12:37:01.000000 LATSourceModel-1.10.7/src/LATSourceModel.egg-info/requires.txt
+-rw-r--r--   0 tyrelj     (501) staff       (20)       15 2023-07-24 12:37:01.000000 LATSourceModel-1.10.7/src/LATSourceModel.egg-info/top_level.txt
```

### Comparing `LATSourceModel-1.10.6/LICENSE` & `LATSourceModel-1.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.6/PKG-INFO` & `LATSourceModel-1.10.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: LATSourceModel
-Version: 1.10.6
+Version: 1.10.7
 Summary: A set of functions and classes to build spatial-spectral models for analysis of Fermi LAT gamma-ray data.
 Author-email: Tyrel Johnson <tyrel.j.johnson@gmail.com>
 License: GPL-3.0
+Project-URL: Home, https://github.com/physicsranger/make4FGLxml
+Project-URL: Issues, https://github.com/physicsranger/make4FGLxml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `LATSourceModel-1.10.6/README.md` & `LATSourceModel-1.10.7/README.md`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.6/pyproject.toml` & `LATSourceModel-1.10.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LATSourceModel"
 authors = [
     {name = "Tyrel Johnson", email = "tyrel.j.johnson@gmail.com"},
 ]
-version = "1.10.6"
+version = "1.10.7"
 description = "A set of functions and classes to build spatial-spectral models for analysis of Fermi LAT gamma-ray data."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.4" #for pathlib
 license = {text = "GPL-3.0"}
 classifiers = [
 "Programming Language :: Python :: 3",
 "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -22,8 +22,12 @@
 dependencies = [
     "numpy",
     "pandas",
     "astropy"
 ]
 
 [project.scripts]
-make4FGLxml = "LATSourceModel.make4FGLxml:cli"
+make4FGLxml = "LATSourceModel.make4FGLxml:cli"
+
+[project.urls]
+"Home" = "https://github.com/physicsranger/make4FGLxml"
+"Issues" = "https://github.com/physicsranger/make4FGLxml/issues"
```

### Comparing `LATSourceModel-1.10.6/src/LATSourceModel/SourceList.py` & `LATSourceModel-1.10.7/src/LATSourceModel/SourceList.py`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.6/src/LATSourceModel/make4FGLxml.py` & `LATSourceModel-1.10.7/src/LATSourceModel/make4FGLxml.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     parser.add_argument("-i","--isotropic_name",type=str,default='iso_P8R3_SOURCE_V3_v1'
                 ,help="Name of isotropic diffuse component in output model, default is for P8R3 SOURCE class.")
     
     parser.add_argument("-N","--norms_free_only",type=mybool,default=False
                 ,help="Flag to only let the normalizations of parameters be free, default is False.",
                 nargs="?",const=True,choices=['True','False','T','F','t','f','TRUE','FALSE','true','false',1,0])
     
-    parser.add_argument("-e","--extended_directory",type=str,default='',
+    parser.add_argument("-e","--extended_directory",type=str,default=None,
                 help="Path to directory with LAT extended source templates, will default to STs default.")
     
     parser.add_argument("-r","--free_radius",type=float,default=-1.,
                 help="Radius, in degrees, from ROI center beyond which all source parameters should be fixed,\
  will default to selection radius.")
     
     parser.add_argument("-R","--max_free_radius",type=float,default=None,
```

### Comparing `LATSourceModel-1.10.6/src/LATSourceModel/model_components.py` & `LATSourceModel-1.10.7/src/LATSourceModel/model_components.py`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.6/src/LATSourceModel/utilities.py` & `LATSourceModel-1.10.7/src/LATSourceModel/utilities.py`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.6/src/LATSourceModel.egg-info/PKG-INFO` & `LATSourceModel-1.10.7/src/LATSourceModel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: LATSourceModel
-Version: 1.10.6
+Version: 1.10.7
 Summary: A set of functions and classes to build spatial-spectral models for analysis of Fermi LAT gamma-ray data.
 Author-email: Tyrel Johnson <tyrel.j.johnson@gmail.com>
 License: GPL-3.0
+Project-URL: Home, https://github.com/physicsranger/make4FGLxml
+Project-URL: Issues, https://github.com/physicsranger/make4FGLxml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

