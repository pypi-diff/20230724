# Comparing `tmp/aoirint_matvtool-0.4.0b2.tar.gz` & `tmp/aoirint_matvtool-0.4.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aoirint_matvtool-0.4.0b2.tar", max compression
+gzip compressed data, was "aoirint_matvtool-0.4.0b3.tar", max compression
```

## Comparing `aoirint_matvtool-0.4.0b2.tar` & `aoirint_matvtool-0.4.0b3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-07-24 07:58:03.226415 aoirint_matvtool-0.4.0b2/LICENSE
--rw-r--r--   0        0        0     7079 2023-07-24 07:58:03.226415 aoirint_matvtool-0.4.0b2/README.md
--rw-r--r--   0        0        0       29 2023-07-24 07:58:19.011569 aoirint_matvtool-0.4.0b2/aoirint_matvtool/__init__.py
--rw-r--r--   0        0        0      104 2023-07-24 07:58:03.226415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/config.py
--rw-r--r--   0        0        0     3004 2023-07-24 07:58:03.226415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/crop_scale.py
--rw-r--r--   0        0        0     5008 2023-07-24 07:58:03.226415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/find_image.py
--rw-r--r--   0        0        0     1345 2023-07-24 07:58:03.226415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/fps.py
--rw-r--r--   0        0        0     6029 2023-07-24 07:58:03.230415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/inputs.py
--rw-r--r--   0        0        0     1278 2023-07-24 07:58:03.230415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/key_frames.py
--rw-r--r--   0        0        0        0 2023-07-24 07:58:03.230415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/scripts/__init__.py
--rw-r--r--   0        0        0    15375 2023-07-24 07:58:03.230415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/scripts/cli.py
--rw-r--r--   0        0        0     2305 2023-07-24 07:58:03.230415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/select_audio.py
--rw-r--r--   0        0        0     2140 2023-07-24 07:58:03.230415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/slice.py
--rw-r--r--   0        0        0     3914 2023-07-24 07:58:03.230415 aoirint_matvtool-0.4.0b2/aoirint_matvtool/util.py
--rw-r--r--   0        0        0     1069 2023-07-24 07:58:19.015569 aoirint_matvtool-0.4.0b2/pyproject.toml
--rw-r--r--   0        0        0     7685 1970-01-01 00:00:00.000000 aoirint_matvtool-0.4.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/LICENSE
+-rw-r--r--   0        0        0     7079 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/README.md
+-rw-r--r--   0        0        0       29 2023-07-24 08:00:14.426840 aoirint_matvtool-0.4.0b3/aoirint_matvtool/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/config.py
+-rw-r--r--   0        0        0     3004 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/crop_scale.py
+-rw-r--r--   0        0        0     5008 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/find_image.py
+-rw-r--r--   0        0        0     1345 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/fps.py
+-rw-r--r--   0        0        0     6029 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/inputs.py
+-rw-r--r--   0        0        0     1278 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/key_frames.py
+-rw-r--r--   0        0        0        0 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/scripts/__init__.py
+-rw-r--r--   0        0        0    15375 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/scripts/cli.py
+-rw-r--r--   0        0        0     2305 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/select_audio.py
+-rw-r--r--   0        0        0     2140 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/slice.py
+-rw-r--r--   0        0        0     3914 2023-07-24 08:00:00.334730 aoirint_matvtool-0.4.0b3/aoirint_matvtool/util.py
+-rw-r--r--   0        0        0     1069 2023-07-24 08:00:14.426840 aoirint_matvtool-0.4.0b3/pyproject.toml
+-rw-r--r--   0        0        0     7685 1970-01-01 00:00:00.000000 aoirint_matvtool-0.4.0b3/PKG-INFO
```

### Comparing `aoirint_matvtool-0.4.0b2/LICENSE` & `aoirint_matvtool-0.4.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/README.md` & `aoirint_matvtool-0.4.0b3/README.md`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/crop_scale.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/crop_scale.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/find_image.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/find_image.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/fps.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/fps.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/inputs.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/inputs.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/key_frames.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/key_frames.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/scripts/cli.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/select_audio.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/select_audio.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/slice.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/slice.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/aoirint_matvtool/util.py` & `aoirint_matvtool-0.4.0b3/aoirint_matvtool/util.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.4.0b2/pyproject.toml` & `aoirint_matvtool-0.4.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
   [[tool.pysen.lint.mypy_targets]]
     paths = ["."]
 
 
 [tool.poetry]
 name = "aoirint-matvtool"
-version = "0.4.0-beta.2"
+version = "0.4.0-beta.3"
 description = "A command line tool to handle a multi audio track video file"
 authors = ["aoirint <aoirint@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aoirint/matvtoolpy"
 packages = [{include = "aoirint_matvtool"}]
```

### Comparing `aoirint_matvtool-0.4.0b2/PKG-INFO` & `aoirint_matvtool-0.4.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aoirint-matvtool
-Version: 0.4.0b2
+Version: 0.4.0b3
 Summary: A command line tool to handle a multi audio track video file
 Home-page: https://github.com/aoirint/matvtoolpy
 License: MIT
 Author: aoirint
 Author-email: aoirint@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

