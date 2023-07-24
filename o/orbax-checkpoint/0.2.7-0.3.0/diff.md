# Comparing `tmp/orbax_checkpoint-0.2.7.tar.gz` & `tmp/orbax_checkpoint-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax_checkpoint-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orbax_checkpoint-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax_checkpoint-0.2.7.tar` & `orbax_checkpoint-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0    11357 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/LICENSE
--rw-r--r--   0        0        0      834 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/README.md
--rw-r--r--   0        0        0     2728 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     3106 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5727 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4744 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    36438 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0    15072 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0    11915 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4022 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1576 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     2002 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7672 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0    45137 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0      757 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/proto/__init__.py
--rw-r--r--   0        0        0      757 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/proto/testing/__init__.py
--rw-r--r--   0        0        0      136 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/proto/testing/foo.proto
--rw-r--r--   0        0        0     1549 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/proto/testing/foo_pb2.py
--rw-r--r--   0        0        0     2279 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/proto_checkpoint_handler.py
--rw-r--r--   0        0        0     2098 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/proto_checkpoint_handler_test.py
--rw-r--r--   0        0        0    25974 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5333 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0    11807 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    15155 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    23190 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    23650 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     7465 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1153 2023-06-28 23:19:11.678790 orbax_checkpoint-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 orbax_checkpoint-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/LICENSE
+-rw-r--r--   0        0        0      834 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/README.md
+-rw-r--r--   0        0        0     2960 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2663 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2832 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5932 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     5692 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2188 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    37382 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0    15104 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0    11915 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4839 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1576 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     2002 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/lazy_utils.py
+-rw-r--r--   0        0        0     7672 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0    45194 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0      757 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/__init__.py
+-rw-r--r--   0        0        0      757 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/__init__.py
+-rw-r--r--   0        0        0      147 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/foo.proto
+-rw-r--r--   0        0        0     1644 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/foo_pb2.py
+-rw-r--r--   0        0        0     1173 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/tree_metadata.proto
+-rw-r--r--   0        0        0     2814 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/tree_metadata_pb2.py
+-rw-r--r--   0        0        0     3016 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto_checkpoint_handler.py
+-rw-r--r--   0        0        0     2108 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto_checkpoint_handler_test.py
+-rw-r--r--   0        0        0    33472 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5328 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0    11807 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    15155 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    26140 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    25612 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     8158 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1153 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 orbax_checkpoint-0.3.0/PKG-INFO
```

### Comparing `orbax_checkpoint-0.2.7/LICENSE` & `orbax_checkpoint-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/README.md` & `orbax_checkpoint-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/__init__.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,43 +10,48 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Defines exported symbols for the namespace package `orbax.checkpoint`."""
 
+import contextlib
 import functools
 
 from orbax.checkpoint import aggregate_handlers
 from orbax.checkpoint import checkpoint_utils
 from orbax.checkpoint import lazy_utils
 from orbax.checkpoint import msgpack_utils
 from orbax.checkpoint import test_utils
 from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 from orbax.checkpoint.abstract_checkpointer import AbstractCheckpointer
 from orbax.checkpoint.array_checkpoint_handler import ArrayCheckpointHandler
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
+from orbax.checkpoint.async_checkpointer import async_checkpointer_context
 from orbax.checkpoint.async_checkpointer import AsyncCheckpointer
 from orbax.checkpoint.checkpoint_handler import CheckpointHandler
+from orbax.checkpoint.checkpoint_manager import checkpoint_manager_context
 from orbax.checkpoint.checkpoint_manager import CheckpointManager
 from orbax.checkpoint.checkpoint_manager import CheckpointManagerOptions
 from orbax.checkpoint.checkpointer import Checkpointer
+from orbax.checkpoint.checkpointer import checkpointer_context
 from orbax.checkpoint.future import Future
 from orbax.checkpoint.json_checkpoint_handler import JsonCheckpointHandler
 from orbax.checkpoint.pytree_checkpoint_handler import ArrayRestoreArgs
 from orbax.checkpoint.pytree_checkpoint_handler import PyTreeCheckpointHandler
 from orbax.checkpoint.pytree_checkpoint_handler import RestoreArgs
 from orbax.checkpoint.pytree_checkpoint_handler import SaveArgs
 from orbax.checkpoint.transform_utils import apply_transformations
 from orbax.checkpoint.transform_utils import merge_trees
 from orbax.checkpoint.transform_utils import RestoreTransform
 from orbax.checkpoint.transform_utils import Transform
 
+
 try:
   __IPYTHON__
   _in_ipython_session = True
 except NameError:
   _in_ipython_session = False
 if _in_ipython_session:
   import nest_asyncio
@@ -55,8 +60,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.2.7'
+__version__ = '0.3.0'
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/abstract_checkpointer.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/abstract_checkpointer.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,7 +75,11 @@
       directory: a path to a saved checkpoint.
 
     Returns:
       the object structure or None, if the underlying handler does not implement
       `structure`.
     """
     pass
+
+  def close(self):
+    """Closes the Checkpointer."""
+    pass
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/aggregate_handlers.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/aggregate_handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,14 +47,19 @@
     pass
 
   @abc.abstractmethod
   def deserialize(self, path: epath.Path) -> PyTree:
     """Reads and deserializes a PyTree from the given directory."""
     pass
 
+  @abc.abstractmethod
+  def close(self):
+    """Closes the handler."""
+    pass
+
 
 class MsgpackHandler(AggregateHandler):
   """An implementation of AggregateHandler that uses msgpack to store the tree.
   """
 
   def __init__(self):
     self._executor = futures.ThreadPoolExecutor(max_workers=1)
@@ -79,24 +84,10 @@
     """See superclass documentation."""
     if path.exists():
       msgpack = path.read_bytes()
       return msgpack_utils.msgpack_restore(msgpack)
     else:
       raise FileNotFoundError(f'Checkpoint does not exist at {path}.')
 
-
-_AGGREGATE_HANDLER = None
-_DEFAULT_AGGREGATE_HANDLER = MsgpackHandler()
-
-
-def set_default_aggregate_handler(handler: AggregateHandler):
-  """Sets the default AggregateHandler for use by PyTreeCheckpointHandler.
-
-  Args:
-    handler: an AggregateHandler implementation.
-  """
-  global _AGGREGATE_HANDLER
-  _AGGREGATE_HANDLER = handler
-
-
-def get_aggregate_handler() -> AggregateHandler:
-  return _AGGREGATE_HANDLER or _DEFAULT_AGGREGATE_HANDLER
+  def close(self):
+    """See superclass documentation."""
+    self._executor.shutdown()
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/array_checkpoint_handler.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     Args:
       checkpoint_name: Provides a name for the directory under which Tensorstore
         files will be saved. Defaults to 'checkpoint'.
     """
     if not checkpoint_name:
       checkpoint_name = 'checkpoint'
     self._checkpoint_name = checkpoint_name
+    self._aggregate_handler = aggregate_handlers.MsgpackHandler()
 
   def _is_supported_type(self, item: ArrayType) -> bool:
     return isinstance(item, (np.ndarray, jax.Array)) or utils.is_scalar(item)
 
   async def async_save(
       self,
       directory: epath.Path,
@@ -63,28 +64,30 @@
 
     Returns:
       A list of commit futures which can be run to complete the save.
     """
     if not self._is_supported_type(item):
       raise TypeError(f'Unsupported type: {type(item)}.')
 
-    if save_args and save_args.aggregate:
-      aggregate_handler = aggregate_handlers.get_aggregate_handler()
-      await aggregate_handler.serialize(
-          directory / self._checkpoint_name, {_ELEMENT_KEY: item}
-      )
-      return []
+    if not save_args:
+      save_args = type_handlers.SaveArgs()
+    if save_args.aggregate:
+      return [
+          await self._aggregate_handler.serialize(
+              directory / self._checkpoint_name, {_ELEMENT_KEY: item}
+          )
+      ]
 
     info = type_handlers.ParamInfo(
         name=self._checkpoint_name,
         path=directory / self._checkpoint_name,
-        aggregate=False,
     )
     type_handler = type_handlers.get_type_handler(type(item))
-    return await type_handler.serialize(item, info, args=save_args)
+    futures = await type_handler.serialize([item], [info], args=[save_args])
+    return list(futures)
 
   def save(self, directory: epath.Path, item: ArrayType, *args, **kwargs):
     """Saves the provided item.
 
     Blocks until both copy and commit complete.
 
     See async_save.
@@ -129,16 +132,17 @@
       restore_args = type_handlers.RestoreArgs()
     if restore_args.lazy:
       raise ValueError(
           'Lazy restoration not supported for ArrayCheckpointHandler.'
       )
 
     if (directory / self._checkpoint_name).is_file():
-      aggregate_handler = aggregate_handlers.get_aggregate_handler()
-      result = aggregate_handler.deserialize(directory / self._checkpoint_name)
+      result = self._aggregate_handler.deserialize(
+          directory / self._checkpoint_name
+      )
       result = result[_ELEMENT_KEY]
       if not self._is_supported_type(result):
         raise TypeError(f'Unsupported type: {type(result)}.')
       if isinstance(restore_args, type_handlers.ArrayRestoreArgs):
         result = result.reshape(restore_args.global_shape)
         sharding = restore_args.sharding or jax.sharding.NamedSharding(
             restore_args.mesh, restore_args.mesh_axes
@@ -146,19 +150,26 @@
         result = jax.make_array_from_callback(
             result.shape, sharding, lambda idx: result[idx]
         )
     else:
       info = type_handlers.ParamInfo(
           name=self._checkpoint_name,
           path=directory / self._checkpoint_name,
-          aggregate=False,
+          skip_deserialize=False,
       )
       type_handler = type_handlers.get_type_handler(restore_args.restore_type)
-      result = asyncio.run(type_handler.deserialize(info, args=restore_args))
+      result = asyncio.run(
+          type_handler.deserialize([info], args=[restore_args])
+      )[0]
 
     utils.sync_global_devices('ArrayCheckpointHandler:restore')
     return result
 
   def structure(self, directory: epath.Path) -> ArrayType:
+    """See superclass documentation."""
     raise NotImplementedError(
         'Unsupported method `structure` for ArrayCheckpointHandler.'
     )
+
+  def close(self):
+    """See superclass documentation."""
+    self._aggregate_handler.close()
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/async_checkpoint_handler.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/async_checkpointer.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/async_checkpointer.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """AsyncCheckpointer."""
 
 import asyncio
+import contextlib
 import functools
 import time
 from typing import Any, Optional
 
 from absl import logging
 from etils import epath
 import jax
@@ -46,17 +47,23 @@
   provided by AsyncManager). Users should call `wait_until_finished` to block
   until a save operation running in the background is complete.
 
   Like its parent, AsyncCheckpointer also makes use of an underlying
   CheckpointHandler to deal with type-specific logic.
   """
 
-  def __init__(self, handler: AsyncCheckpointHandler, timeout_secs: int = 300):
+  def __init__(
+      self,
+      handler: AsyncCheckpointHandler,
+      timeout_secs: int = 300,
+      primary_host: int = 0,
+  ):
     jax.monitoring.record_event('/jax/orbax/async_checkpointer/init')
     self._handler = handler
+    self._primary_host = primary_host
     AsyncManager.__init__(self, timeout_secs=timeout_secs)
 
   def save(self,
            directory: epath.PathLike,
            item: Any,
            *args,
            force: bool = False,
@@ -86,20 +93,22 @@
     directory = epath.Path(directory)
     logging.info('Saving item to %s. Waiting for thread to finish save.',
                  directory)
     self.wait_until_finished()
 
     if directory.exists():
       if force:
-        if jax.process_index() == 0:
+        if jax.process_index() == self._primary_host:
           logging.info('Specified `force`: removing existing directory.')
           directory.rmtree()  # Post-sync handled by create_tmp_directory.
       else:
         raise ValueError(f'Destination {directory} already exists.')
-    tmpdir = utils.create_tmp_directory(directory)
+    tmpdir = utils.create_tmp_directory(
+        directory, primary_host=self._primary_host
+    )
 
     # Run copy ops.
     commit_ops = asyncio.run(
         self._handler.async_save(tmpdir, item, *args, **kwargs))
     commit_ops, _ = jax.tree_util.tree_flatten(commit_ops)
     commit_ops = [op for op in commit_ops if op is not None]
 
@@ -116,7 +125,39 @@
               directory: epath.PathLike,
               *args,
               item: Optional[Any] = None,
               **kwargs) -> Any:
     """See superclass documentation."""
     self.wait_until_finished()
     return super().restore(directory, *args, item=item, **kwargs)
+
+  def close(self):
+    """Waits to finish any outstanding operations before closing."""
+    self.wait_until_finished()
+    super().close()
+
+
+@contextlib.contextmanager
+def async_checkpointer_context(*args, **kwargs):
+  """Context manager for AsyncCheckpointer.
+
+  Initializes AsyncCheckpointer and closes the object when the context is
+  exited.
+
+  Usage::
+    with async_checkpointer_context(PyTreeCheckpointHandler()) as ckptr:
+      ckptr.save(...)
+      ckptr.wait_until_finished()
+      ckptr.restore(...)
+
+  Args:
+    *args: Arguments to initialize AsyncCheckpointer.
+    **kwargs: Keyword arguments to initialize AsyncCheckpointer.
+
+  Yields:
+    AsyncCheckpointer
+  """
+  ckptr = AsyncCheckpointer(*args, **kwargs)
+  try:
+    yield ckptr
+  finally:
+    ckptr.close()
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/checkpoint_handler.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,7 +67,11 @@
     Args:
       directory: the directory where the checkpoint is located.
 
     Returns:
       item structure
     """
     pass
+
+  def close(self):
+    """Closes the CheckpointHandler."""
+    pass
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/checkpoint_manager.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A class providing functionalities for managing multiple checkpoints."""
 
 import asyncio
+import concurrent.futures
+import contextlib
 import dataclasses
 import datetime
 import threading
 from typing import Any, Callable, Container, List, Mapping, Optional, Sequence, Tuple, Union
 import uuid
 
 from absl import logging
@@ -688,34 +690,30 @@
     Returns:
       a list of CheckpointInfo, sorted by increasing step.
     """
     steps = sorted(self.all_steps(read=True))
     if not steps:
       return []
 
-    tz = datetime.timezone.utc
-    times = [
-        datetime.datetime.fromtimestamp(
-            self._get_save_directory(step, self.directory).stat().mtime, tz=tz)
-        for step in steps
-    ]
+    def checkpoint_info(step: int) -> CheckpointInfo:
+      time = datetime.datetime.fromtimestamp(
+          self._get_save_directory(step, self.directory).stat().mtime,
+          tz=datetime.timezone.utc,
+      )
 
-    def get_metrics(step):
+      metrics = None
       if self._track_best:
         restored = self._restore_impl(step, {METRIC_ITEM_NAME: None}, {})
         if METRIC_ITEM_NAME in restored:
-          return restored[METRIC_ITEM_NAME]
-      return None
+          metrics = restored[METRIC_ITEM_NAME]
+      return CheckpointInfo(step=step, time=time, metrics=metrics)
 
-    metrics = [get_metrics(step) for step in steps]
-
-    return [
-        CheckpointInfo(step=s, time=t, metrics=m)
-        for s, t, m in zip(steps, times, metrics)
-    ]
+    with concurrent.futures.ThreadPoolExecutor() as executor:
+      futures = {step: executor.submit(checkpoint_info, step) for step in steps}
+      return [futures[step].result() for step in steps]
 
   def _get_interval_preserved_checkpoints(
       self, checkpoints: List[CheckpointInfo]
   ) -> List[CheckpointInfo]:
     """Gets which checkpoints should be kept based on keep_time_interval."""
     if not checkpoints:
       return []
@@ -967,7 +965,40 @@
 
   def _finalize(self, temp_ckpt_dir: epath.Path):
     """Cleans up old checkpoints and synchronizes hosts."""
     if not self._all_checkpointers_are_sync:
       self.wait_until_finished(join_finalize_thread=False)
     final_ckpt_dir = self._finalize_checkpoint(temp_ckpt_dir)
     self._remove_old_checkpoints()
+
+  def close(self):
+    """Waits for outstanding operations to finish and closes Checkpointers."""
+    self.wait_until_finished()
+    for c in self._checkpointers.values():
+      c.close()
+
+
+@contextlib.contextmanager
+def checkpoint_manager_context(*args, **kwargs):
+  """Context manager for CheckpointManager.
+
+  Initializes CheckpointManager and closes the object when the context is
+  exited.
+
+  Args:
+    *args: Arguments to initialize CheckpointManager.
+    **kwargs: Keyword arguments to initialize CheckpointManager.
+
+  Usage::
+    with checkpoint_manager_context(
+        directory, checkpointers, options) as mngr:
+      mngr.save(...)
+      mngr.all_steps()
+
+  Yields:
+    CheckpointManager
+  """
+  manager = CheckpointManager(*args, **kwargs)
+  try:
+    yield manager
+  finally:
+    manager.close()
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/checkpoint_utils.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
   logging.info(log_str)
   result = -1
   if jax.process_index() == 0:
     while True:
       if not checkpoint_dir.exists():
         if _sleep_and_maybe_exit():
           break
+        continue  # continue waiting until directory creation or timeout.
       steps = utils.checkpoint_steps(checkpoint_dir)
       checkpoint_step = max(steps) if steps else None
       if _reached_desired_step(checkpoint_step, until_step):
         if not _lock_checkpoint(
             checkpoint_dir,
             checkpoint_step,
             step_prefix,
@@ -147,20 +148,20 @@
         ):
           continue
         result = checkpoint_step
         break
       else:
         if _sleep_and_maybe_exit():
           break
-
+  result = multihost_utils.broadcast_one_to_all(np.int32(result)).item()
   wait_duration = time.time() - start
   jax.monitoring.record_event_duration_secs(
       '/jax/orbax/checkpoint_utils/wait_duration', wait_duration
   )
-  result = multihost_utils.broadcast_one_to_all(np.int32(result)).item()
+
   if result == -1:
     logging.info('Timed out waiting for new checkpoint. Returning -1.')
   else:
     logging.info('Found new checkpoint step: %d.', result)
   return result
 
 
@@ -190,15 +191,14 @@
     step_prefix: A prefix applied to step numbers (e.g. <prefix>_42).
     step_format_fixed_length: Expects to find checkpoint step directories with
       exactly this number of digits (leading zeros if necessary).
 
   Yields:
     a new checkpoint step, or -1 if the timeout was reached.
   """
-  logging.info('wait_for_new_checkpoint')
   step = _wait_for_new_checkpoint(
       checkpoint_dir,
       until_step=until_step,
       seconds_to_sleep=seconds_to_sleep,
       timeout=timeout,
       step_prefix=step_prefix,
       step_format_fixed_length=step_format_fixed_length,
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/checkpoint_utils_test.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/conftest.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/future.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/json_checkpoint_handler.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/lazy_utils.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/msgpack_utils.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/msgpack_utils_test.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax_checkpoint-0.3.0/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998946784922395%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(2, "axes = PartitionSpec(\'data\',)\\n"), (3, \'sharding '*

 * *            "= jax.sharding.NamedSharding(mesh, axes)')], delete: [2]}}, 13: {'source': {insert: "*

 * *            "[(12, '  create_sharded_array = pjit(lambda x: x, in_shardings=None, "*

 * *            "out_shardings=sharding)\\n')], delete: [12]}}}"}*

```diff
@@ -70,15 +70,16 @@
             "metadata": {
                 "id": "j8Sfk7-bab2_"
             },
             "outputs": [],
             "source": [
                 "devices = np.asarray(jax.devices())\n",
                 "mesh = Mesh(devices, ('data',))\n",
-                "axes = PartitionSpec('data',)"
+                "axes = PartitionSpec('data',)\n",
+                "sharding = jax.sharding.NamedSharding(mesh, axes)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "8Y1tG-q2agTf"
@@ -171,15 +172,15 @@
                 "      },\n",
                 "      'layer_1': {\n",
                 "          'bias': np.zeros(8),\n",
                 "          'kernel': np.arange(8),\n",
                 "      },\n",
                 "  }\n",
                 "\n",
-                "  create_sharded_array = pjit(lambda x: x, in_axis_resources=None, out_axis_resources=axes)\n",
+                "  create_sharded_array = pjit(lambda x: x, in_shardings=None, out_shardings=sharding)\n",
                 "  with Mesh(mesh.devices, mesh.axis_names):\n",
                 "    state = jax.tree_map(create_sharded_array, state)\n",
                 "\n",
                 "  state['step'] = 0\n",
                 "  return state\n",
                 "\n",
                 "def state_shape(state):\n",
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/proto/__init__.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/proto/testing/__init__.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/proto/testing/foo_pb2.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/foo_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\tfoo.proto\x12\x05orbax"\x1f\n\x03\x46oo\x12\x0b\n\x03\x62\x61r\x18\x01'
-    b' \x01(\t\x12\x0b\n\x03\x62\x61z\x18\x02 \x01(\x05'
+    b'\n\tfoo.proto\x12\x10orbax.checkpoint"9\n\x03\x46oo\x12\x10\n\x03\x62\x61r\x18\x01'
+    b' \x01(\tH\x00\x88\x01\x01\x12\x10\n\x03\x62\x61z\x18\x02'
+    b' \x01(\x05H\x01\x88\x01\x01\x42\x06\n\x04_barB\x06\n\x04_bazb\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'foo_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
+
   DESCRIPTOR._options = None
-  _FOO._serialized_start = 20
-  _FOO._serialized_end = 51
+  _FOO._serialized_start = 31
+  _FOO._serialized_end = 88
 # @@protoc_insertion_point(module_scope)
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/proto_checkpoint_handler.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/proto_checkpoint_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,45 +13,70 @@
 # limitations under the License.
 
 """ProtoCheckpointHandler class.
 
 Implementation of CheckpointHandler interface.
 """
 
-from typing import Any, Optional, Type
+import asyncio
+from concurrent import futures
+import functools
+from typing import Any, List, Optional, Type
 
 from etils import epath
 from google.protobuf import message
 from google.protobuf import text_format
 import jax
-from orbax.checkpoint import checkpoint_handler
+from orbax.checkpoint import async_checkpoint_handler
+from orbax.checkpoint import future
 from orbax.checkpoint import utils
 
 
-class ProtoCheckpointHandler(checkpoint_handler.CheckpointHandler):
+class ProtoCheckpointHandler(async_checkpoint_handler.AsyncCheckpointHandler):
   """Serializes/deserializes protocol buffers."""
 
   def __init__(self, filename: str):
     """Initializes ProtoCheckpointHandler.
 
     Args:
       filename: file name given to the written file.
     """
     self._filename = filename
+    self._executor = futures.ThreadPoolExecutor(max_workers=1)
 
-  def save(self, directory: epath.Path, item: message.Message):
+  async def async_save(
+      self, directory: epath.Path, item: message.Message
+  ) -> List[future.Future]:
     """Saves the given proto.
 
     Args:
       directory: save location directory.
       item: the proto to serialize.
+
+    Returns:
+      A commit future.
     """
-    if jax.process_index() == 0:
-      path = directory / self._filename
-      path.write_text(text_format.MessageToString(item))
+
+    def _save_fn(x):
+      if jax.process_index() == 0:
+        path = directory / self._filename
+        return path.write_text(text_format.MessageToString(x))
+      return 0
+
+    return [self._executor.submit(functools.partial(_save_fn, item))]
+
+  def save(self, directory: epath.Path, item: message.Message):
+    """Saves the provided item."""
+
+    async def async_save(directory, item):
+      commit_futures = await self.async_save(directory, item)
+      for f in commit_futures:
+        f.result()
+
+    asyncio.run(async_save(directory, item))
     utils.sync_global_devices("ProtoCheckpointHandler:save")
 
   def restore(
       self, directory: epath.Path, item: Optional[Type[message.Message]] = None
   ):
     """Restores the proto from directory.
 
@@ -69,7 +94,10 @@
       )
     path = directory / self._filename
     return text_format.Parse(path.read_text(), item())
 
   def structure(self, directory: epath.Path) -> Any:
     """Unimplemented. See parent class."""
     return NotImplementedError
+
+  def close(self):
+    self._executor.shutdown()
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/proto_checkpoint_handler_test.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/proto_checkpoint_handler_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,31 +36,33 @@
     super().setUp()
     self.directory = epath.Path(
         self.create_tempdir(name='checkpointing_test').full_path
     )
 
   def test_save_restore(self):
     item = foo_pb2.Foo(bar='some_str', baz=32)
-    checkpointer = ProtoCheckpointHandler(filename='some_filename')
-    checkpointer.save(self.directory, item)
-    restored = checkpointer.restore(self.directory, foo_pb2.Foo)
+    handler = ProtoCheckpointHandler(filename='some_filename')
+    handler.save(self.directory, item)
+    restored = handler.restore(self.directory, foo_pb2.Foo)
     self.assertEqual(item, restored)
     self.assertTrue((self.directory / 'some_filename').exists())
+    handler.close()
 
   def test_restore_with_none_item_throws_error(self):
     item = foo_pb2.Foo(bar='some_str', baz=32)
-    checkpointer = ProtoCheckpointHandler(filename='some_filename')
-    checkpointer.save(self.directory, item)
+    handler = ProtoCheckpointHandler(filename='some_filename')
+    handler.save(self.directory, item)
 
     with self.assertRaisesRegex(
         ValueError,
         (
             'Must provide `item` in order to deserialize proto to the correct'
             ' type.'
         ),
     ):
       # Call restore without passing the proto class.
-      checkpointer.restore(self.directory)
+      handler.restore(self.directory)
+    handler.close()
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,47 +15,51 @@
 """PyTreeCheckpointHandler class.
 
 Implementation of CheckpointHandler interface.
 """
 
 import asyncio
 import dataclasses
-import functools
 import re
-from typing import Any, Callable, List, Optional, Tuple, Union
+import typing
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental.array_serialization import serialization
 import numpy as np
 from orbax.checkpoint import aggregate_handlers
 from orbax.checkpoint import lazy_utils
+from orbax.checkpoint import proto_checkpoint_handler
 from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
 from orbax.checkpoint.future import Future
+from orbax.checkpoint.proto import tree_metadata_pb2
 import tensorstore as ts
 
 
 PyTree = Any
+TupleKey = Tuple[str, ...]
 RestoreArgs = type_handlers.RestoreArgs
 ArrayRestoreArgs = type_handlers.ArrayRestoreArgs
 SaveArgs = type_handlers.SaveArgs
 ParamInfo = type_handlers.ParamInfo
 TypeHandler = type_handlers.TypeHandler
 AggregateHandler = aggregate_handlers.AggregateHandler
 MsgpackHandler = aggregate_handlers.MsgpackHandler
 TransformFn = Callable[[PyTree, PyTree, PyTree], Tuple[PyTree, PyTree]]
 Transform = transform_utils.Transform
 RestoreTransform = transform_utils.RestoreTransform
 LazyValue = lazy_utils.LazyValue
+ProtoCheckpointHandler = proto_checkpoint_handler.ProtoCheckpointHandler
 
-_TYPE_METADATA_FILE = 'type_metadata'
+_METADATA_FILE = 'tree_metadata'
 _CHECKPOINT_FILE = 'checkpoint'
 
 
 async def _create_param_save_dir(param_info: ParamInfo, args: SaveArgs):
   # Directory will be unused.
   path = param_info.path
   if path is None or args.aggregate:
@@ -90,15 +94,15 @@
     else:
       if hasattr(arr, 'astype'):
         arr = arr.astype(dtype)
   return arr
 
 
 def _maybe_shard_array(value, args):
-  if isinstance(args, ArrayRestoreArgs):
+  if hasattr(value, 'reshape') and isinstance(args, ArrayRestoreArgs):
     value = value.reshape(args.global_shape)
     sharding = args.sharding or jax.sharding.NamedSharding(
         args.mesh, args.mesh_axes
     )
     value = jax.make_array_from_callback(
         value.shape, sharding, lambda idx: value[idx]
     )
@@ -113,21 +117,140 @@
   return jax.tree_util.tree_map_with_path(
       lambda kp, _: _param_name_from_keypath(kp),
       item,
       is_leaf=utils.is_empty_or_leaf,
   )
 
 
-def _get_param_infos_from_structure(directory: epath.Path,
-                                    structure: PyTree) -> PyTree:
-  """Construct ParamInfos based on a PyTree."""
-  names = _get_param_names(structure)
+def _keystr(key: Tuple[Any, ...]) -> str:
+  return '/'.join(key)
+
+
+def _find_matching_input_args(
+    input_key: TupleKey,
+    flat_item: Dict[TupleKey, Any],
+    flat_transforms: Dict[TupleKey, Transform],
+    flat_restore_args: Dict[TupleKey, RestoreArgs],
+) -> Optional[RestoreArgs]:
+  """Given an input_key, tries to find matching RestoreArgs for the input.
+  
+  Args:
+    input_key: A key in the input tree.
+    flat_item: The flattened, user-provided item.
+    flat_transforms: Flattened transformations dict.
+    flat_restore_args: Flattened tree of RestoreArgs, relative to item.
+    
+  Returns:
+    RestoreArgs that match the given input_key, according to the
+    transformations, or None if no match is found.
+  """
+  for transform_key, transform in flat_transforms.items():
+    if transform.multi_value_fn is not None:
+      if not isinstance(transform, RestoreTransform):
+        raise ValueError(
+            'Must use RestoreTransform in order to use multi_value_fn'
+            ' during restore.'
+        )
+      if transform.multi_value_fn_input_args is None:
+        raise ValueError(
+            '`multi_value_fn` was specified, but'
+            ' `multi_value_fn_input_args` were not. The latter must be'
+            ' specified to identify inputs for the function.'
+        )
+      for (
+          input_key_regex,
+          input_args,
+      ) in transform.multi_value_fn_input_args.items():
+        if re.fullmatch(input_key_regex, _keystr(input_key)):
+          return input_args
+    elif not transform.use_fallback:
+      # The following is done to reverse-engineer the regex for the key in
+      # the original tree.
+      for output_key in flat_item:
+        match = re.fullmatch(_keystr(transform_key), _keystr(output_key))
+        if match:
+          if transform.original_key is None:
+            # If transform.original_key is not specified, this transform
+            # does not rename the original key. We can reuse the key from
+            # the item.
+            input_key_pattern = _keystr(output_key)
+          else:
+            input_key_pattern = match.expand(transform.original_key)
+          if input_key_pattern == _keystr(input_key):
+            return flat_restore_args[output_key]
+  return None
+
+
+def _has_use_fallback_transform(
+    input_key: TupleKey, flat_transforms: Dict[TupleKey, Transform]
+) -> bool:
+  result = False
+  for transform_key, transform in flat_transforms.items():
+    match = re.fullmatch(_keystr(transform_key), _keystr(input_key))
+    if match and transform.use_fallback:
+      result = True
+  return result
+
+
+def _get_restore_parameters(
+    directory: epath.Path,
+    item: Optional[PyTree],
+    structure: PyTree,
+    transforms: Optional[PyTree],
+    restore_args: Optional[PyTree],
+    byte_limiter: Optional[serialization._LimitInFlightBytes] = None,
+    transforms_default_to_original: bool = True,
+) -> Tuple[PyTree, PyTree]:
+  """Construct parameters needed for restoration.
+
+  If transforms are not provided, the method is pretty simple: param_infos are
+  constructed from the structure of the original checkpoint, and restore_args
+  are serialized to a tree structure compatible with param_infos and structure.
+
+  If transforms are provided, things become more complicated because we must
+  determine exactly which parameters the user desires to restore, and construct
+  param_infos and restore_args for these, while discarding unneeded parameters.
+  In essence, the process can be thought of as reversing the transformations.
+  This happens differently for different types of transforms.
+  1. Renamed key: Identify the original key name (in the checkpoint) and carry
+    over the provided restore args for the parameter.
+  2. multi_value_fn: Users are required to specify multi_value_fn_input_args.
+    Any keys named here must be loaded, and their restore args are also given
+    here.
+  3. Unspecified key: A key which is unspecified in the transforms but present
+    in the `item` is a key that is carried over from the checkpoint unchanged.
+  4. Fallback key: This is a key that is present in the `item` but not in the
+    original checkpoint. It does not need to be restored.
+  5. Keys present in the original checkpoint but not in the `item`/`transforms`
+    are implicitly ignored, and not restored.
+
+  Args:
+    directory: Checkpoint directory.
+    item: Optional reference item.
+    structure: The structure of the original checkpoint.
+    transforms: User-provided transformations. If None, they were not provided.
+      Has the structure of the desired output tree.
+    restore_args: User-provided restoration arguments. If None, they were not
+      provided. Otherwise, the tree has the same structure as the desired output
+      tree.
+    byte_limiter: A _LimitInFlightBytes object.
+    transforms_default_to_original: See transform_utils.apply_transformations.
+
+  Returns:
+    Tuple of param_infos, and restore_args.
+  """
+  flat_structure = utils.to_flat_dict(structure, keep_empty_nodes=True)
+  if restore_args is None:
+    restore_args = jax.tree_util.tree_map(lambda x: RestoreArgs(), structure)
+  flat_restore_args = utils.to_flat_dict(restore_args, keep_empty_nodes=True)
+  flat_param_infos = {}
+  flat_input_restore_args = {}
   is_ocdbt_checkpoint = type_handlers.is_ocdbt_checkpoint(directory)
 
-  def _get_param_info(name: str, leaf: Any) -> ParamInfo:
+  def _get_param_info(nested_name: Tuple[str, ...], leaf: Any) -> ParamInfo:
     if utils.leaf_is_placeholder(leaf):
       # Leaf is a param name.
       path = directory / utils.name_from_leaf_placeholder(leaf)
     # The following is kept for backwards compatibility.
     elif isinstance(leaf, ts.Spec):
       tspec = leaf.to_json()  # pytype: disable=attribute-error
       # Skip '.', since we need special regex handling for this char.
@@ -137,21 +260,82 @@
       return leaf  # Empty node, ParamInfo should not be returned.
     elif utils.is_supported_aggregation_type(leaf):
       # Value already restored, do not need ts.Spec.
       path = None
     else:
       raise ValueError(f'Unsupported type: {type(leaf)}')
     return ParamInfo(
-        name=name,
+        name='.'.join(nested_name),
         path=path,
-        aggregate=(path is None),
+        skip_deserialize=(path is None),
         is_ocdbt_checkpoint=is_ocdbt_checkpoint,
+        byte_limiter=byte_limiter,
     )
 
-  return jax.tree_util.tree_map(_get_param_info, names, structure)
+  if transforms is None:
+    for key, value in flat_structure.items():
+      flat_param_infos[key] = _get_param_info(key, value)
+    restore_args = utils.serialize_tree(restore_args, keep_empty_nodes=True)
+  else:
+    if item is None:
+      raise ValueError(
+          'If providing `transforms`, must provide `item` matching structure'
+          ' of expected result.'
+      )
+    flat_item = utils.to_flat_dict(item, keep_empty_nodes=True)
+    flat_transforms = utils.to_flat_dict(transforms)
+
+    for input_key, value in flat_structure.items():
+      maybe_input_args = _find_matching_input_args(
+          input_key, flat_item, flat_transforms, flat_restore_args
+      )
+      if maybe_input_args:
+        flat_param_infos[input_key] = _get_param_info(input_key, value)
+        flat_input_restore_args[input_key] = maybe_input_args
+      elif input_key in flat_item and input_key in flat_structure:
+        # Key is present in both input and output.
+        if _has_use_fallback_transform(input_key, flat_transforms):
+          # Indicates that a `use_fallback` transformation was specified.
+          if transforms_default_to_original:
+            # Specified `use_fallback`, but key was also present in the
+            # checkpoint. This means we should skip loading, since it will be
+            # overridden with a new value.
+            flat_param_infos[input_key] = ParamInfo(skip_deserialize=True)
+            flat_input_restore_args[input_key] = RestoreArgs()
+          else:
+            # Specified `use_fallback`, but `transforms_default_to_original`
+            # is False. This means we draw the value from the user-provided
+            # `item`.
+            flat_param_infos[input_key] = _get_param_info(input_key, value)
+            flat_input_restore_args[input_key] = flat_restore_args[input_key]
+        else:
+          # Transform not specified.
+          if transforms_default_to_original:
+            # Key/value is carried over from the original unchanged.
+            flat_param_infos[input_key] = _get_param_info(input_key, value)
+            flat_input_restore_args[input_key] = flat_restore_args[input_key]
+          else:
+            # Take the value from the user-provided `item`, ignoring any value
+            # in the checkpoint.
+            flat_param_infos[input_key] = ParamInfo(skip_deserialize=True)
+            flat_input_restore_args[input_key] = RestoreArgs()
+      else:
+        # No match, restoration not required since it will be dropped from the
+        # output.
+        flat_param_infos[input_key] = ParamInfo(skip_deserialize=True)
+        flat_input_restore_args[input_key] = RestoreArgs()
+
+    restore_args = utils.from_flat_dict(
+        flat_input_restore_args, target=structure
+    )
+
+  return (
+      utils.from_flat_dict(flat_param_infos, target=structure),
+      restore_args,
+  )
 
 
 def _get_tree_for_aggregation(param_infos, save_args, item):
   """Get tree for aggregated checkpoint."""
 
   # TODO(b/283164080): These type checks result in logic from the lower layer
   # (TypeHandler/AggregateHandler) leaking into the upper layer
@@ -173,26 +357,101 @@
       return utils.leaf_placeholder(param_info.name)
 
   return jax.tree_util.tree_map(
       _get_leaf_for_aggregation, param_infos, save_args, item
   )
 
 
+@dataclasses.dataclass
+class _BatchRequest:
+  """Represents a a request for batched serialization or deserialization."""
+  handler: TypeHandler
+  values: List[Any]
+  infos: List[ParamInfo]
+  args: List[Union[SaveArgs, RestoreArgs]]
+  lazy: bool = False
+
+
+def _batched_serialization_requests(
+    tree: PyTree, param_infos: PyTree, args: PyTree
+) -> List[_BatchRequest]:
+  """Gets a list of batched serialization or deserialization requests."""
+  result = []
+  grouped = {}
+
+  def _group_value(info, value, arg):
+    nonlocal result
+    nonlocal grouped
+    # Exclude from serialize/deserialize with TypeHandler if aggregated.
+    if info.skip_deserialize:
+      return
+    if isinstance(arg, RestoreArgs):
+      handler = type_handlers.get_type_handler(arg.restore_type)
+      # Lazy arguments must be restored individually, rather than as a batch.
+      # Thus, we create an individual _BatchRequest for each one.
+      if arg.lazy:
+        result += [_BatchRequest(handler, [value], [info], [arg], lazy=True)]
+        return
+    else:
+      handler = type_handlers.get_type_handler(type(value))
+    if handler not in grouped:
+      grouped[handler] = _BatchRequest(handler, [], [], [])
+    request = grouped[handler]
+    grouped[handler] = dataclasses.replace(
+        request,
+        values=request.values + [value],
+        infos=request.infos + [info],
+        args=request.args + [arg],
+    )
+
+  jax.tree_util.tree_map(
+      _group_value,
+      param_infos,
+      tree,
+      args,
+  )
+  return result + list(grouped.values())
+
+
+def _multi_value_fns_with_args(
+    transforms: PyTree, restore_args: PyTree
+) -> PyTree:
+  """Constructs a wrapper for multi_value_fn including RestoreArgs."""
+  flat_restore_args = utils.to_flat_dict(restore_args, sep='/')
+
+  def _maybe_wrap_transform(transform: Transform):
+    def _multi_value_fn_with_args(transform_key: str, tree: PyTree) -> Any:
+      nonlocal transform
+      transform = typing.cast(RestoreTransform, transform)
+      return transform.multi_value_fn(
+          transform_key, tree, flat_restore_args[transform_key]
+      )
+
+    if transform.multi_value_fn is not None:
+      return Transform(multi_value_fn=_multi_value_fn_with_args)
+    else:
+      return transform
+
+  return jax.tree_util.tree_map(_maybe_wrap_transform, transforms)
+
+
 def _transform_structure(
     item: PyTree,
     restored: PyTree,
+    restore_args: Optional[PyTree],
     transforms: Optional[PyTree],
     transforms_default_to_original: bool,
 ) -> PyTree:
   """Optionally transforms the restored PyTree to the structure of `item`.
 
   Args:
     item: a PyTree representing the result structure ("new tree structure").
     restored: a PyTree representing the original tree structure. Note: this is a
       tree of LazyValues.
+    restore_args: tree of RestoreArgs, with the same structure as `item`.
     transforms: provides instructions on how to transform the input trees. See
       transform_utils.
     transforms_default_to_original: See transform_utils.
 
   Returns:
     A transformed PyTree.
   """
@@ -202,169 +461,65 @@
              ' of expected result.')
       raise ValueError(msg)
     item = restored
   else:
     if transforms is None:
       item = utils.deserialize_tree(restored, item)
     else:
-      restored = _materialize_multi_value_fn_inputs(restored, transforms)
-      transforms = _construct_lazy_transform_wrappers(transforms)
+      if restore_args is None:
+        raise ValueError(
+            'If providing `transforms`, must provide `restore_args` matching'
+            ' structure of expected result.'
+        )
+      transforms = _multi_value_fns_with_args(transforms, restore_args)
       item = transform_utils.apply_transformations(
           restored, transforms, item, transforms_default_to_original)
   return item
 
 
-def _materialize_multi_value_fn_inputs(
-    tree: PyTree, transforms: PyTree
-) -> PyTree:
-  """Materializes values from tree which are marked as multi_value_fn inputs."""
-  flat_tree = utils.to_flat_dict(tree, sep='/')
-  flat_transforms = utils.to_flat_dict(transforms, sep='/')
-  keys = []
-  ops = []
-  for key, lazy_value in flat_tree.items():
-    assert isinstance(lazy_value, LazyValue)
-    for _, transform in flat_transforms.items():
-      if transform.multi_value_fn is not None:
-        if not isinstance(transform, RestoreTransform):
-          raise ValueError(
-              'Must use RestoreTransform in order to use multi_value_fn during'
-              ' restore.'
-          )
-        if transform.multi_value_fn_input_args is None:
-          raise ValueError(
-              '`multi_value_fn` was specified, but `multi_value_fn_input_args`'
-              ' were not. The latter must be specified to identify inputs for'
-              ' the function.'
-          )
-        for (
-            input_key,
-            restore_args,
-        ) in transform.multi_value_fn_input_args.items():
-          if re.fullmatch(input_key, key):
-            keys += [key]
-            ops += [lazy_value.get_async(args=restore_args)]
-
-  async def _await_in_parallel():
-    return await asyncio.gather(*ops)
-
-  values = asyncio.run(_await_in_parallel())
-  for key, value in zip(keys, values):
-    flat_tree[key] = value
-  return utils.from_flat_dict(flat_tree, target=tree, sep='/')
-
-
-def _construct_lazy_transform_wrappers(transforms: PyTree) -> PyTree:
-  """Constructs wrapper functions for user-provided to handle `LazyValue`.
-
-  User-provided value-based transformation functions are written in terms of
-  real values, not `LazyValue`. However, we want to be able to load all
-  parameters as `LazyValue`, so as to avoid materializing unneeded parameters
-  until necessary. As such, we construct wrapper functions which accept
-  `LazyValue` and materialize the value before providing it to the user-defined
-  function.
-
-  Note that because different multi_value_fn's may use the same leaves as
-  inputs, we could run into a situation where we restore the same value many
-  times and OOM. To fix this, _materialize_multi_value_fn_inputs must first be
-  called, so that some of the inputs to these wrapped functions will be
-  LazyValue, while others will be materialized, if marked as needed as an input
-  for a multi_value_fn transformation. As such, we do not need to wrap
-  the multi_value_fn transformations, since all inputs will already be
-  materialized.
-
-  Args:
-    transforms: User-provided tree of Transform objects.
-
-  Returns:
-    A tree of Transform objects which is roughly the same as the input, but
-    where all instances of `value_fn` are wrapped to accept
-    `LazyValue` as input and return `LazyValue` as output.
-  """
-
-  def _maybe_wrap_transform(transform: Transform):
-
-    async def _lazy_value_fn(maybe_lazy_value: Any, args: RestoreArgs) -> Any:
-      # `maybe_lazy_value` is the value over which the function is performed.
-      # It may be LazyValue or may already be materialized.
-      # `args` is `RestoreArgs`, which is used to materialize the value.
-      if isinstance(maybe_lazy_value, LazyValue):
-        value = await maybe_lazy_value.get_async(args=args)
-      else:
-        value = maybe_lazy_value
-      if isinstance(transform, RestoreTransform):
-        return transform.value_fn(value, args)
-      else:
-        return transform.value_fn(value)
-
-    async def _lazy_multi_value_fn(
-        transform_key: str, tree: PyTree, args: RestoreArgs
-    ) -> Any:
-      # Inputs are already materialized.
-      if isinstance(transform, RestoreTransform):
-        return transform.multi_value_fn(transform_key, tree, args)
-      else:
-        return transform.multi_value_fn(transform_key, tree)
-
-    def _wrap_as_lazy_value(func, *args, **kwargs):
-      return LazyValue(functools.partial(func, *args, **kwargs))
-
-    # Only needed values are carried over to the wrapped Transform.
-    if transform.value_fn is not None:
-      return Transform(
-          original_key=transform.original_key,
-          value_fn=functools.partial(_wrap_as_lazy_value, _lazy_value_fn),
-      )
-    elif transform.multi_value_fn is not None:
-      return Transform(
-          multi_value_fn=functools.partial(
-              _wrap_as_lazy_value, _lazy_multi_value_fn
-          )
-      )
-    else:
-      return transform
-
-  return jax.tree_util.tree_map(_maybe_wrap_transform, transforms)
-
-
 class PyTreeCheckpointHandler(AsyncCheckpointHandler):
   """A CheckpointHandler implementation for any PyTree structure.
 
   The PyTree is assumed to be a nested dictionary with array values represented
   as array-like objects (see type_handlers for supported objects). If not
   `jax.Array`, arrays are expected to be fully replicated.
   """
 
   def __init__(
       self,
       aggregate_filename: Optional[str] = None,
       concurrent_gb: int = 96,
       use_ocdbt: bool = False,
       restore_with_serialized_types: bool = True,
+      write_tree_metadata: bool = False,
   ):
     """Creates PyTreeCheckpointHandler.
 
     Args:
       aggregate_filename: name that the aggregated checkpoint should be saved
         as.
       concurrent_gb: max concurrent GB that are allowed to be read.
       use_ocdbt: enables Tensorstore OCDBT driver.
       restore_with_serialized_types: If True, the values with unspecified
         restore types will be restored using the typing information in the
         checkpoint. Otherwise, arrays will be restored as either np.ndarray or
         jax.Array, and will ignore any typing information present in the
         checkpoint.
+      write_tree_metadata: Experimental feature. Do not use. Writes tree
+        metadata in protobuf format.
     """
-    self._aggregate_handler = aggregate_handlers.get_aggregate_handler()
+    self._aggregate_handler = MsgpackHandler()
     if aggregate_filename is None:
       aggregate_filename = _CHECKPOINT_FILE
     self._aggregate_filename = aggregate_filename
     self._concurrent_gb = concurrent_gb
     self._use_ocdbt = use_ocdbt
     self._restore_with_serialized_types = restore_with_serialized_types
+    self._write_tree_metadata = write_tree_metadata
+    self._metadata_handler = ProtoCheckpointHandler(_METADATA_FILE)
 
   def _get_param_names(self, item: PyTree) -> PyTree:
     """Gets parameter names for PyTree elements."""
     return _get_param_names(item)
 
   def _get_param_infos(
       self, item: PyTree, directory: epath.Path, save_args: PyTree
@@ -389,15 +544,16 @@
     names = self._get_param_names(item)
     all_params_aggregated = True
 
     def _param_info(name, args):
       nonlocal all_params_aggregated
       all_params_aggregated &= args.aggregate
       return ParamInfo(
-          name=name, path=(directory / name), aggregate=args.aggregate)
+          name=name, path=(directory / name), skip_deserialize=args.aggregate
+      )
 
     return (
         jax.tree_util.tree_map(_param_info, names, save_args),
         all_params_aggregated,
     )
 
   async def _write_aggregate_file(
@@ -408,14 +564,51 @@
       save_args: PyTree,
   ) -> Future:
     ser_item = _get_tree_for_aggregation(param_infos, save_args, item)
     return await self._aggregate_handler.serialize(
         directory / self._aggregate_filename, ser_item
     )
 
+  async def _write_metadata_file(
+      self,
+      directory: epath.Path,
+      item: PyTree,
+  ) -> List[Future]:
+    if not self._write_tree_metadata:
+      return []
+    flat_with_keys, _ = jax.tree_util.tree_flatten_with_path(
+        item, is_leaf=utils.is_empty_or_leaf
+    )
+    tree_metadata = tree_metadata_pb2.TreeMetadata()
+    for keypath, _ in flat_with_keys:
+      kv = tree_metadata.structure.add()
+      for k in keypath:
+        proto_k = kv.key.add()
+        proto_k.name = str(utils.get_key_name(k))
+        proto_k.type = utils.get_key_metadata_type(k)
+      value_metadata = kv.value
+      # TODO(b/289245667): Placeholder value.
+      value_metadata.type = 'None'
+    return await self._metadata_handler.async_save(directory, tree_metadata)
+
+  def _read_metadata_file(
+      self,
+      directory: epath.Path,
+  ) -> PyTree:
+    tree_metadata = self._metadata_handler.restore(
+        directory, tree_metadata_pb2.TreeMetadata
+    )
+    tree_metadata = typing.cast(tree_metadata_pb2.TreeMetadata, tree_metadata)
+    flat = []
+    for kv_pair in tree_metadata.structure:
+      keys, value = (kv_pair.key, kv_pair.value)
+      keypath = tuple([utils.keypath_from_key_metadata(key) for key in keys])
+      flat.append((keypath, value))
+    return utils.from_flattened_with_keypath(flat)
+
   async def async_save(
       self,
       directory: epath.Path,
       item: PyTree,
       save_args: Optional[PyTree] = None) -> Optional[List[Future]]:
     """Saves a PyTree from a given training step.
 
@@ -461,40 +654,36 @@
               )
           )[0]
       )
       utils.sync_global_devices(
           'PyTreeCheckpointHandler:create_param_save_dirs'
       )
 
-    async def serialize(value, info, args):
-      if args.aggregate:
-        return  # skip serialize now, include in aggregated file
-      handler = type_handlers.get_type_handler(type(value))
-      return await handler.serialize(value, info, args)
-
     if all_params_aggregated:
       commit_futures = []
     else:
-      future_tree = jax.tree_util.tree_map(
-          serialize,
-          item,
-          param_infos,
-          save_args,
-          is_leaf=utils.is_empty_or_leaf,
+      serialize_ops = []
+      batch_requests = _batched_serialization_requests(
+          item, param_infos, save_args
       )
-      copy_futures, _ = jax.tree_util.tree_flatten(future_tree)
-      assert isinstance(copy_futures, list)
-      # Await copy futures.
-      commit_futures = await asyncio.gather(*copy_futures)
+      for request in batch_requests:
+        serialize_ops += [
+            request.handler.serialize(
+                request.values, request.infos, request.args
+            )
+        ]
+      # Await copy futures. Returns list of lists.
+      commit_futures = await asyncio.gather(*serialize_ops)
       commit_futures, _ = jax.tree_util.tree_flatten(commit_futures)
 
+    metadata_commit_futures = await self._write_metadata_file(directory, item)
     aggregate_commit_future = await self._write_aggregate_file(
         directory, item, param_infos, save_args
     )
-    return commit_futures + [aggregate_commit_future]
+    return commit_futures + [aggregate_commit_future] + metadata_commit_futures
 
   def save(self, directory: epath.Path, item: Any, *args, **kwargs):
     """Saves the provided item.
 
     Blocks until both copy and commit complete.
 
     See async_save.
@@ -513,48 +702,67 @@
       if commit_futures:  # May be None.
         for future in commit_futures:
           future.result()  # Block on result.
 
     asyncio.run(async_save(directory, item, *args, **kwargs))
     utils.sync_global_devices('PyTreeCheckpointHandler:save')
 
-  def _maybe_deserialize(self, param_info: ParamInfo, value: Any) -> LazyValue:
-    """Deserializes using handler or returns already restored value.
+  async def _maybe_deserialize(
+      self, structure: PyTree, param_infos: PyTree, restore_args: PyTree
+  ) -> PyTree:
+    """Deserializes values or gets them from the aggregate file."""
 
-    If the ParamInfo indicates that the parameter was aggregated, then it must
-    have already been restored. In this case, we simply perform a cast and
-    convert to LazyArray if requested.
+    # Handle parameters from aggregate file.
+    def _process_aggregated_value(info, value, args):
+      if info.skip_deserialize:
+        value = _try_array_cast(value, args.dtype)
+        value = _maybe_shard_array(value, args)
+      if args.lazy:
+        value = LazyValue(lazy_utils.identity(value))
+      return value
 
-    Otherwise, we deserialize using an appropriate TypeHandler, converting to
-    LazyArray and casting if requested.
+    def _lazy_get_fn(handler, infos, args):
+      async def _get_singular_value_from_handler():
+        result = await handler.deserialize(infos, args)
+        assert len(result) == 1
+        return result[0]
 
-    Args:
-      param_info: ParamInfo
-      value: a tree value which may have already been restored. Not relevant if
-        info.aggregate is False.
+      return _get_singular_value_from_handler
 
-    Returns:
-      A LazyValue.
-    """
+    structure = jax.tree_util.tree_map(
+        _process_aggregated_value, param_infos, structure, restore_args
+    )
 
-    async def _maybe_cast_and_shard(val: Any, args: RestoreArgs) -> Any:
-      val = _try_array_cast(val, args.dtype)
-      val = _maybe_shard_array(val, args)
-      return val
-
-    async def _deserialize(info: ParamInfo, args: RestoreArgs) -> Any:
-      handler = type_handlers.get_type_handler(args.restore_type)
-      return await handler.deserialize(info, args)
+    batch_requests = _batched_serialization_requests(
+        structure, param_infos, restore_args
+    )
+    deserialized_batches = []
+    deserialized_batches_ops = []
+    for request in batch_requests:
+      if request.lazy:
+        deserialized_batches.append(
+            [
+                LazyValue(
+                    _lazy_get_fn(request.handler, request.infos, request.args)
+                )
+            ]
+        )
+      else:
+        deserialized_batches_ops.append(
+            request.handler.deserialize(request.infos, request.args)
+        )
+    deserialized_batches += await asyncio.gather(*deserialized_batches_ops)
 
-    if param_info.aggregate:  # Already restored from AggregateHandler.
-      get_fn = functools.partial(_maybe_cast_and_shard, val=value)
-    else:
-      get_fn = functools.partial(_deserialize, info=param_info)
+    flat_restored = utils.to_flat_dict(structure, sep='.')
+    for request, deserialized in zip(batch_requests, deserialized_batches):
+      for info, value in zip(request.infos, deserialized):
+        flat_restored[info.name] = value
 
-    return LazyValue(get_fn)
+    restored = utils.from_flat_dict(flat_restored, target=structure, sep='.')
+    return restored
 
   def restore(
       self,
       directory: epath.Path,
       item: Optional[PyTree] = None,
       restore_args: Optional[PyTree] = None,
       transforms: Optional[PyTree] = None,
@@ -576,99 +784,76 @@
         restoration. It should be a PyTree matching the structure of `item`, and
         should contain a RestoreArgs object for every value. If `item` is not
         provided, should match the structure of the checkpoint.
       transforms: a PyTree of transformations that should be applied to the
         saved item in order to obtain a final structure. See `transform_utils`
         for further information.
       transforms_default_to_original: See transform_utils.apply_transformations.
-      transform_fn: A function which accepts the `item` argument, a PyTree
-        checkpoint structure and a PyTree of ParamInfos based on the checkpoint.
-        Returns a transformed PyTree matching the desired return tree structure,
-        and a matching ParamInfo tree.
+      transform_fn: WARNING: NOT GENERALLY SUPPORTED. A function which accepts
+        the `item` argument, a PyTree checkpoint structure and a PyTree of
+        ParamInfos based on the checkpoint. Returns a transformed PyTree
+        matching the desired return tree structure, and a matching ParamInfo
+        tree.
 
     Returns:
       A PyTree matching the structure of `item`. If `lazy` restoration is
       enabled, leaves will be returned as `LazyValue`.
 
     Raises:
       FileNotFoundError: `directory` does not exist or is missing required files
       ValueError: `transforms` is provided without `item`.
       ValueError: `transforms` contains elements with `multi_value_fn`.
     """
     if not directory.exists():
       raise FileNotFoundError(
           f'Requested directory for restore does not exist at {directory}')
 
-    structure = self.structure(directory)
-    param_infos = _get_param_infos_from_structure(directory, structure)
-
-    if transform_fn is not None and transforms is not None:
-      raise ValueError('Cannot provide both `transforms` and `transform_fn`.')
-    if transform_fn is not None:
-      structure, param_infos = transform_fn(item, structure, param_infos)
-
     async def _create_byte_limiter():
       # Wrap creation in async function to avoid issues on python<=3.9.
       concurrent_bytes = self._concurrent_gb * 10**9
       # Construction must take place here so that it is within the same async
       # method, to prevent errors resulting from different event loops, and
       # cannot be created below this level because there must be a single object
       # for the entire restore call.
       return serialization._LimitInFlightBytes(concurrent_bytes)  # pylint: disable=protected-access
 
     byte_limiter = asyncio.run(_create_byte_limiter())
-    param_infos = jax.tree_util.tree_map(
-        functools.partial(dataclasses.replace, byte_limiter=byte_limiter),
-        param_infos,
-    )
-    lazy_restored_item = jax.tree_util.tree_map(
-        self._maybe_deserialize,
-        param_infos,
+    structure = self.structure(directory)
+    # `checkpoint_restore_args` has a structure relative to the checkpoint,
+    # while `restore_args` remains structured relative to the output.
+    param_infos, checkpoint_restore_args = _get_restore_parameters(
+        directory,
+        item,
         structure,
+        transforms,
+        restore_args,
+        byte_limiter=byte_limiter,
+        transforms_default_to_original=transforms_default_to_original,
     )
 
-    if not transform_fn:
-      lazy_restored_item = _transform_structure(
-          item, lazy_restored_item, transforms, transforms_default_to_original
-      )
-
-    if restore_args is None:
-      restore_args = jax.tree_util.tree_map(
-          lambda x: RestoreArgs(),
-          item or structure,
-      )
+    if transform_fn is not None and transforms is not None:
+      raise ValueError('Cannot provide both `transforms` and `transform_fn`.')
+    if transform_fn is not None:
+      structure, param_infos = transform_fn(item, structure, param_infos)
+      if restore_args is None:
+        restore_args = jax.tree_util.tree_map(lambda x: RestoreArgs(), item)
+      checkpoint_restore_args = restore_args
 
-    def _maybe_get_materialization_function(
-        value: Union[LazyValue, Any], args: RestoreArgs
-    ) -> Any:
-      # Depending on the value of args.lazy, we either return a function that
-      # allows materializing the value, or return a function that returns
-      # another LazyValue, after passing in RestoreArgs.
-      if args.lazy:
-        if isinstance(value, LazyValue):
-          async_get_fn = functools.partial(value.get_async, args=args)
-        else:
-          async_get_fn = lazy_utils.identity(value)
-        return lazy_utils.identity(LazyValue(async_get_fn))()
-      else:
-        return lazy_utils.maybe_get_async(value, args=args)
+    restored_item = asyncio.run(
+        self._maybe_deserialize(structure, param_infos, checkpoint_restore_args)
+    )
 
-    async def _restore():
-      # Provide RestoreArgs now, since it was previously deferred.
-      flat, item_structure = jax.tree_util.tree_flatten(
-          jax.tree_util.tree_map(
-              _maybe_get_materialization_function,
-              lazy_restored_item,
-              restore_args,
-          )
+    if not transform_fn:
+      restored_item = _transform_structure(
+          item,
+          restored_item,
+          restore_args,
+          transforms,
+          transforms_default_to_original,
       )
-      flat = await asyncio.gather(*flat)
-      return jax.tree_util.tree_unflatten(item_structure, flat)
-
-    restored_item = asyncio.run(_restore())
     utils.sync_global_devices('PyTreeCheckpointHandler:restore')
     return restored_item
 
   def structure(self, directory: epath.Path) -> PyTree:
     """Restores the saved PyTree structure without regard for its leaf values.
 
     Args:
@@ -693,7 +878,12 @@
             (
                 'Checkpoint structure file does not exist at %s.'
                 ' Attempting to assume an implicit tree structure.'
             ),
             directory,
         )
         return utils.pytree_structure(directory)
+
+  def close(self):
+    """See superclass documentation."""
+    self._aggregate_handler.close()
+    self._metadata_handler.close()
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/test_utils.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   mesh = jax.sharding.Mesh(np.asarray(jax.devices()), ('x',))
   replicated_sharding = sharding.NamedSharding(
       mesh,
       jax.sharding.PartitionSpec(
           None,
       ),
   )
-  return pjit.pjit(lambda x: x, out_axis_resources=replicated_sharding)(arr)
+  return pjit.pjit(lambda x: x, out_shardings=replicated_sharding)(arr)
 
 
 def apply_function(tree, function):
   """Applies the given function to every leaf in tree.
 
   Args:
     tree: a nested dict where every leaf is a sharded jax.Array.
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/transform_utils.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/transform_utils_test.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/type_handlers.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/type_handlers.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Provides utils for PytreeCheckpointHandler."""
 
 import abc
+import asyncio
 import dataclasses
+import json
 import os
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union, cast
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental.array_serialization import serialization
 from jax.experimental.array_serialization.serialization import get_tensorstore_spec
 import jax.numpy as jnp
@@ -33,20 +35,16 @@
 
 
 Scalar = Union[int, float, np.number]
 _OCDBT_MANIFEST_FILE = 'manifest.ocdbt'
 _COORDINATOR_SETUP_TIMEOUT_SECS = 30
 
 
-def _get_coordinator_address_without_port(
-    coordinator_address: Optional[str],
-) -> str:
+def _get_coordinator_address_without_port(coordinator_address: str) -> str:
   """Returns JAX coordinator address stripped of port number."""
-  if not coordinator_address:
-    raise ValueError('Coordinator address not set.')
   return coordinator_address.split(':')[0]
 
 
 def create_coordinator_server_and_context() -> (
     Tuple[ts.Context, Optional[ts.ocdbt.DistributedCoordinatorServer]]
 ):
   """Creates OCDBT coordinator and Tensorstore context.
@@ -69,14 +67,25 @@
   Later, when creating the `PyTreeCheckpointHandler`, initialize with
   `use_ocdbt=True`.
 
   Returns:
     Tuple of ts.Context and OCDBT coordinator server object.
   """
   jax_global_state = jax._src.distributed.global_state  # pylint: disable=protected-access
+  if not jax_global_state.coordinator_address:
+    ts_context = {
+        # Provide cache pool for B-tree nodes to avoid repeated reads.
+        # 100MB limit.
+        'cache_pool#ocdbt': {'total_bytes_limit': 100000000},
+    }
+    return (
+        ts.Context(ts_context, parent=serialization.TS_CONTEXT),
+        None,
+    )
+
   ocdbt_address = _get_coordinator_address_without_port(
       jax_global_state.coordinator_address
   )
 
   coordinator_server = None
   if jax_global_state.process_id == 0:
     bind_address = f'{ocdbt_address}:0'
@@ -92,14 +101,15 @@
       'ocdbt_coordinator', _COORDINATOR_SETUP_TIMEOUT_SECS * 1000
   )
   ts_context = {
       'ocdbt_coordinator': {
           'address': ocdbt_address,
       },
       # Provide cache pool for B-tree nodes to avoid repeated reads.
+      # 100MB limit.
       'cache_pool#ocdbt': {'total_bytes_limit': 100000000},
   }
   return (
       ts.Context(ts_context, parent=serialization.TS_CONTEXT),
       coordinator_server,
   )
 
@@ -133,26 +143,29 @@
   internally.
 
   name:
     Name of the parameter.
   path:
     A path providing a location where file(s) should be saved. The path is
     assumed to be a directory.
-  aggregate:
-    Whether the parameter should be / was aggregated.
+  skip_deserialize:
+    If specified, skips deserialization of the given parameter using the
+    TypeHandler. This may be for multiple different reasons, including that the
+    parameter may have been aggregated, or it will be unneeded after
+    transformations.
   byte_limiter:
     Object to limit the number of bytes that can be read in
     parallel.
   is_ocdbt_checkpoint:
     Indicates whether the checkpoint path uses OCDBT format
     or not. Only used for restoration.
   """
   name: Optional[str] = None
   path: Optional[epath.Path] = None
-  aggregate: Optional[bool] = None
+  skip_deserialize: Optional[bool] = None
   byte_limiter: Optional[serialization._LimitInFlightBytes] = None  # pylint: disable=protected-access
   is_ocdbt_checkpoint: Optional[bool] = None
 
 
 @dataclasses.dataclass
 class SaveArgs:
   """Extra arguments that can be provided for saving.
@@ -194,54 +207,70 @@
 
 class TypeHandler(abc.ABC):
   """Interface for reading and writing a PyTree leaf."""
 
   @abc.abstractmethod
   async def serialize(
       self,
-      value: Any,
-      info: ParamInfo,
-      args: Optional[SaveArgs] = None) -> List[Future]:
+      values: Sequence[Any],
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[SaveArgs]] = None,
+  ) -> Sequence[Future]:
     """Writes the parameter to a storage location.
 
     This method is responsible for copying the parameter from a remote device in
     a synchronous fashion (if applicable). It should then return a list of
     futures which can be later awaited to complete the final commit operation
     to a storage location.
 
     The function can be used in a multihost setting, but should not implement
     extra logic to ensure atomicity.
 
     Args:
-      value: the parameter to save.
-      info: contains relevant information for serialization.
-      args: additional arguments for serialization, provided by the user.
+      values: a sequence of parameters to save.
+      infos: a sequence of ParamInfo containing relevant information for
+        serialization of each value.
+      args: a sequnece of additional arguments for serialization, provided by
+        the user.
 
     Returns:
-      List of commit futures which can be awaited to complete the save
+      Sequence of commit futures which can be awaited to complete the save
       operation.
     """
     pass
 
   @abc.abstractmethod
-  async def deserialize(self,
-                        info: ParamInfo,
-                        args: Optional[RestoreArgs] = None) -> Any:
+  async def deserialize(
+      self,
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[RestoreArgs]] = None,
+  ) -> Sequence[Any]:
     """Reads the parameter from a storage location.
 
     Args:
-      info: parameter information.
-      args: user-provided restoration information.
+      infos: Sequnece of ParamInfo for deserialization.
+      args: Sequence of user-provided restoration information.
 
     Returns:
-      The deserialized parameter.
+      The deserialized parameters.
     """
     pass
 
 
+def _check_input_arguments(*args):
+  l = None
+  for arg in args:
+    if l == 0:
+      raise ValueError('Cannot pass TypeHandler input of length 0.')
+    if l is None:
+      l = len(arg)
+    elif len(arg) != l:
+      raise ValueError('Found input args with mismatched lengths.')
+
+
 def is_ocdbt_checkpoint(path: epath.Path) -> bool:
   """Determines whether a checkpoint uses OCDBT format."""
   return (path / _OCDBT_MANIFEST_FILE).exists()
 
 
 def _get_cast_tspec_serialize(tspec, value, args):
   """Creates a Tensorstore spec for casting a param during serialize."""
@@ -268,15 +297,16 @@
         'dtype': jnp.dtype(args.dtype).name,
     }
   return tspec
 
 
 def _add_base_tspec_ocdbt_options(tspec: Dict[str, Any]) -> Dict[str, Any]:
   tspec.update({'recheck_cached_data': False, 'recheck_cached_metadata': False})
-  tspec['kvstore'].update({  # Enable read coalescing.
+  tspec['kvstore'].update({
+      # Enable read coalescing.
       'experimental_read_coalescing_threshold_bytes': 1000000,
       # References the cache specified in ts.Context.
       'cache_pool': 'cache_pool#ocdbt',
   })
   return tspec
 
 
@@ -352,64 +382,96 @@
 
   def _get_json_tspec_read(
       self, info: ParamInfo, use_ocdbt: bool = False
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec for reading."""
     return self._get_json_tspec(info, use_ocdbt=use_ocdbt)
 
-  async def serialize(self,
-                      value: np.ndarray,
-                      info: ParamInfo,
-                      args: Optional[SaveArgs] = None) -> List[Future]:
+  async def serialize(
+      self,
+      values: Sequence[np.ndarray],
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[SaveArgs]] = None,
+  ) -> Sequence[Future]:
     """Uses Tensorstore to serialize a numpy array."""
-    args = args or SaveArgs()
-    tspec = self._get_json_tspec_write(info, value, use_ocdbt=self._use_ocdbt)
-    tspec = _get_cast_tspec_serialize(tspec, value, args)
-    t = await ts.open(
-        ts.Spec(tspec), create=True, open=True, context=self._ts_context
-    )
-    write_future = t.write(value)
-    await write_future.copy
-    return [write_future.commit]
-
-  async def deserialize(self,
-                        info: ParamInfo,
-                        args: Optional[RestoreArgs] = None) -> np.ndarray:
+    args = args or [SaveArgs()] * len(values)
+    _check_input_arguments(values, infos, args)
+    copy_ops = []
+    futures = []
+    for value, info, arg in zip(values, infos, args):
+      tspec = self._get_json_tspec_write(info, value, use_ocdbt=self._use_ocdbt)
+      tspec = _get_cast_tspec_serialize(tspec, value, arg)
+      if jax.process_index() == 0:
+        # Open once to create metadata and allow the operation to happen
+        # asynchronously.
+        open_future = ts.open(
+            ts.Spec(tspec), create=True, open=True, context=self._ts_context
+        )
+        # Open again (no disk I/O) to get the write location.
+        t = await ts.open(
+            ts.Spec(tspec),
+            open=True,
+            assume_metadata=True,
+            context=self._ts_context,
+        )
+        write_future = t.write(value)
+        copy_ops += [write_future.copy]
+        futures += [open_future, write_future.commit]
+    await asyncio.gather(*copy_ops)
+    return futures
+
+  async def deserialize(
+      self,
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[RestoreArgs]] = None,
+  ) -> Sequence[np.ndarray]:
     """Deserializes the array using Tensorstore."""
-    args = args or RestoreArgs()
-    if not info.is_ocdbt_checkpoint:
-      await _assert_parameter_files_exist(info.path, self._metadata_key)
-    # Using OCDBT, but existing checkpoint may be stored in old format.
-    use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
-    tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
-    tspec = _get_cast_tspec_deserialize(tspec, args)
-    t = await ts.open(ts.Spec(tspec), open=True, context=self._ts_context)
-    return await t.read()
+    args = args or [RestoreArgs()] * len(infos)
+    _check_input_arguments(infos, args)
+    open_futures = []
+    for info, arg in zip(infos, args):
+      if not info.is_ocdbt_checkpoint:
+        await _assert_parameter_files_exist(info.path, self._metadata_key)
+      # Using OCDBT, but existing checkpoint may be stored in old format.
+      use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
+      tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
+      tspec = _get_cast_tspec_deserialize(tspec, arg)
+      open_futures += [
+          ts.open(ts.Spec(tspec), open=True, context=self._ts_context)
+      ]
+    tensorstores = await asyncio.gather(*open_futures)
+    read_ops = [t.read() for t in tensorstores]
+    return await asyncio.gather(*read_ops)
 
 
 class ScalarHandler(NumpyHandler):
   """A wrapper around NumpyHandler to deal with scalar types (int, float, etc.).
   """
 
-  async def serialize(self,
-                      value: Scalar,  # pytype: disable=signature-mismatch  # numpy-scalars
-                      info: ParamInfo,
-                      args: Optional[SaveArgs] = None) -> List[Future]:
+  async def serialize(
+      self,
+      values: Sequence[Scalar],  # pytype: disable=signature-mismatch
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[SaveArgs]] = None,
+  ) -> Sequence[Future]:
     """See superclass documentation."""
-    value = np.asarray(value)
-    return await super().serialize(value, info, args)
+    values = [np.asarray(v) for v in values]
+    return await super().serialize(values, infos, args)
 
-  async def deserialize(self,
-                        info: ParamInfo,
-                        args: Optional[RestoreArgs] = None) -> np.ndarray:
+  async def deserialize(
+      self,
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[RestoreArgs]] = None,
+  ) -> Sequence[Scalar]:  # pytype: disable=signature-mismatch
     """See superclass documentation."""
-    result = await super().deserialize(info, args)
-    if result.ndim != 0:
-      raise ValueError('Restored result is not a scalar.')
-    return result.item()
+    results = await super().deserialize(infos, args)
+    for r in results:
+      if r.ndim != 0:
+        raise ValueError('Restored result is not a scalar.')
+    return [r.item() for r in results]
 
 
 @dataclasses.dataclass
 class ArrayRestoreArgs(RestoreArgs):
   """Arguments used when restoring with ArrayHandler.
 
   mesh:
@@ -493,99 +555,139 @@
   def _get_json_tspec_read(
       self, info: ParamInfo, use_ocdbt: bool = False
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec for reading."""
     return self._get_json_tspec(info, use_ocdbt=use_ocdbt)
 
   async def serialize(
-      self, value: jax.Array, info: ParamInfo, args: Optional[SaveArgs] = None
-  ) -> List[Future]:
+      self,
+      values: Sequence[jax.Array],
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[SaveArgs]] = None,
+  ) -> Sequence[Future]:
     """See superclass documentation."""
-    if (
-        isinstance(value, jax.Array)
-        and jax.process_count() > 1
-        and value.is_fully_addressable
-    ):
-      raise ValueError(
-          'Cannot serialize host local arrays. Arrays like this are typically'
-          ' obtained using pmap. Consider using'
-          ' fully_replicated_host_local_array_to_global_array in'
-          ' orbax/checkpoint/utils.py to convert your arrays into serializable'
-          ' objects.'
-      )
-    args = args or SaveArgs()
-    tspec = self._get_json_tspec_write(info, value, use_ocdbt=self._use_ocdbt)
-    tspec = _get_cast_tspec_serialize(tspec, value, args)
-    commit_futures = []
-    await serialization.async_serialize(
-        value, tspec, commit_future=commit_futures, context=self._ts_context
-    )
-    return commit_futures
+    for v in values:
+      if (
+          isinstance(v, jax.Array)
+          and jax.process_count() > 1
+          and v.is_fully_addressable
+      ):
+        raise ValueError(
+            'Cannot serialize host local arrays. Arrays like this are typically'
+            ' obtained using pmap. Consider using'
+            ' fully_replicated_host_local_array_to_global_array in'
+            ' orbax/checkpoint/utils.py to convert your arrays into'
+            ' serializable objects.'
+        )
+    args = args or [SaveArgs()] * len(values)
+    _check_input_arguments(values, infos, args)
+    copy_ops = []
+    futures = []
+    for value, info, arg in zip(values, infos, args):
+      tspec = self._get_json_tspec_write(info, value, use_ocdbt=self._use_ocdbt)
+      tspec = _get_cast_tspec_serialize(tspec, value, arg)
+      copy_ops += [
+          serialization.async_serialize(
+              value,
+              tspec,
+              commit_future=futures,
+              context=self._ts_context,
+          )
+      ]
+    await asyncio.gather(*copy_ops)
+    return futures
 
-  async def deserialize(self,
-                        info: ParamInfo,
-                        args: Optional[RestoreArgs] = None) -> Any:
+  async def deserialize(
+      self,
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[RestoreArgs]] = None,
+  ) -> Sequence[jax.Array]:
     """See superclass documentation.
 
     Args:
-      info: ParamInfo.
+      infos: ParamInfo.
       args: must be of type `ArrayRestoreArgs`.
 
     Returns:
       The deserialized parameter.
 
     Raises:
       ValueError if `args` is not provided.
       ValueError if `args.mesh` or `args.mesh_axes` are not provided.
     """
     if args is None:
       raise ValueError('Must provide ArrayRestoreArgs to restore as jax.Array.')
-    args = cast(ArrayRestoreArgs, args)
-    if args.sharding is None and (args.mesh is None or args.mesh_axes is None):
-      raise ValueError(
-          'Sharding of jax.Array cannot be None. Provide `mesh`'
-          ' and `mesh_axes` OR `sharding`.'
-      )
-    if args.sharding is None:
-      sharding = jax.sharding.NamedSharding(args.mesh, args.mesh_axes)
-    else:
-      sharding = args.sharding
-    if not info.is_ocdbt_checkpoint:
-      await _assert_parameter_files_exist(info.path, self._metadata_key)
-    # Using OCDBT, but existing checkpoint may be stored in old format.
-    use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
-    tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
-    tspec = _get_cast_tspec_deserialize(tspec, args)
-    return await serialization.async_deserialize(
-        sharding,
-        tspec,
-        global_shape=args.global_shape,
-        byte_limiter=info.byte_limiter,
-        context=self._ts_context,
-    )
+    _check_input_arguments(infos, args)
+    deserialize_ops = []
+    for info, arg in zip(infos, args):
+      arg = cast(ArrayRestoreArgs, arg)
+      if arg.sharding is None and (arg.mesh is None or arg.mesh_axes is None):
+        raise ValueError(
+            'Sharding of jax.Array cannot be None. Provide `mesh`'
+            ' and `mesh_axes` OR `sharding`.'
+        )
+
+      if arg.sharding is None:
+        sharding = jax.sharding.NamedSharding(arg.mesh, arg.mesh_axes)
+      else:
+        sharding = arg.sharding
+      if not info.is_ocdbt_checkpoint:
+        await _assert_parameter_files_exist(info.path, self._metadata_key)
+      # Using OCDBT, but existing checkpoint may be stored in old format.
+      use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
+      tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
+      tspec = _get_cast_tspec_deserialize(tspec, arg)
+      deserialize_ops += [
+          serialization.async_deserialize(
+              sharding,
+              tspec,
+              global_shape=arg.global_shape,
+              byte_limiter=info.byte_limiter,
+              context=self._ts_context,
+          )
+      ]
+    return await asyncio.gather(*deserialize_ops)
 
 
 class StringHandler(TypeHandler):
-  """TypeHandler for strings that enforces aggregation."""
+  """TypeHandler for strings."""
+
+  def __init__(self, filename: Optional[str] = None):
+    self._filename = filename or '_strings.json'
 
-  async def serialize(self,
-                      value: str,
-                      info: ParamInfo,
-                      args: Optional[SaveArgs] = None) -> List[Future]:
+  async def serialize(
+      self,
+      values: Sequence[str],
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[SaveArgs]] = None,
+  ) -> Sequence[Future]:
     """See superclass documentation."""
-    args = args or SaveArgs()
-    if not args.aggregate:
-      raise ValueError('Non-aggregated string serialization is not supported.')
+    del args
+    _check_input_arguments(values, infos)
+    if jax.process_index() == 0:
+      directory = infos[0].path
+      strings = {info.name: value for value, info in zip(values, infos)}
+      path = directory / self._filename
+      path.write_text(json.dumps(strings))
     return []
 
-  async def deserialize(self,
-                        info: ParamInfo,
-                        args: Optional[RestoreArgs] = None) -> str:
+  async def deserialize(
+      self,
+      infos: Sequence[ParamInfo],
+      args: Optional[Sequence[RestoreArgs]] = None,
+  ) -> Sequence[Optional[str]]:
     """See superclass documentation."""
-    raise NotImplementedError
+    del args
+    _check_input_arguments(infos)
+    directory = infos[0].path
+    path = directory / self._filename
+    strings = json.loads(path.read_text())
+    return [
+        strings[info.name] if info.name in strings else None for info in infos
+    ]
 
 
 _TYPE_REGISTRY = [
     (lambda ty: issubclass(ty, int), ScalarHandler()),
     (lambda ty: issubclass(ty, float), ScalarHandler()),
     (lambda ty: issubclass(ty, bytes), ScalarHandler()),
     (lambda ty: issubclass(ty, np.number), ScalarHandler()),
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/utils.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 # limitations under the License.
 
 """Utility functions for Orbax.
 
 TODO(b/266449081) Increase unit test coverage.
 """
 import asyncio
+import concurrent.futures
 import functools
 import os
 import re
 import time
 from typing import Any, List, Optional, Tuple, Union
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental import multihost_utils
 import numpy as np
+from orbax.checkpoint.proto import tree_metadata_pb2
+
 
 TMP_DIR_SUFFIX = '.orbax-checkpoint-tmp-'
 # prefix_1000.orbax-checkpoint-tmp-1010101
 # OR
 # 1000.orbax-checkpoint-tmp-1010101
 TMP_DIR_STEP_PATTERN = r'.*?_*?(\d+)\.orbax-checkpoint-tmp-\d+'
 # TODO(b/260759189): Deprecate this prefix when no longer in use by JAX MG.
@@ -92,22 +95,29 @@
   return _wrap(path.mkdir)(*args, parents=parents, exist_ok=exist_ok, **kwargs)
 
 
 def async_write_bytes(path: epath.Path, data: Any):
   return _wrap(path.write_bytes)(data)
 
 
+def async_write_text(path: epath.Path, data: Any):
+  return _wrap(path.write_text)(data)
+
+
 def async_exists(path: epath.Path):
   return _wrap(path.exists)()
 
 
 class EmptyNode:
   pass
 
 
+# TODO(b/289258695): Refactor many of the following functions into tree_util.py.
+
+
 def is_empty_or_leaf(x: Any) -> bool:
   try:
     children, _ = jax._src.tree_util.flatten_one_level(x)  # pylint: disable=protected-access
   except ValueError:
     return True  # Cannot flatten x; means it must be a leaf
   return not children
 
@@ -122,14 +132,43 @@
     return key.name
   elif isinstance(key, jax.tree_util.FlattenedIndexKey):
     return key.key
   else:
     raise ValueError(f'Unsupported KeyEntry: {type(key)}: "{key}"')
 
 
+def get_key_metadata_type(
+    key: Any,
+) -> tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType:
+  """Translates the JAX key class into a proto enum."""
+  if isinstance(
+      key, (jax.tree_util.SequenceKey, jax.tree_util.FlattenedIndexKey)
+  ):
+    return tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType.SEQUENCE
+  elif isinstance(key, (jax.tree_util.DictKey, jax.tree_util.GetAttrKey)):
+    return tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType.DICT
+  else:
+    raise ValueError(f'Unsupported KeyEntry: {type(key)}: "{key}"')
+
+
+def keypath_from_key_metadata(
+    key: tree_metadata_pb2.TreeMetadata.KeyValuePair.Key,
+) -> Any:
+  """Converts from Key in TreeMetadata to JAX keypath class."""
+  if (
+      key.type
+      == tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType.SEQUENCE
+  ):
+    return jax.tree_util.SequenceKey(int(key.name))
+  elif key.type == tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType.DICT:
+    return jax.tree_util.DictKey(key.name)
+  else:
+    raise ValueError(f'Unsupported KeyEntry: {key.type}')
+
+
 def _is_dict_key(key) -> bool:
   return isinstance(key, (jax.tree_util.DictKey, jax.tree_util.GetAttrKey))
 
 
 def _is_sequence_key(key) -> bool:
   return isinstance(
       key, (jax.tree_util.FlattenedIndexKey, jax.tree_util.SequenceKey)
@@ -143,14 +182,67 @@
 def _extend_list(ls, idx, nextvalue):
   assert idx <= len(ls)
   if idx == len(ls):
     ls.append(nextvalue)
   return ls
 
 
+def from_flattened_with_keypath(flat_with_keys: PyTree) -> PyTree:
+  """Reconstructs a tree given the a flat dict with keypaths."""
+  # Accesses the first path element (arbitrary), first tuple element
+  # (keypath tuple), first key in keypath (outermost key in the PyTree).
+  outerkey = flat_with_keys[0][0][0]
+  if _is_dict_key(outerkey):
+    result = {}
+  elif _is_sequence_key(outerkey):
+    result = []
+  else:
+    result = None
+    _raise_unsupported_key_error(outerkey)
+
+  for keypath, value in flat_with_keys:
+    subtree = result
+    for i, key in enumerate(keypath):
+      if i == 0:
+        assert isinstance(key, type(outerkey))
+      if i == len(keypath) - 1:
+        if _is_dict_key(key):
+          assert isinstance(subtree, dict)
+          subtree[get_key_name(key)] = value
+        elif _is_sequence_key(key):
+          assert isinstance(subtree, list)
+          idx = get_key_name(key)
+          subtree = _extend_list(subtree, idx, value)
+      else:
+        nextkey = keypath[i + 1]
+        if _is_dict_key(nextkey):
+          nextvalue = {}
+        elif _is_sequence_key(nextkey):
+          nextvalue = []
+        else:
+          nextvalue = None
+          _raise_unsupported_key_error(nextkey)
+
+        if _is_dict_key(key):
+          assert isinstance(subtree, dict)
+          name = get_key_name(key)
+          if name not in subtree:
+            subtree[name] = nextvalue
+          subtree = subtree[name]
+        elif _is_sequence_key(key):
+          assert isinstance(subtree, list)
+          idx = get_key_name(key)
+          subtree = _extend_list(subtree, idx, nextvalue)
+          subtree = subtree[idx]
+        else:
+          _raise_unsupported_key_error(key)
+
+  return result
+
+
 def to_flat_dict(
     tree: PyTree, sep: Optional[str] = None, keep_empty_nodes: bool = False
 ) -> PyTree:
   """Converts a tree into a flattened dictionary.
 
   The nested keys are flattened to a tuple.
 
@@ -194,63 +286,15 @@
 
   Returns:
     The serialized PyTree.
   """
   flat_with_keys, _ = jax.tree_util.tree_flatten_with_path(
       tree, is_leaf=is_empty_or_leaf if keep_empty_nodes else None
   )
-  # Accesses the first path element (arbitrary), first tuple element
-  # (keypath tuple), first key in keypath (outermost key in the PyTree).
-  outerkey = flat_with_keys[0][0][0]
-  if _is_dict_key(outerkey):
-    result = {}
-  elif _is_sequence_key(outerkey):
-    result = []
-  else:
-    result = None
-    _raise_unsupported_key_error(outerkey)
-
-  for keypath, value in flat_with_keys:
-    subtree = result
-    for i, key in enumerate(keypath):
-      if i == 0:
-        assert isinstance(key, type(outerkey))
-      if i == len(keypath) - 1:
-        if _is_dict_key(key):
-          assert isinstance(subtree, dict)
-          subtree[get_key_name(key)] = value
-        elif _is_sequence_key(key):
-          assert isinstance(subtree, list)
-          idx = get_key_name(key)
-          subtree = _extend_list(subtree, idx, value)
-      else:
-        nextkey = keypath[i + 1]
-        if _is_dict_key(nextkey):
-          nextvalue = {}
-        elif _is_sequence_key(nextkey):
-          nextvalue = []
-        else:
-          nextvalue = None
-          _raise_unsupported_key_error(nextkey)
-
-        if _is_dict_key(key):
-          assert isinstance(subtree, dict)
-          name = get_key_name(key)
-          if name not in subtree:
-            subtree[name] = nextvalue
-          subtree = subtree[name]
-        elif _is_sequence_key(key):
-          assert isinstance(subtree, list)
-          idx = get_key_name(key)
-          subtree = _extend_list(subtree, idx, nextvalue)
-          subtree = subtree[idx]
-        else:
-          _raise_unsupported_key_error(key)
-
-  return result
+  return from_flattened_with_keypath(flat_with_keys)
 
 
 def deserialize_tree(
     serialized: PyTree, target: PyTree, keep_empty_nodes: bool = False
 ) -> PyTree:
   """Deserializes a PyTree to the same structure as `target`."""
 
@@ -279,25 +323,31 @@
   """Reconstructs the original tree object from a flattened dictionary.
 
   Args:
     flat_dict: A dictionary conforming to the return value of `to_flat_dict`.
     target: A reference PyTree. The returned value will conform to this
       structure. If not provided, an unflattened dict will be returned with the
       inferred structure of the original tree, without necessarily matching it
-      exactly.
+      exactly. Note, if not provided, the keys in `flat_dict` need to match
+      `sep`.
     sep: separator used for nested keys in `flat_dict`.
 
   Returns:
     A dict matching the structure of `tree` with the values of `flat_dict`.
   """
   if target is None:
     result = {}
     for k, v in flat_dict.items():
       subtree = result
-      for i, name in enumerate(k):
+      if sep is None:
+        assert isinstance(k, tuple)
+        tuple_k = k
+      else:
+        tuple_k = tuple(k.split(sep))
+      for i, name in enumerate(tuple_k):
         if i == len(k) - 1:
           assert name not in subtree
           subtree[name] = v
         else:
           if name not in subtree:
             subtree[name] = {}
           subtree = subtree[name]
@@ -577,19 +627,24 @@
 def checkpoint_steps_paths(
     checkpoint_dir: epath.PathLike,
 ) -> List[epath.Path]:
   """Returns a list of finalized checkpoint paths in the directory."""
   checkpoint_dir = epath.Path(checkpoint_dir)
   if not checkpoint_dir.exists():
     raise ValueError(f'Path {checkpoint_dir} does not exist.')
-  return [
-      step_dir
-      for step_dir in checkpoint_dir.iterdir()
-      if _is_step_checkpoint(step_dir) and is_checkpoint_finalized(step_dir)
-  ]
+
+  def check_step_dir(step_dir: epath.Path) -> bool:
+    return _is_step_checkpoint(step_dir) and is_checkpoint_finalized(step_dir)
+
+  with concurrent.futures.ThreadPoolExecutor() as executor:
+    futures = {
+        step_dir: executor.submit(check_step_dir, step_dir)
+        for step_dir in checkpoint_dir.iterdir()
+    }
+    return [step_dir for step_dir, future in futures.items() if future.result()]
 
 
 def checkpoint_steps(checkpoint_dir: epath.PathLike) -> List[int]:
   """Returns a list of finalized checkpoint steps in the directory."""
   checkpoint_dir = epath.Path(checkpoint_dir)
   return [
       step_from_checkpoint_name(s.name)
```

### Comparing `orbax_checkpoint-0.2.7/orbax/checkpoint/utils_test.py` & `orbax_checkpoint-0.3.0/orbax/checkpoint/utils_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Test for utils.py."""
+
 from typing import Mapping, Sequence
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from etils import epath
 # TODO(b/275613424): Eliminate flax dependency in Orbax test suite.
 import flax
 import jax
 import optax
+from orbax.checkpoint import test_utils
 from orbax.checkpoint import utils
 
 
 class UtilsTest(parameterized.TestCase):
 
   def setUp(self):
     super().setUp()
@@ -140,24 +142,36 @@
         expected, utils.from_flat_dict(flat_dict, target=empty)
     )
 
   def test_serialize(self):
     tree = {'a': 1, 'b': {'c': {'d': 2}}, 'e': [1, {'x': 5, 'y': 7}, [9, 10]]}
     serialized = utils.serialize_tree(tree, keep_empty_nodes=True)
     self.assertDictEqual(tree, serialized)
+    deserialized = utils.deserialize_tree(
+        serialized, target=tree, keep_empty_nodes=True
+    )
+    test_utils.assert_tree_equal(self, tree, deserialized)
 
   def test_serialize_list(self):
     tree = [1, {'a': 2}, [3, 4]]
     serialized = utils.serialize_tree(tree, keep_empty_nodes=True)
     self.assertListEqual(tree, serialized)
+    deserialized = utils.deserialize_tree(
+        serialized, target=tree, keep_empty_nodes=True
+    )
+    test_utils.assert_tree_equal(self, tree, deserialized)
 
   def test_serialize_filters_empty(self):
     tree = {'a': 1, 'b': None, 'c': {}, 'd': [], 'e': optax.EmptyState()}
     serialized = utils.serialize_tree(tree, keep_empty_nodes=False)
     self.assertDictEqual({'a': 1}, serialized)
+    deserialized = utils.deserialize_tree(
+        serialized, target=tree, keep_empty_nodes=False
+    )
+    test_utils.assert_tree_equal(self, tree, deserialized)
 
   def test_serialize_class(self):
     @flax.struct.dataclass
     class Foo:
       a: int
       b: Mapping[str, str]
       c: Sequence[optax.EmptyState]
@@ -173,14 +187,18 @@
     expected = {
         'a': 1,
         'b': {'a': 'b', 'c': 'd'},
         'c': [optax.EmptyState(), optax.EmptyState()],
         'd': [{}, {'x': 'y'}, None],
     }
     self.assertDictEqual(expected, serialized)
+    deserialized = utils.deserialize_tree(
+        serialized, target=foo, keep_empty_nodes=False
+    )
+    test_utils.assert_tree_equal(self, foo, deserialized)
 
   def test_serialize_nested_class(self):
     @flax.struct.dataclass
     class Foo:
       a: int
 
     nested = {
```

### Comparing `orbax_checkpoint-0.2.7/pyproject.toml` & `orbax_checkpoint-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.7/PKG-INFO` & `orbax_checkpoint-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.2.7
+Version: 0.3.0
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

