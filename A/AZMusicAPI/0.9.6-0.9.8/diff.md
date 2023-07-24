# Comparing `tmp/AZMusicAPI-0.9.6.tar.gz` & `tmp/AZMusicAPI-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AZMusicAPI-0.9.6.tar", last modified: Mon Jul 24 09:45:24 2023, max compression
+gzip compressed data, was "AZMusicAPI-0.9.8.tar", last modified: Mon Jul 24 11:37:00 2023, max compression
```

## Comparing `AZMusicAPI-0.9.6.tar` & `AZMusicAPI-0.9.8.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:45:24.237579 AZMusicAPI-0.9.6/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:45:24.218583 AZMusicAPI-0.9.6/AZMusicAPI/
--rw-rw-rw-   0        0        0     4486 2023-07-24 03:33:51.000000 AZMusicAPI-0.9.6/AZMusicAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:45:24.226583 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/
--rw-rw-rw-   0        0        0     1123 2023-07-24 09:45:23.000000 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-07-24 09:45:24.000000 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:45:23.000000 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 09:45:23.000000 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1123 2023-07-24 09:45:24.235597 AZMusicAPI-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-24 09:45:24.237579 AZMusicAPI-0.9.6/setup.cfg
--rw-rw-rw-   0        0        0      364 2023-07-24 09:45:13.000000 AZMusicAPI-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:37:00.419615 AZMusicAPI-0.9.8/
+drwxrwxrwx   0        0        0        0 2023-07-24 11:37:00.391283 AZMusicAPI-0.9.8/AZMusicAPI/
+-rw-rw-rw-   0        0        0     4486 2023-07-24 03:33:51.000000 AZMusicAPI-0.9.8/AZMusicAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:37:00.413332 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/
+-rw-rw-rw-   0        0        0     1526 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1526 2023-07-24 11:37:00.417374 AZMusicAPI-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-24 11:37:00.419615 AZMusicAPI-0.9.8/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-24 11:36:47.000000 AZMusicAPI-0.9.8/setup.py
```

### Comparing `AZMusicAPI-0.9.6/AZMusicAPI/__init__.py` & `AZMusicAPI-0.9.8/AZMusicAPI/__init__.py`

 * *Files identical despite different names*

