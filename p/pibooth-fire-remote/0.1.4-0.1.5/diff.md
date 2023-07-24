# Comparing `tmp/pibooth_fire_remote-0.1.4-py3-none-any.whl.zip` & `tmp/pibooth_fire_remote-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3992 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4016 b- defN 23-Jul-13 19:53 pibooth_fire_remote.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jul-13 20:02 pibooth_fire_remote-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1478 b- defN 23-Jul-13 20:02 pibooth_fire_remote-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 20:02 pibooth_fire_remote-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-13 20:02 pibooth_fire_remote-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-13 20:02 pibooth_fire_remote-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-13 20:02 pibooth_fire_remote-0.1.4.dist-info/RECORD
-7 files, 7357 bytes uncompressed, 2852 bytes compressed:  61.2%
+Zip file size: 4079 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4279 b- defN 23-Jul-24 07:56 pibooth_fire_remote.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1517 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-24 07:57 pibooth_fire_remote-0.1.5.dist-info/RECORD
+7 files, 7659 bytes uncompressed, 2939 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pibooth_fire_remote.py
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.4.dist-info/LICENSE
+Filename: pibooth_fire_remote-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.4.dist-info/METADATA
+Filename: pibooth_fire_remote-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.4.dist-info/WHEEL
+Filename: pibooth_fire_remote-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.4.dist-info/entry_points.txt
+Filename: pibooth_fire_remote-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.4.dist-info/top_level.txt
+Filename: pibooth_fire_remote-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.4.dist-info/RECORD
+Filename: pibooth_fire_remote-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pibooth_fire_remote.py

```diff
@@ -3,30 +3,38 @@
 from evdev import InputDevice, categorize, ecodes
 import pygame
 
 import pibooth
 from pibooth.utils import LOGGER
 
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
+
 
-try:
-    #creates object 'fire tv remote' to store the data
-    dev = InputDevice('/dev/input/event2')
-except FileNotFoundError:
-    LOGGER.warning("Bluetooth device not Found.")
-    dev = None
 
 BUTTONDOWN = pygame.USEREVENT + 1
 
 SECTION = "FIRE-Remote"
 
+
+def get_device(cfg_in):
+    try:
+        # creates object 'fire tv remote' to store the data
+        right = int(cfg_in.get(SECTION, 'device'))
+        dev = InputDevice('/dev/input/event2')
+    except FileNotFoundError:
+        LOGGER.warning("Bluetooth device not Found.")
+        dev = None
+
+    return dev
 @pibooth.hookimpl
 def pibooth_configure(cfg):
     #button code variables (change to suit your device)
+    cfg.add_option(SECTION, 'device', '/dev/input/event2',
+                   "Device Path")
     cfg.add_option(SECTION, 'enterBtn', 96,
                        "Enter Button Code")
     cfg.add_option(SECTION, 'backBtn', 158,
                    "Back Button Code")
     cfg.add_option(SECTION, 'settingsBtn', 139,
                    "Setting Button Code")
     cfg.add_option(SECTION, 'homeBtn', 172,
@@ -45,21 +53,23 @@
                    "Forward Button Code")
     cfg.add_option(SECTION, 'backward', 168,
                    "Backward Button Code")
 
 
 @pibooth.hookimpl
 def pibooth_startup(cfg, app):
+    dev = get_device(cfg)
     if dev is not None:
         th = threading.Thread(target=run_event_monitor, args=(cfg, app))
         th.daemon = True
         th.start()
 
 def run_event_monitor(cfg, app):
     #loop and filter by event code and print the mapped label
+    dev = get_device(cfg)
     if dev is not None:
 
         enterBtn = int(cfg.get(SECTION, 'enterBtn'))
         backBtn = int(cfg.get(SECTION, 'backBtn'))
         settingsBtn = int(cfg.get(SECTION, 'settingsBtn'))
         homeBtn = int(cfg.get(SECTION, 'homeBtn'))
         up = int(cfg.get(SECTION, 'up'))
```

## Comparing `pibooth_fire_remote-0.1.4.dist-info/LICENSE` & `pibooth_fire_remote-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pibooth_fire_remote-0.1.4.dist-info/METADATA` & `pibooth_fire_remote-0.1.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibooth-fire-remote
-Version: 0.1.4
+Version: 0.1.5
 Summary: UNKNOWN
 Home-page: https://github.com/chilipp89/pibooth-qr-download
 Author: P. Junietz
 License: MIT
 Keywords: Raspberry Pi,camera,photobooth,Bluetooth,Remote
 Platform: unix
 Platform: linux
@@ -29,18 +29,22 @@
 # pibooth-fire-remote
 Remote Control with bluetooth Remote
 
 # Install
 pip install pibooth-fire-remote
 
 The default settings are mapped to my fire stick gen 1 remote.
-Map you bluetooth remote using the quick start manual from evdev.
+Map your bluetooth remote using the quick start manual from evdev.
+
+`$ python -m evdev.evtest`
+
 
 ## Configuration
 [FIRE-Remote]
+- device
 - enterBtn
 - backBtn
 - settingsBtn
 - homeBtn
 - up
 - down
 - left
```

## Comparing `pibooth_fire_remote-0.1.4.dist-info/RECORD` & `pibooth_fire_remote-0.1.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pibooth_fire_remote.py,sha256=_UUj5ZurbmkOc6FRVi63cNAg_drkrtOkr7f4vSIhu58,4016
-pibooth_fire_remote-0.1.4.dist-info/LICENSE,sha256=8MhKKX4jcdh7M60uTWf4zk_cdmFXMxHe26HsSJyZphU,1066
-pibooth_fire_remote-0.1.4.dist-info/METADATA,sha256=5-OtZ5MKbqbzJvaBlvo1s9h-Ze3rgkdpWh3hUqE7-Cg,1478
-pibooth_fire_remote-0.1.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pibooth_fire_remote-0.1.4.dist-info/entry_points.txt,sha256=ExheM_w4JJMaMeao7ARgseEwDMsCCzTXD0F170rgR0U,53
-pibooth_fire_remote-0.1.4.dist-info/top_level.txt,sha256=uzVg30QGLIeuYlAgFLl7efJyUgD2uoKL2lOpC9oJGeY,20
-pibooth_fire_remote-0.1.4.dist-info/RECORD,,
+pibooth_fire_remote.py,sha256=hu-f9_c8Mkb3WVjxB3uQP_CZB0dbPP14mhEhvhPiRLg,4279
+pibooth_fire_remote-0.1.5.dist-info/LICENSE,sha256=8MhKKX4jcdh7M60uTWf4zk_cdmFXMxHe26HsSJyZphU,1066
+pibooth_fire_remote-0.1.5.dist-info/METADATA,sha256=cCao2jC-T_YSDYV_jBWtK5B6TNClLX_amA9-t5oHBPU,1517
+pibooth_fire_remote-0.1.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pibooth_fire_remote-0.1.5.dist-info/entry_points.txt,sha256=ExheM_w4JJMaMeao7ARgseEwDMsCCzTXD0F170rgR0U,53
+pibooth_fire_remote-0.1.5.dist-info/top_level.txt,sha256=uzVg30QGLIeuYlAgFLl7efJyUgD2uoKL2lOpC9oJGeY,20
+pibooth_fire_remote-0.1.5.dist-info/RECORD,,
```

