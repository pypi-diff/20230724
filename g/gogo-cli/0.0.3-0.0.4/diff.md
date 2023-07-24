# Comparing `tmp/gogo_cli-0.0.3.tar.gz` & `tmp/gogo_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogo_cli-0.0.3.tar", max compression
+gzip compressed data, was "gogo_cli-0.0.4.tar", max compression
```

## Comparing `gogo_cli-0.0.3.tar` & `gogo_cli-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/LICENSE
--rw-r--r--   0        0        0        0 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/__init__.py
--rw-r--r--   0        0        0      114 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/__main__.py
--rw-r--r--   0        0        0     2894 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/core/__gogo_cli__.py
--rw-r--r--   0        0        0        0 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/core/__version__.py
--rw-r--r--   0        0        0      743 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/core/utils/__downloader__.py
--rw-r--r--   0        0        0        0 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/core/utils/__init__.py
--rw-r--r--   0        0        0      744 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/core/utils/__menu__.py
--rw-r--r--   0        0        0     1054 2023-07-23 19:20:41.719353 gogo_cli-0.0.3/gogo_cli/core/utils/__player__.py
--rw-r--r--   0        0        0      456 2023-07-23 19:20:41.723353 gogo_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 19:20:41.723353 gogo_cli-0.0.3/readme.txt
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 gogo_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/__main__.py
+-rw-r--r--   0        0        0     2894 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/__gogo_cli__.py
+-rw-r--r--   0        0        0        0 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/__version__.py
+-rw-r--r--   0        0        0       69 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__cast__.py
+-rw-r--r--   0        0        0      743 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__downloader__.py
+-rw-r--r--   0        0        0        0 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__menu__.py
+-rw-r--r--   0        0        0     1054 2023-07-24 08:13:12.189700 gogo_cli-0.0.4/gogo_cli/core/utils/__player__.py
+-rw-r--r--   0        0        0      473 2023-07-24 08:13:12.193700 gogo_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 08:13:12.193700 gogo_cli-0.0.4/readme.txt
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 gogo_cli-0.0.4/PKG-INFO
```

### Comparing `gogo_cli-0.0.3/LICENSE` & `gogo_cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.3/gogo_cli/core/__gogo_cli__.py` & `gogo_cli-0.0.4/gogo_cli/core/__gogo_cli__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.3/gogo_cli/core/utils/__downloader__.py` & `gogo_cli-0.0.4/gogo_cli/core/utils/__downloader__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.3/gogo_cli/core/utils/__menu__.py` & `gogo_cli-0.0.4/gogo_cli/core/utils/__menu__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from .__player__ import play as pl
 from .__downloader__ import download as dl
+from .__cast__ import open_cast
 
 import os
 
 def menu(url, referrer, anime, episode):
     while True:
         os.system('clear')
-        print("\n1. Play\n2. Download\n3. Replay episode\n4. Play next episode\n5. Quit\n")
+        print("\n1. Play\n2. Download\n3. Replay episode\n4. Play next episode\n5. Cast to a chromecast device\n6. Quit\n")
         e = int(input(": "))
         if e == 1:
             pl(url, referrer, anime, episode)
         elif e == 2:
             dl(anime, url, referrer, episode)
         elif e == 3:
             pl(url, referrer, anime, episode)
         elif e == 4:
             from ..__gogo_cli__ import play
             playNext = 1
             play(anime, episode, playNext)
         elif e == 5:
+            open_cast(url)
+        elif e == 6:
             exit(0)
         else:
             print("[!] Invalid option")
             exit(1)
```

### Comparing `gogo_cli-0.0.3/gogo_cli/core/utils/__player__.py` & `gogo_cli-0.0.4/gogo_cli/core/utils/__player__.py`

 * *Files identical despite different names*

