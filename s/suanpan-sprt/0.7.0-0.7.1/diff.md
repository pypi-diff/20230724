# Comparing `tmp/suanpan-sprt-0.7.0.tar.gz` & `tmp/suanpan-sprt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.7.0.tar", last modified: Sun Jul 23 09:30:28 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.7.1.tar", last modified: Mon Jul 24 12:02:46 2023, max compression
```

## Comparing `suanpan-sprt-0.7.0.tar` & `suanpan-sprt-0.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4337 2023-07-18 09:03:49.000000 suanpan-sprt-0.7.0/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4546 2023-07-23 09:30:27.000000 suanpan-sprt-0.7.0/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4375 2023-07-23 09:30:27.000000 suanpan-sprt-0.7.0/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-07-23 08:10:40.000000 suanpan-sprt-0.7.0/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6982 2023-07-23 09:30:27.000000 suanpan-sprt-0.7.0/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.0/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-23 09:30:27.000000 suanpan-sprt-0.7.0/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-23 09:30:28.000000 suanpan-sprt-0.7.0/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4337 2023-07-18 09:03:49.000000 suanpan-sprt-0.7.1/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4546 2023-07-23 09:30:27.000000 suanpan-sprt-0.7.1/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4174 2023-07-24 12:02:45.000000 suanpan-sprt-0.7.1/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-07-23 08:10:40.000000 suanpan-sprt-0.7.1/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     7030 2023-07-24 12:02:45.000000 suanpan-sprt-0.7.1/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.7.1/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-24 12:02:45.000000 suanpan-sprt-0.7.1/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-24 12:02:46.000000 suanpan-sprt-0.7.1/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.7.0/setup.py` & `suanpan-sprt-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.7.0/sprt/__main__.py` & `suanpan-sprt-0.7.1/sprt/__main__.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.7.0/sprt/arguments.py` & `suanpan-sprt-0.7.1/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.7.0/sprt/envs.py` & `suanpan-sprt-0.7.1/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.7.0/sprt/loader.py` & `suanpan-sprt-0.7.1/sprt/loader.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.7.0/sprt/log.py` & `suanpan-sprt-0.7.1/sprt/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,26 +40,25 @@
         logger = cls.get_logger(app_id)
         if not logger:
             return
 
         if logkit is None:
             logkit_handler = cls._app_logkit_handler.pop(app_id)
             if logkit_handler:
+                current_app.logger.info('remove logkit handler: %s', logkit_handler.uri)
                 logger.removeHandler(logkit_handler)
                 logkit_handler.close()
         else:
             logkit_handler = cls._app_logkit_handler.get(app_id)
             if logkit_handler is None:
-                logging.info('setup logkit handler: %s', logkit.uri)
+                current_app.logger.info('setup app %s logkit handler: %s', app_id, logkit.uri)
                 lh = LogkitHandler(logkit.uri, logkit.namespace, logkit.path, logkit.events_append)
                 lh.setLevel(logkit.logs_level.upper())
                 logger.addHandler(lh)
                 cls._app_logkit_handler[app_id] = lh
-            else:
-                logkit_handler.update_uri(logkit.uri)
 
     @classmethod
     def clear_logger(cls, app_id):
         logkit_handler = cls._app_logkit_handler.pop(app_id)
         if logkit_handler:
             current_app.logger.info('close logkit handler: %s', logkit_handler.uri)
             logkit_handler.close()
@@ -88,33 +87,24 @@
         self.client = None
         self.uri = uri
         self.url = urljoin(uri, namespace)
         self.namespace = namespace
         self.socketio_path = socketio_path
         self.event = event
 
-    def update_uri(self, uri):
-        if uri == self.uri:
-            return
-
-        self.close()
-        self.uri = uri
-        self.url = urljoin(uri, self.namespace)
-        self.client = self.make_client()
-
     def make_client(self):
         return master.sio(self.url, namespaces=self.namespace, socketio_path=self.socketio_path, wait_timeout=3)
 
     def send(self, msg):
         if not self.client:
             self.client = self.make_client()
-        elif not self.client.connected:
-            self.client.disconnect()
-            self.client = self.make_client()
-        self.client.emit(self.event, data=msg, namespace=self.namespace)
+
+        if self.client.connected:
+            # socketio will reconnect automatically
+            self.client.emit(self.event, data=msg, namespace=self.namespace)
 
     @staticmethod
     def make_pickle(record):
         app = envs.appId
         extra = {"node": envs.nodeId}
         data = (app,
                 {
```

### Comparing `suanpan-sprt-0.7.0/sprt/master.py` & `suanpan-sprt-0.7.1/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.7.0/sprt/server.py` & `suanpan-sprt-0.7.1/sprt/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,19 +178,19 @@
     user_id = data.context.user_id
     app_id = data.context.app_id
     node_id = data.context.node_id
     working_dir = data.working_dir if data.working_dir else default_dir
     filename = data.file
     function = data.function
 
-    node_function = module_imported.get(node_id)
+    node_function = module_imported.get(f'{user_id}_{app_id}_{node_id}')
     if not node_function:
         logging.info(f'node {node_id} import function {function} from {filename}')
         node_function = loader.NodeFunction(user_id, app_id, node_id, working_dir, filename, function)
-        module_imported[node_id] = node_function
+        module_imported[f'{user_id}_{app_id}_{node_id}'] = node_function
 
     node_function.update_logkit(data.logkit)
     return node_function
 
 
 async def handle_event(event_data, working_dir='.'):
     model_class = validation._to_pydantic_model(FunctionParams)
```

### Comparing `suanpan-sprt-0.7.0/sprt/storage.py` & `suanpan-sprt-0.7.1/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.7.0/sprt/testing.py` & `suanpan-sprt-0.7.1/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.7.0/sprt/utils.py` & `suanpan-sprt-0.7.1/sprt/utils.py`

 * *Files identical despite different names*

