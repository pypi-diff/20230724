# Comparing `tmp/streamlitopencvplayer-1.6.3.tar.gz` & `tmp/streamlitopencvplayer-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.6.3.tar", last modified: Mon Jul 24 15:48:06 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.6.4.tar", last modified: Mon Jul 24 15:51:05 2023, max compression
```

## Comparing `streamlitopencvplayer-1.6.3.tar` & `streamlitopencvplayer-1.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:48:06.031379 streamlitopencvplayer-1.6.3/
--rw-rw-rw-   0        0        0      419 2023-07-24 15:48:06.030374 streamlitopencvplayer-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 15:48:06.032376 streamlitopencvplayer-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-24 15:47:58.000000 streamlitopencvplayer-1.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:48:06.002377 streamlitopencvplayer-1.6.3/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8754 2023-07-24 15:47:49.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:48:06.018377 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-24 15:48:05.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-24 15:48:05.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:48:05.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-24 15:48:05.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 15:48:06.025373 streamlitopencvplayer-1.6.3/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.6.3/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.6.3/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:51:05.920899 streamlitopencvplayer-1.6.4/
+-rw-rw-rw-   0        0        0      419 2023-07-24 15:51:05.919900 streamlitopencvplayer-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:51:05.921898 streamlitopencvplayer-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-24 15:51:00.000000 streamlitopencvplayer-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:51:05.890901 streamlitopencvplayer-1.6.4/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.6.4/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8756 2023-07-24 15:50:48.000000 streamlitopencvplayer-1.6.4/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:51:05.907901 streamlitopencvplayer-1.6.4/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-24 15:51:05.000000 streamlitopencvplayer-1.6.4/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-24 15:51:05.000000 streamlitopencvplayer-1.6.4/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:51:05.000000 streamlitopencvplayer-1.6.4/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-24 15:51:05.000000 streamlitopencvplayer-1.6.4/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 15:51:05.914897 streamlitopencvplayer-1.6.4/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.6.4/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.6.4/test/test.py
```

### Comparing `streamlitopencvplayer-1.6.3/README.md` & `streamlitopencvplayer-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.6.3/setup.py` & `streamlitopencvplayer-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.6.3' 
+VERSION = '1.6.4' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.6.3/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.6.4/streamlitopencvplayer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     while st.session_state["resume"] is False:
         # for x in range(int(st.session_state['fps'])):
         # Read the next frame from the video capture
         ret, frame = st.session_state["capture"].read()
         # Update the current frame in session state
 
         if draw_detections:
-            if len(st.session_state['data'])<= 0 :
+            if len(st.session_state['alerts'])== 0 :
                 st.warning("There's no Detections to draw on this video")
                 break
             else :
             # Perform actions on the frame
                 for i in range(len(st.session_state['data'])):
 
                     # Check if the current frame matches an alert frame
```

### Comparing `streamlitopencvplayer-1.6.3/test/test.py` & `streamlitopencvplayer-1.6.4/test/test.py`

 * *Files identical despite different names*

