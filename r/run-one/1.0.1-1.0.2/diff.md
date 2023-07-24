# Comparing `tmp/run_one-1.0.1.tar.gz` & `tmp/run_one-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.0.1.tar", max compression
+gzip compressed data, was "run_one-1.0.2.tar", max compression
```

## Comparing `run_one-1.0.1.tar` & `run_one-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-21 01:30:47.021902 run_one-1.0.1/LICENSE
--rw-r--r--   0        0        0     1618 2023-07-21 01:30:47.021902 run_one-1.0.1/README.md
--rw-r--r--   0        0        0      741 2023-07-21 01:30:47.021902 run_one-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      345 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/__init__.py
--rw-r--r--   0        0        0      282 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     1877 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1182 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     3198 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0        0 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     4797 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/util/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/util/config.py
--rw-r--r--   0        0        0     3225 2023-07-21 01:30:47.021902 run_one-1.0.1/run_one/util/util.py
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 run_one-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 13:08:18.004482 run_one-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1708 2023-07-24 13:08:18.004482 run_one-1.0.2/README.md
+-rw-r--r--   0        0        0      741 2023-07-24 13:08:18.004482 run_one-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      345 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     1877 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1182 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     3260 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     5319 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/util/config.py
+-rw-r--r--   0        0        0     3225 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/util/util.py
+-rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 run_one-1.0.2/PKG-INFO
```

### Comparing `run_one-1.0.1/LICENSE` & `run_one-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.0.1/README.md` & `run_one-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 processor_config: # processor config in free form
   th2_configs: "th2_configs" # path to directory with th2 configs
   book: "test_book" # book name
   scope: "test_script" # scope name
   use_place_method: False # use th2 act place methods (True) or plain send (False)
   key_fields: ["Side", "ClOrdID", "OrigClOrdID"] # list of key fields for th2-check1 request
   sleep: 1 # delay between each action processing
+  timestamp_shift: 1 # for how many seconds to the past make a shift for event timestamps
 ```
```

### Comparing `run_one-1.0.1/pyproject.toml` & `run_one-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.0.1"
+version = "1.0.2"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
```

### Comparing `run_one-1.0.1/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.0.2/run_one/action_handlers/TH2ActHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.1/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.0.2/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.1/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.0.2/run_one/action_handlers/TH2Check1Handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
         if parent_event_id := Context.get('parent_event_id'):
             check_rule_request.parent_event_id.CopyFrom(parent_event_id)
 
         if checkpoint_id := Context.get('checkpoint_id'):
             check_rule_request.checkpoint.CopyFrom(checkpoint_id)
 
-        chain_id = Context.get('chain_id_mapping').get(user_and_direction)
+        chain_id = Context.get('chain_id_mapping')
+        chain_id = chain_id.get(user_and_direction) if chain_id is not None else None
         if chain_id is not None:
             check_rule_request.chain_id.CopyFrom(chain_id)
 
         response = self._check1_service.submitCheckRule(check_rule_request)
         if chain_id is None:
             Context.get('chain_id_mapping')[user_and_direction] = response.chain_id
```

### Comparing `run_one-1.0.1/run_one/processors/abstract_processor.py` & `run_one-1.0.2/run_one/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.1/run_one/processors/th2_processor.py` & `run_one-1.0.2/run_one/processors/th2_processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from datetime import datetime, timedelta
+from itertools import pairwise, chain
 import logging
 import time
-from itertools import pairwise, chain
 from typing import TypeVar
 
+from google.protobuf.timestamp_pb2 import Timestamp
+from th2_grpc_common.common_pb2 import EventBatch
 from th2_common.schema.event.event_batch_router import EventBatchRouter
 from th2_common.schema.factory.common_factory import CommonFactory
 from th2_common_utils import create_event, create_event_id
-from th2_grpc_common.common_pb2 import EventBatch
 
 from run_one.action_handlers.abstract_action_handler import AbstractActionHandler
 from run_one.action_handlers.context import Context
 from run_one.processors.abstract_processor import AbstractProcessor
 from run_one.util.config import Config
 from run_one.util.util import Action
 
@@ -38,23 +40,28 @@
         if 'key_fields' in kwargs:
             self.key_fields = kwargs['key_fields']
 
         self.sleep = 0
         if 'sleep' in kwargs:
             self.sleep = int(kwargs['sleep'])
 
+        self.timestamp_shift = 0
+        if 'timestamp_shift' in kwargs:
+            self.timestamp_shift = int(kwargs['timestamp_shift'])
+
 
 class Th2Processor(AbstractProcessor):
     def __init__(self, config: Config, processor_config_class=Th2ProcessorConfig):
         self._config = processor_config_class(**config.processor_config)
 
         self._common_factory = CommonFactory(config_path=self._config.th2_configs)
 
         self._event_router: EventBatchRouter = self._common_factory.event_batch_router  # type: ignore
-        self.root_event_id = create_event_id(book_name=self._config.book, scope=self._config.scope)
+        self.root_event_id = create_event_id(book_name=self._config.book, scope=self._config.scope,
+                                             start_timestamp=self.create_timestamp())
         self.root_event = EventBatch(events=[create_event(name='Run One Root Event',
                                                           event_id=self.root_event_id)])
         self._event_router.send(self.root_event)
         Context.set('root_event_id', self.root_event_id)
 
         self._grpc_router = self._common_factory.grpc_router
 
@@ -62,14 +69,19 @@
         action_handlers = self.load_action_handlers(config.processed_actions)
         class_instance_mapping = {x: x(self._config, self._grpc_router) for x in set(action_handlers.values())}
         self.processed_actions: dict[str, HandlerType] = {action: class_instance_mapping[action_handler]
                                                           for action, action_handler in action_handlers.items()}
 
         self.logger = logging.getLogger()
 
+    def create_timestamp(self) -> Timestamp:
+        timestamp = Timestamp()
+        timestamp.FromDatetime(datetime.utcnow() - timedelta(seconds=self._config.timestamp_shift))
+        return timestamp
+
     def process(self, test_cases: dict[str, list[Action]]):
 
         for test_case_name, actions in test_cases.items():
 
             logging.info(f'Processing {test_case_name} test case')
 
             test_case_root_event_id = create_event_id(book_name=self._config.book, scope=self._config.scope)
```

### Comparing `run_one-1.0.1/run_one/util/config.py` & `run_one-1.0.2/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.1/run_one/util/util.py` & `run_one-1.0.2/run_one/util/util.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.1/PKG-INFO` & `run_one-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -59,9 +59,10 @@
 processor_config: # processor config in free form
   th2_configs: "th2_configs" # path to directory with th2 configs
   book: "test_book" # book name
   scope: "test_script" # scope name
   use_place_method: False # use th2 act place methods (True) or plain send (False)
   key_fields: ["Side", "ClOrdID", "OrigClOrdID"] # list of key fields for th2-check1 request
   sleep: 1 # delay between each action processing
+  timestamp_shift: 1 # for how many seconds to the past make a shift for event timestamps
 ```
```

