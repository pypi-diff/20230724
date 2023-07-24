# Comparing `tmp/rec_spotify-1.2.2.tar.gz` & `tmp/rec_spotify-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rec_spotify-1.2.2.tar", max compression
+gzip compressed data, was "rec_spotify-1.2.3.tar", max compression
```

## Comparing `rec_spotify-1.2.2.tar` & `rec_spotify-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.2.2/etc/screen.png
--rw-r--r--   0        0        0     1291 2023-07-23 20:44:03.304974 rec_spotify-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2289 2023-07-23 20:20:05.543332 rec_spotify-1.2.2/README.md
--rw-r--r--   0        0        0       21 2023-07-23 20:45:10.978234 rec_spotify-1.2.2/rec_spotify/__init__.py
--rw-r--r--   0        0        0     1735 2023-07-23 20:50:02.825572 rec_spotify-1.2.2/rec_spotify/cli.py
--rw-r--r--   0        0        0     3915 2023-07-23 18:15:50.766094 rec_spotify-1.2.2/rec_spotify/config.py
--rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.2.2/rec_spotify/console.py
--rw-r--r--   0        0        0     7310 2023-07-23 19:42:31.072891 rec_spotify-1.2.2/rec_spotify/database.py
--rw-r--r--   0        0        0     6427 2023-07-23 15:53:09.981754 rec_spotify-1.2.2/rec_spotify/items.py
--rw-r--r--   0        0        0     2195 2023-07-23 16:28:40.968471 rec_spotify-1.2.2/rec_spotify/lyrics.py
--rw-r--r--   0        0        0     6405 2023-07-23 19:54:00.000154 rec_spotify-1.2.2/rec_spotify/manager.py
--rw-r--r--   0        0        0     1968 2023-07-23 16:07:01.827794 rec_spotify-1.2.2/rec_spotify/messages.py
--rw-r--r--   0        0        0     3317 2023-07-23 18:16:28.832707 rec_spotify-1.2.2/rec_spotify/recorder.py
--rw-r--r--   0        0        0     5375 2023-07-23 17:02:19.699967 rec_spotify-1.2.2/rec_spotify/spotify.py
--rw-r--r--   0        0        0     1457 2023-07-23 16:26:57.110938 rec_spotify-1.2.2/rec_spotify/utils.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 rec_spotify-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.2.3/etc/screen.png
+-rw-r--r--   0        0        0     1291 2023-07-24 08:45:23.861481 rec_spotify-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2289 2023-07-23 20:20:05.543332 rec_spotify-1.2.3/README.md
+-rw-r--r--   0        0        0       23 2023-07-24 08:45:30.849755 rec_spotify-1.2.3/rec_spotify/__init__.py
+-rw-r--r--   0        0        0     1735 2023-07-23 20:50:02.825572 rec_spotify-1.2.3/rec_spotify/cli.py
+-rw-r--r--   0        0        0     4158 2023-07-24 08:47:08.202319 rec_spotify-1.2.3/rec_spotify/config.py
+-rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.2.3/rec_spotify/console.py
+-rw-r--r--   0        0        0     7310 2023-07-23 19:42:31.072891 rec_spotify-1.2.3/rec_spotify/database.py
+-rw-r--r--   0        0        0     6427 2023-07-23 15:53:09.981754 rec_spotify-1.2.3/rec_spotify/items.py
+-rw-r--r--   0        0        0     2195 2023-07-23 16:28:40.968471 rec_spotify-1.2.3/rec_spotify/lyrics.py
+-rw-r--r--   0        0        0     6405 2023-07-23 19:54:00.000154 rec_spotify-1.2.3/rec_spotify/manager.py
+-rw-r--r--   0        0        0     1968 2023-07-23 16:07:01.827794 rec_spotify-1.2.3/rec_spotify/messages.py
+-rw-r--r--   0        0        0     3317 2023-07-23 18:16:28.832707 rec_spotify-1.2.3/rec_spotify/recorder.py
+-rw-r--r--   0        0        0     5548 2023-07-24 08:44:02.491961 rec_spotify-1.2.3/rec_spotify/spotify.py
+-rw-r--r--   0        0        0     1457 2023-07-23 16:26:57.110938 rec_spotify-1.2.3/rec_spotify/utils.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 rec_spotify-1.2.3/PKG-INFO
```

### Comparing `rec_spotify-1.2.2/etc/screen.png` & `rec_spotify-1.2.3/etc/screen.png`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/pyproject.toml` & `rec_spotify-1.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rec-spotify"
-version = "1.2.2"
+version = "1.2.3"
 description = "📻 Record and sync Spotify tracks, albums, and playlists."
 repository = "https://github.com/oSeeLight/rec-spotify"
 authors = ["Jacov Rainz <oSeeLight@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rec_spotify"}]
 include = ["README.md", "etc"]
```

### Comparing `rec_spotify-1.2.2/README.md` & `rec_spotify-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/cli.py` & `rec_spotify-1.2.3/rec_spotify/cli.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/config.py` & `rec_spotify-1.2.3/rec_spotify/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     DATABASE_PATH: str
     AUDIO_FORMAT: str
     AUDIO_QUALITY: int
     SAMPLE_RATE: int
 
     _DEFAULT_FILENAME = "config.ini"
     _DEFAULT_DBNAME = "spotify.db"
+    _DEFAULT_CACHE = ".cache"
 
     @classmethod
     def init(cls) -> None:
         """
         Initializes the Config class.
 
         This method checks if a configuration file exists and if not,
@@ -118,7 +119,14 @@
 
     @classmethod
     def get_config_filepath(cls) -> str:
         """
         Returns the file path for the config file.
         """
         return os.path.join(cls.get_config_folder(), cls._DEFAULT_FILENAME)
+
+    @classmethod
+    def get_cache_filepath(cls) -> str:
+        """
+        Returns the file path for the cache file.
+        """
+        return os.path.join(cls.get_config_folder(), cls._DEFAULT_CACHE)
```

### Comparing `rec_spotify-1.2.2/rec_spotify/console.py` & `rec_spotify-1.2.3/rec_spotify/console.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/database.py` & `rec_spotify-1.2.3/rec_spotify/database.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/items.py` & `rec_spotify-1.2.3/rec_spotify/items.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/lyrics.py` & `rec_spotify-1.2.3/rec_spotify/lyrics.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/manager.py` & `rec_spotify-1.2.3/rec_spotify/manager.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/messages.py` & `rec_spotify-1.2.3/rec_spotify/messages.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/recorder.py` & `rec_spotify-1.2.3/rec_spotify/recorder.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/rec_spotify/spotify.py` & `rec_spotify-1.2.3/rec_spotify/spotify.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import typing as t
 from requests.exceptions import RequestException
 
 import spotipy
 from spotipy.client import Spotify
-from spotipy.oauth2 import SpotifyOAuth
+from spotipy.oauth2 import SpotifyOAuth, CacheFileHandler
 from rec_spotify.items import Track, Collection
 
 import rec_spotify.messages as m
 from rec_spotify.config import Config
 from rec_spotify.console import clear_lines, console
 
 
@@ -23,14 +23,15 @@
     @classmethod
     def init(cls) -> None:
         cls._client = spotipy.Spotify(
             auth_manager=SpotifyOAuth(
                 client_id=Config.CLIENT_ID,
                 client_secret=Config.CLIENT_SECRET,
                 redirect_uri=Config.REDIRECT_URL,
+                cache_handler=CacheFileHandler(cache_path=Config.get_cache_filepath()),
                 scope="streaming, playlist-read-private, user-read-playback-state, user-modify-playback-state",
             )
         )
         cls._set_device_id()
 
     @classmethod
     def get_track(cls, track: Track) -> Track:
@@ -147,13 +148,14 @@
         "Helper method to make API request."
         while True:
             try:
                 resp = method(*args, **kwarsg)
                 return resp
             except RequestException as ex:
                 console.print(m.REQ_ERROR.format(error=ex))
-            except spotipy.exceptions.SpotifyException:
-                breakpoint()
+            except spotipy.exceptions.SpotifyException as ex:
+                console.print(m.REQ_ERROR.format(error=ex))
+                sys.exit(1)
 
     @classmethod
     def close(cls) -> None:
         cls._client.pause_playback(device_id=cls._device_id)
```

### Comparing `rec_spotify-1.2.2/rec_spotify/utils.py` & `rec_spotify-1.2.3/rec_spotify/utils.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.2.2/PKG-INFO` & `rec_spotify-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rec-spotify
-Version: 1.2.2
+Version: 1.2.3
 Summary: 📻 Record and sync Spotify tracks, albums, and playlists.
 Home-page: https://github.com/oSeeLight/rec-spotify
 License: MIT
 Keywords: spotify,record
 Author: Jacov Rainz
 Author-email: oSeeLight@proton.me
 Requires-Python: >=3.11,<4.0
```

