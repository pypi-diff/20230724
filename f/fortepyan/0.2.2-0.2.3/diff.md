# Comparing `tmp/fortepyan-0.2.2.tar.gz` & `tmp/fortepyan-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortepyan-0.2.2.tar", last modified: Mon Jul 24 18:13:40 2023, max compression
+gzip compressed data, was "fortepyan-0.2.3.tar", last modified: Mon Jul 24 19:16:36 2023, max compression
```

## Comparing `fortepyan-0.2.2.tar` & `fortepyan-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.132414 fortepyan-0.2.2/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-24 18:13:40.128414 fortepyan-0.2.2/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.2/README.md
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.120414 fortepyan-0.2.2/fortepyan/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-07-24 18:13:13.000000 fortepyan-0.2.2/fortepyan/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.116414 fortepyan-0.2.2/fortepyan/analytics/
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan/analytics/clustering/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.2/fortepyan/analytics/clustering/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7845 2023-07-17 15:32:45.000000 fortepyan-0.2.2/fortepyan/analytics/clustering/process.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.2/fortepyan/analytics/clustering/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.2/fortepyan/analytics/clustering/views.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan/audio/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.2.2/fortepyan/audio/render.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.2/fortepyan/audio/soundfont.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.2/fortepyan/config.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.2/fortepyan/main.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan/midi/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.2/fortepyan/midi/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.2/fortepyan/midi/tools.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan/view/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      358 2023-07-24 18:12:33.000000 fortepyan-0.2.2/fortepyan/view/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.128414 fortepyan-0.2.2/fortepyan/view/animation/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.2/fortepyan/view/animation/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     3124 2023-07-24 06:40:43.000000 fortepyan-0.2.2/fortepyan/view/animation/dualroll.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.2/fortepyan/view/animation/evolution.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-07-24 18:09:37.000000 fortepyan-0.2.2/fortepyan/view/animation/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5091 2023-07-05 16:46:38.000000 fortepyan-0.2.2/fortepyan/view/animation/pianoroll.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.128414 fortepyan-0.2.2/fortepyan/view/pianoroll/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      126 2023-07-24 06:16:22.000000 fortepyan-0.2.2/fortepyan/view/pianoroll/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2373 2023-07-24 06:40:43.000000 fortepyan-0.2.2/fortepyan/view/pianoroll/dual.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5064 2023-07-24 05:44:31.000000 fortepyan-0.2.2/fortepyan/view/pianoroll/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     6102 2023-07-24 05:43:12.000000 fortepyan-0.2.2/fortepyan/view/pianoroll/structures.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan.egg-info/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      878 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/SOURCES.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/dependency_links.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      172 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/requires.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/top_level.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1474 2023-07-24 18:13:13.000000 fortepyan-0.2.2/pyproject.toml
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-07-24 18:13:40.132414 fortepyan-0.2.2/setup.cfg
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-24 19:16:36.280838 fortepyan-0.2.3/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.3/README.md
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-07-24 19:16:23.000000 fortepyan-0.2.3/fortepyan/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.276838 fortepyan-0.2.3/fortepyan/analytics/
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/analytics/clustering/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.3/fortepyan/analytics/clustering/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7845 2023-07-17 15:32:45.000000 fortepyan-0.2.3/fortepyan/analytics/clustering/process.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.3/fortepyan/analytics/clustering/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.3/fortepyan/analytics/clustering/views.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/audio/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.2.3/fortepyan/audio/render.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.3/fortepyan/audio/soundfont.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.3/fortepyan/config.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.3/fortepyan/main.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/midi/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.3/fortepyan/midi/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.3/fortepyan/midi/tools.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/view/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      358 2023-07-24 18:12:33.000000 fortepyan-0.2.3/fortepyan/view/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/view/animation/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.3/fortepyan/view/animation/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     3124 2023-07-24 06:40:43.000000 fortepyan-0.2.3/fortepyan/view/animation/dualroll.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.3/fortepyan/view/animation/evolution.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-07-24 18:09:37.000000 fortepyan-0.2.3/fortepyan/view/animation/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5091 2023-07-05 16:46:38.000000 fortepyan-0.2.3/fortepyan/view/animation/pianoroll.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/view/pianoroll/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      126 2023-07-24 06:16:22.000000 fortepyan-0.2.3/fortepyan/view/pianoroll/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2389 2023-07-24 19:16:08.000000 fortepyan-0.2.3/fortepyan/view/pianoroll/dual.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5064 2023-07-24 05:44:31.000000 fortepyan-0.2.3/fortepyan/view/pianoroll/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     6102 2023-07-24 05:43:12.000000 fortepyan-0.2.3/fortepyan/view/pianoroll/structures.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan.egg-info/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      878 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/SOURCES.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/dependency_links.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      172 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/requires.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/top_level.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1474 2023-07-24 19:16:23.000000 fortepyan-0.2.3/pyproject.toml
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-07-24 19:16:36.280838 fortepyan-0.2.3/setup.cfg
```

### Comparing `fortepyan-0.2.2/PKG-INFO` & `fortepyan-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.2.2
+Version: 0.2.3
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.2.2/README.md` & `fortepyan-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/analytics/clustering/process.py` & `fortepyan-0.2.3/fortepyan/analytics/clustering/process.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/analytics/clustering/structures.py` & `fortepyan-0.2.3/fortepyan/analytics/clustering/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/analytics/clustering/views.py` & `fortepyan-0.2.3/fortepyan/analytics/clustering/views.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/audio/render.py` & `fortepyan-0.2.3/fortepyan/audio/render.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/audio/soundfont.py` & `fortepyan-0.2.3/fortepyan/audio/soundfont.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/main.py` & `fortepyan-0.2.3/fortepyan/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/midi/structures.py` & `fortepyan-0.2.3/fortepyan/midi/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/midi/tools.py` & `fortepyan-0.2.3/fortepyan/midi/tools.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/view/animation/dualroll.py` & `fortepyan-0.2.3/fortepyan/view/animation/dualroll.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/view/animation/evolution.py` & `fortepyan-0.2.3/fortepyan/view/animation/evolution.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/view/animation/main.py` & `fortepyan-0.2.3/fortepyan/view/animation/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/view/animation/pianoroll.py` & `fortepyan-0.2.3/fortepyan/view/animation/pianoroll.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/view/pianoroll/dual.py` & `fortepyan-0.2.3/fortepyan/view/pianoroll/dual.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
 from cmcrameri import cm
 from matplotlib import pyplot as plt
 from matplotlib.colors import ListedColormap
 
-from fortepyan import MidiPiece
+from fortepyan.midi.structures import MidiPiece
 from fortepyan.view.pianoroll import main as pianoroll_view
 from fortepyan.view.pianoroll.structures import DualPianoRoll, FigureResolution
 
 
 def draw_dual_pianoroll(
     piece: MidiPiece,
     title: str = None,
```

### Comparing `fortepyan-0.2.2/fortepyan/view/pianoroll/main.py` & `fortepyan-0.2.3/fortepyan/view/pianoroll/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan/view/pianoroll/structures.py` & `fortepyan-0.2.3/fortepyan/view/pianoroll/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/fortepyan.egg-info/PKG-INFO` & `fortepyan-0.2.3/fortepyan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.2.2
+Version: 0.2.3
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.2.2/fortepyan.egg-info/SOURCES.txt` & `fortepyan-0.2.3/fortepyan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.2/pyproject.toml` & `fortepyan-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fortepyan"
-version = "0.2.2"
+version = "0.2.3"
 description = "Process MIDI piano with (almost) no pain"
 readme = "README.md"
 authors = [{ name = "Piano For AI", email = "roszcz+fortepyan@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -43,15 +43,15 @@
     "fortepyan.audio",
     "fortepyan.view.animation",
     "fortepyan.view.pianoroll",
     "fortepyan.analytics.clustering",
 ]
 
 [tool.bumpver]
-current_version = "0.2.2"
+current_version = "0.2.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

