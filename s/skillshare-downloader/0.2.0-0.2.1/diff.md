# Comparing `tmp/skillshare_downloader-0.2.0.tar.gz` & `tmp/skillshare_downloader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillshare_downloader-0.2.0.tar", max compression
+gzip compressed data, was "skillshare_downloader-0.2.1.tar", max compression
```

## Comparing `skillshare_downloader-0.2.0.tar` & `skillshare_downloader-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-07-21 06:55:00.000000 skillshare_downloader-0.2.0/LICENSE
--rw-r--r--   0        0        0     3240 2023-07-22 06:03:14.000000 skillshare_downloader-0.2.0/README.md
--rw-r--r--   0        0        0      637 2023-07-22 06:03:20.000000 skillshare_downloader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-22 02:39:12.000000 skillshare_downloader-0.2.0/skillshare_downloader/__init__.py
--rw-r--r--   0        0        0       62 2023-07-22 04:58:55.000000 skillshare_downloader-0.2.0/skillshare_downloader/__main__.py
--rw-r--r--   0        0        0     5977 2023-07-22 05:43:37.000000 skillshare_downloader-0.2.0/skillshare_downloader/main.py
--rw-r--r--   0        0        0     2529 2023-07-19 05:02:18.000000 skillshare_downloader-0.2.0/skillshare_downloader/progress.py
--rw-r--r--   0        0        0    16275 2023-07-22 05:36:41.000000 skillshare_downloader-0.2.0/skillshare_downloader/skillshare.py
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 skillshare_downloader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-21 06:55:00.000000 skillshare_downloader-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3240 2023-07-22 06:03:14.000000 skillshare_downloader-0.2.1/README.md
+-rw-r--r--   0        0        0      637 2023-07-23 07:01:43.000000 skillshare_downloader-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 02:39:12.000000 skillshare_downloader-0.2.1/skillshare_downloader/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-22 04:58:55.000000 skillshare_downloader-0.2.1/skillshare_downloader/__main__.py
+-rw-r--r--   0        0        0     6061 2023-07-23 07:11:13.000000 skillshare_downloader-0.2.1/skillshare_downloader/main.py
+-rw-r--r--   0        0        0     2529 2023-07-19 05:02:18.000000 skillshare_downloader-0.2.1/skillshare_downloader/progress.py
+-rw-r--r--   0        0        0    16425 2023-07-23 07:31:17.000000 skillshare_downloader-0.2.1/skillshare_downloader/skillshare.py
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 skillshare_downloader-0.2.1/PKG-INFO
```

### Comparing `skillshare_downloader-0.2.0/LICENSE` & `skillshare_downloader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skillshare_downloader-0.2.0/README.md` & `skillshare_downloader-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `skillshare_downloader-0.2.0/pyproject.toml` & `skillshare_downloader-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1.1.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "skillshare_downloader"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python package to download Skillshare classes."
 readme = "README.md"  # Make sure you have a valid README.md file in the root of your project.
 license = "MIT"
 authors = ["Uriel Albarran Oropeza <hello@ozonostudio.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `skillshare_downloader-0.2.0/skillshare_downloader/main.py` & `skillshare_downloader-0.2.1/skillshare_downloader/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,16 +100,16 @@
             return instructions + help_text
         
     # parser = CustomArgumentParser()
     parser = CustomArgumentParser(prog='skillshare-download')  # Add "python" before the script name
     parser.add_argument('-h', '--help', action='help', help='show the current help')
     parser.add_argument('id', nargs='?', type=str, default=None, help='your class id, ex: 1749908541')
     parser.add_argument("-config", action="store_true", help="Configure the Skillshare Downloader")
-    parser.add_argument('-s', type=str, default='en-US', choices=['es-MX', 'de', 'en-US', 'pt', 'fr'], help='Subtitles language')
-    parser.add_argument('-r', type=str, default='854x480', choices=['1920x1080', '1728x1080', '1280x720', '1152x720', '854x480', '768x480', '640x360', '576x360', '426x240', '384x240'], help='Video resolution')
+    parser.add_argument('-s', type=str, default='en-US', choices=['es-MX', 'de', 'en-US', 'pt', 'fr'], help='Subtitles language (if nothing found subtitles are going to be downloaded as en-US)')
+    parser.add_argument('-r', type=str, default='854x480', choices=['1920x1080', '1280x720', '854x480', '640x360', '426x240'], help='Video resolution (if not found, the code it\'s going to search for the next lower resolution)')
     parser.add_argument('-t', type=str, default=None, help='Your telegram group to save the files in format .mp4')
     parser.add_argument("-e", action="store_true", help="Erase the files after upload (only if there\'s a valid telegram group or id)")
 
     args = parser.parse_args()
     if args.config:
         configure()
         exit(0)
```

### Comparing `skillshare_downloader-0.2.0/skillshare_downloader/progress.py` & `skillshare_downloader-0.2.1/skillshare_downloader/progress.py`

 * *Files identical despite different names*

### Comparing `skillshare_downloader-0.2.0/skillshare_downloader/skillshare.py` & `skillshare_downloader-0.2.1/skillshare_downloader/skillshare.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,50 +279,59 @@
         video_url = None
         for line in lines:
             if line.startswith("#EXT-X-STREAM-INF:RESOLUTION="):
                 if resolution in line:
                     video_path = lines[lines.index(line) + 1]
                     video_url = f"{base_url}/{video_path}"
                     break
-
+        
         # Download audio
         ffmpegDown(
             ["ffmpeg", "-i", audio_url, "-c:a", "aac", "-b:a", "128k", "-y", audio_file], 'audio'
         ).run()
         pbar.update(1)
 
         # Download video
-        lookres = ['1920x1080', '1728x1080', '1280x720', '1152x720', '854x480', '768x480', '640x360', '576x360', '426x240', '384x240']
+        next_resolution = None  # Variable to store the next lower resolution
+        skip = False  # Flag to indicate if previous resolutions should be skipped
+
         if video_url is not None:
             ffmpegDown(
                 ["ffmpeg", "-i", video_url, "-c", "copy", "-bsf:v", "h264_mp4toannexb", "-y", video_file], 'video'
             ).run()
             pbar.update(1)
         else:
-            skip = False  # Flag to indicate if previous resolutions should be skipped
-            for resolution_choice in lookres:
-                if skip and resolution_choice != resolution:
-                    continue
-                for line in lines:
-                    if line.startswith("#EXT-X-STREAM-INF:RESOLUTION="):
-                        if resolution_choice in line:
-                            video_path = lines[lines.index(line) + 1]
-                            video_url = f"{base_url}/{video_path}"
-                            break
-
-                if video_url is not None:
-                    print(f'\033[91mResolution {resolution} not found looking for lower resolution\033[0m')
-                    print(f'\033[92mDownloading at {resolution_choice}\033[0m')
-                    ffmpegDown(
-                        ["ffmpeg", "-i", video_url, "-c", "copy", "-bsf:v", "h264_mp4toannexb", "-y", video_file], 'video'
-                    ).run()
-                    pbar.update(1)
+            for line in lines:
+                if line.startswith("#EXT-X-STREAM-INF:RESOLUTION="):
+                    # Extract the resolution from the line
+                    resolution_choice = line.split('=')[1].split(',')[0]
+
+                    if skip and resolution_choice != resolution:
+                        continue
+                    
                     if resolution_choice == resolution:
                         skip = True  # Set the flag to True to skip previous resolutions
-                    break
+                    else:
+                        next_resolution = resolution_choice
+                        break
+
+            if next_resolution is not None:
+                print(f'\033[91mResolution {resolution} not found looking for lower resolution\033[0m')
+                print(f'\033[92mDownloading at {next_resolution}\033[0m')
+                for line in lines:
+                    if next_resolution in line:
+                        video_path = lines[lines.index(line) + 1]
+                        video_url = f"{base_url}/{video_path}"
+                        break
+
+                ffmpegDown(
+                    ["ffmpeg", "-i", video_url, "-c", "copy", "-bsf:v", "h264_mp4toannexb", "-y", video_file], 'video'
+                ).run()
+                pbar.update(1)
+
 
 
         if telegram is not None:
             # Combine audio and video into a single .mp4 file
             print(f'\033[33mCombining resources into .mp4 \033[0m')
             subprocess.run(
                 [
```

### Comparing `skillshare_downloader-0.2.0/PKG-INFO` & `skillshare_downloader-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillshare-downloader
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package to download Skillshare classes.
 License: MIT
 Author: Uriel Albarran Oropeza
 Author-email: hello@ozonostudio.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

