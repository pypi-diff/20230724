# Comparing `tmp/yanhui_text2speech-0.1.tar.gz` & `tmp/yanhui_text2speech-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanhui_text2speech-0.1.tar", last modified: Mon Jul 24 04:06:07 2023, max compression
+gzip compressed data, was "yanhui_text2speech-0.2.tar", last modified: Mon Jul 24 06:56:15 2023, max compression
```

## Comparing `yanhui_text2speech-0.1.tar` & `yanhui_text2speech-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:06:07.821374 yanhui_text2speech-0.1/
--rw-r--r--   0 root         (0) root         (0)      213 2023-07-24 04:06:07.821374 yanhui_text2speech-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 04:06:07.821374 yanhui_text2speech-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      286 2023-07-24 04:05:23.000000 yanhui_text2speech-0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:06:07.820374 yanhui_text2speech-0.1/yanhui_text2speech/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 04:05:38.000000 yanhui_text2speech-0.1/yanhui_text2speech/__init__.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-07-24 04:02:05.000000 yanhui_text2speech-0.1/yanhui_text2speech/yanhui_txt2speech.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:06:07.820374 yanhui_text2speech-0.1/yanhui_text2speech.egg-info/
--rw-r--r--   0 root         (0) root         (0)      213 2023-07-24 04:06:07.000000 yanhui_text2speech-0.1/yanhui_text2speech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      288 2023-07-24 04:06:07.000000 yanhui_text2speech-0.1/yanhui_text2speech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 04:06:07.000000 yanhui_text2speech-0.1/yanhui_text2speech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-24 04:06:07.000000 yanhui_text2speech-0.1/yanhui_text2speech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 04:06:07.000000 yanhui_text2speech-0.1/yanhui_text2speech.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 06:56:15.932646 yanhui_text2speech-0.2/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-24 06:56:15.932646 yanhui_text2speech-0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 06:56:15.932646 yanhui_text2speech-0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-24 06:54:20.000000 yanhui_text2speech-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 06:56:15.932646 yanhui_text2speech-0.2/yanhui_text2speech/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 04:05:38.000000 yanhui_text2speech-0.2/yanhui_text2speech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      471 2023-07-24 06:45:39.000000 yanhui_text2speech-0.2/yanhui_text2speech/yanhui_txt2speech.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 06:56:15.932646 yanhui_text2speech-0.2/yanhui_text2speech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-24 06:56:15.000000 yanhui_text2speech-0.2/yanhui_text2speech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      288 2023-07-24 06:56:15.000000 yanhui_text2speech-0.2/yanhui_text2speech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 06:56:15.000000 yanhui_text2speech-0.2/yanhui_text2speech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-24 06:56:15.000000 yanhui_text2speech-0.2/yanhui_text2speech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 06:56:15.000000 yanhui_text2speech-0.2/yanhui_text2speech.egg-info/top_level.txt
```

