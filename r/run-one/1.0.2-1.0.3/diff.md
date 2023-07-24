# Comparing `tmp/run_one-1.0.2.tar.gz` & `tmp/run_one-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.0.2.tar", max compression
+gzip compressed data, was "run_one-1.0.3.tar", max compression
```

## Comparing `run_one-1.0.2.tar` & `run_one-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-24 13:08:18.004482 run_one-1.0.2/LICENSE
--rw-r--r--   0        0        0     1708 2023-07-24 13:08:18.004482 run_one-1.0.2/README.md
--rw-r--r--   0        0        0      741 2023-07-24 13:08:18.004482 run_one-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      345 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/__init__.py
--rw-r--r--   0        0        0      282 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     1877 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1182 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     3260 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0        0 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     5319 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/util/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/util/config.py
--rw-r--r--   0        0        0     3225 2023-07-24 13:08:18.004482 run_one-1.0.2/run_one/util/util.py
--rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 run_one-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 20:02:11.671246 run_one-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1708 2023-07-24 20:02:11.671246 run_one-1.0.3/README.md
+-rw-r--r--   0        0        0      741 2023-07-24 20:02:11.671246 run_one-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      345 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     1877 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1182 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     3391 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     5319 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/util/config.py
+-rw-r--r--   0        0        0     3225 2023-07-24 20:02:11.671246 run_one-1.0.3/run_one/util/util.py
+-rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 run_one-1.0.3/PKG-INFO
```

### Comparing `run_one-1.0.2/LICENSE` & `run_one-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.0.2/README.md` & `run_one-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `run_one-1.0.2/pyproject.toml` & `run_one-1.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.0.2"
+version = "1.0.3"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
```

### Comparing `run_one-1.0.2/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.0.3/run_one/action_handlers/TH2ActHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.2/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.0.3/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.2/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.0.3/run_one/action_handlers/TH2Check1Handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,17 @@
 
         if parent_event_id := Context.get('parent_event_id'):
             check_rule_request.parent_event_id.CopyFrom(parent_event_id)
 
         if checkpoint_id := Context.get('checkpoint_id'):
             check_rule_request.checkpoint.CopyFrom(checkpoint_id)
 
-        chain_id = Context.get('chain_id_mapping')
-        chain_id = chain_id.get(user_and_direction) if chain_id is not None else None
+        chain_id_mapping = Context.get('chain_id_mapping')
+        chain_id = chain_id_mapping.get(user_and_direction) if chain_id_mapping is not None else None
         if chain_id is not None:
             check_rule_request.chain_id.CopyFrom(chain_id)
 
         response = self._check1_service.submitCheckRule(check_rule_request)
-        if chain_id is None:
+        if chain_id_mapping is None:
+            Context.set('chain_id_mapping', {user_and_direction: response.chain_id})
+        else:
             Context.get('chain_id_mapping')[user_and_direction] = response.chain_id
```

### Comparing `run_one-1.0.2/run_one/processors/abstract_processor.py` & `run_one-1.0.3/run_one/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.2/run_one/processors/th2_processor.py` & `run_one-1.0.3/run_one/processors/th2_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.2/run_one/util/config.py` & `run_one-1.0.3/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.2/run_one/util/util.py` & `run_one-1.0.3/run_one/util/util.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.2/PKG-INFO` & `run_one-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

