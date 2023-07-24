# Comparing `tmp/pymov2gif-0.0.1.tar.gz` & `tmp/pymov2gif-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymov2gif-0.0.1.tar", last modified: Sun Feb 13 23:50:57 2022, max compression
+gzip compressed data, was "pymov2gif-0.0.2.tar", last modified: Mon Jul 24 03:27:02 2023, max compression
```

## Comparing `pymov2gif-0.0.1.tar` & `pymov2gif-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 23:50:57.197010 pymov2gif-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-02-13 23:50:54.000000 pymov2gif-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-02-13 23:50:54.000000 pymov2gif-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-02-13 23:50:57.197010 pymov2gif-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-02-13 23:50:54.000000 pymov2gif-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 23:50:57.197010 pymov2gif-0.0.1/pymov2gif/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-02-13 23:50:54.000000 pymov2gif-0.0.1/pymov2gif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-02-13 23:50:54.000000 pymov2gif-0.0.1/pymov2gif/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-02-13 23:50:57.197010 pymov2gif-0.0.1/pymov2gif/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-02-13 23:50:54.000000 pymov2gif-0.0.1/pymov2gif/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-13 23:50:57.197010 pymov2gif-0.0.1/pymov2gif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-02-13 23:50:57.000000 pymov2gif-0.0.1/pymov2gif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-02-13 23:50:57.000000 pymov2gif-0.0.1/pymov2gif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-13 23:50:57.000000 pymov2gif-0.0.1/pymov2gif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-02-13 23:50:57.000000 pymov2gif-0.0.1/pymov2gif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-13 23:50:57.000000 pymov2gif-0.0.1/pymov2gif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-02-13 23:50:57.197010 pymov2gif-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-02-13 23:50:56.000000 pymov2gif-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-02-13 23:50:54.000000 pymov2gif-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:27:02.609534 pymov2gif-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 03:26:59.000000 pymov2gif-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 03:26:59.000000 pymov2gif-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-24 03:27:02.609534 pymov2gif-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-24 03:26:59.000000 pymov2gif-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:27:02.609534 pymov2gif-0.0.2/pymov2gif/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-24 03:26:59.000000 pymov2gif-0.0.2/pymov2gif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-24 03:26:59.000000 pymov2gif-0.0.2/pymov2gif/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 03:27:02.609534 pymov2gif-0.0.2/pymov2gif/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:27:02.609534 pymov2gif-0.0.2/pymov2gif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-24 03:27:02.000000 pymov2gif-0.0.2/pymov2gif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 03:27:02.000000 pymov2gif-0.0.2/pymov2gif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:27:02.000000 pymov2gif-0.0.2/pymov2gif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 03:27:02.000000 pymov2gif-0.0.2/pymov2gif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 03:27:02.000000 pymov2gif-0.0.2/pymov2gif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 03:27:02.609534 pymov2gif-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-24 03:27:02.000000 pymov2gif-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-24 03:26:59.000000 pymov2gif-0.0.2/versioneer.py
```

### Comparing `pymov2gif-0.0.1/LICENSE` & `pymov2gif-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymov2gif-0.0.1/README.md` & `pymov2gif-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pymov2gif
 Convert `*.mov` to `*.gif`:
 
 ## Web Interface 
-[![Open-with-Voila](https://img.shields.io/badge/Open%20with-Voila-4eafa0.svg)](https://mybinder.org/v2/gh/jan-janssen/pymov2gif/master?urlpath=/voila/render/app.ipynb)
+[![Open-with-Voila](https://img.shields.io/badge/Open%20with-Voila-4eafa0.svg)](https://mybinder.org/v2/gh/jan-janssen/pymov2gif/main?urlpath=/voila/render/app.ipynb)
 
 ![Preview](convert.gif) 
 
 ## Python Interface 
 To integrate the functionality in your project, just import the `convert` function: 
 ```
 from pymov2gif import convert
@@ -28,9 +28,13 @@
 * `--resolution`: Resolution of the output *.gif file - default: 800x600
 * `--framerate`: Framerate of the output *.gif file - default: 10
 * `--output_filename`: Filename of the output *.gif file - optional 
 
 ## Installation 
 Both the python interface and the command line interface require `pymov2gif` to be installed via `pip`:
 ```
-pip install git+https://github.com/pyscioffice/mov2gif.git
+pip install pymov2gif
+```
+Alternatively, `pymov2gif` can be installed using conda-forge:
+```
+conda -c conda-forge pymov2gif
 ```
```

### Comparing `pymov2gif-0.0.1/pymov2gif/__main__.py` & `pymov2gif-0.0.2/pymov2gif/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
 Convert *.mov files to *.gif format
 """
 import argparse
-from pymov2gif.convert import convert
+from pymov2gif import convert
 
 
 def command_line_parser():
     """
     Main function primarly used for the command line interface
     """
     parser = argparse.ArgumentParser(prog="pymov2gif")
     parser.add_argument(
         "file",
         help="Video file to be converted - in *.mov format.",
     )
     parser.add_argument(
         "-r",
         "--resolution",
-        action="store_true",
         help="Resolution of the output *.gif file - default: 800x600",
     )
     parser.add_argument(
         "-f",
         "--framerate",
         help="Framerate of the output *.gif file - default: 10",
     )
```

### Comparing `pymov2gif-0.0.1/pymov2gif/convert.py` & `pymov2gif-0.0.2/pymov2gif/__init__.py`

 * *Files identical despite different names*

### Comparing `pymov2gif-0.0.1/versioneer.py` & `pymov2gif-0.0.2/versioneer.py`

 * *Files identical despite different names*

