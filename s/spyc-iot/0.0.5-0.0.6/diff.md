# Comparing `tmp/spyc_iot-0.0.5.tar.gz` & `tmp/spyc_iot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyc_iot-0.0.5.tar", last modified: Thu Jul 20 05:43:21 2023, max compression
+gzip compressed data, was "spyc_iot-0.0.6.tar", last modified: Mon Jul 24 01:51:01 2023, max compression
```

## Comparing `spyc_iot-0.0.5.tar` & `spyc_iot-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 05:43:21.923238 spyc_iot-0.0.5/
--rw-rw-rw-   0        0        0     1072 2023-07-14 04:21:51.000000 spyc_iot-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      307 2023-07-20 05:43:21.923238 spyc_iot-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-14 04:24:10.000000 spyc_iot-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      417 2023-07-20 05:43:21.924236 spyc_iot-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-20 05:43:21.906285 spyc_iot-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 05:43:21.912268 spyc_iot-0.0.5/src/spyc_iot/
--rw-rw-rw-   0        0        0       93 2023-07-20 03:36:28.000000 spyc_iot-0.0.5/src/spyc_iot/__init__.py
--rw-rw-rw-   0        0        0      667 2023-07-14 05:55:28.000000 spyc_iot-0.0.5/src/spyc_iot/ntp.py
--rw-rw-rw-   0        0        0      233 2023-07-20 05:42:07.000000 spyc_iot-0.0.5/src/spyc_iot/time.py
--rw-rw-rw-   0        0        0      505 2023-07-14 04:50:45.000000 spyc_iot-0.0.5/src/spyc_iot/wifi.py
-drwxrwxrwx   0        0        0        0 2023-07-20 05:43:21.922242 spyc_iot-0.0.5/src/spyc_iot.egg-info/
--rw-rw-rw-   0        0        0      307 2023-07-20 05:43:21.000000 spyc_iot-0.0.5/src/spyc_iot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-07-20 05:43:21.000000 spyc_iot-0.0.5/src/spyc_iot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 05:43:21.000000 spyc_iot-0.0.5/src/spyc_iot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 05:43:21.000000 spyc_iot-0.0.5/src/spyc_iot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 01:51:01.259120 spyc_iot-0.0.6/
+-rw-rw-rw-   0        0        0     1117 2023-07-24 01:47:07.000000 spyc_iot-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      307 2023-07-24 01:51:01.260117 spyc_iot-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-14 04:24:10.000000 spyc_iot-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      417 2023-07-24 01:51:01.261114 spyc_iot-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 01:51:01.233189 spyc_iot-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 01:51:01.244160 spyc_iot-0.0.6/src/spyc_iot/
+-rw-rw-rw-   0        0        0      117 2023-07-24 01:47:43.000000 spyc_iot-0.0.6/src/spyc_iot/__init__.py
+-rw-rw-rw-   0        0        0     5897 2023-07-24 01:47:35.000000 spyc_iot-0.0.6/src/spyc_iot/max7219.py
+-rw-rw-rw-   0        0        0      667 2023-07-14 05:55:28.000000 spyc_iot-0.0.6/src/spyc_iot/ntp.py
+-rw-rw-rw-   0        0        0      233 2023-07-20 05:42:07.000000 spyc_iot-0.0.6/src/spyc_iot/time.py
+-rw-rw-rw-   0        0        0      505 2023-07-14 04:50:45.000000 spyc_iot-0.0.6/src/spyc_iot/wifi.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:51:01.259120 spyc_iot-0.0.6/src/spyc_iot.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-07-24 01:51:01.000000 spyc_iot-0.0.6/src/spyc_iot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-24 01:51:01.000000 spyc_iot-0.0.6/src/spyc_iot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:51:01.000000 spyc_iot-0.0.6/src/spyc_iot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 01:51:01.000000 spyc_iot-0.0.6/src/spyc_iot.egg-info/top_level.txt
```

### Comparing `spyc_iot-0.0.5/LICENSE` & `spyc_iot-0.0.6/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (C) 2023 Shatin Pui Ying College
+Copyright (C) 2023 Shatin Pui Ying College. Written by Leung King Hei and Kynson Szetau
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `spyc_iot-0.0.5/src/spyc_iot/ntp.py` & `spyc_iot-0.0.6/src/spyc_iot/ntp.py`

 * *Files identical despite different names*

