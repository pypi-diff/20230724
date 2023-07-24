# Comparing `tmp/pyosutools-0.2.3.tar.gz` & `tmp/pyosutools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosutools-0.2.3.tar", last modified: Sun Jul 16 17:21:17 2023, max compression
+gzip compressed data, was "pyosutools-0.2.4.tar", last modified: Mon Jul 24 10:04:06 2023, max compression
```

## Comparing `pyosutools-0.2.3.tar` & `pyosutools-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-16 17:21:06.000000 pyosutools-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-16 17:21:17.441890 pyosutools-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:06.000000 pyosutools-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/pyosutools/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/pyosutools/beatmaps/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/beatmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/beatmaps/beatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/beatmaps/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/pyosutools/db/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/osu.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/pyosutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:21:17.441890 pyosutools-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.664161 pyosutools-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 10:03:53.000000 pyosutools-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-24 10:04:06.664161 pyosutools-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:53.000000 pyosutools-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.660161 pyosutools-0.2.4/pyosutools/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.664161 pyosutools-0.2.4/pyosutools/beatmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/beatmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/beatmaps/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/beatmaps/beatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/beatmaps/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.664161 pyosutools-0.2.4/pyosutools/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/osu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.664161 pyosutools-0.2.4/pyosutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:04:06.664161 pyosutools-0.2.4/setup.cfg
```

### Comparing `pyosutools-0.2.3/LICENSE` & `pyosutools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.3/PKG-INFO` & `pyosutools-0.2.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.3
+Version: 0.2.4
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.3/pyosutools/beatmaps/datatypes.py` & `pyosutools-0.2.4/pyosutools/beatmaps/datatypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
 from dataclasses import dataclass
 from aenum import IntFlag, Enum
-from typing import List, Tuple, Dict
+from typing import List, Tuple
 
 from pyosutools.datatypes import GameMode
 
 
 class HitObjectType(IntFlag):
     CIRCLE = 1 << 0
     SLIDER = 1 << 1
@@ -14,14 +15,15 @@
     MANIA_HOLD = 1 << 7
 
 
 class EventType(Enum):
     BACKGROUND = 0
     VIDEO = 1
     BREAK = 2
+    BACKGROUND_COLOUR = 3
 
 
 class HitSound(IntFlag):
     NORMAL = 1 << 0
     WHISTLE = 1 << 1
     FINISH = 1 << 2
     CLAP = 1 << 3
@@ -39,15 +41,15 @@
     CATMUL = 'C'
     LINEAR = 'L'
     PERFECT = 'P'
 
 
 @dataclass
 class GeneralSettings:
-    audio_filename: str
+    audio_filename: str = None
     audio_lead_in: int = 0
     audio_hash: str = None  # depricated
     preview_time: int = -1
     countdown: int = 1
     sample_set: str = "Normal"
     stack_leniency: float = 0.7
     mode: GameMode = 0
@@ -102,47 +104,45 @@
     start_time: int
 
 
 @dataclass
 class BackgroundEvent(BaseEvent):
     _id = 0
     filename: str
-    x_offset: int
-    y_offset: int
+    x_offset: int = 0
+    y_offset: int = 0
 
 
 @dataclass
 class VideoEvent(BaseEvent):
     _id = 1
     filename: str
-    x_offset: int
-    y_offset: int
+    x_offset: int = 0
+    y_offset: int = 0
 
 
 @dataclass
 class BreakEvent(BaseEvent):
     _id = 2
     end_time: int
 
 
 @dataclass
 class TimingPoint:
     time: int
     beat_length: float
     meter: int
-    sample_set: int  # 0 = beatmap default, 1 = normal, 2 = soft, 3 = drum
-    sample_index: int
-    volume: int
+    sample_set: HitSample
     uninherited: bool
     effects: int
 
 
 @dataclass
 class ComboColors:
-    combo: Dict[int, Tuple[int, int, int]]
+    combo: List[Tuple[int, int, int]]
     slider_track_override: Tuple[int, int, int] = None
     slider_border: Tuple[int, int, int] = None
 
 
 @dataclass
 class HitSample:
     normal_set: int
@@ -155,14 +155,16 @@
 @dataclass
 class BaseHitObject:
     x: int
     y: int
     time: int
     hit_sound: HitSound
     hit_sample: HitSample
+    new_combo: bool
+    combo_skips: int
 
 
 @dataclass
 class CircleObject(BaseHitObject):
     pass
 
 
@@ -186,11 +188,7 @@
 class SpinnerObject(BaseHitObject):
     end_time: int
 
 
 @dataclass
 class ManiaHoldObject(BaseHitObject):
     end_time: int
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `pyosutools-0.2.3/pyosutools/datatypes.py` & `pyosutools-0.2.4/pyosutools/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.3/pyosutools/db/collection.py` & `pyosutools-0.2.4/pyosutools/db/collection.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.3/pyosutools/db/datatypes.py` & `pyosutools-0.2.4/pyosutools/db/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.3/pyosutools/db/osu.py` & `pyosutools-0.2.4/pyosutools/db/osu.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.3/pyosutools/db/presence.py` & `pyosutools-0.2.4/pyosutools/db/presence.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.3/pyosutools/db/scores.py` & `pyosutools-0.2.4/pyosutools/db/scores.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.3/pyosutools/utils.py` & `pyosutools-0.2.4/pyosutools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,18 +73,17 @@
         return datetime.datetime.fromtimestamp((ticks-621355968000000000)/10_000_000, tz=datetime.timezone.utc)
     else:
         return datetime.datetime.min
 
 
 def is_int(text) -> bool:
     try:
-        assert int(text) == float(text)
+        return float(text).is_integer()
     except (ValueError, AssertionError):
         return False
-    return True
 
 
 def is_number(text) -> bool:
     try:
         float(text)
     except (ValueError):
         return False
```

### Comparing `pyosutools-0.2.3/pyosutools.egg-info/PKG-INFO` & `pyosutools-0.2.4/pyosutools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.3
+Version: 0.2.4
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.3/pyosutools.egg-info/SOURCES.txt` & `pyosutools-0.2.4/pyosutools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 pyosutools/__init__.py
 pyosutools/datatypes.py
+pyosutools/exceptions.py
 pyosutools/utils.py
 pyosutools.egg-info/PKG-INFO
 pyosutools.egg-info/SOURCES.txt
 pyosutools.egg-info/dependency_links.txt
 pyosutools.egg-info/requires.txt
 pyosutools.egg-info/top_level.txt
 pyosutools/beatmaps/__init__.py
+pyosutools/beatmaps/_parsers.py
 pyosutools/beatmaps/beatmap.py
 pyosutools/beatmaps/datatypes.py
 pyosutools/db/__init__.py
 pyosutools/db/collection.py
 pyosutools/db/datatypes.py
 pyosutools/db/osu.py
 pyosutools/db/presence.py
```

### Comparing `pyosutools-0.2.3/pyproject.toml` & `pyosutools-0.2.4/pyproject.toml`

 * *Files identical despite different names*

