# Comparing `tmp/ramqp-9.0.0.tar.gz` & `tmp/ramqp-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-9.0.0.tar", max compression
+gzip compressed data, was "ramqp-9.0.1.tar", max compression
```

## Comparing `ramqp-9.0.0.tar` & `ramqp-9.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-06-02 13:25:50.890882 ramqp-9.0.0/LICENSES/
--rw-r--r--   0        0        0    15177 2023-06-02 13:25:50.890882 ramqp-9.0.0/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-06-02 13:25:50.890882 ramqp-9.0.0/README.md
--rw-r--r--   0        0        0     1465 2023-06-02 13:26:03.776680 ramqp-9.0.0/pyproject.toml
--rw-r--r--   0        0        0      321 2023-06-02 13:25:50.892882 ramqp-9.0.0/ramqp/__init__.py
--rw-r--r--   0        0        0    16392 2023-06-02 13:25:50.892882 ramqp-9.0.0/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-06-02 13:25:50.892882 ramqp-9.0.0/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-06-02 13:25:50.892882 ramqp-9.0.0/ramqp/config.py
--rw-r--r--   0        0        0    10056 2023-06-02 13:25:50.893882 ramqp-9.0.0/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-06-02 13:25:50.893882 ramqp-9.0.0/ramqp/metrics.py
--rw-r--r--   0        0        0     8652 2023-06-02 13:25:50.893882 ramqp-9.0.0/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-06-02 13:25:50.944886 ramqp-9.0.0/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-06-02 13:25:50.893882 ramqp-9.0.0/ramqp/utils.py
--rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 ramqp-9.0.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-07-24 11:42:00.967762 ramqp-9.0.1/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-07-24 11:42:00.967762 ramqp-9.0.1/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-07-24 11:42:00.968762 ramqp-9.0.1/README.md
+-rw-r--r--   0        0        0     1465 2023-07-24 11:42:15.479999 ramqp-9.0.1/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-24 11:42:00.969762 ramqp-9.0.1/ramqp/__init__.py
+-rw-r--r--   0        0        0    16371 2023-07-24 11:42:00.969762 ramqp-9.0.1/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-07-24 11:42:00.969762 ramqp-9.0.1/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/config.py
+-rw-r--r--   0        0        0    10056 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/metrics.py
+-rw-r--r--   0        0        0     8652 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-07-24 11:42:01.103774 ramqp-9.0.1/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-07-24 11:42:00.970763 ramqp-9.0.1/ramqp/utils.py
+-rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 ramqp-9.0.1/PKG-INFO
```

### Comparing `ramqp-9.0.0/LICENSES/MPL-2.0.txt` & `ramqp-9.0.1/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.0/README.md` & `ramqp-9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.0/pyproject.toml` & `ramqp-9.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramqp"
-version = "9.0.0"
+version = "9.0.1"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
```

### Comparing `ramqp-9.0.0/ramqp/abstract.py` & `ramqp-9.0.1/ramqp/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,23 +226,24 @@
         # We expect function_to_name to be unique for each callback
         assert all_unique(map(function_to_name, self.router.registry.keys()))
 
         # We expect queue_prefix to be set if any callbacks are registered
         if self.router.registry:
             assert settings.queue_prefix is not None
 
+        url = settings.get_url()
         logger.info(
             "Establishing AMQP connection",
-            scheme=settings.url.scheme,
-            user=settings.url.user,
-            host=settings.url.host,
-            port=settings.url.port,
-            path=settings.url.path,
+            scheme=url.scheme,
+            user=url.user,
+            host=url.host,
+            port=url.port,
+            path=url.path,
         )
-        self._connection = await connect_robust(settings.url)
+        self._connection = await connect_robust(url)
         _setup_connection_metrics(self._connection)
 
         logger.info("Creating AMQP channel")
         self._channel = cast(AbstractRobustChannel, await self._connection.channel())
         await self._channel.set_qos(prefetch_count=settings.prefetch_count)
         _setup_channel_metrics(self._channel)
```

### Comparing `ramqp-9.0.0/ramqp/amqp.py` & `ramqp-9.0.1/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.0/ramqp/config.py` & `ramqp-9.0.1/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.0/ramqp/depends.py` & `ramqp-9.0.1/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.0/ramqp/metrics.py` & `ramqp-9.0.1/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.0/ramqp/mo.py` & `ramqp-9.0.1/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.0/ramqp/utils.py` & `ramqp-9.0.1/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-9.0.0/PKG-INFO` & `ramqp-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 9.0.0
+Version: 9.0.1
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

