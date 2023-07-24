# Comparing `tmp/pysocklib-0.3.0.tar.gz` & `tmp/pysocklib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysocklib-0.3.0.tar", last modified: Wed Jul 19 22:32:05 2023, max compression
+gzip compressed data, was "pysocklib-0.3.1.tar", last modified: Mon Jul 24 19:41:37 2023, max compression
```

## Comparing `pysocklib-0.3.0.tar` & `pysocklib-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.158176 pysocklib-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-19 22:31:52.000000 pysocklib-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-19 22:32:05.158176 pysocklib-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-19 22:31:52.000000 pysocklib-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-19 22:31:52.000000 pysocklib-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 22:32:05.158176 pysocklib-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.154176 pysocklib-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.154176 pysocklib-0.3.0/src/pysocklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-19 22:32:05.000000 pysocklib-0.3.0/src/pysocklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-19 22:32:05.000000 pysocklib-0.3.0/src/pysocklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:32:05.000000 pysocklib-0.3.0/src/pysocklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-19 22:32:05.000000 pysocklib-0.3.0/src/pysocklib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 22:32:05.000000 pysocklib-0.3.0/src/pysocklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 22:32:05.000000 pysocklib-0.3.0/src/pysocklib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.154176 pysocklib-0.3.0/src/socketlib/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.158176 pysocklib-0.3.0/src/socketlib/basic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/basic/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/basic/receive.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/basic/send.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.158176 pysocklib-0.3.0/src/socketlib/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.158176 pysocklib-0.3.0/src/socketlib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.158176 pysocklib-0.3.0/src/socketlib/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.158176 pysocklib-0.3.0/src/socketlib/services/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/services/abstract_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/services/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:32:05.158176 pysocklib-0.3.0/src/socketlib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-19 22:31:52.000000 pysocklib-0.3.0/src/socketlib/utils/watch_dog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 19:41:24.000000 pysocklib-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-24 19:41:37.398083 pysocklib-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-24 19:41:24.000000 pysocklib-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-24 19:41:24.000000 pysocklib-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:41:37.398083 pysocklib-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.394083 pysocklib-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.394083 pysocklib-0.3.1/src/pysocklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/receive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/send.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/services/abstract_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/services/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/utils/watch_dog.py
```

### Comparing `pysocklib-0.3.0/LICENSE` & `pysocklib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.0/PKG-INFO` & `pysocklib-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysocklib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to work with socket clients and servers.
 Author-email: Daniel Ibarrola <daniel.ibarrola.sanchez@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Daniel Ibarrola Sánchez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -140,15 +140,14 @@
 Installing the development environment:
 
 ```shell
 git clone https://github.com/Daniel-Ibarrola/MServ
 python3.11 -m venv venv
 source venv/bin/activate
 pip install -r requirements/dev.txt
-cd src
-python setup.py develop
+pip install -e .
 ```
 
 ## License
 
-`socketlib` was created by Daniel Ibarrola. It is licensed under the terms
+`pysocklib` was created by Daniel Ibarrola. It is licensed under the terms
 of the MIT license.
```

### Comparing `pysocklib-0.3.0/README.md` & `pysocklib-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,14 @@
 Installing the development environment:
 
 ```shell
 git clone https://github.com/Daniel-Ibarrola/MServ
 python3.11 -m venv venv
 source venv/bin/activate
 pip install -r requirements/dev.txt
-cd src
-python setup.py develop
+pip install -e .
 ```
 
 ## License
 
-`socketlib` was created by Daniel Ibarrola. It is licensed under the terms
+`pysocklib` was created by Daniel Ibarrola. It is licensed under the terms
 of the MIT license.
```

### Comparing `pysocklib-0.3.0/pyproject.toml` & `pysocklib-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=65.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysocklib"
-version = "0.3.0"
+version = "0.3.1"
 description = "Library to work with socket clients and servers."
 readme = "README.md"
 authors = [{ name = "Daniel Ibarrola", email = "daniel.ibarrola.sanchez@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -25,22 +25,22 @@
 [project.urls]
 Homepage = "https://github.com/Daniel-Ibarrola/SocketLib.git"
 
 [project.scripts]
 socketlib = "socketlib.__main__:main"
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
-push = false
+push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"'
 ]
 "src/socketlib/__init__.py" = ["{version}"]
```

### Comparing `pysocklib-0.3.0/src/pysocklib.egg-info/PKG-INFO` & `pysocklib-0.3.1/src/pysocklib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysocklib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to work with socket clients and servers.
 Author-email: Daniel Ibarrola <daniel.ibarrola.sanchez@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Daniel Ibarrola Sánchez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -140,15 +140,14 @@
 Installing the development environment:
 
 ```shell
 git clone https://github.com/Daniel-Ibarrola/MServ
 python3.11 -m venv venv
 source venv/bin/activate
 pip install -r requirements/dev.txt
-cd src
-python setup.py develop
+pip install -e .
 ```
 
 ## License
 
-`socketlib` was created by Daniel Ibarrola. It is licensed under the terms
+`pysocklib` was created by Daniel Ibarrola. It is licensed under the terms
 of the MIT license.
```

### Comparing `pysocklib-0.3.0/src/pysocklib.egg-info/SOURCES.txt` & `pysocklib-0.3.1/src/pysocklib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/pysocklib.egg-info/entry_points.txt
 src/pysocklib.egg-info/requires.txt
 src/pysocklib.egg-info/top_level.txt
 src/socketlib/__init__.py
 src/socketlib/__main__.py
 src/socketlib/basic/__init__.py
 src/socketlib/basic/buffer.py
+src/socketlib/basic/queues.py
 src/socketlib/basic/receive.py
 src/socketlib/basic/send.py
 src/socketlib/cli/__init__.py
 src/socketlib/cli/cli.py
 src/socketlib/client/__init__.py
 src/socketlib/client/client.py
 src/socketlib/server/__init__.py
```

### Comparing `pysocklib-0.3.0/src/socketlib/basic/buffer.py` & `pysocklib-0.3.1/src/socketlib/basic/buffer.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.0/src/socketlib/cli/cli.py` & `pysocklib-0.3.1/src/socketlib/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,16 @@
         help="Whether the client or server should try to reconnect if the connection is lost."
     )
     parser.add_argument(
         "--timeout",
         "-o",
         type=float,
         default=5,
-        help="Timeout for socket receive and send operations."
+        help="Timeout in seconds for socket receive and send operations."
+             " (default (5 seconds)"
     )
     parser.add_argument(
         "--messages",
         "-m",
         type=str,
         nargs="+",
         help="A set of messages that will be sent by a client sender or server sender."
```

### Comparing `pysocklib-0.3.0/src/socketlib/client/client.py` & `pysocklib-0.3.1/src/socketlib/client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,63 +2,70 @@
 import queue
 import socket
 import threading
 import time
 from typing import Callable, Optional
 
 from socketlib.basic.buffer import Buffer
-from socketlib.basic.send import send_msg
-from socketlib.basic.receive import receive_msg
+from socketlib.basic.send import get_and_send_messages
+from socketlib.basic.receive import receive_and_enqueue
 
 
 class ClientBase:
     """ Parent class for other client classes that implements some common methods.
 
         This class should not be instantiated.
     """
 
     def __init__(
             self,
             address: tuple[str, int],
             reconnect: bool = True,
             timeout: Optional[float] = None,
-            stop: Optional[Callable[[], bool]] = lambda: False,
-            stop_reconnect: Optional[Callable[[], bool]] = lambda: False,
+            stop: Optional[Callable[[], bool]] = None,
+            stop_reconnect: Optional[Callable[[], bool]] = None,
             logger: Optional[logging.Logger] = None,
     ):
         self._address = address
         self._socket = None  # type: Optional[socket.socket]
         self._reconnect = reconnect
-        self._stop = stop
-        self._stop_reconnect = stop_reconnect
+
+        self._stop_event = threading.Event()
+        self._stop_reconnect_event = threading.Event()
+        self._stop = self._get_stop_function(stop, self._stop_event)
+        self._stop_reconnect = self._get_stop_function(
+            stop_reconnect, self._stop_reconnect_event)
+
         self._logger = logger
 
         self._run_thread = threading.Thread()
 
         self._wait_for_connection = threading.Event()
         self._connection_failed = False
         self._connect_timeout = None
 
         self._timeout = timeout  # Timeout for send and receive
 
+        self.msg_end = b"\r\n"
+
     @property
     def ip(self) -> str:
         return self._address[0]
 
     @property
     def port(self) -> int:
         return self._address[1]
 
     @property
     def run_thread(self) -> threading.Thread:
         return self._run_thread
 
     def connect(self, timeout: Optional[float] = None) -> None:
-        """ Connect to the server. This will attempt to connect to the server indefinitively
-            unless a timeout is give.
+        """ Connect to the server. This will attempt to connect to the server indefinitely
+            unless a timeout is given.
 
         """
         self._connect_timeout = timeout
         connect_thread = threading.Thread(target=self._connect_to_server, args=(timeout,), daemon=True)
         connect_thread.start()
 
     def _connect_to_server(self, timeout: Optional[float] = None) -> None:
@@ -89,24 +96,36 @@
         if self._logger is not None and not error:
             self._logger.info(
                 f"{self.__class__.__name__}: connected to {(self.ip, self.port)}"
             )
 
         self._wait_for_connection.set()
 
+    @staticmethod
+    def _get_stop_function(
+            stop: Optional[Callable[[], bool]],
+            stop_event: threading.Event
+    ) -> Callable[[], bool]:
+        if stop is None:
+            return lambda: stop_event.is_set()
+        return stop
+
     def start(self) -> None:
         """ Start this client in a new thread. """
         self._run_thread.start()
 
     def join(self) -> None:
         self._run_thread.join()
 
     def shutdown(self) -> None:
-        self._stop = lambda: True
-        self._stop_reconnect = lambda: True
+        """ Stop this client. If a custom stop function is used
+            this will not have any effect.
+        """
+        self._stop_event.set()
+        self._stop_reconnect_event.set()
         self.join()
 
     def close_connection(self) -> None:
         if self._socket is not None:
             self._socket.close()
 
     def __enter__(self):
@@ -121,24 +140,23 @@
 
     def __init__(
             self,
             address: tuple[str, int],
             received: Optional[queue.Queue[bytes]] = None,
             reconnect: bool = True,
             timeout: Optional[float] = None,
-            stop: Optional[Callable[[], bool]] = lambda: False,
+            stop: Optional[Callable[[], bool]] = None,
             logger: Optional[logging.Logger] = None,
     ):
         super().__init__(
             address=address,
             reconnect=reconnect,
             timeout=timeout,
             stop=stop,
             logger=logger)
-        self.msg_end = b"\r\n"
         self._buffer = None  # type: Optional[Buffer]
         self._received = received if received is not None else queue.Queue()
         self._run_thread = threading.Thread(target=self._recv, daemon=True)
 
     @property
     def received(self) -> queue.Queue[bytes]:
         return self._received
@@ -157,90 +175,85 @@
         if not self._connection_failed:
             self._buffer = Buffer(self._socket)
 
     def _recv(self):
         self._wait_for_connection.wait()
         if self._reconnect:
             while not self._stop_reconnect():
-                while not self._stop():
-                    error = receive_msg(
-                        self._buffer,
-                        self._received,
-                        self.msg_end,
-                        self._logger,
-                        self.__class__.__name__
-                    )
-                    if error:
-                        break
+                receive_and_enqueue(
+                    buffer=self._buffer,
+                    msg_end=self.msg_end,
+                    msg_queue=self.received,
+                    stop=self._stop,
+                    timeout=self._timeout,
+                    logger=self._logger,
+                    name=self.__class__.__name__
+                )
                 self._connect_to_server(self._connect_timeout)
         else:
-            while not self._stop():
-                error = receive_msg(
-                    self._buffer,
-                    self._received,
-                    self.msg_end,
-                    self._logger,
-                    self.__class__.__name__
-                )
-                if error:
-                    break
+            receive_and_enqueue(
+                buffer=self._buffer,
+                msg_end=self.msg_end,
+                msg_queue=self.received,
+                stop=self._stop,
+                timeout=self._timeout,
+                logger=self._logger,
+                name=self.__class__.__name__
+            )
 
 
 class ClientSender(ClientBase):
     """ A client that sends messages to a server"""
 
     def __init__(
             self,
             address: tuple[str, int],
             to_send: Optional[queue.Queue[str]] = None,
             reconnect: bool = True,
             timeout: Optional[float] = None,
-            stop: Optional[Callable[[], bool]] = lambda: False,
+            stop: Optional[Callable[[], bool]] = None,
             logger: Optional[logging.Logger] = None,
     ):
         super().__init__(
             address=address,
             reconnect=reconnect,
             timeout=timeout,
             stop=stop,
             logger=logger)
-        self.msg_end = b"\r\n"
         self._to_send = to_send if to_send is not None else queue.Queue()
         self._run_thread = threading.Thread(target=self._send, daemon=True)
 
     @property
     def to_send(self) -> queue.Queue[str]:
         return self._to_send
 
     def _send(self) -> None:
         self._wait_for_connection.wait()
         if self._reconnect:
             while not self._stop_reconnect():
-                while not self._stop():
-                    error = send_msg(
-                        self._socket,
-                        self._to_send,
-                        self.msg_end,
-                        self._logger,
-                        self.__class__.__name__
-                    )
-                    if error:
-                        break
+                get_and_send_messages(
+                    sock=self._socket,
+                    msg_end=self.msg_end,
+                    msg_queue=self.to_send,
+                    stop=self._stop,
+                    timeout=self._timeout,
+                    logger=self._logger,
+                    name=self.__class__.__name__
+                )
                 self._connect_to_server(self._connect_timeout)
         else:
-            while not self._stop():
-                error = send_msg(
-                    self._socket,
-                    self._to_send,
-                    self.msg_end,
-                    self._logger,
-                    self.__class__.__name__
-                )
-                if error:
-                    break
+            get_and_send_messages(
+                sock=self._socket,
+                msg_end=self.msg_end,
+                msg_queue=self.to_send,
+                stop=self._stop,
+                timeout=self._timeout,
+                logger=self._logger,
+                name=self.__class__.__name__
+            )
 
     def start_main_thread(self) -> None:
         """ Start this client in the main thread"""
         self._send()
 
 
 class Client(ClientBase):
@@ -250,26 +263,29 @@
     def __init__(
             self,
             address: tuple[str, int],
             received: Optional[queue.Queue[bytes]] = None,
             to_send: Optional[queue.Queue[str]] = None,
             reconnect: bool = True,
             timeout: Optional[float] = None,
-            stop_receive: Callable[[], bool] = lambda: False,
-            stop_send: Callable[[], bool] = lambda: False,
+            stop_receive: Callable[[], bool] = None,
+            stop_send: Callable[[], bool] = None,
             logger: Optional[logging.Logger] = None,
     ):
         super().__init__(address=address, reconnect=reconnect, timeout=timeout, logger=logger)
         self.msg_end = b"\r\n"
         self._buffer = None  # type: Optional[Buffer]
 
         self._received = received if received is not None else queue.Queue()
         self._to_send = to_send if to_send is not None else queue.Queue()
-        self._stop_receive = stop_receive
-        self._stop_send = stop_send
+
+        self._stop_receive_event = threading.Event()
+        self._stop_send_event = threading.Event()
+        self._stop_receive = self._get_stop_function(stop_receive, self._stop_receive_event)
+        self._stop_send = self._get_stop_function(stop_send, self._stop_send_event)
 
         self._send_thread = threading.Thread(target=self._send, daemon=True)
         self._recv_thread = threading.Thread(target=self._recv, daemon=True)
 
     @property
     def to_send(self) -> queue.Queue[str]:
         return self._to_send
@@ -295,78 +311,74 @@
         super()._connect_to_server(timeout)
         self._buffer = Buffer(self._socket)
 
     def _send(self) -> None:
         self._wait_for_connection.wait()
         if self._reconnect:
             while not self._stop_reconnect():
-                while not self._stop_send():
-                    error = send_msg(
-                        self._socket,
-                        self._to_send,
-                        self.msg_end,
-                        self._logger,
-                        self.__class__.__name__
-                    )
-                    if error:
-                        break
+                get_and_send_messages(
+                    sock=self._socket,
+                    msg_end=self.msg_end,
+                    msg_queue=self.to_send,
+                    stop=self._stop_send,
+                    timeout=self._timeout,
+                    logger=self._logger,
+                    name=self.__class__.__name__
+                )
                 self._wait_for_connection.clear()
                 self._connect_to_server(self._connect_timeout)
         else:
-            while not self._stop_send():
-                error = send_msg(
-                    self._socket,
-                    self._to_send,
-                    self.msg_end,
-                    self._logger,
-                    self.__class__.__name__
-                )
-                if error:
-                    break
+            get_and_send_messages(
+                sock=self._socket,
+                msg_end=self.msg_end,
+                msg_queue=self.to_send,
+                stop=self._stop_send,
+                timeout=self._timeout,
+                logger=self._logger,
+                name=self.__class__.__name__
+            )
 
     def _recv(self) -> None:
         self._wait_for_connection.wait()
         if self._reconnect:
             while not self._stop_reconnect():
-                while not self._stop_receive():
-                    error = receive_msg(
-                        self._buffer,
-                        self._received,
-                        self.msg_end,
-                        self._logger,
-                        self.__class__.__name__
-                    )
-                    if error:
-                        self._wait_for_connection.clear()
-                        break
+                receive_and_enqueue(
+                    buffer=self._buffer,
+                    msg_end=self.msg_end,
+                    msg_queue=self.received,
+                    stop=self._stop_receive,
+                    timeout=self._timeout,
+                    logger=self._logger,
+                    name=self.__class__.__name__
+                )
                 self._wait_for_connection.wait()
         else:
-            while not self._stop_receive():
-                error = receive_msg(
-                    self._buffer,
-                    self._received,
-                    self.msg_end,
-                    self._logger,
-                    self.__class__.__name__
-                )
-                if error:
-                    break
+            receive_and_enqueue(
+                buffer=self._buffer,
+                msg_end=self.msg_end,
+                msg_queue=self.received,
+                stop=self._stop_receive,
+                timeout=self._timeout,
+                logger=self._logger,
+                name=self.__class__.__name__
+            )
 
     def start(self) -> None:
         """ Start this client in a new thread. """
         self._recv_thread.start()
         self._send_thread.start()
 
     def join(self) -> None:
         self._recv_thread.join()
         self._send_thread.join()
 
     def shutdown(self) -> None:
-        self._stop_send = lambda: True
-        self._stop_receive = lambda: True
+        self._stop_receive_event.set()
+        self._stop_send_event.set()
+        self._stop_reconnect_event.set()
         self.join()
 
 
 class ClientReportAlive(Client):
     """ Client that receives messages and sends and alive message periodically
         to the server
     """
```

### Comparing `pysocklib-0.3.0/src/socketlib/server/server.py` & `pysocklib-0.3.1/src/socketlib/server/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 import queue
 import logging
 import socket
 import threading
 from typing import Callable, Optional
 
 from socketlib.basic.buffer import Buffer
-from socketlib.basic.receive import receive_msg
-from socketlib.basic.send import send_msg
+from socketlib.basic.receive import receive_and_enqueue
+from socketlib.basic.send import get_and_send_messages
 
 
 class ServerBase:
     """ Parent class for other server classes that implements some common methods.
 
         This class should not be instantiated.
     """
 
     def __init__(
             self,
             address: tuple[str, int],
             reconnect: bool = True,
             timeout: Optional[float] = None,
-            stop: Optional[Callable[[], bool]] = lambda: False,
-            stop_reconnect: Optional[Callable[[], bool]] = lambda: False,
+            stop: Optional[Callable[[], bool]] = None,
+            stop_reconnect: Optional[Callable[[], bool]] = None,
             logger: Optional[logging.Logger] = None,
     ):
         self._address = address
         self._socket = None  # type: Optional[socket.socket]
         self._connection = None  # The client connection
         self._conn_details = None
-        self._stop = stop
-        self._stop_reconnect = stop_reconnect
+
+        self._stop_event = threading.Event()
+        self._stop_reconnect_event = threading.Event()
+        self._stop = self._get_stop_function(stop, self._stop_event)
+        self._stop_reconnect = self._get_stop_function(
+            stop_reconnect, self._stop_reconnect_event)
 
         self._reconnect = reconnect
         self._logger = logger
 
         self._run_thread = threading.Thread()
 
         self._timeout = timeout  # Timeout for send and receive
 
+        self.msg_end = b"\r\n"
+
     @property
     def ip(self) -> str:
         return self._address[0]
 
     @property
     def port(self) -> int:
         return self._address[1]
@@ -70,59 +76,67 @@
                 f"connection accepted from {self._conn_details}"
             )
 
     def start(self) -> None:
         """ Start this server in a new thread.
 
             If this method is used, there is no need to call the `listen` and `accept_connection`
-            as they are called under the hood.
+            as they are called behind the scenes.
         """
         self.listen()
         self._run_thread.start()
 
     def join(self) -> None:
         self._run_thread.join()
 
     def shutdown(self) -> None:
-        self._stop = lambda: True
-        self._stop_reconnect = lambda: True
+        self._stop_event.set()
+        self._stop_reconnect_event.set()
         self.join()
 
     def __enter__(self):
         return self
 
     def close_connection(self) -> None:
         if self._connection is not None:
             self._connection.close()
         if self._socket is not None:
             self._socket.close()
 
+    @staticmethod
+    def _get_stop_function(
+            stop: Optional[Callable[[], bool]],
+            stop_event: threading.Event
+    ) -> Callable[[], bool]:
+        if stop is None:
+            return lambda: stop_event.is_set()
+        return stop
+
     def __exit__(self, *args):
         self.close_connection()
 
 
 class ServerReceiver(ServerBase):
     """ A server that receives messages from a single client.
     """
     def __init__(
             self,
             address: tuple[str, int],
             received: Optional[queue.Queue[bytes]] = None,
             reconnect: bool = True,
             timeout: Optional[float] = None,
-            stop: Optional[Callable[[], bool]] = lambda: False,
+            stop: Optional[Callable[[], bool]] = None,
             logger: Optional[logging.Logger] = None,
     ):
         super().__init__(
             address=address,
             reconnect=reconnect,
             timeout=timeout,
             stop=stop,
             logger=logger)
-        self.msg_end = b"\r\n"
         self._buffer = None  # type: Optional[Buffer]
         self._received = received if received is not None else queue.Queue()
         self._run_thread = threading.Thread(
             target=self._recv, daemon=True
         )
 
     @property
@@ -133,37 +147,35 @@
         super().accept_connection()
         self._buffer = Buffer(self._connection)
 
     def _recv(self):
         if self._reconnect:
             while not self._stop_reconnect():
                 self.accept_connection()
-                while not self._stop():
-                    error = receive_msg(
-                        self._buffer,
-                        self._received,
-                        self.msg_end,
-                        self._logger,
-                        self.__class__.__name__
-                    )
-                    if error:
-                        break
+                receive_and_enqueue(
+                    buffer=self._buffer,
+                    msg_end=self.msg_end,
+                    msg_queue=self.received,
+                    stop=self._stop,
+                    timeout=self._timeout,
+                    logger=self._logger,
+                    name=self.__class__.__name__
+                )
                 self.listen()
         else:
             self.accept_connection()
-            while not self._stop():
-                error = receive_msg(
-                    self._buffer,
-                    self._received,
-                    self.msg_end,
-                    self._logger,
-                    self.__class__.__name__
-                )
-                if error:
-                    break
+            receive_and_enqueue(
+                buffer=self._buffer,
+                msg_end=self.msg_end,
+                msg_queue=self.received,
+                stop=self._stop,
+                timeout=self._timeout,
+                logger=self._logger,
+                name=self.__class__.__name__
+            )
 
     def start_main_thread(self) -> None:
         self.listen()
         self._recv()
 
 
 class ServerSender(ServerBase):
@@ -171,15 +183,15 @@
 
     def __init__(
             self,
             address: tuple[str, int],
             to_send: Optional[queue.Queue[str]] = None,
             reconnect: bool = True,
             timeout: Optional[float] = None,
-            stop: Optional[Callable[[], bool]] = lambda: False,
+            stop: Optional[Callable[[], bool]] = None,
             logger: Optional[logging.Logger] = None,
     ):
         super().__init__(
             address=address,
             reconnect=reconnect,
             timeout=timeout,
             stop=stop,
@@ -198,62 +210,62 @@
         self.listen()
         self._send()
 
     def _send(self):
         if self._reconnect:
             while not self._stop_reconnect():
                 self.accept_connection()
-                while not self._stop():
-                    error = send_msg(
-                        self._connection,
-                        self._to_send,
-                        self.msg_end,
-                        self._logger,
-                        self.__class__.__name__
-                    )
-                    if error:
-                        break
+                get_and_send_messages(
+                    sock=self._connection,
+                    msg_end=self.msg_end,
+                    msg_queue=self.to_send,
+                    stop=self._stop,
+                    timeout=self._timeout,
+                    logger=self._logger,
+                    name=self.__class__.__name__
+                )
                 self.listen()
         else:
             self.accept_connection()
-            while not self._stop():
-                error = send_msg(
-                    self._connection,
-                    self._to_send,
-                    self.msg_end,
-                    self._logger,
-                    self.__class__.__name__
-                )
-                if error:
-                    break
+            get_and_send_messages(
+                sock=self._connection,
+                msg_end=self.msg_end,
+                msg_queue=self.to_send,
+                stop=self._stop,
+                timeout=self._timeout,
+                logger=self._logger,
+                name=self.__class__.__name__
+            )
 
 
 class Server(ServerBase):
     """ A server that sends and receives messages to and from a single client.
     """
 
     def __init__(
             self,
             address: tuple[str, int],
             received: Optional[queue.Queue[bytes]] = None,
             to_send: Optional[queue.Queue[str]] = None,
             reconnect: bool = True,
             timeout: Optional[float] = None,
-            stop_receive: Optional[Callable[[], bool]] = lambda: False,
-            stop_send: Optional[Callable[[], bool]] = lambda: False,
+            stop_receive: Optional[Callable[[], bool]] = None,
+            stop_send: Optional[Callable[[], bool]] = None,
             logger: Optional[logging.Logger] = None,
     ):
         super().__init__(address=address, reconnect=reconnect, timeout=timeout, logger=logger)
-        self.msg_end = b"\r\n"
         self._buffer = None  # type: Optional[Buffer]
 
         self._received = received if received is not None else queue.Queue()
         self._to_send = to_send if to_send is not None else queue.Queue()
-        self._stop_receive = stop_receive
-        self._stop_send = stop_send
+
+        self._stop_receive_event = threading.Event()
+        self._stop_send_event = threading.Event()
+        self._stop_receive = self._get_stop_function(stop_receive, self._stop_receive_event)
+        self._stop_send = self._get_stop_function(stop_send, self._stop_send_event)
 
         self._send_thread = threading.Thread(target=self._send, daemon=True)
         self._recv_thread = threading.Thread(target=self._recv, daemon=True)
         self._connected = threading.Event()
 
     @property
     def to_send(self) -> queue.Queue[str]:
@@ -271,65 +283,61 @@
     def receive_thread(self) -> threading.Thread:
         return self._recv_thread
 
     def _send(self) -> None:
         self._connected.wait()
         if self._reconnect:
             while not self._stop_reconnect():
-                while not self._stop_send():
-                    error = send_msg(
-                        self._connection,
-                        self._to_send,
-                        self.msg_end,
-                        self._logger,
-                        self.__class__.__name__
-                    )
-                    if error:
-                        break
+                get_and_send_messages(
+                    sock=self._connection,
+                    msg_end=self.msg_end,
+                    msg_queue=self.to_send,
+                    stop=self._stop_send,
+                    timeout=self._timeout,
+                    logger=self._logger,
+                    name=self.__class__.__name__
+                )
                 self._connected.clear()
                 self.listen()
                 self.accept_connection()
         else:
-            while not self._stop_send():
-                error = send_msg(
-                    self._connection,
-                    self._to_send,
-                    self.msg_end,
-                    self._logger,
-                    self.__class__.__name__
-                )
-                if error:
-                    break
+            get_and_send_messages(
+                sock=self._connection,
+                msg_end=self.msg_end,
+                msg_queue=self.to_send,
+                stop=self._stop_send,
+                timeout=self._timeout,
+                logger=self._logger,
+                name=self.__class__.__name__
+            )
 
     def _recv(self):
         self._connected.wait()
         if self._reconnect:
             while not self._stop_reconnect():
-                while not self._stop_receive():
-                    error = receive_msg(
-                        self._buffer,
-                        self._received,
-                        self.msg_end,
-                        self._logger,
-                        self.__class__.__name__
-                    )
-                    if error:
-                        break
+                receive_and_enqueue(
+                    buffer=self._buffer,
+                    msg_end=self.msg_end,
+                    msg_queue=self.received,
+                    stop=self._stop_receive,
+                    timeout=self._timeout,
+                    logger=self._logger,
+                    name=self.__class__.__name__
+                )
                 self._connected.wait()
         else:
-            while not self._stop_receive():
-                error = receive_msg(
-                    self._buffer,
-                    self._received,
-                    self.msg_end,
-                    self._logger,
-                    self.__class__.__name__
-                )
-                if error:
-                    break
+            receive_and_enqueue(
+                buffer=self._buffer,
+                msg_end=self.msg_end,
+                msg_queue=self.received,
+                stop=self._stop_receive,
+                timeout=self._timeout,
+                logger=self._logger,
+                name=self.__class__.__name__
+            )
 
     def accept_connection(self) -> None:
         super().accept_connection()
         self._buffer = Buffer(self._connection)
         self._connected.set()
 
     def start(self) -> None:
@@ -341,11 +349,11 @@
         self._send_thread.start()
 
     def join(self) -> None:
         self._recv_thread.join()
         self._send_thread.join()
 
     def shutdown(self) -> None:
-        self._stop_send = lambda: True
-        self._stop_receive = lambda: True
-        self._stop_reconnect = lambda: True
+        self._stop_receive_event.set()
+        self._stop_send_event.set()
+        self._stop_reconnect_event.set()
         self.join()
```

### Comparing `pysocklib-0.3.0/src/socketlib/services/abstract_service.py` & `pysocklib-0.3.1/src/socketlib/services/abstract_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,17 +67,7 @@
         self._process_thread.join()
 
     def shutdown(self) -> None:
         self._stop = lambda: True
         self.join()
         if self._logger is not None:
             self._logger.debug(f"Shutting down {self.__class__.__name__}")
-
-    @staticmethod
-    def _get_from_queue(data_queue: queue, timeout: float) -> Optional[Any]:
-        """ Get an item from the queue. If timeout expires and there is
-            nothing in the queue returns None.
-        """
-        try:
-            return data_queue.get(timeout=timeout)
-        except queue.Empty:
-            pass
```

### Comparing `pysocklib-0.3.0/src/socketlib/services/samples.py` & `pysocklib-0.3.1/src/socketlib/services/samples.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import logging
 import queue
 import time
 from typing import Callable, Optional
+
 from socketlib.services.abstract_service import AbstractService
+from socketlib.basic.queues import get_from_queue
 
 
 class MessageLogger(AbstractService):
 
-    def __init__(self, messages: queue.Queue, logger: logging.Logger):
+    def __init__(self, messages: queue.Queue[bytes], logger: logging.Logger):
         super().__init__(in_queue=messages, logger=logger)
 
+    @property
+    def messages(self) -> queue.Queue[bytes]:
+        return self._in
+
     def _handle_message(self):
         while not self._stop():
-            msg = self._in.get()
-            self._logger.info(f"New message {msg}")
+            msg = get_from_queue(self.messages, 2)
+            if msg is not None:
+                msg_str = msg.decode()
+                self._logger.info(msg_str)
 
 
 class MessageGenerator(AbstractService):
 
     def __init__(self, messages: queue.Queue, logger: logging.Logger, name: Optional[str] = ""):
         super().__init__(out_queue=messages, logger=logger)
         self.name = name
```

### Comparing `pysocklib-0.3.0/src/socketlib/utils/logger.py` & `pysocklib-0.3.1/src/socketlib/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.0/src/socketlib/utils/watch_dog.py` & `pysocklib-0.3.1/src/socketlib/utils/watch_dog.py`

 * *Files identical despite different names*

