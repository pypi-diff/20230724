# Comparing `tmp/streamlitopencvplayer-1.5.7.tar.gz` & `tmp/streamlitopencvplayer-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.5.7.tar", last modified: Sun Jul 23 22:58:31 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.5.8.tar", last modified: Sun Jul 23 22:59:55 2023, max compression
```

## Comparing `streamlitopencvplayer-1.5.7.tar` & `streamlitopencvplayer-1.5.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 22:58:31.461945 streamlitopencvplayer-1.5.7/
--rw-rw-rw-   0        0        0      419 2023-07-23 22:58:31.459906 streamlitopencvplayer-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-23 22:58:31.462945 streamlitopencvplayer-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-23 22:58:24.000000 streamlitopencvplayer-1.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 22:58:31.428011 streamlitopencvplayer-1.5.7/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8278 2023-07-23 22:58:19.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-23 22:58:31.447922 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-23 22:58:31.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-23 22:58:31.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 22:58:31.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-23 22:58:31.000000 streamlitopencvplayer-1.5.7/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 22:58:31.456369 streamlitopencvplayer-1.5.7/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.7/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:59:55.867715 streamlitopencvplayer-1.5.8/
+-rw-rw-rw-   0        0        0      419 2023-07-23 22:59:55.866429 streamlitopencvplayer-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-23 22:59:55.868717 streamlitopencvplayer-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-23 22:59:50.000000 streamlitopencvplayer-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:59:55.833812 streamlitopencvplayer-1.5.8/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8185 2023-07-23 22:59:46.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:59:55.855361 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-23 22:59:55.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-23 22:59:55.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 22:59:55.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-23 22:59:55.000000 streamlitopencvplayer-1.5.8/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-23 22:59:55.862573 streamlitopencvplayer-1.5.8/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.8/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.8/test/test.py
```

### Comparing `streamlitopencvplayer-1.5.7/README.md` & `streamlitopencvplayer-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.5.7/setup.py` & `streamlitopencvplayer-1.5.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.5.7' 
+VERSION = '1.5.8' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.5.7/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.5.8/streamlitopencvplayer/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,15 @@
     with column3:
         # Create buttons for alerts
         st.subheader('Alerts :')
         # Determine the number of buttons based on the number of alerts
         num_buttons = len(st.session_state['alerts'])
         # Create a dictionary to store the button values
         button_values = {f'{i}': 0 for i in range(num_buttons)}
-        st.write(len(st.session_state['alerts']))
-        st.write(st.session_state['data'])
+
 
         # Display the buttons and update their values
         for button_label, button_value in button_values.items():
             if st.button(str('Alert ')+button_label):
                 # Set the selected button to 1, others to 0
                 button_values = {label: 1 if label ==
                                  button_label else 0 for label in button_values}
```

### Comparing `streamlitopencvplayer-1.5.7/test/test.py` & `streamlitopencvplayer-1.5.8/test/test.py`

 * *Files identical despite different names*

