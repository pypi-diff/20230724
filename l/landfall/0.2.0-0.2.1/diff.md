# Comparing `tmp/landfall-0.2.0.tar.gz` & `tmp/landfall-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landfall-0.2.0.tar", last modified: Fri Jul 21 17:38:04 2023, max compression
+gzip compressed data, was "landfall-0.2.1.tar", last modified: Mon Jul 24 15:03:08 2023, max compression
```

## Comparing `landfall-0.2.0.tar` & `landfall-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-21 17:38:04.657163 landfall-0.2.0/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.2.0/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-21 17:38:04.657316 landfall-0.2.0/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1348 2023-07-21 17:24:03.000000 landfall-0.2.0/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.2.0/pyproject.toml
--rw-r--r--   0 odosmatthews   (501) staff       (20)      856 2023-07-21 17:38:04.658549 landfall-0.2.0/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-02-28 17:08:57.000000 landfall-0.2.0/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-21 17:38:04.643072 landfall-0.2.0/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-21 17:38:04.650142 landfall-0.2.0/src/landfall/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      121 2023-07-21 17:35:38.000000 landfall-0.2.0/src/landfall/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.2.0/src/landfall/color.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.2.0/src/landfall/colorsys.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.2.0/src/landfall/distinctipy.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2550 2023-07-21 17:37:15.000000 landfall-0.2.0/src/landfall/points.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-21 17:38:04.656866 landfall-0.2.0/src/landfall.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-21 17:38:04.000000 landfall-0.2.0/src/landfall.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      388 2023-07-21 17:38:04.000000 landfall-0.2.0/src/landfall.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-21 17:38:04.000000 landfall-0.2.0/src/landfall.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.2.0/src/landfall.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      142 2023-07-21 17:38:04.000000 landfall-0.2.0/src/landfall.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-21 17:38:04.000000 landfall-0.2.0/src/landfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 15:03:08.553761 landfall-0.2.1/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.2.1/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-24 15:03:08.553911 landfall-0.2.1/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1348 2023-07-21 17:24:03.000000 landfall-0.2.1/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.2.1/pyproject.toml
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      871 2023-07-24 15:03:08.555961 landfall-0.2.1/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-02-28 17:08:57.000000 landfall-0.2.1/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 15:03:08.527670 landfall-0.2.1/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 15:03:08.542930 landfall-0.2.1/src/landfall/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      121 2023-07-24 15:01:36.000000 landfall-0.2.1/src/landfall/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.2.1/src/landfall/color.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.2.1/src/landfall/colorsys.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.2.1/src/landfall/distinctipy.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2550 2023-07-21 17:37:15.000000 landfall-0.2.1/src/landfall/points.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-24 15:03:08.553401 landfall-0.2.1/src/landfall.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      388 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.2.1/src/landfall.egg-info/not-zip-safe
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      156 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-24 15:03:08.000000 landfall-0.2.1/src/landfall.egg-info/top_level.txt
```

### Comparing `landfall-0.2.0/LICENSE` & `landfall-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `landfall-0.2.0/PKG-INFO` & `landfall-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `landfall-0.2.0/README.md` & `landfall-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `landfall-0.2.0/setup.cfg` & `landfall-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = landfall
-version = 0.2.0
+version = 0.2.1
 description = Easy to use functions to plot geospatial data on maps using staticmaps.
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 	landfall
 install_requires = 
 	py-staticmaps
 	more-itertools
 	tinytim
 	range_key_dict
 	distinctipy
+	Pillow<=9.5.0
 python_requires = >=3.8
 package_dir = 
 	=src
 zip_safe = no
 
 [options.extras_require]
 testing =
```

### Comparing `landfall-0.2.0/src/landfall/color.py` & `landfall-0.2.1/src/landfall/color.py`

 * *Files identical despite different names*

### Comparing `landfall-0.2.0/src/landfall/colorsys.py` & `landfall-0.2.1/src/landfall/colorsys.py`

 * *Files identical despite different names*

### Comparing `landfall-0.2.0/src/landfall/points.py` & `landfall-0.2.1/src/landfall/points.py`

 * *Files identical despite different names*

### Comparing `landfall-0.2.0/src/landfall.egg-info/PKG-INFO` & `landfall-0.2.1/src/landfall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

