# Comparing `tmp/ezshare-0.0.8.tar.gz` & `tmp/ezshare-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezshare-0.0.8.tar", last modified: Thu Jul 28 11:40:48 2022, max compression
+gzip compressed data, was "ezshare-0.0.9.tar", last modified: Thu Jul 28 12:12:17 2022, max compression
```

## Comparing `ezshare-0.0.8.tar` & `ezshare-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 necromant  (1000) necromant  (1000)        0 2022-07-28 11:40:48.892368 ezshare-0.0.8/
--rw-r--r--   0 necromant  (1000) necromant  (1000)      471 2022-07-28 11:12:16.000000 ezshare-0.0.8/LICENSE.TXT
--rw-r--r--   0 necromant  (1000) necromant  (1000)     8665 2022-07-28 11:40:48.892368 ezshare-0.0.8/PKG-INFO
--rw-r--r--   0 necromant  (1000) necromant  (1000)     7528 2022-07-28 11:08:19.000000 ezshare-0.0.8/README.md
-drwxr-xr-x   0 necromant  (1000) necromant  (1000)        0 2022-07-28 11:40:48.892368 ezshare-0.0.8/ezshare/
--rw-r--r--   0 necromant  (1000) necromant  (1000)     5891 2022-07-27 14:40:23.000000 ezshare-0.0.8/ezshare/__main__.py
-drwxr-xr-x   0 necromant  (1000) necromant  (1000)        0 2022-07-28 11:40:48.892368 ezshare-0.0.8/ezshare.egg-info/
--rw-r--r--   0 necromant  (1000) necromant  (1000)     8665 2022-07-28 11:40:48.000000 ezshare-0.0.8/ezshare.egg-info/PKG-INFO
--rw-r--r--   0 necromant  (1000) necromant  (1000)      244 2022-07-28 11:40:48.000000 ezshare-0.0.8/ezshare.egg-info/SOURCES.txt
--rw-r--r--   0 necromant  (1000) necromant  (1000)        1 2022-07-28 11:40:48.000000 ezshare-0.0.8/ezshare.egg-info/dependency_links.txt
--rw-r--r--   0 necromant  (1000) necromant  (1000)       54 2022-07-28 11:40:48.000000 ezshare-0.0.8/ezshare.egg-info/entry_points.txt
--rw-r--r--   0 necromant  (1000) necromant  (1000)       44 2022-07-28 11:40:48.000000 ezshare-0.0.8/ezshare.egg-info/requires.txt
--rw-r--r--   0 necromant  (1000) necromant  (1000)        8 2022-07-28 11:40:48.000000 ezshare-0.0.8/ezshare.egg-info/top_level.txt
--rw-r--r--   0 necromant  (1000) necromant  (1000)      852 2022-07-28 11:40:43.000000 ezshare-0.0.8/pyproject.toml
--rw-r--r--   0 necromant  (1000) necromant  (1000)       38 2022-07-28 11:40:48.892368 ezshare-0.0.8/setup.cfg
+drwxr-xr-x   0 necromant  (1000) necromant  (1000)        0 2022-07-28 12:12:17.050258 ezshare-0.0.9/
+-rw-r--r--   0 necromant  (1000) necromant  (1000)      471 2022-07-28 11:12:16.000000 ezshare-0.0.9/LICENSE.TXT
+-rw-r--r--   0 necromant  (1000) necromant  (1000)     8787 2022-07-28 12:12:17.050258 ezshare-0.0.9/PKG-INFO
+-rw-r--r--   0 necromant  (1000) necromant  (1000)     7650 2022-07-28 12:11:09.000000 ezshare-0.0.9/README.md
+drwxr-xr-x   0 necromant  (1000) necromant  (1000)        0 2022-07-28 12:12:17.050258 ezshare-0.0.9/ezshare/
+-rw-r--r--   0 necromant  (1000) necromant  (1000)     5891 2022-07-27 14:40:23.000000 ezshare-0.0.9/ezshare/__main__.py
+drwxr-xr-x   0 necromant  (1000) necromant  (1000)        0 2022-07-28 12:12:17.050258 ezshare-0.0.9/ezshare.egg-info/
+-rw-r--r--   0 necromant  (1000) necromant  (1000)     8787 2022-07-28 12:12:17.000000 ezshare-0.0.9/ezshare.egg-info/PKG-INFO
+-rw-r--r--   0 necromant  (1000) necromant  (1000)      244 2022-07-28 12:12:17.000000 ezshare-0.0.9/ezshare.egg-info/SOURCES.txt
+-rw-r--r--   0 necromant  (1000) necromant  (1000)        1 2022-07-28 12:12:17.000000 ezshare-0.0.9/ezshare.egg-info/dependency_links.txt
+-rw-r--r--   0 necromant  (1000) necromant  (1000)       54 2022-07-28 12:12:17.000000 ezshare-0.0.9/ezshare.egg-info/entry_points.txt
+-rw-r--r--   0 necromant  (1000) necromant  (1000)       44 2022-07-28 12:12:17.000000 ezshare-0.0.9/ezshare.egg-info/requires.txt
+-rw-r--r--   0 necromant  (1000) necromant  (1000)        8 2022-07-28 12:12:17.000000 ezshare-0.0.9/ezshare.egg-info/top_level.txt
+-rw-r--r--   0 necromant  (1000) necromant  (1000)      852 2022-07-28 12:12:11.000000 ezshare-0.0.9/pyproject.toml
+-rw-r--r--   0 necromant  (1000) necromant  (1000)       38 2022-07-28 12:12:17.050258 ezshare-0.0.9/setup.cfg
```

### Comparing `ezshare-0.0.8/PKG-INFO` & `ezshare-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezshare
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple library and commandline tool to access EzShare WiFi SD Cards
 Author-email: Andrew 'Necromant' Andrianov <andrew@ncrmnt.org>
 License:  DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                             Version 2, December 2004
         
          Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
         
@@ -25,14 +25,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # What is it?
 
 A python library and commandline tool to access and sync data from a ezShare WIFI SD Card.
 
+[![asciicast](https://asciinema.org/a/R7jcHXTVy1rP97TQdyQfSFwf8.svg)](https://asciinema.org/a/R7jcHXTVy1rP97TQdyQfSFwf8)
+
 
 # How to install?
 
 ```
     pip install ezshare
 ```
```

### Comparing `ezshare-0.0.8/README.md` & `ezshare-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # What is it?
 
 A python library and commandline tool to access and sync data from a ezShare WIFI SD Card.
 
+[![asciicast](https://asciinema.org/a/R7jcHXTVy1rP97TQdyQfSFwf8.svg)](https://asciinema.org/a/R7jcHXTVy1rP97TQdyQfSFwf8)
+
 
 # How to install?
 
 ```
     pip install ezshare
 ```
```

### Comparing `ezshare-0.0.8/ezshare/__main__.py` & `ezshare-0.0.9/ezshare/__main__.py`

 * *Files identical despite different names*

### Comparing `ezshare-0.0.8/ezshare.egg-info/PKG-INFO` & `ezshare-0.0.9/ezshare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezshare
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple library and commandline tool to access EzShare WiFi SD Cards
 Author-email: Andrew 'Necromant' Andrianov <andrew@ncrmnt.org>
 License:  DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                             Version 2, December 2004
         
          Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
         
@@ -25,14 +25,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # What is it?
 
 A python library and commandline tool to access and sync data from a ezShare WIFI SD Card.
 
+[![asciicast](https://asciinema.org/a/R7jcHXTVy1rP97TQdyQfSFwf8.svg)](https://asciinema.org/a/R7jcHXTVy1rP97TQdyQfSFwf8)
+
 
 # How to install?
 
 ```
     pip install ezshare
 ```
```

### Comparing `ezshare-0.0.8/pyproject.toml` & `ezshare-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ezshare"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Andrew 'Necromant' Andrianov", email="andrew@ncrmnt.org" },
 ]
 description = "A simple library and commandline tool to access EzShare WiFi SD Cards"
 readme = "README.md"
 license = { file="LICENSE.TXT" }
 requires-python = ">=3.7"
```

