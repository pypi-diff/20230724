# Comparing `tmp/streamlitopencvplayer-1.6.0.tar.gz` & `tmp/streamlitopencvplayer-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.6.0.tar", last modified: Sun Jul 23 23:09:57 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.6.1.tar", last modified: Mon Jul 24 10:01:53 2023, max compression
```

## Comparing `streamlitopencvplayer-1.6.0.tar` & `streamlitopencvplayer-1.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 23:09:57.498009 streamlitopencvplayer-1.6.0/
--rw-rw-rw-   0        0        0      419 2023-07-23 23:09:57.495913 streamlitopencvplayer-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-23 23:09:57.499009 streamlitopencvplayer-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-23 23:09:52.000000 streamlitopencvplayer-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 23:09:57.465785 streamlitopencvplayer-1.6.0/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.6.0/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8517 2023-07-23 23:09:11.000000 streamlitopencvplayer-1.6.0/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-23 23:09:57.484522 streamlitopencvplayer-1.6.0/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-23 23:09:57.000000 streamlitopencvplayer-1.6.0/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-23 23:09:57.000000 streamlitopencvplayer-1.6.0/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 23:09:57.000000 streamlitopencvplayer-1.6.0/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-23 23:09:57.000000 streamlitopencvplayer-1.6.0/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 23:09:57.490914 streamlitopencvplayer-1.6.0/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.6.0/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.6.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:01:53.297991 streamlitopencvplayer-1.6.1/
+-rw-rw-rw-   0        0        0      419 2023-07-24 10:01:53.296185 streamlitopencvplayer-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 10:01:53.298995 streamlitopencvplayer-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-24 10:01:48.000000 streamlitopencvplayer-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:01:53.254528 streamlitopencvplayer-1.6.1/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.6.1/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8574 2023-07-24 10:01:40.000000 streamlitopencvplayer-1.6.1/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:01:53.281611 streamlitopencvplayer-1.6.1/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-24 10:01:52.000000 streamlitopencvplayer-1.6.1/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-24 10:01:53.000000 streamlitopencvplayer-1.6.1/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 10:01:52.000000 streamlitopencvplayer-1.6.1/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-24 10:01:52.000000 streamlitopencvplayer-1.6.1/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 10:01:53.291093 streamlitopencvplayer-1.6.1/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.6.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.6.1/test/test.py
```

### Comparing `streamlitopencvplayer-1.6.0/README.md` & `streamlitopencvplayer-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.6.0/setup.py` & `streamlitopencvplayer-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.6.0' 
+VERSION = '1.6.1' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.6.0/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.6.1/streamlitopencvplayer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
             frame, st.session_state['data'][i][j][3], (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
     # Display the frame with detections
     stframe.image(output, caption='', width=500)
     time.sleep(0.05)
 
 
 def display_video(video_path, json_file):
+    st.write(video_path)
+    st.write(json_file)
     # Check if video_url variables exists in session state
     if "name_vid_old" not in st.session_state and "name_vid_sel" not in st.session_state:
         if "capture" not in st.session_state:
             # Open the video file
             st.session_state['capture'] = cv2.VideoCapture(video_path)
     else:
         # Check if the video URL has changed
@@ -179,17 +181,17 @@
     if st.session_state["resume"]:
         # Clear the container
         container_2.empty()
         pause = container_2.button('▶')
         st.session_state["resume"] = False
 
 
-def main():
+"""def main():
 
     video_path = "https://cvlogger.blob.core.windows.net/json-concat-files/1689004947.7068138_1689004953.7068138.webm?sv=2021-10-04&st=2023-07-11T15%3A21%3A27Z&se=2023-07-26T15%3A21%3A00Z&sr=b&sp=r&sig=u6uuOUo9wvn5KJFNUnUR3axYtC815SUQBuDqNIC4L%2Bw%3D"
     down_json = "https://cvlogger.blob.core.windows.net/json-concat-files/1689004947.7068138_1689004953.7068138_global.json?sv=2021-10-04&st=2023-07-11T15%3A22%3A03Z&se=2023-07-26T15%3A22%3A00Z&sr=b&sp=r&sig=qSHWvDUIOOT%2F%2Bff270JVX7ucSRn5Lylgw5%2Fh9iTa4BY%3D"
     if video_path is not None:
         display_video(video_path, down_json)
 
 
 if __name__ == "__main__":
-    main()
+    main()"""
```

### Comparing `streamlitopencvplayer-1.6.0/test/test.py` & `streamlitopencvplayer-1.6.1/test/test.py`

 * *Files identical despite different names*

