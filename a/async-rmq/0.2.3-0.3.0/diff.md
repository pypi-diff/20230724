# Comparing `tmp/async_rmq-0.2.3.tar.gz` & `tmp/async_rmq-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_rmq-0.2.3.tar", last modified: Wed May 10 11:00:57 2023, max compression
+gzip compressed data, was "async_rmq-0.3.0.tar", last modified: Mon Jul 24 11:55:05 2023, max compression
```

## Comparing `async_rmq-0.2.3.tar` & `async_rmq-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:00:57.721200 async_rmq-0.2.3/
--rw-rw-rw-   0        0        0      162 2023-05-10 11:00:57.722195 async_rmq-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2023-02-22 10:40:51.000000 async_rmq-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 11:00:57.707382 async_rmq-0.2.3/async_rmq/
--rw-rw-rw-   0        0        0        0 2023-01-30 13:24:34.000000 async_rmq-0.2.3/async_rmq/_init_.py
--rw-rw-rw-   0        0        0     2439 2023-03-15 10:40:00.000000 async_rmq-0.2.3/async_rmq/abstract_rmq_consumer.py
--rw-rw-rw-   0        0        0     1390 2023-05-10 10:58:25.000000 async_rmq-0.2.3/async_rmq/consumer_threading.py
--rw-rw-rw-   0        0        0     7642 2023-05-10 10:59:43.000000 async_rmq-0.2.3/async_rmq/rmq_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:00:57.721200 async_rmq-0.2.3/async_rmq.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-10 11:00:57.000000 async_rmq-0.2.3/async_rmq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-10 11:00:57.000000 async_rmq-0.2.3/async_rmq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:00:57.000000 async_rmq-0.2.3/async_rmq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-20 13:54:08.000000 async_rmq-0.2.3/async_rmq.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-05-10 11:00:57.000000 async_rmq-0.2.3/async_rmq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 11:00:57.723183 async_rmq-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      259 2023-05-10 11:00:11.000000 async_rmq-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:55:05.676097 async_rmq-0.3.0/
+-rw-rw-rw-   0        0        0      162 2023-07-24 11:55:05.676097 async_rmq-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2023-02-22 10:40:51.000000 async_rmq-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 11:55:05.653004 async_rmq-0.3.0/async_rmq/
+-rw-rw-rw-   0        0        0        0 2023-01-30 13:24:34.000000 async_rmq-0.3.0/async_rmq/_init_.py
+-rw-rw-rw-   0        0        0     2439 2023-03-15 10:40:00.000000 async_rmq-0.3.0/async_rmq/abstract_rmq_consumer.py
+-rw-rw-rw-   0        0        0     2199 2023-07-24 11:42:31.000000 async_rmq-0.3.0/async_rmq/abstract_rmq_rpc_server.py
+-rw-rw-rw-   0        0        0     2638 2023-07-24 11:42:31.000000 async_rmq-0.3.0/async_rmq/abtract_rmq_rpc_client.py
+-rw-rw-rw-   0        0        0     1956 2023-07-21 13:23:06.000000 async_rmq-0.3.0/async_rmq/consumer_threading.py
+-rw-rw-rw-   0        0        0    10205 2023-07-24 11:43:06.000000 async_rmq-0.3.0/async_rmq/rmq_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:55:05.675130 async_rmq-0.3.0/async_rmq.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-07-24 11:55:05.000000 async_rmq-0.3.0/async_rmq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-24 11:55:05.000000 async_rmq-0.3.0/async_rmq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:55:05.000000 async_rmq-0.3.0/async_rmq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-20 13:54:08.000000 async_rmq-0.3.0/async_rmq.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-07-24 11:55:05.000000 async_rmq-0.3.0/async_rmq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 11:55:05.677096 async_rmq-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      259 2023-07-24 11:54:00.000000 async_rmq-0.3.0/setup.py
```

### Comparing `async_rmq-0.2.3/README.md` & `async_rmq-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `async_rmq-0.2.3/async_rmq/abstract_rmq_consumer.py` & `async_rmq-0.3.0/async_rmq/abstract_rmq_consumer.py`

 * *Files identical despite different names*

### Comparing `async_rmq-0.2.3/async_rmq/consumer_threading.py` & `async_rmq-0.3.0/async_rmq/consumer_threading.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from .rmq_functions import run_consumer
+from .rmq_functions import run_consumer, run_rpc_server
 
 
 class WorkerThreader:
 
     def __init__(self, consumers_conf, credentials):
         self.consumers_conf = consumers_conf
         self.credentials = credentials
@@ -14,18 +14,27 @@
         self.consumer_classes = [workers_data["consumer_class"] for workers_data in self.consumers_conf]
         for workers_data in self.consumers_conf:
             workers_count = workers_data["workers_count"]
             consumer_class = workers_data["consumer_class"]
             consumer_settings = workers_data["consumer_settings"]
             dead_letter_params = workers_data["dead_letter_params"]
 
-            consumer_functions = [run_consumer(consumer_class,
-                                               **self.credentials,
-                                               **consumer_settings,
-                                               **dead_letter_params) for i in range(1, workers_count + 1)]
+            if workers_data["is_rpc"]:
+                consumer_functions = [run_rpc_server(consumer_class,
+                                                     workers_data["resp_exchange"],
+                                                     **self.credentials,
+                                                     **consumer_settings,
+                                                     **dead_letter_params
+                                                     ) for i in range(1, workers_count + 1)]
+
+            else:
+                consumer_functions = [run_consumer(consumer_class,
+                                                   **self.credentials,
+                                                   **consumer_settings,
+                                                   **dead_letter_params) for i in range(1, workers_count + 1)]
             self.workers.extend(consumer_functions)
 
     def stop_consumers(self):
         import gc
         consumer_objs = [ob for ob in gc.get_objects() if isinstance(ob, tuple(self.consumer_classes))]
 
         for obj in consumer_objs:
```

### Comparing `async_rmq-0.2.3/async_rmq/rmq_functions.py` & `async_rmq-0.3.0/async_rmq/rmq_functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import aio_pika
 import logging
 import copy
 from typing import Optional
 from aiormq.exceptions import ChannelNotFoundEntity
 from aio_pika import Channel, Queue, Exchange, ExchangeType
 from .abstract_rmq_consumer import RabbitMQConsumer
+from .abstract_rmq_rpc_server import RPCRabbitMQServer
 
 logger = logging.getLogger("async_rmq")
 
 DEFAULT_QUEUE_PARAMETERS = {
     "durable": True,
     "arguments": {
         "x-queue-type": "quorum"
@@ -84,23 +85,15 @@
                        dl_queue_name: Optional[str] = None,
                        dl_queue_params: Optional[dict] = {},
                        dl_exchange_name: Optional[str] = None,
                        dl_exchange_type: Optional[str] = None,
                        dl_exchange_params: Optional[dict] = {},
                        dl_bindings: Optional[list] = []) -> None:
     loop = asyncio.get_event_loop()
-
-    rabbitmq_connection = await aio_pika.connect_robust(
-        loop=loop,
-        host=host,
-        port=port,
-        login=login,
-        password=password,
-        virtualhost=vhost
-    )
+    rabbitmq_connection = await get_rmq_connection(host, port, login, password, vhost, loop)
 
     async with rabbitmq_connection.channel() as channel:
         await channel.set_qos(prefetch_count=1)
 
         if dl_enabled:
             dead_letter_queue, dead_letter_exchange = await _prepare_dead_letter_queue(channel,
                                                                                        dl_queue_name,
@@ -122,29 +115,78 @@
             queue=queue
         )
         await consumer.consume()
 
     logger.info("Shutdown complete")
     await rabbitmq_connection.close()
 
+# Running a consumer
+async def run_rpc_server(rpc_server_class: RPCRabbitMQServer,
+                         resp_exchange_name: str,
+                         host: str,
+                         port: int,
+                         login: str,
+                         password: str,
+                         vhost: str,
+                         queue_name: str,
+                         exchange_name: str,
+                         exchange_type: str,
+                         binding: str,
+                         queue_params: dict = DEFAULT_QUEUE_PARAMETERS,
+                         exchange_params: dict = DEFAULT_EXCHANGE_PARAMETERS,
+                         dl_enabled: Optional[bool] = False,
+                         dl_queue_name: Optional[str] = None,
+                         dl_queue_params: Optional[dict] = {},
+                         dl_exchange_name: Optional[str] = None,
+                         dl_exchange_type: Optional[str] = None,
+                         dl_exchange_params: Optional[dict] = {},
+                         dl_bindings: Optional[list] = []) -> None:
+    loop = asyncio.get_event_loop()
+    rabbitmq_connection = await get_rmq_connection(host, port, login, password, vhost, loop)
+
+    async with rabbitmq_connection.channel() as channel:
+        await channel.set_qos(prefetch_count=1)
+
+        if dl_enabled:
+            dead_letter_queue, dead_letter_exchange = await _prepare_dead_letter_queue(channel,
+                                                                                       dl_queue_name,
+                                                                                       dl_exchange_name,
+                                                                                       get_exchange_type(dl_exchange_type),
+                                                                                       dl_queue_params,
+                                                                                       dl_exchange_params,
+                                                                                       dl_bindings)
+        queue = await _prepare_consumed_queue(channel,
+                                              queue_name,
+                                              exchange_name,
+                                              get_exchange_type(exchange_type),
+                                              binding,
+                                              queue_params,
+                                              exchange_params,
+                                              dl_enabled,
+                                              dl_exchange_name)
+        resp_exchange = await channel.declare_exchange(resp_exchange_name, ExchangeType.TOPIC, **exchange_params)
+        rpc_server = rpc_server_class(
+            queue=queue,
+            resp_exchange=resp_exchange
+        )
+        await rpc_server.run_rpc_server()
+
+    logger.info("Shutdown complete")
+    await rabbitmq_connection.close()
+
 async def send_message(msg_data: dict,
                        exchange_name: str,
                        routing_key: str,
                        host: str,
                        port: int,
                        login: str,
                        password: str,
                        vhost: str):
-    connection = await aio_pika.connect_robust(
-        host=host,
-        port=port,
-        login=login,
-        password=password,
-        virtualhost=vhost
-    )
+    connection = await get_rmq_connection(host, port, login, password, vhost)
+
     async with connection:
         channel = await connection.channel()
 
         try:
             exchange = await channel.get_exchange(exchange_name)
             msg = aio_pika.Message(body=msg_data)
             await exchange.publish(
@@ -152,32 +194,24 @@
                 routing_key=routing_key
             )
 
         except ChannelNotFoundEntity:
             logger.warning("The message could not be sent because the exchange with the name '%s' was not found"
                            % exchange_name)
 
-async def init_queue(consumer_settings: dict,
-                     host: str,
-                     port: int,
-                     login: str,
-                     password: str,
-                     vhost: str,
-                     queue_params: dict = DEFAULT_QUEUE_PARAMETERS,
-                     exchange_params: dict = DEFAULT_EXCHANGE_PARAMETERS):
+async def get_rmq_connection(host: str, port: int, login: str, password: str, vhost: str, loop: Optional = None):
     connection = await aio_pika.connect_robust(
         host=host,
         port=port,
         login=login,
         password=password,
-        virtualhost=vhost
+        virtualhost=vhost,
+        loop=loop
     )
-
-    async with connection.channel() as channel:
-        queue = await _prepare_consumed_queue(channel, **consumer_settings)
+    return connection
 
 
 def get_exchange_type(s):
     if s == ExchangeType.DIRECT.value:
         return ExchangeType.DIRECT
     elif s == ExchangeType.TOPIC.value:
         return ExchangeType.TOPIC
```

