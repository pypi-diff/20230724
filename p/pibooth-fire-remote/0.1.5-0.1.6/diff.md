# Comparing `tmp/pibooth_fire_remote-0.1.5-py3-none-any.whl.zip` & `tmp/pibooth_fire_remote-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4079 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4279 b- defN 23-Jul-24 07:56 pibooth_fire_remote.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1517 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/RECORD
-7 files, 7659 bytes uncompressed, 2939 bytes compressed:  61.6%
+Zip file size: 4081 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4279 b- defN 23-Jul-24 08:09 pibooth_fire_remote.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1517 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/RECORD
+7 files, 7659 bytes uncompressed, 2941 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pibooth_fire_remote.py
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.5.dist-info/LICENSE
+Filename: pibooth_fire_remote-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.5.dist-info/METADATA
+Filename: pibooth_fire_remote-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.5.dist-info/WHEEL
+Filename: pibooth_fire_remote-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.5.dist-info/entry_points.txt
+Filename: pibooth_fire_remote-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.5.dist-info/top_level.txt
+Filename: pibooth_fire_remote-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.5.dist-info/RECORD
+Filename: pibooth_fire_remote-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pibooth_fire_remote.py

```diff
@@ -3,27 +3,27 @@
 from evdev import InputDevice, categorize, ecodes
 import pygame
 
 import pibooth
 from pibooth.utils import LOGGER
 
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 
 
 BUTTONDOWN = pygame.USEREVENT + 1
 
 SECTION = "FIRE-Remote"
 
 
 def get_device(cfg_in):
     try:
         # creates object 'fire tv remote' to store the data
-        right = int(cfg_in.get(SECTION, 'device'))
+        right = str(cfg_in.get(SECTION, 'device'))
         dev = InputDevice('/dev/input/event2')
     except FileNotFoundError:
         LOGGER.warning("Bluetooth device not Found.")
         dev = None
 
     return dev
 @pibooth.hookimpl
```

## Comparing `pibooth_fire_remote-0.1.5.dist-info/LICENSE` & `pibooth_fire_remote-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pibooth_fire_remote-0.1.5.dist-info/METADATA` & `pibooth_fire_remote-0.1.6.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibooth-fire-remote
-Version: 0.1.5
+Version: 0.1.6
 Summary: UNKNOWN
 Home-page: https://github.com/chilipp89/pibooth-qr-download
 Author: P. Junietz
 License: MIT
 Keywords: Raspberry Pi,camera,photobooth,Bluetooth,Remote
 Platform: unix
 Platform: linux
```

