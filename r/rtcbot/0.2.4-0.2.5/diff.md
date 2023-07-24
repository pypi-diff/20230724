# Comparing `tmp/rtcbot-0.2.4.tar.gz` & `tmp/rtcbot-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtcbot-0.2.4.tar", last modified: Thu Mar 11 01:00:20 2021, max compression
+gzip compressed data, was "rtcbot-0.2.5.tar", last modified: Mon Jul 24 05:39:28 2023, max compression
```

## Comparing `rtcbot-0.2.4.tar` & `rtcbot-0.2.5.tar`

### file list

```diff
@@ -1,39 +1,145 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2021-03-11 01:00:20.079154 rtcbot-0.2.4/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       24 2019-03-15 00:34:33.000000 rtcbot-0.2.4/MANIFEST.in
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6887 2021-03-11 01:00:20.079154 rtcbot-0.2.4/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5184 2020-11-26 06:41:48.000000 rtcbot-0.2.4/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2021-03-11 01:00:20.075821 rtcbot-0.2.4/rtcbot/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      392 2021-03-10 16:39:35.000000 rtcbot-0.2.4/rtcbot/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     9319 2019-01-21 05:15:24.000000 rtcbot-0.2.4/rtcbot/arduino.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3770 2021-03-10 16:43:11.000000 rtcbot-0.2.4/rtcbot/audio.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2021-03-11 01:00:20.075821 rtcbot-0.2.4/rtcbot/base/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      351 2019-03-15 02:02:40.000000 rtcbot-0.2.4/rtcbot/base/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20446 2021-03-10 22:02:18.000000 rtcbot-0.2.4/rtcbot/base/base.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8452 2020-10-18 20:51:27.000000 rtcbot-0.2.4/rtcbot/base/events.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5568 2019-03-23 22:11:25.000000 rtcbot-0.2.4/rtcbot/base/multiprocess.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5980 2020-04-24 16:52:39.000000 rtcbot-0.2.4/rtcbot/base/thread.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7360 2020-06-16 21:19:28.000000 rtcbot-0.2.4/rtcbot/camera.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20285 2021-03-11 00:32:56.000000 rtcbot-0.2.4/rtcbot/connection.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2021-03-11 01:00:20.075821 rtcbot-0.2.4/rtcbot/devices/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2019-01-19 21:18:05.000000 rtcbot-0.2.4/rtcbot/devices/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1599 2019-01-21 05:21:37.000000 rtcbot-0.2.4/rtcbot/devices/gps.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2142 2019-03-23 22:13:23.000000 rtcbot-0.2.4/rtcbot/inputs.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      984 2019-03-15 00:07:05.000000 rtcbot-0.2.4/rtcbot/javascript.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6472 2021-03-11 01:00:19.000000 rtcbot-0.2.4/rtcbot/rtcbot.js
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8014 2020-04-24 17:28:05.000000 rtcbot-0.2.4/rtcbot/subscriptions.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12078 2020-10-19 01:32:49.000000 rtcbot-0.2.4/rtcbot/tracks.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4172 2020-10-18 22:55:54.000000 rtcbot-0.2.4/rtcbot/websocket.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2021-03-11 01:00:20.075821 rtcbot-0.2.4/rtcbot.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6887 2021-03-11 01:00:19.000000 rtcbot-0.2.4/rtcbot.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      668 2021-03-11 01:00:20.000000 rtcbot-0.2.4/rtcbot.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2021-03-11 01:00:19.000000 rtcbot-0.2.4/rtcbot.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       72 2021-03-11 01:00:19.000000 rtcbot-0.2.4/rtcbot.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       13 2021-03-11 01:00:19.000000 rtcbot-0.2.4/rtcbot.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2021-03-11 01:00:20.079154 rtcbot-0.2.4/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1116 2021-03-10 16:39:19.000000 rtcbot-0.2.4/setup.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2021-03-11 01:00:20.079154 rtcbot-0.2.4/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2019-01-04 06:11:14.000000 rtcbot-0.2.4/tests/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1435 2019-03-12 06:04:44.000000 rtcbot-0.2.4/tests/test_RTCConnection.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4082 2019-08-28 01:09:34.000000 rtcbot-0.2.4/tests/test_base.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1669 2019-01-10 05:10:35.000000 rtcbot-0.2.4/tests/test_subscriptions.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      991 2019-03-23 06:35:11.000000 rtcbot-0.2.4/tests/test_websocket.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.907623 rtcbot-0.2.5/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.880955 rtcbot-0.2.5/.github/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.884289 rtcbot-0.2.5/.github/workflows/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1330 2021-11-25 19:49:54.000000 rtcbot-0.2.5/.github/workflows/tests.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1395 2021-11-25 19:49:54.000000 rtcbot-0.2.5/.gitignore
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1068 2021-11-25 19:49:54.000000 rtcbot-0.2.5/LICENSE.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       24 2021-11-25 19:49:54.000000 rtcbot-0.2.5/MANIFEST.in
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      580 2021-11-25 19:49:54.000000 rtcbot-0.2.5/Makefile
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5738 2023-07-24 05:39:28.907623 rtcbot-0.2.5/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5184 2021-11-25 19:49:54.000000 rtcbot-0.2.5/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.887622 rtcbot-0.2.5/docs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/.nojekyll
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      375 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/API.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      580 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/Makefile
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.890956 rtcbot-0.2.5/docs/_static/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2171732 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/_static/control_example.m4v
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6676 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/arduino.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2664 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/audio.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1702 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/base.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3414 2023-07-24 05:18:39.000000 rtcbot-0.2.5/docs/camera.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6497 2023-07-24 05:18:39.000000 rtcbot-0.2.5/docs/conf.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1397 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3713 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/inputs.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4314 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/installing.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3007 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/javascript.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      787 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/make.bat
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       83 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/requirements.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      194 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/rtcconnection.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      388 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/subscriptions.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      188 2021-11-25 19:49:54.000000 rtcbot-0.2.5/docs/websocket.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.894289 rtcbot-0.2.5/examples/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.894289 rtcbot-0.2.5/examples/arduino/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      435 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/arduino/basic.ino
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      516 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/arduino/basic.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1025 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/arduino/raw.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.894289 rtcbot-0.2.5/examples/basics/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8033 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/basics/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      240 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/basics/audio.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      374 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/basics/both.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      228 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/basics/video.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      584 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/index.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.894289 rtcbot-0.2.5/examples/misc/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      321 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/misc/audiolouder.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      333 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/misc/bwvideo.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      237 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/misc/gamepad.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      241 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/misc/keyboard.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      233 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/misc/mouse.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.897622 rtcbot-0.2.5/examples/mobile/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14414 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/mobile/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      636 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/mobile/robot.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2574 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/mobile/server.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.897622 rtcbot-0.2.5/examples/multiconnect/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6919 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/multiconnect/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3459 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/multiconnect/multiconnect.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.897622 rtcbot-0.2.5/examples/offloading/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6401 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/offloading/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      935 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/offloading/desktop.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      627 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/offloading/robot.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.897622 rtcbot-0.2.5/examples/old/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      313 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/audio2.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      798 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/audiotest.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      373 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/avshow.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      949 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/closetest.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5351 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/evtest.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      266 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/gps.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      686 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/inputtest.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/joyst.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1227 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/old/rtcaudio.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.900956 rtcbot-0.2.5/examples/remotecontrol/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    13240 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/remotecontrol/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2131 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/remotecontrol/gamepad.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2133 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/remotecontrol/keyboard.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/remotecontrol/rc.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1971 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/remotecontrol/skeleton.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.900956 rtcbot-0.2.5/examples/streaming/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    12176 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/streaming/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2436 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/streaming/audiovideo.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2466 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/streaming/browser_audiovideo.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1994 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/streaming/skeleton.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2203 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/streaming/video.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.900956 rtcbot-0.2.5/examples/threads/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7230 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/threads/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2688 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/threads/bad_sensor.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3296 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/threads/threaded_sensor.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.900956 rtcbot-0.2.5/examples/webrtc/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    15599 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/webrtc/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      886 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/webrtc/basicserver.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2447 2022-10-23 18:04:58.000000 rtcbot-0.2.5/examples/webrtc/dataconnection.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2427 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/webrtc/jsonbackandforth.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    20533 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/webrtc/python_screenshot.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    18061 2021-11-25 19:49:54.000000 rtcbot-0.2.5/examples/webrtc/web_screenshot.png
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.904290 rtcbot-0.2.5/js/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1210 2021-11-25 19:49:54.000000 rtcbot-0.2.5/js/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    81210 2023-07-24 05:39:27.000000 rtcbot-0.2.5/js/package-lock.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      717 2023-07-24 05:32:32.000000 rtcbot-0.2.5/js/package.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      980 2021-11-25 19:49:54.000000 rtcbot-0.2.5/js/rollup.config.js
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.904290 rtcbot-0.2.5/js/src/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8941 2021-11-25 19:49:54.000000 rtcbot-0.2.5/js/src/connection.js
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5865 2021-11-25 19:49:54.000000 rtcbot-0.2.5/js/src/inputs.js
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1089 2021-11-25 19:49:54.000000 rtcbot-0.2.5/js/src/main.js
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      853 2021-11-25 19:49:54.000000 rtcbot-0.2.5/js/src/websocket.js
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.904290 rtcbot-0.2.5/js/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      578 2021-11-25 19:49:54.000000 rtcbot-0.2.5/js/tests/jstest.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1182 2021-11-25 19:49:54.000000 rtcbot-0.2.5/js/tests/test.js
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      160 2021-11-25 19:49:54.000000 rtcbot-0.2.5/requirements.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.904290 rtcbot-0.2.5/rtcbot/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      403 2023-07-24 05:18:39.000000 rtcbot-0.2.5/rtcbot/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     9319 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/arduino.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3770 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/audio.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.907623 rtcbot-0.2.5/rtcbot/base/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      380 2022-10-23 17:30:23.000000 rtcbot-0.2.5/rtcbot/base/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    20458 2022-10-23 17:53:20.000000 rtcbot-0.2.5/rtcbot/base/base.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8452 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/base/events.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    19525 2022-10-23 17:30:23.000000 rtcbot-0.2.5/rtcbot/base/multiprocess.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5980 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/base/thread.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     9840 2023-07-24 05:18:39.000000 rtcbot-0.2.5/rtcbot/camera.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    20285 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/connection.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.907623 rtcbot-0.2.5/rtcbot/devices/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/devices/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1599 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/devices/gps.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2142 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/inputs.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      984 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/javascript.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6472 2023-07-24 05:39:28.000000 rtcbot-0.2.5/rtcbot/rtcbot.js
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8014 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/subscriptions.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    12078 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/tracks.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4172 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot/websocket.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.907623 rtcbot-0.2.5/rtcbot.dev/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      591 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot.dev/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4453 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot.dev/main.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      799 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot.dev/test.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      696 2021-11-25 19:49:54.000000 rtcbot-0.2.5/rtcbot.dev/testclient.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.907623 rtcbot-0.2.5/rtcbot.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5738 2023-07-24 05:39:28.000000 rtcbot-0.2.5/rtcbot.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2761 2023-07-24 05:39:28.000000 rtcbot-0.2.5/rtcbot.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-24 05:39:28.000000 rtcbot-0.2.5/rtcbot.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       72 2023-07-24 05:39:28.000000 rtcbot-0.2.5/rtcbot.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       13 2023-07-24 05:39:28.000000 rtcbot-0.2.5/rtcbot.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-24 05:39:28.907623 rtcbot-0.2.5/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1116 2023-07-24 05:29:20.000000 rtcbot-0.2.5/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-24 05:39:28.907623 rtcbot-0.2.5/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2021-11-25 19:49:54.000000 rtcbot-0.2.5/tests/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1435 2021-11-25 19:49:54.000000 rtcbot-0.2.5/tests/test_RTCConnection.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4082 2021-11-25 19:49:54.000000 rtcbot-0.2.5/tests/test_base.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1669 2021-11-25 19:49:54.000000 rtcbot-0.2.5/tests/test_subscriptions.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      991 2021-11-25 19:49:54.000000 rtcbot-0.2.5/tests/test_websocket.py
```

### Comparing `rtcbot-0.2.4/PKG-INFO` & `rtcbot-0.2.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,160 +1,160 @@
 Metadata-Version: 2.1
 Name: rtcbot
-Version: 0.2.4
+Version: 0.2.5
 Summary: An asyncio-focused library for webrtc robot control
 Home-page: https://github.com/dkumor/rtcbot
 Author: Daniel Kumor
 Author-email: pypi@dkumor.com
 License: MIT
-Description: # RTCBot
-        
-        [![PyPI](https://img.shields.io/pypi/v/rtcbot.svg?style=flat-square)](https://pypi.org/project/rtcbot/)
-        [![npm](https://img.shields.io/npm/v/rtcbot.svg?style=flat-square)](https://www.npmjs.com/package/rtcbot)
-        [![Documentation Status](https://readthedocs.org/projects/rtcbot/badge/?version=latest&style=flat-square)](https://rtcbot.readthedocs.io/en/latest/?badge=latest)
-        [![Join the chat at https://gitter.im/rtcbot/community](https://img.shields.io/gitter/room/dkumor/rtcbot.svg?style=flat-square)](https://gitter.im/rtcbot/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-        ![Tests](https://github.com/dkumor/rtcbot/workflows/tests/badge.svg)
-        
-        RTCBot's purpose is to provide a set of simple modules that help in developing remote-controlled robots in Python, with a focus on the Raspberry Pi.
-        
-        The documentation includes tutorials that guide in developing your robot, starting from a basic connection between a Raspberry Pi and Browser, and encompass
-        creating a video-streaming robot controlled entirely over a 4G mobile connection, all the way to a powerful system that offloads complex computation to a desktop PC in real-time.
-        
-        All communication happens through [WebRTC](https://en.wikipedia.org/wiki/WebRTC),
-        using Python 3's asyncio and the wonderful [aiortc](https://github.com/jlaine/aiortc) library,
-        meaning that your robot can be controlled with low latency both from the browser and through Python,
-        even when it is not connected to your local network.
-        
-        The library is explained piece by piece in [the documentation](https://rtcbot.readthedocs.io/en/latest/index.html).
-        
-        ### [See Documentation & Tutorials](https://rtcbot.readthedocs.io/en/latest/index.html)
-        
-        ## Installing
-        
-        RTCBot relies on some Python libraries that will need to be compiled by pip, so
-        you need to install their dependencies. The following commands will work on Ubuntu and Raspbian Buster:
-        
-        ```bash
-        sudo apt-get install build-essential python3-numpy python3-cffi python3-aiohttp \
-                libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev \
-                libswscale-dev libswresample-dev libavfilter-dev libopus-dev \
-                libvpx-dev pkg-config libsrtp2-dev python3-opencv pulseaudio
-        ```
-        
-        And then install rtcbot:
-        
-        ```bash
-        sudo pip3 install rtcbot
-        ```
-        
-        For installation instructions for Windows and Mac, [refer to the documentation](https://rtcbot.readthedocs.io/en/latest/installing.html)
-        
-        ## Example
-        
-        This example uses RTCBot to live stream a webcam to the browser. For details, please look at [the tutorials](https://rtcbot.readthedocs.io/en/latest/examples/index.html).
-        
-        Python code that streams video to the browser:
-        
-        ```python
-        from aiohttp import web
-        routes = web.RouteTableDef()
-        
-        from rtcbot import RTCConnection, getRTCBotJS, CVCamera
-        
-        camera = CVCamera()
-        # For this example, we use just one global connection
-        conn = RTCConnection()
-        conn.video.putSubscription(camera)
-        
-        # Serve the RTCBot javascript library at /rtcbot.js
-        @routes.get("/rtcbot.js")
-        async def rtcbotjs(request):
-            return web.Response(content_type="application/javascript", text=getRTCBotJS())
-        
-        # This sets up the connection
-        @routes.post("/connect")
-        async def connect(request):
-            clientOffer = await request.json()
-            serverResponse = await conn.getLocalDescription(clientOffer)
-            return web.json_response(serverResponse)
-        
-        @routes.get("/")
-        async def index(request):
-            with open("index.html", "r") as f:
-                return web.Response(content_type="text/html", text=f.read())
-        
-        async def cleanup(app=None):
-            await conn.close()
-            camera.close()
-        
-        app = web.Application()
-        app.add_routes(routes)
-        app.on_shutdown.append(cleanup)
-        web.run_app(app)
-        ```
-        
-        Browser code (index.html) that displays the video stream:
-        
-        ```html
-        <html>
-          <head>
-            <title>RTCBot: Video</title>
-            <script src="/rtcbot.js"></script>
-          </head>
-          <body style="text-align: center;padding-top: 30px;">
-            <video autoplay playsinline></video> <audio autoplay></audio>
-            <p>
-              Open the browser's developer tools to see console messages (CTRL+SHIFT+C)
-            </p>
-            <script>
-              var conn = new rtcbot.RTCConnection();
-        
-              conn.video.subscribe(function (stream) {
-                document.querySelector("video").srcObject = stream;
-              });
-        
-              async function connect() {
-                let offer = await conn.getLocalDescription();
-        
-                // POST the information to /connect
-                let response = await fetch("/connect", {
-                  method: "POST",
-                  cache: "no-cache",
-                  body: JSON.stringify(offer),
-                });
-        
-                await conn.setRemoteDescription(await response.json());
-        
-                console.log("Ready!");
-              }
-              connect();
-            </script>
-          </body>
-        </html>
-        ```
-        
-        ## Development
-        
-        To use `rtcbot` code directly, clone the repository, and install the requirements:
-        
-        ```
-        pip install -r requirements.txt
-        ```
-        
-        Then, you will need to perform the javascript build step, to prepare the browser code. This step requires both `make` and `npm` to be installed on your machine. To build the javascript, type in:
-        
-        ```
-        make js
-        ```
-        
-        This creates `rtcbot/rtcbot.js`, which is returned by `rtcbot.getRTCBotJS()`.
-        
-        After these two steps, you should be able to successfully import and use the library.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# RTCBot
+
+[![PyPI](https://img.shields.io/pypi/v/rtcbot.svg?style=flat-square)](https://pypi.org/project/rtcbot/)
+[![npm](https://img.shields.io/npm/v/rtcbot.svg?style=flat-square)](https://www.npmjs.com/package/rtcbot)
+[![Documentation Status](https://readthedocs.org/projects/rtcbot/badge/?version=latest&style=flat-square)](https://rtcbot.readthedocs.io/en/latest/?badge=latest)
+[![Join the chat at https://gitter.im/rtcbot/community](https://img.shields.io/gitter/room/dkumor/rtcbot.svg?style=flat-square)](https://gitter.im/rtcbot/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+![Tests](https://github.com/dkumor/rtcbot/workflows/tests/badge.svg)
+
+RTCBot's purpose is to provide a set of simple modules that help in developing remote-controlled robots in Python, with a focus on the Raspberry Pi.
+
+The documentation includes tutorials that guide in developing your robot, starting from a basic connection between a Raspberry Pi and Browser, and encompass
+creating a video-streaming robot controlled entirely over a 4G mobile connection, all the way to a powerful system that offloads complex computation to a desktop PC in real-time.
+
+All communication happens through [WebRTC](https://en.wikipedia.org/wiki/WebRTC),
+using Python 3's asyncio and the wonderful [aiortc](https://github.com/jlaine/aiortc) library,
+meaning that your robot can be controlled with low latency both from the browser and through Python,
+even when it is not connected to your local network.
+
+The library is explained piece by piece in [the documentation](https://rtcbot.readthedocs.io/en/latest/index.html).
+
+### [See Documentation & Tutorials](https://rtcbot.readthedocs.io/en/latest/index.html)
+
+## Installing
+
+RTCBot relies on some Python libraries that will need to be compiled by pip, so
+you need to install their dependencies. The following commands will work on Ubuntu and Raspbian Buster:
+
+```bash
+sudo apt-get install build-essential python3-numpy python3-cffi python3-aiohttp \
+        libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev \
+        libswscale-dev libswresample-dev libavfilter-dev libopus-dev \
+        libvpx-dev pkg-config libsrtp2-dev python3-opencv pulseaudio
+```
+
+And then install rtcbot:
+
+```bash
+sudo pip3 install rtcbot
+```
+
+For installation instructions for Windows and Mac, [refer to the documentation](https://rtcbot.readthedocs.io/en/latest/installing.html)
+
+## Example
+
+This example uses RTCBot to live stream a webcam to the browser. For details, please look at [the tutorials](https://rtcbot.readthedocs.io/en/latest/examples/index.html).
+
+Python code that streams video to the browser:
+
+```python
+from aiohttp import web
+routes = web.RouteTableDef()
+
+from rtcbot import RTCConnection, getRTCBotJS, CVCamera
+
+camera = CVCamera()
+# For this example, we use just one global connection
+conn = RTCConnection()
+conn.video.putSubscription(camera)
+
+# Serve the RTCBot javascript library at /rtcbot.js
+@routes.get("/rtcbot.js")
+async def rtcbotjs(request):
+    return web.Response(content_type="application/javascript", text=getRTCBotJS())
+
+# This sets up the connection
+@routes.post("/connect")
+async def connect(request):
+    clientOffer = await request.json()
+    serverResponse = await conn.getLocalDescription(clientOffer)
+    return web.json_response(serverResponse)
+
+@routes.get("/")
+async def index(request):
+    with open("index.html", "r") as f:
+        return web.Response(content_type="text/html", text=f.read())
+
+async def cleanup(app=None):
+    await conn.close()
+    camera.close()
+
+app = web.Application()
+app.add_routes(routes)
+app.on_shutdown.append(cleanup)
+web.run_app(app)
+```
+
+Browser code (index.html) that displays the video stream:
+
+```html
+<html>
+  <head>
+    <title>RTCBot: Video</title>
+    <script src="/rtcbot.js"></script>
+  </head>
+  <body style="text-align: center;padding-top: 30px;">
+    <video autoplay playsinline></video> <audio autoplay></audio>
+    <p>
+      Open the browser's developer tools to see console messages (CTRL+SHIFT+C)
+    </p>
+    <script>
+      var conn = new rtcbot.RTCConnection();
+
+      conn.video.subscribe(function (stream) {
+        document.querySelector("video").srcObject = stream;
+      });
+
+      async function connect() {
+        let offer = await conn.getLocalDescription();
+
+        // POST the information to /connect
+        let response = await fetch("/connect", {
+          method: "POST",
+          cache: "no-cache",
+          body: JSON.stringify(offer),
+        });
+
+        await conn.setRemoteDescription(await response.json());
+
+        console.log("Ready!");
+      }
+      connect();
+    </script>
+  </body>
+</html>
+```
+
+## Development
+
+To use `rtcbot` code directly, clone the repository, and install the requirements:
+
+```
+pip install -r requirements.txt
+```
+
+Then, you will need to perform the javascript build step, to prepare the browser code. This step requires both `make` and `npm` to be installed on your machine. To build the javascript, type in:
+
+```
+make js
+```
+
+This creates `rtcbot/rtcbot.js`, which is returned by `rtcbot.getRTCBotJS()`.
+
+After these two steps, you should be able to successfully import and use the library.
```

### Comparing `rtcbot-0.2.4/README.md` & `rtcbot-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/arduino.py` & `rtcbot-0.2.5/rtcbot/arduino.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/audio.py` & `rtcbot-0.2.5/rtcbot/audio.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/base/base.py` & `rtcbot-0.2.5/rtcbot/base/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,16 @@
             except SubscriptionClosed:
                 self.__sclog.debug(
                     "Incoming subscription closed - checking for new subscription"
                 )
             except GeneratorExit:
                 raise SubscriptionClosed("SubscriptionConsumer has been closed")
             except:
-                self.__sclog.exception("Got unrecognized error from task. ignoring:")
+                self.__sclog.exception("Got unrecognized error from task.")
+                raise
 
         self.__sclog.debug("close() was called. raising SubscriptionClosed.")
         raise SubscriptionClosed("SubscriptionConsumer has been closed")
 
     def put_nowait(self, data):
         """
         This function allows you to directly send data to the object, without needing to
```

### Comparing `rtcbot-0.2.4/rtcbot/base/events.py` & `rtcbot-0.2.5/rtcbot/base/events.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/base/thread.py` & `rtcbot-0.2.5/rtcbot/base/thread.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/camera.py` & `rtcbot-0.2.5/rtcbot/camera.py`

 * *Files 17% similar despite different names*

```diff
@@ -130,20 +130,26 @@
             cam = CVCamera()
 
     This enables simple drop-in replacement between the two.
     """
 
     _log = logging.getLogger("rtcbot.PiCamera")
 
+    # Valid values for rotation are 0, 90, 180, 270
+    def __init__(self, rotation=0, **kwargs):
+        super().__init__(**kwargs)
+        self._rotation = rotation
+
     def _producer(self):
         import picamera
 
         with picamera.PiCamera() as cam:
             cam.resolution = (self._width, self._height)
             cam.framerate = self._fps
+            cam.rotation = self._rotation
             time.sleep(2)  # Why is this needed?
             self._log.debug("PiCamera Ready")
             self._setReady(True)
 
             t = time.time()
             i = 0
             while not self._shouldClose:
@@ -154,14 +160,76 @@
 
                 # This optional function is given by the user. default is identity x->x
                 frame = self._processframe(frame)
 
                 # Set the frame arrival event
                 self._loop.call_soon_threadsafe(self._put_nowait, frame)
 
+                i += 1
+                if time.time() > t + 1:
+                    self._log.debug(" %d fps", i)
+                    i = 0
+                    t = time.time()
+        self._setReady(False)
+        self._log.info("Closed camera capture")
+
+
+class PiCamera2(CVCamera):
+    """
+    Instead of using OpenCV camera support, uses the picamera2 library for direct access to the Raspberry Pi's CSI camera.
+
+    The interface is identical to CVCamera. When testing code on a desktop computer, it can be useful to
+    have the code automatically choose the correct camera::
+
+        try:
+            import picamera2 # picamera2 import will fail if not on pi
+            cam = PiCamera2()
+        except ImportError:
+            cam = CVCamera()
+
+    This enables simple drop-in replacement between the two.
+
+    You can use the parameter hflip=True to flip the camera horizontally, vflip=True to flip vertically,
+    or both to rotate 180 degrees.
+    """
+
+    _log = logging.getLogger("rtcbot.PiCamera2")
+
+    def __init__(self, hflip=False, vflip=False, **kwargs):
+        super().__init__(**kwargs)
+        self._hflip = hflip
+        self._vflip = vflip
+
+    def _producer(self):
+        from picamera2 import Picamera2
+        from libcamera import Transform
+
+        with Picamera2() as cam:
+            cam.preview_configuration.transform = Transform(hflip=self._hflip, vflip=self._vflip)
+            cam.preview_configuration.main.size = (self._width, self._height)
+            cam.preview_configuration.display = None
+            cam.preview_configuration.main.format = 'RGB888'
+            if self._fps > 0:
+                cam.video_configuration.controls.FrameDurationLimits = (round(1000000/self._fps), round(1000000/self._fps))
+            cam.start()
+            time.sleep(2)
+            self._log.debug("PiCamera2 Ready")
+            self._setReady(True)
+
+            t = time.time()
+            i = 0
+            while not self._shouldClose:
+                frame = cam.capture_array()
+
+                # This optional function is given by the user. default is identity x->x
+                frame = self._processframe(frame)
+
+                # Set the frame arrival event
+                self._loop.call_soon_threadsafe(self._put_nowait, frame)
+
                 i += 1
                 if time.time() > t + 1:
                     self._log.debug(" %d fps", i)
                     i = 0
                     t = time.time()
         self._setReady(False)
         self._log.info("Closed camera capture")
```

### Comparing `rtcbot-0.2.4/rtcbot/connection.py` & `rtcbot-0.2.5/rtcbot/connection.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/devices/gps.py` & `rtcbot-0.2.5/rtcbot/devices/gps.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/inputs.py` & `rtcbot-0.2.5/rtcbot/inputs.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/javascript.py` & `rtcbot-0.2.5/rtcbot/javascript.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/rtcbot.js` & `rtcbot-0.2.5/rtcbot/rtcbot.js`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/subscriptions.py` & `rtcbot-0.2.5/rtcbot/subscriptions.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/tracks.py` & `rtcbot-0.2.5/rtcbot/tracks.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot/websocket.py` & `rtcbot-0.2.5/rtcbot/websocket.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/rtcbot.egg-info/PKG-INFO` & `rtcbot-0.2.5/rtcbot.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,160 +1,160 @@
 Metadata-Version: 2.1
 Name: rtcbot
-Version: 0.2.4
+Version: 0.2.5
 Summary: An asyncio-focused library for webrtc robot control
 Home-page: https://github.com/dkumor/rtcbot
 Author: Daniel Kumor
 Author-email: pypi@dkumor.com
 License: MIT
-Description: # RTCBot
-        
-        [![PyPI](https://img.shields.io/pypi/v/rtcbot.svg?style=flat-square)](https://pypi.org/project/rtcbot/)
-        [![npm](https://img.shields.io/npm/v/rtcbot.svg?style=flat-square)](https://www.npmjs.com/package/rtcbot)
-        [![Documentation Status](https://readthedocs.org/projects/rtcbot/badge/?version=latest&style=flat-square)](https://rtcbot.readthedocs.io/en/latest/?badge=latest)
-        [![Join the chat at https://gitter.im/rtcbot/community](https://img.shields.io/gitter/room/dkumor/rtcbot.svg?style=flat-square)](https://gitter.im/rtcbot/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-        ![Tests](https://github.com/dkumor/rtcbot/workflows/tests/badge.svg)
-        
-        RTCBot's purpose is to provide a set of simple modules that help in developing remote-controlled robots in Python, with a focus on the Raspberry Pi.
-        
-        The documentation includes tutorials that guide in developing your robot, starting from a basic connection between a Raspberry Pi and Browser, and encompass
-        creating a video-streaming robot controlled entirely over a 4G mobile connection, all the way to a powerful system that offloads complex computation to a desktop PC in real-time.
-        
-        All communication happens through [WebRTC](https://en.wikipedia.org/wiki/WebRTC),
-        using Python 3's asyncio and the wonderful [aiortc](https://github.com/jlaine/aiortc) library,
-        meaning that your robot can be controlled with low latency both from the browser and through Python,
-        even when it is not connected to your local network.
-        
-        The library is explained piece by piece in [the documentation](https://rtcbot.readthedocs.io/en/latest/index.html).
-        
-        ### [See Documentation & Tutorials](https://rtcbot.readthedocs.io/en/latest/index.html)
-        
-        ## Installing
-        
-        RTCBot relies on some Python libraries that will need to be compiled by pip, so
-        you need to install their dependencies. The following commands will work on Ubuntu and Raspbian Buster:
-        
-        ```bash
-        sudo apt-get install build-essential python3-numpy python3-cffi python3-aiohttp \
-                libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev \
-                libswscale-dev libswresample-dev libavfilter-dev libopus-dev \
-                libvpx-dev pkg-config libsrtp2-dev python3-opencv pulseaudio
-        ```
-        
-        And then install rtcbot:
-        
-        ```bash
-        sudo pip3 install rtcbot
-        ```
-        
-        For installation instructions for Windows and Mac, [refer to the documentation](https://rtcbot.readthedocs.io/en/latest/installing.html)
-        
-        ## Example
-        
-        This example uses RTCBot to live stream a webcam to the browser. For details, please look at [the tutorials](https://rtcbot.readthedocs.io/en/latest/examples/index.html).
-        
-        Python code that streams video to the browser:
-        
-        ```python
-        from aiohttp import web
-        routes = web.RouteTableDef()
-        
-        from rtcbot import RTCConnection, getRTCBotJS, CVCamera
-        
-        camera = CVCamera()
-        # For this example, we use just one global connection
-        conn = RTCConnection()
-        conn.video.putSubscription(camera)
-        
-        # Serve the RTCBot javascript library at /rtcbot.js
-        @routes.get("/rtcbot.js")
-        async def rtcbotjs(request):
-            return web.Response(content_type="application/javascript", text=getRTCBotJS())
-        
-        # This sets up the connection
-        @routes.post("/connect")
-        async def connect(request):
-            clientOffer = await request.json()
-            serverResponse = await conn.getLocalDescription(clientOffer)
-            return web.json_response(serverResponse)
-        
-        @routes.get("/")
-        async def index(request):
-            with open("index.html", "r") as f:
-                return web.Response(content_type="text/html", text=f.read())
-        
-        async def cleanup(app=None):
-            await conn.close()
-            camera.close()
-        
-        app = web.Application()
-        app.add_routes(routes)
-        app.on_shutdown.append(cleanup)
-        web.run_app(app)
-        ```
-        
-        Browser code (index.html) that displays the video stream:
-        
-        ```html
-        <html>
-          <head>
-            <title>RTCBot: Video</title>
-            <script src="/rtcbot.js"></script>
-          </head>
-          <body style="text-align: center;padding-top: 30px;">
-            <video autoplay playsinline></video> <audio autoplay></audio>
-            <p>
-              Open the browser's developer tools to see console messages (CTRL+SHIFT+C)
-            </p>
-            <script>
-              var conn = new rtcbot.RTCConnection();
-        
-              conn.video.subscribe(function (stream) {
-                document.querySelector("video").srcObject = stream;
-              });
-        
-              async function connect() {
-                let offer = await conn.getLocalDescription();
-        
-                // POST the information to /connect
-                let response = await fetch("/connect", {
-                  method: "POST",
-                  cache: "no-cache",
-                  body: JSON.stringify(offer),
-                });
-        
-                await conn.setRemoteDescription(await response.json());
-        
-                console.log("Ready!");
-              }
-              connect();
-            </script>
-          </body>
-        </html>
-        ```
-        
-        ## Development
-        
-        To use `rtcbot` code directly, clone the repository, and install the requirements:
-        
-        ```
-        pip install -r requirements.txt
-        ```
-        
-        Then, you will need to perform the javascript build step, to prepare the browser code. This step requires both `make` and `npm` to be installed on your machine. To build the javascript, type in:
-        
-        ```
-        make js
-        ```
-        
-        This creates `rtcbot/rtcbot.js`, which is returned by `rtcbot.getRTCBotJS()`.
-        
-        After these two steps, you should be able to successfully import and use the library.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# RTCBot
+
+[![PyPI](https://img.shields.io/pypi/v/rtcbot.svg?style=flat-square)](https://pypi.org/project/rtcbot/)
+[![npm](https://img.shields.io/npm/v/rtcbot.svg?style=flat-square)](https://www.npmjs.com/package/rtcbot)
+[![Documentation Status](https://readthedocs.org/projects/rtcbot/badge/?version=latest&style=flat-square)](https://rtcbot.readthedocs.io/en/latest/?badge=latest)
+[![Join the chat at https://gitter.im/rtcbot/community](https://img.shields.io/gitter/room/dkumor/rtcbot.svg?style=flat-square)](https://gitter.im/rtcbot/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+![Tests](https://github.com/dkumor/rtcbot/workflows/tests/badge.svg)
+
+RTCBot's purpose is to provide a set of simple modules that help in developing remote-controlled robots in Python, with a focus on the Raspberry Pi.
+
+The documentation includes tutorials that guide in developing your robot, starting from a basic connection between a Raspberry Pi and Browser, and encompass
+creating a video-streaming robot controlled entirely over a 4G mobile connection, all the way to a powerful system that offloads complex computation to a desktop PC in real-time.
+
+All communication happens through [WebRTC](https://en.wikipedia.org/wiki/WebRTC),
+using Python 3's asyncio and the wonderful [aiortc](https://github.com/jlaine/aiortc) library,
+meaning that your robot can be controlled with low latency both from the browser and through Python,
+even when it is not connected to your local network.
+
+The library is explained piece by piece in [the documentation](https://rtcbot.readthedocs.io/en/latest/index.html).
+
+### [See Documentation & Tutorials](https://rtcbot.readthedocs.io/en/latest/index.html)
+
+## Installing
+
+RTCBot relies on some Python libraries that will need to be compiled by pip, so
+you need to install their dependencies. The following commands will work on Ubuntu and Raspbian Buster:
+
+```bash
+sudo apt-get install build-essential python3-numpy python3-cffi python3-aiohttp \
+        libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev \
+        libswscale-dev libswresample-dev libavfilter-dev libopus-dev \
+        libvpx-dev pkg-config libsrtp2-dev python3-opencv pulseaudio
+```
+
+And then install rtcbot:
+
+```bash
+sudo pip3 install rtcbot
+```
+
+For installation instructions for Windows and Mac, [refer to the documentation](https://rtcbot.readthedocs.io/en/latest/installing.html)
+
+## Example
+
+This example uses RTCBot to live stream a webcam to the browser. For details, please look at [the tutorials](https://rtcbot.readthedocs.io/en/latest/examples/index.html).
+
+Python code that streams video to the browser:
+
+```python
+from aiohttp import web
+routes = web.RouteTableDef()
+
+from rtcbot import RTCConnection, getRTCBotJS, CVCamera
+
+camera = CVCamera()
+# For this example, we use just one global connection
+conn = RTCConnection()
+conn.video.putSubscription(camera)
+
+# Serve the RTCBot javascript library at /rtcbot.js
+@routes.get("/rtcbot.js")
+async def rtcbotjs(request):
+    return web.Response(content_type="application/javascript", text=getRTCBotJS())
+
+# This sets up the connection
+@routes.post("/connect")
+async def connect(request):
+    clientOffer = await request.json()
+    serverResponse = await conn.getLocalDescription(clientOffer)
+    return web.json_response(serverResponse)
+
+@routes.get("/")
+async def index(request):
+    with open("index.html", "r") as f:
+        return web.Response(content_type="text/html", text=f.read())
+
+async def cleanup(app=None):
+    await conn.close()
+    camera.close()
+
+app = web.Application()
+app.add_routes(routes)
+app.on_shutdown.append(cleanup)
+web.run_app(app)
+```
+
+Browser code (index.html) that displays the video stream:
+
+```html
+<html>
+  <head>
+    <title>RTCBot: Video</title>
+    <script src="/rtcbot.js"></script>
+  </head>
+  <body style="text-align: center;padding-top: 30px;">
+    <video autoplay playsinline></video> <audio autoplay></audio>
+    <p>
+      Open the browser's developer tools to see console messages (CTRL+SHIFT+C)
+    </p>
+    <script>
+      var conn = new rtcbot.RTCConnection();
+
+      conn.video.subscribe(function (stream) {
+        document.querySelector("video").srcObject = stream;
+      });
+
+      async function connect() {
+        let offer = await conn.getLocalDescription();
+
+        // POST the information to /connect
+        let response = await fetch("/connect", {
+          method: "POST",
+          cache: "no-cache",
+          body: JSON.stringify(offer),
+        });
+
+        await conn.setRemoteDescription(await response.json());
+
+        console.log("Ready!");
+      }
+      connect();
+    </script>
+  </body>
+</html>
+```
+
+## Development
+
+To use `rtcbot` code directly, clone the repository, and install the requirements:
+
+```
+pip install -r requirements.txt
+```
+
+Then, you will need to perform the javascript build step, to prepare the browser code. This step requires both `make` and `npm` to be installed on your machine. To build the javascript, type in:
+
+```
+make js
+```
+
+This creates `rtcbot/rtcbot.js`, which is returned by `rtcbot.getRTCBotJS()`.
+
+After these two steps, you should be able to successfully import and use the library.
```

### Comparing `rtcbot-0.2.4/setup.py` & `rtcbot-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setuptools.setup(
     name="rtcbot",
-    version="0.2.4",
+    version="0.2.5",
     description="An asyncio-focused library for webrtc robot control",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/dkumor/rtcbot",
     author="Daniel Kumor",
     author_email="pypi@dkumor.com",
     license="MIT",
```

### Comparing `rtcbot-0.2.4/tests/test_RTCConnection.py` & `rtcbot-0.2.5/tests/test_RTCConnection.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/tests/test_base.py` & `rtcbot-0.2.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/tests/test_subscriptions.py` & `rtcbot-0.2.5/tests/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `rtcbot-0.2.4/tests/test_websocket.py` & `rtcbot-0.2.5/tests/test_websocket.py`

 * *Files identical despite different names*

