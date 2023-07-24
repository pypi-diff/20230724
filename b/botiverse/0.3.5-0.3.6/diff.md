# Comparing `tmp/botiverse-0.3.5.tar.gz` & `tmp/botiverse-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botiverse-0.3.5.tar", last modified: Mon Jul 24 16:23:43 2023, max compression
+gzip compressed data, was "botiverse-0.3.6.tar", last modified: Mon Jul 24 16:40:42 2023, max compression
```

## Comparing `botiverse-0.3.5.tar` & `botiverse-0.3.6.tar`

### file list

```diff
@@ -1,22 +1,47 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.420411 botiverse-0.3.5/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 16:23:43.420182 botiverse-0.3.5/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.5/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.416896 botiverse-0.3.5/botiverse/
--rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 15:57:44.000000 botiverse-0.3.5/botiverse/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.418365 botiverse-0.3.5/botiverse/bots/
--rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 15:31:32.000000 botiverse-0.3.5/botiverse/bots/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.418882 botiverse-0.3.5/botiverse/gui/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.5/botiverse/gui/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.5/botiverse/gui/gui.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.419255 botiverse-0.3.5/botiverse/models/
--rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.5/botiverse/models/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.419636 botiverse-0.3.5/botiverse/preprocessors/
--rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.5/botiverse/preprocessors/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:23:43.418142 botiverse-0.3.5/botiverse.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      343 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 16:23:43.000000 botiverse-0.3.5/botiverse.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 16:23:43.420488 botiverse-0.3.5/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     2208 2023-07-24 16:23:39.000000 botiverse-0.3.5/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.234712 botiverse-0.3.6/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 16:40:42.234375 botiverse-0.3.6/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.3.6/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.218710 botiverse-0.3.6/botiverse/
+-rw-r--r--   0 essam      (501) staff       (20)       84 2023-07-24 15:57:44.000000 botiverse-0.3.6/botiverse/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.224696 botiverse-0.3.6/botiverse/bots/
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.225812 botiverse-0.3.6/botiverse/bots/BasicBot/
+-rw-r--r--   0 essam      (501) staff       (20)     7769 2023-07-24 14:11:30.000000 botiverse-0.3.6/botiverse/bots/BasicBot/BasicBot.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:10.000000 botiverse-0.3.6/botiverse/bots/BasicBot/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.226589 botiverse-0.3.6/botiverse/bots/ConverseBot/
+-rw-r--r--   0 essam      (501) staff       (20)     6760 2023-07-24 15:08:00.000000 botiverse-0.3.6/botiverse/bots/ConverseBot/ConverseBot.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.6/botiverse/bots/ConverseBot/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.227911 botiverse-0.3.6/botiverse/bots/VoiceBot/
+-rw-r--r--   0 essam      (501) staff       (20)     4025 2023-07-24 13:43:59.000000 botiverse-0.3.6/botiverse/bots/VoiceBot/SpeechClassifier.py
+-rw-r--r--   0 essam      (501) staff       (20)     3473 2023-07-24 13:43:43.000000 botiverse-0.3.6/botiverse/bots/VoiceBot/VoiceBot.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:19:05.000000 botiverse-0.3.6/botiverse/bots/VoiceBot/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1758 2023-07-24 13:20:58.000000 botiverse-0.3.6/botiverse/bots/VoiceBot/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.229591 botiverse-0.3.6/botiverse/bots/WhizBot/
+-rw-r--r--   0 essam      (501) staff       (20)     2691 2023-07-24 14:25:02.000000 botiverse-0.3.6/botiverse/bots/WhizBot/WhizBot.py
+-rw-r--r--   0 essam      (501) staff       (20)     5084 2023-07-24 15:08:20.000000 botiverse-0.3.6/botiverse/bots/WhizBot/WhizBot_BERT.py
+-rw-r--r--   0 essam      (501) staff       (20)     5309 2023-07-24 15:08:14.000000 botiverse-0.3.6/botiverse/bots/WhizBot/WhizBot_GRU.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-10 23:47:13.000000 botiverse-0.3.6/botiverse/bots/WhizBot/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)      407 2023-07-24 16:36:12.000000 botiverse-0.3.6/botiverse/bots/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.230794 botiverse-0.3.6/botiverse/bots/basic_TODS/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:16:45.000000 botiverse-0.3.6/botiverse/bots/basic_TODS/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     4076 2023-07-24 07:57:53.000000 botiverse-0.3.6/botiverse/bots/basic_TODS/basic_TODS.py
+-rw-r--r--   0 essam      (501) staff       (20)     1387 2023-07-10 06:53:03.000000 botiverse-0.3.6/botiverse/bots/basic_TODS/tods_example.py
+-rw-r--r--   0 essam      (501) staff       (20)     7368 2023-07-10 06:53:03.000000 botiverse-0.3.6/botiverse/bots/basic_TODS/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.231898 botiverse-0.3.6/botiverse/bots/deep_TODS/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-06 20:16:45.000000 botiverse-0.3.6/botiverse/bots/deep_TODS/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     5990 2023-07-24 07:57:53.000000 botiverse-0.3.6/botiverse/bots/deep_TODS/deep_TODS.py
+-rw-r--r--   0 essam      (501) staff       (20)     5169 2023-07-10 06:53:03.000000 botiverse-0.3.6/botiverse/bots/deep_TODS/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.232816 botiverse-0.3.6/botiverse/gui/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-07-02 09:46:31.000000 botiverse-0.3.6/botiverse/gui/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1004 2023-07-24 13:02:01.000000 botiverse-0.3.6/botiverse/gui/gui.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.233324 botiverse-0.3.6/botiverse/models/
+-rw-r--r--   0 essam      (501) staff       (20)      559 2023-07-10 23:47:13.000000 botiverse-0.3.6/botiverse/models/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.233674 botiverse-0.3.6/botiverse/preprocessors/
+-rw-r--r--   0 essam      (501) staff       (20)      584 2023-07-24 06:37:23.000000 botiverse-0.3.6/botiverse/preprocessors/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-24 16:40:42.224440 botiverse-0.3.6/botiverse.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-24 16:40:42.000000 botiverse-0.3.6/botiverse.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)     1055 2023-07-24 16:40:42.000000 botiverse-0.3.6/botiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-24 16:40:42.000000 botiverse-0.3.6/botiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-24 16:40:42.000000 botiverse-0.3.6/botiverse.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-24 16:40:42.000000 botiverse-0.3.6/botiverse.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-24 16:40:42.234813 botiverse-0.3.6/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     2440 2023-07-24 16:40:25.000000 botiverse-0.3.6/setup.py
```

### Comparing `botiverse-0.3.5/PKG-INFO` & `botiverse-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.5
+Version: 0.3.6
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `botiverse-0.3.5/botiverse/gui/gui.py` & `botiverse-0.3.6/botiverse/gui/gui.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.5/botiverse/models/__init__.py` & `botiverse-0.3.6/botiverse/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.5/botiverse/preprocessors/__init__.py` & `botiverse-0.3.6/botiverse/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `botiverse-0.3.5/botiverse.egg-info/PKG-INFO` & `botiverse-0.3.6/botiverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.3.5
+Version: 0.3.6
 Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

