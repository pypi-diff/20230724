# Comparing `tmp/reddit-dl-0.0.2.tar.gz` & `tmp/reddit-dl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit-dl-0.0.2.tar", last modified: Sun Jul 23 21:25:07 2023, max compression
+gzip compressed data, was "reddit-dl-0.0.3.tar", last modified: Mon Jul 24 03:42:20 2023, max compression
```

## Comparing `reddit-dl-0.0.2.tar` & `reddit-dl-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 beg       (1000) beg       (1000)        0 2023-07-23 21:25:07.558393 reddit-dl-0.0.2/
--rw-r--r--   0 beg       (1000) beg       (1000)     1066 2023-07-23 20:29:11.000000 reddit-dl-0.0.2/LICENSE
--rw-r--r--   0 beg       (1000) beg       (1000)      582 2023-07-23 21:25:07.558393 reddit-dl-0.0.2/PKG-INFO
--rw-r--r--   0 beg       (1000) beg       (1000)       57 2023-07-23 20:41:11.000000 reddit-dl-0.0.2/README.md
--rw-r--r--   0 beg       (1000) beg       (1000)      742 2023-07-23 21:23:04.000000 reddit-dl-0.0.2/pyproject.toml
--rw-r--r--   0 beg       (1000) beg       (1000)       38 2023-07-23 21:25:07.558393 reddit-dl-0.0.2/setup.cfg
-drwxr-xr-x   0 beg       (1000) beg       (1000)        0 2023-07-23 21:25:07.554393 reddit-dl-0.0.2/src/
-drwxr-xr-x   0 beg       (1000) beg       (1000)        0 2023-07-23 21:25:07.554393 reddit-dl-0.0.2/src/reddit_dl/
--rw-r--r--   0 beg       (1000) beg       (1000)       24 2023-07-23 21:24:26.000000 reddit-dl-0.0.2/src/reddit_dl/__init__.py
--rw-r--r--   0 beg       (1000) beg       (1000)     5853 2023-07-23 21:24:28.000000 reddit-dl-0.0.2/src/reddit_dl/__main__.py
--rw-r--r--   0 beg       (1000) beg       (1000)    12672 2023-07-23 21:24:31.000000 reddit-dl-0.0.2/src/reddit_dl/constants.py
--rw-r--r--   0 beg       (1000) beg       (1000)     5675 2023-07-23 21:24:33.000000 reddit-dl-0.0.2/src/reddit_dl/downloader.py
--rw-r--r--   0 beg       (1000) beg       (1000)      325 2023-07-23 21:24:35.000000 reddit-dl-0.0.2/src/reddit_dl/exceptions.py
--rw-r--r--   0 beg       (1000) beg       (1000)    14627 2023-07-23 21:24:38.000000 reddit-dl-0.0.2/src/reddit_dl/reddit_dl.py
--rw-r--r--   0 beg       (1000) beg       (1000)     1395 2023-07-23 21:24:41.000000 reddit-dl-0.0.2/src/reddit_dl/redgifs.py
--rw-r--r--   0 beg       (1000) beg       (1000)     1009 2023-07-23 21:24:43.000000 reddit-dl-0.0.2/src/reddit_dl/utils.py
-drwxr-xr-x   0 beg       (1000) beg       (1000)        0 2023-07-23 21:25:07.558393 reddit-dl-0.0.2/src/reddit_dl.egg-info/
--rw-r--r--   0 beg       (1000) beg       (1000)      582 2023-07-23 21:25:07.000000 reddit-dl-0.0.2/src/reddit_dl.egg-info/PKG-INFO
--rw-r--r--   0 beg       (1000) beg       (1000)      466 2023-07-23 21:25:07.000000 reddit-dl-0.0.2/src/reddit_dl.egg-info/SOURCES.txt
--rw-r--r--   0 beg       (1000) beg       (1000)        1 2023-07-23 21:25:07.000000 reddit-dl-0.0.2/src/reddit_dl.egg-info/dependency_links.txt
--rw-r--r--   0 beg       (1000) beg       (1000)       54 2023-07-23 21:25:07.000000 reddit-dl-0.0.2/src/reddit_dl.egg-info/entry_points.txt
--rw-r--r--   0 beg       (1000) beg       (1000)       46 2023-07-23 21:25:07.000000 reddit-dl-0.0.2/src/reddit_dl.egg-info/requires.txt
--rw-r--r--   0 beg       (1000) beg       (1000)       10 2023-07-23 21:25:07.000000 reddit-dl-0.0.2/src/reddit_dl.egg-info/top_level.txt
+drwxr-xr-x   0 beg       (1000) beg       (1000)        0 2023-07-24 03:42:20.063922 reddit-dl-0.0.3/
+-rw-r--r--   0 beg       (1000) beg       (1000)     1066 2023-07-23 21:28:45.000000 reddit-dl-0.0.3/LICENSE
+-rw-r--r--   0 beg       (1000) beg       (1000)     3600 2023-07-24 03:42:20.063922 reddit-dl-0.0.3/PKG-INFO
+-rw-r--r--   0 beg       (1000) beg       (1000)     3076 2023-07-24 03:38:17.000000 reddit-dl-0.0.3/README.md
+-rw-r--r--   0 beg       (1000) beg       (1000)      742 2023-07-24 03:05:34.000000 reddit-dl-0.0.3/pyproject.toml
+-rw-r--r--   0 beg       (1000) beg       (1000)       38 2023-07-24 03:42:20.063922 reddit-dl-0.0.3/setup.cfg
+drwxr-xr-x   0 beg       (1000) beg       (1000)        0 2023-07-24 03:42:20.059922 reddit-dl-0.0.3/src/
+drwxr-xr-x   0 beg       (1000) beg       (1000)        0 2023-07-24 03:42:20.063922 reddit-dl-0.0.3/src/reddit_dl/
+-rw-r--r--   0 beg       (1000) beg       (1000)       47 2023-07-24 03:24:20.000000 reddit-dl-0.0.3/src/reddit_dl/__init__.py
+-rw-r--r--   0 beg       (1000) beg       (1000)     5800 2023-07-24 03:28:33.000000 reddit-dl-0.0.3/src/reddit_dl/__main__.py
+-rw-r--r--   0 beg       (1000) beg       (1000)    12697 2023-07-24 03:24:13.000000 reddit-dl-0.0.3/src/reddit_dl/constants.py
+-rw-r--r--   0 beg       (1000) beg       (1000)     5565 2023-07-24 03:30:23.000000 reddit-dl-0.0.3/src/reddit_dl/downloader.py
+-rw-r--r--   0 beg       (1000) beg       (1000)      349 2023-07-24 03:30:27.000000 reddit-dl-0.0.3/src/reddit_dl/exceptions.py
+-rw-r--r--   0 beg       (1000) beg       (1000)    14628 2023-07-24 03:30:40.000000 reddit-dl-0.0.3/src/reddit_dl/reddit_dl.py
+-rw-r--r--   0 beg       (1000) beg       (1000)     1557 2023-07-24 03:30:48.000000 reddit-dl-0.0.3/src/reddit_dl/redgifs.py
+-rw-r--r--   0 beg       (1000) beg       (1000)     1002 2023-07-24 03:30:51.000000 reddit-dl-0.0.3/src/reddit_dl/utils.py
+drwxr-xr-x   0 beg       (1000) beg       (1000)        0 2023-07-24 03:42:20.063922 reddit-dl-0.0.3/src/reddit_dl.egg-info/
+-rw-r--r--   0 beg       (1000) beg       (1000)     3600 2023-07-24 03:42:20.000000 reddit-dl-0.0.3/src/reddit_dl.egg-info/PKG-INFO
+-rw-r--r--   0 beg       (1000) beg       (1000)      466 2023-07-24 03:42:20.000000 reddit-dl-0.0.3/src/reddit_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 beg       (1000) beg       (1000)        1 2023-07-24 03:42:20.000000 reddit-dl-0.0.3/src/reddit_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 beg       (1000) beg       (1000)       54 2023-07-24 03:42:20.000000 reddit-dl-0.0.3/src/reddit_dl.egg-info/entry_points.txt
+-rw-r--r--   0 beg       (1000) beg       (1000)       46 2023-07-24 03:42:20.000000 reddit-dl-0.0.3/src/reddit_dl.egg-info/requires.txt
+-rw-r--r--   0 beg       (1000) beg       (1000)       10 2023-07-24 03:42:20.000000 reddit-dl-0.0.3/src/reddit_dl.egg-info/top_level.txt
```

### Comparing `reddit-dl-0.0.2/LICENSE` & `reddit-dl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit-dl-0.0.2/pyproject.toml` & `reddit-dl-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reddit-dl"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="redloaders", email="redloader@tutanota.com" },
 ]
 description = "Limitless Reddit Downloader. No API no LIMIT."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `reddit-dl-0.0.2/src/reddit_dl/__main__.py` & `reddit-dl-0.0.3/src/reddit_dl/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 """Download pictures, gifs, videos along with their captions and other metadata from Reddit."""
 
+import os
+import sys
 from typing import List
 from argparse import ArgumentParser, ArgumentTypeError, SUPPRESS
 from urllib.parse import urlparse, urlunparse
-import os
 
 from . import __version__
 from .reddit_dl import RedditDownloader
 from .utils import is_valid_url
 from .exceptions import ExistFileOnUpdateModeException, ConnectionException
 
 
@@ -58,35 +59,37 @@
 def _main(redl: RedditDownloader, targetlist: List[str]) -> None:
 
     for target in targetlist:
         print(f'Downloading: {urlparse(target).path}')
 
         try:
             redl.download(target)
-        except ExistFileOnUpdateModeException as err:
+        except ExistFileOnUpdateModeException:
             print('\nUpdate completed.')
-        except ConnectionException as err:
-            print(err)
+        except ConnectionException:
+            if redl.raise_exception:
+                raise
 
 def main():
     """Entry point for cli."""
 
     try:
         parser = ArgumentParser(
             description=__doc__, add_help=False, fromfile_prefix_chars='+',
-            epilog="The complete documentation can be found at https://instaloader.github.io/.")
+            epilog="https://github.com/reddit-dl/reddit-dl")
 
         g_misc = parser.add_argument_group('Miscellaneous Options')
         g_misc.add_argument('-h', '--help', action='help', help='Show this help message and exit.')
         g_misc.add_argument(
-            '--version', action='version', help='Show version number and exit.', version=__version__)
+            '--version', action='version', 
+            help='Show version number and exit.', version=__version__)
 
         g_targets = parser.add_argument_group(
             "What to Download",
-            "Specify a list of targets. For each of these, RedditDL creates a folder "
+            "Specify a list of targets. For each of these, reddit-dl creates a folder "
             "and downloads all media content. The following targets are supported:")
         g_targets.add_argument(
             'target',
             nargs='*',
             type=is_valid_target,
             help="Full url of users, subreddits or their local folder names."
                 "Exp. `https://reddit.com/r/UkrainianConflict/`")
@@ -95,19 +98,17 @@
         g_targets.add_argument('-r', '--reddit', nargs='*', help="Subreddit names to download.")
 
         g_post = parser.add_argument_group("What to Download of each Post")
         g_post.add_argument('--metadata-json', action='store_true', help=SUPPRESS)
         g_post.add_argument(
             '-V', '--no-videos', action='store_true', help='Do not download videos.')
         g_post.add_argument(
-            '-P', '--no-pictures', action='store_true',
-            help='Do not download pictures. Cannot be used together with --fast-update.')
+            '-P', '--no-pictures', action='store_true', help='Do not download pictures.')
         g_post.add_argument(
-            '-G', '--no-gifs', action='store_true',
-            help='Do not download pictures. Cannot be used together with --fast-update.')
+            '-G', '--no-gifs', action='store_true',help='Do not download pictures.')
         g_post.add_argument(
             '-N', '--no-nsfw', action='store_true', help='Do not download NSFW content.')
 
         g_cond = parser.add_argument_group("Which Posts to Download")
         g_cond.add_argument(
             '--update', action='store_true',
             help='For each target, stop when encountering the first already-downloaded content.')
@@ -117,16 +118,16 @@
         g_how.add_argument(
             '--request-timeout', metavar='N', type=float, default=300.0,
             help='Seconds to wait before timing out a connection request. Defaults to 300.')
         g_how.add_argument(
             '--max-connection-attempts', metavar='N', type=int, default=3,
             help='Maximum number of connection attempts until a request is aborted.')
         g_how.add_argument('-S', '--no-sleep', action='store_true', help=SUPPRESS)
-
-        args = parser.parse_args()
+        
+        args = parser.parse_args(args=None if sys.argv[1:] else ['--help'])
         url_list = [
             *build_url(args.user, 'user'),
             *build_url(args.reddit, 'reddit'),
             *build_url(args.target, 'target'),
         ]
 
         redl = RedditDownloader(
```

### Comparing `reddit-dl-0.0.2/src/reddit_dl/constants.py` & `reddit-dl-0.0.3/src/reddit_dl/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf-8 -*-
+
 USERAGENTS = [
   "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
   "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.67",
   "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.3",
   "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
   "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0",
   "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:109.0) Gecko/20100101 Firefox/114.0",
```

### Comparing `reddit-dl-0.0.2/src/reddit_dl/downloader.py` & `reddit-dl-0.0.3/src/reddit_dl/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+# -*- coding: utf-8 -*-
+
 """reddit_dl.downloader: downloader module"""
 
 import os
 import re
 import subprocess
 from random import choice
 from urllib.parse import urlparse, unquote, urljoin, urlunparse
 from pathlib import PurePosixPath
 from typing import Optional
 
 import requests
 import m3u8
 
 from .utils import url_to_filename
-from .exceptions import ExistFileOnUpdateModeException
 from .constants import USERAGENTS, TIMEOUT
 
+
 HEADERS = {
     'User-Agent': choice(USERAGENTS),
     'Accept-Language': 'en-US,en;q=0.5',
     'Accept': '*/*',
 }
 
 def hls_extractor(url: str) -> list:
@@ -67,31 +69,31 @@
 
     return hls_data
 
 def merge_hls(
         output: str,
         video: str,
         audio: Optional[str] = None,
-        ) -> None:
+        ):
     """Merge audio and video file.
 
     :param output: Output file full path. exp. /home/sky/funny_video.mp4
     :param video: Video file full path. exp. /home/sky/video.webm
     :param audio: Audio file full path. exp. /home/sky/audio.mp3"""
 
     if audio and video:
         cmd = f'ffmpeg -loglevel panic -i "{video}" -i "{audio}" -c:v copy -c:a aac "{output}"'
         subprocess.call(cmd, shell=True)
-        if os.path.exist(output):
+        if os.path.exists(output):
             os.remove(video)
             os.remove(audio)
     elif video:
         cmd = f'ffmpeg -loglevel panic -i "{video}" {output}'
         subprocess.call(cmd, shell=True)
-        if os.path.exist(output):
+        if os.path.exists(output):
             os.remove(video)
 
 class Downloader:
     """Simple downloader"""
     def __init__(
             self, update_mode: bool = False, request_timeout: int = TIMEOUT,
             raise_exception: bool = True, headers: Optional[dict] = None,):
@@ -113,38 +115,36 @@
 
         # Check is hls
         if re.search(r'.m3u8(\?+|$)', url):
             return self._hls_downloader(url, path, output_format)
         return self._downloader(url, path)
 
     def _downloader(
-            self, url, path: str) -> None:
+            self, url, path: str):
         """Download video, image or gif."""
 
         file_name = url_to_filename(url)
         full_path = os.path.join(path, file_name)
 
         with requests.get(
             url, stream=True, headers=self.headers, timeout=self.request_timeout) as res:
             if not res.status_code == 404 and self.raise_exception:
                 res.raise_for_status()
-             # If last part of url has changed, than return
+
+            # If last part of url has changed, than return
             res_url = PurePosixPath(unquote(urlparse(res.url).path)).parts[-1]
             req_url = PurePosixPath(unquote(urlparse(url).path)).parts[-1]
-            if res_url != req_url:
-                return None
 
-            with open(full_path, 'wb') as file:
-                for chunk in res.iter_content(chunk_size=8192):
-                    file.write(chunk)
-
-        return None
+            if res_url == req_url:
+                with open(full_path, 'wb') as file:
+                    for chunk in res.iter_content(chunk_size=8192):
+                        file.write(chunk)
 
     def _hls_downloader(
-            self, url: str, path: str, output_format: str='mp4') -> None:
+            self, url: str, path: str, output_format: str='mp4'):
         """Downloads hls media."""
 
         file_name = url_to_filename(url)
         media_path = os.path.join(path, file_name)
         output_full_path = f"{media_path}.{output_format}"
         to_merged = {"output": output_full_path}
         hls_data = hls_extractor(url)
@@ -158,13 +158,11 @@
             with open(f"{media_path}.{data['type']}", "wb") as file:
                 for url_ in data['segment_urls']:
                     res =  requests.get(url_, timeout=self.request_timeout, headers=self.headers)
 
                     if res.ok:
                         file.write(res.content)
                     elif self.raise_exception:
-                         res.raise_for_status()
+                        res.raise_for_status()
 
         # Finally merge or convert to .mp4
         merge_hls(**to_merged)
-
-        return None
```

### Comparing `reddit-dl-0.0.2/src/reddit_dl/reddit_dl.py` & `reddit-dl-0.0.3/src/reddit_dl/reddit_dl.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from .downloader import Downloader
 from .utils import url_to_filename
 from .exceptions import ConnectionException, ExistFileOnUpdateModeException
 from .constants import USERAGENTS
 from .redgifs import get_redgifs_token, get_redgifs_video
 
+
 __version__ = "0.0.1"
 
 HEADERS = {
     'Cookie': 'over18=1',
     'User-Agent': choice(USERAGENTS),
     'Accept': '*/*',
 }
```

### Comparing `reddit-dl-0.0.2/src/reddit_dl/redgifs.py` & `reddit-dl-0.0.3/src/reddit_dl/redgifs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,45 @@
+# -*- coding: utf-8 -*-
+
+"""redgifs.com Related Module"""
 
 from urllib.parse import urlparse, unquote
 from pathlib import PurePosixPath
 from random import choice
 
 import requests
 
 from .constants import USERAGENTS, TIMEOUT
 
+
 HEADERS = {
     'User-Agent': choice(USERAGENTS),
     'Accept': '*/*',
 }
 
-
 def get_redgifs_token(timeout: int = TIMEOUT) -> str:
     """Returns guest bearer token for redgifs api."""
     token_url = 'https://api.redgifs.com/v2/auth/temporary'
     res = requests.get(token_url, headers=HEADERS, timeout=timeout)
     res.raise_for_status()
 
     return res.json()['token']
 
-
 def get_redgifs_video(url: str, bearer: str = None, timeout: int = TIMEOUT) -> str:
+    """Returns downloadable video url from url. 
+    If url can't be found than returns empty string."""
 
     bearer = get_redgifs_token() if not bearer else bearer
     bearered_header = {'Authorization': f'Bearer {bearer}'}
     vid_name = PurePosixPath(unquote(urlparse(url).path)).parts[-1].lower()
 
-
     vid_url = f'https://api.redgifs.com/v2/gifs/{vid_name}'
     res = requests.get(vid_url, headers=bearered_header, timeout=timeout)
 
-    # When content is deleted gives error code `413`
+    # When content is deleted gives error code `410`
     if res.status_code in [410, 404] :
         return ''
 
     # Raise for other bad codes
     res.raise_for_status()
 
     try:
@@ -47,8 +50,8 @@
         return ''
 
     vd_url = urls['hd'] if urls.get('hd') else urls.get('sd')
 
     if not vd_url:
         return ''
 
-    return vd_url
+    return vd_url
```

### Comparing `reddit-dl-0.0.2/src/reddit_dl/utils.py` & `reddit-dl-0.0.3/src/reddit_dl/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
+# -*- coding: utf-8 -*-
+
 """Helper Utils Module"""
 
-import os
-import json
 import re
-from urllib.parse import urlparse, unquote
-from pathlib import PurePosixPath, Path
-
-import requests
+from urllib.parse import urlparse
 
 from .constants import ALLOWED_URLS
 
+
 def is_valid_url(url: str) -> bool:
     """Checks url is valid for Reddit, Teddit or Libreddit instances.
     If url is valid than returns url other wise False."""
 
     parsed_url = urlparse(url)
 
     if not re.search(r'/(r|reddit|u|user)+\/[a-zA-Z_0-9-]+?', parsed_url.path):
         return False
 
     for _ in ALLOWED_URLS:
         if urlparse(_).netloc in url:
             return True
-
+            
     return False
 
-def url_to_filename(url):
+def url_to_filename(url: str):
+    """Create file name from url."""
+
     filename_regexed = re.search(r'[^/\\&\?]+\.\w{3,4}(?=([\?&].*$|$))', url)
 
     if not filename_regexed:
         return None
 
     filename = filename_regexed[0]
```

