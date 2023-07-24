# Comparing `tmp/py4AxisStage-0.0.1-py3-none-any.whl.zip` & `tmp/py4AxisStage-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2243 bytes, number of entries: 6
+Zip file size: 2371 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       39 b- defN 23-Jul-24 02:03 py4AxisStage/__init__.py
--rw-rw-rw-  2.0 fat     1785 b- defN 23-Jul-24 01:59 py4AxisStage/py4AxisStage.py
--rw-rw-rw-  2.0 fat      191 b- defN 23-Jul-24 02:07 py4AxisStage-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 02:07 py4AxisStage-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-24 02:07 py4AxisStage-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      481 b- defN 23-Jul-24 02:07 py4AxisStage-0.0.1.dist-info/RECORD
-6 files, 2601 bytes uncompressed, 1365 bytes compressed:  47.5%
+-rw-rw-rw-  2.0 fat     2015 b- defN 23-Jul-24 02:37 py4AxisStage/py4AxisStage.py
+-rw-rw-rw-  2.0 fat      191 b- defN 23-Jul-24 02:39 py4AxisStage-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 02:39 py4AxisStage-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-24 02:39 py4AxisStage-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      481 b- defN 23-Jul-24 02:39 py4AxisStage-0.0.2.dist-info/RECORD
+6 files, 2831 bytes uncompressed, 1493 bytes compressed:  47.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: py4AxisStage/__init__.py
 Comment: 
 
 Filename: py4AxisStage/py4AxisStage.py
 Comment: 
 
-Filename: py4AxisStage-0.0.1.dist-info/METADATA
+Filename: py4AxisStage-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: py4AxisStage-0.0.1.dist-info/WHEEL
+Filename: py4AxisStage-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: py4AxisStage-0.0.1.dist-info/top_level.txt
+Filename: py4AxisStage-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: py4AxisStage-0.0.1.dist-info/RECORD
+Filename: py4AxisStage-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## py4AxisStage/py4AxisStage.py

```diff
@@ -1,8 +1,8 @@
-# v0.0.1
+# v0.0.2
 
 from socket import socket, AF_INET, SOCK_DGRAM
 from threading import Thread
 import json
 import subprocess
 
 class py4AxisStage:
@@ -10,25 +10,30 @@
         x = 0
         y = 1
         z = 2
         stay = 3
     class Coord:
         ABS = 0
         REL = 1
-
     class _socket_setting:
         port_send = 9000  # Python→C++
         port_recv = 9001  # C++→Python
         address = "127.0.0.1"
+    class StageError(Exception):
+        pass
 
     def __init__(self):
         self._s_send = socket(AF_INET, SOCK_DGRAM)
         self._s_recv = socket(AF_INET, SOCK_DGRAM)
         self._s_recv.bind((self._socket_setting.address, self._socket_setting.port_recv))
-        self._cpp_app = subprocess.Popen(r"C:\Users\hmi\Documents\nishimura\build\My4axisStage_for_ExternalControl\debug\My4axisStage_for_ExternalControl.exe")
+        try:
+            self._cpp_app = subprocess.Popen(r"C:\Users\hmi\Documents\nishimura\build\My4axisStage_for_ExternalControl\debug\My4axisStage_for_ExternalControl.exe")
+        except FileNotFoundError:
+            raise self.StageError('4軸ステージが接続されていないPCの可能性があります')
+            exit()
         self._th_monitor_pos = Thread(target=self._get_position, daemon=True)
         self._th_monitor_pos.start()
         self.position = {}
         while len(self.position) == 0:
             pass
     def _get_position(self):
         msg_recv, _ = self._s_recv.recvfrom(2048)
```

