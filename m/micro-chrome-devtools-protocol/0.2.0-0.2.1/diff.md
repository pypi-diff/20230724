# Comparing `tmp/micro-chrome-devtools-protocol-0.2.0.tar.gz` & `tmp/micro-chrome-devtools-protocol-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micro-chrome-devtools-protocol-0.2.0.tar", last modified: Sun Jul 23 18:47:56 2023, max compression
+gzip compressed data, was "micro-chrome-devtools-protocol-0.2.1.tar", last modified: Mon Jul 24 08:53:28 2023, max compression
```

## Comparing `micro-chrome-devtools-protocol-0.2.0.tar` & `micro-chrome-devtools-protocol-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 aib       (1000) aib       (1000)        0 2023-07-23 18:47:56.979317 micro-chrome-devtools-protocol-0.2.0/
--rw-rw-r--   0 aib       (1000) aib       (1000)     1074 2023-07-22 18:06:46.000000 micro-chrome-devtools-protocol-0.2.0/LICENSE
--rw-rw-r--   0 aib       (1000) aib       (1000)     1050 2023-07-23 18:47:56.979317 micro-chrome-devtools-protocol-0.2.0/PKG-INFO
--rw-rw-r--   0 aib       (1000) aib       (1000)      297 2023-07-22 18:18:13.000000 micro-chrome-devtools-protocol-0.2.0/README.md
-drwxrwxr-x   0 aib       (1000) aib       (1000)        0 2023-07-23 18:47:56.979317 micro-chrome-devtools-protocol-0.2.0/micro_chrome_devtools_protocol.egg-info/
--rw-rw-r--   0 aib       (1000) aib       (1000)     1050 2023-07-23 18:47:56.000000 micro-chrome-devtools-protocol-0.2.0/micro_chrome_devtools_protocol.egg-info/PKG-INFO
--rw-rw-r--   0 aib       (1000) aib       (1000)      315 2023-07-23 18:47:56.000000 micro-chrome-devtools-protocol-0.2.0/micro_chrome_devtools_protocol.egg-info/SOURCES.txt
--rw-rw-r--   0 aib       (1000) aib       (1000)        1 2023-07-23 18:47:56.000000 micro-chrome-devtools-protocol-0.2.0/micro_chrome_devtools_protocol.egg-info/dependency_links.txt
--rw-rw-r--   0 aib       (1000) aib       (1000)        5 2023-07-23 18:47:56.000000 micro-chrome-devtools-protocol-0.2.0/micro_chrome_devtools_protocol.egg-info/top_level.txt
--rw-rw-r--   0 aib       (1000) aib       (1000)        0 2023-07-22 18:06:33.000000 micro-chrome-devtools-protocol-0.2.0/pyproject.toml
--rw-rw-r--   0 aib       (1000) aib       (1000)      807 2023-07-23 18:47:56.979317 micro-chrome-devtools-protocol-0.2.0/setup.cfg
-drwxrwxr-x   0 aib       (1000) aib       (1000)        0 2023-07-23 18:47:56.979317 micro-chrome-devtools-protocol-0.2.0/ucdp/
--rw-rw-r--   0 aib       (1000) aib       (1000)       62 2023-07-23 18:41:46.000000 micro-chrome-devtools-protocol-0.2.0/ucdp/__init__.py
--rw-rw-r--   0 aib       (1000) aib       (1000)      234 2023-07-22 17:53:51.000000 micro-chrome-devtools-protocol-0.2.0/ucdp/data.py
--rw-rw-r--   0 aib       (1000) aib       (1000)       98 2023-07-22 17:53:51.000000 micro-chrome-devtools-protocol-0.2.0/ucdp/event.py
--rw-rw-r--   0 aib       (1000) aib       (1000)     3668 2023-07-23 18:21:41.000000 micro-chrome-devtools-protocol-0.2.0/ucdp/ucdp.py
+drwxrwxr-x   0 aib       (1000) aib       (1000)        0 2023-07-24 08:53:28.402273 micro-chrome-devtools-protocol-0.2.1/
+-rw-rw-r--   0 aib       (1000) aib       (1000)     1074 2023-07-22 18:06:46.000000 micro-chrome-devtools-protocol-0.2.1/LICENSE
+-rw-rw-r--   0 aib       (1000) aib       (1000)     1050 2023-07-24 08:53:28.402273 micro-chrome-devtools-protocol-0.2.1/PKG-INFO
+-rw-rw-r--   0 aib       (1000) aib       (1000)      297 2023-07-22 18:18:13.000000 micro-chrome-devtools-protocol-0.2.1/README.md
+drwxrwxr-x   0 aib       (1000) aib       (1000)        0 2023-07-24 08:53:28.402273 micro-chrome-devtools-protocol-0.2.1/micro_chrome_devtools_protocol.egg-info/
+-rw-rw-r--   0 aib       (1000) aib       (1000)     1050 2023-07-24 08:53:28.000000 micro-chrome-devtools-protocol-0.2.1/micro_chrome_devtools_protocol.egg-info/PKG-INFO
+-rw-rw-r--   0 aib       (1000) aib       (1000)      315 2023-07-24 08:53:28.000000 micro-chrome-devtools-protocol-0.2.1/micro_chrome_devtools_protocol.egg-info/SOURCES.txt
+-rw-rw-r--   0 aib       (1000) aib       (1000)        1 2023-07-24 08:53:28.000000 micro-chrome-devtools-protocol-0.2.1/micro_chrome_devtools_protocol.egg-info/dependency_links.txt
+-rw-rw-r--   0 aib       (1000) aib       (1000)        5 2023-07-24 08:53:28.000000 micro-chrome-devtools-protocol-0.2.1/micro_chrome_devtools_protocol.egg-info/top_level.txt
+-rw-rw-r--   0 aib       (1000) aib       (1000)        0 2023-07-22 18:06:33.000000 micro-chrome-devtools-protocol-0.2.1/pyproject.toml
+-rw-rw-r--   0 aib       (1000) aib       (1000)      807 2023-07-24 08:53:28.406273 micro-chrome-devtools-protocol-0.2.1/setup.cfg
+drwxrwxr-x   0 aib       (1000) aib       (1000)        0 2023-07-24 08:53:28.402273 micro-chrome-devtools-protocol-0.2.1/ucdp/
+-rw-rw-r--   0 aib       (1000) aib       (1000)       62 2023-07-24 08:41:58.000000 micro-chrome-devtools-protocol-0.2.1/ucdp/__init__.py
+-rw-rw-r--   0 aib       (1000) aib       (1000)      234 2023-07-22 17:53:51.000000 micro-chrome-devtools-protocol-0.2.1/ucdp/data.py
+-rw-rw-r--   0 aib       (1000) aib       (1000)       98 2023-07-22 17:53:51.000000 micro-chrome-devtools-protocol-0.2.1/ucdp/event.py
+-rw-rw-r--   0 aib       (1000) aib       (1000)     3579 2023-07-24 08:41:35.000000 micro-chrome-devtools-protocol-0.2.1/ucdp/ucdp.py
```

### Comparing `micro-chrome-devtools-protocol-0.2.0/LICENSE` & `micro-chrome-devtools-protocol-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micro-chrome-devtools-protocol-0.2.0/PKG-INFO` & `micro-chrome-devtools-protocol-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micro-chrome-devtools-protocol
-Version: 0.2.0
+Version: 0.2.1
 Summary: A lightweight library for speaking the Chrome DevTools Protocol in order to debug JavaScript
 Home-page: https://github.com/aib/ucdp
 Author: Orhan "aib" Kavrakoglu
 Author-email: aibok42@gmail.com
 License: MIT
 Keywords: chrome,chromium,devtools,protocol,node,nodejs,electron,debugging,debugger
 Classifier: Intended Audience :: Developers
```

### Comparing `micro-chrome-devtools-protocol-0.2.0/micro_chrome_devtools_protocol.egg-info/PKG-INFO` & `micro-chrome-devtools-protocol-0.2.1/micro_chrome_devtools_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micro-chrome-devtools-protocol
-Version: 0.2.0
+Version: 0.2.1
 Summary: A lightweight library for speaking the Chrome DevTools Protocol in order to debug JavaScript
 Home-page: https://github.com/aib/ucdp
 Author: Orhan "aib" Kavrakoglu
 Author-email: aibok42@gmail.com
 License: MIT
 Keywords: chrome,chromium,devtools,protocol,node,nodejs,electron,debugging,debugger
 Classifier: Intended Audience :: Developers
```

### Comparing `micro-chrome-devtools-protocol-0.2.0/setup.cfg` & `micro-chrome-devtools-protocol-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `micro-chrome-devtools-protocol-0.2.0/ucdp/ucdp.py` & `micro-chrome-devtools-protocol-0.2.1/ucdp/ucdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,17 +97,15 @@
 		self._method_logger.debug("<- Method %s: %s %s", msg['id'], msg['method'], msg['params'])
 		self._sender(json.dumps(msg))
 
 	def _process_result(self, result_id: int, result: dict):
 		self._method_logger.debug("-> Result %s: %s", result_id, result)
 
 		pending = self._pending_results.get(result_id, None)
-		if pending is None:
-			self._logger.warning("Received result %s with no waiters: %s", result_id, result)
-		else:
+		if pending is not None:
 			pending.put(result)
 
 	def _process_event(self, event: UcdpEvent):
 		self._event_logger.debug("-> Event %s: %s", event.name, event.params)
 		self.data._process_event(event)
 		if self.use_event_thread:
 			self._event_queue.put(event)
```

