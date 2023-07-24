# Comparing `tmp/fajrGPT-1.4.2.tar.gz` & `tmp/fajrGPT-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.4.2.tar", last modified: Mon Jul 24 01:50:18 2023, max compression
+gzip compressed data, was "fajrGPT-1.4.3.tar", last modified: Mon Jul 24 11:58:05 2023, max compression
```

## Comparing `fajrGPT-1.4.2.tar` & `fajrGPT-1.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 01:50:18.295879 fajrGPT-1.4.2/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.2/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 01:50:18.294832 fajrGPT-1.4.2/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.2/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 01:50:18.292606 fajrGPT-1.4.2/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.2/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.2/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    18218 2023-07-23 19:28:17.000000 fajrGPT-1.4.2/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 01:50:18.294052 fajrGPT-1.4.2/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 01:50:18.000000 fajrGPT-1.4.2/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-24 01:50:18.000000 fajrGPT-1.4.2/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-24 01:50:18.000000 fajrGPT-1.4.2/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-24 01:50:18.000000 fajrGPT-1.4.2/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-24 01:50:18.000000 fajrGPT-1.4.2/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-24 01:50:18.000000 fajrGPT-1.4.2/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-24 01:50:18.296003 fajrGPT-1.4.2/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-24 01:49:33.000000 fajrGPT-1.4.2/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 11:58:05.812394 fajrGPT-1.4.3/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.3/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 11:58:05.812213 fajrGPT-1.4.3/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.3/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 11:58:05.810573 fajrGPT-1.4.3/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.3/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.3/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    18392 2023-07-24 11:56:49.000000 fajrGPT-1.4.3/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 11:58:05.811922 fajrGPT-1.4.3/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-24 11:58:05.812434 fajrGPT-1.4.3/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-24 11:57:42.000000 fajrGPT-1.4.3/setup.py
```

### Comparing `fajrGPT-1.4.2/LICENSE` & `fajrGPT-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.2/PKG-INFO` & `fajrGPT-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.2/README.md` & `fajrGPT-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.2/fajrGPT/quran_metadata.py` & `fajrGPT-1.4.3/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.2/fajrGPT/wake.py` & `fajrGPT-1.4.3/fajrGPT/wake.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 COMPLETIONS_MODEL = "gpt-3.5-turbo"
 
 @click.command()
 @click.option('--url', required=True, help='YouTube URL containing desired audio data.')
 @click.option('--time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
 @click.option('--output', required=True, help='Name of the output file.')
 @click.option('--names-flag', required=False, help='Whether or not to include a randomly selected name of Allah in the preamble.', default=True)
+@click.option('--transition-time', required=False, help='Time in seconds for the transition between the output audio and the Quran verses.')
 @click.option('--surah', required=False, help='Specific Surah from the Quran. Should be given as integer.')
 
-def main(url, time, output, names_flag, surah=None):
+def main(url, time, output, names_flag, transition_time=600, surah=None):
     # Check surah option
     if surah:
         # make the output file name the same as the surah
         output = 'quran-' + '{:03d}'.format(int(surah))
         flag = download_surah(surah, output)
     else:
         # Download video
@@ -41,15 +42,15 @@
     # convert time to seconds
     countdown_seconds = convert_to_seconds(time)
 
     # Start countdown
     countdown(countdown_seconds)
 
     # Play audio with fade-in effect on a separate thread
-    play_audio_thread = Thread(target=play_audio, args=(f'{output}.mp3',600))
+    play_audio_thread = Thread(target=play_audio, args=(f'{output}.mp3',transition_time))
     play_audio_thread.start()
 
     # display a name of Allah
     get_name_of_allah_and_explanation(names_flag)
 
     # stop the misharay audio once the user has finished reading the name of Allah on a separate thread
     stop_audio(5)
```

### Comparing `fajrGPT-1.4.2/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.4.3/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.2/setup.py` & `fajrGPT-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.4.2",
+    version="1.4.3",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

