# Comparing `tmp/streams_py-0.3.1.tar.gz` & `tmp/streams_py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams_py-0.3.1.tar", max compression
+gzip compressed data, was "streams_py-0.3.2.tar", max compression
```

## Comparing `streams_py-0.3.1.tar` & `streams_py-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-07-21 14:03:59.216597 streams_py-0.3.1/LICENSE
--rw-r--r--   0        0        0    10867 2023-07-21 14:03:59.216597 streams_py-0.3.1/README.md
--rw-r--r--   0        0        0      733 2023-07-21 14:03:59.220598 streams_py-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      157 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/__init__.py
--rw-r--r--   0        0        0      336 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/__iterate.py
--rw-r--r--   0        0        0     3910 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/__optional.py
--rw-r--r--   0        0        0     3483 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/__stream.py
--rw-r--r--   0        0        0        0 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_itertools/__init__.py
--rw-r--r--   0        0        0     1713 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_itertools/tools.py
--rw-r--r--   0        0        0        0 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_lazy/__init__.py
--rw-r--r--   0        0        0      626 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_lazy/process.py
--rw-r--r--   0        0        0      593 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_lazy/queue.py
--rw-r--r--   0        0        0        0 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_parallel/__init__.py
--rw-r--r--   0        0        0     3885 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_parallel/fork_and_join.py
--rw-r--r--   0        0        0      787 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_parallel/parallelizer.py
--rw-r--r--   0        0        0    14521 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_streams/__base_stream.py
--rw-r--r--   0        0        0        0 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_streams/__init__.py
--rw-r--r--   0        0        0     3629 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/__parallel_stream.py
--rw-r--r--   0        0        0     2482 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/__sequential_stream.py
--rw-r--r--   0        0        0     3062 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/error/__error.py
--rw-r--r--   0        0        0      258 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/error/__levels.py
--rw-r--r--   0        0        0      307 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/error/__sentinel.py
--rw-r--r--   0        0        0     3595 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/numeric/__numeric_base_stream.py
--rw-r--r--   0        0        0      861 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
--rw-r--r--   0        0        0      686 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
--rw-r--r--   0        0        0      221 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/__init__.py
--rw-r--r--   0        0        0      307 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/combiners.py
--rw-r--r--   0        0        0    10878 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/date.py
--rw-r--r--   0        0        0     4937 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/numeric.py
--rw-r--r--   0        0        0     1385 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/string.py
--rw-r--r--   0        0        0      735 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/types.py
--rw-r--r--   0        0        0    11722 1970-01-01 00:00:00.000000 streams_py-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-24 12:47:16.224164 streams_py-0.3.2/LICENSE
+-rw-r--r--   0        0        0    10867 2023-07-24 12:47:16.224164 streams_py-0.3.2/README.md
+-rw-r--r--   0        0        0      733 2023-07-24 12:47:16.228164 streams_py-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__iterate.py
+-rw-r--r--   0        0        0     3910 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__optional.py
+-rw-r--r--   0        0        0     3483 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__stream.py
+-rw-r--r--   0        0        0     1654 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__stream_converter.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_itertools/__init__.py
+-rw-r--r--   0        0        0     1713 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_itertools/tools.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_lazy/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_lazy/process.py
+-rw-r--r--   0        0        0      593 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_lazy/queue.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_parallel/__init__.py
+-rw-r--r--   0        0        0     3885 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_parallel/fork_and_join.py
+-rw-r--r--   0        0        0      787 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_parallel/parallelizer.py
+-rw-r--r--   0        0        0    15476 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/__base_stream.py
+-rw-r--r--   0        0        0        0 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/__parallel_stream.py
+-rw-r--r--   0        0        0     2227 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/__sequential_stream.py
+-rw-r--r--   0        0        0     3062 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/error/__error.py
+-rw-r--r--   0        0        0      258 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/error/__levels.py
+-rw-r--r--   0        0        0      307 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/error/__sentinel.py
+-rw-r--r--   0        0        0     3595 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/numeric/__numeric_base_stream.py
+-rw-r--r--   0        0        0      861 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
+-rw-r--r--   0        0        0      686 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
+-rw-r--r--   0        0        0      221 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/combiners.py
+-rw-r--r--   0        0        0    10878 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/date.py
+-rw-r--r--   0        0        0     4937 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/numeric.py
+-rw-r--r--   0        0        0     1385 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/string.py
+-rw-r--r--   0        0        0      735 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/types.py
+-rw-r--r--   0        0        0    11722 1970-01-01 00:00:00.000000 streams_py-0.3.2/PKG-INFO
```

### Comparing `streams_py-0.3.1/LICENSE` & `streams_py-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/README.md` & `streams_py-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pyproject.toml` & `streams_py-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streams.py"
-version = "0.3.1"
+version = "0.3.2"
 authors = ["Stefan Garlonta <stefan@pickwicksoft.org>"]
 description = "A stream library for Python inspired by Java Stream API"
 keywords = ["streams", "parallel", "data"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/PickwickSoft/pystreamapi"
 repository = "https://github.com/PickwickSoft/pystreamapi"
 readme = "README.md"
```

### Comparing `streams_py-0.3.1/pystreamapi/__optional.py` & `streams_py-0.3.2/pystreamapi/__optional.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/__stream.py` & `streams_py-0.3.2/pystreamapi/__stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_itertools/tools.py` & `streams_py-0.3.2/pystreamapi/_itertools/tools.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_lazy/process.py` & `streams_py-0.3.2/pystreamapi/_lazy/process.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_lazy/queue.py` & `streams_py-0.3.2/pystreamapi/_lazy/queue.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_parallel/fork_and_join.py` & `streams_py-0.3.2/pystreamapi/_parallel/fork_and_join.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_parallel/parallelizer.py` & `streams_py-0.3.2/pystreamapi/_parallel/parallelizer.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_streams/__base_stream.py` & `streams_py-0.3.2/pystreamapi/_streams/__base_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from pystreamapi._lazy.process import Process
 from pystreamapi._lazy.queue import ProcessQueue
 from pystreamapi._streams.error.__error import ErrorHandler
 from pystreamapi._streams.error.__levels import ErrorLevel
 
 if TYPE_CHECKING:
     from pystreamapi._streams.numeric.__numeric_base_stream import NumericBaseStream
+    from pystreamapi._streams.__parallel_stream import ParallelStream
+    from pystreamapi._streams.__sequential_stream import SequentialStream
 
 K = TypeVar('K')
 _V = TypeVar('_V')
 _identity_missing = object()
 
 
 def _operation(func):
@@ -234,14 +236,21 @@
         return self
 
     def __map_to_str(self):
         """Converts the stream to strings."""
         self._map(str)
 
     @_operation
+    def parallel(self) -> 'ParallelStream[K]':
+        """Returns a parallel stream. If the stream is already parallel, it is returned."""
+        # pylint: disable=import-outside-toplevel
+        from pystreamapi.__stream_converter import StreamConverter
+        return StreamConverter.to_parallel_stream(self)
+
+    @_operation
     def peek(self, action: Callable) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the elements of this stream, additionally performing the
         provided action on each element as elements are consumed from the resulting stream.
 
         :param action:
         """
@@ -266,14 +275,21 @@
         """Reverses the stream."""
         try:
             self._source = reversed(self._source)
         except TypeError:
             self._source = reversed(list(self._source))
 
     @_operation
+    def sequential(self) -> SequentialStream[K]:
+        """Returns a sequential stream. If the stream is already sequential, it is returned."""
+        # pylint: disable=import-outside-toplevel
+        from pystreamapi.__stream_converter import StreamConverter
+        return StreamConverter.to_sequential_stream(self)
+
+    @_operation
     def skip(self, n: int) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the remaining elements of this stream after discarding the
         first n elements of the stream.
 
         :param n:
         """
@@ -426,10 +442,12 @@
         """
         Returns a dictionary consisting of the results of grouping the elements of this stream
         by the given classifier.
 
         :param key_mapper:
         """
 
-    @abstractmethod
     def _to_numeric_stream(self) -> NumericBaseStream:
-        """Converts a stream to a numeric stream. To be implemented by subclasses."""
+        """Converts a stream to a numeric stream using the stream converter"""
+        # pylint: disable=import-outside-toplevel
+        from pystreamapi.__stream_converter import StreamConverter
+        return StreamConverter.to_numeric_stream(self)
```

### Comparing `streams_py-0.3.1/pystreamapi/_streams/__parallel_stream.py` & `streams_py-0.3.2/pystreamapi/_streams/__parallel_stream.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,13 +87,7 @@
         return dict(self._group_to_dict(key_mapper))
 
     def _set_parallelizer_src(self):
         self._parallelizer.set_source(self._source, self)
 
     def __mapper(self, mapper):
         return lambda x: self._one(mapper=mapper, item=x)
-
-    def _to_numeric_stream(self):
-        # pylint: disable=import-outside-toplevel
-        from pystreamapi._streams.numeric.__parallel_numeric_stream import ParallelNumericStream
-        self.__class__ = ParallelNumericStream
-        return self
```

### Comparing `streams_py-0.3.1/pystreamapi/_streams/__sequential_stream.py` & `streams_py-0.3.2/pystreamapi/_streams/__sequential_stream.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,13 +58,7 @@
                 return reduce(predicate, self._source)
             return Optional.of(reduce(predicate, self._source, handler=self))
         return identity if identity is not _identity_missing else Optional.empty()
 
     @stream.terminal
     def to_dict(self, key_mapper: Callable[[Any], Any]) -> dict:
         return self._group_to_dict(key_mapper)
-
-    def _to_numeric_stream(self):
-        # pylint: disable=import-outside-toplevel
-        from pystreamapi._streams.numeric.__sequential_numeric_stream import SequentialNumericStream
-        self.__class__ = SequentialNumericStream
-        return self
```

### Comparing `streams_py-0.3.1/pystreamapi/_streams/error/__error.py` & `streams_py-0.3.2/pystreamapi/_streams/error/__error.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_streams/numeric/__numeric_base_stream.py` & `streams_py-0.3.2/pystreamapi/_streams/numeric/__numeric_base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_streams/numeric/__parallel_numeric_stream.py` & `streams_py-0.3.2/pystreamapi/_streams/numeric/__parallel_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/_streams/numeric/__sequential_numeric_stream.py` & `streams_py-0.3.2/pystreamapi/_streams/numeric/__sequential_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/conditions/date.py` & `streams_py-0.3.2/pystreamapi/conditions/date.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/conditions/numeric.py` & `streams_py-0.3.2/pystreamapi/conditions/numeric.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/conditions/string.py` & `streams_py-0.3.2/pystreamapi/conditions/string.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/pystreamapi/conditions/types.py` & `streams_py-0.3.2/pystreamapi/conditions/types.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.1/PKG-INFO` & `streams_py-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streams-py
-Version: 0.3.1
+Version: 0.3.2
 Summary: A stream library for Python inspired by Java Stream API
 Home-page: https://github.com/PickwickSoft/pystreamapi
 License: GPL-3.0-or-later
 Keywords: streams,parallel,data
 Author: Stefan Garlonta
 Author-email: stefan@pickwicksoft.org
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streams-py Version: 0.3.1 Summary: A stream library
+Metadata-Version: 2.1 Name: streams-py Version: 0.3.2 Summary: A stream library
 for Python inspired by Java Stream API Home-page: https://github.com/
 PickwickSoft/pystreamapi License: GPL-3.0-or-later Keywords:
 streams,parallel,data Author: Stefan Garlonta Author-email:
 stefan@pickwicksoft.org Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

