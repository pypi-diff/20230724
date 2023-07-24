# Comparing `tmp/streamlitopencvplayer-1.6.2.tar.gz` & `tmp/streamlitopencvplayer-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.6.2.tar", last modified: Mon Jul 24 15:42:08 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.6.3.tar", last modified: Mon Jul 24 15:48:06 2023, max compression
```

## Comparing `streamlitopencvplayer-1.6.2.tar` & `streamlitopencvplayer-1.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:42:08.078187 streamlitopencvplayer-1.6.2/
--rw-rw-rw-   0        0        0      419 2023-07-24 15:42:08.077186 streamlitopencvplayer-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 15:42:08.079187 streamlitopencvplayer-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-24 15:42:02.000000 streamlitopencvplayer-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:42:08.045189 streamlitopencvplayer-1.6.2/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.6.2/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8568 2023-07-24 15:41:38.000000 streamlitopencvplayer-1.6.2/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:42:08.064188 streamlitopencvplayer-1.6.2/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-24 15:42:07.000000 streamlitopencvplayer-1.6.2/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-24 15:42:07.000000 streamlitopencvplayer-1.6.2/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:42:07.000000 streamlitopencvplayer-1.6.2/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-24 15:42:07.000000 streamlitopencvplayer-1.6.2/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 15:42:08.072189 streamlitopencvplayer-1.6.2/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.6.2/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.6.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:48:06.031379 streamlitopencvplayer-1.6.3/
+-rw-rw-rw-   0        0        0      419 2023-07-24 15:48:06.030374 streamlitopencvplayer-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:48:06.032376 streamlitopencvplayer-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-24 15:47:58.000000 streamlitopencvplayer-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:48:06.002377 streamlitopencvplayer-1.6.3/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8754 2023-07-24 15:47:49.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:48:06.018377 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-24 15:48:05.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-24 15:48:05.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:48:05.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-24 15:48:05.000000 streamlitopencvplayer-1.6.3/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 15:48:06.025373 streamlitopencvplayer-1.6.3/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.6.3/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.6.3/test/test.py
```

### Comparing `streamlitopencvplayer-1.6.2/README.md` & `streamlitopencvplayer-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.6.2/setup.py` & `streamlitopencvplayer-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.6.2' 
+VERSION = '1.6.3' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.6.2/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.6.3/streamlitopencvplayer/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,20 +141,24 @@
     while st.session_state["resume"] is False:
         # for x in range(int(st.session_state['fps'])):
         # Read the next frame from the video capture
         ret, frame = st.session_state["capture"].read()
         # Update the current frame in session state
 
         if draw_detections:
+            if len(st.session_state['data'])<= 0 :
+                st.warning("There's no Detections to draw on this video")
+                break
+            else :
             # Perform actions on the frame
-            for i in range(len(st.session_state['data'])):
+                for i in range(len(st.session_state['data'])):
 
-                # Check if the current frame matches an alert frame
-                if int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)) == int(st.session_state['alerts'][i]):
-                    draw_on_frames(stframe, frame, i)
+                    # Check if the current frame matches an alert frame
+                    if int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)) == int(st.session_state['alerts'][i]):
+                        draw_on_frames(stframe, frame, i)
         # Display the original frame
         stframe.image(
             frame, caption='', width=500)
         time.sleep(0.05)
 
         # Handle button clicks
         if pause:
```

### Comparing `streamlitopencvplayer-1.6.2/test/test.py` & `streamlitopencvplayer-1.6.3/test/test.py`

 * *Files identical despite different names*

