# Comparing `tmp/rec_spotify-1.2.3.tar.gz` & `tmp/rec_spotify-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rec_spotify-1.2.3.tar", max compression
+gzip compressed data, was "rec_spotify-1.3.tar", max compression
```

## Comparing `rec_spotify-1.2.3.tar` & `rec_spotify-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.2.3/etc/screen.png
--rw-r--r--   0        0        0     1291 2023-07-24 08:45:23.861481 rec_spotify-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2289 2023-07-23 20:20:05.543332 rec_spotify-1.2.3/README.md
--rw-r--r--   0        0        0       23 2023-07-24 08:45:30.849755 rec_spotify-1.2.3/rec_spotify/__init__.py
--rw-r--r--   0        0        0     1735 2023-07-23 20:50:02.825572 rec_spotify-1.2.3/rec_spotify/cli.py
--rw-r--r--   0        0        0     4158 2023-07-24 08:47:08.202319 rec_spotify-1.2.3/rec_spotify/config.py
--rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.2.3/rec_spotify/console.py
--rw-r--r--   0        0        0     7310 2023-07-23 19:42:31.072891 rec_spotify-1.2.3/rec_spotify/database.py
--rw-r--r--   0        0        0     6427 2023-07-23 15:53:09.981754 rec_spotify-1.2.3/rec_spotify/items.py
--rw-r--r--   0        0        0     2195 2023-07-23 16:28:40.968471 rec_spotify-1.2.3/rec_spotify/lyrics.py
--rw-r--r--   0        0        0     6405 2023-07-23 19:54:00.000154 rec_spotify-1.2.3/rec_spotify/manager.py
--rw-r--r--   0        0        0     1968 2023-07-23 16:07:01.827794 rec_spotify-1.2.3/rec_spotify/messages.py
--rw-r--r--   0        0        0     3317 2023-07-23 18:16:28.832707 rec_spotify-1.2.3/rec_spotify/recorder.py
--rw-r--r--   0        0        0     5548 2023-07-24 08:44:02.491961 rec_spotify-1.2.3/rec_spotify/spotify.py
--rw-r--r--   0        0        0     1457 2023-07-23 16:26:57.110938 rec_spotify-1.2.3/rec_spotify/utils.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 rec_spotify-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.3/etc/screen.png
+-rw-r--r--   0        0        0     1289 2023-07-24 14:44:08.434018 rec_spotify-1.3/pyproject.toml
+-rw-r--r--   0        0        0     2406 2023-07-24 14:24:13.736829 rec_spotify-1.3/README.md
+-rw-r--r--   0        0        0       21 2023-07-24 14:44:02.445931 rec_spotify-1.3/rec_spotify/__init__.py
+-rw-r--r--   0        0        0     1735 2023-07-24 09:38:53.871492 rec_spotify-1.3/rec_spotify/cli.py
+-rw-r--r--   0        0        0     4277 2023-07-24 14:27:16.962415 rec_spotify-1.3/rec_spotify/config.py
+-rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.3/rec_spotify/console.py
+-rw-r--r--   0        0        0     7310 2023-07-23 19:42:31.072891 rec_spotify-1.3/rec_spotify/database.py
+-rw-r--r--   0        0        0     6427 2023-07-23 15:53:09.981754 rec_spotify-1.3/rec_spotify/items.py
+-rw-r--r--   0        0        0     2195 2023-07-23 16:28:40.968471 rec_spotify-1.3/rec_spotify/lyrics.py
+-rw-r--r--   0        0        0     6507 2023-07-24 14:41:59.508868 rec_spotify-1.3/rec_spotify/manager.py
+-rw-r--r--   0        0        0     1968 2023-07-23 16:07:01.827794 rec_spotify-1.3/rec_spotify/messages.py
+-rw-r--r--   0        0        0     3317 2023-07-23 18:16:28.832707 rec_spotify-1.3/rec_spotify/recorder.py
+-rw-r--r--   0        0        0     5548 2023-07-24 08:44:02.491961 rec_spotify-1.3/rec_spotify/spotify.py
+-rw-r--r--   0        0        0     2207 2023-07-24 14:59:10.819037 rec_spotify-1.3/rec_spotify/utils.py
+-rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 rec_spotify-1.3/PKG-INFO
```

### Comparing `rec_spotify-1.2.3/etc/screen.png` & `rec_spotify-1.3/etc/screen.png`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/pyproject.toml` & `rec_spotify-1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rec-spotify"
-version = "1.2.3"
+version = "1.3"
 description = "📻 Record and sync Spotify tracks, albums, and playlists."
 repository = "https://github.com/oSeeLight/rec-spotify"
 authors = ["Jacov Rainz <oSeeLight@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rec_spotify"}]
 include = ["README.md", "etc"]
```

### Comparing `rec_spotify-1.2.3/README.md` & `rec_spotify-1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 📻 Rec-Spotify
 
 ![](etc/screen.png)
 
-The program allows you to record Spotify tracks, albums, and playlists with a single simple command. It is also able to fully synchronize your Spotify playlists to a local folder and keep them up-to-date.
+The program allows you to record Spotify tracks, albums, and playlists with a single simple command. It is also able to fully synchronize your Spotify playlists to a local folder and keep them up-to-date. For now it works **only** on Windows.
 
-For now it works **only** on Windows.
+Video Guide: [Watch](https://mega.nz/file/nV8XlKzT#yJhTn7TrQR_6TH3J-26-W2hBHL4W_auAAR0nkzwDsgs)
 
 ## Requirements
 
 - Python3
 - Spotify Premium (no ad blocking functionality)
 - [Virtual Audio Cable](https://vb-audio.com/Cable) (recommended, read below)
 
@@ -49,14 +49,15 @@
 REDIRECT_URL = <REDIRECT_URL>
 
 [SETTINGS]
 MUSIC_DIR = D:\Music
 AUDIO_FORMAT = mp3
 AUDIO_QUALITY = 320
 SAMPLE_RATE = 48000
+TRIM_SILENCE = True
 ```
 
 ## FAQ
 
 ### 1. What is the purpose of this program?
 
 The answer is simple: I want to have local copies of all my Spotify tracks and playlists in original quality. Because who knows maybe one day i will lose access to my account or something else will happen.
@@ -65,10 +66,10 @@
 
 Virtual Audio Cable installation is optional but highly recommended for improved recording quality. It also allows listening to other audio while recording.
 
 
 ## TODO
 
 - [ ] Linux support.
-- [ ] Trim silence from beginning and end of track.
+- [x] Trim silence from beginning and end of track.
 - [ ] Command-line interface for database management of tracks and playlists.
 - [ ] Ad blocking.
```

### Comparing `rec_spotify-1.2.3/rec_spotify/cli.py` & `rec_spotify-1.3/rec_spotify/cli.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/rec_spotify/config.py` & `rec_spotify-1.3/rec_spotify/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     CLIENT_SECRET: str
     REDIRECT_URL: str
     MUSIC_DIR: str
     DATABASE_PATH: str
     AUDIO_FORMAT: str
     AUDIO_QUALITY: int
     SAMPLE_RATE: int
+    TRIM_SILENCE: bool
 
     _DEFAULT_FILENAME = "config.ini"
     _DEFAULT_DBNAME = "spotify.db"
     _DEFAULT_CACHE = ".cache"
 
     @classmethod
     def init(cls) -> None:
@@ -59,14 +60,15 @@
         cls.CLIENT_ID = sp.get("CLIENT_ID")
         cls.CLIENT_SECRET = sp.get("CLIENT_SECRET")
         cls.REDIRECT_URL = sp.get("REDIRECT_URL")
         cls.MUSIC_DIR = os.path.normpath(sn.get("MUSIC_DIR"))
         cls.AUDIO_FORMAT = sn.get("AUDIO_FORMAT")
         cls.AUDIO_QUALITY = sn.getint("AUDIO_QUALITY")
         cls.SAMPLE_RATE = sn.getint("SAMPLE_RATE")
+        cls.TRIM_SILENCE = sn.getboolean("TRIM_SILENCE")
 
     @classmethod
     def create_config_file(cls) -> None:
         """
         Creates a new configuration file.
 
         This method creates a new configuration file by prompting the user for input using the console.
@@ -79,14 +81,15 @@
             "REDIRECT_URL": console.input(":link: REDIRECT_URL: "),
         }
         config["SETTINGS"] = {
             "MUSIC_DIR": console.input(":file_folder: MUSIC DIRECTORY: "),
             "AUDIO_FORMAT": "mp3",
             "AUDIO_QUALITY": "320",
             "SAMPLE_RATE": "48000",
+            "TRIM_SILENCE": "True",
         }
 
         if not os.path.exists(cls.get_config_folder()):
             os.mkdir(cls.get_config_folder())
 
         with open(cls.get_config_filepath(), "w") as file:
             config.write(file)
```

### Comparing `rec_spotify-1.2.3/rec_spotify/console.py` & `rec_spotify-1.3/rec_spotify/console.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/rec_spotify/database.py` & `rec_spotify-1.3/rec_spotify/database.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/rec_spotify/items.py` & `rec_spotify-1.3/rec_spotify/items.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/rec_spotify/lyrics.py` & `rec_spotify-1.3/rec_spotify/lyrics.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/rec_spotify/manager.py` & `rec_spotify-1.3/rec_spotify/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from rec_spotify.database import Database
 import rec_spotify.messages as m
 from rec_spotify.console import console
 from rec_spotify.spotify import SpotifyClient
 from rec_spotify.items import Track, Collection
 from rec_spotify.config import Config
-from rec_spotify.utils import download_cover, get_estimate_time
+from rec_spotify.utils import download_cover, get_estimate_time, trim_silence
 from rec_spotify.recorder import Recorder
 from rec_spotify.lyrics import Lyrics
 
 
 class Manager(object):
     @classmethod
     def sync(cls) -> None:
@@ -145,14 +145,16 @@
     @classmethod
     def _record_and_save(cls, track: Track) -> None:
         "Helper method to record and save a single track."
         metadata = SpotifyClient.get_track_metadata(track)
         song_cover = download_cover(metadata["cover_url"])
         recorded_obj = Recorder.record(track)
         track.set_download_path()
+        if Config.TRIM_SILENCE:
+            recorded_obj = trim_silence(recorded_obj)
         recorded_obj.export(
             out_f=track.filepath,
             format=Config.AUDIO_FORMAT,
             codec="libmp3lame",
             parameters=["-b:a", "320k", "-abr", "1"],
             tags=metadata,
             cover=song_cover.name,
```

### Comparing `rec_spotify-1.2.3/rec_spotify/messages.py` & `rec_spotify-1.3/rec_spotify/messages.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/rec_spotify/recorder.py` & `rec_spotify-1.3/rec_spotify/recorder.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/rec_spotify/spotify.py` & `rec_spotify-1.3/rec_spotify/spotify.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.3/rec_spotify/utils.py` & `rec_spotify-1.3/rec_spotify/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import re
 import tempfile
 import shutil
 import requests
 import math
+import typing as t
+
+from pydub import AudioSegment
+from pydub.silence import detect_leading_silence
 
 
 def parse_spotify_url(url: str) -> tuple[str, str] | None:
     "Parses a Spotify URL and returns the type of link and its ID."
     match = re.search(r"open\.spotify\.com/(track|album|playlist)/(\w+)", url.strip())
     if match:
         link_type = match.group(1)
@@ -41,7 +45,28 @@
 def clear_unwanted(text: str) -> str:
     "Clear unwanted characters from a string."
     text = text.strip()
     unwanted_chars = r" /\:*?\"<>|%^&!()'."
     table = str.maketrans({char: "_" for char in unwanted_chars})
     text = text.translate(table)
     return text
+
+
+@t.no_type_check
+def trim_silence(audio: AudioSegment) -> AudioSegment:
+    "Remove leading and trailing silence from an audio segment."
+
+    def trim_leading_silence(x):
+        return x[detect_leading_silence(x) :]  # noqa
+
+    def trim_trailing_silence(x):
+        reversed_x = x.reverse()
+        trimmed = trim_leading_silence(reversed_x)
+        return trimmed.reverse()
+
+    def strip_silence(x):
+        trimmed_leading = trim_leading_silence(x)
+        trimmed_trailing = trim_trailing_silence(trimmed_leading)
+        return trimmed_trailing
+
+    stripped: AudioSegment = strip_silence(audio)
+    return stripped
```

### Comparing `rec_spotify-1.2.3/PKG-INFO` & `rec_spotify-1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rec-spotify
-Version: 1.2.3
+Version: 1.3
 Summary: 📻 Record and sync Spotify tracks, albums, and playlists.
 Home-page: https://github.com/oSeeLight/rec-spotify
 License: MIT
 Keywords: spotify,record
 Author: Jacov Rainz
 Author-email: oSeeLight@proton.me
 Requires-Python: >=3.11,<4.0
@@ -20,17 +20,17 @@
 Project-URL: Repository, https://github.com/oSeeLight/rec-spotify
 Description-Content-Type: text/markdown
 
 # 📻 Rec-Spotify
 
 ![](etc/screen.png)
 
-The program allows you to record Spotify tracks, albums, and playlists with a single simple command. It is also able to fully synchronize your Spotify playlists to a local folder and keep them up-to-date.
+The program allows you to record Spotify tracks, albums, and playlists with a single simple command. It is also able to fully synchronize your Spotify playlists to a local folder and keep them up-to-date. For now it works **only** on Windows.
 
-For now it works **only** on Windows.
+Video Guide: [Watch](https://mega.nz/file/nV8XlKzT#yJhTn7TrQR_6TH3J-26-W2hBHL4W_auAAR0nkzwDsgs)
 
 ## Requirements
 
 - Python3
 - Spotify Premium (no ad blocking functionality)
 - [Virtual Audio Cable](https://vb-audio.com/Cable) (recommended, read below)
 
@@ -71,14 +71,15 @@
 REDIRECT_URL = <REDIRECT_URL>
 
 [SETTINGS]
 MUSIC_DIR = D:\Music
 AUDIO_FORMAT = mp3
 AUDIO_QUALITY = 320
 SAMPLE_RATE = 48000
+TRIM_SILENCE = True
 ```
 
 ## FAQ
 
 ### 1. What is the purpose of this program?
 
 The answer is simple: I want to have local copies of all my Spotify tracks and playlists in original quality. Because who knows maybe one day i will lose access to my account or something else will happen.
@@ -87,11 +88,11 @@
 
 Virtual Audio Cable installation is optional but highly recommended for improved recording quality. It also allows listening to other audio while recording.
 
 
 ## TODO
 
 - [ ] Linux support.
-- [ ] Trim silence from beginning and end of track.
+- [x] Trim silence from beginning and end of track.
 - [ ] Command-line interface for database management of tracks and playlists.
 - [ ] Ad blocking.
```

