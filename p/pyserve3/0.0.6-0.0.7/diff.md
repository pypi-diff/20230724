# Comparing `tmp/pyserve3-0.0.6.tar.gz` & `tmp/pyserve3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserve3-0.0.6.tar", last modified: Tue May  9 00:55:03 2023, max compression
+gzip compressed data, was "pyserve3-0.0.7.tar", last modified: Mon Jul 24 17:13:40 2023, max compression
```

## Comparing `pyserve3-0.0.6.tar` & `pyserve3-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:55:03.437190 pyserve3-0.0.6/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-03-26 23:32:22.000000 pyserve3-0.0.6/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-05-09 00:55:03.433190 pyserve3-0.0.6/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)      944 2023-03-19 20:01:09.000000 pyserve3-0.0.6/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:55:03.433190 pyserve3-0.0.6/pyserve/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5942 2023-05-09 00:45:08.000000 pyserve3-0.0.6/pyserve/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2139 2023-05-09 00:45:25.000000 pyserve3-0.0.6/pyserve/abc.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6849 2023-05-09 00:45:41.000000 pyserve3-0.0.6/pyserve/threading.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2997 2023-05-06 22:37:04.000000 pyserve3-0.0.6/pyserve/transport.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:55:03.433190 pyserve3-0.0.6/pyserve3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-05-09 00:55:03.000000 pyserve3-0.0.6/pyserve3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      231 2023-05-09 00:55:03.000000 pyserve3-0.0.6/pyserve3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-05-09 00:55:03.000000 pyserve3-0.0.6/pyserve3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2023-05-09 00:55:03.000000 pyserve3-0.0.6/pyserve3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-05-09 00:55:03.437190 pyserve3-0.0.6/setup.cfg
--rw-r--r--   0 andrew    (1000) andrew    (1000)      674 2023-05-09 00:54:46.000000 pyserve3-0.0.6/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:13:40.887075 pyserve3-0.0.7/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-03-26 23:32:22.000000 pyserve3-0.0.7/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1752 2023-07-24 17:13:40.887075 pyserve3-0.0.7/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      944 2023-03-19 20:01:09.000000 pyserve3-0.0.7/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:13:40.887075 pyserve3-0.0.7/pyserve/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5942 2023-05-27 08:48:26.000000 pyserve3-0.0.7/pyserve/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2191 2023-07-20 00:35:10.000000 pyserve3-0.0.7/pyserve/abc.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7792 2023-07-20 00:35:10.000000 pyserve3-0.0.7/pyserve/threading.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3990 2023-07-20 00:35:10.000000 pyserve3-0.0.7/pyserve/transport.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:13:40.887075 pyserve3-0.0.7/pyserve3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1752 2023-07-24 17:13:40.000000 pyserve3-0.0.7/pyserve3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      262 2023-07-24 17:13:40.000000 pyserve3-0.0.7/pyserve3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-07-24 17:13:40.000000 pyserve3-0.0.7/pyserve3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       17 2023-07-24 17:13:40.000000 pyserve3-0.0.7/pyserve3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2023-07-24 17:13:40.000000 pyserve3-0.0.7/pyserve3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-07-24 17:13:40.887075 pyserve3-0.0.7/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      717 2023-07-24 17:02:39.000000 pyserve3-0.0.7/setup.py
```

### Comparing `pyserve3-0.0.6/LICENSE` & `pyserve3-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyserve3-0.0.6/PKG-INFO` & `pyserve3-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: pyserve3
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unify SocketServer Implementations based on a Session Model
 Home-page: https://github.com/imgurbot12/pyserve
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
+Description: pyserve
+        --------
+        Unify SocketServer Implementations based on a Session Model
+        
+        ### Install
+        
+        ```bash
+        pip install pyserve3
+        ```
+        
+        ### Example
+        
+        ```python
+        from pyserve import *
+        from typing import Optional
+        
+        class EchoServer(Session):
+            
+            def connection_made(self, addr: Address, writer: Writer):
+                print('connection made!', addr, writer)
+                self.addr   = addr
+                self.writer = writer
+        
+            def data_recieved(self, data: bytes):
+                print(f'recieved {data!r} from {self.addr}')
+                self.writer.write(data)
+                self.writer.close()
+        
+            def connection_lost(self, err: Optional[Exception]):
+                print('connection lost!', self.addr, err)
+        
+        # run sync
+        # listen_udp_threaded(('127.0.0.1', 8000), EchoServer)
+        # listen_tcp_threaded(('127.0.0.1', 8000), EchoServer)
+        
+        # run async
+        import asyncio
+        # asyncio.run(listen_udp_async(('127.0.0.1', 8000), EchoServer))
+        asyncio.run(listen_tcp_async(('127.0.0.1', 8000), EchoServer))
+        ```
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-pyserve
---------
-Unify SocketServer Implementations based on a Session Model
-
-### Install
-
-```bash
-pip install pyserve3
-```
-
-### Example
-
-```python
-from pyserve import *
-from typing import Optional
-
-class EchoServer(Session):
-    
-    def connection_made(self, addr: Address, writer: Writer):
-        print('connection made!', addr, writer)
-        self.addr   = addr
-        self.writer = writer
-
-    def data_recieved(self, data: bytes):
-        print(f'recieved {data!r} from {self.addr}')
-        self.writer.write(data)
-        self.writer.close()
-
-    def connection_lost(self, err: Optional[Exception]):
-        print('connection lost!', self.addr, err)
-
-# run sync
-# listen_udp_threaded(('127.0.0.1', 8000), EchoServer)
-# listen_tcp_threaded(('127.0.0.1', 8000), EchoServer)
-
-# run async
-import asyncio
-# asyncio.run(listen_udp_async(('127.0.0.1', 8000), EchoServer))
-asyncio.run(listen_tcp_async(('127.0.0.1', 8000), EchoServer))
-```
-
```

### Comparing `pyserve3-0.0.6/README.md` & `pyserve3-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyserve3-0.0.6/pyserve/__init__.py` & `pyserve3-0.0.7/pyserve/__init__.py`

 * *Files identical despite different names*

### Comparing `pyserve3-0.0.6/pyserve/abc.py` & `pyserve3-0.0.7/pyserve/abc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 
 """
 import socket
+from ssl import SSLContext
 from abc import abstractmethod
 from collections import namedtuple
 from typing import Tuple, Protocol, Optional, Union
 
 #** Variables **#
 __all__ = [
     'modify_socket',
@@ -46,43 +47,43 @@
 
 #** Classes **#
 
 class Writer(Protocol):
     """
     abstract data-writing implementation for single server connection
     """
+    
+    @abstractmethod
+    def using_tls(self) -> bool:
+        raise NotImplementedError
+
+    @abstractmethod
+    def start_tls(self, context: SSLContext):
+        raise NotImplementedError
 
     @abstractmethod
     def write(self, data: bytes):
         raise NotImplementedError
     
     @abstractmethod
     def close(self):
         raise NotImplementedError
-
+ 
     @abstractmethod
     def is_closing(self) -> bool:
         raise NotImplementedError
 
 class UdpWriter(Writer, Protocol):
     """
     abstract data-writing implementation for udp server connection
     """
 
     @abstractmethod
     def write(self, data: bytes, addr: Optional[AnyAddr] = None):
         raise NotImplementedError
-    
-    @abstractmethod
-    def close(self):
-        raise NotImplementedError
-
-    @abstractmethod
-    def is_closing(self) -> bool:
-        raise NotImplementedError
 
 class Session(Protocol):
     """
     abstract session-manager implemention for single server connection
     """
     
     @abstractmethod
```

### Comparing `pyserve3-0.0.6/pyserve/threading.py` & `pyserve3-0.0.7/pyserve/threading.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Threading Implementations of session-based servers
 """
 import socket
 import socketserver
-from ssl import SSLContext
-from dataclasses import dataclass, field
-from typing import Type, Optional, Dict, Any, ClassVar
+from ssl import SSLContext, SSLSocket
+from typing import Type, Optional, Dict, Any, ClassVar, Protocol
+
+from pyderive import dataclass, field
 
 from .abc import *
 
 #** Variables **#
 __all__ = ['UdpThreadServer', 'TcpThreadServer']
 
 #** Functions **#
@@ -33,44 +34,50 @@
         args=args,
         kwargs=kwargs,
         blocksize=blocksize,
     ))
 
 #** Classes **#
 
-@dataclass
-class UdpWriter(UdpWriter):
-    addr: Address
-    sock: socket.socket
-    closing: bool = False
+class BaseWriter(Writer, Protocol):
+    sock:    socket.socket
+    closing: bool
+    
+    def using_tls(self) -> bool:
+        return isinstance(self.sock, SSLSocket)
 
-    def write(self, data: bytes, addr: Optional[AnyAddr] = None):
-        self.sock.sendto(data, addr or self.addr)
+    def start_tls(self, context: SSLContext):
+        self.sock = context.wrap_socket(self.sock, server_side=True)
 
     def close(self):
-        self.sock.close()
         self.closing = True
+        self.sock.close()
 
     def is_closing(self) -> bool:
         return self.closing
 
-@dataclass
-class TcpWriter(Writer):
+@dataclass(slots=True)
+class UdpWriter(UdpWriter, BaseWriter):
+    addr: Address
     sock: socket.socket
     closing: bool = False
+    
+    def start_tls(self, context: SSLContext):
+        raise NotImplementedError('Cannot Use SSL over UDP')
 
-    def write(self, data: bytes):
-        self.sock.sendall(data)
+    def write(self, data: bytes, addr: Optional[AnyAddr] = None):
+        self.sock.sendto(data, addr or self.addr)
 
-    def close(self):
-        self.closing = True
-        self.sock.close()
+@dataclass(slots=True)
+class TcpWriter(BaseWriter):
+    sock: socket.socket
+    closing: bool = False
 
-    def is_closing(self) -> bool:
-        return self.closing
+    def write(self, data: bytes):
+        self.sock.sendall(data)
 
 class BaseRequestHandler(socketserver.BaseRequestHandler):
     factory:   Type[Session]
     args:      tuple           
     kwargs:    Dict[str, Any]
     blocksize: int
 
@@ -78,28 +85,28 @@
         """configure and generate session w/ information collected"""
         self.addr:   Address = Address(*self.client_address)
         self.writer: Writer
         self.error:  Optional[Exception] = None
         # spawn session object
         self.session = self.factory(*self.args, **self.kwargs)
         self.session.connection_made(self.addr, self.writer)
-    
+ 
     def finish(self):
         """notify that connection disconnected"""
         self.session.connection_lost(self.error)
 
 class UdpHandler(BaseRequestHandler):
-    
+ 
     def setup(self):
         """handle connection spawn"""
         self.addr    = Address(*self.client_address) 
         self.sock    = self.request[1]
         self.writer: UdpWriter = UdpWriter(self.addr, self.sock)
         super().setup()
-    
+ 
     def handle(self):
         """handle single inbound udp packet"""
         try:
             data = self.request[0]
             self.session.data_recieved(data)
         except socket.error as e:
             self.error = e
@@ -114,15 +121,15 @@
         self.writer: TcpWriter = TcpWriter(self.sock)
         super().setup()
 
     def handle(self):
         """handle subsequent reads of inbound data"""
         while not self.writer.closing:
             try:
-                data = self.sock.recv(self.blocksize)
+                data = self.writer.sock.recv(self.blocksize)
                 if not data:
                     break
                 self.session.data_recieved(data)
             except socket.error as e:
                 self.error = e
                 if not self.writer.closing:
                     self.writer.close()
@@ -137,14 +144,15 @@
     args:       tuple          = field(default_factory=tuple)
     kwargs:     Dict[str, Any] = field(default_factory=dict)
     interface:  Optional[str]  = None
     reuse_port: bool           = False
     blocksize: int             = 8192
  
     def __post_init__(self):
+        self.daemon_threads   = True
         self.max_packet_size  = self.blocksize
         self.allow_reuse_port = self.reuse_port
 
     def new_handler(self) -> Type[BaseRequestHandler]:
         return new_handler(
             base=self.handler, 
             factory=self.factory, 
@@ -182,18 +190,28 @@
     def get_request(self):
         """respawn socket after socket error to prevent infinite hanging loop"""
         try:
             return super().get_request()
         except socket.error as e:
             self.rebuild_socket(self)
             raise e
+ 
+    def serve_forever(self, poll_interval: float = 0.5):
+        """
+        polls server forever until its closed by something else
 
-    def shutdown(self):
+        :param poll_interval: how often server polls for close
+        """
+        try:
+            return super().serve_forever(poll_interval)
+        finally:
+            self.cleanup()
+
+    def cleanup(self):
         """override shutdown behavior"""
-        super().shutdown()
         self.socket.close()
         self.server_close()
 
 @dataclass
 class TcpThreadServer(BaseThreadServer, socketserver.TCPServer):
     handler = TcpHandler
 
@@ -221,14 +239,24 @@
             modify_socket(sock, self.timeout, None)
             return (sock, addr)
         except socket.timeout as e:
             raise e
         except socket.error as e:
             self.rebuild_socket(self)
             raise e
+ 
+    def serve_forever(self, poll_interval: float = 0.5):
+        """
+        polls server forever until its closed by something else
+
+        :param poll_interval: how often server polls for close
+        """
+        try:
+            return super().serve_forever(poll_interval)
+        finally:
+            self.cleanup()
 
-    def shutdown(self):
+    def cleanup(self):
         """override shutdown behavior"""
-        super().shutdown()
         self.socket.shutdown(socket.SHUT_RDWR)
         self.socket.close()
         self.server_close()
```

### Comparing `pyserve3-0.0.6/pyserve/transport.py` & `pyserve3-0.0.7/pyserve/transport.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,67 @@
 """
 AsyncIO Implementations of session-based servers
 """
 import asyncio
-from dataclasses import dataclass, field
-from typing import Type, Optional, Dict, Any
+from ssl import SSLContext
+from typing import Type, Optional, Dict, Any, Protocol
+
+from pyderive import dataclass, field
 
 from .abc import * 
 
 #** Variables **#
 __all__ = ['UdpProtocol', 'TcpProtocol']
 
 #** Classes **#
 
-@dataclass
-class UdpWriter(UdpWriter):
-    addr:      Address
-    transport: asyncio.DatagramTransport
+class BaseWriter(Writer, Protocol):
+    transport: asyncio.Transport
+ 
+    def using_tls(self) -> bool:
+        return 'ssl' in self.transport.__class__.__name__.lower()
 
-    def write(self, data: bytes, addr: Optional[AnyAddr] = None):
-        self.transport.sendto(data, addr or self.addr)
+    def start_tls(self, context: SSLContext):
+        protocol  = self.transport.get_protocol()
+        loop      = asyncio.get_event_loop()
+        future    = loop.start_tls(
+            transport=self.transport,
+            protocol=protocol,
+            sslcontext=context,
+            server_side=True,
+        )
+        def callback(task: asyncio.Task):
+            self.transport = task.result()
+        task = loop.create_task(future)
+        task.add_done_callback(callback)
 
     def close(self):
         self.transport.close()
 
     def is_closing(self) -> bool:
         return self.transport.is_closing()
 
+@dataclass(slots=True)
+class UdpWriter(UdpWriter, BaseWriter):
+    addr:      Address
+    transport: asyncio.DatagramTransport 
+ 
+    def start_tls(self, context: SSLContext):
+        raise NotImplementedError('Cannot Use SSL over UDP')
+
+    def write(self, data: bytes, addr: Optional[AnyAddr] = None):
+        self.transport.sendto(data, addr or self.addr)
+
+@dataclass(slots=True)
+class TcpWriter(BaseWriter):
+    transport: asyncio.Transport 
+
+    def write(self, data: bytes):
+        self.transport.write(data)
+
 @dataclass
 class BaseProtocol:
     factory:   Type[Session]
     args:      tuple           = field(default_factory=tuple)
     kwargs:    Dict[str, Any]  = field(default_factory=dict)
 
     def test_factory(self):
@@ -76,15 +108,15 @@
         # collect attributes and prepare socket for session
         address = Address(*transport.get_extra_info('peername'))
         # handle modifying socket and making changes for handling
         if self.timeout is not None:
             self.set_timeout(self.timeout, transport)
         # generate session w/ attributes and notify on connection-made
         self.session = self.factory(*self.args, **self.kwargs)
-        self.session.connection_made(address, transport)
+        self.session.connection_made(address, TcpWriter(transport))
 
     def data_received(self, data: bytes):
         """"""
         self.session.data_recieved(data)
 
     def connection_lost(self, err: Optional[Exception]):
         """"""
```

### Comparing `pyserve3-0.0.6/pyserve3.egg-info/PKG-INFO` & `pyserve3-0.0.7/pyserve3.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: pyserve3
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unify SocketServer Implementations based on a Session Model
 Home-page: https://github.com/imgurbot12/pyserve
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
+Description: pyserve
+        --------
+        Unify SocketServer Implementations based on a Session Model
+        
+        ### Install
+        
+        ```bash
+        pip install pyserve3
+        ```
+        
+        ### Example
+        
+        ```python
+        from pyserve import *
+        from typing import Optional
+        
+        class EchoServer(Session):
+            
+            def connection_made(self, addr: Address, writer: Writer):
+                print('connection made!', addr, writer)
+                self.addr   = addr
+                self.writer = writer
+        
+            def data_recieved(self, data: bytes):
+                print(f'recieved {data!r} from {self.addr}')
+                self.writer.write(data)
+                self.writer.close()
+        
+            def connection_lost(self, err: Optional[Exception]):
+                print('connection lost!', self.addr, err)
+        
+        # run sync
+        # listen_udp_threaded(('127.0.0.1', 8000), EchoServer)
+        # listen_tcp_threaded(('127.0.0.1', 8000), EchoServer)
+        
+        # run async
+        import asyncio
+        # asyncio.run(listen_udp_async(('127.0.0.1', 8000), EchoServer))
+        asyncio.run(listen_tcp_async(('127.0.0.1', 8000), EchoServer))
+        ```
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-pyserve
---------
-Unify SocketServer Implementations based on a Session Model
-
-### Install
-
-```bash
-pip install pyserve3
-```
-
-### Example
-
-```python
-from pyserve import *
-from typing import Optional
-
-class EchoServer(Session):
-    
-    def connection_made(self, addr: Address, writer: Writer):
-        print('connection made!', addr, writer)
-        self.addr   = addr
-        self.writer = writer
-
-    def data_recieved(self, data: bytes):
-        print(f'recieved {data!r} from {self.addr}')
-        self.writer.write(data)
-        self.writer.close()
-
-    def connection_lost(self, err: Optional[Exception]):
-        print('connection lost!', self.addr, err)
-
-# run sync
-# listen_udp_threaded(('127.0.0.1', 8000), EchoServer)
-# listen_tcp_threaded(('127.0.0.1', 8000), EchoServer)
-
-# run async
-import asyncio
-# asyncio.run(listen_udp_async(('127.0.0.1', 8000), EchoServer))
-asyncio.run(listen_tcp_async(('127.0.0.1', 8000), EchoServer))
-```
-
```

