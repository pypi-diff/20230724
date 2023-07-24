# Comparing `tmp/aoirint_matvtool-0.3.0b1.tar.gz` & `tmp/aoirint_matvtool-0.3.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aoirint_matvtool-0.3.0b1.tar", last modified: Mon Jul 24 01:58:31 2023, max compression
+gzip compressed data, was "aoirint_matvtool-0.3.0b4.tar", max compression
```

## Comparing `aoirint_matvtool-0.3.0b1.tar` & `aoirint_matvtool-0.3.0b4.tar`

### file list

```diff
@@ -1,27 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:31.372105 aoirint_matvtool-0.3.0b1/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7341 2023-07-24 01:58:31.372105 aoirint_matvtool-0.3.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:31.368105 aoirint_matvtool-0.3.0b1/aoirint_matvtool/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-24 01:58:30.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2611 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/crop_scale.py
--rw-r--r--   0 runner    (1001) docker     (122)     4269 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/find_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/fps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5233 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/inputs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/key_frames.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:31.368105 aoirint_matvtool-0.3.0b1/aoirint_matvtool/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12548 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/select_audio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/slice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3515 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 01:58:31.368105 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7341 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-24 01:58:31.000000 aoirint_matvtool-0.3.0b1/aoirint_matvtool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-24 01:58:31.372105 aoirint_matvtool-0.3.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-07-24 01:58:15.000000 aoirint_matvtool-0.3.0b1/setup.py
+-rw-r--r--   0        0        0     1064 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/LICENSE
+-rw-r--r--   0        0        0     7079 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/README.md
+-rw-r--r--   0        0        0       29 2023-07-24 02:21:09.217930 aoirint_matvtool-0.3.0b4/aoirint_matvtool/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/config.py
+-rw-r--r--   0        0        0     3004 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/crop_scale.py
+-rw-r--r--   0        0        0     5008 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/find_image.py
+-rw-r--r--   0        0        0     1345 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/fps.py
+-rw-r--r--   0        0        0     6029 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/inputs.py
+-rw-r--r--   0        0        0     1278 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/key_frames.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/scripts/__init__.py
+-rw-r--r--   0        0        0    15229 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/scripts/cli.py
+-rw-r--r--   0        0        0     2305 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/select_audio.py
+-rw-r--r--   0        0        0     2140 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/slice.py
+-rw-r--r--   0        0        0     3914 2023-07-24 02:20:52.032734 aoirint_matvtool-0.3.0b4/aoirint_matvtool/util.py
+-rw-r--r--   0        0        0     1069 2023-07-24 02:21:09.221931 aoirint_matvtool-0.3.0b4/pyproject.toml
+-rw-r--r--   0        0        0     7685 1970-01-01 00:00:00.000000 aoirint_matvtool-0.3.0b4/PKG-INFO
```

### Comparing `aoirint_matvtool-0.3.0b1/LICENSE` & `aoirint_matvtool-0.3.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `aoirint_matvtool-0.3.0b1/PKG-INFO` & `aoirint_matvtool-0.3.0b4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
-Name: aoirint_matvtool
-Version: 0.3.0b1
+Name: aoirint-matvtool
+Version: 0.3.0b4
 Summary: A command line tool to handle a multi audio track video file
 Home-page: https://github.com/aoirint/matvtoolpy
+License: MIT
 Author: aoirint
 Author-email: aoirint@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Repository, https://github.com/aoirint/matvtoolpy
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # matvtoolpy / MultiAudioTrackVideoToolPy
 
 A command line tool to handle a multi audio track video file.
 
 マルチオーディオトラック動画ファイルを取り扱うためのコマンドラインツール
 
@@ -27,14 +25,15 @@
 
 基本的にFFmpegのラッパーです。別途FFmpegのインストールが必要です。
 FFmpeg 4.2（Ubuntu 20.04の標準バージョン）および4.4（Ubuntu 22.04の標準バージョン）をサポートしています。
 
 - <https://ffmpeg.org/download.html>
 
 `matvtool`本体は、以下からダウンロード・インストールできます。
+Pythonパッケージとして導入する場合、Python 3.11をサポートしています。
 
 - バイナリ（Windows, Linux, macOS）
   - GitHub Release: <https://github.com/aoirint/matvtoolpy/releases>
 - Pythonパッケージ: `pip3 install aoirint_matvtool`
   - PyPI: <https://pypi.org/project/aoirint-matvtool/>
 - Dockerイメージ
   - Docker Hub: <https://hub.docker.com/r/aoirint/matvtoolpy>
@@ -125,15 +124,23 @@
 ```shell
 matvtool select_audio -i input.mkv --audio_index 2 3 -- output.mkv
 ```
 
 
 ## 開発
 
-### 依存関係の追加・更新
+Python 3.11を使って開発しています。
+
+### 依存関係
+
+依存関係の管理に[Poetry](https://python-poetry.org/docs/#installation)を使っています。
 
 ```shell
-pip-compile requirements.in
-pip-compile requirements-test.in
-```
+# Pythonパッケージを追加
+poetry add pydantic
+poetry add --group dev pytest
 
+# requirements*.txtを更新
+poetry export --without-hashes -o requirements.txt
+poetry export --without-hashes --with dev -o requirements-dev.txt
+```
```

### Comparing `aoirint_matvtool-0.3.0b1/README.md` & `aoirint_matvtool-0.3.0b4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 基本的にFFmpegのラッパーです。別途FFmpegのインストールが必要です。
 FFmpeg 4.2（Ubuntu 20.04の標準バージョン）および4.4（Ubuntu 22.04の標準バージョン）をサポートしています。
 
 - <https://ffmpeg.org/download.html>
 
 `matvtool`本体は、以下からダウンロード・インストールできます。
+Pythonパッケージとして導入する場合、Python 3.11をサポートしています。
 
 - バイナリ（Windows, Linux, macOS）
   - GitHub Release: <https://github.com/aoirint/matvtoolpy/releases>
 - Pythonパッケージ: `pip3 install aoirint_matvtool`
   - PyPI: <https://pypi.org/project/aoirint-matvtool/>
 - Dockerイメージ
   - Docker Hub: <https://hub.docker.com/r/aoirint/matvtoolpy>
@@ -106,13 +107,22 @@
 ```shell
 matvtool select_audio -i input.mkv --audio_index 2 3 -- output.mkv
 ```
 
 
 ## 開発
 
-### 依存関係の追加・更新
+Python 3.11を使って開発しています。
+
+### 依存関係
+
+依存関係の管理に[Poetry](https://python-poetry.org/docs/#installation)を使っています。
 
 ```shell
-pip-compile requirements.in
-pip-compile requirements-test.in
+# Pythonパッケージを追加
+poetry add pydantic
+poetry add --group dev pytest
+
+# requirements*.txtを更新
+poetry export --without-hashes -o requirements.txt
+poetry export --without-hashes --with dev -o requirements-dev.txt
 ```
```

### Comparing `aoirint_matvtool-0.3.0b1/aoirint_matvtool/crop_scale.py` & `aoirint_matvtool-0.3.0b4/aoirint_matvtool/select_audio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,91 @@
-from pathlib import Path
 import re
 import subprocess
-from typing import Iterable, Optional, Union
+from pathlib import Path
+from typing import Iterable, List, Optional, Union
+
 from pydantic import BaseModel
 
 from . import config
-from .util import exclude_none
 from .find_image import FfmpegProgressLine
 
 
-class FfmpegCropScaleResult(BaseModel):
-  success: bool
-  message: Optional[str]
-
-
-def ffmpeg_crop_scale(
-  input_path: Path,
-  crop: Optional[str],
-  scale: Optional[str],
-  video_codec: Optional[str],
-  output_path: Path,
-) -> Iterable[Union[FfmpegCropScaleResult, FfmpegProgressLine]]:
-  # TODO: quality control
-  if crop is not None and ',' in crop:
-    raise ValueError('Invalid crop argument. Remove \',\' from crop.')
-
-  if scale is not None and ',' in scale:
-    raise ValueError('Invalid scale argument. Remove \',\' from scale.')
-
-  crop_filter_string = f'crop={crop}' if crop is not None else None
-  scale_filter_string = f'scale={scale}' if scale is not None else None
-
-  video_filters = list(exclude_none([
-    crop_filter_string,
-    scale_filter_string,
-  ]))
-  video_filter_opts = [ '-filter:v', ','.join(video_filters) ] if len(video_filters) != 0 else []
-
-  video_codec_opts =  [ '-c:v', video_codec ] if video_codec is not None else []
-
-  command = [
-    config.FFMPEG_PATH,
-    '-hide_banner',
-    '-n', # fail if already exists
-    '-i',
-    str(input_path),
-    *video_filter_opts,
-    *video_codec_opts,
-    '-c:a',
-    'copy',
-    '-map',
-    '0',
-    '-map_metadata',
-    '0',
-    str(output_path),
-  ]
-  proc = subprocess.Popen(
-    command,
-    stdout=subprocess.DEVNULL,
-    stderr=subprocess.PIPE,
-    encoding='utf-8',
-  )
-  
-  lines = []
-  try:
-    while proc.poll() is None:
-      assert proc.stderr is not None
-      line = proc.stderr.readline().rstrip()
-      lines += [ line ]
-
-      match = re.match(r'^frame=\ *(\d+?)\ .+time=(.+?)\ bitrate.+$', line)
-      if match:
-        frame = int(match.group(1))
-        _time = match.group(2).strip()
-
-        progress = FfmpegProgressLine(
-          frame=frame,
-          time=_time,
-        )
-        yield progress
-
-    returncode = proc.wait()
-  finally:
-    proc.kill()
-
-  if returncode != 0:
-    # skip Input or indented block to head the error message
-    line_index = 0
-    while line_index < len(lines):
-      line = lines[line_index]
-      match = re.search(r'^(Input|  ).+$', line)
-      if not match:
-        break
-      line_index += 1
-
-    message = '\n'.join(lines[line_index:]) if line_index != len(lines) else None
-
-    yield FfmpegCropScaleResult(
-      success=False,
-      message=message,
-    )
-  else:
-    yield FfmpegCropScaleResult(
-      success=True,
-      message=None,
+class FfmpegSelectAudioResult(BaseModel):
+    success: bool
+    message: Optional[str]
+
+
+def ffmpeg_select_audio(
+    input_path: Path,
+    audio_indexes: List[int],
+    output_path: Path,
+) -> Iterable[Union[FfmpegSelectAudioResult, FfmpegProgressLine]]:
+    audio_map_options = []
+    for audio_index in audio_indexes:
+        audio_map_options.append("-map")
+        audio_map_options.append(f"0:a:{audio_index}")
+
+    command = [
+        config.FFMPEG_PATH,
+        "-hide_banner",
+        "-n",  # fail if already exists
+        "-i",
+        str(input_path),
+        "-map",
+        "0:v:0",
+        *audio_map_options,
+        "-map_metadata",
+        "0",
+        "-c",
+        "copy",
+        str(output_path),
+    ]
+    proc = subprocess.Popen(
+        command,
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.PIPE,
+        encoding="utf-8",
     )
+
+    lines = []
+    try:
+        while proc.poll() is None:
+            assert proc.stderr is not None
+            line = proc.stderr.readline().rstrip()
+            lines += [line]
+
+            match = re.match(r"^frame=\ *(\d+?)\ .+time=(.+?)\ bitrate.+$", line)
+            if match:
+                frame = int(match.group(1))
+                _time = match.group(2).strip()
+
+                progress = FfmpegProgressLine(
+                    frame=frame,
+                    time=_time,
+                )
+                yield progress
+
+        returncode = proc.wait()
+    finally:
+        proc.kill()
+
+    if returncode != 0:
+        # skip Input or indented block to head the error message
+        line_index = 0
+        while line_index < len(lines):
+            line = lines[line_index]
+            match = re.search(r"^(Input|  ).+$", line)
+            if not match:
+                break
+            line_index += 1
+
+        message = "\n".join(lines[line_index:]) if line_index != len(lines) else None
+
+        yield FfmpegSelectAudioResult(
+            success=False,
+            message=message,
+        )
+    else:
+        yield FfmpegSelectAudioResult(
+            success=True,
+            message=None,
+        )
```

### Comparing `aoirint_matvtool-0.3.0b1/aoirint_matvtool/fps.py` & `aoirint_matvtool-0.3.0b4/aoirint_matvtool/fps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,45 @@
-from pathlib import Path
 import re
+from pathlib import Path
 from typing import Optional
+
 from pydantic import BaseModel
 
 from .inputs import ffmpeg_get_input
 from .util import integer_part_and_decimal_part_to_float
 
+
 class FfmpegFpsResult(BaseModel):
-  success: bool
-  fps: Optional[float]
+    success: bool
+    fps: Optional[float]
 
-def ffmpeg_fps(input_path: Path) -> FfmpegFpsResult:
-  input_video = ffmpeg_get_input(input_path=input_path)
 
-  input_video_track = next(filter(lambda track: track.type == 'Video', input_video.streams[0].tracks))
-  # h264 (High), yuv420p(tv, bt709, progressive), 1920x1080 [SAR 1:1 DAR 16:9], 60 fps, 60 tbr, 1k tbn, 120 tbc (default)
-  input_video_track_text = input_video_track.text
-  match = re.search(r'(\d+)(\.\d+)?\ fps', input_video_track_text)
-
-  if match:
-    input_video_fps_integer_part = int(match.group(1))
-    input_video_fps_decimal_part = int(match.group(2)[1:]) if match.group(2) is not None else 0 # maybe None
+def ffmpeg_fps(input_path: Path) -> FfmpegFpsResult:
+    input_video = ffmpeg_get_input(input_path=input_path)
 
-    input_video_fps = integer_part_and_decimal_part_to_float(integer_part=input_video_fps_integer_part, decimal_part=input_video_fps_decimal_part)
+    input_video_track = next(
+        filter(lambda track: track.type == "Video", input_video.streams[0].tracks)
+    )
+    # h264 (High), yuv420p(tv, bt709, progressive), 1920x1080 [SAR 1:1 DAR 16:9], 60 fps, 60 tbr, 1k tbn, 120 tbc (default)  # noqa: B950
+    input_video_track_text = input_video_track.text
+    match = re.search(r"(\d+)(\.\d+)?\ fps", input_video_track_text)
+
+    if match:
+        input_video_fps_integer_part = int(match.group(1))
+        input_video_fps_decimal_part = (
+            int(match.group(2)[1:]) if match.group(2) is not None else 0
+        )  # maybe None
+
+        input_video_fps = integer_part_and_decimal_part_to_float(
+            integer_part=input_video_fps_integer_part,
+            decimal_part=input_video_fps_decimal_part,
+        )
+
+        return FfmpegFpsResult(
+            success=True,
+            fps=float(input_video_fps),
+        )
 
     return FfmpegFpsResult(
-      success=True,
-      fps=float(input_video_fps),
+        success=False,
+        fps=None,
     )
-
-  return FfmpegFpsResult(
-    success=False,
-    fps=None,
-  )
```

### Comparing `aoirint_matvtool-0.3.0b1/aoirint_matvtool/inputs.py` & `aoirint_matvtool-0.3.0b4/aoirint_matvtool/inputs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,174 +1,202 @@
-
-from pathlib import Path
 import re
 import subprocess
+from pathlib import Path
 from typing import List
+
 from pydantic import BaseModel
 
 from . import config
 from .config import logger
 
 
 class FfmpegMetadataItem(BaseModel):
-  key: str
-  value: str
+    key: str
+    value: str
+
 
 class FfmpegTrack(BaseModel):
-  index: int
-  type: str
-  text: str
-  metadatas: List[FfmpegMetadataItem]
+    index: int
+    type: str
+    text: str
+    metadatas: List[FfmpegMetadataItem]
+
 
 class FfmpegStream(BaseModel):
-  index: int
-  tracks: List[FfmpegTrack]
+    index: int
+    tracks: List[FfmpegTrack]
+
 
 class FfmpegInput(BaseModel):
-  index: str
-  text: str
-  streams: List[FfmpegStream]
-  metadatas: List[FfmpegMetadataItem]
+    index: int
+    text: str
+    streams: List[FfmpegStream]
+    metadatas: List[FfmpegMetadataItem]
 
 
 def __find_all_input_line_index(lines: List[str]) -> List[int]:
-  indexes: List[int] = []
+    indexes: List[int] = []
 
-  for line_index, line in enumerate(lines):
-    match = re.search(r'^Input #.+$', line)
-    if match:
-      indexes.append(line_index)
+    for line_index, line in enumerate(lines):
+        match = re.search(r"^Input #.+$", line)
+        if match:
+            indexes.append(line_index)
+
+    return indexes
 
-  return indexes
 
 def __find_all_stream_line_index(lines: List[str]) -> List[int]:
-  indexes: List[int] = []
+    indexes: List[int] = []
+
+    for line_index, line in enumerate(lines):
+        # FFmpeg 4.2: indent level 4
+        # FFmpeg 4.4: indent level 2
+        match = re.search(r"^(?:\s{2}|\s{4})Stream #.+$", line)
+        if match:
+            indexes.append(line_index)
 
-  for line_index, line in enumerate(lines):
-    # FFmpeg 4.2: indent level 4
-    # FFmpeg 4.4: indent level 2
-    match = re.search(r'^(?:\s{2}|\s{4})Stream #.+$', line)
-    if match:
-      indexes.append(line_index)
+    return indexes
 
-  return indexes
 
 def __find_all_metadata_line_index(lines: List[str], level: int) -> List[int]:
-  indent = ' ' * level
+    indent = " " * level
 
-  indexes: List[int] = []
+    indexes: List[int] = []
 
-  for line_index, line in enumerate(lines):
-    match = re.search(r'^' + indent + r'Metadata:', line)
-    if match:
-      indexes.append(line_index)
+    for line_index, line in enumerate(lines):
+        match = re.search(r"^" + indent + r"Metadata:", line)
+        if match:
+            indexes.append(line_index)
 
-  return indexes
+    return indexes
 
-def __read_first_metadata_items(lines: List[str], level: int) -> List[FfmpegMetadataItem]:
-  metadata_line_indexes = __find_all_metadata_line_index(lines=lines, level=level)
-  assert len(metadata_line_indexes) != 0
 
-  indent = ' ' * (level+2)
+def __read_first_metadata_items(
+    lines: List[str], level: int
+) -> List[FfmpegMetadataItem]:
+    metadata_line_indexes = __find_all_metadata_line_index(lines=lines, level=level)
+    assert len(metadata_line_indexes) != 0
 
-  metadatas: List[FfmpegMetadataItem] = []
+    indent = " " * (level + 2)
 
-  metadata_line_index = metadata_line_indexes[0]
-  metadata_line_index_end = len(lines)
-  metadata_lines = lines[metadata_line_index:metadata_line_index_end]
-  for metadata_line in metadata_lines:
-    match_metadata_item = re.search(r'^' + indent + r'(.+?):(.+)$', metadata_line)
-    if not match_metadata_item:
-      continue
+    metadatas: List[FfmpegMetadataItem] = []
 
-    metadata_key = match_metadata_item.group(1).strip()
-    metadata_value = match_metadata_item.group(2).strip()
-    metadatas.append(FfmpegMetadataItem(key=metadata_key, value=metadata_value))
+    metadata_line_index = metadata_line_indexes[0]
+    metadata_line_index_end = len(lines)
+    metadata_lines = lines[metadata_line_index:metadata_line_index_end]
+    for metadata_line in metadata_lines:
+        match_metadata_item = re.search(r"^" + indent + r"(.+?):(.+)$", metadata_line)
+        if not match_metadata_item:
+            continue
 
-  return metadatas
+        metadata_key = match_metadata_item.group(1).strip()
+        metadata_value = match_metadata_item.group(2).strip()
+        metadatas.append(FfmpegMetadataItem(key=metadata_key, value=metadata_value))
+
+    return metadatas
 
 
 # API
 def ffmpeg_get_input(input_path: Path) -> FfmpegInput:
-  command = [
-    config.FFMPEG_PATH,
-    '-hide_banner',
-    '-i',
-    str(input_path),
-  ]
-  proc = subprocess.run(command, stderr=subprocess.PIPE)
-  stderr = proc.stderr.decode('utf-8')
-
-  lines = stderr.splitlines()
-
-  inputs: List[FfmpegInput] = []
-
-  input_line_indexes = __find_all_input_line_index(lines=lines)
-  for input_index, input_line_index in enumerate(input_line_indexes):
-    input_line_index_end = input_line_indexes[input_index + 1] if input_index + 1 != len(input_line_indexes) else len(lines)
-
-    input_line_header = lines[input_line_index]
-    match_input = re.search(r'^Input #(\d+?), (.+)$', input_line_header)
-    if not match_input:
-      continue
-
-    input_header_index = int(match_input.group(1))
-    input_header_text = match_input.group(2)
-    logger.debug(f'Input {input_header_index} {input_header_text}')
-
-    input_lines = lines[input_line_index+1:input_line_index_end]
-    stream_line_indexes = __find_all_stream_line_index(lines=input_lines)
-
-    input_metadata_lines = input_lines[0:stream_line_indexes[0]]
-    input_metadatas = __read_first_metadata_items(lines=input_metadata_lines, level=2)
-    logger.debug(f'Input Metadatas {input_metadatas}')
-
-    streams: List[FfmpegStream] = []
-
-    for stream_index, stream_line_index in enumerate(stream_line_indexes):
-      stream_line_index_end = stream_line_indexes[stream_index + 1] if stream_index + 1 != len(stream_line_indexes) else len(input_lines)
-
-      stream_line_header = input_lines[stream_line_index]
-
-    # FFmpeg 4.2: indent level 4
-    # FFmpeg 4.4: indent level 2
-      match_stream = re.search(r'^(?:\s{2}|\s{4})Stream #(\d+?):(\d+?).*?: (Video|Audio): (.+)$', stream_line_header)
-      if not match_stream:
-        continue
-
-      stream_header_index = int(match_stream.group(1))
-      stream_track_index = int(match_stream.group(2))
-      stream_type = match_stream.group(3)
-      stream_text = match_stream.group(4)
-      logger.debug(f'Stream Track {stream_index} {stream_track_index} {stream_type} {stream_text}')
-
-      stream_lines = input_lines[stream_line_index+1:stream_line_index_end]
-      track_metadatas = __read_first_metadata_items(lines=stream_lines, level=4)
-      logger.debug(f'Stream Track Metadatas {track_metadatas}')
-
-      stream = next(filter(lambda stream: stream.index == stream_header_index, streams), None)
-      track = FfmpegTrack(
-        index=stream_track_index,
-        type=stream_type,
-        text=stream_text,
-        metadatas=track_metadatas,
-      )
-      if stream is None:
-        stream = FfmpegStream(
-          index=stream_header_index,
-          tracks=[],
+    command = [
+        config.FFMPEG_PATH,
+        "-hide_banner",
+        "-i",
+        str(input_path),
+    ]
+    proc = subprocess.run(command, stderr=subprocess.PIPE)
+    stderr = proc.stderr.decode("utf-8")
+
+    lines = stderr.splitlines()
+
+    inputs: List[FfmpegInput] = []
+
+    input_line_indexes = __find_all_input_line_index(lines=lines)
+    for input_index, input_line_index in enumerate(input_line_indexes):
+        input_line_index_end = (
+            input_line_indexes[input_index + 1]
+            if input_index + 1 != len(input_line_indexes)
+            else len(lines)
         )
-        streams.append(stream)
 
-      stream.tracks.append(track)
-  
-    inputs.append(FfmpegInput(
-      index=input_header_index,
-      text=input_header_text,
-      streams=streams,
-      metadatas=input_metadatas,
-    ))
+        input_line_header = lines[input_line_index]
+        match_input = re.search(r"^Input #(\d+?), (.+)$", input_line_header)
+        if not match_input:
+            continue
+
+        input_header_index = int(match_input.group(1))
+        input_header_text = match_input.group(2)
+        logger.debug(f"Input {input_header_index} {input_header_text}")
+
+        input_lines = lines[input_line_index + 1 : input_line_index_end]
+        stream_line_indexes = __find_all_stream_line_index(lines=input_lines)
+
+        input_metadata_lines = input_lines[0 : stream_line_indexes[0]]
+        input_metadatas = __read_first_metadata_items(
+            lines=input_metadata_lines, level=2
+        )
+        logger.debug(f"Input Metadatas {input_metadatas}")
+
+        streams: List[FfmpegStream] = []
+
+        for stream_index, stream_line_index in enumerate(stream_line_indexes):
+            stream_line_index_end = (
+                stream_line_indexes[stream_index + 1]
+                if stream_index + 1 != len(stream_line_indexes)
+                else len(input_lines)
+            )
+
+            stream_line_header = input_lines[stream_line_index]
+
+            # FFmpeg 4.2: indent level 4
+            # FFmpeg 4.4: indent level 2
+            match_stream = re.search(
+                r"^(?:\s{2}|\s{4})Stream #(\d+?):(\d+?).*?: (Video|Audio): (.+)$",
+                stream_line_header,
+            )
+            if not match_stream:
+                continue
+
+            stream_header_index = int(match_stream.group(1))
+            stream_track_index = int(match_stream.group(2))
+            stream_type = match_stream.group(3)
+            stream_text = match_stream.group(4)
+            logger.debug(
+                f"Stream Track {stream_index} {stream_track_index} {stream_type} {stream_text}"
+            )
+
+            stream_lines = input_lines[stream_line_index + 1 : stream_line_index_end]
+            track_metadatas = __read_first_metadata_items(lines=stream_lines, level=4)
+            logger.debug(f"Stream Track Metadatas {track_metadatas}")
+
+            stream = next(
+                filter(lambda stream: stream.index == stream_header_index, streams),
+                None,
+            )
+            track = FfmpegTrack(
+                index=stream_track_index,
+                type=stream_type,
+                text=stream_text,
+                metadatas=track_metadatas,
+            )
+            if stream is None:
+                stream = FfmpegStream(
+                    index=stream_header_index,
+                    tracks=[],
+                )
+                streams.append(stream)
+
+            stream.tracks.append(track)
+
+        inputs.append(
+            FfmpegInput(
+                index=input_header_index,
+                text=input_header_text,
+                streams=streams,
+                metadatas=input_metadatas,
+            )
+        )
 
-  if len(inputs) == 0:
-    raise Exception(f'File not found: {input_path}')
+    if len(inputs) == 0:
+        raise Exception(f"File not found: {input_path}")
 
-  return inputs[0]
+    return inputs[0]
```

### Comparing `aoirint_matvtool-0.3.0b1/aoirint_matvtool/key_frames.py` & `aoirint_matvtool-0.3.0b4/aoirint_matvtool/key_frames.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-from pathlib import Path
 import re
 import subprocess
+from pathlib import Path
 from typing import Generator
+
 from pydantic import BaseModel
 
 from . import config
 
+
 class FfmpegKeyFrameOutputLine(BaseModel):
-  time: float
+    time: float
+
 
 def ffmpeg_key_frames(
-  input_path: Path,
+    input_path: Path,
 ) -> Generator[FfmpegKeyFrameOutputLine, None, None]:
-  command = [
-    config.FFPROBE_PATH,
-    '-hide_banner',
-    '-skip_frame',
-    'nokey',
-    '-select_streams',
-    'v',
-    '-show_frames',
-    '-show_entries',
-    'frame=pkt_pts_time',
-    '-of',
-    'csv',
-    str(input_path),
-  ]
-
-  proc = subprocess.Popen(
-    command,
-    stdout=subprocess.PIPE,
-    stderr=subprocess.DEVNULL,
-    encoding='utf-8',
-  )
-
-  try:
-    while proc.poll() is None:
-      assert proc.stdout is not None
-      line = proc.stdout.readline().rstrip()
-
-      match = re.match(r'^frame,(.+)$', line)
-      if match: # frame,1.983000
-        seconds = float(match.group(1).strip())
-        output = FfmpegKeyFrameOutputLine(time=seconds)
-        yield output
-
-    result_code = proc.wait()
-    if result_code != 0:
-      raise Exception(f'FFmpeg errored. code {result_code}')
-  finally:
-    proc.kill()
+    command = [
+        config.FFPROBE_PATH,
+        "-hide_banner",
+        "-skip_frame",
+        "nokey",
+        "-select_streams",
+        "v",
+        "-show_frames",
+        "-show_entries",
+        "frame=pkt_pts_time",
+        "-of",
+        "csv",
+        str(input_path),
+    ]
+
+    proc = subprocess.Popen(
+        command,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.DEVNULL,
+        encoding="utf-8",
+    )
+
+    try:
+        while proc.poll() is None:
+            assert proc.stdout is not None
+            line = proc.stdout.readline().rstrip()
+
+            match = re.match(r"^frame,(.+)$", line)
+            if match:  # frame,1.983000
+                seconds = float(match.group(1).strip())
+                output = FfmpegKeyFrameOutputLine(time=seconds)
+                yield output
+
+        result_code = proc.wait()
+        if result_code != 0:
+            raise Exception(f"FFmpeg errored. code {result_code}")
+    finally:
+        proc.kill()
```

### Comparing `aoirint_matvtool-0.3.0b1/aoirint_matvtool/util.py` & `aoirint_matvtool-0.3.0b4/aoirint_matvtool/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,133 @@
+import re
 from datetime import timedelta
 from math import log10
 from pathlib import Path
-import re
 from typing import Iterable, Optional, TypeVar
+
 from pydantic import BaseModel
 
 from .key_frames import FfmpegKeyFrameOutputLine, ffmpeg_key_frames
 
+T = TypeVar("T")
+
 
-T = TypeVar('T')
 def exclude_none(iterable: Iterable[Optional[T]]) -> Iterable[T]:
-  """
+    """
     Type-safe exclusion function for None
-  """
-  for item in iterable:
-    if item is None:
-      continue
+    """
+    for item in iterable:
+        if item is None:
+            continue
 
-    yield item
+        yield item
 
 
 class FfmpegTimeUnitSyntax(BaseModel):
-  hours: int
-  minutes: int
-  seconds: int
-  microseconds: int
-
-  def to_timedelta(self) -> timedelta:
-    return timedelta(hours=self.hours, minutes=self.minutes, seconds=self.seconds, microseconds=self.microseconds)
-
+    hours: int
+    minutes: int
+    seconds: int
+    microseconds: int
+
+    def to_timedelta(self) -> timedelta:
+        return timedelta(
+            hours=self.hours,
+            minutes=self.minutes,
+            seconds=self.seconds,
+            microseconds=self.microseconds,
+        )
+
+
+def integer_part_and_decimal_part_to_float(
+    integer_part: int, decimal_part: int
+) -> float:
+    ret = 0.0
+    ret += integer_part
 
-def integer_part_and_decimal_part_to_float(integer_part: int, decimal_part: int) -> float:
-  ret = 0.0
-  ret += integer_part
+    decimal_part_num_digits = log10(decimal_part) if decimal_part != 0 else 0  # 桁数
+    decimal_part_scale = 10 ** (-decimal_part_num_digits)  # 桁補正係数
 
-  decimal_part_num_digits = log10(decimal_part) if decimal_part != 0 else 0 # 桁数
-  decimal_part_scale = 10 ** (-decimal_part_num_digits) # 桁補正係数
+    ret += decimal_part * decimal_part_scale
 
-  ret += decimal_part * decimal_part_scale
-
-  return ret
+    return ret
 
 
 def parse_ffmpeg_time_unit_syntax(string: str) -> FfmpegTimeUnitSyntax:
-  match = re.match(r'^(\d+):(\d+):(\d+)(\.\d+)?$', string) # HOURS:MM:SS.MILLISECONDS
-  if match:
-    hours = int(match.group(1))
-    minutes = int(match.group(2))
-    seconds = int(match.group(3))
-    microseconds = int(match.group(4)[1:]) if match.group(4) is not None else 0 # maybe None
-
-    return FfmpegTimeUnitSyntax(
-      hours=hours,
-      minutes=minutes,
-      seconds=seconds,
-      microseconds=microseconds,
-    )
+    match = re.match(r"^(\d+):(\d+):(\d+)(\.\d+)?$", string)  # HOURS:MM:SS.MILLISECONDS
+    if match:
+        hours = int(match.group(1))
+        minutes = int(match.group(2))
+        seconds = int(match.group(3))
+        microseconds = (
+            int(match.group(4)[1:]) if match.group(4) is not None else 0
+        )  # maybe None
+
+        return FfmpegTimeUnitSyntax(
+            hours=hours,
+            minutes=minutes,
+            seconds=seconds,
+            microseconds=microseconds,
+        )
+
+    match = re.match(r"^(\d+)(\.\d+)?$", string)  # SECONDS
+    if match:
+        time_seconds_integer_part = int(match.group(1))
+        time_seconds_decimal_part = int(match.group(2)) if match.group(2) is None else 0
+
+        time_seconds = integer_part_and_decimal_part_to_float(
+            integer_part=time_seconds_integer_part,
+            decimal_part=time_seconds_decimal_part,
+        )
+
+        td = timedelta(seconds=time_seconds)
+        hours, remainder = divmod(td.seconds, 3600)
+        minutes, seconds = divmod(remainder, 60)
+        microseconds = td.microseconds
+
+        return FfmpegTimeUnitSyntax(
+            hours=hours,
+            minutes=minutes,
+            seconds=seconds,
+            microseconds=microseconds,
+        )
 
-  match = re.match(r'^(\d+)(\.\d+)?$', string) # SECONDS
-  if match:
-    time_seconds_integer_part = int(match.group(1))
-    time_seconds_decimal_part = int(match.group(2)) if match.group(2) is None else 0
-
-    time_seconds = integer_part_and_decimal_part_to_float(integer_part=time_seconds_integer_part, decimal_part=time_seconds_decimal_part)
-
-    td = timedelta(seconds=time_seconds)
-    hours, remainder = divmod(td.seconds, 3600)
-    minutes, seconds = divmod(remainder, 60)
-    microseconds = td.microseconds
-
-    return FfmpegTimeUnitSyntax(
-      hours=hours,
-      minutes=minutes,
-      seconds=seconds,
-      microseconds=microseconds,
-    )
-
-  raise ValueError(f'Unsupported syntax: {string}')
+    raise ValueError(f"Unsupported syntax: {string}")
 
 
 def get_real_start_timedelta_by_ss(
-  video_path: Path,
-  ss: Optional[str],
+    video_path: Path,
+    ss: Optional[str],
 ) -> timedelta:
-  """
+    """
     ssオプションから実時間での開始時間を計算
-  """
-  raw_start_time = parse_ffmpeg_time_unit_syntax(ss) if ss is not None else None
-  raw_start_timedelta = raw_start_time.to_timedelta() if raw_start_time is not None else timedelta(seconds=0)
-  # raw_end_time = parse_ffmpeg_time_unit_syntax(to) if to is not None else None
-
-  # キーフレーム情報をもとにstart_timedeltaを補正
-  start_timedelta = timedelta(seconds=0)
-  for output in ffmpeg_key_frames(
-    input_path=video_path,
-  ):
-    if isinstance(output, FfmpegKeyFrameOutputLine):
-      next_key_frame_timedelta = timedelta(seconds=output.time)
-
-      # raw_start_timedeltaより前のキーフレームを選択（-ssオプションの挙動）
-      if raw_start_timedelta <= next_key_frame_timedelta:
-        break
+    """
+    raw_start_time = parse_ffmpeg_time_unit_syntax(ss) if ss is not None else None
+    raw_start_timedelta = (
+        raw_start_time.to_timedelta()
+        if raw_start_time is not None
+        else timedelta(seconds=0)
+    )
+    # raw_end_time = parse_ffmpeg_time_unit_syntax(to) if to is not None else None
+
+    # キーフレーム情報をもとにstart_timedeltaを補正
+    start_timedelta = timedelta(seconds=0)
+    for output in ffmpeg_key_frames(
+        input_path=video_path,
+    ):
+        if isinstance(output, FfmpegKeyFrameOutputLine):
+            next_key_frame_timedelta = timedelta(seconds=output.time)
+
+            # raw_start_timedeltaより前のキーフレームを選択（-ssオプションの挙動）
+            if raw_start_timedelta <= next_key_frame_timedelta:
+                break
 
-      start_timedelta = next_key_frame_timedelta
+            start_timedelta = next_key_frame_timedelta
 
-  return start_timedelta
+    return start_timedelta
 
 
 def format_timedelta_as_time_unit_syntax_string(td: timedelta) -> str:
-  hours, remainder = divmod(td.seconds, 3600)
-  minutes, seconds = divmod(remainder, 60)
-  microseconds = td.microseconds
+    hours, remainder = divmod(td.seconds, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    microseconds = td.microseconds
 
-  return f'{hours:02d}:{minutes:02d}:{seconds:02d}.{microseconds:06d}'
+    return f"{hours:02d}:{minutes:02d}:{seconds:02d}.{microseconds:06d}"
```

