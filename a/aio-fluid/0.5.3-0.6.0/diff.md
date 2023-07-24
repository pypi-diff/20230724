# Comparing `tmp/aio_fluid-0.5.3.tar.gz` & `tmp/aio_fluid-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_fluid-0.5.3.tar", max compression
+gzip compressed data, was "aio_fluid-0.6.0.tar", max compression
```

## Comparing `aio_fluid-0.5.3.tar` & `aio_fluid-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1517 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/LICENSE
--rw-r--r--   0        0        0       64 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/__init__.py
--rw-r--r--   0        0        0     1633 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/backdoor.py
--rw-r--r--   0        0        0      593 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/cors.py
--rw-r--r--   0        0        0     2165 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/datajson.py
--rw-r--r--   0        0        0     1493 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/db.py
--rw-r--r--   0        0        0      218 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/dev.py
--rw-r--r--   0        0        0      575 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/executor.py
--rw-r--r--   0        0        0     1225 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/fields.py
--rw-r--r--   0        0        0       75 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/github/__init__.py
--rw-r--r--   0        0        0      866 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/github/client.py
--rw-r--r--   0        0        0     4084 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/github/repo.py
--rw-r--r--   0        0        0    11637 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/http.py
--rw-r--r--   0        0        0      138 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/json.py
--rw-r--r--   0        0        0     2471 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/kernel.py
--rw-r--r--   0        0        0      296 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/kong.py
--rw-r--r--   0        0        0     2936 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/log.py
--rw-r--r--   0        0        0     9519 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/node.py
--rw-r--r--   0        0        0        0 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/py.typed
--rw-r--r--   0        0        0     3784 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/redis.py
--rw-r--r--   0        0        0      620 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/redis_status.py
--rw-r--r--   0        0        0      758 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/__init__.py
--rw-r--r--   0        0        0     8327 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/broker.py
--rw-r--r--   0        0        0      347 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/constants.py
--rw-r--r--   0        0        0     9568 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/consumer.py
--rw-r--r--   0        0        0     2788 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/cpubound.py
--rw-r--r--   0        0        0     4209 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/crontab.py
--rw-r--r--   0        0        0     1263 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/every.py
--rw-r--r--   0        0        0     2306 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/readme.md
--rw-r--r--   0        0        0     1491 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/scheduler.py
--rw-r--r--   0        0        0      170 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/settings.py
--rw-r--r--   0        0        0     4676 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/task.py
--rw-r--r--   0        0        0     1547 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/task_run.py
--rw-r--r--   0        0        0      363 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/utils.py
--rw-r--r--   0        0        0     2023 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/service.py
--rw-r--r--   0        0        0      429 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/settings.py
--rw-r--r--   0        0        0     6692 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/stacksampler.py
--rw-r--r--   0        0        0     1003 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/status.py
--rw-r--r--   0        0        0      399 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/sync_run.py
--rw-r--r--   0        0        0      526 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/text.py
--rw-r--r--   0        0        0      599 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/types.py
--rw-r--r--   0        0        0     2605 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/utils.py
--rw-r--r--   0        0        0     2383 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1213 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/readme.md
--rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 aio_fluid-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/LICENSE
+-rw-r--r--   0        0        0       64 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/__init__.py
+-rw-r--r--   0        0        0     1633 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/backdoor.py
+-rw-r--r--   0        0        0      593 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/cors.py
+-rw-r--r--   0        0        0     2165 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/datajson.py
+-rw-r--r--   0        0        0     1493 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/db.py
+-rw-r--r--   0        0        0      218 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/dev.py
+-rw-r--r--   0        0        0      575 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/executor.py
+-rw-r--r--   0        0        0     1225 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/fields.py
+-rw-r--r--   0        0        0       75 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/github/__init__.py
+-rw-r--r--   0        0        0      866 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/github/client.py
+-rw-r--r--   0        0        0     4084 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/github/repo.py
+-rw-r--r--   0        0        0    11637 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/http.py
+-rw-r--r--   0        0        0      138 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/json.py
+-rw-r--r--   0        0        0     2471 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/kernel.py
+-rw-r--r--   0        0        0      296 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/kong.py
+-rw-r--r--   0        0        0     2949 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/log.py
+-rw-r--r--   0        0        0     9527 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/node.py
+-rw-r--r--   0        0        0        0 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/py.typed
+-rw-r--r--   0        0        0     3784 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/redis.py
+-rw-r--r--   0        0        0      620 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/redis_status.py
+-rw-r--r--   0        0        0      834 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/__init__.py
+-rw-r--r--   0        0        0     8222 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/broker.py
+-rw-r--r--   0        0        0      347 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/constants.py
+-rw-r--r--   0        0        0     9666 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/consumer.py
+-rw-r--r--   0        0        0     3153 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/cpubound.py
+-rw-r--r--   0        0        0     4209 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/crontab.py
+-rw-r--r--   0        0        0     1263 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/every.py
+-rw-r--r--   0        0        0     2306 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/readme.md
+-rw-r--r--   0        0        0     1491 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/scheduler.py
+-rw-r--r--   0        0        0      170 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/settings.py
+-rw-r--r--   0        0        0     5110 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/task.py
+-rw-r--r--   0        0        0      729 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/task_info.py
+-rw-r--r--   0        0        0     1580 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/task_run.py
+-rw-r--r--   0        0        0      370 2023-07-24 11:43:23.657412 aio_fluid-0.6.0/fluid/scheduler/utils.py
+-rw-r--r--   0        0        0     2023 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/fluid/service.py
+-rw-r--r--   0        0        0      429 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/fluid/settings.py
+-rw-r--r--   0        0        0     6692 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/fluid/stacksampler.py
+-rw-r--r--   0        0        0     1003 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/fluid/status.py
+-rw-r--r--   0        0        0      399 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/fluid/sync_run.py
+-rw-r--r--   0        0        0      526 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/fluid/text.py
+-rw-r--r--   0        0        0      599 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/fluid/types.py
+-rw-r--r--   0        0        0     2605 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/fluid/utils.py
+-rw-r--r--   0        0        0     2329 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1311 2023-07-24 11:43:23.661412 aio_fluid-0.6.0/readme.md
+-rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 aio_fluid-0.6.0/PKG-INFO
```

### Comparing `aio_fluid-0.5.3/LICENSE` & `aio_fluid-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/backdoor.py` & `aio_fluid-0.6.0/fluid/backdoor.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/cors.py` & `aio_fluid-0.6.0/fluid/cors.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/datajson.py` & `aio_fluid-0.6.0/fluid/datajson.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/db.py` & `aio_fluid-0.6.0/fluid/db.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/executor.py` & `aio_fluid-0.6.0/fluid/executor.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/fields.py` & `aio_fluid-0.6.0/fluid/fields.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/github/client.py` & `aio_fluid-0.6.0/fluid/github/client.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/github/repo.py` & `aio_fluid-0.6.0/fluid/github/repo.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/http.py` & `aio_fluid-0.6.0/fluid/http.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/kernel.py` & `aio_fluid-0.6.0/fluid/kernel.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/log.py` & `aio_fluid-0.6.0/fluid/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 from logging.config import dictConfig
-from typing import Dict, Optional
+from typing import Any, cast
 
 import click
 
 logger = logging.getLogger()
 
 
 LOG_LEVEL = (os.environ.get("LOG_LEVEL") or "info").upper()
@@ -28,23 +28,23 @@
 
 
 def get_logger(name: str = "") -> logging.Logger:
     return logger.getChild(name) if name else logger
 
 
 def level_num(level: str) -> int:
-    return getattr(logging, level)
+    return cast(int, getattr(logging, level))
 
 
 def log_config(
     level: int,
     other_level: int = logging.WARNING,
-    app_name: Optional[str] = None,
+    app_name: str | None = None,
     json: bool = bool(K8S),
-) -> Dict:
+) -> dict[str, Any]:
     app_name = app_name if app_name is not None else APP_NAME
     other_level = max(level, other_level)
     handler = LOG_HANDLER or ("main" if json else "color")
     return {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
```

### Comparing `aio_fluid-0.5.3/fluid/node.py` & `aio_fluid-0.6.0/fluid/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             self.logger.exception("unhandled exception in worker")
             await self.system_exit()
         else:
             await self.close(close_worker=False)
 
 
 class WorkerApplication(dict[str, Any]):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.on_startup = []
         self.on_shutdown = []
 
     async def startup(self) -> None:
         for on_startup in self.on_startup:
             await on_startup(self)
```

### Comparing `aio_fluid-0.5.3/fluid/redis.py` & `aio_fluid-0.6.0/fluid/redis.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/redis_status.py` & `aio_fluid-0.6.0/fluid/redis_status.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/scheduler/__init__.py` & `aio_fluid-0.6.0/fluid/scheduler/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from .broker import Broker, QueuedTask
 from .constants import TaskPriority, TaskState
 from .consumer import TaskConsumer, TaskManager
-from .crontab import crontab
+from .crontab import Scheduler, crontab
 from .every import every
 from .scheduler import TaskScheduler
 from .task import (
     Task,
     TaskConstructor,
     TaskContext,
     TaskDecoratorError,
     TaskExecutor,
     TaskRunError,
     create_task_app,
     task,
 )
+from .task_info import TaskInfo
 from .task_run import TaskRun
 
 __all__ = [
+    "Scheduler",
     "TaskPriority",
     "TaskState",
     "TaskScheduler",
     "task",
     "Task",
     "TaskContext",
     "TaskRunError",
     "TaskExecutor",
     "TaskConstructor",
     "TaskDecoratorError",
     "TaskManager",
     "TaskConsumer",
+    "TaskInfo",
     "TaskRun",
     "QueuedTask",
     "Broker",
     "create_task_app",
     "crontab",
     "every",
 ]
```

### Comparing `aio_fluid-0.5.3/fluid/scheduler/broker.py` & `aio_fluid-0.6.0/fluid/scheduler/broker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from abc import ABC, abstractmethod, abstractproperty
 from functools import cached_property
 from typing import Any, Dict, Iterable, List, NamedTuple, Optional
 from uuid import uuid4
 
 from yarl import URL
 
 from fluid import json
 from fluid.redis import FluidRedis
 from fluid.utils import microseconds
 
 from . import settings
 from .constants import TaskPriority, TaskState
 from .task import Task
+from .task_info import TaskInfo
 from .task_run import TaskRun
 
 _brokers: dict[str, type[Broker]] = {}
 
 
 def broker_url_from_env() -> URL:
     return URL(settings.SCHEDULER_BROKER_URL)
@@ -32,26 +32,14 @@
     pass
 
 
 class DisabledTask(TaskError):
     pass
 
 
-@dataclass
-class TaskInfo:
-    name: str
-    description: str
-    priority: str
-    schedule: Optional[str] = None
-    enabled: bool = True
-    last_run_end: Optional[int] = None
-    last_run_duration: Optional[int] = None
-    last_run_state: Optional[str] = None
-
-
 class TaskRegistry(Dict[str, Task]):
     def periodic(self) -> Iterable[Task]:
         for task in self.values():
             yield task
 
 
 class QueuedTask(NamedTuple):
@@ -62,32 +50,36 @@
 
 
 class Broker(ABC):
     def __init__(self, url: URL) -> None:
         self.url: URL = url
         self.registry: TaskRegistry = TaskRegistry()
 
+    @abstractproperty
+    def task_queue_names(self) -> tuple[str, ...]:
+        """Names of the task queues"""
+
     @abstractmethod
     async def queue_task(self, queued_task: QueuedTask) -> TaskRun:
         """Queue a task"""
 
     @abstractmethod
     async def get_task_run(self) -> Optional[TaskRun]:
         """Get a Task run from the task queue"""
 
     @abstractmethod
     async def queue_length(self) -> Dict[str, int]:
         """Length of task queues"""
 
     @abstractmethod
-    async def get_tasks_info(self, *task_names: str) -> List[TaskInfo]:
+    async def get_tasks_info(self, *task_names: str) -> list[TaskInfo]:
         """List of TaskInfo objects"""
 
     @abstractmethod
-    async def update_task(self, task: Task, params: dict) -> TaskInfo:
+    async def update_task(self, task: Task, params: dict[str, Any]) -> TaskInfo:
         """Update a task dynamic parameters"""
 
     async def close(self) -> None:
         """Close the broker on shutdown"""
 
     def new_uuid(self) -> str:
         return uuid4().hex
@@ -188,29 +180,29 @@
 
     def task_hash_name(self, name: str) -> str:
         return f"{self.name}-tasks-{name}"
 
     def task_queue_name(self, priority: TaskPriority) -> str:
         return f"{self.name}-queue-{priority.name}"
 
-    async def get_tasks_info(self, *task_names: str) -> List[TaskInfo]:
+    async def get_tasks_info(self, *task_names: str) -> list[TaskInfo]:
         pipe = self.redis.cli.pipeline()
         names = task_names or self.registry
         requested_task_names = []
         for name in names:
             if name in self.registry:
                 requested_task_names.append(name)
                 pipe.hgetall(self.task_hash_name(name))
         tasks_info = await pipe.execute()
         return [
             self._decode_task(self.registry[name], task_info)
             for name, task_info in zip(requested_task_names, tasks_info)
         ]
 
-    async def update_task(self, task: Task, params: dict) -> TaskInfo:
+    async def update_task(self, task: Task, params: dict[str, Any]) -> TaskInfo:
         pipe = self.redis.cli.pipeline()
         pipe.hset(
             self.task_hash_name(task.name),
             mapping={name: json.dumps(value) for name, value in params.items()},
         )
         pipe.hgetall(self.task_hash_name(task.name))
         _, info = await pipe.execute()
@@ -240,15 +232,15 @@
     async def queue_task(self, queued_task: QueuedTask) -> TaskRun:
         task = self.task_from_registry(queued_task.task)
         priority = queued_task.priority or task.priority
         data = self.task_run_data(queued_task, TaskState.queued)
         await self.redis.cli.lpush(self.task_queue_name(priority), json.dumps(data))
         return self.task_run_from_data(data)
 
-    def _decode_task(self, task: Task, data: dict) -> TaskInfo:
+    def _decode_task(self, task: Task, data: dict[bytes, Any]) -> TaskInfo:
         info = {name.decode(): json.loads(value) for name, value in data.items()}
         return TaskInfo(
             name=task.name,
             description=task.description,
             schedule=str(task.schedule) if task.schedule else None,
             priority=task.priority.name,
             enabled=info.get("enabled", True),
```

### Comparing `aio_fluid-0.5.3/fluid/scheduler/consumer.py` & `aio_fluid-0.6.0/fluid/scheduler/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections import defaultdict, deque
 from dataclasses import dataclass
 from functools import cached_property
-from typing import Any, Callable, Coroutine, Deque, Dict, NamedTuple, Optional, Tuple
+from typing import Any, Callable, Coroutine, Deque, Dict, NamedTuple, Optional
 
 from inflection import underscore
 
 from fluid.node import Consumer, NodeWorkers, Worker
 from fluid.utils import microseconds
 
 from .broker import Broker, QueuedTask, TaskRegistry, UnknownTask
 from .constants import TaskPriority, TaskState
 from .task import Task
 from .task_run import TaskRun
 
 ConsumerCallback = Callable[[TaskRun, "TaskManager"], None]
 AsyncExecutor = Callable[..., Coroutine[Any, Any, None]]
-AsyncMessage = Tuple[AsyncExecutor, Tuple]
+AsyncMessage = tuple[AsyncExecutor, tuple[Any, ...]]
 
 
 class TaskFailure(RuntimeError):
     pass
 
 
 @dataclass
@@ -143,16 +143,16 @@
 
 
 class TaskConsumer(TaskManager):
     """The Task Consumer is responsible for consuming tasks from a task queue"""
 
     def __init__(self, **config: Any) -> None:
         super().__init__(**config)
-        self._concurrent_tasks: Dict[str, Dict[str, TaskRun]] = defaultdict(dict)
-        self._priority_task_run_queue: Deque = deque()
+        self._concurrent_tasks: dict[str, dict[str, TaskRun]] = defaultdict(dict)
+        self._priority_task_run_queue: deque[TaskRun] = deque()
         for i in range(self.config.max_concurrent_tasks):
             self.add_workers(
                 Worker(
                     self._consume_tasks, logger=self.logger.getChild(f"worker-{i+1}")
                 )
             )
 
@@ -187,25 +187,27 @@
             if not self.config.consume_tasks:
                 await asyncio.sleep(self.config.sleep)
                 continue
             if self._priority_task_run_queue:
                 task_run = self._priority_task_run_queue.pop()
             else:
                 try:
-                    task_run = await self.broker.get_task_run()
+                    maybe_task_run = await self.broker.get_task_run()
                 except UnknownTask as exc:
                     self.logger.error(
                         "unknown task %s - it looks like it is not "
                         "registered with this consumer",
                         exc,
                     )
-                    task_run = None
-                if not task_run:
+                    maybe_task_run = None
+                if not maybe_task_run:
                     await asyncio.sleep(self.config.sleep)
                     continue
+                else:
+                    task_run = maybe_task_run
             task_name = task_run.name
             task_run.start = microseconds()
             task_run.set_state(TaskState.running)
             task_context = task_run.task.create_context(self, task_run=task_run)
             self._concurrent_tasks[task_name][task_run.id] = task_run
             #
             if task_run.task.max_concurrency < self.num_concurrent_tasks_for(task_name):
```

### Comparing `aio_fluid-0.5.3/fluid/scheduler/cpubound.py` & `aio_fluid-0.6.0/fluid/scheduler/cpubound.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import asyncio
 import logging
 import os
 import sys
 from logging.config import dictConfig
-from typing import Any
+from typing import Any, overload
 
 from fluid import kernel, log
 from fluid.scheduler import (
+    Scheduler,
     Task,
     TaskConstructor,
     TaskContext,
     TaskDecoratorError,
     TaskExecutor,
     TaskManager,
+    TaskPriority,
     TaskRun,
+    TaskState,
     create_task_app,
     settings,
 )
-from fluid.scheduler.constants import TaskState
+from fluid.scheduler.task import RandomizeType
 
 
 class RemoteLog:
     def __init__(self, out: Any) -> None:
         self.out = out
 
     def __call__(self, data: bytes) -> None:
@@ -55,26 +58,44 @@
             cpu_executor = executor
         else:
             self.kwargs["name"] = executor.__name__
             cpu_executor = spawn
         return super().__call__(cpu_executor)
 
 
-def cpu_task(*args: Any, **kwargs: Any) -> Task | CpuTaskConstructor:
+@overload
+def cpu_task(executor: TaskExecutor) -> Task:
+    ...
+
+
+@overload
+def cpu_task(
+    *,
+    name: str | None = None,
+    schedule: Scheduler | None = None,
+    description: str | None = None,
+    randomize: RandomizeType | None = None,
+    max_concurrency: int = 1,
+    priority: TaskPriority = TaskPriority.medium,
+) -> CpuTaskConstructor:
+    ...
+
+
+def cpu_task(
+    executor: TaskExecutor | None = None, **kwargs: Any
+) -> Task | CpuTaskConstructor:
     """Decorator for creating a CPU bound task"""
-    if kwargs and args:
+    if kwargs and executor:
         raise TaskDecoratorError("cannot use positional parameters")
     elif kwargs:
         return CpuTaskConstructor(**kwargs)
-    elif len(args) > 1:
-        raise TaskDecoratorError("cannot use positional parameters")
-    elif not args:
+    elif not executor:
         raise TaskDecoratorError("this is a decorator cannot be invoked in this way")
     else:
-        return CpuTaskConstructor()(args[0])
+        return CpuTaskConstructor()(executor)
 
 
 async def main(name: str, run_id: str) -> int:
     dictConfig(
         log.log_config(logging.INFO, logging.CRITICAL, f"{log.APP_NAME}.task.{name}")
     )
     app = create_task_app()
```

### Comparing `aio_fluid-0.5.3/fluid/scheduler/crontab.py` & `aio_fluid-0.6.0/fluid/scheduler/crontab.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/scheduler/every.py` & `aio_fluid-0.6.0/fluid/scheduler/every.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/scheduler/readme.md` & `aio_fluid-0.6.0/fluid/scheduler/readme.md`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/scheduler/scheduler.py` & `aio_fluid-0.6.0/fluid/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/scheduler/task.py` & `aio_fluid-0.6.0/fluid/scheduler/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from __future__ import annotations
 
 import inspect
 import logging
 import os
 from importlib import import_module
-from typing import TYPE_CHECKING, Any, Callable, Coroutine, NamedTuple, TypeVar
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Coroutine,
+    NamedTuple,
+    TypeVar,
+    cast,
+    overload,
+)
 from uuid import uuid4
 
 from openapi.spec.utils import trim_docstring
 
 from fluid import log
 from fluid.node import WorkerApplication
 from fluid.utils import microseconds
@@ -45,15 +54,15 @@
         raise ImproperlyConfigured("missing TASK_MANAGER_APP environment variable")
     bits = TASK_MANAGER_APP.split(":")
     if len(bits) != 2:
         raise ImproperlyConfigured(
             "TASK_MANAGER_APP must be of the form <module>:<function>"
         )
     mod = import_module(bits[0])
-    return getattr(mod, bits[1])()
+    return cast(WorkerApplication, getattr(mod, bits[1])())
 
 
 class TaskContext(NamedTuple):
     task_manager: "TaskManager"
     task_run: TaskRun
     log: LogType
     logger: logging.Logger
@@ -130,43 +139,60 @@
             task_manager=task_manager,
             task_run=task_run,
             log=log or self.logger.info,
             logger=self.logger.getChild(task_run.id),
         )
 
 
-def task(*args: Any, **kwargs: Any) -> Task | TaskConstructor:
-    if kwargs and args:
+@overload
+def task(executor: TaskExecutor) -> Task:
+    ...
+
+
+@overload
+def task(
+    *,
+    name: str | None = None,
+    schedule: Scheduler | None = None,
+    description: str | None = None,
+    randomize: RandomizeType | None = None,
+    max_concurrency: int = 1,
+    priority: TaskPriority = TaskPriority.medium,
+) -> TaskConstructor:
+    ...
+
+
+# implementation of the task decorator
+def task(executor: TaskExecutor | None = None, **kwargs: Any) -> Task | TaskConstructor:
+    if kwargs and executor:
         raise TaskDecoratorError("cannot use positional parameters")
     elif kwargs:
         return TaskConstructor(**kwargs)
-    elif len(args) > 1:
-        raise TaskDecoratorError("cannot use positional parameters")
-    elif not args:
+    elif not executor:
         raise TaskDecoratorError("this is a decorator cannot be invoked in this way")
     else:
-        return TaskConstructor()(args[0])
+        return TaskConstructor()(executor)
 
 
 class TaskConstructor:
-    def __init__(self, **kwargs: Any):
+    def __init__(self, **kwargs: Any) -> None:
         self.kwargs = kwargs
 
     def __call__(self, executor: TaskExecutor) -> Task:
         kwargs: dict[str, Any] = {
             "name": get_name(executor),
             "description": trim_docstring(inspect.getdoc(executor) or ""),
-            **self.kwargs,
             "executor": executor,
         }
+        kwargs.update(self.kwargs)
         name = kwargs["name"]
         kwargs["logger"] = log.get_logger(f"task.{name}")
         return Task(**kwargs)
 
 
 def get_name(o: Any) -> str:
     if hasattr(o, "__name__"):
-        return o.__name__
+        return str(o.__name__)
     elif hasattr(o, "__class__"):
-        return o.__class__.__name__
+        return str(o.__class__.__name__)
     else:
         return str(o)
```

### Comparing `aio_fluid-0.5.3/fluid/scheduler/task_run.py` & `aio_fluid-0.6.0/fluid/scheduler/task_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+from __future__ import annotations
+
 import asyncio
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 from .constants import FINISHED_STATES, TaskState
 
 if TYPE_CHECKING:
     from .task import Task
 
 
 @dataclass
 class TaskRun:
     """A TaskRun contains all the data generated by a Task run"""
 
     id: str
     queued: int
-    task: "Task"
-    params: Dict[str, Any]
+    task: Task
+    params: dict[str, Any]
     start: int = 0
     end: int = 0
     priority: str = ""
     state: str = TaskState.init.name
-    waiter: asyncio.Future = field(default_factory=asyncio.Future)
+    waiter: asyncio.Future[Any] = field(default_factory=asyncio.Future)
 
     @property
     def in_queue(self) -> int:
         return self.start - self.queued
 
     @property
     def duration(self) -> int:
```

### Comparing `aio_fluid-0.5.3/fluid/service.py` & `aio_fluid-0.6.0/fluid/service.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/stacksampler.py` & `aio_fluid-0.6.0/fluid/stacksampler.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/status.py` & `aio_fluid-0.6.0/fluid/status.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/text.py` & `aio_fluid-0.6.0/fluid/text.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/types.py` & `aio_fluid-0.6.0/fluid/types.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/fluid/utils.py` & `aio_fluid-0.6.0/fluid/utils.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.3/pyproject.toml` & `aio_fluid-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-fluid"
-version = "0.5.3"
+version = "0.6.0"
 description = "Tools for backend python services"
 license = "BSD"
 authors = ["Luca <luca@quantmind.com>"]
 readme = "readme.md"
 packages = [
     {include = "fluid"}
 ]
@@ -44,24 +44,26 @@
 aiohttp_cors = "^0.7.0"
 aiobotocore = {version = "~2.5.0", extras=["boto3"]}
 s3fs = {version = "^2023.5.0"}
 aio-kong = "^3.3.0"
 uvloop = "^0.17.0"
 pycountry = "^22.3.5"
 redis = "^4.4.0"
+pydantic = "^2.0.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 isort = "^5.9.3"
 black = "^23.3.0"
 pytest-cov = "^4.0.0"
 mypy = "^1.3.0"
 pytest-asyncio = "^0.21.0"
 ruff = "^0.0.270"
 types-ujson = "^5.7.0.5"
+types-redis = "^4.6.0.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
@@ -77,18 +79,15 @@
 profile = "black"
 
 [tool.ruff]
 select = ["E", "F"]
 line-length = 88
 
 [tool.mypy]
-disallow_untyped_calls = "true"
-warn_return_any = "false"
-disallow_untyped_defs = "true"
-warn_no_return = "true"
+strict = true
 
 [[tool.mypy.overrides]]
 module = "fluid.utils"
 ignore_errors = "true"
 
 
 [[tool.mypy.overrides]]
```

### Comparing `aio_fluid-0.5.3/readme.md` & `aio_fluid-0.6.0/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Tools for backend python services
 
 [![PyPI version](https://badge.fury.io/py/aio-fluid.svg)](https://badge.fury.io/py/aio-fluid)
 [![Python versions](https://img.shields.io/pypi/pyversions/aio-fluid.svg)](https://pypi.org/project/aio-fluid)
 [![build](https://github.com/quantmind/fluid/workflows/build/badge.svg)](https://github.com/quantmind/aio-fluid/actions?query=workflow%3Abuild)
 [![codecov](https://codecov.io/gh/quantmind/aio-fluid/branch/main/graph/badge.svg?token=81oWUoyEVp)](https://codecov.io/gh/quantmind/aio-fluid)
+[![Downloads](https://img.shields.io/pypi/dd/aio-fluid.svg)](https://pypi.org/project/aio-fluid/)
 
 ## Installation
 
 This is a simple python package you can install via pip:
 
 ```
 pip install aio-fluid
```

### Comparing `aio_fluid-0.5.3/PKG-INFO` & `aio_fluid-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-fluid
-Version: 0.5.3
+Version: 0.6.0
 Summary: Tools for backend python services
 License: BSD
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -28,14 +28,15 @@
 Requires-Dist: aiobotocore[boto3] (>=2.5.0,<2.6.0)
 Requires-Dist: aioconsole (>=0.6.1,<0.7.0)
 Requires-Dist: aiohttp_cors (>=0.7.0,<0.8.0)
 Requires-Dist: colorlog (>=6.6.0,<7.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: prometheus-async (>=22.1.0,<23.0.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: python-json-logger (>=2.0.2,<3.0.0)
 Requires-Dist: python-slugify[unidecode] (>=8.0.1,<9.0.0)
 Requires-Dist: redis (>=4.4.0,<5.0.0)
 Requires-Dist: s3fs (>=2023.5.0,<2024.0.0)
 Requires-Dist: ujson (>=5.1.0,<6.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Project-URL: Issues, https://github.com/quantmind/aio-fluid/issues
@@ -44,14 +45,15 @@
 
 # Tools for backend python services
 
 [![PyPI version](https://badge.fury.io/py/aio-fluid.svg)](https://badge.fury.io/py/aio-fluid)
 [![Python versions](https://img.shields.io/pypi/pyversions/aio-fluid.svg)](https://pypi.org/project/aio-fluid)
 [![build](https://github.com/quantmind/fluid/workflows/build/badge.svg)](https://github.com/quantmind/aio-fluid/actions?query=workflow%3Abuild)
 [![codecov](https://codecov.io/gh/quantmind/aio-fluid/branch/main/graph/badge.svg?token=81oWUoyEVp)](https://codecov.io/gh/quantmind/aio-fluid)
+[![Downloads](https://img.shields.io/pypi/dd/aio-fluid.svg)](https://pypi.org/project/aio-fluid/)
 
 ## Installation
 
 This is a simple python package you can install via pip:
 
 ```
 pip install aio-fluid
```

