# Comparing `tmp/gogo_cli-0.0.5.tar.gz` & `tmp/gogo_cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogo_cli-0.0.5.tar", max compression
+gzip compressed data, was "gogo_cli-0.0.6.tar", max compression
```

## Comparing `gogo_cli-0.0.5.tar` & `gogo_cli-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/LICENSE
--rw-r--r--   0        0        0        0 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/__init__.py
--rw-r--r--   0        0        0      114 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/__main__.py
--rw-r--r--   0        0        0     2894 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/__gogo_cli__.py
--rw-r--r--   0        0        0        0 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/__version__.py
--rw-r--r--   0        0        0      251 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__cast__.py
--rw-r--r--   0        0        0      743 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__downloader__.py
--rw-r--r--   0        0        0        0 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__init__.py
--rw-r--r--   0        0        0      856 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__menu__.py
--rw-r--r--   0        0        0     1054 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/gogo_cli/core/utils/__player__.py
--rw-r--r--   0        0        0      459 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 14:02:01.597474 gogo_cli-0.0.5/readme.txt
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/__main__.py
+-rw-r--r--   0        0        0     2894 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/__gogo_cli__.py
+-rw-r--r--   0        0        0        0 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/__version__.py
+-rw-r--r--   0        0        0      251 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__cast__.py
+-rw-r--r--   0        0        0      743 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__downloader__.py
+-rw-r--r--   0        0        0        0 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0      981 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__menu__.py
+-rw-r--r--   0        0        0     1054 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/gogo_cli/core/utils/__player__.py
+-rw-r--r--   0        0        0      459 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 18:23:29.321226 gogo_cli-0.0.6/readme.txt
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.0.6/PKG-INFO
```

### Comparing `gogo_cli-0.0.5/LICENSE` & `gogo_cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.5/gogo_cli/core/__gogo_cli__.py` & `gogo_cli-0.0.6/gogo_cli/core/__gogo_cli__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.5/gogo_cli/core/utils/__downloader__.py` & `gogo_cli-0.0.6/gogo_cli/core/utils/__downloader__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.5/gogo_cli/core/utils/__menu__.py` & `gogo_cli-0.0.6/gogo_cli/core/utils/__menu__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+import platform
+
 from .__player__ import play as pl
 from .__downloader__ import download as dl
 from .__cast__ import open_cast
 
 import os
 
 def menu(url, referrer, anime, episode):
     while True:
-        os.system('clear')
+        plt = platform.system()
+        if plt == "Windows":
+            os.system("cls")
+        else:
+            os.system('clear')
         print("\n1. Play\n2. Download\n3. Replay episode\n4. Play next episode\n5. Cast to a chromecast device\n6. Quit\n")
         e = int(input(": "))
         if e == 1:
             pl(url, referrer, anime, episode)
         elif e == 2:
             dl(anime, url, referrer, episode)
         elif e == 3:
```

### Comparing `gogo_cli-0.0.5/gogo_cli/core/utils/__player__.py` & `gogo_cli-0.0.6/gogo_cli/core/utils/__player__.py`

 * *Files identical despite different names*

