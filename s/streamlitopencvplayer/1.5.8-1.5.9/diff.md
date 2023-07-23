# Comparing `tmp/streamlitopencvplayer-1.5.8.tar.gz` & `tmp/streamlitopencvplayer-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.5.8.tar", last modified: Sun Jul 23 22:59:55 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.5.9.tar", last modified: Sun Jul 23 23:04:33 2023, max compression
```

## Comparing `streamlitopencvplayer-1.5.8.tar` & `streamlitopencvplayer-1.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 22:59:55.867715 streamlitopencvplayer-1.5.8/
--rw-rw-rw-   0        0        0      419 2023-07-23 22:59:55.866429 streamlitopencvplayer-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-23 22:59:55.868717 streamlitopencvplayer-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-23 22:59:50.000000 streamlitopencvplayer-1.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 22:59:55.833812 streamlitopencvplayer-1.5.8/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8185 2023-07-23 22:59:46.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-23 22:59:55.855361 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-23 22:59:55.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-23 22:59:55.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 22:59:55.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-23 22:59:55.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 22:59:55.862573 streamlitopencvplayer-1.5.8/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.8/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-23 23:04:33.430564 streamlitopencvplayer-1.5.9/
+-rw-rw-rw-   0        0        0      419 2023-07-23 23:04:33.429564 streamlitopencvplayer-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-23 23:04:33.431987 streamlitopencvplayer-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-23 23:04:27.000000 streamlitopencvplayer-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-23 23:04:33.399417 streamlitopencvplayer-1.5.9/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.9/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8610 2023-07-23 23:04:18.000000 streamlitopencvplayer-1.5.9/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-23 23:04:33.418621 streamlitopencvplayer-1.5.9/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-23 23:04:33.000000 streamlitopencvplayer-1.5.9/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-23 23:04:33.000000 streamlitopencvplayer-1.5.9/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 23:04:33.000000 streamlitopencvplayer-1.5.9/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-23 23:04:33.000000 streamlitopencvplayer-1.5.9/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-23 23:04:33.425118 streamlitopencvplayer-1.5.9/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.9/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.9/test/test.py
```

### Comparing `streamlitopencvplayer-1.5.8/README.md` & `streamlitopencvplayer-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.5.8/setup.py` & `streamlitopencvplayer-1.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.5.8' 
+VERSION = '1.5.9' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.5.8/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.5.9/streamlitopencvplayer/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import streamlit as st
 
 
 if "alerts" not in st.session_state:
     st.session_state['alerts'] = []
 if "data" not in st.session_state:
     st.session_state['data'] = []
-if "capture" not in st.session_state:
-            # Open the video file
-    st.session_state['capture'] = None
+
 # Function to display video in the Streamlit app
 
 
 def draw_on_frames(stframe, frame, i):
     # Draw detections on the frame
     for j in range(len(st.session_state['data'][i])):
         output = cv2.rectangle(frame, (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]), (
@@ -26,17 +24,23 @@
     # Display the frame with detections
     stframe.image(output, caption='', width=500)
     time.sleep(0.05)
 
 
 def display_video(video_path, json_file):
     # Check if video_url variables exists in session state
-    # Open the video file
-    st.session_state['capture'] = cv2.VideoCapture(video_path)
-
+    if "name_vid_old" not in st.session_state and "name_vid_sel" not in st.session_state:
+        if "capture" not in st.session_state:
+            # Open the video file
+            st.session_state['capture'] = cv2.VideoCapture(video_path)
+    else:
+        # Check if the video URL has changed
+        if st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
+            st.session_state['capture'] = cv2.VideoCapture(video_path)
+            st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
 
 
     # Check if "fps" variable exists in session state
     if "fps" not in st.session_state:
         st.session_state['fps'] = st.session_state['capture'].get(
             cv2.CAP_PROP_FPS)
     if not st.session_state["capture"].isOpened():
@@ -84,15 +88,16 @@
     with column3:
         # Create buttons for alerts
         st.subheader('Alerts :')
         # Determine the number of buttons based on the number of alerts
         num_buttons = len(st.session_state['alerts'])
         # Create a dictionary to store the button values
         button_values = {f'{i}': 0 for i in range(num_buttons)}
-
+        st.write(len(st.session_state['alerts']))
+        st.write(st.session_state['data'])
 
         # Display the buttons and update their values
         for button_label, button_value in button_values.items():
             if st.button(str('Alert ')+button_label):
                 # Set the selected button to 1, others to 0
                 button_values = {label: 1 if label ==
                                  button_label else 0 for label in button_values}
```

### Comparing `streamlitopencvplayer-1.5.8/test/test.py` & `streamlitopencvplayer-1.5.9/test/test.py`

 * *Files identical despite different names*

