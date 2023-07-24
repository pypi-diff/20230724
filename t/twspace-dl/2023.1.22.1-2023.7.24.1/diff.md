# Comparing `tmp/twspace_dl-2023.1.22.1.tar.gz` & `tmp/twspace_dl-2023.7.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twspace_dl-2023.1.22.1.tar", max compression
+gzip compressed data, was "twspace_dl-2023.7.24.1.tar", max compression
```

## Comparing `twspace_dl-2023.1.22.1.tar` & `twspace_dl-2023.7.24.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    18092 2023-01-22 11:31:33.441857 twspace_dl-2023.1.22.1/LICENSE
--rw-r--r--   0        0        0     5989 2023-01-22 11:31:33.441857 twspace_dl-2023.1.22.1/README.md
--rw-r--r--   0        0        0     1065 2023-01-22 11:31:33.901864 twspace_dl-2023.1.22.1/pyproject.toml
--rw-r--r--   0        0        0      259 2023-01-22 11:31:33.905865 twspace_dl-2023.1.22.1/twspace_dl/__init__.py
--rw-r--r--   0        0        0     7952 2023-01-22 11:31:33.905865 twspace_dl-2023.1.22.1/twspace_dl/__main__.py
--rw-r--r--   0        0        0    10508 2023-01-22 11:31:33.905865 twspace_dl-2023.1.22.1/twspace_dl/login.py
--rw-r--r--   0        0        0     1581 2023-01-22 11:31:33.905865 twspace_dl-2023.1.22.1/twspace_dl/twitter.py
--rw-r--r--   0        0        0    10104 2023-01-22 11:31:33.905865 twspace_dl-2023.1.22.1/twspace_dl/twspace.py
--rw-r--r--   0        0        0     6774 2023-01-22 11:31:33.905865 twspace_dl-2023.1.22.1/twspace_dl/twspace_dl.py
--rw-r--r--   0        0        0     6945 1970-01-01 00:00:00.000000 twspace_dl-2023.1.22.1/setup.py
--rw-r--r--   0        0        0     6819 1970-01-01 00:00:00.000000 twspace_dl-2023.1.22.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-07-24 11:01:34.849208 twspace_dl-2023.7.24.1/LICENSE
+-rw-r--r--   0        0        0     6428 2023-07-24 11:01:34.849208 twspace_dl-2023.7.24.1/README.md
+-rw-r--r--   0        0        0     1085 2023-07-24 11:01:35.353206 twspace_dl-2023.7.24.1/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-07-24 11:01:35.353206 twspace_dl-2023.7.24.1/twspace_dl/__init__.py
+-rw-r--r--   0        0        0     7394 2023-07-24 11:01:35.353206 twspace_dl-2023.7.24.1/twspace_dl/__main__.py
+-rw-r--r--   0        0        0    16837 2023-07-24 11:01:35.353206 twspace_dl-2023.7.24.1/twspace_dl/api.py
+-rw-r--r--   0        0        0     1978 2023-07-24 11:01:35.353206 twspace_dl-2023.7.24.1/twspace_dl/cookies.py
+-rw-r--r--   0        0        0     6084 2023-07-24 11:01:35.353206 twspace_dl-2023.7.24.1/twspace_dl/twspace.py
+-rw-r--r--   0        0        0     7061 2023-07-24 11:01:35.353206 twspace_dl-2023.7.24.1/twspace_dl/twspace_dl.py
+-rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 twspace_dl-2023.7.24.1/PKG-INFO
```

### Comparing `twspace_dl-2023.1.22.1/LICENSE` & `twspace_dl-2023.7.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twspace_dl-2023.1.22.1/README.md` & `twspace_dl-2023.7.24.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 ![running](https://user-images.githubusercontent.com/77058942/172581500-174834c5-6883-44f9-a0a7-610dbb2103e5.png)
 
 </details>
 
 
 ## Requirements
 
-ffmpeg if not using portable binaries
+- `ffmpeg` if not using portable binaries.
+- A logged in user's cookies file exported from Twitter in the [Netscape format](https://curl.se/docs/http-cookies.html).
 
 ## Install
 
 ### GUI
 
 Use this if you're not sure.
 
@@ -74,85 +75,86 @@
 ```bash
 pip install git+https://github.com/HoloArchivists/twspace-dl
 ```
 
 ## Usage
 
 ```bash
-twspace_dl -i space_url
+twspace_dl -i space_url -c COOKIE_FILE
 ```
 
 <details>
 <summary>With binaries</summary>
 
 ### Windows
 
-```bash
-.\twspace_dl.exe -i space_url
+```powershell
+.\twspace_dl.exe -i space_url -c COOKIE_FILE
 ```
 
 </details>
 
 ## Features
 
 Here's the output of the help option
 
 ```txt
-usage: twspace_dl [-h] [-v] [-s] [-k] [-l] [--input-cookie-file COOKIE_FILE]
-                  [--username USERNAME] [--password PASSWORD]
-                  [--output-cookie-file OUTPUT_COOKIE_FILE]
+usage: twspace_dl [-h] [-v] [-s] [-k] [-l] -c COOKIE_FILE
                   [-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-M PATH]
-                  [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT]
+                  [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT] [-e]
 
 Script designed to help download twitter spaces
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -v, --verbose
   -s, --skip-download
   -k, --keep-files
   -l, --log             create logfile
-  --input-cookie-file COOKIE_FILE
+  -c COOKIE_FILE, --input-cookie-file COOKIE_FILE
+                        cookies file in the Netscape format. The specs of the
+                        Netscape cookies format can be found here:
+                        https://curl.se/docs/http-cookies.html. The cookies
+                        file is now required due to the Twitter API change
+                        that prohibited guest user access to Twitter API
+                        endpoints on 2023-07-01.
 
 input:
   -i SPACE_URL, --input-url SPACE_URL
   -U USER_URL, --user-url USER_URL
   -d DYN_URL, --from-dynamic-url DYN_URL
                         use the dynamic url for the processes(useful for ended
-                        spaces) example: https://prod-fastly-ap-northeast-1.vi
-                        deo.pscp.tv/Transcoding/v1/hls/zUUpEgiM0M18jCGxo2eSZs9
-                        9p49hfyFQr1l4cdze-Sp4T-DQOMMoZpkbdyetgfwscfvvUkAdeF-I5
-                        hPI4bGoYg/non_transcode/ap-northeast-1/periscope-
+                        spaces) example: https://prod-fastly-ap-northeast-
+                        1.video.pscp.tv/Transcoding/v1/hls/zUUpEgiM0M18jCGxo2e
+                        SZs99p49hfyFQr1l4cdze-Sp4T-
+                        DQOMMoZpkbdyetgfwscfvvUkAdeF-
+                        I5hPI4bGoYg/non_transcode/ap-northeast-1/periscope-
                         replay-direct-prod-ap-northeast-1-public/audio-
                         space/dynamic_playlist.m3u8?type=live
   -f URL, --from-master-url URL
                         use the master url for the processes(useful for ended
-                        spaces) example: https://prod-fastly-ap-northeast-1.vi
-                        deo.pscp.tv/Transcoding/v1/hls/YRSsw6_P5xUZHMualK5-ihv
-                        ePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_vpZ2HnFkoRfar4_uJO
-                        jqC8OCo5A/non_transcode/ap-northeast-1/periscope-
+                        spaces) example: https://prod-fastly-ap-northeast-
+                        1.video.pscp.tv/Transcoding/v1/hls/YRSsw6_P5xUZHMualK5
+                        -ihvePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_vpZ2HnFkoRfar4
+                        _uJOjqC8OCo5A/non_transcode/ap-northeast-1/periscope-
                         replay-direct-prod-ap-northeast-1-public/audio-
                         space/master_playlist.m3u8
   -M PATH, --input-metadata PATH
                         use a metadata json file instead of input url (useful
                         for very old ended spaces)
 
 output:
   -o FORMAT_STR, --output FORMAT_STR
   -m, --write-metadata  write the full metadata json to a file
   -p, --write-playlist  write the m3u8 used to download the stream(e.g. if you
                         want to use another downloader)
   -u, --url             display the master url
   --write-url URL_OUTPUT
                         write master url to file
-
-login:
-  --username USERNAME
-  --password PASSWORD
-  --output-cookie-file OUTPUT_COOKIE_FILE
+  -e, --embed-cover     embed user avatar as cover art
 ```
 
 ## Format
 
 You can use the following identifiers for the formatting
 
 ```python
@@ -169,23 +171,23 @@
 
 ## Known Errors
 
 `Changing ID3 metadata in HLS audio elementary stream is not implemented....`
 
 This is an error in ffmpeg that does not affect twspace_dl at all as far as I know.
 
-## Service 
+## Service
 
 To run as a systemd service please refer to https://github.com/HoloArchivists/twspace-dl/blob/main/SERVICE.md
 
 ## Docker
 
 ### Run once
 
-> Use ${pwd} in powershell, or $(pwd) in bash
+> Use `${pwd}` in powershell, or `$(pwd)` in bash
 
 ```bash
 docker run --rm -v ${pwd}:/output ryu1845/twspace-dl -i space_url
 ```
 
 ### Run as monitoring service
```

#### html2text {}

```diff
@@ -7,57 +7,61 @@
 41f6-852b-b68d32532add.png) ![running tab](https://user-
 images.githubusercontent.com/77058942/172580589-fd6b05bd-f081-4c7a-ab05-
 0640abda00ce.png) ![success pop up](https://user-images.githubusercontent.com/
 77058942/172580861-18b3ac9f-88d2-44cf-8b5d-135990a78f77.png)   CLI ![help]
 (https://user-images.githubusercontent.com/77058942/172581224-9b465f78-4894-
 456f-9b85-5b76ee9bbfca.png) ![running](https://user-
 images.githubusercontent.com/77058942/172581500-174834c5-6883-44f9-a0a7-
-610dbb2103e5.png)  ## Requirements ffmpeg if not using portable binaries ##
-Install ### GUI Use this if you're not sure. ### From portable binaries
-[Windows](https://github.com/HoloArchivists/twspace-dl/releases/latest/
-download/twspace-dl-GUI.exe) ### From source ```bash pip install git+https://
-github.com/HoloArchivists/twspace-dl@gooey ``` ### CLI ### From portable
-binaries [Windows](https://github.com/HoloArchivists/twspace-dl/releases/
-latest/download/twspace-dl-CLI.exe) ### From PyPI ```bash pip install twspace-
-dl ``` ### From source ```bash pip install git+https://github.com/
-HoloArchivists/twspace-dl ``` ## Usage ```bash twspace_dl -i space_url ```
-With binaries ### Windows ```bash .\twspace_dl.exe -i space_url ```  ##
-Features Here's the output of the help option ```txt usage: twspace_dl [-h] [-
-v] [-s] [-k] [-l] [--input-cookie-file COOKIE_FILE] [--username USERNAME] [--
-password PASSWORD] [--output-cookie-file OUTPUT_COOKIE_FILE] [-i SPACE_URL | -
-U USER_URL] [-d DYN_URL] [-f URL] [-M PATH] [-o FORMAT_STR] [-m] [-p] [-u] [--
-write-url URL_OUTPUT] Script designed to help download twitter spaces optional
-arguments: -h, --help show this help message and exit -v, --verbose -s, --skip-
-download -k, --keep-files -l, --log create logfile --input-cookie-file
-COOKIE_FILE input: -i SPACE_URL, --input-url SPACE_URL -U USER_URL, --user-url
-USER_URL -d DYN_URL, --from-dynamic-url DYN_URL use the dynamic url for the
-processes(useful for ended spaces) example: https://prod-fastly-ap-northeast-
-1.vi deo.pscp.tv/Transcoding/v1/hls/zUUpEgiM0M18jCGxo2eSZs9 9p49hfyFQr1l4cdze-
-Sp4T-DQOMMoZpkbdyetgfwscfvvUkAdeF-I5 hPI4bGoYg/non_transcode/ap-northeast-1/
-periscope- replay-direct-prod-ap-northeast-1-public/audio- space/
-dynamic_playlist.m3u8?type=live -f URL, --from-master-url URL use the master
-url for the processes(useful for ended spaces) example: https://prod-fastly-ap-
-northeast-1.vi deo.pscp.tv/Transcoding/v1/hls/YRSsw6_P5xUZHMualK5-ihv
-ePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_vpZ2HnFkoRfar4_uJO jqC8OCo5A/non_transcode/
-ap-northeast-1/periscope- replay-direct-prod-ap-northeast-1-public/audio-
-space/master_playlist.m3u8 -M PATH, --input-metadata PATH use a metadata json
-file instead of input url (useful for very old ended spaces) output: -
-o FORMAT_STR, --output FORMAT_STR -m, --write-metadata write the full metadata
-json to a file -p, --write-playlist write the m3u8 used to download the stream
-(e.g. if you want to use another downloader) -u, --url display the master url -
--write-url URL_OUTPUT write master url to file login: --username USERNAME --
-password PASSWORD --output-cookie-file OUTPUT_COOKIE_FILE ``` ## Format You can
-use the following identifiers for the formatting ```python %(title)s %(id)s %
+610dbb2103e5.png)  ## Requirements - `ffmpeg` if not using portable binaries. -
+A logged in user's cookies file exported from Twitter in the [Netscape format]
+(https://curl.se/docs/http-cookies.html). ## Install ### GUI Use this if you're
+not sure. ### From portable binaries [Windows](https://github.com/
+HoloArchivists/twspace-dl/releases/latest/download/twspace-dl-GUI.exe) ### From
+source ```bash pip install git+https://github.com/HoloArchivists/twspace-
+dl@gooey ``` ### CLI ### From portable binaries [Windows](https://github.com/
+HoloArchivists/twspace-dl/releases/latest/download/twspace-dl-CLI.exe) ### From
+PyPI ```bash pip install twspace-dl ``` ### From source ```bash pip install
+git+https://github.com/HoloArchivists/twspace-dl ``` ## Usage ```bash
+twspace_dl -i space_url -c COOKIE_FILE ```  With binaries ### Windows
+```powershell .\twspace_dl.exe -i space_url -c COOKIE_FILE ```  ## Features
+Here's the output of the help option ```txt usage: twspace_dl [-h] [-v] [-s] [-
+k] [-l] -c COOKIE_FILE [-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-
+M PATH] [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT] [-e] Script
+designed to help download twitter spaces options: -h, --help show this help
+message and exit -v, --verbose -s, --skip-download -k, --keep-files -l, --log
+create logfile -c COOKIE_FILE, --input-cookie-file COOKIE_FILE cookies file in
+the Netscape format. The specs of the Netscape cookies format can be found
+here: https://curl.se/docs/http-cookies.html. The cookies file is now required
+due to the Twitter API change that prohibited guest user access to Twitter API
+endpoints on 2023-07-01. input: -i SPACE_URL, --input-url SPACE_URL -
+U USER_URL, --user-url USER_URL -d DYN_URL, --from-dynamic-url DYN_URL use the
+dynamic url for the processes(useful for ended spaces) example: https://prod-
+fastly-ap-northeast- 1.video.pscp.tv/Transcoding/v1/hls/zUUpEgiM0M18jCGxo2e
+SZs99p49hfyFQr1l4cdze-Sp4T- DQOMMoZpkbdyetgfwscfvvUkAdeF- I5hPI4bGoYg/
+non_transcode/ap-northeast-1/periscope- replay-direct-prod-ap-northeast-1-
+public/audio- space/dynamic_playlist.m3u8?type=live -f URL, --from-master-url
+URL use the master url for the processes(useful for ended spaces) example:
+https://prod-fastly-ap-northeast- 1.video.pscp.tv/Transcoding/v1/hls/
+YRSsw6_P5xUZHMualK5 -ihvePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_vpZ2HnFkoRfar4
+_uJOjqC8OCo5A/non_transcode/ap-northeast-1/periscope- replay-direct-prod-ap-
+northeast-1-public/audio- space/master_playlist.m3u8 -M PATH, --input-metadata
+PATH use a metadata json file instead of input url (useful for very old ended
+spaces) output: -o FORMAT_STR, --output FORMAT_STR -m, --write-metadata write
+the full metadata json to a file -p, --write-playlist write the m3u8 used to
+download the stream(e.g. if you want to use another downloader) -u, --url
+display the master url --write-url URL_OUTPUT write master url to file -e, --
+embed-cover embed user avatar as cover art ``` ## Format You can use the
+following identifiers for the formatting ```python %(title)s %(id)s %
 (start_date)s %(creator_name)s %(creator_screen_name)s %(url)s %(creator_id)s
 ``` Example: `[%(creator_screen_name)s]-%(title)s|%(start_date)s` ## Known
 Errors `Changing ID3 metadata in HLS audio elementary stream is not
 implemented....` This is an error in ffmpeg that does not affect twspace_dl at
 all as far as IÂ know. ## Service To run as a systemd service please refer to
 https://github.com/HoloArchivists/twspace-dl/blob/main/SERVICE.md ## Docker ###
-Run once > Use ${pwd} in powershell, or $(pwd) in bash ```bash docker run --rm
--v ${pwd}:/output ryu1845/twspace-dl -i space_url ``` ### Run as monitoring
+Run once > Use `${pwd}` in powershell, or `$(pwd)` in bash ```bash docker run -
+-rm -v ${pwd}:/output ryu1845/twspace-dl -i space_url ``` ### Run as monitoring
 service Using a cookie can help solve some problem with the twitter api.
 However, using one is not necessary. #### Without cookie 1. Download the
 `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named
 `twspace-dl`. 2. Edit `.env` and fill in the Twitter username you want to
 monitor. 3. \[Optional] If you want to used a cookies file, put it into the
 folder and named it `cookies.txt`. 4. `docker-compose up -d`
```

### Comparing `twspace_dl-2023.1.22.1/pyproject.toml` & `twspace_dl-2023.7.24.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "twspace-dl"
-version = "2023.1.22.1"
+version = "2023.7.24.1"
 description = "The only tool to record Twitter spaces (yet)"
 authors = ["Ryu1845 <ryu@tpgjbo.xyz>"]
 readme = "README.md"
 license = "GPL-2.0-only"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "Topic :: Multimedia :: Sound/Audio :: Capture/Recording"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
+mutagen = "^1.46.0"
 
 
 [tool.poetry.scripts]
 twspace_dl = "twspace_dl.__main__:main"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
@@ -29,15 +30,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.bumpver]
-current_version = "2023.1.22.1"
+current_version = "2023.7.24.1"
 version_pattern = "YYYY.MM.DD.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `twspace_dl-2023.1.22.1/twspace_dl/__main__.py` & `twspace_dl-2023.7.24.1/twspace_dl/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Script designed to help download twitter spaces"""
 import argparse
 import datetime
 import json
 import logging
-import os
-import shutil
 import sys
 from types import TracebackType
-from typing import Iterable, Type
+from typing import Optional, Type
 
-from twspace_dl.login import Login, is_expired, load_from_file, write_to_file
-from twspace_dl.twitter import guest_token
+from twspace_dl.api import API
+from twspace_dl.cookies import load_cookies
 from twspace_dl.twspace import Twspace
 from twspace_dl.twspace_dl import TwspaceDL
 
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_ERROR = 1
 EXIT_CODE_MISUSE = 2
 
@@ -34,29 +32,28 @@
     has_input = (
         args.user_url
         or args.input_url
         or args.input_metadata
         or args.from_dynamic_url
         or args.from_master_url
     )
-    has_login = (args.username and args.password) or args.input_cookie_file
     if not has_input:
         print(
             "Either user url, space url, dynamic url or master url should be provided"
         )
         return EXIT_CODE_MISUSE
 
     if args.log:
         log_filename = datetime.datetime.now().strftime(
             ".twspace-dl.%Y-%m-%d_%H-%M-%S_%f.log"
         )
-        handlers = [
+        handlers: Optional[list[logging.Handler]] = [
             logging.FileHandler(log_filename),
             logging.StreamHandler(),
-        ]  # type: Iterable[logging.Handler] | None
+        ]
     else:
         handlers = None
 
     if not args.verbose:
         sys.excepthook = exception_hook
         logging.basicConfig(
             level=logging.INFO,
@@ -66,30 +63,17 @@
     else:
         logging.basicConfig(
             level=logging.DEBUG,
             format="%(asctime)s [%(levelname)s] %(message)s",
             handlers=handlers,
         )
 
-    auth_token = ""
-    if has_login:
-        if args.input_cookie_file:
-            if args.username and args.password and is_expired(args.input_cookie_file):
-                auth_token = Login(args.username, args.password, guest_token()).login()
-                write_to_file(auth_token, args.output_cookie_file)
-            else:
-                auth_token = load_from_file(args.input_cookie_file)
-        else:
-            auth_token = Login(args.username, args.password, guest_token()).login()
-
+    API.init_apis(load_cookies(args.input_cookie_file))
     if args.user_url:
-        if auth_token:
-            twspace = Twspace.from_user_avatar(args.user_url, auth_token)
-        else:
-            twspace = Twspace.from_user_tweets(args.user_url)
+        twspace = Twspace.from_user_avatar(args.user_url)
     elif args.input_metadata:
         twspace = Twspace.from_file(args.input_metadata)
     elif args.input_url:
         twspace = Twspace.from_space_url(args.input_url)
     else:
         logging.warning(
             (
@@ -103,61 +87,63 @@
 
     if args.from_dynamic_url:
         twspace_dl.dyn_url = args.from_dynamic_url
     if args.from_master_url:
         twspace_dl.master_url = args.from_master_url
 
     if args.write_metadata:
-        metadata = json.dumps(twspace.source, indent=4)
-        filename = twspace_dl.filename
-        with open(f"{filename}.json", "w", encoding="utf-8") as metadata_io:
-            metadata_io.write(metadata)
+        with open(f"{twspace_dl.filename}.json", "w", encoding="utf-8") as metadata_io:
+            json.dump(twspace.source, metadata_io, indent=4)
     if args.url:
         print(twspace_dl.master_url)
     if args.write_url:
         with open(args.write_url, "a", encoding="utf-8") as url_output:
-            url_output.write("{}\n".format(twspace_dl.master_url))
+            url_output.write(f"{twspace_dl.master_url}\n")
     if args.write_playlist:
         twspace_dl.write_playlist()
 
     if not args.skip_download:
         try:
             twspace_dl.download()
+            if args.embed_cover:
+                twspace_dl.embed_cover()
         except KeyboardInterrupt:
             logging.info("Download Interrupted by user")
         finally:
-            if not args.keep_files and os.path.exists(twspace_dl.tempdir):
-                shutil.rmtree(twspace_dl.tempdir)
+            if not args.keep_files:
+                twspace_dl.cleanup()
     return EXIT_CODE_SUCCESS
 
 
 def main() -> int:
     """Main function, creates the argument parser"""
     parser = argparse.ArgumentParser(
         description="Script designed to help download twitter spaces"
     )
 
     input_group = parser.add_argument_group("input")
     input_method = input_group.add_mutually_exclusive_group()
     output_group = parser.add_argument_group("output")
-    login_group = parser.add_argument_group("login")
 
     parser.add_argument("-v", "--verbose", action="store_true")
     parser.add_argument("-s", "--skip-download", action="store_true")
     parser.add_argument("-k", "--keep-files", action="store_true")
     parser.add_argument("-l", "--log", action="store_true", help="create logfile")
-    parser.add_argument("--input-cookie-file", type=str, metavar="COOKIE_FILE")
-
-    login_group.add_argument("--username", type=str, metavar="USERNAME", default=None)
-    login_group.add_argument("--password", type=str, metavar="PASSWORD", default=None)
-    login_group.add_argument(
-        "--output-cookie-file",
+    parser.add_argument(
+        "-c",
+        "--input-cookie-file",
         type=str,
-        metavar="OUTPUT_COOKIE_FILE",
-        default=None,
+        metavar="COOKIE_FILE",
+        help=(
+            "cookies file in the Netscape format. The specs of the Netscape cookies format "
+            "can be found here: https://curl.se/docs/http-cookies.html. The cookies file is "
+            "now required due to the Twitter API change that prohibited guest user access to "
+            "Twitter API endpoints on 2023-07-01."
+        ),
+        required=True,
     )
 
     input_method.add_argument("-i", "--input-url", type=str, metavar="SPACE_URL")
     input_method.add_argument("-U", "--user-url", type=str, metavar="USER_URL")
     input_group.add_argument(
         "-d",
         "--from-dynamic-url",
@@ -220,14 +206,20 @@
     )
     output_group.add_argument(
         "-u", "--url", action="store_true", help="display the master url"
     )
     output_group.add_argument(
         "--write-url", type=str, metavar="URL_OUTPUT", help="write master url to file"
     )
+    output_group.add_argument(
+        "-e",
+        "--embed-cover",
+        action="store_true",
+        help="embed user avatar as cover art",
+    )
     parser.set_defaults(func=space)
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         return EXIT_CODE_ERROR
     args = parser.parse_args()
     args.func(args)
     return EXIT_CODE_SUCCESS
```

### Comparing `twspace_dl-2023.1.22.1/twspace_dl/twspace_dl.py` & `twspace_dl-2023.7.24.1/twspace_dl/twspace_dl.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 import re
 import shutil
 import subprocess
 import tempfile
 from functools import cached_property
 from urllib.parse import urlparse
 
-import requests
-from requests.adapters import HTTPAdapter, Retry
+from mutagen.mp4 import MP4, MP4Cover
 
+from .api import API
 from .twspace import Twspace
 
 DEFAULT_FNAME_FORMAT = "(%(creator_name)s)%(title)s-%(id)s"
+MP4_COVER_FORMAT_MAP = {"jpg": MP4Cover.FORMAT_JPEG, "png": MP4Cover.FORMAT_PNG}
 
 
 class TwspaceDL:
     """Downloader class for twitter spaces"""
 
     def __init__(self, space: Twspace, format_str: str) -> None:
         self.space = space
         self.format_str = format_str or DEFAULT_FNAME_FORMAT
-        self.session = requests.Session()
-        self.session.mount(
-            "https://", HTTPAdapter(max_retries=(Retry(total=5, backoff_factor=0.1)))
-        )
-        self._tempdir = tempfile.mkdtemp(dir=".")
+        self._tempdir = ""
 
     @cached_property
     def filename(self) -> str:
         """Returns the formatted filename"""
         filename = self.space.format(self.format_str)
         return filename
 
@@ -41,30 +38,17 @@
             logging.error(
                 (
                     "Can't Download. Space has ended, can't retrieve master url. "
                     "You can provide it with -f URL if you have it."
                 )
             )
             raise ValueError("Space Ended")
-        headers = {
-            "authorization": (
-                "Bearer "
-                "AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs"
-                "=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA"
-            ),
-            "cookie": "auth_token=",
-        }
         media_key = space["media_key"]
-        response = self.session.get(
-            "https://twitter.com/i/api/1.1/live_video_stream/status/" + media_key,
-            headers=headers,
-            timeout=30,
-        )
         try:
-            metadata = response.json()
+            metadata = API.live_video_stream_api.status(media_key)
         except Exception as err:
             raise RuntimeError("Space isn't available", space.source) from err
         dyn_url = metadata["source"]["location"]
         return dyn_url
 
     @cached_property
     def master_url(self) -> str:
@@ -73,46 +57,42 @@
             r"(?<=/audio-space/).*", "master_playlist.m3u8", self.dyn_url
         )
         return master_url
 
     @property
     def playlist_url(self) -> str:
         """Get the URL containing the chunks filenames"""
-        response = requests.get(self.master_url, timeout=30)
+        response = API.client.get(self.master_url)
         playlist_suffix = response.text.splitlines()[3]
         domain = urlparse(self.master_url).netloc
         playlist_url = f"https://{domain}{playlist_suffix}"
         return playlist_url
 
     @property
     def playlist_text(self) -> str:
         """Modify the chunks URL using the master one to be able to download"""
-        playlist_text = requests.get(self.playlist_url, timeout=30).text
+        playlist_text = API.client.get(self.playlist_url).text
         master_url_wo_file = re.sub(r"master_playlist\.m3u8.*", "", self.master_url)
         playlist_text = re.sub(r"(?=chunk)", master_url_wo_file, playlist_text)
         return playlist_text
 
     def write_playlist(self, save_dir: str = "./") -> None:
         """Write the modified playlist for external use"""
         filename = os.path.basename(self.filename) + ".m3u8"
         path = os.path.join(save_dir, filename)
         with open(path, "w", encoding="utf-8") as stream_io:
             stream_io.write(self.playlist_text)
         logging.debug("%(path)s written to disk", dict(path=path))
 
-    @property
-    def tempdir(self):
-        """Return tempdir"""
-        return self._tempdir
-
     def download(self) -> None:
         """Download a twitter space"""
         if not shutil.which("ffmpeg"):
             raise FileNotFoundError("ffmpeg not installed")
         space = self.space
+        self._tempdir = tempfile.mkdtemp(dir=".")
         self.write_playlist(save_dir=self._tempdir)
         state = space["state"]
 
         cmd_base = [
             "ffmpeg",
             "-y",
             "-stats",
@@ -130,15 +110,15 @@
         ]
 
         filename = os.path.basename(self.filename)
         filename_m3u8 = os.path.join(self._tempdir, filename + ".m3u8")
         filename_old = os.path.join(self._tempdir, filename + ".m4a")
         cmd_old = cmd_base.copy()
         cmd_old.insert(1, "-protocol_whitelist")
-        cmd_old.insert(2, "file,https,tls,tcp")
+        cmd_old.insert(2, "file,https,httpproxy,tls,tcp")
         cmd_old.insert(8, filename_m3u8)
         cmd_old.append(filename_old)
         logging.debug("Command for the old part: %s", " ".join(cmd_old))
 
         if state == "Running":
             filename_new = os.path.join(self._tempdir, filename + "_new.m4a")
             cmd_new = cmd_base.copy()
@@ -180,7 +160,29 @@
                     + "\nThis might be a temporary error, retry in a few minutes"
                 ) from err
             if os.path.dirname(self.filename):
                 os.makedirs(os.path.dirname(self.filename), exist_ok=True)
             shutil.move(filename_old, self.filename + ".m4a")
 
         logging.info("Finished downloading")
+
+    def embed_cover(self) -> None:
+        """Embed the user profile image as the cover art"""
+        cover_url = self.space["creator_profile_image_url"]
+        cover_ext = cover_url.split(".")[-1]
+        try:
+            response = API.client.get(cover_url)
+            if cover_format := MP4_COVER_FORMAT_MAP.get(cover_ext):
+                meta = MP4(f"{self.filename}.m4a")
+                meta.tags["covr"] = [
+                    MP4Cover(response.content, imageformat=cover_format)
+                ]
+                meta.save()
+            else:
+                logging.error(f"Unsupported user profile image format: {cover_ext}")
+        except RuntimeError:
+            logging.error(f"Cannot download user profile image from URL: {cover_url}")
+            raise
+
+    def cleanup(self) -> None:
+        if os.path.exists(self._tempdir):
+            shutil.rmtree(self._tempdir)
```

### Comparing `twspace_dl-2023.1.22.1/setup.py` & `twspace_dl-2023.7.24.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,224 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: twspace-dl
+Version: 2023.7.24.1
+Summary: The only tool to record Twitter spaces (yet)
+License: GPL-2.0-only
+Author: Ryu1845
+Author-email: ryu@tpgjbo.xyz
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
+Requires-Dist: mutagen (>=1.46.0,<2.0.0)
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['twspace_dl']
+<!-- markdownlint-disable MD033 MD041 -->
 
-package_data = \
-{'': ['*']}
+<div align="center">
+  <h1 id="twspace-dl">Twspace-dl</h1>
+  <p>
+    <a href="https://pypi.org/project/twspace-dl/">
+      <img src="https://img.shields.io/pypi/v/twspace-dl?style=for-the-badge" alt="PyPI">
+    </a>
+    <a href="https://pypi.org/project/twspace-dl/">
+      <img src="https://img.shields.io/pypi/dm/twspace-dl?label=DOWNLOADS%20%28PYPI%29&amp;style=for-the-badge" alt="PyPI DLs">
+    </a>
+    <a href="https://github.com/HoloArchivists/twspace-dl/releases">
+      <img src="https://img.shields.io/github/downloads/HoloArchivists/twspace-dl/total?label=DOWNLOADS%20%28GITHUB%29&amp;style=for-the-badge" alt="Github Releases DLs">
+    </a>
+  </p>
+  <p>A python module to download twitter spaces.</p>
+</div>
 
-install_requires = \
-['requests>=2.26.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['twspace_dl = twspace_dl.__main__:main']}
-
-setup_kwargs = {
-    'name': 'twspace-dl',
-    'version': '2023.1.22.1',
-    'description': 'The only tool to record Twitter spaces (yet)',
-    'long_description': '<!-- markdownlint-disable MD033 MD041 -->\n\n<div align="center">\n  <h1 id="twspace-dl">Twspace-dl</h1>\n  <p>\n    <a href="https://pypi.org/project/twspace-dl/">\n      <img src="https://img.shields.io/pypi/v/twspace-dl?style=for-the-badge" alt="PyPI">\n    </a>\n    <a href="https://pypi.org/project/twspace-dl/">\n      <img src="https://img.shields.io/pypi/dm/twspace-dl?label=DOWNLOADS%20%28PYPI%29&amp;style=for-the-badge" alt="PyPI DLs">\n    </a>\n    <a href="https://github.com/HoloArchivists/twspace-dl/releases">\n      <img src="https://img.shields.io/github/downloads/HoloArchivists/twspace-dl/total?label=DOWNLOADS%20%28GITHUB%29&amp;style=for-the-badge" alt="Github Releases DLs">\n    </a>\n  </p>\n  <p>A python module to download twitter spaces.</p>\n</div>\n\n## Screensots\n\n<details>\n<summary>GUI</summary>\n\n![general tab](https://user-images.githubusercontent.com/77058942/172580094-3663f86d-3ee2-48d0-9313-f4ed71f048aa.png)\n![input tab](https://user-images.githubusercontent.com/77058942/172580476-bb34dce0-08b0-41f6-852b-b68d32532add.png)\n![running tab](https://user-images.githubusercontent.com/77058942/172580589-fd6b05bd-f081-4c7a-ab05-0640abda00ce.png)\n![success pop up](https://user-images.githubusercontent.com/77058942/172580861-18b3ac9f-88d2-44cf-8b5d-135990a78f77.png)\n\n</details>\n\n<details>\n<summary>CLI</summary>\n\n![help](https://user-images.githubusercontent.com/77058942/172581224-9b465f78-4894-456f-9b85-5b76ee9bbfca.png)\n![running](https://user-images.githubusercontent.com/77058942/172581500-174834c5-6883-44f9-a0a7-610dbb2103e5.png)\n\n</details>\n\n\n## Requirements\n\nffmpeg if not using portable binaries\n\n## Install\n\n### GUI\n\nUse this if you\'re not sure.\n\n### From portable binaries\n\n[Windows](https://github.com/HoloArchivists/twspace-dl/releases/latest/download/twspace-dl-GUI.exe)\n\n### From source\n\n```bash\npip install git+https://github.com/HoloArchivists/twspace-dl@gooey\n```\n\n### CLI\n\n### From portable binaries\n\n[Windows](https://github.com/HoloArchivists/twspace-dl/releases/latest/download/twspace-dl-CLI.exe)\n\n### From PyPI\n\n```bash\npip install twspace-dl\n```\n\n### From source\n\n```bash\npip install git+https://github.com/HoloArchivists/twspace-dl\n```\n\n## Usage\n\n```bash\ntwspace_dl -i space_url\n```\n\n<details>\n<summary>With binaries</summary>\n\n### Windows\n\n```bash\n.\\twspace_dl.exe -i space_url\n```\n\n</details>\n\n## Features\n\nHere\'s the output of the help option\n\n```txt\nusage: twspace_dl [-h] [-v] [-s] [-k] [-l] [--input-cookie-file COOKIE_FILE]\n                  [--username USERNAME] [--password PASSWORD]\n                  [--output-cookie-file OUTPUT_COOKIE_FILE]\n                  [-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-M PATH]\n                  [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT]\n\nScript designed to help download twitter spaces\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -v, --verbose\n  -s, --skip-download\n  -k, --keep-files\n  -l, --log             create logfile\n  --input-cookie-file COOKIE_FILE\n\ninput:\n  -i SPACE_URL, --input-url SPACE_URL\n  -U USER_URL, --user-url USER_URL\n  -d DYN_URL, --from-dynamic-url DYN_URL\n                        use the dynamic url for the processes(useful for ended\n                        spaces) example: https://prod-fastly-ap-northeast-1.vi\n                        deo.pscp.tv/Transcoding/v1/hls/zUUpEgiM0M18jCGxo2eSZs9\n                        9p49hfyFQr1l4cdze-Sp4T-DQOMMoZpkbdyetgfwscfvvUkAdeF-I5\n                        hPI4bGoYg/non_transcode/ap-northeast-1/periscope-\n                        replay-direct-prod-ap-northeast-1-public/audio-\n                        space/dynamic_playlist.m3u8?type=live\n  -f URL, --from-master-url URL\n                        use the master url for the processes(useful for ended\n                        spaces) example: https://prod-fastly-ap-northeast-1.vi\n                        deo.pscp.tv/Transcoding/v1/hls/YRSsw6_P5xUZHMualK5-ihv\n                        ePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_vpZ2HnFkoRfar4_uJO\n                        jqC8OCo5A/non_transcode/ap-northeast-1/periscope-\n                        replay-direct-prod-ap-northeast-1-public/audio-\n                        space/master_playlist.m3u8\n  -M PATH, --input-metadata PATH\n                        use a metadata json file instead of input url (useful\n                        for very old ended spaces)\n\noutput:\n  -o FORMAT_STR, --output FORMAT_STR\n  -m, --write-metadata  write the full metadata json to a file\n  -p, --write-playlist  write the m3u8 used to download the stream(e.g. if you\n                        want to use another downloader)\n  -u, --url             display the master url\n  --write-url URL_OUTPUT\n                        write master url to file\n\nlogin:\n  --username USERNAME\n  --password PASSWORD\n  --output-cookie-file OUTPUT_COOKIE_FILE\n```\n\n## Format\n\nYou can use the following identifiers for the formatting\n\n```python\n%(title)s\n%(id)s\n%(start_date)s\n%(creator_name)s\n%(creator_screen_name)s\n%(url)s\n%(creator_id)s\n```\n\nExample: `[%(creator_screen_name)s]-%(title)s|%(start_date)s`\n\n## Known Errors\n\n`Changing ID3 metadata in HLS audio elementary stream is not implemented....`\n\nThis is an error in ffmpeg that does not affect twspace_dl at all as far as I\xa0know.\n\n## Service \n\nTo run as a systemd service please refer to https://github.com/HoloArchivists/twspace-dl/blob/main/SERVICE.md\n\n## Docker\n\n### Run once\n\n> Use ${pwd} in powershell, or $(pwd) in bash\n\n```bash\ndocker run --rm -v ${pwd}:/output ryu1845/twspace-dl -i space_url\n```\n\n### Run as monitoring service\n\nUsing a cookie can help solve some problem with the twitter api. However, using one is not necessary.\n\n#### Without cookie\n\n1. Download the `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named `twspace-dl`.\n2. Edit `.env` and fill in the Twitter username you want to monitor.\n3. \\[Optional] If you want to used a cookies file, put it into the folder and named it `cookies.txt`.\n4. `docker-compose up -d`\n',
-    'author': 'Ryu1845',
-    'author_email': 'ryu@tpgjbo.xyz',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Screensots
 
+<details>
+<summary>GUI</summary>
+
+![general tab](https://user-images.githubusercontent.com/77058942/172580094-3663f86d-3ee2-48d0-9313-f4ed71f048aa.png)
+![input tab](https://user-images.githubusercontent.com/77058942/172580476-bb34dce0-08b0-41f6-852b-b68d32532add.png)
+![running tab](https://user-images.githubusercontent.com/77058942/172580589-fd6b05bd-f081-4c7a-ab05-0640abda00ce.png)
+![success pop up](https://user-images.githubusercontent.com/77058942/172580861-18b3ac9f-88d2-44cf-8b5d-135990a78f77.png)
+
+</details>
+
+<details>
+<summary>CLI</summary>
+
+![help](https://user-images.githubusercontent.com/77058942/172581224-9b465f78-4894-456f-9b85-5b76ee9bbfca.png)
+![running](https://user-images.githubusercontent.com/77058942/172581500-174834c5-6883-44f9-a0a7-610dbb2103e5.png)
+
+</details>
+
+
+## Requirements
+
+- `ffmpeg` if not using portable binaries.
+- A logged in user's cookies file exported from Twitter in the [Netscape format](https://curl.se/docs/http-cookies.html).
+
+## Install
+
+### GUI
+
+Use this if you're not sure.
+
+### From portable binaries
+
+[Windows](https://github.com/HoloArchivists/twspace-dl/releases/latest/download/twspace-dl-GUI.exe)
+
+### From source
+
+```bash
+pip install git+https://github.com/HoloArchivists/twspace-dl@gooey
+```
+
+### CLI
+
+### From portable binaries
+
+[Windows](https://github.com/HoloArchivists/twspace-dl/releases/latest/download/twspace-dl-CLI.exe)
+
+### From PyPI
+
+```bash
+pip install twspace-dl
+```
+
+### From source
+
+```bash
+pip install git+https://github.com/HoloArchivists/twspace-dl
+```
+
+## Usage
+
+```bash
+twspace_dl -i space_url -c COOKIE_FILE
+```
+
+<details>
+<summary>With binaries</summary>
+
+### Windows
+
+```powershell
+.\twspace_dl.exe -i space_url -c COOKIE_FILE
+```
+
+</details>
+
+## Features
+
+Here's the output of the help option
+
+```txt
+usage: twspace_dl [-h] [-v] [-s] [-k] [-l] -c COOKIE_FILE
+                  [-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-M PATH]
+                  [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT] [-e]
+
+Script designed to help download twitter spaces
+
+options:
+  -h, --help            show this help message and exit
+  -v, --verbose
+  -s, --skip-download
+  -k, --keep-files
+  -l, --log             create logfile
+  -c COOKIE_FILE, --input-cookie-file COOKIE_FILE
+                        cookies file in the Netscape format. The specs of the
+                        Netscape cookies format can be found here:
+                        https://curl.se/docs/http-cookies.html. The cookies
+                        file is now required due to the Twitter API change
+                        that prohibited guest user access to Twitter API
+                        endpoints on 2023-07-01.
+
+input:
+  -i SPACE_URL, --input-url SPACE_URL
+  -U USER_URL, --user-url USER_URL
+  -d DYN_URL, --from-dynamic-url DYN_URL
+                        use the dynamic url for the processes(useful for ended
+                        spaces) example: https://prod-fastly-ap-northeast-
+                        1.video.pscp.tv/Transcoding/v1/hls/zUUpEgiM0M18jCGxo2e
+                        SZs99p49hfyFQr1l4cdze-Sp4T-
+                        DQOMMoZpkbdyetgfwscfvvUkAdeF-
+                        I5hPI4bGoYg/non_transcode/ap-northeast-1/periscope-
+                        replay-direct-prod-ap-northeast-1-public/audio-
+                        space/dynamic_playlist.m3u8?type=live
+  -f URL, --from-master-url URL
+                        use the master url for the processes(useful for ended
+                        spaces) example: https://prod-fastly-ap-northeast-
+                        1.video.pscp.tv/Transcoding/v1/hls/YRSsw6_P5xUZHMualK5
+                        -ihvePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_vpZ2HnFkoRfar4
+                        _uJOjqC8OCo5A/non_transcode/ap-northeast-1/periscope-
+                        replay-direct-prod-ap-northeast-1-public/audio-
+                        space/master_playlist.m3u8
+  -M PATH, --input-metadata PATH
+                        use a metadata json file instead of input url (useful
+                        for very old ended spaces)
+
+output:
+  -o FORMAT_STR, --output FORMAT_STR
+  -m, --write-metadata  write the full metadata json to a file
+  -p, --write-playlist  write the m3u8 used to download the stream(e.g. if you
+                        want to use another downloader)
+  -u, --url             display the master url
+  --write-url URL_OUTPUT
+                        write master url to file
+  -e, --embed-cover     embed user avatar as cover art
+```
+
+## Format
+
+You can use the following identifiers for the formatting
+
+```python
+%(title)s
+%(id)s
+%(start_date)s
+%(creator_name)s
+%(creator_screen_name)s
+%(url)s
+%(creator_id)s
+```
+
+Example: `[%(creator_screen_name)s]-%(title)s|%(start_date)s`
+
+## Known Errors
+
+`Changing ID3 metadata in HLS audio elementary stream is not implemented....`
+
+This is an error in ffmpeg that does not affect twspace_dl at all as far as I know.
+
+## Service
+
+To run as a systemd service please refer to https://github.com/HoloArchivists/twspace-dl/blob/main/SERVICE.md
+
+## Docker
+
+### Run once
+
+> Use `${pwd}` in powershell, or `$(pwd)` in bash
+
+```bash
+docker run --rm -v ${pwd}:/output ryu1845/twspace-dl -i space_url
+```
+
+### Run as monitoring service
+
+Using a cookie can help solve some problem with the twitter api. However, using one is not necessary.
+
+#### Without cookie
+
+1. Download the `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named `twspace-dl`.
+2. Edit `.env` and fill in the Twitter username you want to monitor.
+3. \[Optional] If you want to used a cookies file, put it into the folder and named it `cookies.txt`.
+4. `docker-compose up -d`
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,83 +1,79 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['twspace_dl'] package_data = \ {'': ['*']} install_requires = \
-['requests>=2.26.0,<3.0.0'] entry_points = \ {'console_scripts': ['twspace_dl =
-twspace_dl.__main__:main']} setup_kwargs = { 'name': 'twspace-dl', 'version':
-'2023.1.22.1', 'description': 'The only tool to record Twitter spaces (yet)',
-'long_description': '\n\n
-                                      \n
+Metadata-Version: 2.1 Name: twspace-dl Version: 2023.7.24.1 Summary: The only
+tool to record Twitter spaces (yet) License: GPL-2.0-only Author: Ryu1845
+Author-email: ryu@tpgjbo.xyz Requires-Python: >=3.8,<4.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
+Approved :: GNU General Public License v2 (GPLv2) Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording Requires-
+Dist: mutagen (>=1.46.0,<2.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0)
+Description-Content-Type: text/markdown
                            ****** Twspace-dl ******
-                                      \n
-        \n \n_[PyPI]\n\n \n_[PyPI_DLs]\n\n \n_[Github_Releases_DLs]\n\n
-                                      \n
+                    [PyPI] [PyPI_DLs] [Github_Releases_DLs]
                   A python module to download twitter spaces.
-                                      \n
-\n\n## Screensots\n\n\nGUI\n\n![general tab](https://user-
-images.githubusercontent.com/77058942/172580094-3663f86d-3ee2-48d0-9313-
-f4ed71f048aa.png)\n![input tab](https://user-images.githubusercontent.com/
-77058942/172580476-bb34dce0-08b0-41f6-852b-b68d32532add.png)\n![running tab]
-(https://user-images.githubusercontent.com/77058942/172580589-fd6b05bd-f081-
-4c7a-ab05-0640abda00ce.png)\n![success pop up](https://user-
-images.githubusercontent.com/77058942/172580861-18b3ac9f-88d2-44cf-8b5d-
-135990a78f77.png)\n\n\n\n\nCLI\n\n![help](https://user-
-images.githubusercontent.com/77058942/172581224-9b465f78-4894-456f-9b85-
-5b76ee9bbfca.png)\n![running](https://user-images.githubusercontent.com/
-77058942/172581500-174834c5-6883-44f9-a0a7-610dbb2103e5.png)\n\n\n\n\n##
-Requirements\n\nffmpeg if not using portable binaries\n\n## Install\n\n###
-GUI\n\nUse this if you\'re not sure.\n\n### From portable binaries\n\n[Windows]
-(https://github.com/HoloArchivists/twspace-dl/releases/latest/download/twspace-
-dl-GUI.exe)\n\n### From source\n\n```bash\npip install git+https://github.com/
-HoloArchivists/twspace-dl@gooey\n```\n\n### CLI\n\n### From portable
-binaries\n\n[Windows](https://github.com/HoloArchivists/twspace-dl/releases/
-latest/download/twspace-dl-CLI.exe)\n\n### From PyPI\n\n```bash\npip install
-twspace-dl\n```\n\n### From source\n\n```bash\npip install git+https://
-github.com/HoloArchivists/twspace-dl\n```\n\n## Usage\n\n```bash\ntwspace_dl -
-i space_url\n```\n\n\nWith binaries\n\n###
-Windows\n\n```bash\n.\\twspace_dl.exe -i space_url\n```\n\n\n\n##
-Features\n\nHere\'s the output of the help option\n\n```txt\nusage: twspace_dl
-[-h] [-v] [-s] [-k] [-l] [--input-cookie-file COOKIE_FILE]\n [--username
-USERNAME] [--password PASSWORD]\n [--output-cookie-file OUTPUT_COOKIE_FILE]\n
-[-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-M PATH]\n [-o FORMAT_STR]
-[-m] [-p] [-u] [--write-url URL_OUTPUT]\n\nScript designed to help download
-twitter spaces\n\noptional arguments:\n -h, --help show this help message and
-exit\n -v, --verbose\n -s, --skip-download\n -k, --keep-files\n -l, --log
-create logfile\n --input-cookie-file COOKIE_FILE\n\ninput:\n -i SPACE_URL, --
-input-url SPACE_URL\n -U USER_URL, --user-url USER_URL\n -d DYN_URL, --from-
-dynamic-url DYN_URL\n use the dynamic url for the processes(useful for ended\n
-spaces) example: https://prod-fastly-ap-northeast-1.vi\n deo.pscp.tv/
-Transcoding/v1/hls/zUUpEgiM0M18jCGxo2eSZs9\n 9p49hfyFQr1l4cdze-Sp4T-
-DQOMMoZpkbdyetgfwscfvvUkAdeF-I5\n hPI4bGoYg/non_transcode/ap-northeast-1/
-periscope-\n replay-direct-prod-ap-northeast-1-public/audio-\n space/
-dynamic_playlist.m3u8?type=live\n -f URL, --from-master-url URL\n use the
-master url for the processes(useful for ended\n spaces) example: https://prod-
-fastly-ap-northeast-1.vi\n deo.pscp.tv/Transcoding/v1/hls/YRSsw6_P5xUZHMualK5-
-ihv\n ePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_vpZ2HnFkoRfar4_uJO\n jqC8OCo5A/
-non_transcode/ap-northeast-1/periscope-\n replay-direct-prod-ap-northeast-1-
-public/audio-\n space/master_playlist.m3u8\n -M PATH, --input-metadata PATH\n
-use a metadata json file instead of input url (useful\n for very old ended
-spaces)\n\noutput:\n -o FORMAT_STR, --output FORMAT_STR\n -m, --write-metadata
-write the full metadata json to a file\n -p, --write-playlist write the m3u8
-used to download the stream(e.g. if you\n want to use another downloader)\n -u,
---url display the master url\n --write-url URL_OUTPUT\n write master url to
-file\n\nlogin:\n --username USERNAME\n --password PASSWORD\n --output-cookie-
-file OUTPUT_COOKIE_FILE\n```\n\n## Format\n\nYou can use the following
-identifiers for the formatting\n\n```python\n%(title)s\n%(id)s\n%
-(start_date)s\n%(creator_name)s\n%(creator_screen_name)s\n%(url)s\n%
-(creator_id)s\n```\n\nExample: `[%(creator_screen_name)s]-%(title)s|%
-(start_date)s`\n\n## Known Errors\n\n`Changing ID3 metadata in HLS audio
-elementary stream is not implemented....`\n\nThis is an error in ffmpeg that
-does not affect twspace_dl at all as far as I\xa0know.\n\n## Service \n\nTo run
-as a systemd service please refer to https://github.com/HoloArchivists/twspace-
-dl/blob/main/SERVICE.md\n\n## Docker\n\n### Run once\n\n> Use ${pwd} in
-powershell, or $(pwd) in bash\n\n```bash\ndocker run --rm -v ${pwd}:/output
-ryu1845/twspace-dl -i space_url\n```\n\n### Run as monitoring service\n\nUsing
-a cookie can help solve some problem with the twitter api. However, using one
-is not necessary.\n\n#### Without cookie\n\n1. Download the `docker-
-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named
-`twspace-dl`.\n2. Edit `.env` and fill in the Twitter username you want to
-monitor.\n3. \\[Optional] If you want to used a cookies file, put it into the
-folder and named it `cookies.txt`.\n4. `docker-compose up -d`\n', 'author':
-'Ryu1845', 'author_email': 'ryu@tpgjbo.xyz', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+## Screensots  GUI ![general tab](https://user-images.githubusercontent.com/
+77058942/172580094-3663f86d-3ee2-48d0-9313-f4ed71f048aa.png) ![input tab]
+(https://user-images.githubusercontent.com/77058942/172580476-bb34dce0-08b0-
+41f6-852b-b68d32532add.png) ![running tab](https://user-
+images.githubusercontent.com/77058942/172580589-fd6b05bd-f081-4c7a-ab05-
+0640abda00ce.png) ![success pop up](https://user-images.githubusercontent.com/
+77058942/172580861-18b3ac9f-88d2-44cf-8b5d-135990a78f77.png)   CLI ![help]
+(https://user-images.githubusercontent.com/77058942/172581224-9b465f78-4894-
+456f-9b85-5b76ee9bbfca.png) ![running](https://user-
+images.githubusercontent.com/77058942/172581500-174834c5-6883-44f9-a0a7-
+610dbb2103e5.png)  ## Requirements - `ffmpeg` if not using portable binaries. -
+A logged in user's cookies file exported from Twitter in the [Netscape format]
+(https://curl.se/docs/http-cookies.html). ## Install ### GUI Use this if you're
+not sure. ### From portable binaries [Windows](https://github.com/
+HoloArchivists/twspace-dl/releases/latest/download/twspace-dl-GUI.exe) ### From
+source ```bash pip install git+https://github.com/HoloArchivists/twspace-
+dl@gooey ``` ### CLI ### From portable binaries [Windows](https://github.com/
+HoloArchivists/twspace-dl/releases/latest/download/twspace-dl-CLI.exe) ### From
+PyPI ```bash pip install twspace-dl ``` ### From source ```bash pip install
+git+https://github.com/HoloArchivists/twspace-dl ``` ## Usage ```bash
+twspace_dl -i space_url -c COOKIE_FILE ```  With binaries ### Windows
+```powershell .\twspace_dl.exe -i space_url -c COOKIE_FILE ```  ## Features
+Here's the output of the help option ```txt usage: twspace_dl [-h] [-v] [-s] [-
+k] [-l] -c COOKIE_FILE [-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-
+M PATH] [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT] [-e] Script
+designed to help download twitter spaces options: -h, --help show this help
+message and exit -v, --verbose -s, --skip-download -k, --keep-files -l, --log
+create logfile -c COOKIE_FILE, --input-cookie-file COOKIE_FILE cookies file in
+the Netscape format. The specs of the Netscape cookies format can be found
+here: https://curl.se/docs/http-cookies.html. The cookies file is now required
+due to the Twitter API change that prohibited guest user access to Twitter API
+endpoints on 2023-07-01. input: -i SPACE_URL, --input-url SPACE_URL -
+U USER_URL, --user-url USER_URL -d DYN_URL, --from-dynamic-url DYN_URL use the
+dynamic url for the processes(useful for ended spaces) example: https://prod-
+fastly-ap-northeast- 1.video.pscp.tv/Transcoding/v1/hls/zUUpEgiM0M18jCGxo2e
+SZs99p49hfyFQr1l4cdze-Sp4T- DQOMMoZpkbdyetgfwscfvvUkAdeF- I5hPI4bGoYg/
+non_transcode/ap-northeast-1/periscope- replay-direct-prod-ap-northeast-1-
+public/audio- space/dynamic_playlist.m3u8?type=live -f URL, --from-master-url
+URL use the master url for the processes(useful for ended spaces) example:
+https://prod-fastly-ap-northeast- 1.video.pscp.tv/Transcoding/v1/hls/
+YRSsw6_P5xUZHMualK5 -ihvePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_vpZ2HnFkoRfar4
+_uJOjqC8OCo5A/non_transcode/ap-northeast-1/periscope- replay-direct-prod-ap-
+northeast-1-public/audio- space/master_playlist.m3u8 -M PATH, --input-metadata
+PATH use a metadata json file instead of input url (useful for very old ended
+spaces) output: -o FORMAT_STR, --output FORMAT_STR -m, --write-metadata write
+the full metadata json to a file -p, --write-playlist write the m3u8 used to
+download the stream(e.g. if you want to use another downloader) -u, --url
+display the master url --write-url URL_OUTPUT write master url to file -e, --
+embed-cover embed user avatar as cover art ``` ## Format You can use the
+following identifiers for the formatting ```python %(title)s %(id)s %
+(start_date)s %(creator_name)s %(creator_screen_name)s %(url)s %(creator_id)s
+``` Example: `[%(creator_screen_name)s]-%(title)s|%(start_date)s` ## Known
+Errors `Changing ID3 metadata in HLS audio elementary stream is not
+implemented....` This is an error in ffmpeg that does not affect twspace_dl at
+all as far as IÂ know. ## Service To run as a systemd service please refer to
+https://github.com/HoloArchivists/twspace-dl/blob/main/SERVICE.md ## Docker ###
+Run once > Use `${pwd}` in powershell, or `$(pwd)` in bash ```bash docker run -
+-rm -v ${pwd}:/output ryu1845/twspace-dl -i space_url ``` ### Run as monitoring
+service Using a cookie can help solve some problem with the twitter api.
+However, using one is not necessary. #### Without cookie 1. Download the
+`docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named
+`twspace-dl`. 2. Edit `.env` and fill in the Twitter username you want to
+monitor. 3. \[Optional] If you want to used a cookies file, put it into the
+folder and named it `cookies.txt`. 4. `docker-compose up -d`
```

