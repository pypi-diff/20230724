# Comparing `tmp/fortepyan-0.2.1.tar.gz` & `tmp/fortepyan-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortepyan-0.2.1.tar", last modified: Wed Jul  5 16:50:11 2023, max compression
+gzip compressed data, was "fortepyan-0.2.2.tar", last modified: Mon Jul 24 18:13:40 2023, max compression
```

## Comparing `fortepyan-0.2.1.tar` & `fortepyan-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.319666 fortepyan-0.2.1/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-05 16:50:11.315666 fortepyan-0.2.1/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.1/README.md
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-07-05 16:49:56.000000 fortepyan-0.2.1/fortepyan/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/analytics/
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/analytics/clustering/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.1/fortepyan/analytics/clustering/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7846 2023-06-11 11:36:25.000000 fortepyan-0.2.1/fortepyan/analytics/clustering/process.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.1/fortepyan/analytics/clustering/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.1/fortepyan/analytics/clustering/views.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/audio/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.2.1/fortepyan/audio/render.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.1/fortepyan/audio/soundfont.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.1/fortepyan/config.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.1/fortepyan/main.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/midi/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.1/fortepyan/midi/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.1/fortepyan/midi/tools.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/view/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      208 2023-06-11 08:17:56.000000 fortepyan-0.2.1/fortepyan/view/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/view/animation/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.1/fortepyan/view/animation/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.1/fortepyan/view/animation/evolution.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      761 2023-06-11 08:41:24.000000 fortepyan-0.2.1/fortepyan/view/animation/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5091 2023-07-05 16:46:38.000000 fortepyan-0.2.1/fortepyan/view/animation/pianoroll.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan/view/pianoroll/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       65 2023-06-11 11:36:25.000000 fortepyan-0.2.1/fortepyan/view/pianoroll/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5568 2023-07-05 16:45:29.000000 fortepyan-0.2.1/fortepyan/view/pianoroll/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     3321 2023-07-05 16:48:53.000000 fortepyan-0.2.1/fortepyan/view/pianoroll/structures.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-05 16:50:11.315666 fortepyan-0.2.1/fortepyan.egg-info/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      808 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/SOURCES.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/dependency_links.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      157 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/requires.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-07-05 16:50:11.000000 fortepyan-0.2.1/fortepyan.egg-info/top_level.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1452 2023-07-05 16:49:56.000000 fortepyan-0.2.1/pyproject.toml
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-07-05 16:50:11.319666 fortepyan-0.2.1/setup.cfg
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.132414 fortepyan-0.2.2/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-24 18:13:40.128414 fortepyan-0.2.2/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.2/README.md
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.120414 fortepyan-0.2.2/fortepyan/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-07-24 18:13:13.000000 fortepyan-0.2.2/fortepyan/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.116414 fortepyan-0.2.2/fortepyan/analytics/
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan/analytics/clustering/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.2/fortepyan/analytics/clustering/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7845 2023-07-17 15:32:45.000000 fortepyan-0.2.2/fortepyan/analytics/clustering/process.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.2/fortepyan/analytics/clustering/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.2/fortepyan/analytics/clustering/views.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan/audio/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.2.2/fortepyan/audio/render.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.2/fortepyan/audio/soundfont.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.2/fortepyan/config.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.2/fortepyan/main.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan/midi/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.2/fortepyan/midi/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.2/fortepyan/midi/tools.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan/view/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      358 2023-07-24 18:12:33.000000 fortepyan-0.2.2/fortepyan/view/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.128414 fortepyan-0.2.2/fortepyan/view/animation/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.2/fortepyan/view/animation/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     3124 2023-07-24 06:40:43.000000 fortepyan-0.2.2/fortepyan/view/animation/dualroll.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.2/fortepyan/view/animation/evolution.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-07-24 18:09:37.000000 fortepyan-0.2.2/fortepyan/view/animation/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5091 2023-07-05 16:46:38.000000 fortepyan-0.2.2/fortepyan/view/animation/pianoroll.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.128414 fortepyan-0.2.2/fortepyan/view/pianoroll/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      126 2023-07-24 06:16:22.000000 fortepyan-0.2.2/fortepyan/view/pianoroll/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2373 2023-07-24 06:40:43.000000 fortepyan-0.2.2/fortepyan/view/pianoroll/dual.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5064 2023-07-24 05:44:31.000000 fortepyan-0.2.2/fortepyan/view/pianoroll/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     6102 2023-07-24 05:43:12.000000 fortepyan-0.2.2/fortepyan/view/pianoroll/structures.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 18:13:40.124414 fortepyan-0.2.2/fortepyan.egg-info/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      878 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/SOURCES.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/dependency_links.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      172 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/requires.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-07-24 18:13:40.000000 fortepyan-0.2.2/fortepyan.egg-info/top_level.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1474 2023-07-24 18:13:13.000000 fortepyan-0.2.2/pyproject.toml
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-07-24 18:13:40.132414 fortepyan-0.2.2/setup.cfg
```

### Comparing `fortepyan-0.2.1/PKG-INFO` & `fortepyan-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.2.1
+Version: 0.2.2
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.2.1/README.md` & `fortepyan-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/analytics/clustering/process.py` & `fortepyan-0.2.2/fortepyan/analytics/clustering/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 def get_gram_variants(
     gram: str,
     ngrams: NgramContainer,
 ) -> dict:
     idxs = np.where(ngrams.df.ngram == gram)[0]
     idxs = filter_overlaping_sequences(idxs, ngrams.n)
 
-    # Fuzzy-wuzzy extension of thee seeds, *threshold* is a measure
+    # Fuzzy-wuzzy extension of the seeds, *threshold* is a measure
     # of deviation between two sequences that are being compared
     # "if the sequence is extended further, next *threshold* notes
     # are going to be different between both sequences
     threshold = 4
     left_shifts, right_shifts = calculate_group_shifts(
         pitch_sequence=ngrams.pitch_sequence,
         idxs=idxs,
```

### Comparing `fortepyan-0.2.1/fortepyan/analytics/clustering/structures.py` & `fortepyan-0.2.2/fortepyan/analytics/clustering/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/analytics/clustering/views.py` & `fortepyan-0.2.2/fortepyan/analytics/clustering/views.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/audio/render.py` & `fortepyan-0.2.2/fortepyan/audio/render.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/audio/soundfont.py` & `fortepyan-0.2.2/fortepyan/audio/soundfont.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/main.py` & `fortepyan-0.2.2/fortepyan/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/midi/structures.py` & `fortepyan-0.2.2/fortepyan/midi/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/midi/tools.py` & `fortepyan-0.2.2/fortepyan/midi/tools.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/view/animation/evolution.py` & `fortepyan-0.2.2/fortepyan/view/animation/evolution.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/view/animation/main.py` & `fortepyan-0.2.2/fortepyan/view/animation/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import subprocess
 
 from fortepyan.audio.render import midi_to_mp3
 from fortepyan.midi.structures import MidiPiece
+from fortepyan.view.animation import dualroll as dualroll_animation
 from fortepyan.view.animation import pianoroll as pianoroll_animation
 
 
 def make_piano_roll_video(
     piece: MidiPiece,
     movie_path: str,
     title: str = "animation",
@@ -15,10 +16,35 @@
     mp3_path = midi_to_mp3(piece.to_midi())
 
     scene_frames_dir = scene.render_mp()
     command = f"""
         ffmpeg -y -f image2 -framerate 30 -i {str(scene_frames_dir)}/10%4d.png\
         -loglevel quiet -i {mp3_path} -map 0:v:0 -map 1:a:0\
         {movie_path}
+    """
+    print("Rendering a movie to file:", movie_path)
+    subprocess.call(command, shell=True)
+
+
+def make_dual_roll_video(
+    piece: MidiPiece,
+    movie_path: str,
+    title: str = "animation",
+    base_cmap: str = "PuBuGn",
+    marked_cmap: str = "Reds",
+):
+    scene = dualroll_animation.DualRollScene(
+        piece=piece,
+        title=title,
+        base_cmap=base_cmap,
+        marked_cmap=marked_cmap,
+    )
+    mp3_path = midi_to_mp3(piece.to_midi())
+
+    scene_frames_dir = scene.render_mp()
+    command = f"""
+        ffmpeg -y -f image2 -framerate 30 -i {str(scene_frames_dir)}/10%4d.png\
+        -loglevel quiet -i {mp3_path} -map 0:v:0 -map 1:a:0\
+        {movie_path}
     """
     print("Rendering a movie to file:", movie_path)
     subprocess.call(command, shell=True)
```

### Comparing `fortepyan-0.2.1/fortepyan/view/animation/pianoroll.py` & `fortepyan-0.2.2/fortepyan/view/animation/pianoroll.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.1/fortepyan/view/pianoroll/main.py` & `fortepyan-0.2.2/fortepyan/view/pianoroll/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import matplotlib
 import numpy as np
-import pandas as pd
 from matplotlib import pyplot as plt
 
 from fortepyan.midi.structures import MidiPiece
 from fortepyan.view.pianoroll.structures import PianoRoll, FigureResolution
 
 
 def draw_pianoroll_with_velocities(
@@ -53,34 +52,14 @@
         # TODO Logger
         print("Warning: playtime too long! Showing after trim")
         piece = piece.trim(0, duration_threshold)
 
     return piece
 
 
-def sanitize_midi_frame(mf: pd.DataFrame) -> pd.DataFrame:
-    # Do not modify input data
-    df = mf.copy()
-
-    # Make it start at 0.0
-    df.end -= df.start.min()
-    df.start -= df.start.min()
-    duration_in = df.end.max()
-
-    # 20 minutes?
-    duration_threshold = 1200
-    if duration_in > duration_threshold:
-        # TODO Logger
-        print("Warning: playtime to long! Showing after trim")
-        ids = df.end <= duration_threshold
-        df = df[ids]
-
-    return df
-
-
 def draw_piano_roll(
     ax: plt.Axes,
     piano_roll: PianoRoll,
     time: float = 0.0,
     cmap: str = "GnBu",
 ) -> plt.Axes:
     """
```

### Comparing `fortepyan-0.2.1/fortepyan.egg-info/PKG-INFO` & `fortepyan-0.2.2/fortepyan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.2.1
+Version: 0.2.2
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.2.1/fortepyan.egg-info/SOURCES.txt` & `fortepyan-0.2.2/fortepyan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,13 +14,15 @@
 fortepyan/analytics/clustering/views.py
 fortepyan/audio/render.py
 fortepyan/audio/soundfont.py
 fortepyan/midi/structures.py
 fortepyan/midi/tools.py
 fortepyan/view/__init__.py
 fortepyan/view/animation/__init__.py
+fortepyan/view/animation/dualroll.py
 fortepyan/view/animation/evolution.py
 fortepyan/view/animation/main.py
 fortepyan/view/animation/pianoroll.py
 fortepyan/view/pianoroll/__init__.py
+fortepyan/view/pianoroll/dual.py
 fortepyan/view/pianoroll/main.py
 fortepyan/view/pianoroll/structures.py
```

### Comparing `fortepyan-0.2.1/pyproject.toml` & `fortepyan-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fortepyan"
-version = "0.2.1"
+version = "0.2.2"
 description = "Process MIDI piano with (almost) no pain"
 readme = "README.md"
 authors = [{ name = "Piano For AI", email = "roszcz+fortepyan@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,14 +24,15 @@
     "numpy>=1.23.4",
     "pretty-midi>=0.2.9",
     "psycopg2>=2.9.5",
     "pydub>=0.25",
     "SQLAlchemy>=1.4.45",
     "matplotlib>=3.6.2",
     "Levenshtein>=0.20.9",
+    "cmcrameri>=1.5",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/Nospoko/fortepyan"
 
 [tool.setuptools]
@@ -42,15 +43,15 @@
     "fortepyan.audio",
     "fortepyan.view.animation",
     "fortepyan.view.pianoroll",
     "fortepyan.analytics.clustering",
 ]
 
 [tool.bumpver]
-current_version = "0.2.1"
+current_version = "0.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

