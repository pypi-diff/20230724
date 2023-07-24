# Comparing `tmp/jac_speech-1.4.1.7.tar.gz` & `tmp/jac_speech-1.4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_speech-1.4.1.7.tar", last modified: Thu Jul 20 04:00:55 2023, max compression
+gzip compressed data, was "jac_speech-1.4.1.8.tar", last modified: Mon Jul 24 16:59:13 2023, max compression
```

## Comparing `jac_speech-1.4.1.7.tar` & `jac_speech-1.4.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.065070 jac_speech-1.4.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-20 04:00:55.065070 jac_speech-1.4.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.061070 jac_speech-1.4.1.7/jac_speech/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.065070 jac_speech-1.4.1.7/jac_speech/stt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/stt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.065070 jac_speech-1.4.1.7/jac_speech/vc_tts/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/vc_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/vc_tts/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/vc_tts/models.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/vc_tts/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.065070 jac_speech-1.4.1.7/jac_speech/vc_tts/text/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/vc_tts/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/vc_tts/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/vc_tts/text/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/jac_speech/vc_tts/vc_tts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.065070 jac_speech-1.4.1.7/jac_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-20 04:00:55.000000 jac_speech-1.4.1.7/jac_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 04:00:55.000000 jac_speech-1.4.1.7/jac_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:00:55.000000 jac_speech-1.4.1.7/jac_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 04:00:55.000000 jac_speech-1.4.1.7/jac_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 04:00:55.000000 jac_speech-1.4.1.7/jac_speech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:00:55.065070 jac_speech-1.4.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-20 04:00:37.000000 jac_speech-1.4.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:13.517391 jac_speech-1.4.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-24 16:59:13.517391 jac_speech-1.4.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:13.513391 jac_speech-1.4.1.8/jac_speech/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:13.517391 jac_speech-1.4.1.8/jac_speech/stt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/stt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:13.517391 jac_speech-1.4.1.8/jac_speech/vc_tts/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/vc_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/vc_tts/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/vc_tts/models.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 16:58:51.000000 jac_speech-1.4.1.8/jac_speech/vc_tts/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:13.517391 jac_speech-1.4.1.8/jac_speech/vc_tts/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 16:58:52.000000 jac_speech-1.4.1.8/jac_speech/vc_tts/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-24 16:58:52.000000 jac_speech-1.4.1.8/jac_speech/vc_tts/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-24 16:58:52.000000 jac_speech-1.4.1.8/jac_speech/vc_tts/text/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-24 16:58:52.000000 jac_speech-1.4.1.8/jac_speech/vc_tts/vc_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:13.517391 jac_speech-1.4.1.8/jac_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-24 16:59:13.000000 jac_speech-1.4.1.8/jac_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 16:59:13.000000 jac_speech-1.4.1.8/jac_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:59:13.000000 jac_speech-1.4.1.8/jac_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-24 16:59:13.000000 jac_speech-1.4.1.8/jac_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 16:59:13.000000 jac_speech-1.4.1.8/jac_speech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:59:13.517391 jac_speech-1.4.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-24 16:58:52.000000 jac_speech-1.4.1.8/setup.py
```

### Comparing `jac_speech-1.4.1.7/README.md` & `jac_speech-1.4.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.7/jac_speech/stt/stt.py` & `jac_speech-1.4.1.8/jac_speech/stt/stt.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.7/jac_speech/vc_tts/action_utils.py` & `jac_speech-1.4.1.8/jac_speech/vc_tts/action_utils.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.7/jac_speech/vc_tts/models.json` & `jac_speech-1.4.1.8/jac_speech/vc_tts/models.json`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.7/jac_speech/vc_tts/text/cleaners.py` & `jac_speech-1.4.1.8/jac_speech/vc_tts/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.7/jac_speech/vc_tts/text/numbers.py` & `jac_speech-1.4.1.8/jac_speech/vc_tts/text/numbers.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.7/jac_speech/vc_tts/vc_tts.py` & `jac_speech-1.4.1.8/jac_speech/vc_tts/vc_tts.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.7/jac_speech.egg-info/SOURCES.txt` & `jac_speech-1.4.1.8/jac_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.7/setup.py` & `jac_speech-1.4.1.8/setup.py`

 * *Files identical despite different names*

