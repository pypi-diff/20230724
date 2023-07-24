# Comparing `tmp/kissio-0.0.1.tar.gz` & `tmp/kissio-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kissio-0.0.1.tar", last modified: Sun Jul 23 22:58:04 2023, max compression
+gzip compressed data, was "kissio-0.0.2.tar", last modified: Mon Jul 24 00:03:24 2023, max compression
```

## Comparing `kissio-0.0.1.tar` & `kissio-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:58:04.022942 kissio-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-23 22:57:49.000000 kissio-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-23 22:58:04.022942 kissio-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-23 22:57:49.000000 kissio-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:58:04.018941 kissio-0.0.1/kissio/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-23 22:57:49.000000 kissio-0.0.1/kissio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-23 22:57:49.000000 kissio-0.0.1/kissio/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:58:04.018941 kissio-0.0.1/kissio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-23 22:58:03.000000 kissio-0.0.1/kissio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-23 22:58:03.000000 kissio-0.0.1/kissio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:58:03.000000 kissio-0.0.1/kissio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-23 22:58:03.000000 kissio-0.0.1/kissio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 22:58:04.022942 kissio-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-23 22:57:49.000000 kissio-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:58:04.018941 kissio-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-23 22:57:49.000000 kissio-0.0.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:03:24.798290 kissio-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 00:03:10.000000 kissio-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 00:03:24.798290 kissio-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-24 00:03:10.000000 kissio-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:03:24.798290 kissio-0.0.2/kissio/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 00:03:10.000000 kissio-0.0.2/kissio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-24 00:03:10.000000 kissio-0.0.2/kissio/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:03:24.798290 kissio-0.0.2/kissio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 00:03:24.000000 kissio-0.0.2/kissio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 00:03:24.000000 kissio-0.0.2/kissio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:03:24.000000 kissio-0.0.2/kissio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 00:03:24.000000 kissio-0.0.2/kissio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:03:24.798290 kissio-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 00:03:10.000000 kissio-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:03:24.798290 kissio-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-24 00:03:10.000000 kissio-0.0.2/test/test.py
```

### Comparing `kissio-0.0.1/LICENSE` & `kissio-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kissio-0.0.1/kissio/pipe.py` & `kissio-0.0.2/kissio/pipe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from concurrent.futures import ThreadPoolExecutor
 from functools import reduce
 import itertools
+import logging
+from datetime import datetime
 from queue import Empty, Queue
 import time
 import timeit
 from typing import List, Callable, Iterable, Iterator, TypeVar
 
 T = TypeVar("T")
 R = TypeVar("R")
@@ -19,81 +21,141 @@
     def __next__(self) -> T:
         return next(self.iterator)
 
     def __iter__(self) -> T:
         return self
 
     def chain(self, *others: Iterable["Pipe[T]"]) -> "Pipe[T]":
-        return Pipe(
-            itertools.chain(self.iterator, *(other.iterator for other in others))
-        )
+        return Pipe(itertools.chain(self, *others))
 
     def merge(self, *others: Iterable["Pipe[T]"]) -> "Pipe[T]":
-        return _ConcurrentlyMergingPipe(
-            [self.iterator, *(other.iterator for other in others)]
-        )
+        return _ConcurrentlyMergingPipe([self, *others])
 
     def map(self, func: Callable[[T], R], num_threads: int = 0) -> "Pipe[R]":
         if num_threads <= 1:
-            return Pipe(map(func, self.iterator))
+            return Pipe(map(func, self))
         else:
 
             def iterable():
                 executor = ThreadPoolExecutor(max_workers=num_threads)
-                yield from executor.map(func, self.iterator)
+                yield from executor.map(func, self)
                 executor.shutdown()
 
             return Pipe(iter(iterable()))
 
     def filter(self, predicate: Callable[[T], bool]) -> "Pipe[R]":
-        return Pipe(filter(predicate, self.iterator))
+        return Pipe(filter(predicate, self))
 
     def batch(
         self, max_size: int = 100, max_window_seconds: float = float("inf")
     ) -> "Pipe[List[T]]":
-        return _BatchingPipe(self.iterator, max_size, max_window_seconds)
+        return _BatchingPipe(self, max_size, max_window_seconds)
 
     def rate_limit(self, max_yields_per_second: int) -> "Pipe[T]":
-        return Pipe(_RateLimitingIterator(self.iterator, max_yields_per_second))
+        return Pipe(_RateLimitingIterator(self, max_yields_per_second))
 
     def head(self, n) -> "Pipe[T]":
-        return Pipe(itertools.islice(self.iterator, n))
+        return Pipe(itertools.islice(self, n))
+
+    def catch(self) -> "Pipe[T]":
+        return _CatchingPipe(self)
+
+    def log(self) -> "Pipe[T]":
+        return _LoggingPipe(self)
 
     def reduce(self, f: Callable[[R, T], R], initial: R) -> R:
-        return reduce(f, self.iterator, initial)
+        return reduce(f, self, initial)
 
-    def collect(self, limit: int = float("inf")) -> List[T]:
+    def exhaust_into_limited_list(self, limit: int = float("inf")) -> List[T]:
         return [elem for i, elem in enumerate(self.iterator) if i < limit]
 
     def timeit(self) -> float:
         def iterate():
             for _ in self:
                 pass
 
         return timeit.timeit(iterate, number=1)
 
 
-class _RateLimitingIterator(Iterator[T]):
+class CatchedPipeError:
+    def __init__(self, e: Exception) -> None:
+        self.error_type = type(e)
+        self.message = str(e)
+
+    def __str__(self) -> str:
+        return f"{self.error_type}: {self.message}"
+
+
+class _CatchingPipe(Pipe[T]):
+    def __next__(self) -> T:
+        try:
+            return super().__next__()
+        except Exception as e:
+            if isinstance(e, StopIteration):
+                raise
+            else:
+                return CatchedPipeError(e)
+
+
+class _LoggingPipe(Pipe[T]):
+    def __init__(self, iterator: Iterator[T]) -> None:
+        super().__init__(iterator)
+        logging.getLogger().setLevel(logging.INFO)
+        self.yields_count = 0
+        self.errors_count = 0
+        self.last_log_at_yields_count = 0
+        self.start_time = time.time()
+
+    def _log(self) -> None:
+        logging.info(
+            "%s yields in %s, leading to the catch of %s errors.",
+            self.yields_count,
+            str(
+                datetime.fromtimestamp(time.time())
+                - datetime.fromtimestamp(self.start_time)
+            ),
+            self.errors_count,
+        )
+
+    def __next__(self) -> T:
+        try:
+            elem = super().__next__()
+        except StopIteration:
+            self._log()
+            raise
+
+        self.yields_count += 1
+        if isinstance(elem, CatchedPipeError):
+            self.errors_count += 1
+
+        if self.yields_count + self.errors_count >= 2 * self.last_log_at_yields_count:
+            self._log()
+            self.last_log_at_yields_count = self.yields_count + self.errors_count
+
+        return elem
+
+
+class _RateLimitingIterator(Pipe[T]):
     def __init__(self, iterator: Iterator[T], max_yields_per_second: int) -> None:
-        self.iterator = iterator
+        super().__init__(iterator)
         self.max_yields_per_second = max_yields_per_second
         self.start = None
         self.num_yielded_elements = 0
 
     def __next__(self) -> T:
         if not self.start:
             self.start = time.time()
         while True:
             while (
                 self.num_yielded_elements
                 > (time.time() - self.start) * self.max_yields_per_second
             ):
                 time.sleep(1 / self.max_yields_per_second)
             self.num_yielded_elements += 1
-            return next(self.iterator)
+            return super().__next__()
 
 
 class _BatchingPipe(Pipe[List[T]]):
     def __init__(
         self, iterator: Iterator[T], max_size: int, max_window_seconds: float
     ) -> None:
         super().__init__(iterator)
@@ -115,16 +177,16 @@
                 return batch
             else:
                 raise
 
 
 class _ConcurrentlyMergingPipe(Pipe[T]):
     def __init__(self, iterators: List[Iterator[T]]) -> None:
-        self.iterator = iter(
-            _ConcurrentlyMergingPipe._concurrently_merging_iterable(iterators)
+        super().__init__(
+            iter(_ConcurrentlyMergingPipe._concurrently_merging_iterable(iterators))
         )
 
     @staticmethod
     def _pull_in_queue(iterator: Iterator[T], queue: Queue) -> None:
         for elem in iterator:
             queue.put(elem)
```

### Comparing `kissio-0.0.1/test/test.py` & `kissio-0.0.2/test/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import time
+import timeit
 import unittest
 
 from kissio import Pipe
+from kissio.pipe import CatchedPipeError
 
+TEN_MS = 0.01
+
+
+def ten_millis_identity(x):
+    time.sleep(TEN_MS)
+    return x
 
-class TestPipe(unittest.TestCase):
-    @staticmethod
-    def ten_millis_identity(x):
-        time.sleep(0.01)
-        return x
 
+class TestPipe(unittest.TestCase):
     def test_init(self):
         # from iterable
         self.assertListEqual(list(Pipe(range(8))), list(range(8)))
         # from iterator
         self.assertListEqual(list(Pipe(iter(range(8)))), list(range(8)))
 
     def test_chain(self):
@@ -42,23 +46,22 @@
         # non threaded
         self.assertListEqual(list(Pipe(range(8)).map(func)), list(map(func, range(8))))
         # threaded
         self.assertListEqual(
             list(Pipe(range(8)).map(func, num_threads=2)), list(map(func, range(8)))
         )
         # non-threaded vs threaded execution time
-        ten_ms = 0.01
-        pipe = Pipe(range(8)).map(TestPipe.ten_millis_identity)
-        self.assertAlmostEqual(pipe.timeit(), ten_ms * 8, delta=0.3 * (ten_ms * 8))
+        pipe = Pipe(range(8)).map(ten_millis_identity)
+        self.assertAlmostEqual(pipe.timeit(), TEN_MS * 8, delta=0.3 * (TEN_MS * 8))
         num_threads = 2
-        pipe = Pipe(range(8)).map(TestPipe.ten_millis_identity, num_threads=num_threads)
+        pipe = Pipe(range(8)).map(ten_millis_identity, num_threads=num_threads)
         self.assertAlmostEqual(
             pipe.timeit(),
-            ten_ms * 8 / num_threads,
-            delta=0.3 * (ten_ms * 8) / num_threads,
+            TEN_MS * 8 / num_threads,
+            delta=0.3 * (TEN_MS * 8) / num_threads,
         )
 
     def test_filter(self):
         self.assertListEqual(list(Pipe(range(8)).filter(lambda x: x % 2)), [1, 3, 5, 7])
 
         self.assertListEqual(list(Pipe(range(8)).filter(lambda _: False)), [])
 
@@ -72,36 +75,65 @@
         self.assertListEqual(
             list(Pipe(range(8)).batch(max_size=1)), list(map(lambda x: [x], range(8)))
         )
         self.assertListEqual(list(Pipe(range(8)).batch(max_size=8)), [list(range(8))])
 
     def test_rate_limit(self):
         max_yields_per_second = 64
-        pipe = (
-            Pipe(range(8))
-            .map(TestPipe.ten_millis_identity)
-            .rate_limit(max_yields_per_second)
-        )
+        pipe = Pipe(range(8)).map(ten_millis_identity).rate_limit(max_yields_per_second)
         self.assertAlmostEqual(
             pipe.timeit(),
             1 / max_yields_per_second * 8,
             delta=0.3 * (1 / max_yields_per_second * 8),
         )
 
     def test_head(self):
         self.assertListEqual(list(Pipe(range(8)).head(3)), [0, 1, 2])
+        # stops after the second element
+        self.assertAlmostEqual(
+            Pipe(range(8)).map(ten_millis_identity).head(2).timeit(),
+            TEN_MS * 2,
+            delta=0.3 * TEN_MS * 2,
+        )
+
+    def test_exhaust_into_limited_list(self):
+        self.assertListEqual(
+            Pipe(range(8)).exhaust_into_limited_list(limit=6), list(range(6))
+        )
+        self.assertListEqual(Pipe(range(8)).exhaust_into_limited_list(), list(range(8)))
+        self.assertAlmostEqual(
+            timeit.timeit(
+                lambda: Pipe(range(8))
+                .map(ten_millis_identity)
+                .exhaust_into_limited_list(0),
+                number=1,
+            ),
+            TEN_MS * 8,
+            delta=0.3 * TEN_MS * 8,
+        )
 
     def test_reduce(self):
         self.assertEqual(Pipe(range(8)).reduce(lambda count, elem: count + 1, 0), 8)
 
-    def test_collect(self):
-        self.assertListEqual(Pipe(range(8)).collect(limit=6), list(range(6)))
-        self.assertListEqual(Pipe(range(8)).collect(), list(range(8)))
-
     def test_timeit(self):
         get_pipe = lambda: Pipe(range(8)).rate_limit(64)
         start_time = time.time()
         list(get_pipe())
         execution_time = time.time() - start_time
         self.assertAlmostEqual(
             execution_time, get_pipe().timeit(), delta=0.3 * execution_time
         )
+
+    def test_catch(self):
+        self.assertListEqual(
+            list(Pipe(["1", "r", "2"]).map(int).catch().map(type)),
+            [int, CatchedPipeError, int],
+        )
+
+    def test_log(self):
+        list(
+            Pipe(range(9))
+            .map(lambda elem: ("_" if elem % 2 else "") + str(elem))
+            .map(int)
+            .catch()
+            .log()
+        )
```

