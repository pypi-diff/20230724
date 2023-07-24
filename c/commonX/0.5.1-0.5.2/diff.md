# Comparing `tmp/commonX-0.5.1.tar.gz` & `tmp/commonX-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.5.1.tar", last modified: Thu Jul 13 07:39:58 2023, max compression
+gzip compressed data, was "commonX-0.5.2.tar", last modified: Mon Jul 24 03:00:27 2023, max compression
```

## Comparing `commonX-0.5.1.tar` & `commonX-0.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 07:39:58.000000 commonX-0.5.1/
--rw-rw-rw-   0        0        0      760 2023-07-13 07:39:58.000000 commonX-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-07-13 07:39:47.000000 commonX-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 07:39:58.000000 commonX-0.5.1/common/
--rw-rw-rw-   0        0        0      107 2023-07-13 07:39:47.000000 commonX-0.5.1/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:39:58.000000 commonX-0.5.1/common/base/
--rw-rw-rw-   0        0        0      653 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/mapper.py
--rw-rw-rw-   0        0        0     9340 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5194 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-07-13 07:39:47.000000 commonX-0.5.1/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:39:58.000000 commonX-0.5.1/common/ext/
--rw-rw-rw-   0        0        0      187 2023-07-13 07:39:47.000000 commonX-0.5.1/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-07-13 07:39:47.000000 commonX-0.5.1/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-07-13 07:39:47.000000 commonX-0.5.1/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-07-13 07:39:47.000000 commonX-0.5.1/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-07-13 07:39:47.000000 commonX-0.5.1/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:39:58.000000 commonX-0.5.1/common/postman/
--rw-rw-rw-   0        0        0       87 2023-07-13 07:39:47.000000 commonX-0.5.1/common/postman/__init__.py
--rw-rw-rw-   0        0        0     5045 2023-07-13 07:39:47.000000 commonX-0.5.1/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     5201 2023-07-13 07:39:47.000000 commonX-0.5.1/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     4782 2023-07-13 07:39:47.000000 commonX-0.5.1/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:39:58.000000 commonX-0.5.1/common/util/
--rw-rw-rw-   0        0        0      304 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/assert_util.py
--rw-rw-rw-   0        0        0     2513 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     2725 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/exception_utll.py
--rw-rw-rw-   0        0        0     7244 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/file_util.py
--rw-rw-rw-   0        0        0     2935 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/image_util.py
--rw-rw-rw-   0        0        0     2921 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/json_util.py
--rw-rw-rw-   0        0        0     7041 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4611 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-07-13 07:39:47.000000 commonX-0.5.1/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:39:58.000000 commonX-0.5.1/commonX.egg-info/
--rw-rw-rw-   0        0        0      760 2023-07-13 07:39:58.000000 commonX-0.5.1/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-07-13 07:39:58.000000 commonX-0.5.1/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 07:39:58.000000 commonX-0.5.1/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-13 07:39:58.000000 commonX-0.5.1/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 07:39:58.000000 commonX-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1410 2023-07-13 07:39:47.000000 commonX-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.986121 commonX-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 03:00:27.986121 commonX-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 03:00:18.000000 commonX-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.982121 commonX-0.5.2/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-24 03:00:18.000000 commonX-0.5.2/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.982121 commonX-0.5.2/common/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/genor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/multi_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.982121 commonX-0.5.2/common/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/cookie_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/iphone_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/ocr_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/qq_email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.982121 commonX-0.5.2/common/postman/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 03:00:18.000000 commonX-0.5.2/common/postman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-24 03:00:18.000000 commonX-0.5.2/common/postman/postman_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-24 03:00:18.000000 commonX-0.5.2/common/postman/postman_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-24 03:00:18.000000 commonX-0.5.2/common/postman/postman_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.986121 commonX-0.5.2/common/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/args_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/assert_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/decorator_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/exception_utll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/image_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/requests_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/sys_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/typing_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.986121 commonX-0.5.2/commonX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 03:00:27.000000 commonX-0.5.2/commonX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 03:00:27.000000 commonX-0.5.2/commonX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:00:27.000000 commonX-0.5.2/commonX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 03:00:27.000000 commonX-0.5.2/commonX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:00:27.986121 commonX-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 03:00:18.000000 commonX-0.5.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `commonX-0.5.1/PKG-INFO` & `commonX-0.5.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
-Name: commonX
-Version: 0.5.1
-Summary: python common toolkit
-Home-page: https://github.com/hect0x7/common
-Author: hect0x7
-Author-email: 93357912+hect0x7@users.noreply.github.com
-Keywords: python,toolkit,postman
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires: requests
-Requires: requests_toolbelt
-Requires: PyYAML
-Requires: pyperclip
-Requires: curl_cffi
-Description-Content-Type: text/markdown
-
-
-python common toolkit
-
-see source code: https://github.com/hect0x7/common
+Metadata-Version: 2.1
+Name: commonX
+Version: 0.5.2
+Summary: python common toolkit
+Home-page: https://github.com/hect0x7/common
+Author: hect0x7
+Author-email: 93357912+hect0x7@users.noreply.github.com
+Keywords: python,toolkit,postman
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires: requests
+Requires: requests_toolbelt
+Requires: PyYAML
+Requires: pyperclip
+Requires: curl_cffi
+Description-Content-Type: text/markdown
+
+
+python common toolkit
+
+see source code: https://github.com/hect0x7/common
```

### Comparing `commonX-0.5.1/common/base/__init__.py` & `commonX-0.5.2/common/base/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .hook import HookChainContainer, JudgeHook, ProcessHook
-from .packer import Packer, JsonPacker, YmlPacker, PicklePacker, \
-    PackerUtil, PackerFactory
-from .multi_task import MultiTaskLauncher, \
-    multi_task_launcher, multi_thread_launcher, \
-    multi_process_launcher, thread_pool_executor, \
-    wait_a_task, wait_tasks, \
-    multi_task_launcher_batch, multi_call, \
-    CacheRunner, cache_run
-from .entity import SaveableEntity, IterableEntity
-from .registry import AtexitRegistry, ThreadRegistry
-from .mapper import Mapper, MapperFactory
-from .logger import Logger, LoggerFactory
-from .genor import Genor, GeneratorFactory
+from .hook import HookChainContainer, JudgeHook, ProcessHook
+from .packer import Packer, JsonPacker, YmlPacker, PicklePacker, \
+    PackerUtil, PackerFactory
+from .multi_task import MultiTaskLauncher, \
+    multi_task_launcher, multi_thread_launcher, \
+    multi_process_launcher, thread_pool_executor, \
+    wait_a_task, wait_tasks, \
+    multi_task_launcher_batch, multi_call, \
+    CacheRunner, cache_async_run
+from .entity import SaveableEntity, IterableEntity
+from .registry import AtexitRegistry, ThreadRegistry
+from .mapper import Mapper, MapperFactory
+from .logger import Logger, LoggerFactory
+from .genor import Genor, GeneratorFactory
```

### Comparing `commonX-0.5.1/common/base/hook.py` & `commonX-0.5.2/common/base/hook.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from common import Dict, List, Callable, Any, Optional
-
-
-class HookChainContainer:
-    """
-    封装数据结构：Dict[int, List[callable]]
-    键是int -> chain_key
-    值是List[callable] -> chain
-
-    """
-
-    def __init__(self):
-        self.__chain_dict: Dict[int, List[Callable]] = {}
-
-    def get_chain(self, chain_key: int) -> List[Callable]:
-        return self.__chain_dict.get(chain_key)
-
-    def register_hook(self, callback: Callable, chain_key: int):
-        if callback is None:
-            raise AssertionError(f"Parameter 'callback' mustn't be None (key is {chain_key})")
-
-        chain = self.get_chain(chain_key)
-
-        if chain is None:
-            self.__chain_dict[chain_key] = [callback]
-        else:
-            self.__chain_dict[chain_key].append(callback)
-
-    def register_ifnn(self, callback: Optional[Callable], chain_key: int):
-        if callback is not None:
-            self.register_hook(callback, chain_key)
-
-    def add_chain(self, chain_key: int):
-        if chain_key in self.__chain_dict:
-            raise KeyError(f"chain_key已存在: '{chain_key}'")
-        self.__chain_dict[chain_key] = []
-
-    def clear_chain(self, chain_key: int = None):
-        if chain_key is None:
-            self.__chain_dict.clear()
-        else:
-            self.get_chain(chain_key).clear()
-
-
-class ProcessHook(HookChainContainer):
-    ProcessFunc = Callable[[Any], Any]
-    process_chain_key = 1
-
-    def __init__(self):
-        super().__init__()
-        self.add_chain(self.process_chain_key)
-
-    def process(self, value: Any) -> Any:
-        process_chain = self.process_chain()
-
-        for processor in process_chain:
-            value = processor(value)
-
-        return value
-
-    def process_chain(self) -> List[Callable]:
-        return self.get_chain(self.process_chain_key)
-
-
-class JudgeHook(HookChainContainer):
-    JudgeFunc = Callable[[Any], bool]
-    judge_chain_key = 2
-
-    def __init__(self):
-        super().__init__()
-        self.add_chain(self.judge_chain_key)
-
-    def judge(self, value: Any, condition: bool = True) -> bool:
-        if condition is False:
-            return False
-
-        judge_chain = self.judge_chain()
-
-        for asserter in judge_chain:
-            if asserter(value) is False:
-                return False
-
-        return condition
-
-    def judge_chain(self) -> List[Callable]:
-        return self.get_chain(self.judge_chain_key)
-
-
-class ProcessSupport:
-
-    @staticmethod
-    def apply_callback(callback: ProcessHook.ProcessFunc,
-                       data,
-                       error_msg: str = '回调返回值不能为None'):
-        if callback is None:
-            return data
-
-        data = callback(data)
-        if data is None:
-            raise AssertionError(f"{error_msg}：callback={callback}")
-
-        return data
+from common import Dict, List, Callable, Any, Optional
+
+
+class HookChainContainer:
+    """
+    封装数据结构：Dict[int, List[callable]]
+    键是int -> chain_key
+    值是List[callable] -> chain
+
+    """
+
+    def __init__(self):
+        self.__chain_dict: Dict[int, List[Callable]] = {}
+
+    def get_chain(self, chain_key: int) -> List[Callable]:
+        return self.__chain_dict.get(chain_key)
+
+    def register_hook(self, callback: Callable, chain_key: int):
+        if callback is None:
+            raise AssertionError(f"Parameter 'callback' mustn't be None (key is {chain_key})")
+
+        chain = self.get_chain(chain_key)
+
+        if chain is None:
+            self.__chain_dict[chain_key] = [callback]
+        else:
+            self.__chain_dict[chain_key].append(callback)
+
+    def register_ifnn(self, callback: Optional[Callable], chain_key: int):
+        if callback is not None:
+            self.register_hook(callback, chain_key)
+
+    def add_chain(self, chain_key: int):
+        if chain_key in self.__chain_dict:
+            raise KeyError(f"chain_key已存在: '{chain_key}'")
+        self.__chain_dict[chain_key] = []
+
+    def clear_chain(self, chain_key: int = None):
+        if chain_key is None:
+            self.__chain_dict.clear()
+        else:
+            self.get_chain(chain_key).clear()
+
+
+class ProcessHook(HookChainContainer):
+    ProcessFunc = Callable[[Any], Any]
+    process_chain_key = 1
+
+    def __init__(self):
+        super().__init__()
+        self.add_chain(self.process_chain_key)
+
+    def process(self, value: Any) -> Any:
+        process_chain = self.process_chain()
+
+        for processor in process_chain:
+            value = processor(value)
+
+        return value
+
+    def process_chain(self) -> List[Callable]:
+        return self.get_chain(self.process_chain_key)
+
+
+class JudgeHook(HookChainContainer):
+    JudgeFunc = Callable[[Any], bool]
+    judge_chain_key = 2
+
+    def __init__(self):
+        super().__init__()
+        self.add_chain(self.judge_chain_key)
+
+    def judge(self, value: Any, condition: bool = True) -> bool:
+        if condition is False:
+            return False
+
+        judge_chain = self.judge_chain()
+
+        for asserter in judge_chain:
+            if asserter(value) is False:
+                return False
+
+        return condition
+
+    def judge_chain(self) -> List[Callable]:
+        return self.get_chain(self.judge_chain_key)
+
+
+class ProcessSupport:
+
+    @staticmethod
+    def apply_callback(callback: ProcessHook.ProcessFunc,
+                       data,
+                       error_msg: str = '回调返回值不能为None'):
+        if callback is None:
+            return data
+
+        data = callback(data)
+        if data is None:
+            raise AssertionError(f"{error_msg}：callback={callback}")
+
+        return data
```

### Comparing `commonX-0.5.1/common/base/logger.py` & `commonX-0.5.2/common/base/logger.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from common import Optional, Iterable, file_not_exists, create_file
-from .hook import ProcessSupport
-
-
-class Logger:
-
-    def is_done(self, obj) -> bool:
-        raise NotImplementedError
-
-    def is_not_done(self, obj) -> bool:
-        return not self.is_done(obj)
-
-    def add(self, obj, save=False):
-        raise NotImplementedError
-
-    def add_all(self, data: Iterable, save=False):
-        for each in data:
-            self.add(each, save)
-
-    def size(self) -> int:
-        raise NotImplementedError
-
-    def remove(self, obj, save=False):
-        raise NotImplementedError
-
-    def set_data(self, data):
-        raise NotImplementedError
-
-    def get_data(self) -> set:
-        raise NotImplementedError
-
-    def clear_data(self):
-        raise NotImplementedError
-
-    def load(self):
-        raise NotImplementedError
-
-    def save(self, callback=None):
-        raise NotImplementedError
-
-    def __len__(self):
-        return self.size()
-
-    def __contains__(self, item):
-        return self.is_done(item)
-
-    def __iter__(self):
-        raise NotImplementedError
-
-    def make_sure_loaded(self):
-        raise NotImplementedError
-
-
-# noinspection PyAbstractClass
-class AbstractSetLogger(Logger):
-
-    def __init__(self):
-        super().__init__()
-        self.data: Optional[set] = None
-
-    def is_done(self, obj) -> bool:
-        self.make_sure_loaded()
-        return obj in self.data
-
-    def add(self, obj, save=False):
-        self.make_sure_loaded()
-        self.data.add(obj)
-        if save is True:
-            self.save()
-
-    def set_data(self, data):
-        self.data = data
-
-    def get_data(self) -> set:
-        self.make_sure_loaded()
-        return self.data
-
-    def remove(self, obj, save=False):
-        if self.is_done(obj):
-            self.data.remove(obj)
-            if save is True:
-                self.save()
-
-    def size(self):
-        self.make_sure_loaded()
-        return len(self.data)
-
-    def clear_data(self):
-        self.data = set()
-
-    def make_sure_loaded(self):
-        if self.data is None:
-            self.load()
-
-    def __iter__(self):
-        self.make_sure_loaded()
-        return self.data.__iter__()
-
-
-class LoggerImpl(AbstractSetLogger, ProcessSupport):
-
-    def __init__(self, log_file_path: str):
-        super().__init__()
-        self.log_file_path = log_file_path
-
-    def load(self):
-        self.clear_data()
-        # check file
-        if file_not_exists(self.log_file_path):
-            create_file(self.log_file_path)
-            return
-        # read file
-        with open(self.log_file_path, 'r', encoding='utf-8') as f:
-            for line in f:
-                line = line.strip()
-                if len(line) != 0:
-                    self.data.add(line)
-
-    def save(self, callback=None):
-        # no load, no save
-        if self.data is None:
-            return
-
-        data = self.apply_callback(callback, self.data, "Logger.save方法的回调返回值不能为None")
-        with open(self.log_file_path, 'w', encoding='utf-8') as f:
-            for obj in data:
-                f.write(f"{obj}\n")
-
-    def __str__(self):
-        return self.log_file_path
-
-
-class LoggerFactory:
-
-    @classmethod
-    def get_logger(cls,
-                   filepath: str,
-                   load_after_created=False,
-                   save_at_exit=False,
-                   ) -> Logger:
-        """
-        工厂模式，暴露获取logger的接口
-
-        :param filepath: logger管理的文件路径
-        :param load_after_created: 是否创建后就立即加载数据，多线程下建议传True以保证数据一致
-        :param save_at_exit: atexit_register(logger.save)
-        :return: Logger实现类
-        """
-        logger = LoggerImpl(filepath)
-
-        # load after created
-        if load_after_created:
-            logger.load()
-
-        if save_at_exit:
-            from common import atexit_register
-            atexit_register(logger.save)
-
-        return logger
+from common import Optional, Iterable, file_not_exists, create_file
+from .hook import ProcessSupport
+
+
+class Logger:
+
+    def is_done(self, obj) -> bool:
+        raise NotImplementedError
+
+    def is_not_done(self, obj) -> bool:
+        return not self.is_done(obj)
+
+    def add(self, obj, save=False):
+        raise NotImplementedError
+
+    def add_all(self, data: Iterable, save=False):
+        for each in data:
+            self.add(each, save)
+
+    def size(self) -> int:
+        raise NotImplementedError
+
+    def remove(self, obj, save=False):
+        raise NotImplementedError
+
+    def set_data(self, data):
+        raise NotImplementedError
+
+    def get_data(self) -> set:
+        raise NotImplementedError
+
+    def clear_data(self):
+        raise NotImplementedError
+
+    def load(self):
+        raise NotImplementedError
+
+    def save(self, callback=None):
+        raise NotImplementedError
+
+    def __len__(self):
+        return self.size()
+
+    def __contains__(self, item):
+        return self.is_done(item)
+
+    def __iter__(self):
+        raise NotImplementedError
+
+    def make_sure_loaded(self):
+        raise NotImplementedError
+
+
+# noinspection PyAbstractClass
+class AbstractSetLogger(Logger):
+
+    def __init__(self):
+        super().__init__()
+        self.data: Optional[set] = None
+
+    def is_done(self, obj) -> bool:
+        self.make_sure_loaded()
+        return obj in self.data
+
+    def add(self, obj, save=False):
+        self.make_sure_loaded()
+        self.data.add(obj)
+        if save is True:
+            self.save()
+
+    def set_data(self, data):
+        self.data = data
+
+    def get_data(self) -> set:
+        self.make_sure_loaded()
+        return self.data
+
+    def remove(self, obj, save=False):
+        if self.is_done(obj):
+            self.data.remove(obj)
+            if save is True:
+                self.save()
+
+    def size(self):
+        self.make_sure_loaded()
+        return len(self.data)
+
+    def clear_data(self):
+        self.data = set()
+
+    def make_sure_loaded(self):
+        if self.data is None:
+            self.load()
+
+    def __iter__(self):
+        self.make_sure_loaded()
+        return self.data.__iter__()
+
+
+class LoggerImpl(AbstractSetLogger, ProcessSupport):
+
+    def __init__(self, log_file_path: str):
+        super().__init__()
+        self.log_file_path = log_file_path
+
+    def load(self):
+        self.clear_data()
+        # check file
+        if file_not_exists(self.log_file_path):
+            create_file(self.log_file_path)
+            return
+        # read file
+        with open(self.log_file_path, 'r', encoding='utf-8') as f:
+            for line in f:
+                line = line.strip()
+                if len(line) != 0:
+                    self.data.add(line)
+
+    def save(self, callback=None):
+        # no load, no save
+        if self.data is None:
+            return
+
+        data = self.apply_callback(callback, self.data, "Logger.save方法的回调返回值不能为None")
+        with open(self.log_file_path, 'w', encoding='utf-8') as f:
+            for obj in data:
+                f.write(f"{obj}\n")
+
+    def __str__(self):
+        return self.log_file_path
+
+
+class LoggerFactory:
+
+    @classmethod
+    def get_logger(cls,
+                   filepath: str,
+                   load_after_created=False,
+                   save_at_exit=False,
+                   ) -> Logger:
+        """
+        工厂模式，暴露获取logger的接口
+
+        :param filepath: logger管理的文件路径
+        :param load_after_created: 是否创建后就立即加载数据，多线程下建议传True以保证数据一致
+        :param save_at_exit: atexit_register(logger.save)
+        :return: Logger实现类
+        """
+        logger = LoggerImpl(filepath)
+
+        # load after created
+        if load_after_created:
+            logger.load()
+
+        if save_at_exit:
+            from common import atexit_register
+            atexit_register(logger.save)
+
+        return logger
```

### Comparing `commonX-0.5.1/common/base/mapper.py` & `commonX-0.5.2/common/base/mapper.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-from common import Any, Optional, Dict, Iterable
-from common import file_not_exists, create_file
-from .hook import ProcessSupport
-
-
-class Mapper:
-
-    def set(self, key: Any, value: Any, save=False):
-        raise NotImplementedError
-
-    def get(self, key: Any, default_v: Any = None) -> Any:
-        raise NotImplementedError
-
-    def has_not_key(self, key: Any) -> bool:
-        return not self.__contains__(key)
-
-    def remove(self, obj, save=False):
-        raise NotImplementedError
-
-    def size(self) -> int:
-        raise NotImplementedError
-
-    def set_data(self, data: dict):
-        raise NotImplementedError
-
-    def get_data(self) -> dict:
-        raise NotImplementedError
-
-    def clear_data(self):
-        raise NotImplementedError
-
-    def load(self):
-        raise NotImplementedError
-
-    def save(self, callback=None):
-        raise NotImplementedError
-
-    def make_sure_loaded(self):
-        raise NotImplementedError
-
-    def items(self):
-        raise NotImplementedError
-
-    def keys(self) -> Iterable[str]:
-        raise NotImplementedError
-
-    def values(self) -> Iterable[str]:
-        raise NotImplementedError
-
-    def get_separator(self) -> str:
-        raise NotImplementedError
-
-    def set_separator(self, separator: str):
-        raise NotImplementedError
-
-    def __iter__(self):
-        raise NotImplementedError
-
-    def __getitem__(self, key):
-        obj = self.get(key)
-        if obj is None:
-            raise KeyError(key)
-        return obj
-
-    def __setitem__(self, key, value):
-        self.set(key, value)
-
-    def __contains__(self, key):
-        raise NotImplementedError
-
-    def __len__(self):
-        return self.size()
-
-
-# noinspection PyAbstractClass
-class AbstractDictMapper(Mapper):
-
-    def __init__(self):
-        self.data: Optional[Dict] = None
-
-    def set(self, key, value, save=False):
-        self.make_sure_loaded()
-        self.data[key] = value
-        if save is True:
-            self.save()
-
-    def get(self, key, default_v=None) -> Any:
-        self.make_sure_loaded()
-        return self.data.get(key, default_v)
-
-    def __contains__(self, key):
-        self.make_sure_loaded()
-        return self.data.__contains__(key)
-
-    def remove(self, key, save=False):
-        self.make_sure_loaded()
-        if key in self.data:
-            del self.data[key]
-            if save is True:
-                self.save()
-
-    def size(self) -> int:
-        self.make_sure_loaded()
-        return len(self.data)
-
-    def set_data(self, data):
-        self.data = data
-
-    def get_data(self):
-        self.make_sure_loaded()
-        return self.data
-
-    def clear_data(self):
-        self.data = {}
-
-    def make_sure_loaded(self):
-        if self.data is None:
-            self.load()
-
-    def __iter__(self):
-        self.make_sure_loaded()
-        return iter(self.data.items())
-
-    def __len__(self):
-        self.make_sure_loaded()
-        return len(self.data)
-
-    def items(self):
-        self.make_sure_loaded()
-        return self.data.items()
-
-    def keys(self):
-        self.make_sure_loaded()
-        return self.data.keys()
-
-    def values(self):
-        self.make_sure_loaded()
-        return self.data.values()
-
-
-class MapperImpl(AbstractDictMapper, ProcessSupport):
-
-    def __init__(self, map_file_path: str, separator: str):
-        super().__init__()
-        self.map_file_path = map_file_path
-        self.separator = separator
-
-    def load(self):
-        self.clear_data()
-
-        # check file
-        if file_not_exists(self.map_file_path):
-            create_file(self.map_file_path)
-            return
-
-        # read file
-        with open(self.map_file_path, 'r', encoding='utf-8') as f:
-            for line in f:
-                line = line.strip()
-                if len(line) == 0:
-                    continue
-
-                split_word_index = line.find(self.separator)
-                if split_word_index == -1:
-                    continue
-
-                key = line[:split_word_index].strip()
-                value = line[split_word_index + 1:].strip()
-                self.data[key] = value
-
-    def save(self, callback=None):
-        if self.data is None:
-            return
-
-        data = self.apply_callback(callback, self.data, "Mapper.save方法的回调返回值不能为None")
-
-        # write file
-        with open(self.map_file_path, 'w', encoding='utf-8') as f:
-            if isinstance(data, (tuple, list)):
-                for (k, v) in data:
-                    f.write(f"{k}{self.separator}{v}\n")
-            elif isinstance(data, dict):
-                for k, v in data.items():
-                    f.write(f"{k}{self.separator}{v}\n")
-            else:
-                raise AssertionError(f"无法序列化data, type={type(data)}")
-
-        return data
-
-    def get_separator(self) -> str:
-        return self.separator
-
-    def set_separator(self, separator: str):
-        self.separator = separator
-
-    def __str__(self) -> str:
-        return self.map_file_path
-
-
-class MapperFactory:
-
-    @classmethod
-    def get_mapper(cls,
-                   filepath: str,
-                   separator=',',
-                   load_after_created=False,
-                   save_at_exit=False
-                   ) -> Mapper:
-        mapper = MapperImpl(filepath, separator)
-
-        if load_after_created:
-            mapper.load()
-
-        if save_at_exit:
-            from common import atexit_register
-            atexit_register(mapper.save)
-
-        return mapper
+from common import Any, Optional, Dict, Iterable
+from common import file_not_exists, create_file
+from .hook import ProcessSupport
+
+
+class Mapper:
+
+    def set(self, key: Any, value: Any, save=False):
+        raise NotImplementedError
+
+    def get(self, key: Any, default_v: Any = None) -> Any:
+        raise NotImplementedError
+
+    def has_not_key(self, key: Any) -> bool:
+        return not self.__contains__(key)
+
+    def remove(self, obj, save=False):
+        raise NotImplementedError
+
+    def size(self) -> int:
+        raise NotImplementedError
+
+    def set_data(self, data: dict):
+        raise NotImplementedError
+
+    def get_data(self) -> dict:
+        raise NotImplementedError
+
+    def clear_data(self):
+        raise NotImplementedError
+
+    def load(self):
+        raise NotImplementedError
+
+    def save(self, callback=None):
+        raise NotImplementedError
+
+    def make_sure_loaded(self):
+        raise NotImplementedError
+
+    def items(self):
+        raise NotImplementedError
+
+    def keys(self) -> Iterable[str]:
+        raise NotImplementedError
+
+    def values(self) -> Iterable[str]:
+        raise NotImplementedError
+
+    def get_separator(self) -> str:
+        raise NotImplementedError
+
+    def set_separator(self, separator: str):
+        raise NotImplementedError
+
+    def __iter__(self):
+        raise NotImplementedError
+
+    def __getitem__(self, key):
+        obj = self.get(key)
+        if obj is None:
+            raise KeyError(key)
+        return obj
+
+    def __setitem__(self, key, value):
+        self.set(key, value)
+
+    def __contains__(self, key):
+        raise NotImplementedError
+
+    def __len__(self):
+        return self.size()
+
+
+# noinspection PyAbstractClass
+class AbstractDictMapper(Mapper):
+
+    def __init__(self):
+        self.data: Optional[Dict] = None
+
+    def set(self, key, value, save=False):
+        self.make_sure_loaded()
+        self.data[key] = value
+        if save is True:
+            self.save()
+
+    def get(self, key, default_v=None) -> Any:
+        self.make_sure_loaded()
+        return self.data.get(key, default_v)
+
+    def __contains__(self, key):
+        self.make_sure_loaded()
+        return self.data.__contains__(key)
+
+    def remove(self, key, save=False):
+        self.make_sure_loaded()
+        if key in self.data:
+            del self.data[key]
+            if save is True:
+                self.save()
+
+    def size(self) -> int:
+        self.make_sure_loaded()
+        return len(self.data)
+
+    def set_data(self, data):
+        self.data = data
+
+    def get_data(self):
+        self.make_sure_loaded()
+        return self.data
+
+    def clear_data(self):
+        self.data = {}
+
+    def make_sure_loaded(self):
+        if self.data is None:
+            self.load()
+
+    def __iter__(self):
+        self.make_sure_loaded()
+        return iter(self.data.items())
+
+    def __len__(self):
+        self.make_sure_loaded()
+        return len(self.data)
+
+    def items(self):
+        self.make_sure_loaded()
+        return self.data.items()
+
+    def keys(self):
+        self.make_sure_loaded()
+        return self.data.keys()
+
+    def values(self):
+        self.make_sure_loaded()
+        return self.data.values()
+
+
+class MapperImpl(AbstractDictMapper, ProcessSupport):
+
+    def __init__(self, map_file_path: str, separator: str):
+        super().__init__()
+        self.map_file_path = map_file_path
+        self.separator = separator
+
+    def load(self):
+        self.clear_data()
+
+        # check file
+        if file_not_exists(self.map_file_path):
+            create_file(self.map_file_path)
+            return
+
+        # read file
+        with open(self.map_file_path, 'r', encoding='utf-8') as f:
+            for line in f:
+                line = line.strip()
+                if len(line) == 0:
+                    continue
+
+                split_word_index = line.find(self.separator)
+                if split_word_index == -1:
+                    continue
+
+                key = line[:split_word_index].strip()
+                value = line[split_word_index + 1:].strip()
+                self.data[key] = value
+
+    def save(self, callback=None):
+        if self.data is None:
+            return
+
+        data = self.apply_callback(callback, self.data, "Mapper.save方法的回调返回值不能为None")
+
+        # write file
+        with open(self.map_file_path, 'w', encoding='utf-8') as f:
+            if isinstance(data, (tuple, list)):
+                for (k, v) in data:
+                    f.write(f"{k}{self.separator}{v}\n")
+            elif isinstance(data, dict):
+                for k, v in data.items():
+                    f.write(f"{k}{self.separator}{v}\n")
+            else:
+                raise AssertionError(f"无法序列化data, type={type(data)}")
+
+        return data
+
+    def get_separator(self) -> str:
+        return self.separator
+
+    def set_separator(self, separator: str):
+        self.separator = separator
+
+    def __str__(self) -> str:
+        return self.map_file_path
+
+
+class MapperFactory:
+
+    @classmethod
+    def get_mapper(cls,
+                   filepath: str,
+                   separator=',',
+                   load_after_created=False,
+                   save_at_exit=False
+                   ) -> Mapper:
+        mapper = MapperImpl(filepath, separator)
+
+        if load_after_created:
+            mapper.load()
+
+        if save_at_exit:
+            from common import atexit_register
+            atexit_register(mapper.save)
+
+        return mapper
```

### Comparing `commonX-0.5.1/common/base/multi_task.py` & `commonX-0.5.2/common/base/multi_task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,298 +1,298 @@
-from common import Thread, Process, \
-    List, Callable, Iterable, Optional, Any, Union, Type, Dict, Tuple, \
-    process_args_kwargs, process_single_arg_to_args_and_kwargs, \
-    is_function, sleep, current_thread
-
-
-def wait_a_task(task):
-    if task == current_thread():
-        return
-
-    while task.is_alive():
-        task.join(timeout=1)
-
-
-def wait_tasks(tasks: Iterable[Any]):
-    for task in tasks:
-        if isinstance(task, list):
-            wait_tasks(task)
-            continue
-
-        wait_a_task(task)
-
-
-class MultiTaskLauncher:
-    OptionalTask = Union[Thread, Process, None]
-
-    def __init__(self, task_meta_data: Optional[Dict[str, Any]] = None):
-        if task_meta_data is None:
-            task_meta_data = {}
-
-        self.task_ls: list = []
-        self.task_meta_data_kwargs: dict = task_meta_data
-
-    def create_task(self,
-                    target: Callable,
-                    args: Optional[Any] = None,
-                    kwargs: Optional[dict] = None,
-                    TaskType=Thread) -> Union[Thread, Process]:
-        args, kwargs = process_args_kwargs(args, kwargs)
-        t = self.new_task(TaskType,
-                          target=target,
-                          args=args,
-                          kwargs=kwargs,
-                          meta_data=self.task_meta_data_kwargs)
-        t.start()
-        self.task_ls.append(t)
-        return t
-
-    def add_task(self, task: OptionalTask):
-        if task is not None and task.is_alive():
-            self.task_ls.append(task)
-
-    def wait_finish(self):
-        wait_tasks(self.task_ls)
-
-    """
-    收集所有的 Task
-    """
-    tasks_of_launcher_context = []
-
-    @classmethod
-    def new_task(cls,
-                 TaskType: Type,
-                 target: Callable,
-                 args: Iterable,
-                 kwargs: dict,
-                 meta_data: dict):
-
-        task = TaskType(target=target,
-                        args=args,
-                        kwargs=kwargs,
-                        **meta_data)
-        cls.tasks_of_launcher_context.append(task)
-
-        return task
-
-    @classmethod
-    def sleep_with_condition(cls, condition, index, obj):
-        if condition is None:
-            return
-
-        interval_to_sleep = condition(index, obj) if is_function(condition) else condition
-
-        if isinstance(interval_to_sleep, int) or isinstance(interval_to_sleep, float):
-            if interval_to_sleep > 0:
-                sleep(interval_to_sleep)
-        else:
-            # condition 不是以下类型，则暂未实现以何种方式调用
-            # 1. 函数
-            # 2. int
-            # 3. float
-            raise NotImplementedError
-
-    @classmethod
-    def build_daemon(cls):
-        return MultiTaskLauncher({"daemon": True})
-
-
-def multi_task_launcher(iter_objs: Iterable,
-                        apply_each_obj_func: Callable,
-                        TaskType: Union[Type[Thread], Type[Process]],
-                        wait_finish=True,
-                        sleep_interval: Any = -1,
-                        batch_size: Optional[int] = None,
-                        **meta_data_kwargs
-                        ) -> list:
-    if batch_size is not None:
-        return multi_task_launcher_batch(
-            iter_objs,
-            apply_each_obj_func,
-            batch_size,
-            TaskType,
-            sleep_interval,
-        )
-
-    task_ls: list = []
-
-    for index, obj in enumerate(iter_objs):
-        args, kwargs = process_single_arg_to_args_and_kwargs(obj)
-        meta_data = {
-            meta_arg: meta_value(index) if is_function(meta_value) else meta_value
-            for meta_arg, meta_value in meta_data_kwargs.items()
-        }
-
-        # set daemon default True to ensure that
-        # program can be forced to exit by ctrl + c successfully in windows
-        meta_data.setdefault("daemon", True)
-
-        task = MultiTaskLauncher.new_task(TaskType=TaskType,
-                                          target=apply_each_obj_func,
-                                          args=args,
-                                          kwargs=kwargs,
-                                          meta_data=meta_data)
-        task.start()
-        task_ls.append(task)
-
-        MultiTaskLauncher.sleep_with_condition(sleep_interval, index + 1, obj)
-
-    if wait_finish is True:
-        wait_tasks(task_ls)
-
-    return task_ls
-
-
-def multi_thread_launcher(iter_objs: Iterable,
-                          apply_each_obj_func: Callable,
-                          wait_finish=True,
-                          sleep_interval=-1,
-                          batch_size=None,
-                          **meta_data_kwargs
-                          ) -> List[Thread]:
-    return multi_task_launcher(iter_objs,
-                               apply_each_obj_func,
-                               Thread,
-                               wait_finish,
-                               sleep_interval,
-                               batch_size,
-                               **meta_data_kwargs
-                               )
-
-
-def multi_process_launcher(iter_objs: Iterable,
-                           apply_each_obj_func: Callable,
-                           wait_finish=True,
-                           sleep_interval=-1,
-                           batch_size=None,
-                           **meta_data_kwargs,
-                           ) -> List[Process]:
-    return multi_task_launcher(iter_objs,
-                               apply_each_obj_func,
-                               Process,
-                               wait_finish,
-                               sleep_interval,
-                               batch_size,
-                               **meta_data_kwargs
-                               )
-
-
-def thread_pool_executor(
-        iter_objs: Iterable,
-        apply_each_obj_func: Callable,
-        wait_finish=True,
-        max_workers=None,
-):
-    def wrap_func(*args, **kwargs):
-        try:
-            apply_each_obj_func(*args, **kwargs)
-        except Exception:
-            from common import traceback_print_exec
-            traceback_print_exec()
-
-    ret = []
-    from concurrent.futures import ThreadPoolExecutor
-    executor = ThreadPoolExecutor(max_workers)
-    for obj in iter_objs:
-        args, kwargs = process_single_arg_to_args_and_kwargs(obj)
-        future = executor.submit(wrap_func, *args, **kwargs)
-        ret.append(future)
-
-    executor.shutdown(wait_finish)
-    return ret
-
-
-def multi_task_launcher_batch(iter_objs: Iterable,
-                              apply_each_obj_func: Callable,
-                              batch_size: int,
-                              TaskType=Thread,
-                              sleep_interval: Any = -1,
-                              **meta_data_kwargs):
-    meta_data_kwargs.setdefault("daemon", True)
-    task_ls = []
-
-    for index, obj in enumerate(iter_objs):
-        args, kwargs = process_single_arg_to_args_and_kwargs(obj)
-        meta_data = {
-            meta_arg: meta_value(index) if is_function(meta_value) else meta_value
-            for meta_arg, meta_value in meta_data_kwargs.items()
-        }
-
-        task = MultiTaskLauncher.new_task(TaskType=TaskType,
-                                          target=apply_each_obj_func,
-                                          args=args,
-                                          kwargs=kwargs,
-                                          meta_data=meta_data)
-        task.start()
-        task_ls.append(task)
-
-        if len(task_ls) == batch_size:
-            wait_tasks(task_ls)
-            task_ls.clear()
-
-        MultiTaskLauncher.sleep_with_condition(sleep_interval, index + 1, obj)
-
-    if task_ls:
-        wait_tasks(task_ls)
-
-    return task_ls
-
-
-def multi_call(func, iter_objs, launcher=multi_thread_launcher, wait=True) -> Union[dict, Tuple[dict, List]]:
-    ret_dict = {}
-
-    def get_ret(obj):
-        ret = func(obj)
-        ret_dict[obj] = ret
-
-    task_ls = launcher(
-        iter_objs=iter_objs,
-        apply_each_obj_func=get_ret,
-        wait_finish=wait
-    )
-
-    if wait is not True:
-        return ret_dict, task_ls
-
-    return ret_dict
-
-
-"""
-提供阻塞获取一个线程的target函数返回值
-"""
-
-
-class CacheRunner(Thread):
-
-    def __init__(self, group=None, target=None, name=None,
-                 args=(), kwargs=None, *, daemon=None):
-        super().__init__(group, self.deco_target(target), name, args, kwargs, daemon=daemon)
-        self._cache = None
-
-    def get(self) -> Any:
-        cache = self._cache
-
-        if cache is not None:
-            return cache
-
-        if not self.is_alive():
-            self.start()
-
-        self.join()
-        return self._cache
-
-    def deco_target(self, target):
-
-        def deco_cache():
-            result = target()
-            self._cache = result
-
-        return deco_cache
-
-    def __call__(self, *args, **kwargs):
-        return self.get()
-
-
-def cache_run(func) -> CacheRunner:
-    cache_runner = CacheRunner(target=func)
-    cache_runner.start()
-    return cache_runner
+from common import Thread, Process, \
+    List, Callable, Iterable, Optional, Any, Union, Type, Dict, Tuple, \
+    process_args_kwargs, process_single_arg_to_args_and_kwargs, \
+    is_function, sleep, current_thread
+
+
+def wait_a_task(task):
+    if task == current_thread():
+        return
+
+    while task.is_alive():
+        task.join(timeout=1)
+
+
+def wait_tasks(tasks: Iterable[Any]):
+    for task in tasks:
+        if isinstance(task, list):
+            wait_tasks(task)
+            continue
+
+        wait_a_task(task)
+
+
+class MultiTaskLauncher:
+    OptionalTask = Union[Thread, Process, None]
+
+    def __init__(self, task_meta_data: Optional[Dict[str, Any]] = None):
+        if task_meta_data is None:
+            task_meta_data = {}
+
+        self.task_ls: list = []
+        self.task_meta_data_kwargs: dict = task_meta_data
+
+    def create_task(self,
+                    target: Callable,
+                    args: Optional[Any] = None,
+                    kwargs: Optional[dict] = None,
+                    TaskType=Thread) -> Union[Thread, Process]:
+        args, kwargs = process_args_kwargs(args, kwargs)
+        t = self.new_task(TaskType,
+                          target=target,
+                          args=args,
+                          kwargs=kwargs,
+                          meta_data=self.task_meta_data_kwargs)
+        t.start()
+        self.task_ls.append(t)
+        return t
+
+    def add_task(self, task: OptionalTask):
+        if task is not None and task.is_alive():
+            self.task_ls.append(task)
+
+    def wait_finish(self):
+        wait_tasks(self.task_ls)
+
+    """
+    收集所有的 Task
+    """
+    tasks_of_launcher_context = []
+
+    @classmethod
+    def new_task(cls,
+                 TaskType: Type,
+                 target: Callable,
+                 args: Iterable,
+                 kwargs: dict,
+                 meta_data: dict):
+
+        task = TaskType(target=target,
+                        args=args,
+                        kwargs=kwargs,
+                        **meta_data)
+        cls.tasks_of_launcher_context.append(task)
+
+        return task
+
+    @classmethod
+    def sleep_with_condition(cls, condition, index, obj):
+        if condition is None:
+            return
+
+        interval_to_sleep = condition(index, obj) if is_function(condition) else condition
+
+        if isinstance(interval_to_sleep, int) or isinstance(interval_to_sleep, float):
+            if interval_to_sleep > 0:
+                sleep(interval_to_sleep)
+        else:
+            # condition 不是以下类型，则暂未实现以何种方式调用
+            # 1. 函数
+            # 2. int
+            # 3. float
+            raise NotImplementedError
+
+    @classmethod
+    def build_daemon(cls):
+        return MultiTaskLauncher({"daemon": True})
+
+
+def multi_task_launcher(iter_objs: Iterable,
+                        apply_each_obj_func: Callable,
+                        TaskType: Union[Type[Thread], Type[Process]],
+                        wait_finish=True,
+                        sleep_interval: Any = -1,
+                        batch_size: Optional[int] = None,
+                        **meta_data_kwargs
+                        ) -> list:
+    if batch_size is not None:
+        return multi_task_launcher_batch(
+            iter_objs,
+            apply_each_obj_func,
+            batch_size,
+            TaskType,
+            sleep_interval,
+        )
+
+    task_ls: list = []
+
+    for index, obj in enumerate(iter_objs):
+        args, kwargs = process_single_arg_to_args_and_kwargs(obj)
+        meta_data = {
+            meta_arg: meta_value(index) if is_function(meta_value) else meta_value
+            for meta_arg, meta_value in meta_data_kwargs.items()
+        }
+
+        # set daemon default True to ensure that
+        # program can be forced to exit by ctrl + c successfully in windows
+        meta_data.setdefault("daemon", True)
+
+        task = MultiTaskLauncher.new_task(TaskType=TaskType,
+                                          target=apply_each_obj_func,
+                                          args=args,
+                                          kwargs=kwargs,
+                                          meta_data=meta_data)
+        task.start()
+        task_ls.append(task)
+
+        MultiTaskLauncher.sleep_with_condition(sleep_interval, index + 1, obj)
+
+    if wait_finish is True:
+        wait_tasks(task_ls)
+
+    return task_ls
+
+
+def multi_thread_launcher(iter_objs: Iterable,
+                          apply_each_obj_func: Callable,
+                          wait_finish=True,
+                          sleep_interval=-1,
+                          batch_size=None,
+                          **meta_data_kwargs
+                          ) -> List[Thread]:
+    return multi_task_launcher(iter_objs,
+                               apply_each_obj_func,
+                               Thread,
+                               wait_finish,
+                               sleep_interval,
+                               batch_size,
+                               **meta_data_kwargs
+                               )
+
+
+def multi_process_launcher(iter_objs: Iterable,
+                           apply_each_obj_func: Callable,
+                           wait_finish=True,
+                           sleep_interval=-1,
+                           batch_size=None,
+                           **meta_data_kwargs,
+                           ) -> List[Process]:
+    return multi_task_launcher(iter_objs,
+                               apply_each_obj_func,
+                               Process,
+                               wait_finish,
+                               sleep_interval,
+                               batch_size,
+                               **meta_data_kwargs
+                               )
+
+
+def thread_pool_executor(
+        iter_objs: Iterable,
+        apply_each_obj_func: Callable,
+        wait_finish=True,
+        max_workers=None,
+):
+    def wrap_func(*args, **kwargs):
+        try:
+            apply_each_obj_func(*args, **kwargs)
+        except Exception:
+            from common import traceback_print_exec
+            traceback_print_exec()
+
+    ret = []
+    from concurrent.futures import ThreadPoolExecutor
+    executor = ThreadPoolExecutor(max_workers)
+    for obj in iter_objs:
+        args, kwargs = process_single_arg_to_args_and_kwargs(obj)
+        future = executor.submit(wrap_func, *args, **kwargs)
+        ret.append(future)
+
+    executor.shutdown(wait_finish)
+    return ret
+
+
+def multi_task_launcher_batch(iter_objs: Iterable,
+                              apply_each_obj_func: Callable,
+                              batch_size: int,
+                              TaskType=Thread,
+                              sleep_interval: Any = -1,
+                              **meta_data_kwargs):
+    meta_data_kwargs.setdefault("daemon", True)
+    task_ls = []
+
+    for index, obj in enumerate(iter_objs):
+        args, kwargs = process_single_arg_to_args_and_kwargs(obj)
+        meta_data = {
+            meta_arg: meta_value(index) if is_function(meta_value) else meta_value
+            for meta_arg, meta_value in meta_data_kwargs.items()
+        }
+
+        task = MultiTaskLauncher.new_task(TaskType=TaskType,
+                                          target=apply_each_obj_func,
+                                          args=args,
+                                          kwargs=kwargs,
+                                          meta_data=meta_data)
+        task.start()
+        task_ls.append(task)
+
+        if len(task_ls) == batch_size:
+            wait_tasks(task_ls)
+            task_ls.clear()
+
+        MultiTaskLauncher.sleep_with_condition(sleep_interval, index + 1, obj)
+
+    if task_ls:
+        wait_tasks(task_ls)
+
+    return task_ls
+
+
+def multi_call(func, iter_objs, launcher=multi_thread_launcher, wait=True) -> Union[dict, Tuple[dict, List]]:
+    ret_dict = {}
+
+    def get_ret(obj):
+        ret = func(obj)
+        ret_dict[obj] = ret
+
+    task_ls = launcher(
+        iter_objs=iter_objs,
+        apply_each_obj_func=get_ret,
+        wait_finish=wait
+    )
+
+    if wait is not True:
+        return ret_dict, task_ls
+
+    return ret_dict
+
+
+"""
+提供阻塞获取一个线程的target函数返回值
+"""
+
+
+class CacheRunner(Thread):
+
+    def __init__(self, group=None, target=None, name=None,
+                 args=(), kwargs=None, *, daemon=None):
+        super().__init__(group, self.deco_target(target), name, args, kwargs, daemon=daemon)
+        self._cache = None
+
+    def get(self) -> Any:
+        cache = self._cache
+
+        if cache is not None:
+            return cache
+
+        if not self.is_alive():
+            self.start()
+
+        self.join()
+        return self._cache
+
+    def deco_target(self, target):
+
+        def deco_cache():
+            result = target()
+            self._cache = result
+
+        return deco_cache
+
+    def __call__(self, *args, **kwargs):
+        return self.get()
+
+
+def cache_async_run(func) -> CacheRunner:
+    cache_runner = CacheRunner(target=func)
+    cache_runner.start()
+    return cache_runner
```

### Comparing `commonX-0.5.1/common/base/packer.py` & `commonX-0.5.2/common/base/packer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-from common import Callable, Type, Dict, Union, Optional, Any, Tuple
-
-
-class Packer:
-
-    def pack(self, obj: object, filepath: str):
-        raise NotImplementedError
-
-    def unpack(self, filepath: str, clazz=None) -> Any:
-        """
-        反序列化得到对象
-
-        :param filepath: 文件路径
-        :param clazz: 预期的class对象，Packer不一定会使用此参数（如YmlPacker就不会，而JsonPacker会）。
-        此参数需要是callable，并且能返回一个对象，即：obj = clazz()
-        :return:
-        """
-        raise NotImplementedError
-
-
-class AbstractSerializablePacker(Packer):
-    pack_mode = 'w'
-    unpack_mode = 'r'
-    encoding = 'utf-8'
-
-    def pack(self, obj: object, filepath: str):
-        self.with_file(filepath,
-                       self.pack_mode,
-                       self.dump,
-                       obj=obj,
-                       )
-
-    def unpack(self, filepath: str, clazz=None) -> Any:
-        return self.with_file(filepath,
-                              self.unpack_mode,
-                              self.load,
-                              clazz=clazz,
-                              )
-
-    def dump(self, fp, obj: object):
-        raise NotImplementedError
-
-    def load(self, fp, clazz: Optional[Type]) -> Any:
-        raise NotImplementedError
-
-    @classmethod
-    def with_file(cls,
-                  filepath: str,
-                  mode: str,
-                  visitor: Callable,
-                  **kwargs
-                  ):
-        with open(filepath, mode, encoding=cls.encoding) as f:
-            return visitor(f, **kwargs)
-
-
-class YmlPacker(AbstractSerializablePacker):
-
-    def dump(self, fp, obj):
-        import yaml
-        yaml.dump(obj,
-                  fp,
-                  allow_unicode=True,
-                  indent=2,
-                  )
-
-    def load(self, fp, clazz) -> Any:
-        import yaml
-        return yaml.load(fp, yaml.FullLoader)
-
-    @staticmethod
-    def add_constructor(tag, constructor: Callable):
-        from yaml import add_constructor
-        add_constructor(tag, constructor)
-
-
-class JsonPacker(AbstractSerializablePacker):
-
-    def dump(self, fp, obj, indent=2):
-        from json import dump
-        dump(self.to_dict(obj),
-             fp,
-             ensure_ascii=False,
-             indent=indent,
-             )
-
-    def load(self, fp, clazz) -> Any:
-        from json import load
-        dic: dict = load(fp)
-        if clazz is None:
-            return dic
-
-        obj: object = clazz()
-        obj.__dict__.update(dic)
-        return obj
-
-    @classmethod
-    def to_dict(cls, obj):
-        """将对象转换为字典"""
-        if hasattr(obj, "__dict__"):
-            d = dict(obj.__dict__)
-            for key, value in d.items():
-                if hasattr(value, "__dict__"):
-                    d[key] = cls.to_dict(value)
-            return d
-        elif isinstance(obj, list):
-            return [cls.to_dict(item) for item in obj]
-        else:
-            return obj
-
-
-class PicklePacker(AbstractSerializablePacker):
-    pack_mode = 'wb'
-    unpack_mode = 'rb'
-    encoding = None
-
-    def dump(self, fp, obj: object):
-        import pickle
-        pickle.dump(obj, fp)
-
-    def load(self, fp, clazz: Optional[Type]) -> Any:
-        import pickle
-        return pickle.load(fp)
-
-
-class PackerFactory:
-    mode_yml = 'yml'
-    mode_json = 'json'
-    mode_py_pickle = 'pickle'
-
-    mode_mapping: Dict[str, Union[Packer, Type[Packer]]] = {
-        mode_yml: YmlPacker,
-        mode_json: JsonPacker,
-        mode_py_pickle: PicklePacker,
-
-    }
-
-    @classmethod
-    def get_packer(cls, mode: str) -> Packer:
-        packer_caller = cls.mode_mapping.get(mode, None)
-
-        if packer_caller is None:
-            raise AssertionError(f"unknown mode: '{mode}', acceptable modes={list(cls.mode_mapping.keys())}")
-
-        packer: Packer
-        if isinstance(packer_caller, Packer):
-            packer_caller: Packer
-            packer = packer_caller
-        else:
-            packer_caller: Type[Packer]
-            packer = packer_caller()
-            # cache
-            cls.mode_mapping[mode] = packer
-
-        return packer
-
-
-class PackerUtil:
-
-    @staticmethod
-    def get_packer(filepath: str):
-        mode_intelligent = filepath[filepath.rfind('.') + 1::]
-        return PackerFactory.get_packer(mode=mode_intelligent)
-
-    @classmethod
-    def pack(cls, obj: object, filepath: str, packer=None, only_fields=False):
-        packer = packer or cls.get_packer(filepath)
-
-        # 只序列化类属性
-        if only_fields is True:
-            import inspect
-            obj = inspect.getmembers(obj, lambda f: not inspect.ismethod(f))
-            obj = dict(filter(lambda f: not f[0].startswith('_'), obj))
-
-        packer.pack(obj, filepath)
-
-    @classmethod
-    def unpack(cls, filepath: str, clazz=None, packer=None) -> Tuple[Any, Packer]:
-        packer = packer or cls.get_packer(filepath)
-        return packer.unpack(filepath, clazz), packer
+from common import Callable, Type, Dict, Union, Optional, Any, Tuple
+
+
+class Packer:
+
+    def pack(self, obj: object, filepath: str):
+        raise NotImplementedError
+
+    def unpack(self, filepath: str, clazz=None) -> Any:
+        """
+        反序列化得到对象
+
+        :param filepath: 文件路径
+        :param clazz: 预期的class对象，Packer不一定会使用此参数（如YmlPacker就不会，而JsonPacker会）。
+        此参数需要是callable，并且能返回一个对象，即：obj = clazz()
+        :return:
+        """
+        raise NotImplementedError
+
+
+class AbstractSerializablePacker(Packer):
+    pack_mode = 'w'
+    unpack_mode = 'r'
+    encoding = 'utf-8'
+
+    def pack(self, obj: object, filepath: str):
+        self.with_file(filepath,
+                       self.pack_mode,
+                       self.dump,
+                       obj=obj,
+                       )
+
+    def unpack(self, filepath: str, clazz=None) -> Any:
+        return self.with_file(filepath,
+                              self.unpack_mode,
+                              self.load,
+                              clazz=clazz,
+                              )
+
+    def dump(self, fp, obj: object):
+        raise NotImplementedError
+
+    def load(self, fp, clazz: Optional[Type]) -> Any:
+        raise NotImplementedError
+
+    @classmethod
+    def with_file(cls,
+                  filepath: str,
+                  mode: str,
+                  visitor: Callable,
+                  **kwargs
+                  ):
+        with open(filepath, mode, encoding=cls.encoding) as f:
+            return visitor(f, **kwargs)
+
+
+class YmlPacker(AbstractSerializablePacker):
+
+    def dump(self, fp, obj):
+        import yaml
+        yaml.dump(obj,
+                  fp,
+                  allow_unicode=True,
+                  indent=2,
+                  )
+
+    def load(self, fp, clazz) -> Any:
+        import yaml
+        return yaml.load(fp, yaml.FullLoader)
+
+    @staticmethod
+    def add_constructor(tag, constructor: Callable):
+        from yaml import add_constructor
+        add_constructor(tag, constructor)
+
+
+class JsonPacker(AbstractSerializablePacker):
+
+    def dump(self, fp, obj, indent=2):
+        from json import dump
+        dump(self.to_dict(obj),
+             fp,
+             ensure_ascii=False,
+             indent=indent,
+             )
+
+    def load(self, fp, clazz) -> Any:
+        from json import load
+        dic: dict = load(fp)
+        if clazz is None:
+            return dic
+
+        obj: object = clazz()
+        obj.__dict__.update(dic)
+        return obj
+
+    @classmethod
+    def to_dict(cls, obj):
+        """将对象转换为字典"""
+        if hasattr(obj, "__dict__"):
+            d = dict(obj.__dict__)
+            for key, value in d.items():
+                if hasattr(value, "__dict__"):
+                    d[key] = cls.to_dict(value)
+            return d
+        elif isinstance(obj, list):
+            return [cls.to_dict(item) for item in obj]
+        else:
+            return obj
+
+
+class PicklePacker(AbstractSerializablePacker):
+    pack_mode = 'wb'
+    unpack_mode = 'rb'
+    encoding = None
+
+    def dump(self, fp, obj: object):
+        import pickle
+        pickle.dump(obj, fp)
+
+    def load(self, fp, clazz: Optional[Type]) -> Any:
+        import pickle
+        return pickle.load(fp)
+
+
+class PackerFactory:
+    mode_yml = 'yml'
+    mode_json = 'json'
+    mode_py_pickle = 'pickle'
+
+    mode_mapping: Dict[str, Union[Packer, Type[Packer]]] = {
+        mode_yml: YmlPacker,
+        mode_json: JsonPacker,
+        mode_py_pickle: PicklePacker,
+
+    }
+
+    @classmethod
+    def get_packer(cls, mode: str) -> Packer:
+        packer_caller = cls.mode_mapping.get(mode, None)
+
+        if packer_caller is None:
+            raise AssertionError(f"unknown mode: '{mode}', acceptable modes={list(cls.mode_mapping.keys())}")
+
+        packer: Packer
+        if isinstance(packer_caller, Packer):
+            packer_caller: Packer
+            packer = packer_caller
+        else:
+            packer_caller: Type[Packer]
+            packer = packer_caller()
+            # cache
+            cls.mode_mapping[mode] = packer
+
+        return packer
+
+
+class PackerUtil:
+
+    @staticmethod
+    def get_packer(filepath: str):
+        mode_intelligent = filepath[filepath.rfind('.') + 1::]
+        return PackerFactory.get_packer(mode=mode_intelligent)
+
+    @classmethod
+    def pack(cls, obj: object, filepath: str, packer=None, only_fields=False):
+        packer = packer or cls.get_packer(filepath)
+
+        # 只序列化类属性
+        if only_fields is True:
+            import inspect
+            obj = inspect.getmembers(obj, lambda f: not inspect.ismethod(f))
+            obj = dict(filter(lambda f: not f[0].startswith('_'), obj))
+
+        packer.pack(obj, filepath)
+
+    @classmethod
+    def unpack(cls, filepath: str, clazz=None, packer=None) -> Tuple[Any, Packer]:
+        packer = packer or cls.get_packer(filepath)
+        return packer.unpack(filepath, clazz), packer
```

### Comparing `commonX-0.5.1/common/ext/cookie_parser.py` & `commonX-0.5.2/common/ext/cookie_parser.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from common import Dict, Optional, Set
-
-
-class CookieParser:
-
-    def check_cookies_str_is_valid(self, cookies_str: str) -> bool:
-        raise NotImplementedError
-
-    def parse_to_cookies(self, cookies_str: str) -> dict:
-        raise NotImplementedError
-
-    def apply(self, cookies_str: str = None, when_valid_message=None) -> Optional[dict]:
-        if cookies_str is None:
-            from pyperclip import paste
-            cookies_str = paste()
-        if self.check_cookies_str_is_valid(cookies_str):
-            if when_valid_message is not None:
-                print(when_valid_message)
-
-            return self.parse_to_cookies(cookies_str)
-
-
-# suit for the chrome plugin: [cookie-editor]
-# the format of cookie data exported by this plugin is as follow :
-# [
-#     {
-#         "domain": ".bilibili.com",
-#         "expirationDate": 1693404645,
-#         "hostOnly": false,
-#         "httpOnly": false,
-#         "name": "buvid_fp_plain",
-#         "path": "/",
-#         "sameSite": null,
-#         "secure": false,
-#         "session": false,
-#         "storeId": null,
-#         "value": "undefined"
-#     },
-#     ...
-# ]
-
-class ChromePluginCookieParser(CookieParser):
-    default_required = {
-        "domain",
-        "hostOnly",
-        "httpOnly",
-        "name",
-        "path",
-        "sameSite",
-        "secure",
-        "session",
-        "storeId",
-        "value",
-    }
-
-    def __init__(self, required_word_for_cookies_str: Set[str] = None):
-        self.required_word = self.default_required.union(required_word_for_cookies_str or set())
-
-    def check_cookies_str_is_valid(self, cookies_str: str) -> bool:
-        if cookies_str == '':
-            return False
-        if not cookies_str.startswith('['):
-            return False
-
-        for word in self.required_word:
-            if word not in cookies_str:
-                return False
-
-        return True
-
-    def parse_to_cookies(self, cookies_str: str) -> Dict[str, str]:
-        from json import loads
-        dic: dict = loads(cookies_str)
-        return {cookie['name']: cookie['value'] for cookie in dic}
+from common import Dict, Optional, Set
+
+
+class CookieParser:
+
+    def check_cookies_str_is_valid(self, cookies_str: str) -> bool:
+        raise NotImplementedError
+
+    def parse_to_cookies(self, cookies_str: str) -> dict:
+        raise NotImplementedError
+
+    def apply(self, cookies_str: str = None, when_valid_message=None) -> Optional[dict]:
+        if cookies_str is None:
+            from pyperclip import paste
+            cookies_str = paste()
+        if self.check_cookies_str_is_valid(cookies_str):
+            if when_valid_message is not None:
+                print(when_valid_message)
+
+            return self.parse_to_cookies(cookies_str)
+
+
+# suit for the chrome plugin: [cookie-editor]
+# the format of cookie data exported by this plugin is as follow :
+# [
+#     {
+#         "domain": ".bilibili.com",
+#         "expirationDate": 1693404645,
+#         "hostOnly": false,
+#         "httpOnly": false,
+#         "name": "buvid_fp_plain",
+#         "path": "/",
+#         "sameSite": null,
+#         "secure": false,
+#         "session": false,
+#         "storeId": null,
+#         "value": "undefined"
+#     },
+#     ...
+# ]
+
+class ChromePluginCookieParser(CookieParser):
+    default_required = {
+        "domain",
+        "hostOnly",
+        "httpOnly",
+        "name",
+        "path",
+        "sameSite",
+        "secure",
+        "session",
+        "storeId",
+        "value",
+    }
+
+    def __init__(self, required_word_for_cookies_str: Set[str] = None):
+        self.required_word = self.default_required.union(required_word_for_cookies_str or set())
+
+    def check_cookies_str_is_valid(self, cookies_str: str) -> bool:
+        if cookies_str == '':
+            return False
+        if not cookies_str.startswith('['):
+            return False
+
+        for word in self.required_word:
+            if word not in cookies_str:
+                return False
+
+        return True
+
+    def parse_to_cookies(self, cookies_str: str) -> Dict[str, str]:
+        from json import loads
+        dic: dict = loads(cookies_str)
+        return {cookie['name']: cookie['value'] for cookie in dic}
```

### Comparing `commonX-0.5.1/common/postman/postman_api.py` & `commonX-0.5.2/common/postman/postman_api.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-from typing import Any, Callable
-
-
-class Postman:
-
-    def get(self,
-            url: str,
-            data: Any = None,
-            json: Any = None,
-            params: Any = None,
-            headers: Any = None,
-            cookies: Any = None,
-            files: Any = None,
-            auth: Any = None,
-            timeout: Any = None,
-            allow_redirects: bool = None,
-            proxies: Any = None,
-            hooks: Any = None,
-            stream: bool = None,
-            verify: Any = None,
-            cert: Any = None,
-            ):
-        raise NotImplementedError
-
-    def post(self,
-             url: str,
-             data: Any = None,
-             json: Any = None,
-             params: Any = None,
-             headers: Any = None,
-             cookies: Any = None,
-             files: Any = None,
-             auth: Any = None,
-             timeout: Any = None,
-             allow_redirects: bool = None,
-             proxies: Any = None,
-             hooks: Any = None,
-             stream: bool = None,
-             verify: Any = None,
-             cert: Any = None,
-             ):
-        raise NotImplementedError
-
-    def copy(self) -> 'Postman':
-        raise NotImplementedError
-
-    def get_meta_data(self, key=None, dv=None) -> dict:
-        """
-        获取Postman的元信息，调用示例：
-        # 1.
-        headers = postman.get_meta_data().get('headers', {})
-        # 2.
-        headers = postman.get_meta_data('headers', {})
-        # 3.
-        headers = postman['headers'] or {}
-
-        :param key: 键
-        :param dv: default-value，当键不存在时的默认值
-        """
-        raise NotImplementedError
-
-    def __getitem__(self, item):
-        return self.get_meta_data(item, None)
-
-    def __setitem__(self, key, value):
-        self.get_meta_data()[key] = value
-
-    @classmethod
-    def create(cls, clazz=None, **kwargs):
-        if clazz is None:
-            from .postman_impl import RequestsPostman
-            clazz = RequestsPostman
-
-        return clazz(kwargs)
-
-    def get_root_postman(self):
-        from .postman_proxy import PostmanProxy
-        if isinstance(self, PostmanProxy):
-            return self.postman.get_root_postman()
-        return self
-
-    # proxy method
-
-    def with_fix_url(self, url: str):
-        from .postman_proxy import FixUrlPostman
-        return FixUrlPostman(self, url)
-
-    def with_retry(self, retry_times, clazz=None):
-        if clazz is None:
-            from .postman_proxy import RetryPostman
-            clazz = RetryPostman
-
-        return clazz(self, retry_times)
-
-    def with_multi_part(self):
-        from .postman_proxy import MultiPartPostman
-        return MultiPartPostman(self)
-
-    def with_wrap_resp(self, clazz=None):
-        from .postman_proxy import WrapRespPostman
-        return WrapRespPostman(self, clazz)
-
-    def with_redirect_catching(self, clazz=None):
-        if clazz is None:
-            from .postman_proxy import RedirectPostman
-            clazz = RedirectPostman
-
-        return clazz(self)
-
-
-class AbstractPostman(Postman):
-
-    @classmethod
-    def create(cls, **kwargs):
-        return cls(kwargs)
-
-    def __init__(self, kwargs) -> None:
-        if not isinstance(kwargs, dict):
-            raise AssertionError('kwargs is not a dict')
-
-        self.meta_data: dict = kwargs
-
-    def get(self, url, **kwargs):
-        kwargs = self.before_request(kwargs)
-        return self.__get__()(url, **kwargs)
-
-    def post(self, url, **kwargs):
-        kwargs = self.before_request(kwargs)
-        return self.__post__()(url, **kwargs)
-
-    def __get__(self) -> Callable:
-        raise NotImplementedError
-
-    def __post__(self) -> Callable:
-        raise NotImplementedError
-
-    def before_request(self, kwargs):
-        return self.merge_kwargs(kwargs)
-
-    def merge_kwargs(self, kwargs):
-        """
-        把 kwargs 合并到 self.meta_data.copy()
-        """
-        ret = self.meta_data.copy()
-        for k, v in kwargs.items():
-            if v is None:
-                continue
-            ret[k] = v
-        return ret
-
-    def get_meta_data(self, key=None, dv=None) -> dict:
-        if key is None:
-            return self.meta_data
-        else:
-            return self.meta_data.get(key, dv)
-
-    def copy(self):
-        return self.__class__(self.meta_data.copy())
-
-
-class AbstractSessionPostman(AbstractPostman):
-
-    def __init__(self, kwargs: dict) -> None:
-        super().__init__(kwargs)
-
-        self.session = self.create_session(kwargs)
-
-    def create_session(self, kwargs):
-        raise NotImplementedError
-
-    def __get__(self):
-        return self.session.get
-
-    def __post__(self):
-        return self.session.post
-
-    def __getitem__(self, item):
-        return getattr(self.session, item)
-
-    def __setitem__(self, key, value):
-        setattr(self.session, key, value)
+from typing import Any, Callable
+
+
+class Postman:
+
+    def get(self,
+            url: str,
+            data: Any = None,
+            json: Any = None,
+            params: Any = None,
+            headers: Any = None,
+            cookies: Any = None,
+            files: Any = None,
+            auth: Any = None,
+            timeout: Any = None,
+            allow_redirects: bool = None,
+            proxies: Any = None,
+            hooks: Any = None,
+            stream: bool = None,
+            verify: Any = None,
+            cert: Any = None,
+            ):
+        raise NotImplementedError
+
+    def post(self,
+             url: str,
+             data: Any = None,
+             json: Any = None,
+             params: Any = None,
+             headers: Any = None,
+             cookies: Any = None,
+             files: Any = None,
+             auth: Any = None,
+             timeout: Any = None,
+             allow_redirects: bool = None,
+             proxies: Any = None,
+             hooks: Any = None,
+             stream: bool = None,
+             verify: Any = None,
+             cert: Any = None,
+             ):
+        raise NotImplementedError
+
+    def copy(self) -> 'Postman':
+        raise NotImplementedError
+
+    def get_meta_data(self, key=None, dv=None) -> dict:
+        """
+        获取Postman的元信息，调用示例：
+        # 1.
+        headers = postman.get_meta_data().get('headers', {})
+        # 2.
+        headers = postman.get_meta_data('headers', {})
+        # 3.
+        headers = postman['headers'] or {}
+
+        :param key: 键
+        :param dv: default-value，当键不存在时的默认值
+        """
+        raise NotImplementedError
+
+    def __getitem__(self, item):
+        return self.get_meta_data(item, None)
+
+    def __setitem__(self, key, value):
+        self.get_meta_data()[key] = value
+
+    @classmethod
+    def create(cls, clazz=None, **kwargs):
+        if clazz is None:
+            from .postman_impl import RequestsPostman
+            clazz = RequestsPostman
+
+        return clazz(kwargs)
+
+    def get_root_postman(self):
+        from .postman_proxy import PostmanProxy
+        if isinstance(self, PostmanProxy):
+            return self.postman.get_root_postman()
+        return self
+
+    # proxy method
+
+    def with_fix_url(self, url: str):
+        from .postman_proxy import FixUrlPostman
+        return FixUrlPostman(self, url)
+
+    def with_retry(self, retry_times, clazz=None):
+        if clazz is None:
+            from .postman_proxy import RetryPostman
+            clazz = RetryPostman
+
+        return clazz(self, retry_times)
+
+    def with_multi_part(self):
+        from .postman_proxy import MultiPartPostman
+        return MultiPartPostman(self)
+
+    def with_wrap_resp(self, clazz=None):
+        from .postman_proxy import WrapRespPostman
+        return WrapRespPostman(self, clazz)
+
+    def with_redirect_catching(self, clazz=None):
+        if clazz is None:
+            from .postman_proxy import RedirectPostman
+            clazz = RedirectPostman
+
+        return clazz(self)
+
+
+class AbstractPostman(Postman):
+
+    @classmethod
+    def create(cls, **kwargs):
+        return cls(kwargs)
+
+    def __init__(self, kwargs) -> None:
+        if not isinstance(kwargs, dict):
+            raise AssertionError('kwargs is not a dict')
+
+        self.meta_data: dict = kwargs
+
+    def get(self, url, **kwargs):
+        kwargs = self.before_request(kwargs)
+        return self.__get__()(url, **kwargs)
+
+    def post(self, url, **kwargs):
+        kwargs = self.before_request(kwargs)
+        return self.__post__()(url, **kwargs)
+
+    def __get__(self) -> Callable:
+        raise NotImplementedError
+
+    def __post__(self) -> Callable:
+        raise NotImplementedError
+
+    def before_request(self, kwargs):
+        return self.merge_kwargs(kwargs)
+
+    def merge_kwargs(self, kwargs):
+        """
+        把 kwargs 合并到 self.meta_data.copy()
+        """
+        ret = self.meta_data.copy()
+        for k, v in kwargs.items():
+            if v is None:
+                continue
+            ret[k] = v
+        return ret
+
+    def get_meta_data(self, key=None, dv=None) -> dict:
+        if key is None:
+            return self.meta_data
+        else:
+            return self.meta_data.get(key, dv)
+
+    def copy(self):
+        return self.__class__(self.meta_data.copy())
+
+
+class AbstractSessionPostman(AbstractPostman):
+
+    def __init__(self, kwargs: dict) -> None:
+        super().__init__(kwargs)
+
+        self.session = self.create_session(kwargs)
+
+    def create_session(self, kwargs):
+        raise NotImplementedError
+
+    def __get__(self):
+        return self.session.get
+
+    def __post__(self):
+        return self.session.post
+
+    def __getitem__(self, item):
+        return getattr(self.session, item)
+
+    def __setitem__(self, key, value):
+        setattr(self.session, key, value)
```

### Comparing `commonX-0.5.1/common/postman/postman_proxy.py` & `commonX-0.5.2/common/postman/postman_proxy.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-from .postman_api import *
-
-
-class PostmanProxy(Postman):
-
-    def __init__(self, postman: Postman):
-        self.postman = postman
-
-    def get(self, *args, **kwargs):
-        return self.postman.get(*args, **kwargs)
-
-    def post(self, *args, **kwargs):
-        return self.postman.post(*args, **kwargs)
-
-    def get_meta_data(self, key=None, dv=None) -> dict:
-        return self.postman.get_meta_data(key, dv)
-
-    def __getitem__(self, item):
-        return self.postman.__getitem__(item)
-
-    def __setitem__(self, key, value):
-        self.postman.__setitem__(key, value)
-
-    def copy(self):
-        return self.__class__(self.postman.copy())
-
-    def get_root_postman(self):
-        return self.postman.get_root_postman()
-
-
-class FixUrlPostman(PostmanProxy):
-
-    def __init__(self,
-                 postman: Postman,
-                 fix_url: str,
-                 ):
-        super().__init__(postman)
-        self.fix_url = fix_url
-
-    def get(self, url=None, **kwargs):
-        return super().get(url or self.fix_url, **kwargs)
-
-    def post(self, url=None, **kwargs):
-        return super().post(url or self.fix_url, **kwargs)
-
-    def copy(self):
-        return self.__class__(self.postman.copy(), self.fix_url)
-
-
-class RetryPostman(PostmanProxy):
-
-    def __init__(self,
-                 postman: Postman,
-                 retry_times: int,
-                 ):
-        super().__init__(postman)
-        self.retry_times = retry_times
-
-    def retry_request(self, request, url, **kwargs):
-        retry_times = self.retry_times
-        if retry_times <= 0:
-            return request(url, **kwargs)
-
-        for i in range(retry_times):
-            try:
-                return request(url, **kwargs)
-            except KeyboardInterrupt as e:
-                raise e
-            except Exception as e:
-                self.excp_handle(e)
-                self.tip_retrying(i, request, url, kwargs)
-
-        return self.fallback(url, kwargs)
-
-    def get(self, *args, **kwargs):
-        return self.retry_request(self.postman.get, *args, **kwargs)
-
-    def post(self, *args, **kwargs):
-        return self.retry_request(self.postman.post, *args, **kwargs)
-
-    def fallback(self, url, kwargs):
-        raise RuntimeError(f"请求失败，重试了{self.retry_times}次后依然失败: {url}，携带参数: {kwargs}")
-
-    # noinspection PyMethodMayBeStatic,PyUnusedLocal
-    def excp_handle(self, e):
-        from common import traceback_print_exec
-        traceback_print_exec()
-
-    def tip_retrying(self, time, _request, url, kwargs):
-        pass
-
-
-class MultiPartPostman(PostmanProxy):
-
-    def build_headers(self, data, kwargs):
-        headers = kwargs.get('headers', None)
-        if headers is None:
-            headers = self.get_meta_data().get('headers', {})
-        headers['Content-Type'] = data.content_type
-        return headers
-
-    def post(self, *args, **kwargs):
-        data = kwargs.get('data', None)
-        from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
-        if isinstance(data, (MultipartEncoder, MultipartEncoderMonitor)):
-            kwargs['headers'] = self.build_headers(data, kwargs)
-        return super().post(*args, **kwargs)
-
-
-class WrapRespPostman(PostmanProxy):
-
-    def __init__(self, postman: Postman, wrap_resp_class=None):
-        super().__init__(postman)
-        if wrap_resp_class is None:
-            from common import CommonResp
-            wrap_resp_class = CommonResp
-        self.WrapResp = wrap_resp_class
-
-    def get(self, *args, **kwargs):
-        return self.WrapResp(super().get(*args, **kwargs))
-
-    def post(self, *args, **kwargs):
-        return self.WrapResp(super().post(*args, **kwargs))
-
-
-# noinspection PyMethodMayBeStatic
-class RedirectPostman(PostmanProxy):
-
-    def request(self, url, kwargs, method):
-        kwargs.setdefault("allow_redirects", False)
-
-        while True:
-            resp = method(url, **kwargs)
-            status_code = resp.status_code
-
-            if status_code == 301:
-                # 永久移除
-                url = self.get_redirect_url_from_resp(resp)
-                continue
-            if status_code == 302:
-                # 暂时重定向
-                break
-            else:
-                raise NotImplementedError(f"status_code = {status_code}")
-
-        return self.get_redirect_url_from_resp(resp)
-
-    def get_redirect_url_from_resp(self, resp):
-        return resp.headers['Location']
-
-    def get(self, url, **kwargs):
-        return self.request(url, kwargs, super().get)
-
-    def post(self, url, **kwargs):
-        return self.request(url, kwargs, super().post)
+from .postman_api import *
+
+
+class PostmanProxy(Postman):
+
+    def __init__(self, postman: Postman):
+        self.postman = postman
+
+    def get(self, *args, **kwargs):
+        return self.postman.get(*args, **kwargs)
+
+    def post(self, *args, **kwargs):
+        return self.postman.post(*args, **kwargs)
+
+    def get_meta_data(self, key=None, dv=None) -> dict:
+        return self.postman.get_meta_data(key, dv)
+
+    def __getitem__(self, item):
+        return self.postman.__getitem__(item)
+
+    def __setitem__(self, key, value):
+        self.postman.__setitem__(key, value)
+
+    def copy(self):
+        return self.__class__(self.postman.copy())
+
+    def get_root_postman(self):
+        return self.postman.get_root_postman()
+
+
+class FixUrlPostman(PostmanProxy):
+
+    def __init__(self,
+                 postman: Postman,
+                 fix_url: str,
+                 ):
+        super().__init__(postman)
+        self.fix_url = fix_url
+
+    def get(self, url=None, **kwargs):
+        return super().get(url or self.fix_url, **kwargs)
+
+    def post(self, url=None, **kwargs):
+        return super().post(url or self.fix_url, **kwargs)
+
+    def copy(self):
+        return self.__class__(self.postman.copy(), self.fix_url)
+
+
+class RetryPostman(PostmanProxy):
+
+    def __init__(self,
+                 postman: Postman,
+                 retry_times: int,
+                 ):
+        super().__init__(postman)
+        self.retry_times = retry_times
+
+    def retry_request(self, request, url, **kwargs):
+        retry_times = self.retry_times
+        if retry_times <= 0:
+            return request(url, **kwargs)
+
+        for i in range(retry_times):
+            try:
+                return request(url, **kwargs)
+            except KeyboardInterrupt as e:
+                raise e
+            except Exception as e:
+                self.excp_handle(e)
+                self.tip_retrying(i, request, url, kwargs)
+
+        return self.fallback(url, kwargs)
+
+    def get(self, *args, **kwargs):
+        return self.retry_request(self.postman.get, *args, **kwargs)
+
+    def post(self, *args, **kwargs):
+        return self.retry_request(self.postman.post, *args, **kwargs)
+
+    def fallback(self, url, kwargs):
+        raise RuntimeError(f"请求失败，重试了{self.retry_times}次后依然失败: {url}，携带参数: {kwargs}")
+
+    # noinspection PyMethodMayBeStatic,PyUnusedLocal
+    def excp_handle(self, e):
+        from common import traceback_print_exec
+        traceback_print_exec()
+
+    def tip_retrying(self, time, _request, url, kwargs):
+        pass
+
+
+class MultiPartPostman(PostmanProxy):
+
+    def build_headers(self, data, kwargs):
+        headers = kwargs.get('headers', None)
+        if headers is None:
+            headers = self.get_meta_data().get('headers', {})
+        headers['Content-Type'] = data.content_type
+        return headers
+
+    def post(self, *args, **kwargs):
+        data = kwargs.get('data', None)
+        from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
+        if isinstance(data, (MultipartEncoder, MultipartEncoderMonitor)):
+            kwargs['headers'] = self.build_headers(data, kwargs)
+        return super().post(*args, **kwargs)
+
+
+class WrapRespPostman(PostmanProxy):
+
+    def __init__(self, postman: Postman, wrap_resp_class=None):
+        super().__init__(postman)
+        if wrap_resp_class is None:
+            from common import CommonResp
+            wrap_resp_class = CommonResp
+        self.WrapResp = wrap_resp_class
+
+    def get(self, *args, **kwargs):
+        return self.WrapResp(super().get(*args, **kwargs))
+
+    def post(self, *args, **kwargs):
+        return self.WrapResp(super().post(*args, **kwargs))
+
+
+# noinspection PyMethodMayBeStatic
+class RedirectPostman(PostmanProxy):
+
+    def request(self, url, kwargs, method):
+        kwargs.setdefault("allow_redirects", False)
+
+        while True:
+            resp = method(url, **kwargs)
+            status_code = resp.status_code
+
+            if status_code == 301:
+                # 永久移除
+                url = self.get_redirect_url_from_resp(resp)
+                continue
+            if status_code == 302:
+                # 暂时重定向
+                break
+            else:
+                raise NotImplementedError(f"status_code = {status_code}")
+
+        return self.get_redirect_url_from_resp(resp)
+
+    def get_redirect_url_from_resp(self, resp):
+        return resp.headers['Location']
+
+    def get(self, url, **kwargs):
+        return self.request(url, kwargs, super().get)
+
+    def post(self, url, **kwargs):
+        return self.request(url, kwargs, super().post)
```

### Comparing `commonX-0.5.1/common/util/assert_util.py` & `commonX-0.5.2/common/util/assert_util.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from .typing_util import *
-from .args_util import process_args_kwargs
-
-
-class Asserter:
-    Ret = Union[bool, Any]
-
-    @staticmethod
-    def assert_equal(raw: Any,
-                     correct: Any,
-                     ret_when_false=None,
-                     callback_when_true=None,
-                     args=None,
-                     kwargs=None
-                     ) -> Ret:
-        is_success = raw == correct
-        return_value = True if is_success else \
-            (raw if ret_when_false is None else ret_when_false)
-
-        if callback_when_true is not None and \
-                return_value is True:
-            Asserter.call_func(callback_when_true, args, kwargs)
-
-        return return_value
-
-    @staticmethod
-    def any_match(raw,
-                  accepted: list,
-                  ret_when_false=None,
-                  callback_when_true=None,
-                  args=None,
-                  kwargs=None
-                  ) -> Ret:
-        is_success = any(each in raw for each in accepted)
-        return_value = True if is_success else \
-            (False if ret_when_false is None else ret_when_false)
-
-        if callback_when_true is not None and \
-                return_value is True:
-            Asserter.call_func(callback_when_true, args, kwargs)
-
-        return return_value
-
-    @staticmethod
-    def require_not_empty(obj):
-        if obj is None or len(obj) == 0:
-            raise AssertionError('参数为空')
-
-    @staticmethod
-    def call_func(func, args, kwargs):
-        args, kwargs = process_args_kwargs(args, kwargs)
-        func(*args, **kwargs)
-
-    @staticmethod
-    def pattern_search(p: Pattern,
-                       text: str,
-                       index=0,
-                       no_match_msg='无法匹配',
-                       ):
-        match = p.search(text)
-        if match is None:
-            raise AssertionError(no_match_msg)
-        else:
-            return match[index]
-
-
-any_match = Asserter.any_match
-assert_equal = Asserter.assert_equal
-require_not_empty = Asserter.require_not_empty
-pattern_search = Asserter.pattern_search
+from .typing_util import *
+from .args_util import process_args_kwargs
+
+
+class Asserter:
+    Ret = Union[bool, Any]
+
+    @staticmethod
+    def assert_equal(raw: Any,
+                     correct: Any,
+                     ret_when_false=None,
+                     callback_when_true=None,
+                     args=None,
+                     kwargs=None
+                     ) -> Ret:
+        is_success = raw == correct
+        return_value = True if is_success else \
+            (raw if ret_when_false is None else ret_when_false)
+
+        if callback_when_true is not None and \
+                return_value is True:
+            Asserter.call_func(callback_when_true, args, kwargs)
+
+        return return_value
+
+    @staticmethod
+    def any_match(raw,
+                  accepted: list,
+                  ret_when_false=None,
+                  callback_when_true=None,
+                  args=None,
+                  kwargs=None
+                  ) -> Ret:
+        is_success = any(each in raw for each in accepted)
+        return_value = True if is_success else \
+            (False if ret_when_false is None else ret_when_false)
+
+        if callback_when_true is not None and \
+                return_value is True:
+            Asserter.call_func(callback_when_true, args, kwargs)
+
+        return return_value
+
+    @staticmethod
+    def require_not_empty(obj):
+        if obj is None or len(obj) == 0:
+            raise AssertionError('参数为空')
+
+    @staticmethod
+    def call_func(func, args, kwargs):
+        args, kwargs = process_args_kwargs(args, kwargs)
+        func(*args, **kwargs)
+
+    @staticmethod
+    def pattern_search(p: Pattern,
+                       text: str,
+                       index=0,
+                       no_match_msg='无法匹配',
+                       ):
+        match = p.search(text)
+        if match is None:
+            raise AssertionError(no_match_msg)
+        else:
+            return match[index]
+
+
+any_match = Asserter.any_match
+assert_equal = Asserter.assert_equal
+require_not_empty = Asserter.require_not_empty
+pattern_search = Asserter.pattern_search
```

### Comparing `commonX-0.5.1/common/util/exception_utll.py` & `commonX-0.5.2/common/util/exception_utll.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import sys
-import threading
-import traceback
-from typing import List, Tuple, Type
-import types
-
-ExceptHookArgs = Tuple[Type[BaseException], BaseException, types.TracebackType]
-
-
-def print_exception(except_info: ExceptHookArgs):
-    """
-    打印所有未捕获异常
-    """
-    if len(except_info) == 0:
-        return
-
-    print(except_info)
-    print(len(except_info))
-    print(f"Unhandled exception: {except_info[0]} - {except_info[1]}")
-    print(*traceback.format_exception(*except_info), sep='')
-
-
-class UncaughtExceptionHandler:
-
-    def __init__(self):
-        self.uncaught_exceptions: List[ExceptHookArgs] = []
-        self.handle_exception_func = print_exception  # 默认的处理方式是打印
-
-    @property
-    def except_count(self):
-        """
-        for tests
-        """
-        return len(self.uncaught_exceptions)
-
-    # noinspection PyUnresolvedReferences, PyAttributeOutsideInit, PyProtectedMember
-    def register(self, at_exit=True):
-        # 注册全局的sys.excepthook
-        sys.excepthook = self.hook_uncaught_exception
-
-        if sys.version_info >= (3, 8):
-            threading.excepthook = self.hook_uncaught_exception
-        else:
-            import warnings
-            warnings.warn('python version <= 3.7 may not work')
-            self.threading_org_hook = threading._format_exc
-            threading._format_exc = self.hook_uncaught_exception
-
-        if at_exit is True:
-            # 自动在程序退出时，处理所有未捕获异常
-            import atexit
-            atexit.unregister(self.handle_all_exception)
-            atexit.register(self.handle_all_exception)
-
-    def handle_all_exception(self):
-        """
-        处理所有未捕获异常
-        """
-        func = self.handle_exception_func
-        for except_info in self.uncaught_exceptions:
-            func(except_info)
-
-    def hook_uncaught_exception(self, except_info):
-        """
-        将未捕获异常添加到列表中
-        """
-        # noinspection PyTypeChecker
-        print(except_info, len(except_info))
-        self.uncaught_exceptions.append(except_info)
-
-        if sys.version_info < (3, 8):
-            return self.threading_org_hook()
-
-
-def global_caught(at_exit=True, except_handler=None):
-    uncaught_exception_handler = UncaughtExceptionHandler()
-
-    if except_handler is not None:
-        uncaught_exception_handler.handle_exception_func = uncaught_exception_handler
-
-    def decorator(func):
-        uncaught_exception_handler.register(at_exit)
-
-        def wrapper(*args, **kwargs):
-            return func(*args, **kwargs)
-
-        return wrapper
-
-    return decorator
+import sys
+import threading
+import traceback
+from typing import List, Tuple, Type
+import types
+
+ExceptHookArgs = Tuple[Type[BaseException], BaseException, types.TracebackType]
+
+
+def print_exception(except_info: ExceptHookArgs):
+    """
+    打印所有未捕获异常
+    """
+    if len(except_info) == 0:
+        return
+
+    print(except_info)
+    print(len(except_info))
+    print(f"Unhandled exception: {except_info[0]} - {except_info[1]}")
+    print(*traceback.format_exception(*except_info), sep='')
+
+
+class UncaughtExceptionHandler:
+
+    def __init__(self):
+        self.uncaught_exceptions: List[ExceptHookArgs] = []
+        self.handle_exception_func = print_exception  # 默认的处理方式是打印
+
+    @property
+    def except_count(self):
+        """
+        for tests
+        """
+        return len(self.uncaught_exceptions)
+
+    # noinspection PyUnresolvedReferences, PyAttributeOutsideInit, PyProtectedMember
+    def register(self, at_exit=True):
+        # 注册全局的sys.excepthook
+        sys.excepthook = self.hook_uncaught_exception
+
+        if sys.version_info >= (3, 8):
+            threading.excepthook = self.hook_uncaught_exception
+        else:
+            import warnings
+            warnings.warn('python version <= 3.7 may not work')
+            self.threading_org_hook = threading._format_exc
+            threading._format_exc = self.hook_uncaught_exception
+
+        if at_exit is True:
+            # 自动在程序退出时，处理所有未捕获异常
+            import atexit
+            atexit.unregister(self.handle_all_exception)
+            atexit.register(self.handle_all_exception)
+
+    def handle_all_exception(self):
+        """
+        处理所有未捕获异常
+        """
+        func = self.handle_exception_func
+        for except_info in self.uncaught_exceptions:
+            func(except_info)
+
+    def hook_uncaught_exception(self, except_info):
+        """
+        将未捕获异常添加到列表中
+        """
+        # noinspection PyTypeChecker
+        print(except_info, len(except_info))
+        self.uncaught_exceptions.append(except_info)
+
+        if sys.version_info < (3, 8):
+            return self.threading_org_hook()
+
+
+def global_caught(at_exit=True, except_handler=None):
+    uncaught_exception_handler = UncaughtExceptionHandler()
+
+    if except_handler is not None:
+        uncaught_exception_handler.handle_exception_func = uncaught_exception_handler
+
+    def decorator(func):
+        uncaught_exception_handler.register(at_exit)
+
+        def wrapper(*args, **kwargs):
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
```

### Comparing `commonX-0.5.1/common/util/image_util.py` & `commonX-0.5.2/common/util/image_util.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import os
-
-from PIL import Image
-
-
-def merge_images(folder_path, limit=None, delete_org_file=True, suffix='.webp'):
-    # 获取文件夹名称
-    folder_name = os.path.basename(folder_path)
-
-    # 获取所有webp图片路径
-
-    webp_files = [f for f in os.listdir(folder_path) if f.endswith(suffix)]
-
-    # 如果没有webp图片则报错
-    if not webp_files:
-        raise ValueError(f'文件夹中没有{suffix}图片')
-
-    # 根据limit参数拆分webp_files列表
-    if limit:
-        webp_list = [webp_files[i:i + limit]
-                     for i in range(0, len(webp_files), limit)]
-    else:
-        webp_list = [webp_files]
-
-    # 打印图片数量、总长度和总宽度
-    num_images = len(webp_files)
-    total_width = 0
-    total_height = 0
-    for file_name in webp_files:
-        img_path = os.path.join(folder_path, file_name)
-        with Image.open(img_path) as im:
-            total_width = max(total_width, im.width)
-            total_height += im.height
-    print(f'共有{num_images}张图片，总长度为{total_width}，总高度为{total_height}')
-
-    # 拼接图片并保存
-    for i, webp_group in enumerate(webp_list):
-        images = []
-        for file_name in webp_group:
-            img_path = os.path.join(folder_path, file_name)
-            with Image.open(img_path) as im:
-                images.append(im)
-
-        # 对所有图片进行纵向拼接
-        result = Image.new('RGB', (images[0].width, sum(
-            img.height for img in images)), (255, 255, 255))
-        y_offset = 0
-        for img in images:
-            result.paste(img, (0, y_offset))
-            y_offset += img.size[1]
-
-        # 保存结果图片
-        if len(webp_list) > 1:
-            img_name = f'{folder_name}_{i + 1}{suffix}'
-        else:
-            img_name = f'{folder_name}{suffix}'
-
-        save_path = os.path.join(folder_path, img_name)
-        result.save(save_path)
-        print(f'保存: {save_path}')
-
-    if delete_org_file is True:
-        for f in webp_files:
-            os.remove(os.path.join(folder_path, f))
-
-
-def convert_images_to_jpg(folder_path, delete_org_file=True):
-    for root, dirs, files in os.walk(folder_path):
-        for filename in files:
-            # 检查文件扩展名是否为图片格式
-            if filename.lower().endswith(('.png', '.bmp', '.gif', '.jpeg', '.ppm', '.tiff', 'webp')):
-                file_path = os.path.join(root, filename)
-                # 打开图片并转换为JPG格式
-                with Image.open(file_path) as img:
-                    new_file_path = os.path.splitext(file_path)[0] + '.jpg'
-                    img.convert('RGB').save(new_file_path)
-
-                if delete_org_file is True:
-                    # 删除原始文件
-                    os.remove(file_path)
-                print(f'{file_path} → {new_file_path}')
+import os
+
+from PIL import Image
+
+
+def merge_images(folder_path, limit=None, delete_org_file=True, suffix='.webp'):
+    # 获取文件夹名称
+    folder_name = os.path.basename(folder_path)
+
+    # 获取所有webp图片路径
+
+    webp_files = [f for f in os.listdir(folder_path) if f.endswith(suffix)]
+
+    # 如果没有webp图片则报错
+    if not webp_files:
+        raise ValueError(f'文件夹中没有{suffix}图片')
+
+    # 根据limit参数拆分webp_files列表
+    if limit:
+        webp_list = [webp_files[i:i + limit]
+                     for i in range(0, len(webp_files), limit)]
+    else:
+        webp_list = [webp_files]
+
+    # 打印图片数量、总长度和总宽度
+    num_images = len(webp_files)
+    total_width = 0
+    total_height = 0
+    for file_name in webp_files:
+        img_path = os.path.join(folder_path, file_name)
+        with Image.open(img_path) as im:
+            total_width = max(total_width, im.width)
+            total_height += im.height
+    print(f'共有{num_images}张图片，总长度为{total_width}，总高度为{total_height}')
+
+    # 拼接图片并保存
+    for i, webp_group in enumerate(webp_list):
+        images = []
+        for file_name in webp_group:
+            img_path = os.path.join(folder_path, file_name)
+            with Image.open(img_path) as im:
+                images.append(im)
+
+        # 对所有图片进行纵向拼接
+        result = Image.new('RGB', (images[0].width, sum(
+            img.height for img in images)), (255, 255, 255))
+        y_offset = 0
+        for img in images:
+            result.paste(img, (0, y_offset))
+            y_offset += img.size[1]
+
+        # 保存结果图片
+        if len(webp_list) > 1:
+            img_name = f'{folder_name}_{i + 1}{suffix}'
+        else:
+            img_name = f'{folder_name}{suffix}'
+
+        save_path = os.path.join(folder_path, img_name)
+        result.save(save_path)
+        print(f'保存: {save_path}')
+
+    if delete_org_file is True:
+        for f in webp_files:
+            os.remove(os.path.join(folder_path, f))
+
+
+def convert_images_to_jpg(folder_path, delete_org_file=True):
+    for root, dirs, files in os.walk(folder_path):
+        for filename in files:
+            # 检查文件扩展名是否为图片格式
+            if filename.lower().endswith(('.png', '.bmp', '.gif', '.jpeg', '.ppm', '.tiff', 'webp')):
+                file_path = os.path.join(root, filename)
+                # 打开图片并转换为JPG格式
+                with Image.open(file_path) as img:
+                    new_file_path = os.path.splitext(file_path)[0] + '.jpg'
+                    img.convert('RGB').save(new_file_path)
+
+                if delete_org_file is True:
+                    # 删除原始文件
+                    os.remove(file_path)
+                print(f'{file_path} → {new_file_path}')
```

### Comparing `commonX-0.5.1/common/util/json_util.py` & `commonX-0.5.2/common/util/json_util.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-from json import load, loads, dump, dumps
-
-from .typing_util import *
-
-json_loads = loads
-json_load = load
-
-json_dumps = dumps
-json_dump = dump
-
-
-class DictModel:
-
-    def __init__(self, data: dict):
-        if data is None:
-            raise AssertionError(f"data is None")
-
-        self._data = data
-
-    def __getattr__(self, item):
-        v = self._data[item]
-        if isinstance(v, (list, tuple)):
-            v = [self.__class__(e) if isinstance(e, dict) else e for e in v]
-        elif isinstance(v, dict):
-            v = self.__class__(v)
-
-        setattr(self, item, v)
-        return v
-
-    def __getitem__(self, item):
-        return self._data[item]
-
-    def __contains__(self, item):
-        return item in self._data
-
-    @property
-    def src_dict(self):
-        return self._data
-
-    def get(self, *args, **kwargs):
-        return self._data.get(*args, **kwargs)
-
-
-def dict_2_obj(data: dict):
-    return DictModel(data)
-
-
-def json_loadf(filepath,
-               encoding='utf-8',
-               decode_unicode=False,
-               ):
-    from .file_util import file_not_exists
-    if file_not_exists(filepath):
-        raise AssertionError(f"不存在的json文件路径：{filepath}")
-
-    with open(filepath, 'r', encoding=encoding) as f:
-        if decode_unicode is False:
-            return json_load(f)
-        else:
-            from .sys_util import parse_unicode_escape_text
-            return json_loads(parse_unicode_escape_text(f.read()))
-
-
-def json_dumpf(obj, fp, encoding='utf-8', indent=2):
-    with open(fp, 'w', encoding=encoding) as f:
-        json_dump(obj, f, indent=indent)
-
-
-def accpet_json(fp, accept_v: Callable[[Any], None] = None, accpet_k: Callable[[str], None] = None):
-    def __accept_json_keys_values(data):
-        if isinstance(data, list):
-            for each in data:
-                __accept_json_keys_values(each)
-
-        elif isinstance(data, dict):
-            for k, v in data.items():
-                if accpet_k is not None:
-                    accpet_k(k)
-                __accept_json_keys_values(v)
-        else:
-            if accept_v is not None:
-                accept_v(data)
-
-    data = json_load(fp)
-
-    if accpet_k is not None or accept_v is not None:
-        __accept_json_keys_values(data)
-
-    return data
-
-
-def keys_of_json(data) -> Generator:
-    if isinstance(data, list):
-        for each in data:
-            keys_of_json(each)
-
-    elif isinstance(data, dict):
-        for k, v in data.items():
-            yield k
-            keys_of_json(v)
-
-
-def values_of_json(data) -> Generator:
-    if isinstance(data, list):
-        for each in data:
-            yield from values_of_json(each)
-
-    elif isinstance(data, dict):
-        for v in data.values():
-            yield from values_of_json(v)
-
-    else:
-        yield data
+from json import load, loads, dump, dumps
+
+from .typing_util import *
+
+json_loads = loads
+json_load = load
+
+json_dumps = dumps
+json_dump = dump
+
+
+class DictModel:
+
+    def __init__(self, data: dict):
+        if data is None:
+            raise AssertionError(f"data is None")
+
+        self._data = data
+
+    def __getattr__(self, item):
+        v = self._data[item]
+        if isinstance(v, (list, tuple)):
+            v = [self.__class__(e) if isinstance(e, dict) else e for e in v]
+        elif isinstance(v, dict):
+            v = self.__class__(v)
+
+        setattr(self, item, v)
+        return v
+
+    def __getitem__(self, item):
+        return self._data[item]
+
+    def __contains__(self, item):
+        return item in self._data
+
+    @property
+    def src_dict(self):
+        return self._data
+
+    def get(self, *args, **kwargs):
+        return self._data.get(*args, **kwargs)
+
+
+def dict_2_obj(data: dict):
+    return DictModel(data)
+
+
+def json_loadf(filepath,
+               encoding='utf-8',
+               decode_unicode=False,
+               ):
+    from .file_util import file_not_exists
+    if file_not_exists(filepath):
+        raise AssertionError(f"不存在的json文件路径：{filepath}")
+
+    with open(filepath, 'r', encoding=encoding) as f:
+        if decode_unicode is False:
+            return json_load(f)
+        else:
+            from .sys_util import parse_unicode_escape_text
+            return json_loads(parse_unicode_escape_text(f.read()))
+
+
+def json_dumpf(obj, fp, encoding='utf-8', indent=2):
+    with open(fp, 'w', encoding=encoding) as f:
+        json_dump(obj, f, indent=indent)
+
+
+def accpet_json(fp, accept_v: Callable[[Any], None] = None, accpet_k: Callable[[str], None] = None):
+    def __accept_json_keys_values(data):
+        if isinstance(data, list):
+            for each in data:
+                __accept_json_keys_values(each)
+
+        elif isinstance(data, dict):
+            for k, v in data.items():
+                if accpet_k is not None:
+                    accpet_k(k)
+                __accept_json_keys_values(v)
+        else:
+            if accept_v is not None:
+                accept_v(data)
+
+    data = json_load(fp)
+
+    if accpet_k is not None or accept_v is not None:
+        __accept_json_keys_values(data)
+
+    return data
+
+
+def keys_of_json(data) -> Generator:
+    if isinstance(data, list):
+        for each in data:
+            keys_of_json(each)
+
+    elif isinstance(data, dict):
+        for k, v in data.items():
+            yield k
+            keys_of_json(v)
+
+
+def values_of_json(data) -> Generator:
+    if isinstance(data, list):
+        for each in data:
+            yield from values_of_json(each)
+
+    elif isinstance(data, dict):
+        for v in data.values():
+            yield from values_of_json(v)
+
+    else:
+        yield data
```

### Comparing `commonX-0.5.1/common/util/requests_util.py` & `commonX-0.5.2/common/util/requests_util.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-from .typing_util import *
-from .json_util import DictModel
-
-
-class ProxyBuilder:
-    proxy_protocols = ['https', 'http']
-    addr_f = '{}:{}'
-
-    @classmethod
-    def build_proxy(cls, address):
-        proxies = {protocol: address for protocol in cls.proxy_protocols}
-        return proxies
-
-    @classmethod
-    def clash_proxy(cls, ip='127.0.0.1', port='7890'):
-        return cls.build_proxy(cls.addr_f.format(ip, port))
-
-    @classmethod
-    def v2ray_proxy(cls, ip='127.0.0.1', port='10809'):
-        return cls.build_proxy(cls.addr_f.format(ip, port))
-
-    @classmethod
-    def build_by_str(cls, text):
-        """
-        :param text: 127.0.0.1:1234 / clash / v2ray
-        """
-        proxy = getattr(cls, text + '_proxy', None)
-        if proxy is None:
-            # 127.0.0.1:1234
-            return cls.build_proxy(text)
-        else:
-            # clash_proxy
-            return proxy()
-
-    v2Ray_proxy = v2ray_proxy
-
-
-def save_resp_content(resp, filepath: str):
-    from .file_util import of_dir_path
-    of_dir_path(filepath, mkdir=True)
-    with open(filepath, 'wb') as f:
-        f.write(resp.content)
-
-
-def set_global_proxy(status='off'):
-    """
-    全局性的关闭或者启用系统代理。
-    测试时发现，如果设置了系统代理，在访问 https 网站时发生错误 requests.exceptions.ProxyError
-    原因是 SSL: self._sslobj.do_handshake() -> OSError: [Errno 0] Error
-    进一步，是因为 urllib3 1.26.0 以上版本支持 https协议，但是代理软件不支持，导致连接错误。
-    所以使用 { 'https': 'http://127.0.0.1:1080' }，http的协议访问 https 的网址（本地通信），即可解决。
-    或者在 requests.get 函数中增加 proxies={'https': None} 参数来解决，但每次访问都需加这个参数，太麻烦，
-    此处通过修改 requests 库中的 get_environ_proxies 函数的方法来全局性地关闭系统代理，或者仅关闭 https 的代理。
-
-    注意：仅影响本 Python程序的 requests包，不影响其他 Python程序，
-    不影响 Windows系统的代理设置，也不影响浏览器的代理设置。
-
-    :param status: status - 'off', 关闭系统代理；'on', 打开系统代理；'toggle', 切换关闭或者打开状态；
-    """
-    from requests import sessions, utils
-    init_func = sessions.get_environ_proxies
-    if status == 'off':
-        # 关闭系统代理
-        if init_func.__name__ == '<lambda>':
-            # 已经替换了原始函数，即已经是关闭状态，无需设置
-            return
-        # 修改函数，也可以是 lambda *x, **y: {'https': None}
-        sessions.get_environ_proxies = lambda *x, **y: {}
-    elif status == 'on':
-        # 打开系统代理，如果设置了代理的话
-        # 对高版本的 urllib3(>1.26.0) 打补丁，修正 https代理 BUG: OSError: [Errno 0] Error
-        # noinspection PyUnresolvedReferences
-        proxies = utils.getproxies()
-        if 'https' in proxies:
-            proxies['https'] = proxies.get('http')  # None 或者 'http://127.0.0.1:1080'
-        sessions.get_environ_proxies = lambda *x, **y: proxies
-        sessions.get_environ_proxies.__name__ = 'get_environ_proxies'
-    else:
-        # 切换开关状态
-        if init_func.__name__ == '<lambda>':
-            # 已经是关闭状态
-            set_global_proxy('on')
-        else:
-            # 已经是打开状态
-            set_global_proxy('off')
-
-
-def print_resp_json(resp, indent=2):
-    from .json_util import json_dumps
-    json_str = json_dumps(resp.json(), indent=indent)
-    from .sys_util import parse_unicode_escape_text
-    print(parse_unicode_escape_text(json_str))
-
-
-def WebKit_format(data, boundary="----WebKitFormBoundary*********ABC", headers=None):
-    # 从headers中提取boundary信息
-    if headers is None:
-        headers = {}
-    if "content-type" in headers:
-        fd_val = str(headers["content-type"])
-        if "boundary" in fd_val:
-            fd_val = fd_val.split(";")[1].strip()
-            boundary = fd_val.split("=")[1].strip()
-        else:
-            raise Exception("multipart/form-data头信息错误，请检查content-type key是否包含boundary")
-    # form-data格式定式
-    jion_str = '--{}\r\nContent-Disposition: form-data; name="{}"\r\n\r\n{}\r\n'
-    end_str = "--{}--".format(boundary)
-    args_str = ""
-    if not isinstance(data, dict):
-        raise Exception("multipart/form-data参数错误，data参数应为dict类型")
-    for key, value in data.items():
-        args_str += jion_str.format(boundary, key, value)
-    args_str += end_str.format(boundary)
-    args_str = args_str.replace("\'", "\"")
-    return args_str
-
-
-class IResp:
-
-    @property
-    def http_code(self) -> str:
-        raise NotImplementedError
-
-    @property
-    def is_success(self) -> bool:
-        raise NotImplementedError
-
-    @property
-    def is_not_success(self) -> bool:
-        return not self.is_success
-
-    def require_success(self):
-        if self.is_not_success:
-            raise AssertionError('response is failed')
-
-    @property
-    def text(self) -> str:
-        raise NotImplementedError
-
-    @property
-    def url(self) -> str:
-        raise NotImplementedError
-
-    @property
-    def headers(self) -> dict:
-        raise NotImplementedError
-
-    @property
-    def content(self):
-        raise NotImplementedError
-
-    @property
-    def redirect_url(self) -> str:
-        return self.headers['Location']
-
-    @property
-    def res_data(self) -> dict:
-        raise NotImplementedError
-
-    @property
-    def model_data(self) -> DictModel:
-        raise NotImplementedError
-
-    def json(self, **kwargs) -> dict:
-        raise NotImplementedError
-
-    def model(self) -> DictModel:
-        raise NotImplementedError
-
-
-class CommonResp(IResp):
-
-    def __init__(self, resp):
-        self.resp = resp
-
-    @property
-    def http_code(self):
-        return self.resp.status_code
-
-    @property
-    def is_success(self) -> bool:
-        return self.resp.status_code == 200
-
-    @property
-    def text(self) -> str:
-        return self.resp.text
-
-    @property
-    def url(self) -> str:
-        return self.resp.url
-
-    @property
-    def headers(self) -> dict:
-        return self.resp.headers
-
-    @property
-    def content(self):
-        return self.resp.content
-
-    @property
-    def code(self):
-        return self.json()['code']
-
-    @property
-    def msg(self):
-        return self.json()['msg']
-
-    @property
-    def res_data(self) -> Any:
-        self.require_success()
-        return self.json()['data']
-
-    @property
-    def model_data(self) -> Any:
-        self.require_success()
-        return self.model().data
-
-    def json(self, **kwargs) -> Dict:
-        raise NotImplementedError
-
-    def model(self) -> DictModel:
-        raise NotImplementedError
+from .typing_util import *
+from .json_util import DictModel
+
+
+class ProxyBuilder:
+    proxy_protocols = ['https', 'http']
+    addr_f = '{}:{}'
+
+    @classmethod
+    def build_proxy(cls, address):
+        proxies = {protocol: address for protocol in cls.proxy_protocols}
+        return proxies
+
+    @classmethod
+    def clash_proxy(cls, ip='127.0.0.1', port='7890'):
+        return cls.build_proxy(cls.addr_f.format(ip, port))
+
+    @classmethod
+    def v2ray_proxy(cls, ip='127.0.0.1', port='10809'):
+        return cls.build_proxy(cls.addr_f.format(ip, port))
+
+    @classmethod
+    def build_by_str(cls, text):
+        """
+        :param text: 127.0.0.1:1234 / clash / v2ray
+        """
+        proxy = getattr(cls, text + '_proxy', None)
+        if proxy is None:
+            # 127.0.0.1:1234
+            return cls.build_proxy(text)
+        else:
+            # clash_proxy
+            return proxy()
+
+    v2Ray_proxy = v2ray_proxy
+
+
+def save_resp_content(resp, filepath: str):
+    from .file_util import of_dir_path
+    of_dir_path(filepath, mkdir=True)
+    with open(filepath, 'wb') as f:
+        f.write(resp.content)
+
+
+def set_global_proxy(status='off'):
+    """
+    全局性的关闭或者启用系统代理。
+    测试时发现，如果设置了系统代理，在访问 https 网站时发生错误 requests.exceptions.ProxyError
+    原因是 SSL: self._sslobj.do_handshake() -> OSError: [Errno 0] Error
+    进一步，是因为 urllib3 1.26.0 以上版本支持 https协议，但是代理软件不支持，导致连接错误。
+    所以使用 { 'https': 'http://127.0.0.1:1080' }，http的协议访问 https 的网址（本地通信），即可解决。
+    或者在 requests.get 函数中增加 proxies={'https': None} 参数来解决，但每次访问都需加这个参数，太麻烦，
+    此处通过修改 requests 库中的 get_environ_proxies 函数的方法来全局性地关闭系统代理，或者仅关闭 https 的代理。
+
+    注意：仅影响本 Python程序的 requests包，不影响其他 Python程序，
+    不影响 Windows系统的代理设置，也不影响浏览器的代理设置。
+
+    :param status: status - 'off', 关闭系统代理；'on', 打开系统代理；'toggle', 切换关闭或者打开状态；
+    """
+    from requests import sessions, utils
+    init_func = sessions.get_environ_proxies
+    if status == 'off':
+        # 关闭系统代理
+        if init_func.__name__ == '<lambda>':
+            # 已经替换了原始函数，即已经是关闭状态，无需设置
+            return
+        # 修改函数，也可以是 lambda *x, **y: {'https': None}
+        sessions.get_environ_proxies = lambda *x, **y: {}
+    elif status == 'on':
+        # 打开系统代理，如果设置了代理的话
+        # 对高版本的 urllib3(>1.26.0) 打补丁，修正 https代理 BUG: OSError: [Errno 0] Error
+        # noinspection PyUnresolvedReferences
+        proxies = utils.getproxies()
+        if 'https' in proxies:
+            proxies['https'] = proxies.get('http')  # None 或者 'http://127.0.0.1:1080'
+        sessions.get_environ_proxies = lambda *x, **y: proxies
+        sessions.get_environ_proxies.__name__ = 'get_environ_proxies'
+    else:
+        # 切换开关状态
+        if init_func.__name__ == '<lambda>':
+            # 已经是关闭状态
+            set_global_proxy('on')
+        else:
+            # 已经是打开状态
+            set_global_proxy('off')
+
+
+def print_resp_json(resp, indent=2):
+    from .json_util import json_dumps
+    json_str = json_dumps(resp.json(), indent=indent)
+    from .sys_util import parse_unicode_escape_text
+    print(parse_unicode_escape_text(json_str))
+
+
+def WebKit_format(data, boundary="----WebKitFormBoundary*********ABC", headers=None):
+    # 从headers中提取boundary信息
+    if headers is None:
+        headers = {}
+    if "content-type" in headers:
+        fd_val = str(headers["content-type"])
+        if "boundary" in fd_val:
+            fd_val = fd_val.split(";")[1].strip()
+            boundary = fd_val.split("=")[1].strip()
+        else:
+            raise Exception("multipart/form-data头信息错误，请检查content-type key是否包含boundary")
+    # form-data格式定式
+    jion_str = '--{}\r\nContent-Disposition: form-data; name="{}"\r\n\r\n{}\r\n'
+    end_str = "--{}--".format(boundary)
+    args_str = ""
+    if not isinstance(data, dict):
+        raise Exception("multipart/form-data参数错误，data参数应为dict类型")
+    for key, value in data.items():
+        args_str += jion_str.format(boundary, key, value)
+    args_str += end_str.format(boundary)
+    args_str = args_str.replace("\'", "\"")
+    return args_str
+
+
+class IResp:
+
+    @property
+    def http_code(self) -> str:
+        raise NotImplementedError
+
+    @property
+    def is_success(self) -> bool:
+        raise NotImplementedError
+
+    @property
+    def is_not_success(self) -> bool:
+        return not self.is_success
+
+    def require_success(self):
+        if self.is_not_success:
+            raise AssertionError('response is failed')
+
+    @property
+    def text(self) -> str:
+        raise NotImplementedError
+
+    @property
+    def url(self) -> str:
+        raise NotImplementedError
+
+    @property
+    def headers(self) -> dict:
+        raise NotImplementedError
+
+    @property
+    def content(self):
+        raise NotImplementedError
+
+    @property
+    def redirect_url(self) -> str:
+        return self.headers['Location']
+
+    @property
+    def res_data(self) -> dict:
+        raise NotImplementedError
+
+    @property
+    def model_data(self) -> DictModel:
+        raise NotImplementedError
+
+    def json(self, **kwargs) -> dict:
+        raise NotImplementedError
+
+    def model(self) -> DictModel:
+        raise NotImplementedError
+
+
+class CommonResp(IResp):
+
+    def __init__(self, resp):
+        self.resp = resp
+
+    @property
+    def http_code(self):
+        return self.resp.status_code
+
+    @property
+    def is_success(self) -> bool:
+        return self.resp.status_code == 200
+
+    @property
+    def text(self) -> str:
+        return self.resp.text
+
+    @property
+    def url(self) -> str:
+        return self.resp.url
+
+    @property
+    def headers(self) -> dict:
+        return self.resp.headers
+
+    @property
+    def content(self):
+        return self.resp.content
+
+    @property
+    def code(self):
+        return self.json()['code']
+
+    @property
+    def msg(self):
+        return self.json()['msg']
+
+    @property
+    def res_data(self) -> Any:
+        self.require_success()
+        return self.json()['data']
+
+    @property
+    def model_data(self) -> Any:
+        self.require_success()
+        return self.model().data
+
+    def json(self, **kwargs) -> Dict:
+        raise NotImplementedError
+
+    def model(self) -> DictModel:
+        raise NotImplementedError
```

### Comparing `commonX-0.5.1/common/util/sys_util.py` & `commonX-0.5.2/common/util/sys_util.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-import inspect
-
-from .typing_util import *
-from .args_util import process_args_kwargs
-from .file_util import fix_filepath, mkdir_if_not_exists
-
-_workspace = ""
-
-
-def workspace(sub_file=None, mode=None, encoding='utf-8', is_dir=False) -> Union[str, IO]:
-    global _workspace
-
-    if len(_workspace) != 0:
-        workspace = _workspace
-    else:
-        import os
-        workspace = fix_filepath(os.getcwd())
-
-    if sub_file is None:
-        return workspace
-
-    sub_file = fix_filepath(workspace + sub_file, is_dir)
-    if is_dir:
-        if mode is not None:
-            raise AssertionError(f'不可以读取文件夹！args=({sub_file}, {mode}, {encoding}, {is_dir})')
-
-        mkdir_if_not_exists(sub_file)
-        return sub_file
-    else:
-        if mode is None:
-            return sub_file
-
-        return open(sub_file,
-                    mode=mode,
-                    encoding=encoding,
-                    )
-
-
-def set_application_workspace(workspace: str):
-    global _workspace
-    _workspace = fix_filepath(workspace, is_dir=True)
-
-
-def current_thread():
-    from threading import current_thread
-    return current_thread()
-
-
-def copy_obj(obj):
-    if obj is None:
-        return None
-    return obj.copy()
-
-
-def pause_console():
-    import os
-    os.system("pause")
-
-
-def atexit_register(func, args=None, kwargs=None, ensure_only_once=False):
-    if ensure_only_once is True:
-        atexit_unregister(func)
-    args, kwargs = process_args_kwargs(args, kwargs)
-    import atexit
-    atexit.register(func, *args, **kwargs)
-
-
-def atexit_unregister(func):
-    import atexit
-    atexit.unregister(func)
-
-
-def atexit_clear():
-    # noinspection PyProtectedMember
-    from atexit import _clear
-    _clear()
-
-
-def atexit_ncallbacks():
-    # noinspection PyProtectedMember
-    from atexit import _ncallbacks
-    return _ncallbacks()
-
-
-ismethod = inspect.ismethod
-is_function = inspect.isfunction
-
-
-class ApplicationMessageCenter:
-    msg_need_to_confirm: Dict[Any, List[str]] = {}
-
-    @staticmethod
-    def __ofKey():
-        # from threading import current_thread
-        # return current_thread()
-        return 1
-
-    @classmethod
-    def append_msg(cls, msg: str, key=None):
-        key = key or cls.__ofKey()
-        msgs = cls.msg_need_to_confirm
-        if key not in msgs:
-            msgs[key] = [msg]
-        else:
-            msgs[key].append(msg)
-
-    @classmethod
-    def of_msgs_need_to_confirm(cls) -> List[str]:
-        msgs = cls.msg_need_to_confirm.get(cls.__ofKey(), None)
-        return msgs if msgs is not None else []
-
-
-def print_sep(text='-', length=70):
-    print(''.center(length, text))
-
-
-def print_eye_catching(text, need_to_confirm=False, surround='\n', multiple=1, key=None):
-    if need_to_confirm is True:
-        ApplicationMessageCenter.append_msg(text, key)
-    margin = surround * multiple
-    print(f"{margin}{text}{margin}")
-
-
-def print_list(data: Iterable, sep='\n', **kwargs):
-    print(*data, sep=sep, **kwargs)
-
-
-def print_obj_dict(obj: object, sep='\n', **kwargs):
-    dic = obj if isinstance(obj, dict) else obj.__dict__
-    print_list(list(dic.items()), sep=sep, **kwargs)
-
-
-def paste_from_clip() -> str:
-    from pyperclip import paste
-    return paste()
-
-
-def copy_to_clip(text: str, do_print=False):
-    from pyperclip import copy
-    copy(text)
-    if do_print is True:
-        print(text)
-
-
-def ask_open_sys_explorer(message: str, dirpath):
-    import tkinter
-    from tkinter.messagebox import askyesno
-    window = tkinter.Tk()
-    window.attributes('-topmost', True)
-    window.withdraw()  # 退出默认 tk 窗口
-    if askyesno('打开文件夹', message):
-        import os
-        r = "\\"
-        os.system(f"explorer {dirpath.replace('/', r)}")
-
-
-def parse_unicode_escape_text(text: str) -> str:
-    def decode(raw: re.Match):
-        return raw.group(0).encode('utf-8').decode('unicode_escape')
-
-    return re.sub(r"\\u\w{4}", decode, text).replace(r"\/", "/")
-
-
-def traceback_print_exec():
-    import traceback
-    traceback.print_exc()
-
-
-def str_to_line_iter(lines: str):
-    for line in lines.strip().splitlines():
-        line = line.strip()
-        if line != '':
-            yield line
-
-
-def str_to_list(lines: str):
-    return list(str_to_line_iter(lines))
-
-
-def str_to_set(lines: str):
-    return set(str_to_line_iter(lines))
-
-
-def show_bytecodes():
-    from dis import dis
-    try:
-        dis(paste_from_clip())
-    except:
-        return
+import inspect
+
+from .typing_util import *
+from .args_util import process_args_kwargs
+from .file_util import fix_filepath, mkdir_if_not_exists
+
+_workspace = ""
+
+
+def workspace(sub_file=None, mode=None, encoding='utf-8', is_dir=False) -> Union[str, IO]:
+    global _workspace
+
+    if len(_workspace) != 0:
+        workspace = _workspace
+    else:
+        import os
+        workspace = fix_filepath(os.getcwd())
+
+    if sub_file is None:
+        return workspace
+
+    sub_file = fix_filepath(workspace + sub_file, is_dir)
+    if is_dir:
+        if mode is not None:
+            raise AssertionError(f'不可以读取文件夹！args=({sub_file}, {mode}, {encoding}, {is_dir})')
+
+        mkdir_if_not_exists(sub_file)
+        return sub_file
+    else:
+        if mode is None:
+            return sub_file
+
+        return open(sub_file,
+                    mode=mode,
+                    encoding=encoding,
+                    )
+
+
+def set_application_workspace(workspace: str):
+    global _workspace
+    _workspace = fix_filepath(workspace, is_dir=True)
+
+
+def current_thread():
+    from threading import current_thread
+    return current_thread()
+
+
+def copy_obj(obj):
+    if obj is None:
+        return None
+    return obj.copy()
+
+
+def pause_console():
+    import os
+    os.system("pause")
+
+
+def atexit_register(func, args=None, kwargs=None, ensure_only_once=False):
+    if ensure_only_once is True:
+        atexit_unregister(func)
+    args, kwargs = process_args_kwargs(args, kwargs)
+    import atexit
+    atexit.register(func, *args, **kwargs)
+
+
+def atexit_unregister(func):
+    import atexit
+    atexit.unregister(func)
+
+
+def atexit_clear():
+    # noinspection PyProtectedMember
+    from atexit import _clear
+    _clear()
+
+
+def atexit_ncallbacks():
+    # noinspection PyProtectedMember
+    from atexit import _ncallbacks
+    return _ncallbacks()
+
+
+ismethod = inspect.ismethod
+is_function = inspect.isfunction
+
+
+class ApplicationMessageCenter:
+    msg_need_to_confirm: Dict[Any, List[str]] = {}
+
+    @staticmethod
+    def __ofKey():
+        # from threading import current_thread
+        # return current_thread()
+        return 1
+
+    @classmethod
+    def append_msg(cls, msg: str, key=None):
+        key = key or cls.__ofKey()
+        msgs = cls.msg_need_to_confirm
+        if key not in msgs:
+            msgs[key] = [msg]
+        else:
+            msgs[key].append(msg)
+
+    @classmethod
+    def of_msgs_need_to_confirm(cls) -> List[str]:
+        msgs = cls.msg_need_to_confirm.get(cls.__ofKey(), None)
+        return msgs if msgs is not None else []
+
+
+def print_sep(text='-', length=70):
+    print(''.center(length, text))
+
+
+def print_eye_catching(text, need_to_confirm=False, surround='\n', multiple=1, key=None):
+    if need_to_confirm is True:
+        ApplicationMessageCenter.append_msg(text, key)
+    margin = surround * multiple
+    print(f"{margin}{text}{margin}")
+
+
+def print_list(data: Iterable, sep='\n', **kwargs):
+    print(*data, sep=sep, **kwargs)
+
+
+def print_obj_dict(obj: object, sep='\n', **kwargs):
+    dic = obj if isinstance(obj, dict) else obj.__dict__
+    print_list(list(dic.items()), sep=sep, **kwargs)
+
+
+def paste_from_clip() -> str:
+    from pyperclip import paste
+    return paste()
+
+
+def copy_to_clip(text: str, do_print=False):
+    from pyperclip import copy
+    copy(text)
+    if do_print is True:
+        print(text)
+
+
+def ask_open_sys_explorer(message: str, dirpath):
+    import tkinter
+    from tkinter.messagebox import askyesno
+    window = tkinter.Tk()
+    window.attributes('-topmost', True)
+    window.withdraw()  # 退出默认 tk 窗口
+    if askyesno('打开文件夹', message):
+        import os
+        r = "\\"
+        os.system(f"explorer {dirpath.replace('/', r)}")
+
+
+def parse_unicode_escape_text(text: str) -> str:
+    def decode(raw: re.Match):
+        return raw.group(0).encode('utf-8').decode('unicode_escape')
+
+    return re.sub(r"\\u\w{4}", decode, text).replace(r"\/", "/")
+
+
+def traceback_print_exec():
+    import traceback
+    traceback.print_exc()
+
+
+def str_to_line_iter(lines: str):
+    for line in lines.strip().splitlines():
+        line = line.strip()
+        if line != '':
+            yield line
+
+
+def str_to_list(lines: str):
+    return list(str_to_line_iter(lines))
+
+
+def str_to_set(lines: str):
+    return set(str_to_line_iter(lines))
+
+
+def show_bytecodes():
+    from dis import dis
+    try:
+        dis(paste_from_clip())
+    except:
+        return
```

### Comparing `commonX-0.5.1/common/util/typing_util.py` & `commonX-0.5.2/common/util/typing_util.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# noinspection PyUnresolvedReferences
-import typing
-# noinspection PyUnresolvedReferences
-from typing import Dict, List, Tuple, Set, \
-    Type, Callable, Any, Optional, Union, \
-    Iterable, Iterator, Generator, Sequence, \
-    IO, Match, Pattern
-# noinspection PyUnresolvedReferences
-import threading
-# noinspection PyUnresolvedReferences
-from threading import Thread
-# noinspection PyUnresolvedReferences
-import multiprocessing
-# noinspection PyUnresolvedReferences
-from multiprocessing import Process
-# noinspection PyUnresolvedReferences
-import re
-# noinspection PyUnresolvedReferences
-from re import compile
-
-StrNone = Optional[str]
-ListNone = Optional[List]
-DictNone = Optional[Dict]
+# noinspection PyUnresolvedReferences
+import typing
+# noinspection PyUnresolvedReferences
+from typing import Dict, List, Tuple, Set, \
+    Type, Callable, Any, Optional, Union, \
+    Iterable, Iterator, Generator, Sequence, \
+    IO, Match, Pattern
+# noinspection PyUnresolvedReferences
+import threading
+# noinspection PyUnresolvedReferences
+from threading import Thread
+# noinspection PyUnresolvedReferences
+import multiprocessing
+# noinspection PyUnresolvedReferences
+from multiprocessing import Process
+# noinspection PyUnresolvedReferences
+import re
+# noinspection PyUnresolvedReferences
+from re import compile
+
+StrNone = Optional[str]
+ListNone = Optional[List]
+DictNone = Optional[Dict]
```

### Comparing `commonX-0.5.1/commonX.egg-info/PKG-INFO` & `commonX-0.5.2/commonX.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
-Name: commonX
-Version: 0.5.1
-Summary: python common toolkit
-Home-page: https://github.com/hect0x7/common
-Author: hect0x7
-Author-email: 93357912+hect0x7@users.noreply.github.com
-Keywords: python,toolkit,postman
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires: requests
-Requires: requests_toolbelt
-Requires: PyYAML
-Requires: pyperclip
-Requires: curl_cffi
-Description-Content-Type: text/markdown
-
-
-python common toolkit
-
-see source code: https://github.com/hect0x7/common
+Metadata-Version: 2.1
+Name: commonX
+Version: 0.5.2
+Summary: python common toolkit
+Home-page: https://github.com/hect0x7/common
+Author: hect0x7
+Author-email: 93357912+hect0x7@users.noreply.github.com
+Keywords: python,toolkit,postman
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires: requests
+Requires: requests_toolbelt
+Requires: PyYAML
+Requires: pyperclip
+Requires: curl_cffi
+Description-Content-Type: text/markdown
+
+
+python common toolkit
+
+see source code: https://github.com/hect0x7/common
```

### Comparing `commonX-0.5.1/commonX.egg-info/SOURCES.txt` & `commonX-0.5.2/commonX.egg-info/SOURCES.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 README.md
 setup.py
 common/__init__.py
-commonX.egg-info/PKG-INFO
-commonX.egg-info/SOURCES.txt
-commonX.egg-info/dependency_links.txt
-commonX.egg-info/top_level.txt
 common/base/__init__.py
 common/base/entity.py
 common/base/factory.py
 common/base/genor.py
 common/base/hook.py
 common/base/logger.py
 common/base/mapper.py
@@ -31,8 +27,12 @@
 common/util/exception_utll.py
 common/util/file_util.py
 common/util/image_util.py
 common/util/json_util.py
 common/util/requests_util.py
 common/util/sys_util.py
 common/util/time_util.py
-common/util/typing_util.py
+common/util/typing_util.py
+commonX.egg-info/PKG-INFO
+commonX.egg-info/SOURCES.txt
+commonX.egg-info/dependency_links.txt
+commonX.egg-info/top_level.txt
```

### Comparing `commonX-0.5.1/setup.py` & `commonX-0.5.2/setup.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import os
-import codecs
-
-from setuptools import setup, find_packages
-
-here = os.path.abspath(os.path.dirname(__file__))
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
-    long_description = "\n" + f.read()
-
-VERSION = None
-with open(os.path.join(here, './common/__init__.py')) as f:
-    for line in f:
-        if line.startswith("VERSION"):
-            VERSION = line[line.index("'") + 1: line.rindex("'")]
-            break
-
-if VERSION is None:
-    print('Set VERSION first!')
-    exit(1)
-
-DESCRIPTION = 'python common toolkit'
-
-setup(
-    name='commonX',
-    version=VERSION,
-    description=DESCRIPTION,
-    author='hect0x7',
-    packages=find_packages(),
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    requires=[
-        "requests",
-        "requests_toolbelt",
-        "PyYAML",
-        "pyperclip",
-        "curl_cffi",
-    ],
-    keywords=['python', 'toolkit', 'postman'],
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3.7",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ],
-    author_email='93357912+hect0x7@users.noreply.github.com',
-    url='https://github.com/hect0x7/common',
-)
+import os
+import codecs
+
+from setuptools import setup, find_packages
+
+here = os.path.abspath(os.path.dirname(__file__))
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+    long_description = "\n" + f.read()
+
+VERSION = None
+with open(os.path.join(here, './common/__init__.py')) as f:
+    for line in f:
+        if line.startswith("VERSION"):
+            VERSION = line[line.index("'") + 1: line.rindex("'")]
+            break
+
+if VERSION is None:
+    print('Set VERSION first!')
+    exit(1)
+
+DESCRIPTION = 'python common toolkit'
+
+setup(
+    name='commonX',
+    version=VERSION,
+    description=DESCRIPTION,
+    author='hect0x7',
+    packages=find_packages(),
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    requires=[
+        "requests",
+        "requests_toolbelt",
+        "PyYAML",
+        "pyperclip",
+        "curl_cffi",
+    ],
+    keywords=['python', 'toolkit', 'postman'],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3.7",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ],
+    author_email='93357912+hect0x7@users.noreply.github.com',
+    url='https://github.com/hect0x7/common',
+)
```

