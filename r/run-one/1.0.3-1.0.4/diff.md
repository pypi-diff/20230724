# Comparing `tmp/run_one-1.0.3.tar.gz` & `tmp/run_one-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.0.3.tar", max compression
+gzip compressed data, was "run_one-1.0.4.tar", max compression
```

## Comparing `run_one-1.0.3.tar` & `run_one-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-24 20:02:11.671246 run_one-1.0.3/LICENSE
--rw-r--r--   0        0        0     1708 2023-07-24 20:02:11.671246 run_one-1.0.3/README.md
--rw-r--r--   0        0        0      741 2023-07-24 20:02:11.671246 run_one-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      345 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/__init__.py
--rw-r--r--   0        0        0      282 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     1877 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1182 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     3391 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0        0 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     5319 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/util/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/util/config.py
--rw-r--r--   0        0        0     3225 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/util/util.py
--rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 run_one-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 20:28:34.972903 run_one-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1708 2023-07-24 20:28:34.972903 run_one-1.0.4/README.md
+-rw-r--r--   0        0        0      741 2023-07-24 20:28:34.972903 run_one-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      345 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     1916 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1182 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     3391 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     5414 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:28:34.972903 run_one-1.0.4/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-24 20:28:34.976904 run_one-1.0.4/run_one/util/config.py
+-rw-r--r--   0        0        0     3225 2023-07-24 20:28:34.976904 run_one-1.0.4/run_one/util/util.py
+-rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 run_one-1.0.4/PKG-INFO
```

### Comparing `run_one-1.0.3/LICENSE` & `run_one-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.0.3/README.md` & `run_one-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `run_one-1.0.3/pyproject.toml` & `run_one-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.0.3"
+version = "1.0.4"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
```

### Comparing `run_one-1.0.3/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.0.4/run_one/action_handlers/TH2ActHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 
         if parent_event_id := Context.get('parent_event_id'):
             message.parent_event_id.CopyFrom(parent_event_id)
 
         if not self._config.use_place_method:
             response = self._act_service.sendMessage(message)
         else:
-            response = self._get_act_method(message_type)(message)
+            response = self._get_act_method(message_type)(message, timeout=action.extra_data.get('Time'))
 
         Context.set('checkpoint_id', response.checkpoint_id)
```

### Comparing `run_one-1.0.3/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.0.4/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.3/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.0.4/run_one/action_handlers/TH2Check1Handler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.3/run_one/processors/abstract_processor.py` & `run_one-1.0.4/run_one/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.3/run_one/processors/th2_processor.py` & `run_one-1.0.4/run_one/processors/th2_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 
     def process(self, test_cases: dict[str, list[Action]]):
 
         for test_case_name, actions in test_cases.items():
 
             logging.info(f'Processing {test_case_name} test case')
 
-            test_case_root_event_id = create_event_id(book_name=self._config.book, scope=self._config.scope)
+            test_case_root_event_id = create_event_id(book_name=self._config.book, scope=self._config.scope,
+                                                      start_timestamp=self.create_timestamp())
             test_case_event_batch = EventBatch(events=[create_event(name=test_case_name,
                                                                     event_id=test_case_root_event_id,
                                                                     parent_id=self.root_event_id)])
             self._event_router.send(test_case_event_batch)
             Context.set('parent_event_id', test_case_root_event_id)
 
             for previous_action, current_action in pairwise(chain([None], actions)):
```

### Comparing `run_one-1.0.3/run_one/util/config.py` & `run_one-1.0.4/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.3/run_one/util/util.py` & `run_one-1.0.4/run_one/util/util.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.3/PKG-INFO` & `run_one-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

