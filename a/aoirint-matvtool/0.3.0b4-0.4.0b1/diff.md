# Comparing `tmp/aoirint_matvtool-0.3.0b4.tar.gz` & `tmp/aoirint_matvtool-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aoirint_matvtool-0.3.0b4.tar", max compression
+gzip compressed data, was "aoirint_matvtool-0.4.0b1.tar", max compression
```

## Comparing `aoirint_matvtool-0.3.0b4.tar` & `aoirint_matvtool-0.4.0b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/LICENSE
--rw-r--r--   0        0        0     7079 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/README.md
--rw-r--r--   0        0        0       29 2023-07-24 02:21:09.217930 aoirint_matvtool-0.3.0b4/aoirint_matvtool/__init__.py
--rw-r--r--   0        0        0      104 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/config.py
--rw-r--r--   0        0        0     3004 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/crop_scale.py
--rw-r--r--   0        0        0     5008 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/find_image.py
--rw-r--r--   0        0        0     1345 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/fps.py
--rw-r--r--   0        0        0     6029 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/inputs.py
--rw-r--r--   0        0        0     1278 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/key_frames.py
--rw-r--r--   0        0        0        0 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/scripts/__init__.py
--rw-r--r--   0        0        0    15229 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/scripts/cli.py
--rw-r--r--   0        0        0     2305 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/select_audio.py
--rw-r--r--   0        0        0     2140 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/slice.py
--rw-r--r--   0        0        0     3914 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/util.py
--rw-r--r--   0        0        0     1069 2023-07-24 02:21:09.221931 aoirint_matvtool-0.3.0b4/pyproject.toml
--rw-r--r--   0        0        0     7685 1970-01-01 00:00:00.000000 aoirint_matvtool-0.3.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/LICENSE
+-rw-r--r--   0        0        0     7079 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/README.md
+-rw-r--r--   0        0        0       29 2023-07-24 07:40:53.639804 aoirint_matvtool-0.4.0b1/aoirint_matvtool/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/config.py
+-rw-r--r--   0        0        0     3004 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/crop_scale.py
+-rw-r--r--   0        0        0     5008 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/find_image.py
+-rw-r--r--   0        0        0     1345 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/fps.py
+-rw-r--r--   0        0        0     6029 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/inputs.py
+-rw-r--r--   0        0        0     1278 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/key_frames.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/scripts/__init__.py
+-rw-r--r--   0        0        0    15375 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/scripts/cli.py
+-rw-r--r--   0        0        0     2305 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/select_audio.py
+-rw-r--r--   0        0        0     2140 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/slice.py
+-rw-r--r--   0        0        0     3914 2023-07-24 07:40:38.115895 aoirint_matvtool-0.4.0b1/aoirint_matvtool/util.py
+-rw-r--r--   0        0        0     1069 2023-07-24 07:40:53.643804 aoirint_matvtool-0.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     7685 1970-01-01 00:00:00.000000 aoirint_matvtool-0.4.0b1/PKG-INFO
```

### Comparing `aoirint_matvtool-0.3.0b4/LICENSE` & `aoirint_matvtool-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/README.md` & `aoirint_matvtool-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/crop_scale.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/crop_scale.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/find_image.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/find_image.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/fps.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/fps.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/inputs.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/inputs.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/key_frames.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/key_frames.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/scripts/cli.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/scripts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import sys
 from argparse import ArgumentParser, Namespace
 from datetime import timedelta
 from pathlib import Path
 
+from aoirint_matvtool import __VERSION__ as PACKAGE_VERSION
 from aoirint_matvtool import config
 from aoirint_matvtool.crop_scale import FfmpegCropScaleResult, ffmpeg_crop_scale
 from aoirint_matvtool.find_image import (
     FfmpegBlackframeOutputLine,
     FfmpegProgressLine,
     ffmpeg_find_image_generator,
 )
@@ -327,14 +328,15 @@
         if tqdm_pbar is not None:
             tqdm_pbar.close()
 
 
 def main() -> None:
     parser = ArgumentParser()
     parser.add_argument("-l", "--log_level", type=int, default=logging.INFO)
+    parser.add_argument("-v", "--version", action="version", version=PACKAGE_VERSION)
     parser.add_argument("--ffmpeg_path", type=str, default=config.FFMPEG_PATH)
     parser.add_argument("--ffprobe_path", type=str, default=config.FFPROBE_PATH)
 
     subparsers = parser.add_subparsers()
 
     parser_input = subparsers.add_parser("input")
     parser_input.add_argument("-i", "--input_path", type=str, required=True)
```

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/select_audio.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/select_audio.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/slice.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/slice.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/aoirint_matvtool/util.py` & `aoirint_matvtool-0.4.0b1/aoirint_matvtool/util.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b4/pyproject.toml` & `aoirint_matvtool-0.4.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
   [[tool.pysen.lint.mypy_targets]]
     paths = ["."]
 
 
 [tool.poetry]
 name = "aoirint-matvtool"
-version = "0.3.0-beta.4"
+version = "0.4.0-beta.1"
 description = "A command line tool to handle a multi audio track video file"
 authors = ["aoirint <aoirint@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aoirint/matvtoolpy"
 packages = [{include = "aoirint_matvtool"}]
```

### Comparing `aoirint_matvtool-0.3.0b4/PKG-INFO` & `aoirint_matvtool-0.4.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aoirint-matvtool
-Version: 0.3.0b4
+Version: 0.4.0b1
 Summary: A command line tool to handle a multi audio track video file
 Home-page: https://github.com/aoirint/matvtoolpy
 License: MIT
 Author: aoirint
 Author-email: aoirint@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

