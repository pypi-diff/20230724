# Comparing `tmp/aoirint_matvtool-0.2.0.tar.gz` & `tmp/aoirint_matvtool-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aoirint_matvtool-0.2.0.tar", last modified: Sat Sep 10 03:51:12 2022, max compression
+gzip compressed data, was "aoirint_matvtool-0.3.0b1.tar", last modified: Mon Jul 24 01:58:31 2023, max compression
```

## Comparing `aoirint_matvtool-0.2.0.tar` & `aoirint_matvtool-0.3.0b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 03:51:12.498854 aoirint_matvtool-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7199 2022-09-10 03:51:12.498854 aoirint_matvtool-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6539 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 03:51:12.498854 aoirint_matvtool-0.2.0/aoirint_matvtool/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-10 03:51:12.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/crop_scale.py
--rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/find_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/fps.py
--rw-r--r--   0 runner    (1001) docker     (121)     5078 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/key_frames.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 03:51:12.498854 aoirint_matvtool-0.2.0/aoirint_matvtool/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12548 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/select_audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/slice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3515 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/aoirint_matvtool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 03:51:12.498854 aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7199 2022-09-10 03:51:12.000000 aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-09-10 03:51:12.000000 aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-10 03:51:12.000000 aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-10 03:51:12.000000 aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-10 03:51:12.000000 aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-10 03:51:12.000000 aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-10 03:51:12.498854 aoirint_matvtool-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-09-10 03:51:07.000000 aoirint_matvtool-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:31.372105 aoirint_matvtool-0.3.0b1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7341 2023-07-24 01:58:31.372105 aoirint_matvtool-0.3.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:31.368105 aoirint_matvtool-0.3.0b1/aoirint_matvtool/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-24 01:58:30.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2611 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/crop_scale.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4269 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/find_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/fps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5233 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/key_frames.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:31.368105 aoirint_matvtool-0.3.0b1/aoirint_matvtool/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12548 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/select_audio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/slice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3515 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:31.368105 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7341 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-24 01:58:31.372105 aoirint_matvtool-0.3.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/setup.py
```

### Comparing `aoirint_matvtool-0.2.0/LICENSE` & `aoirint_matvtool-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/PKG-INFO` & `aoirint_matvtool-0.3.0b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aoirint_matvtool
-Version: 0.2.0
+Version: 0.3.0b1
 Summary: A command line tool to handle a multi audio track video file
 Home-page: https://github.com/aoirint/matvtoolpy
 Author: aoirint
 Author-email: aoirint@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,15 @@
 A command line tool to handle a multi audio track video file.
 
 マルチオーディオトラック動画ファイルを取り扱うためのコマンドラインツール
 
 ## インストール
 
 基本的にFFmpegのラッパーです。別途FFmpegのインストールが必要です。
+FFmpeg 4.2（Ubuntu 20.04の標準バージョン）および4.4（Ubuntu 22.04の標準バージョン）をサポートしています。
 
 - <https://ffmpeg.org/download.html>
 
 `matvtool`本体は、以下からダウンロード・インストールできます。
 
 - バイナリ（Windows, Linux, macOS）
   - GitHub Release: <https://github.com/aoirint/matvtoolpy/releases>
```

### Comparing `aoirint_matvtool-0.2.0/README.md` & `aoirint_matvtool-0.3.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 A command line tool to handle a multi audio track video file.
 
 マルチオーディオトラック動画ファイルを取り扱うためのコマンドラインツール
 
 ## インストール
 
 基本的にFFmpegのラッパーです。別途FFmpegのインストールが必要です。
+FFmpeg 4.2（Ubuntu 20.04の標準バージョン）および4.4（Ubuntu 22.04の標準バージョン）をサポートしています。
 
 - <https://ffmpeg.org/download.html>
 
 `matvtool`本体は、以下からダウンロード・インストールできます。
 
 - バイナリ（Windows, Linux, macOS）
   - GitHub Release: <https://github.com/aoirint/matvtoolpy/releases>
```

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/crop_scale.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/crop_scale.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/find_image.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/find_image.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/fps.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/fps.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/inputs.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/inputs.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 
   return indexes
 
 def __find_all_stream_line_index(lines: List[str]) -> List[int]:
   indexes: List[int] = []
 
   for line_index, line in enumerate(lines):
-    match = re.search(r'^    Stream #.+$', line)
+    # FFmpeg 4.2: indent level 4
+    # FFmpeg 4.4: indent level 2
+    match = re.search(r'^(?:\s{2}|\s{4})Stream #.+$', line)
     if match:
       indexes.append(line_index)
 
   return indexes
 
 def __find_all_metadata_line_index(lines: List[str], level: int) -> List[int]:
   indent = ' ' * level
@@ -122,15 +124,18 @@
 
     streams: List[FfmpegStream] = []
 
     for stream_index, stream_line_index in enumerate(stream_line_indexes):
       stream_line_index_end = stream_line_indexes[stream_index + 1] if stream_index + 1 != len(stream_line_indexes) else len(input_lines)
 
       stream_line_header = input_lines[stream_line_index]
-      match_stream = re.search(r'^    Stream #(\d+?):(\d+?).*?: (Video|Audio): (.+)$', stream_line_header)
+
+    # FFmpeg 4.2: indent level 4
+    # FFmpeg 4.4: indent level 2
+      match_stream = re.search(r'^(?:\s{2}|\s{4})Stream #(\d+?):(\d+?).*?: (Video|Audio): (.+)$', stream_line_header)
       if not match_stream:
         continue
 
       stream_header_index = int(match_stream.group(1))
       stream_track_index = int(match_stream.group(2))
       stream_type = match_stream.group(3)
       stream_text = match_stream.group(4)
```

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/key_frames.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/key_frames.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/scripts/cli.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/select_audio.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/select_audio.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/slice.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/slice.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool/util.py` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool/util.py`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/PKG-INFO` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aoirint-matvtool
-Version: 0.2.0
+Version: 0.3.0b1
 Summary: A command line tool to handle a multi audio track video file
 Home-page: https://github.com/aoirint/matvtoolpy
 Author: aoirint
 Author-email: aoirint@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,15 @@
 A command line tool to handle a multi audio track video file.
 
 マルチオーディオトラック動画ファイルを取り扱うためのコマンドラインツール
 
 ## インストール
 
 基本的にFFmpegのラッパーです。別途FFmpegのインストールが必要です。
+FFmpeg 4.2（Ubuntu 20.04の標準バージョン）および4.4（Ubuntu 22.04の標準バージョン）をサポートしています。
 
 - <https://ffmpeg.org/download.html>
 
 `matvtool`本体は、以下からダウンロード・インストールできます。
 
 - バイナリ（Windows, Linux, macOS）
   - GitHub Release: <https://github.com/aoirint/matvtoolpy/releases>
```

### Comparing `aoirint_matvtool-0.2.0/aoirint_matvtool.egg-info/SOURCES.txt` & `aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.2.0/setup.py` & `aoirint_matvtool-0.3.0b1/setup.py`

 * *Files identical despite different names*

