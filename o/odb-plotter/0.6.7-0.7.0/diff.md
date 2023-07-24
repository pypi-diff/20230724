# Comparing `tmp/odb-plotter-0.6.7.tar.gz` & `tmp/odb-plotter-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.6.7.tar", last modified: Thu Jul 13 19:01:02 2023, max compression
+gzip compressed data, was "odb-plotter-0.7.0.tar", last modified: Mon Jul 24 21:16:29 2023, max compression
```

## Comparing `odb-plotter-0.6.7.tar` & `odb-plotter-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.7/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     4253 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     2287 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-06-22 22:29:35.000000 odb-plotter-0.6.7/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.424299 odb-plotter-0.6.7/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.424299 odb-plotter-0.6.7/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     4253 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.7/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.7/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.7/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.7/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)    37876 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.7/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)    10576 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/src/odbp/py2_scripts/converter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5522 2023-07-13 17:33:44.000000 odb-plotter-0.6.7/src/odbp/py2_scripts/extractor.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3196 2023-07-13 17:33:44.000000 odb-plotter-0.6.7/src/odbp/py2_scripts/state_collector.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.7/src/odbp/reader.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.7/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.7/src/odbp/util.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3909 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/src/odbp/writer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-24 21:16:29.704798 odb-plotter-0.7.0/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.7.0/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     4237 2023-07-24 21:16:29.704798 odb-plotter-0.7.0/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     2271 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-07-24 21:16:29.704798 odb-plotter-0.7.0/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-24 21:16:29.701465 odb-plotter-0.7.0/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-24 21:16:29.701465 odb-plotter-0.7.0/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4237 2023-07-24 21:16:29.000000 odb-plotter-0.7.0/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      584 2023-07-24 21:16:29.000000 odb-plotter-0.7.0/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-07-24 21:16:29.000000 odb-plotter-0.7.0/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-07-24 21:16:29.000000 odb-plotter-0.7.0/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-07-24 21:16:29.000000 odb-plotter-0.7.0/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-24 21:16:29.704798 odb-plotter-0.7.0/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       43 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)      103 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    45246 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-24 21:16:29.704798 odb-plotter-0.7.0/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     5268 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      106 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      362 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/magic.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26202 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    23372 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/odb_settings.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     9214 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/process_input.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-24 21:16:29.704798 odb-plotter-0.7.0/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)    11461 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     6018 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/py2_scripts/extractor.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3111 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/py2_scripts/odb_info_getter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2575 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)      600 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/types.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     6428 2023-07-24 21:16:11.000000 odb-plotter-0.7.0/src/odbp/writer.py
```

### Comparing `odb-plotter-0.6.7/LICENSE` & `odb-plotter-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.7/PKG-INFO` & `odb-plotter-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.7
+Version: 0.7.0
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -78,12 +78,11 @@
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
     * 0.6.5: Fixing Python2 Error Reporting in more places
     * 0.6.6: Fixing conversion problems
     * 0.6.7: Implementing tools for .odbs with coords in only some steps or tools for frame steps with different sizes
+* 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5. Reqwrite CLI to use Python's cmd module and pyreadline/GNU readline.
 * Upcoming:
-    * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
-    * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
-    * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
+    * 1.1.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
```

### Comparing `odb-plotter-0.6.7/README.md` & `odb-plotter-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,12 +41,11 @@
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
     * 0.6.5: Fixing Python2 Error Reporting in more places
     * 0.6.6: Fixing conversion problems
     * 0.6.7: Implementing tools for .odbs with coords in only some steps or tools for frame steps with different sizes
+* 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5. Reqwrite CLI to use Python's cmd module and pyreadline/GNU readline.
 * Upcoming:
-    * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
-    * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
-    * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
+    * 1.1.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
```

### Comparing `odb-plotter-0.6.7/pyproject.toml` & `odb-plotter-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 [project.urls]
 "Homepage" = "https://www.cmml.me.msstate.edu"
 "Bug Reports" = "https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter/issues"
 "Source" = "https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter"
 
 [tool.setuptools]
-package-data = {odbp = ["data/views.toml", "data/config.toml", "py2_scripts/converter.py", "py2_scripts/extractor.py", "py2_scripts/state_collector.py",]}
+package-data = {odbp = ["data/views.toml", "data/config.toml", "py2_scripts/converter.py", "py2_scripts/extractor.py", "py2_scripts/odb_info_getter.py",]}
 
 [tool.setuptools.dynamic]
 version = {attr = "odbp.__version__"}
 
 [build-system]
 requires = ["setuptools", "wheel",]
 build-backend = "setuptools.build_meta"
```

### Comparing `odb-plotter-0.6.7/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.7.0/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.7
+Version: 0.7.0
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -78,12 +78,11 @@
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
     * 0.6.5: Fixing Python2 Error Reporting in more places
     * 0.6.6: Fixing conversion problems
     * 0.6.7: Implementing tools for .odbs with coords in only some steps or tools for frame steps with different sizes
+* 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5. Reqwrite CLI to use Python's cmd module and pyreadline/GNU readline.
 * Upcoming:
-    * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
-    * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
-    * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
+    * 1.1.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
```

### Comparing `odb-plotter-0.6.7/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.7.0/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 src/odb_plotter.egg-info/SOURCES.txt
 src/odb_plotter.egg-info/dependency_links.txt
 src/odb_plotter.egg-info/requires.txt
 src/odb_plotter.egg-info/top_level.txt
 src/odbp/__init__.py
 src/odbp/__main__.py
 src/odbp/cli.py
+src/odbp/magic.py
 src/odbp/odb.py
-src/odbp/odb_visualizer.py
+src/odbp/odb_settings.py
+src/odbp/process_input.py
 src/odbp/reader.py
-src/odbp/state.py
-src/odbp/util.py
+src/odbp/types.py
 src/odbp/writer.py
 src/odbp/data/config.toml
 src/odbp/data/views.toml
 src/odbp/py2_scripts/converter.py
 src/odbp/py2_scripts/extractor.py
-src/odbp/py2_scripts/state_collector.py
+src/odbp/py2_scripts/odb_info_getter.py
```

### Comparing `odb-plotter-0.6.7/src/odbp/data/config.toml` & `odb-plotter-0.7.0/src/odbp/data/config.toml`

 * *Files 24% similar despite different names*

```diff
@@ -8,40 +8,44 @@
 
 # Many values here are not set by default, and do not make much sense as
 # values in a global config file, but are useful as a template for input
 # files and also are here for completeness
 
 # Path (relative or absolute) to .hdf5 files
 # Default "." (present working directory)
-hdf_source_directory = "."
+hdf_source_dir = "."
 
 # Path (relative or absolute) to .odb files
 # Default "." (present working directory)
-odb_source_directory = "."
+odb_source_dir = "."
 
 # Path (relative or absolute) to the results directory
 # Default "results"
 # If this directory does not exist, it will be created
-results_directory = "results"
+result_dir = "results"
 
 # path to the .hdf5 file
 # Not set by default. Enter a value and uncomment to pass a default value
-# hdf =
+# hdf_path =
 
 # path to the .odb file
 # Not set by default. Enter a value and uncomment to pass a default value
-# odb =
+# odb_path =
 
 #####
-# parts, nodesets, and nodes cannot be easily set via the cli, and must be set
+# steps, parts, nodesets, and nodes cannot be easily set via the cli, and must be set
 # interactively or using this config file or another .toml input file
 
-# Parts from which to extract
-# By default, we can use the Abaqus default of "PART-1-1", but you can add whatever you'd like here
-parts = [ "PART-1-1", ]
+# Steps which to extract or convert.
+# Not set by default, which uses all available.
+# steps = []
+
+# Parts from which to extrat or convert
+# Not set by default, to use all available.
+# parts = []
 
 # Nodesets from which to extract
 # Not set by default, which will use all present nodesets
 # nodesets =
 
 # Custom nodesets to create and extract
 # Must be 0 or more arrays in a .toml table
@@ -53,121 +57,145 @@
 # Not set by default, which will extract all nodes present
 # [nodes]
 
 #####
 
 # lower x-axis extreme
 # Not set by default. Enter a value and uncomment to pass a default value
-# low_x =
+# x_low =
 
 # upper x-axis extreme
 # Not set by default. Enter a value and uncomment to pass a default value
-# high_x =
+# x_high =
 
 # lower y-axis extreme
 # Not set by default. Enter a value and uncomment to pass a default value
-# low_y =
+# y_low =
 
 # upper y-axis extreme
 # Not set by default. Enter a value and uncomment to pass a default value
-# high_y =
+# y_high =
 
 # lower z-axis extreme
 # Not set by default. Enter a value and uncomment to pass a default value
-# low_z =
+# z_low =
 
 # upper z-axis extreme
 # Not set by default. Enter a value and uncomment to pass a default value
-# high_z =
+# z_high =
 
 # lower time extreme
 # Defaulted to 0, as it can't be lower than this
-low_time = 0
+time_low = 0
 
 # upper time extreme
 # Defaulted to inf, as this will extract all times starting from time_low
-high_time = +inf
+time_high = +inf
 
 #####
 
 # In general, don't set temperatures with these files unless you are
 # using an input file to generate a .hdf5 file from a .odb file.
 # Otherwise, these values should be stored in your directory of .hdf5
 # files in their corresponding config files.
 
 # lower temperature extreme
 # Not set by default. Enter a value and uncomment to pass a default value
-# low_temp =
+# temp_low =
 
 # upper temperature extreme/melting point
 # Not set by default. Enter a value and uncomment to pass a default value
-# meltpoint =
-
-#####
-
-#####
-
-# A default time sample of 1 works, but should almost always be overwritten
-# Otherwise, you should rely on the corresponding config file with the .hdf5
+# temp_high =
 
 #####
 
 # time sampling interval (N for "extract every Nth frame")
 # Default value of 1, but expect this to almost always be overwritten
-time_sample = 1
+time_step = 1
 
 #####
 
+# Number of cpu cores to use for this process
+# Unset by default, which uses all available cores
+# cpus =
+
 # which program to run the abaqus python commands with
 # Defaults to "abaqus" but, for example, if you have both abaqus 2019 and 2022
 # installed, and use abaqus 2019, you would set this to "abq2019"
-abaqus_program = "abaqus"
+abaqus_executable = "abaqus"
 
-# Do you want to open the interative 3D viewer?
-# If not, PNG Images will be generated and saved automatically
-# Default true
-interactive = true
+# Which value in the .odb or .hdf5 refers to coordinates
+# Defaults to "COORD"
+coord_key = "COORD"
+
+# List of outputs which should be converted
+# Not set by default, which will convert all outputs
+# target_outputs = []
 
 # Which colormap to use for the plots
 # Default "turbo"
-colormap_name = "turbo"
+colormap = "turbo"
 
-# The title to save the images under
+# Should images be saved to hard drive
+# Default true
+save = true
+
+# In what format should images be saved?
+# Default ".png"
+save_format = ".png"
+
+# The filename to save the images under
 # Whatever you put will automatically have .png appended
 # By leaving this unset, you will automatically get 
-# <name of the .hdf5 file>.png
-# title =
+# <name of the .hdf5 file>
+# filename =
 
-# The label to display on the generated iamges
-# By leaving blank, this will be the title, without
+# The title to display on the generated iamges
+# By leaving blank, this will be the filename, without
 # the ".png"
-# label =
+# title =
 
-# Whether or not to run automatically when started
-# This will crash if not all necessary parameters are given
-# Default false
-run = false
+# The font to use on the plots
+# Defaults to "courier"
+font = "courier"
+
+# The color for fonts
+# Defaults to "#000000"
+font_color = "#000000"
+
+# The size of fonts
+# Defaults to 14.0
+font_size = 14.0
+
+# Background color for images
+# Defaults to "#FFFFFF"
+background_color = "#FFFFFF"
+
+# Above-range color for colormaps
+# Defaults to "#C0C0C0"
+above_range_color = "#C0C0C0"
+
+# Below-range color for colormaps
+# Not set by default
+# below_range_color = 
 
 # These are the viewing angles at which you can show the plot
 # These named values are set internally
-# Or, you can specify a 3-tuple value for a custom view
 # Possible values can be seen in the interactive plotter
 # They're also listed here for your convenience
-# Top
-# Bottom
-# Front
-# Back
-# Left
-# Right
-# Isometric Front-Right
-# Isometric Front-Left
-# Isometric Back-Right
-# Isometric Back-Left
-
-# Default is Isometric Front-Right
-view = "Isometric Front-Right"
-
-# A custom example
-#[view]
-#    elev = 90
-#    azim = 45
-#    roll = -45
+# "isometric"
+# "negative isometric"
+# "xy"
+# "negative xy"
+# "xz"
+# "negative xz"
+# "yx"
+# "negative yx"
+# "yz"
+# "negative yz"
+# "zx"
+# "negative zx"
+# "zy"
+# "negative zy"
+
+# Default is isometric
+view = "isometric"
```

### Comparing `odb-plotter-0.6.7/src/odbp/py2_scripts/converter.py` & `odb-plotter-0.7.0/src/odbp/py2_scripts/converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,16 +62,14 @@
     if unicode_nodesets is not None:
         user_nodesets = list()
         for nodeset in unicode_nodesets:
             user_nodesets.append(str(nodeset))
     else:
         user_nodesets = None
 
-    user_frames = input_dict.get("frames")
-
     unicode_parts = input_dict.get("parts")
     if unicode_parts is not None:
         user_parts = list()
         for part in unicode_parts:
             user_parts.append(str(part))
     else:
         user_parts = None
@@ -81,26 +79,31 @@
         user_steps = list()
         for step in unicode_steps:
             user_steps.append(str(step))
     else:
         user_steps = None
 
     coord_key = str(input_dict.get("coord_key", "COORD"))
-    temp_key = str(input_dict.get("temp_key", "NT11"))
+    target_outputs = input_dict.get("target_outputs", ["NT11"])
+    if isinstance(target_outputs, collections.Iterable):
+        target_outputs = [str(key) for key in target_outputs]
+    elif isinstance(target_outputs, str):
+        target_outputs = [str(target_outputs)]
     num_cpus = int(input_dict.get("cpus"))
+    time_step = int(input_dict.get("time_step", 1))
 
-    result_name = convert_odb_to_npz(odb_path, user_nodesets, user_nodes, user_frames, user_parts, user_steps, coord_key, temp_key, num_cpus)
+    result_name = convert_odb_to_npz(odb_path, user_nodesets, user_nodes, user_parts, user_steps, coord_key, target_outputs, num_cpus, time_step)
     try:
         result_file = open(result_path, "wb")
         pickle.dump(result_name, result_file)
     finally:
         result_file.close()
 
 
-def convert_odb_to_npz(odb_path, user_nodesets, user_nodes, user_frames, user_parts, user_steps, coord_key, temp_key, num_cpus):
+def convert_odb_to_npz(odb_path, user_nodesets, user_nodes, user_parts, user_steps, coord_key, target_outputs, num_cpus, time_step):
     """
     Based on the 4 lists given, convert the .odb data to .npz files
     odb_path: str path to the .odb file
     user_parts: list[str] which parts to convert (default to all)
     user_nodesets: list[str] which nodesets to convert (default to all)
     user_nodes: list[int] which nodes to turn into a new nodeset (default to None)
     frames: list[int] which frames to convert (default to all)
@@ -110,17 +113,17 @@
     """
 
     # Create the results directory
     parent_dir = os.path.join(os.getcwd(), "tmp_npz")
     if not os.path.exists(parent_dir):
         os.mkdir(parent_dir)
 
-    temps_dir = os.path.join(parent_dir, "temps")
-    if not os.path.exists(temps_dir):
-        os.mkdir(temps_dir)
+    data_dir = os.path.join(parent_dir, "data")
+    if not os.path.exists(data_dir):
+        os.mkdir(data_dir)
 
     time_dir = os.path.join(parent_dir, "step_frame_times")
     if not os.path.exists(time_dir):
         os.mkdir(time_dir)
 
     try:
         odb = openOdb(odb_path, readOnly=True)
@@ -129,37 +132,42 @@
         print("Abaqus Error:")
         print(e)
         sys.exit(1)
 
     try:
         steps = odb.steps
 
-        base_times = [
-            (step_key, step_val.totalTime) for step_key, step_val in steps.items()
-            ]
-
+        base_times = list()
+        total_idx = 0
+        for step_key, step_val in steps.items():
+            base_times.append((step_key, step_val.totalTime, total_idx))
+            total_idx += len(step_val.frames)
+            
+        max_idx = base_times[-1][2] + len(steps[base_times[-1][0]].frames) - 1
         assembly = odb.rootAssembly
 
-        target_frames = set()
+        target_frames = dict()
         if user_steps is not None:
             for step in user_steps:
                 step_data = steps[step]
+                target_frames[step] = set()
                 for frame in step_data.frames:
-                    target_frames.add(frame.frameId)
+                    target_frames[step].add(frame.frameId)
 
-        if user_frames is not None:
-            for frame in user_frames:
-                target_frames.add(frame.frameId)
-
-        target_frames = sorted(list(target_frames))
-
-        if len(target_frames) == 0:
-            for step_data in steps.values():
-                for i, _ in enumerate(step_data.frames):
-                    target_frames.append(i) 
+            for step in target_frames:
+                target_frames[step] = sorted(list(target_frames[step]))
+
+        else:
+            for step, step_data in steps.items():
+                target_frames[step] = list()
+                for frame in step_data.frames:
+                    target_frames[step].append(frame.frameId)
+
+        for step in target_frames:
+            target_frames[step] = target_frames[step][::time_step]
 
         target_nodesets = set()
         if user_nodes is not None:
             if isinstance(user_nodes, collections.Mapping):
                 for key, val in user_nodes.items():
                     assembly.NodeSetFromNodeLabels(name=key, nodeLabels=(val,))
                     target_nodesets.add(key)
@@ -179,58 +187,59 @@
             for nodeset in user_nodesets:
                 target_nodesets.add(nodeset)
 
         target_nodesets = sorted(list(target_nodesets))
 
         if len(target_nodesets) == 0:
             target_nodesets = list(assembly.nodeSets.keys())
+            
+        if target_outputs is None or len(target_outputs) == 0:
+            target_outputs = list(steps[steps.keys()[0]].frames[0].fieldOutputs.keys())
+            target_outputs.remove(coord_key)
 
     finally:
         odb.close()
 
     for nodeset in target_nodesets:
-        for step_key, base_time in base_times:
+        for step_key, base_time, base_idx in base_times:
             coord_file = os.path.join(parent_dir, "node_coords.npz")
             read_nodeset_coords(odb_path, nodeset, coord_file, step_key, coord_key)
-            read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, target_frames, nodeset, temp_key, num_cpus)
+            read_step_data(odb_path, data_dir, time_dir, step_key, base_time, base_idx, max_idx, target_frames[step_key], nodeset, target_outputs, num_cpus)
 
     return parent_dir
 
 
-def read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, target_frames, nodeset, temp_key, num_cpus):
+def read_step_data(odb_path, data_dir, time_dir, step_key, base_time, base_idx, max_idx, target_frames, nodeset, target_outputs, num_cpus):
     try:
         odb = openOdb(odb_path, readOnly=True)
 
     except Exception as e:
         print("Abaqus Error:")
         print(e)
         sys.exit(1)
 
     try:
         steps = odb.steps
 
-        curr_step_dir = os.path.join(temps_dir, step_key)
+        curr_step_dir = os.path.join(data_dir, step_key)
         if not os.path.exists(curr_step_dir):
             os.mkdir(curr_step_dir)
 
-        max_frame = max(target_frames)
-
-        max_pad = len(str(max_frame))
+        max_pad = len(str(max_idx))
 
         manager = multiprocessing.Manager()
         frame_times = manager.list()
         if len(steps[step_key].frames) > 0:
-            idx_list = [i for i in range(len(steps[step_key].frames))]
-            idx_list_len = len(idx_list)
+            frame_list_len = len(target_frames)
             # TODO: what if the length isn't divisible by the number of processors (is it now?)
-            final_idx_list = [idx_list[i: i + int(idx_list_len / num_cpus)] for i in range(0, idx_list_len, max(int(idx_list_len / num_cpus), 1))]
+            combined_frame_list = [target_frames[i: i + max(int(frame_list_len / num_cpus), 1)] for i in range(0, frame_list_len, max(int(frame_list_len / num_cpus), 1))]
 
             temp_procs = list()
-            for idx_list in final_idx_list:
-                p = multiprocessing.Process(target=read_single_frame_temp, args=(odb_path, idx_list, max_pad, target_frames, step_key, curr_step_dir, frame_times, base_time, nodeset, temp_key))
+            for frame_list in combined_frame_list:
+                p = multiprocessing.Process(target=read_single_frame_temp, args=(odb_path, frame_list, max_pad, step_key, curr_step_dir, frame_times, base_time, base_idx, nodeset, target_outputs))
                 p.start()
                 temp_procs.append(p)
 
             for p in temp_procs:
                 p.join()
 
             np.savez_compressed(
@@ -247,48 +256,49 @@
                     )
                 )
 
     finally:
         odb.close()
 
 
-def read_single_frame_temp(odb_path, idx_list, max_pad, target_frames, step_key, curr_step_dir, frame_times, base_time, nodeset, temp_key):
+def read_single_frame_temp(odb_path, frame_list, max_pad, step_key, curr_step_dir, frame_times, base_time, base_idx, nodeset, target_outputs):
 
     try:
         odb = openOdb(odb_path, readOnly=True)
 
     except Exception as e:
         print("Abaqus Error:")
         print(e)
         sys.exit(1)
 
     try:
         steps = odb.steps
         assembly = odb.rootAssembly
 
-        for idx in idx_list:
-            if idx not in target_frames:
+        for idx, frame in enumerate(steps[step_key].frames):
+            if frame.frameId not in frame_list:
                 continue
-            
-            frame = steps[step_key].frames[idx]
-
-            field = frame.fieldOutputs[temp_key].getSubset(region=assembly.nodeSets[nodeset])
-            frame_times.append(float(format(round(frame.frameValue + base_time, 5), ".2f")))
-            node_temps = list()
-            for item in field.values:
-                temp = item.data
-                node_temps.append(temp)
-
-            num = str(idx + 1).zfill(max_pad)
-            np.savez_compressed(
-                    os.path.join(
-                        curr_step_dir,
-                        "frame_{}".format(num)
+                
+            frame_times.append(float(format(round(frame.frameValue + base_time, 5), ".2f")))    
+            for output in target_outputs:
+                field = frame.fieldOutputs[output].getSubset(region=assembly.nodeSets[nodeset])
+                node_vals = list()
+                for item in field.values:
+                    val = item.data
+                    node_vals.append(val)
+
+
+                if len(node_vals) > 0:
+                    num = str(idx + base_idx).zfill(max_pad)
+                    np.savez_compressed(
+                        os.path.join(
+                            curr_step_dir,
+                            "{}_{}".format(output, num)
                         ),
-                    np.array(node_temps)
+                        np.array(node_vals)
                     )
 
     finally:
         odb.close()
 
 
 def read_nodeset_coords(odb_path, nodeset, coord_file, step_key, coord_key):
@@ -327,8 +337,8 @@
                 pass
 
         finally:
             odb.close()
 
     
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `odb-plotter-0.6.7/src/odbp/py2_scripts/extractor.py` & `odb-plotter-0.7.0/src/odbp/py2_scripts/extractor.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,16 +43,14 @@
     if unicode_nodesets is not None:
         user_nodesets = list()
         for nodeset in unicode_nodesets:
             user_nodesets.append(str(nodeset))
     else:
         user_nodesets = None
 
-    user_frames = input_dict.get("frames")
-
     unicode_parts = input_dict.get("parts")
     if unicode_parts is not None:
         user_parts = list()
         for part in unicode_parts:
             user_parts.append(str(part))
     else:
         user_parts = None
@@ -61,45 +59,48 @@
     if unicode_steps is not None:
         user_steps = list()
         for step in unicode_steps:
             user_steps.append(str(step))
     else:
         user_steps = None
 
-    temp_key = str(input_dict.get("temp_key", "NT11"))
+    target_outputs = str(input_dict.get("target_outputs", ["NT11"]))
 
     try:
         odb = openOdb(odb_path, readOnly=True)
 
     except Exception as e:
         print("Abaqus Error:")
         print(e)
         sys.exit(1)
 
     try:
         steps = odb.steps
         assembly = odb.rootAssembly
 
-        target_frames = set()
+        target_frames = dict()
         if user_steps is not None:
             for step in user_steps:
                 step_data = steps[step]
+                target_frames[step] - set()
                 for frame in step_data.frames:
-                    target_frames.add(frame.frameId)
-
-        if user_frames is not None:
-            for frame in user_frames:
-                target_frames.add(frame.frameId)
+                    target_frames[step].add(frame.frameId)
 
-        target_frames = sorted(list(target_frames))
+            for step in target_frames():
+                target_frames[step] = sorted(list(target_frames[step]))
 
-        if len(target_frames) == 0:
-            for step_data in steps.values():
+        else:
+            for step, step_data in steps.items():
+                target_frames[step] = list()
                 for frame in step_data.frames:
-                    target_frames.append(frame.frameId) 
+                    target_frames[step].append(frame.frameId)
+
+        time_step = int(input_dict.get("time_step"), 1)
+        for step in target_frames:
+            target_frames[step] = target_frames[step][::time_step]
 
         target_nodesets = set()
         if user_nodes is not None:
             if isinstance(user_nodes, collections.Mapping):
                 for key, val in user_nodes.items():
                     assembly.NodeSetFromNodeLabels(name=key, nodeLabels=(val,))
                     target_nodesets.add(key)
@@ -123,54 +124,57 @@
 
         if len(target_nodesets) == 0:
             target_nodesets = list(assembly.nodeSets.keys())
 
     finally:
         odb.close()
 
-    extract(odb_path, save_path, target_nodesets, target_frames, temp_key)
+    extract(odb_path, save_path, target_nodesets, target_frames, target_outputs)
 
 
-def extract(odb_path, save_path, target_nodesets, target_frames, temp_key):
+def extract(odb_path, save_path, target_nodesets, target_frames, target_outputs):
 
     try:
         odb = openOdb(odb_path, readOnly=True)
 
     except Exception as e:
         print("Abaqus Error:")
         print(e)
         sys.exit(1)
 
     try:
         steps = odb.steps
         assembly = odb.rootAssembly
 
-        final_record = list()
-        for step in steps.keys():
-            step_start_time = steps[step].totalTime
-            for frame in steps[step].frames:
-                if frame.frameId not in target_frames:
-                    continue
-                frame_time = step_start_time + frame.frameValue
-                selected_temp_results = frame.fieldOutputs[temp_key]
-                for nodeset in target_nodesets:
-
-                    region = assembly.nodeSets[nodeset]
-                    temp_subset = selected_temp_results.getSubset(region=region)
-                    temp = np.copy(temp_subset.bulkDataBlocks[0].data).astype("float64")
-                    temp[temp == 0] = np.nan
-                    temp[temp == 300] = np.nan
-                    temp = temp[~np.isnan(temp)]
-
-                    final_record.append({
-                        "time": frame_time,
-                        "max": np.max(temp) if len(temp) > 0 else np.nan,
-                        "mean": np.mean(temp) if len(temp) > 0 else np.nan,
-                        "min": np.min(temp) if len(temp) > 0 else np.nan,
-                    })
+        final_record = dict()
+        for output in target_outputs:
+            final_record[output] = list()
+            for step in steps.keys():
+                step_start_time = steps[step].totalTime
+                for frame in steps[step].frames:
+                    if frame.frameId not in target_frames[step]:
+                        continue
+                    frame_time = step_start_time + frame.frameValue
+                    selected_output_results = frame.fieldOutputs[output]
+                    for nodeset in target_nodesets:
+
+                        region = assembly.nodeSets[nodeset]
+                        output_subset = selected_output_results.getSubset(region=region)
+                        output_vals = np.copy(output_subset.bulkDataBlocks[0].data).astype("float64")
+                        if output in ("NT11",):
+                            output_vals[output_vals == 0] = np.nan
+                            output_vals[output_vals == 300] = np.nan
+                        output_vals = output_vals[~np.isnan(output_vals)]
+
+                        final_record[output].append({
+                            "time": frame_time,
+                            "max": np.max(output_vals) if len(output_vals) > 0 else np.nan,
+                            "mean": np.mean(output_vals) if len(output_vals) > 0 else np.nan,
+                            "min": np.min(output_vals) if len(output_vals) > 0 else np.nan,
+                        })
 
     finally:
         odb.close()
 
     try:
         save_file = open(save_path, "wb")
         pickle.dump(final_record, save_file, protocol=2)
```

### Comparing `odb-plotter-0.6.7/src/odbp/py2_scripts/state_collector.py` & `odb-plotter-0.7.0/src/odbp/py2_scripts/odb_info_getter.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 from odbAccess import openOdb
 
 def main():
     input_args = "input args"
     parser = argparse.ArgumentParser()
     parser.add_argument(input_args, nargs="*")
     odb_path, result_path = vars(parser.parse_args())[input_args]
-    results = collect_state(odb_path)
+    results = get_odb_info(odb_path)
     try:
         result_file = open(result_path, "wb")
         pickle.dump(results, result_file)
     finally:
         result_file.close()
 
-def collect_state(odb_path):
+def get_odb_info(odb_path):
     result = dict()
     try:
         odb = openOdb(odb_path, readOnly=True)
 
     except Exception as e:
         print("Abaqus Error:")
         print(e)
@@ -48,29 +48,29 @@
         # What are our targets:
         # Frames
         # Steps --> Frames
         # Nodesets
         # Parts --> Nodesets
         # # Nodes --> Nodesets
         steps = odb.steps
-        steps_to_lens = dict()
-        steps_to_frames = dict()
+        step_lens = dict()
         all_frames = list()
         all_parts = list()
         frame_keys = list()
+        frame_keys_per_step = dict()
+        frame_range = 0
         for step_key, step_data in steps.items():
-            steps_to_lens[step_key] = len(step_data.frames)
-
-        frame_keys = list(steps[steps.keys()[0]].frames[0].fieldOutputs.keys())
-
-        prev = 0
-        for s, l in steps_to_lens.items():
-            all_frames.append((prev, l + prev))
-            steps_to_frames[s] = (prev, l + prev)
-            prev += l + 1
+            step_lens[step_key] = len(step_data.frames)
+            frame_range += step_lens[step_key]
+            frame_keys_per_step[step_key] = list(step_data.frames[0].fieldOutputs.keys())
+
+        for v in frame_keys_per_step.values():
+            for k in v:
+                if k not in frame_keys:
+                    frame_keys.append(k)
 
         assembly = odb.rootAssembly
         nodesets = assembly.nodeSets.keys()
 
         all_parts = assembly.instances.keys()
 
         all_nodes = list()
@@ -78,21 +78,19 @@
         for key in all_parts:
             parts_to_nodes[key] = list()
             for node in assembly.instances[key].nodes:
                 parts_to_nodes[key].append(node.label)
                 all_nodes.append(node.label)
 
         #Temporal
-        result["frame_range"] = (all_frames[0][0], all_frames[-1][-1])
         result["frame_keys"] = frame_keys
-        result["step_names"] = list(steps_to_frames.keys())
-        frame_ranges_per_steps = dict()
-        for s, f in steps_to_frames.items():
-            frame_ranges_per_steps[s] = f
-        result["frame_ranges_per_steps"] = frame_ranges_per_steps 
+        result["frame_keys_per_step"] = frame_keys_per_step
+        result["frame_range"] = frame_range
+        result["step_names"] = list(step_lens.keys())
+        result["step_lens"] = step_lens
         
         #Spatial
         result["nodeset_names"] = nodesets
         result["part_names"] = list(all_parts)
 
         result["node_range"] = (all_nodes[0], all_nodes[-1])
         node_ranges_per_part = dict()
```

