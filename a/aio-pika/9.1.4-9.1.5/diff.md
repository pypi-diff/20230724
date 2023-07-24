# Comparing `tmp/aio_pika-9.1.4.tar.gz` & `tmp/aio_pika-9.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_pika-9.1.4.tar", max compression
+gzip compressed data, was "aio_pika-9.1.5.tar", max compression
```

## Comparing `aio_pika-9.1.4.tar` & `aio_pika-9.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7568 2023-07-04 13:02:10.950030 aio_pika-9.1.4/README.rst
--rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.1.4/aio_pika/__init__.py
--rw-r--r--   0        0        0    24756 2023-06-01 15:55:44.119921 aio_pika-9.1.4/aio_pika/abc.py
--rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.1.4/aio_pika/channel.py
--rw-r--r--   0        0        0    10892 2023-06-01 15:55:44.123355 aio_pika-9.1.4/aio_pika/connection.py
--rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.1.4/aio_pika/exceptions.py
--rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.1.4/aio_pika/exchange.py
--rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.1.4/aio_pika/log.py
--rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.1.4/aio_pika/message.py
--rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.1.4/aio_pika/patterns/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.1.4/aio_pika/patterns/base.py
--rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.1.4/aio_pika/patterns/master.py
--rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.1.4/aio_pika/patterns/rpc.py
--rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.1.4/aio_pika/pool.py
--rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.1.4/aio_pika/py.typed
--rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.1.4/aio_pika/queue.py
--rw-r--r--   0        0        0     8219 2023-06-01 15:55:44.133275 aio_pika-9.1.4/aio_pika/robust_channel.py
--rw-r--r--   0        0        0    10445 2023-06-01 15:55:44.135097 aio_pika-9.1.4/aio_pika/robust_connection.py
--rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.1.4/aio_pika/robust_exchange.py
--rw-r--r--   0        0        0     4683 2023-07-04 14:24:49.233661 aio_pika-9.1.4/aio_pika/robust_queue.py
--rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.1.4/aio_pika/tools.py
--rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.1.4/aio_pika/transaction.py
--rw-r--r--   0        0        0     3269 2023-07-04 14:25:10.969778 aio_pika-9.1.4/pyproject.toml
--rw-r--r--   0        0        0     9471 1970-01-01 00:00:00.000000 aio_pika-9.1.4/PKG-INFO
+-rw-r--r--   0        0        0    15383 2023-07-24 18:31:14.983747 aio_pika-9.1.5/README.rst
+-rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.1.5/aio_pika/__init__.py
+-rw-r--r--   0        0        0    24756 2023-06-01 15:55:44.119921 aio_pika-9.1.5/aio_pika/abc.py
+-rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.1.5/aio_pika/channel.py
+-rw-r--r--   0        0        0    10892 2023-06-01 15:55:44.123355 aio_pika-9.1.5/aio_pika/connection.py
+-rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.1.5/aio_pika/exceptions.py
+-rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.1.5/aio_pika/exchange.py
+-rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.1.5/aio_pika/log.py
+-rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.1.5/aio_pika/message.py
+-rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.1.5/aio_pika/patterns/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.1.5/aio_pika/patterns/base.py
+-rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.1.5/aio_pika/patterns/master.py
+-rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.1.5/aio_pika/patterns/rpc.py
+-rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.1.5/aio_pika/pool.py
+-rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.1.5/aio_pika/py.typed
+-rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.1.5/aio_pika/queue.py
+-rw-r--r--   0        0        0     8275 2023-07-24 18:23:35.142833 aio_pika-9.1.5/aio_pika/robust_channel.py
+-rw-r--r--   0        0        0    10445 2023-06-01 15:55:44.135097 aio_pika-9.1.5/aio_pika/robust_connection.py
+-rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.1.5/aio_pika/robust_exchange.py
+-rw-r--r--   0        0        0     4683 2023-07-04 14:24:49.233661 aio_pika-9.1.5/aio_pika/robust_queue.py
+-rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.1.5/aio_pika/tools.py
+-rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.1.5/aio_pika/transaction.py
+-rw-r--r--   0        0        0     3269 2023-07-24 18:25:15.528884 aio_pika-9.1.5/pyproject.toml
+-rw-r--r--   0        0        0    16986 1970-01-01 00:00:00.000000 aio_pika-9.1.5/PKG-INFO
```

### Comparing `aio_pika-9.1.4/aio_pika/__init__.py` & `aio_pika-9.1.5/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/abc.py` & `aio_pika-9.1.5/aio_pika/abc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/channel.py` & `aio_pika-9.1.5/aio_pika/channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/connection.py` & `aio_pika-9.1.5/aio_pika/connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/exceptions.py` & `aio_pika-9.1.5/aio_pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/exchange.py` & `aio_pika-9.1.5/aio_pika/exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/message.py` & `aio_pika-9.1.5/aio_pika/message.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/patterns/base.py` & `aio_pika-9.1.5/aio_pika/patterns/base.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/patterns/master.py` & `aio_pika-9.1.5/aio_pika/patterns/master.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/patterns/rpc.py` & `aio_pika-9.1.5/aio_pika/patterns/rpc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/pool.py` & `aio_pika-9.1.5/aio_pika/pool.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/queue.py` & `aio_pika-9.1.5/aio_pika/queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/robust_channel.py` & `aio_pika-9.1.5/aio_pika/robust_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,50 +65,51 @@
         self._queues = defaultdict(WeakSet)
         self._prefetch_count: int = 0
         self._prefetch_size: int = 0
         self._global_qos: bool = False
         self.reopen_callbacks: CallbackCollection = CallbackCollection(self)
         self.__restore_lock = asyncio.Lock()
         self.__ready = asyncio.Event()
-        self.__restored = True
+        self.__restored = asyncio.Event()
+        self.__restored.set()
         self.close_callbacks.add(self.__close_callback)
 
     async def ready(self) -> None:
-        while not self.__restored:
-            await self.__ready.wait()
+        await self.__ready.wait()
+        await self.__restored.wait()
 
     async def get_underlay_channel(self) -> aiormq.abc.AbstractChannel:
         await self._connection.ready()
         return await super().get_underlay_channel()
 
     async def restore(self, channel: Any = None) -> None:
         if channel is not None:
             warnings.warn(
                 "Channel argument will be ignored because you "
                 "don't need to pass this anymore.",
                 DeprecationWarning,
             )
 
         async with self.__restore_lock:
-            if self.__restored:
+            if self.__restored.is_set():
                 return
 
             await self.reopen()
-            self.__restored = True
+            self.__restored.set()
 
     async def __close_callback(self, _: Any, exc: BaseException) -> None:
         if isinstance(exc, asyncio.CancelledError):
             # This happens only if the channel is forced to close from the
             # outside, for example, if the connection is closed.
             # Of course, here you need to exit from this function
             # as soon as possible and to avoid a recovery attempt.
             return
 
-        in_restore_state = not self.__restored
-        self.__restored = False
+        in_restore_state = not self.__restored.is_set()
+        self.__restored.clear()
         self.__ready.clear()
 
         if self._closed or in_restore_state:
             return
 
         await self.restore()
```

### Comparing `aio_pika-9.1.4/aio_pika/robust_connection.py` & `aio_pika-9.1.5/aio_pika/robust_connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/robust_exchange.py` & `aio_pika-9.1.5/aio_pika/robust_exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/robust_queue.py` & `aio_pika-9.1.5/aio_pika/robust_queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/tools.py` & `aio_pika-9.1.5/aio_pika/tools.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/aio_pika/transaction.py` & `aio_pika-9.1.5/aio_pika/transaction.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.4/pyproject.toml` & `aio_pika-9.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-pika"
-version = "9.1.4"
+version = "9.1.5"
 description = "Wrapper around the aiormq for asyncio and humans"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "aiormq"]
 homepage = "https://github.com/mosquito/aio-pika"
 classifiers = [
```

