# Comparing `tmp/pibooth_fire_remote-0.1.8-py3-none-any.whl.zip` & `tmp/pibooth_fire_remote-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4164 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4741 b- defN 23-Jul-24 08:29 pibooth_fire_remote.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jul-24 08:30 pibooth_fire_remote-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1539 b- defN 23-Jul-24 08:30 pibooth_fire_remote-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:30 pibooth_fire_remote-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 08:30 pibooth_fire_remote-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 08:30 pibooth_fire_remote-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-24 08:30 pibooth_fire_remote-0.1.8.dist-info/RECORD
-7 files, 8143 bytes uncompressed, 3024 bytes compressed:  62.9%
+Zip file size: 4193 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4830 b- defN 23-Jul-24 08:43 pibooth_fire_remote.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1539 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/RECORD
+7 files, 8232 bytes uncompressed, 3053 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pibooth_fire_remote.py
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.8.dist-info/LICENSE
+Filename: pibooth_fire_remote-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.8.dist-info/METADATA
+Filename: pibooth_fire_remote-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.8.dist-info/WHEEL
+Filename: pibooth_fire_remote-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.8.dist-info/entry_points.txt
+Filename: pibooth_fire_remote-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.8.dist-info/top_level.txt
+Filename: pibooth_fire_remote-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.8.dist-info/RECORD
+Filename: pibooth_fire_remote-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pibooth_fire_remote.py

```diff
@@ -7,15 +7,15 @@
 
 keyboard = Controller()
 
 import pibooth
 from pibooth.utils import LOGGER
 
 
-__version__ = "0.1.8"
+__version__ = "0.2.0"
 
 
 
 BUTTONDOWN = pygame.USEREVENT + 1
 
 SECTION = "FIRE-Remote"
 
@@ -31,36 +31,36 @@
 
     return dev
 @pibooth.hookimpl
 def pibooth_configure(cfg):
     #button code variables (change to suit your device)
     cfg.add_option(SECTION, 'device', '/dev/input/event2',
                    "Device Path")
-    cfg.add_option(SECTION, 'enterBtn', 96,
-                       "Enter Button Code")
-    cfg.add_option(SECTION, 'backBtn', 158,
-                   "Back Button Code")
+    cfg.add_option(SECTION, 'pictureBtn', 96,
+                       "pictureBtn Button Code")
+    # cfg.add_option(SECTION, 'backBtn', 158,
+    #                "Back Button Code")
     cfg.add_option(SECTION, 'settingsBtn', 139,
                    "Setting Button Code")
-    cfg.add_option(SECTION, 'homeBtn', 172,
-                   "Home Button Code")
-    cfg.add_option(SECTION, 'up', 103,
-                   "Up Button Code")
-    cfg.add_option(SECTION, 'down', 108,
-                   "Down Button Code")
+    # cfg.add_option(SECTION, 'homeBtn', 172,
+    #                "Home Button Code")
+    # cfg.add_option(SECTION, 'up', 103,
+    #                "Up Button Code")
+    # cfg.add_option(SECTION, 'down', 108,
+    #                "Down Button Code")
     cfg.add_option(SECTION, 'left', 105,
                    "Left Button Code")
     cfg.add_option(SECTION, 'right', 106,
                    "Right Button Code")
-    cfg.add_option(SECTION, 'playpause', 164,
-                   "Play Button Code")
-    cfg.add_option(SECTION, 'forward', 208,
-                   "Forward Button Code")
-    cfg.add_option(SECTION, 'backward', 168,
-                   "Backward Button Code")
+    # cfg.add_option(SECTION, 'playpause', 164,
+    #                "Play Button Code")
+    cfg.add_option(SECTION, 'printBtn', 208,
+                   "printBtn Button Code")
+    # cfg.add_option(SECTION, 'backward', 168,
+    #                "Backward Button Code")
 
 
 @pibooth.hookimpl
 def pibooth_startup(cfg, app):
     dev = get_device(cfg)
     if dev is not None:
         th = threading.Thread(target=run_event_monitor, args=(cfg, app))
@@ -68,60 +68,60 @@
         th.start()
 
 def run_event_monitor(cfg, app):
     #loop and filter by event code and print the mapped label
     dev = get_device(cfg)
     if dev is not None:
 
-        enterBtn = int(cfg.get(SECTION, 'enterBtn'))
-        backBtn = int(cfg.get(SECTION, 'backBtn'))
+        pictureBtn = int(cfg.get(SECTION, 'pictureBtn'))
+        # backBtn = int(cfg.get(SECTION, 'backBtn'))
         settingsBtn = int(cfg.get(SECTION, 'settingsBtn'))
-        homeBtn = int(cfg.get(SECTION, 'homeBtn'))
-        up = int(cfg.get(SECTION, 'up'))
-        down = int(cfg.get(SECTION, 'down'))
+        # homeBtn = int(cfg.get(SECTION, 'homeBtn'))
+        # up = int(cfg.get(SECTION, 'up'))
+        # down = int(cfg.get(SECTION, 'down'))
         left = int(cfg.get(SECTION, 'left'))
         right = int(cfg.get(SECTION, 'right'))
-        playpause = int(cfg.get(SECTION, 'playpause'))
-        forward = int(cfg.get(SECTION, 'forward'))
-        backward = int(cfg.get(SECTION, 'backward'))
+        # playpause = int(cfg.get(SECTION, 'playpause'))
+        printBtn = int(cfg.get(SECTION, 'printBtn'))
+        # backward = int(cfg.get(SECTION, 'backward'))
 
         for event in dev.read_loop():
 
             if event.type == ecodes.EV_KEY and hasattr(event, "code"):
                 if event.value == 1:
-                    if event.code == enterBtn:
+                    if event.code == pictureBtn:
                         pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=1, printer=0,
                                                    button=app.buttons.capture))
 
-                        LOGGER.info("enterBtn")
+                        LOGGER.info("pictureBtn")
                     elif event.code == settingsBtn:
                         pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=1, printer=1,
                                                              button=app.buttons))
                         LOGGER.info("settingsBtn")
-                    if event.code == homeBtn:
-                        LOGGER.info("homeBtn")
-                    elif event.code == backBtn:
-                        LOGGER.info("backBtn")
-                    elif event.code == playpause:
-                        LOGGER.info("Play/Pause")
-                    elif event.code == up:
-                        keyboard.press(Key.up)
-                        keyboard.release(Key.up)
-                        LOGGER.info("up")
-                    elif event.code == down:
-                        keyboard.press(Key.up)
-                        keyboard.release(Key.up)
-                        LOGGER.info("down")
+                    # if event.code == homeBtn:
+                    #     LOGGER.info("homeBtn")
+                    # elif event.code == backBtn:
+                    #     LOGGER.info("backBtn")
+                    # elif event.code == playpause:
+                    #     LOGGER.info("Play/Pause")
+                    # elif event.code == up:
+                    #     keyboard.press(Key.up)
+                    #     keyboard.release(Key.up)
+                    #     LOGGER.info("up")
+                    # elif event.code == down:
+                    #     keyboard.press(Key.up)
+                    #     keyboard.release(Key.up)
+                    #     LOGGER.info("down")
                     elif event.code == left:
                         keyboard.press(Key.left)
                         keyboard.release(Key.left)
                         LOGGER.info("left")
                     elif event.code == right:
                         keyboard.press(Key.right)
                         keyboard.release(Key.right)
                         LOGGER.info("right")
-                    elif event.code == forward:
+                    elif event.code == printBtn:
                         pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=0, printer=1,
                                                              button=app.buttons.printer))
-                        LOGGER.info("forward")
-                    elif event.code == backward:
-                        LOGGER.info("backward")
+                        LOGGER.info("printBtn")
+                    # elif event.code == backward:
+                    #     LOGGER.info("backward")
```

## Comparing `pibooth_fire_remote-0.1.8.dist-info/LICENSE` & `pibooth_fire_remote-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pibooth_fire_remote-0.1.8.dist-info/METADATA` & `pibooth_fire_remote-0.2.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibooth-fire-remote
-Version: 0.1.8
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: https://github.com/chilipp89/pibooth-qr-download
 Author: P. Junietz
 License: MIT
 Keywords: Raspberry Pi,camera,photobooth,Bluetooth,Remote
 Platform: unix
 Platform: linux
```

