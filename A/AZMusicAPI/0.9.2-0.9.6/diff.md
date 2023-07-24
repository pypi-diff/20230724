# Comparing `tmp/AZMusicAPI-0.9.2.tar.gz` & `tmp/AZMusicAPI-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AZMusicAPI-0.9.2.tar", last modified: Mon Jul 24 09:34:30 2023, max compression
+gzip compressed data, was "AZMusicAPI-0.9.6.tar", last modified: Mon Jul 24 09:45:24 2023, max compression
```

## Comparing `AZMusicAPI-0.9.2.tar` & `AZMusicAPI-0.9.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:34:30.554315 AZMusicAPI-0.9.2/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:34:30.548317 AZMusicAPI-0.9.2/AZMusicAPI.egg-info/
--rw-rw-rw-   0        0        0     1082 2023-07-24 09:34:30.000000 AZMusicAPI-0.9.2/AZMusicAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-07-24 09:34:30.000000 AZMusicAPI-0.9.2/AZMusicAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:34:30.000000 AZMusicAPI-0.9.2/AZMusicAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 09:34:30.000000 AZMusicAPI-0.9.2/AZMusicAPI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 09:34:30.550315 AZMusicAPI-0.9.2/MusicAPI/
--rw-rw-rw-   0        0        0     4486 2023-07-24 03:33:51.000000 AZMusicAPI-0.9.2/MusicAPI/__init__.py
--rw-rw-rw-   0        0        0     1082 2023-07-24 09:34:30.553316 AZMusicAPI-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-24 09:34:30.556317 AZMusicAPI-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      310 2023-07-24 09:34:26.000000 AZMusicAPI-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:24.237579 AZMusicAPI-0.9.6/
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:24.218583 AZMusicAPI-0.9.6/AZMusicAPI/
+-rw-rw-rw-   0        0        0     4486 2023-07-24 03:33:51.000000 AZMusicAPI-0.9.6/AZMusicAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:45:24.226583 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/
+-rw-rw-rw-   0        0        0     1123 2023-07-24 09:45:23.000000 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-07-24 09:45:24.000000 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:45:23.000000 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 09:45:23.000000 AZMusicAPI-0.9.6/AZMusicAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1123 2023-07-24 09:45:24.235597 AZMusicAPI-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:45:24.237579 AZMusicAPI-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      364 2023-07-24 09:45:13.000000 AZMusicAPI-0.9.6/setup.py
```

### Comparing `AZMusicAPI-0.9.2/AZMusicAPI.egg-info/PKG-INFO` & `AZMusicAPI-0.9.6/AZMusicAPI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: AZMusicAPI
-Version: 0.9.2
+Version: 0.9.6
 Summary: Easy access to music information and song audio links
 Author: AZ Studio
+Description-Content-Type: text/markdown
 
 # AZMusicAPI模块使用指南
 
 ```
 getmusic(keyword)
 ```
```

### Comparing `AZMusicAPI-0.9.2/MusicAPI/__init__.py` & `AZMusicAPI-0.9.6/AZMusicAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `AZMusicAPI-0.9.2/PKG-INFO` & `AZMusicAPI-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: AZMusicAPI
-Version: 0.9.2
+Version: 0.9.6
 Summary: Easy access to music information and song audio links
 Author: AZ Studio
+Description-Content-Type: text/markdown
 
 # AZMusicAPI模块使用指南
 
 ```
 getmusic(keyword)
 ```
```

