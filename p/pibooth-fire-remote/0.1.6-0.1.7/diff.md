# Comparing `tmp/pibooth_fire_remote-0.1.6-py3-none-any.whl.zip` & `tmp/pibooth_fire_remote-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4081 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4279 b- defN 23-Jul-24 08:09 pibooth_fire_remote.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1517 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-24 08:09 pibooth_fire_remote-0.1.6.dist-info/RECORD
-7 files, 7659 bytes uncompressed, 2941 bytes compressed:  61.6%
+Zip file size: 4080 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4277 b- defN 23-Jul-24 08:18 pibooth_fire_remote.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-24 08:18 pibooth_fire_remote-0.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1517 b- defN 23-Jul-24 08:18 pibooth_fire_remote-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:18 pibooth_fire_remote-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 08:18 pibooth_fire_remote-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 08:18 pibooth_fire_remote-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-24 08:18 pibooth_fire_remote-0.1.7.dist-info/RECORD
+7 files, 7657 bytes uncompressed, 2940 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pibooth_fire_remote.py
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.6.dist-info/LICENSE
+Filename: pibooth_fire_remote-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.6.dist-info/METADATA
+Filename: pibooth_fire_remote-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.6.dist-info/WHEEL
+Filename: pibooth_fire_remote-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.6.dist-info/entry_points.txt
+Filename: pibooth_fire_remote-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.6.dist-info/top_level.txt
+Filename: pibooth_fire_remote-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.6.dist-info/RECORD
+Filename: pibooth_fire_remote-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pibooth_fire_remote.py

```diff
@@ -3,28 +3,28 @@
 from evdev import InputDevice, categorize, ecodes
 import pygame
 
 import pibooth
 from pibooth.utils import LOGGER
 
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 
 
 BUTTONDOWN = pygame.USEREVENT + 1
 
 SECTION = "FIRE-Remote"
 
 
 def get_device(cfg_in):
     try:
         # creates object 'fire tv remote' to store the data
-        right = str(cfg_in.get(SECTION, 'device'))
-        dev = InputDevice('/dev/input/event2')
+        device_name = str(cfg_in.get(SECTION, 'device'))
+        dev = InputDevice(device_name)
     except FileNotFoundError:
         LOGGER.warning("Bluetooth device not Found.")
         dev = None
 
     return dev
 @pibooth.hookimpl
 def pibooth_configure(cfg):
```

## Comparing `pibooth_fire_remote-0.1.6.dist-info/LICENSE` & `pibooth_fire_remote-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pibooth_fire_remote-0.1.6.dist-info/METADATA` & `pibooth_fire_remote-0.1.7.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibooth-fire-remote
-Version: 0.1.6
+Version: 0.1.7
 Summary: UNKNOWN
 Home-page: https://github.com/chilipp89/pibooth-qr-download
 Author: P. Junietz
 License: MIT
 Keywords: Raspberry Pi,camera,photobooth,Bluetooth,Remote
 Platform: unix
 Platform: linux
```

## Comparing `pibooth_fire_remote-0.1.6.dist-info/RECORD` & `pibooth_fire_remote-0.1.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pibooth_fire_remote.py,sha256=y5qL-KKoFjPMzIo0cjN8HAbtgOkfUYZqC1y73m9L_qo,4279
-pibooth_fire_remote-0.1.6.dist-info/LICENSE,sha256=8MhKKX4jcdh7M60uTWf4zk_cdmFXMxHe26HsSJyZphU,1066
-pibooth_fire_remote-0.1.6.dist-info/METADATA,sha256=O0-ZezACEwZFti2CToUhbGQJWqLUZzuAxai4XsCaLnM,1517
-pibooth_fire_remote-0.1.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pibooth_fire_remote-0.1.6.dist-info/entry_points.txt,sha256=ExheM_w4JJMaMeao7ARgseEwDMsCCzTXD0F170rgR0U,53
-pibooth_fire_remote-0.1.6.dist-info/top_level.txt,sha256=uzVg30QGLIeuYlAgFLl7efJyUgD2uoKL2lOpC9oJGeY,20
-pibooth_fire_remote-0.1.6.dist-info/RECORD,,
+pibooth_fire_remote.py,sha256=9V5sMXzaJkgA7D0VGYplbbabURFFQ7Wwi4dIEhlS19M,4277
+pibooth_fire_remote-0.1.7.dist-info/LICENSE,sha256=8MhKKX4jcdh7M60uTWf4zk_cdmFXMxHe26HsSJyZphU,1066
+pibooth_fire_remote-0.1.7.dist-info/METADATA,sha256=r09MlwlSowqc3cAGWHPXvt3TU6NxjnQXPbp36jQgtrM,1517
+pibooth_fire_remote-0.1.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pibooth_fire_remote-0.1.7.dist-info/entry_points.txt,sha256=ExheM_w4JJMaMeao7ARgseEwDMsCCzTXD0F170rgR0U,53
+pibooth_fire_remote-0.1.7.dist-info/top_level.txt,sha256=uzVg30QGLIeuYlAgFLl7efJyUgD2uoKL2lOpC9oJGeY,20
+pibooth_fire_remote-0.1.7.dist-info/RECORD,,
```

