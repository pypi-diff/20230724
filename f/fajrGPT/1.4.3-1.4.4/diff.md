# Comparing `tmp/fajrGPT-1.4.3.tar.gz` & `tmp/fajrGPT-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.4.3.tar", last modified: Mon Jul 24 11:58:05 2023, max compression
+gzip compressed data, was "fajrGPT-1.4.4.tar", last modified: Mon Jul 24 12:09:09 2023, max compression
```

## Comparing `fajrGPT-1.4.3.tar` & `fajrGPT-1.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 11:58:05.812394 fajrGPT-1.4.3/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.3/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 11:58:05.812213 fajrGPT-1.4.3/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.3/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 11:58:05.810573 fajrGPT-1.4.3/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.3/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.3/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    18392 2023-07-24 11:56:49.000000 fajrGPT-1.4.3/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 11:58:05.811922 fajrGPT-1.4.3/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-24 11:58:05.000000 fajrGPT-1.4.3/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-24 11:58:05.812434 fajrGPT-1.4.3/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-24 11:57:42.000000 fajrGPT-1.4.3/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 12:09:09.440852 fajrGPT-1.4.4/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.4/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 12:09:09.440639 fajrGPT-1.4.4/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.4/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 12:09:09.438543 fajrGPT-1.4.4/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.4/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.4/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    18421 2023-07-24 12:08:27.000000 fajrGPT-1.4.4/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 12:09:09.440418 fajrGPT-1.4.4/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-24 12:09:09.440893 fajrGPT-1.4.4/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-24 12:08:38.000000 fajrGPT-1.4.4/setup.py
```

### Comparing `fajrGPT-1.4.3/LICENSE` & `fajrGPT-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.3/PKG-INFO` & `fajrGPT-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.3
+Version: 1.4.4
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.3/README.md` & `fajrGPT-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.3/fajrGPT/quran_metadata.py` & `fajrGPT-1.4.4/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.3/fajrGPT/wake.py` & `fajrGPT-1.4.4/fajrGPT/wake.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,22 +278,22 @@
             I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
 
             First please give some brief context about Chapter {chapter_number} from the Qur'an. Then, to the best of your ability, explain the meaning of the verse below. 
             I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to interpret the possible meaning of the verse given. \n\n Verse: {verse_text} \n\n Explanation:
             """
             explanation = query_gpt(prompt2)
         else:
-            concatenated_explanations = '\n\n'.join(explanations)
+            context = explanations[0].split('\n')[0] # get the context about what the chapter is about.
             prompt2 = f"""
             I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
             You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
             I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
 
             To the best of your ability, explain the meaning of the verse below. 
-            I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to emulate Sheikh Hamza Yusuf and interpret the possible meaning of the given verse. \n\n Verse: {verse_text} \n\n Context: {concatenated_explanations} \n\n Explanation:
+            I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to emulate Sheikh Hamza Yusuf and interpret the possible meaning of the given verse. \n\n Verse: \n {verse_text} \n\n Context: \n {context} \n\n Explanation: \n
             """
             explanation = query_gpt(prompt2)
         verse_texts.append(verse_text)
         explanations.append(explanation)
     
     # begin the interactive session
     for verse_text, explanation, verse in zip(verse_texts, explanations, verses):
```

### Comparing `fajrGPT-1.4.3/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.4.4/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.3
+Version: 1.4.4
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.3/setup.py` & `fajrGPT-1.4.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.4.3",
+    version="1.4.4",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

