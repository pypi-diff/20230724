# Comparing `tmp/spyc_iot-0.0.6.tar.gz` & `tmp/spyc_iot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyc_iot-0.0.6.tar", last modified: Mon Jul 24 01:51:01 2023, max compression
+gzip compressed data, was "spyc_iot-0.0.7.tar", last modified: Mon Jul 24 05:53:29 2023, max compression
```

## Comparing `spyc_iot-0.0.6.tar` & `spyc_iot-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 01:51:01.259120 spyc_iot-0.0.6/
--rw-rw-rw-   0        0        0     1117 2023-07-24 01:47:07.000000 spyc_iot-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      307 2023-07-24 01:51:01.260117 spyc_iot-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-14 04:24:10.000000 spyc_iot-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      417 2023-07-24 01:51:01.261114 spyc_iot-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 01:51:01.233189 spyc_iot-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 01:51:01.244160 spyc_iot-0.0.6/src/spyc_iot/
--rw-rw-rw-   0        0        0      117 2023-07-24 01:47:43.000000 spyc_iot-0.0.6/src/spyc_iot/__init__.py
--rw-rw-rw-   0        0        0     5897 2023-07-24 01:47:35.000000 spyc_iot-0.0.6/src/spyc_iot/max7219.py
--rw-rw-rw-   0        0        0      667 2023-07-14 05:55:28.000000 spyc_iot-0.0.6/src/spyc_iot/ntp.py
--rw-rw-rw-   0        0        0      233 2023-07-20 05:42:07.000000 spyc_iot-0.0.6/src/spyc_iot/time.py
--rw-rw-rw-   0        0        0      505 2023-07-14 04:50:45.000000 spyc_iot-0.0.6/src/spyc_iot/wifi.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:51:01.259120 spyc_iot-0.0.6/src/spyc_iot.egg-info/
--rw-rw-rw-   0        0        0      307 2023-07-24 01:51:01.000000 spyc_iot-0.0.6/src/spyc_iot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-07-24 01:51:01.000000 spyc_iot-0.0.6/src/spyc_iot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 01:51:01.000000 spyc_iot-0.0.6/src/spyc_iot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 01:51:01.000000 spyc_iot-0.0.6/src/spyc_iot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 05:53:29.357733 spyc_iot-0.0.7/
+-rw-rw-rw-   0        0        0     1117 2023-07-24 01:47:07.000000 spyc_iot-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      307 2023-07-24 05:53:29.357733 spyc_iot-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-14 04:24:10.000000 spyc_iot-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      417 2023-07-24 05:53:29.359750 spyc_iot-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 05:53:29.332798 spyc_iot-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 05:53:29.342771 spyc_iot-0.0.7/src/spyc_iot/
+-rw-rw-rw-   0        0        0      117 2023-07-24 01:47:43.000000 spyc_iot-0.0.7/src/spyc_iot/__init__.py
+-rw-rw-rw-   0        0        0     5911 2023-07-24 04:23:06.000000 spyc_iot-0.0.7/src/spyc_iot/max7219.py
+-rw-rw-rw-   0        0        0      667 2023-07-14 05:55:28.000000 spyc_iot-0.0.7/src/spyc_iot/ntp.py
+-rw-rw-rw-   0        0        0      240 2023-07-24 04:23:07.000000 spyc_iot-0.0.7/src/spyc_iot/time.py
+-rw-rw-rw-   0        0        0      505 2023-07-14 04:50:45.000000 spyc_iot-0.0.7/src/spyc_iot/wifi.py
+drwxrwxrwx   0        0        0        0 2023-07-24 05:53:29.355736 spyc_iot-0.0.7/src/spyc_iot.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-07-24 05:53:29.000000 spyc_iot-0.0.7/src/spyc_iot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-24 05:53:29.000000 spyc_iot-0.0.7/src/spyc_iot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 05:53:29.000000 spyc_iot-0.0.7/src/spyc_iot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 05:53:29.000000 spyc_iot-0.0.7/src/spyc_iot.egg-info/top_level.txt
```

### Comparing `spyc_iot-0.0.6/LICENSE` & `spyc_iot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spyc_iot-0.0.6/src/spyc_iot/max7219.py` & `spyc_iot-0.0.7/src/spyc_iot/max7219.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,14 @@
         digit_index = ord(digit) - 48
         
         if digit_index < 0 or digit_index > 10:
             return
         
         self.byte_sequence(digit_pixels[digit_index], x, y, col)
         
-    def scroll_text(self, msg, refresh_rate):
+    def scroll_text(self, msg, refresh_rate, y, col = 1):
         msg_len = len(msg)
         for x in range(self.num * 8, -msg_len * 8, -1):
-            self.text(msg, x, 0, 1)
+            self.text(msg, x, y, col)
             self.show()
             sleep(1 / refresh_rate)
             self.fill(0)
```

### Comparing `spyc_iot-0.0.6/src/spyc_iot/ntp.py` & `spyc_iot-0.0.7/src/spyc_iot/ntp.py`

 * *Files identical despite different names*

