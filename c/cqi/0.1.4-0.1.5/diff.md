# Comparing `tmp/cqi-0.1.4.tar.gz` & `tmp/cqi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqi-0.1.4.tar", last modified: Fri Jul 14 10:35:42 2023, max compression
+gzip compressed data, was "cqi-0.1.5.tar", last modified: Mon Jul 24 13:10:04 2023, max compression
```

## Comparing `cqi-0.1.4.tar` & `cqi-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.620060 cqi-0.1.4/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.4/LICENSE
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1498 2023-07-14 10:35:42.620060 cqi-0.1.4/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1012 2023-07-14 10:29:35.000000 cqi-0.1.4/README.md
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.610060 cqi-0.1.4/cqi/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.4/cqi/__init__.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.620060 cqi-0.1.4/cqi/api/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.4/cqi/api/__init__.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    20355 2023-07-14 10:23:10.000000 cqi-0.1.4/cqi/api/client.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.4/cqi/api/specification.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1826 2023-07-14 10:26:07.000000 cqi-0.1.4/cqi/client.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5141 2023-07-14 10:03:47.000000 cqi-0.1.4/cqi/errors.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.620060 cqi-0.1.4/cqi/models/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.4/cqi/models/__init__.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     7077 2023-07-13 06:38:32.000000 cqi-0.1.4/cqi/models/attributes.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2789 2023-07-04 07:00:23.000000 cqi-0.1.4/cqi/models/corpora.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2374 2023-07-04 06:58:38.000000 cqi-0.1.4/cqi/models/resource.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3911 2023-07-04 06:55:29.000000 cqi-0.1.4/cqi/models/subcorpora.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1180 2023-07-14 10:03:17.000000 cqi-0.1.4/cqi/status.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-07-14 10:29:43.000000 cqi-0.1.4/cqi/version.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.610060 cqi-0.1.4/cqi.egg-info/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1498 2023-07-14 10:35:42.000000 cqi-0.1.4/cqi.egg-info/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-07-14 10:35:42.000000 cqi-0.1.4/cqi.egg-info/SOURCES.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-07-14 10:35:42.000000 cqi-0.1.4/cqi.egg-info/dependency_links.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-07-14 10:35:42.000000 cqi-0.1.4/cqi.egg-info/top_level.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-07-14 10:35:42.620060 cqi-0.1.4/setup.cfg
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.4/setup.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-24 13:10:04.893474 cqi-0.1.5/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.5/LICENSE
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1498 2023-07-24 13:10:04.893474 cqi-0.1.5/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1012 2023-07-24 13:06:22.000000 cqi-0.1.5/README.md
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-24 13:10:04.893474 cqi-0.1.5/cqi/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.5/cqi/__init__.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-24 13:10:04.893474 cqi-0.1.5/cqi/api/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.5/cqi/api/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    20783 2023-07-24 13:05:37.000000 cqi-0.1.5/cqi/api/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.5/cqi/api/specification.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1806 2023-07-24 12:52:29.000000 cqi-0.1.5/cqi/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5141 2023-07-14 10:03:47.000000 cqi-0.1.5/cqi/errors.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-24 13:10:04.893474 cqi-0.1.5/cqi/models/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.5/cqi/models/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     7077 2023-07-13 06:38:32.000000 cqi-0.1.5/cqi/models/attributes.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2789 2023-07-04 07:00:23.000000 cqi-0.1.5/cqi/models/corpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2374 2023-07-04 06:58:38.000000 cqi-0.1.5/cqi/models/resource.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3911 2023-07-04 06:55:29.000000 cqi-0.1.5/cqi/models/subcorpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1180 2023-07-14 10:03:17.000000 cqi-0.1.5/cqi/status.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-07-24 13:05:46.000000 cqi-0.1.5/cqi/version.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-24 13:10:04.893474 cqi-0.1.5/cqi.egg-info/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1498 2023-07-24 13:10:04.000000 cqi-0.1.5/cqi.egg-info/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-07-24 13:10:04.000000 cqi-0.1.5/cqi.egg-info/SOURCES.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-07-24 13:10:04.000000 cqi-0.1.5/cqi.egg-info/dependency_links.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-07-24 13:10:04.000000 cqi-0.1.5/cqi.egg-info/top_level.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-07-24 13:10:04.893474 cqi-0.1.5/setup.cfg
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.5/setup.py
```

### Comparing `cqi-0.1.4/LICENSE` & `cqi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cqi-0.1.4/PKG-INFO` & `cqi-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqi
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
 Home-page: https://github.com/Pevtrick/cqi-py
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 pip install cqi
 ```
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
-| 0.1.0 - 0.1.4   | 0.1              |
+| 0.1.0 - 0.1.5   | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.4/README.md` & `cqi-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pip install cqi
 ```
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
-| 0.1.0 - 0.1.4   | 0.1              |
+| 0.1.0 - 0.1.5   | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.4/cqi/api/client.py` & `cqi-0.1.5/cqi/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Callable, Dict, List, Optional, Tuple
+from typing import Callable, Dict, List, Tuple
 import socket
 import struct
+import time
 from . import specification
 from .. import errors
 from .. import status
 
 
 class APIClient:
     '''
@@ -31,23 +32,22 @@
     version (str): The version of the CQi protocol to use. Default: ``0.1``
     '''
 
     def __init__(
         self,
         host: str,
         port: int = 4877,
-        timeout: Optional[float] = 60.0,
+        timeout: float = 60.0,
         version: str = '0.1'
     ):
         self.host: str = host
         self.port: int = port
         self.socket: socket.socket = socket.socket()
-        self.timeout: Optional[float] = timeout
+        self.timeout: float = timeout
         self.version: str = version
-        self.socket.settimeout(self.timeout)
 
     def ctrl_connect(
         self,
         username: str,
         password: str
     ) -> status.StatusConnectOk:
         self.socket.connect((self.host, self.port))
@@ -458,29 +458,43 @@
             except KeyError:
                 raise errors.CQiException(f'Unknown error code: {byte_data}')
         else:
             raise errors.CQiException(
                 f'Unknown response type: {response_type}'
             )
 
+    def __recv(self, bufsize: int):
+        # This method should not be necessary but
+        # self.socket.recv(bufsize, socket.MSG_WAITALL)
+        # does not work for some reason
+        start_time = time.time()
+        while time.time() - start_time < self.timeout:
+            # Check if the server already sent over the desired number of bytes
+            if len(self.socket.recv(bufsize, socket.MSG_PEEK)) == bufsize:
+                return self.socket.recv(bufsize)
+            # Wait a bit before checking again
+            time.sleep(0.05)
+        raise TimeoutError()
+
     def __recv_DATA_BYTE(self) -> int:
-        byte_data: bytes = self.socket.recv(1, socket.MSG_WAITALL)
+        byte_data: bytes = self.__recv(1)
         return struct.unpack('!B', byte_data)[0]
 
     def __recv_DATA_BOOL(self) -> bool:
-        byte_data: bytes = self.socket.recv(1, socket.MSG_WAITALL)
+        byte_data: bytes = self.__recv(1)
         return struct.unpack('!?', byte_data)[0]
 
     def __recv_DATA_INT(self) -> int:
-        byte_data: bytes = self.socket.recv(4, socket.MSG_WAITALL)
+        byte_data: bytes = self.__recv(4)
         return struct.unpack('!i', byte_data)[0]
 
     def __recv_DATA_STRING(self) -> str:
         n: int = self.__recv_WORD()
-        byte_data: bytes = self.socket.recv(n, socket.MSG_WAITALL)
+        byte_data: bytes = self.__recv(n)
+        # return byte_data.decode()
         return struct.unpack(f'!{n}s', byte_data)[0].decode()
 
     def __recv_DATA_BYTE_LIST(self) -> List[int]:
         data: List[int] = []
         n: int = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_BYTE())
@@ -544,15 +558,15 @@
         776: __recv_DATA_STRING_LIST,
         777: __recv_DATA_INT_INT,
         778: __recv_DATA_INT_INT_INT_INT,
         779: __recv_DATA_INT_TABLE
     }
 
     def __recv_WORD(self) -> int:
-        byte_data: bytes = self.socket.recv(2, socket.MSG_WAITALL)
+        byte_data: bytes = self.__recv(2)
         return struct.unpack('!H', byte_data)[0]
 
     def __send_BYTE(self, byte_data: int):
         data: bytes = struct.pack('!B', byte_data)
         self.socket.sendall(data)
 
     def __send_BOOL(self, bool_data: bool):
```

### Comparing `cqi-0.1.4/cqi/api/specification.py` & `cqi-0.1.5/cqi/api/specification.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.4/cqi/client.py` & `cqi-0.1.5/cqi/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .status import StatusByeOk, StatusConnectOk, StatusPingOk
 from .api import APIClient
 from .models.corpora import CorpusCollection
 
 
 
@@ -24,15 +24,15 @@
     api (APIClient): An API client pointing to the specified CQP server.
     '''
 
     def __init__(
         self,
         host: str,
         port: int = 4877,
-        timeout: Optional[float] = 60.0,
+        timeout: float = 60.0,
         version: str = '0.1'
     ):
         '''
         CQiClient constructor
 
         Args:
         host (str): URL to the CQP server. For example,
```

### Comparing `cqi-0.1.4/cqi/errors.py` & `cqi-0.1.5/cqi/errors.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.4/cqi/models/attributes.py` & `cqi-0.1.5/cqi/models/attributes.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.4/cqi/models/corpora.py` & `cqi-0.1.5/cqi/models/corpora.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.4/cqi/models/resource.py` & `cqi-0.1.5/cqi/models/resource.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.4/cqi/models/subcorpora.py` & `cqi-0.1.5/cqi/models/subcorpora.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.4/cqi/status.py` & `cqi-0.1.5/cqi/status.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.4/cqi.egg-info/PKG-INFO` & `cqi-0.1.5/cqi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqi
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
 Home-page: https://github.com/Pevtrick/cqi-py
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 pip install cqi
 ```
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
-| 0.1.0 - 0.1.4   | 0.1              |
+| 0.1.0 - 0.1.5   | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.4/setup.py` & `cqi-0.1.5/setup.py`

 * *Files identical despite different names*

