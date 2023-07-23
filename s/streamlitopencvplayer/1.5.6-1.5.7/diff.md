# Comparing `tmp/streamlitopencvplayer-1.5.6.tar.gz` & `tmp/streamlitopencvplayer-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.5.6.tar", last modified: Sun Jul 23 21:32:54 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.5.7.tar", last modified: Sun Jul 23 22:58:31 2023, max compression
```

## Comparing `streamlitopencvplayer-1.5.6.tar` & `streamlitopencvplayer-1.5.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 21:32:54.465499 streamlitopencvplayer-1.5.6/
--rw-rw-rw-   0        0        0      419 2023-07-23 21:32:54.463296 streamlitopencvplayer-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-23 21:32:54.465499 streamlitopencvplayer-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-23 21:32:48.000000 streamlitopencvplayer-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 21:32:54.432676 streamlitopencvplayer-1.5.6/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.6/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8225 2023-07-23 21:30:10.000000 streamlitopencvplayer-1.5.6/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-23 21:32:54.452299 streamlitopencvplayer-1.5.6/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-23 21:32:54.000000 streamlitopencvplayer-1.5.6/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-23 21:32:54.000000 streamlitopencvplayer-1.5.6/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 21:32:54.000000 streamlitopencvplayer-1.5.6/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-23 21:32:54.000000 streamlitopencvplayer-1.5.6/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 21:32:54.458635 streamlitopencvplayer-1.5.6/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.6/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.6/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:58:31.461945 streamlitopencvplayer-1.5.7/
+-rw-rw-rw-   0        0        0      419 2023-07-23 22:58:31.459906 streamlitopencvplayer-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-23 22:58:31.462945 streamlitopencvplayer-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-23 22:58:24.000000 streamlitopencvplayer-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:58:31.428011 streamlitopencvplayer-1.5.7/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8278 2023-07-23 22:58:19.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:58:31.447922 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-23 22:58:31.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-23 22:58:31.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 22:58:31.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-23 22:58:31.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-23 22:58:31.456369 streamlitopencvplayer-1.5.7/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.7/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.7/test/test.py
```

### Comparing `streamlitopencvplayer-1.5.6/README.md` & `streamlitopencvplayer-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.5.6/setup.py` & `streamlitopencvplayer-1.5.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.5.6' 
+VERSION = '1.5.7' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.5.6/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.5.7/streamlitopencvplayer/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import streamlit as st
 
 
 if "alerts" not in st.session_state:
     st.session_state['alerts'] = []
 if "data" not in st.session_state:
     st.session_state['data'] = []
-
+if "capture" not in st.session_state:
+            # Open the video file
+    st.session_state['capture'] = None
 # Function to display video in the Streamlit app
 
 
 def draw_on_frames(stframe, frame, i):
     # Draw detections on the frame
     for j in range(len(st.session_state['data'][i])):
         output = cv2.rectangle(frame, (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]), (
@@ -24,17 +26,16 @@
     # Display the frame with detections
     stframe.image(output, caption='', width=500)
     time.sleep(0.05)
 
 
 def display_video(video_path, json_file):
     # Check if video_url variables exists in session state
-    if "capture" not in st.session_state:
-            # Open the video file
-            st.session_state['capture'] = cv2.VideoCapture(video_path)
+    # Open the video file
+    st.session_state['capture'] = cv2.VideoCapture(video_path)
 
 
 
     # Check if "fps" variable exists in session state
     if "fps" not in st.session_state:
         st.session_state['fps'] = st.session_state['capture'].get(
             cv2.CAP_PROP_FPS)
```

### Comparing `streamlitopencvplayer-1.5.6/test/test.py` & `streamlitopencvplayer-1.5.7/test/test.py`

 * *Files identical despite different names*

