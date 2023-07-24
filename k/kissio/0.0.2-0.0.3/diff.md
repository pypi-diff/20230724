# Comparing `tmp/kissio-0.0.2.tar.gz` & `tmp/kissio-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kissio-0.0.2.tar", last modified: Mon Jul 24 00:03:24 2023, max compression
+gzip compressed data, was "kissio-0.0.3.tar", last modified: Mon Jul 24 10:38:24 2023, max compression
```

## Comparing `kissio-0.0.2.tar` & `kissio-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:03:24.798290 kissio-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 00:03:10.000000 kissio-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 00:03:24.798290 kissio-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-24 00:03:10.000000 kissio-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:03:24.798290 kissio-0.0.2/kissio/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 00:03:10.000000 kissio-0.0.2/kissio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-24 00:03:10.000000 kissio-0.0.2/kissio/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:03:24.798290 kissio-0.0.2/kissio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 00:03:24.000000 kissio-0.0.2/kissio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 00:03:24.000000 kissio-0.0.2/kissio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:03:24.000000 kissio-0.0.2/kissio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 00:03:24.000000 kissio-0.0.2/kissio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 00:03:24.798290 kissio-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 00:03:10.000000 kissio-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:03:24.798290 kissio-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-24 00:03:10.000000 kissio-0.0.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:24.806990 kissio-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 10:38:14.000000 kissio-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 10:38:24.806990 kissio-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 10:38:14.000000 kissio-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:24.806990 kissio-0.0.3/kissio/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 10:38:14.000000 kissio-0.0.3/kissio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-24 10:38:14.000000 kissio-0.0.3/kissio/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:24.806990 kissio-0.0.3/kissio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 10:38:24.000000 kissio-0.0.3/kissio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 10:38:24.000000 kissio-0.0.3/kissio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:38:24.000000 kissio-0.0.3/kissio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 10:38:24.000000 kissio-0.0.3/kissio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:38:24.806990 kissio-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 10:38:14.000000 kissio-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:24.806990 kissio-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-24 10:38:14.000000 kissio-0.0.3/test/test.py
```

### Comparing `kissio-0.0.2/LICENSE` & `kissio-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kissio-0.0.2/kissio/pipe.py` & `kissio-0.0.3/kissio/pipe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from concurrent.futures import ThreadPoolExecutor
-from functools import reduce
 import itertools
 import logging
-from datetime import datetime
-from queue import Empty, Queue
 import time
 import timeit
-from typing import List, Callable, Iterable, Iterator, TypeVar
+from concurrent.futures import ThreadPoolExecutor
+from datetime import datetime
+from functools import reduce
+from queue import Empty, Queue
+from typing import Callable, Iterable, Iterator, List, TypeVar
 
 T = TypeVar("T")
 R = TypeVar("R")
 
 
 class Pipe(Iterator[T]):
     def __init__(self, iterator: Iterator[T]) -> None:
@@ -38,48 +38,64 @@
             def iterable():
                 executor = ThreadPoolExecutor(max_workers=num_threads)
                 yield from executor.map(func, self)
                 executor.shutdown()
 
             return Pipe(iter(iterable()))
 
+    def explode(self) -> "Pipe":
+        return _ExplodingPipe(self)
+
     def filter(self, predicate: Callable[[T], bool]) -> "Pipe[R]":
         return Pipe(filter(predicate, self))
 
     def batch(
         self, max_size: int = 100, max_window_seconds: float = float("inf")
     ) -> "Pipe[List[T]]":
         return _BatchingPipe(self, max_size, max_window_seconds)
 
-    def rate_limit(self, max_yields_per_second: int) -> "Pipe[T]":
-        return Pipe(_RateLimitingIterator(self, max_yields_per_second))
+    def slow(self, freq: int) -> "Pipe[T]":
+        return Pipe(_SlowingIterator(self, freq))
 
     def head(self, n) -> "Pipe[T]":
         return Pipe(itertools.islice(self, n))
 
     def catch(self) -> "Pipe[T]":
         return _CatchingPipe(self)
 
     def log(self) -> "Pipe[T]":
         return _LoggingPipe(self)
 
     def reduce(self, f: Callable[[R, T], R], initial: R) -> R:
         return reduce(f, self, initial)
 
-    def exhaust_into_limited_list(self, limit: int = float("inf")) -> List[T]:
-        return [elem for i, elem in enumerate(self.iterator) if i < limit]
+    def list(self, limit: int = float("inf")) -> List[T]:
+        return [elem for i, elem in enumerate(self) if i < limit]
 
     def timeit(self) -> float:
         def iterate():
             for _ in self:
                 pass
 
         return timeit.timeit(iterate, number=1)
 
 
+class _ExplodingPipe(Pipe[T]):
+    def __init__(self, iterator: Iterator[Iterable[T]]) -> None:
+        super().__init__(iterator)
+        self.current_iterator_elem = iter(super().__next__())
+
+    def __next__(self) -> T:
+        try:
+            return next(self.current_iterator_elem)
+        except StopIteration:
+            self.current_iterator_elem = iter(super().__next__())
+            return next(self)
+
+
 class CatchedPipeError:
     def __init__(self, e: Exception) -> None:
         self.error_type = type(e)
         self.message = str(e)
 
     def __str__(self) -> str:
         return f"{self.error_type}: {self.message}"
@@ -130,30 +146,30 @@
         if self.yields_count + self.errors_count >= 2 * self.last_log_at_yields_count:
             self._log()
             self.last_log_at_yields_count = self.yields_count + self.errors_count
 
         return elem
 
 
-class _RateLimitingIterator(Pipe[T]):
-    def __init__(self, iterator: Iterator[T], max_yields_per_second: int) -> None:
+class _SlowingIterator(Pipe[T]):
+    def __init__(self, iterator: Iterator[T], freq: int) -> None:
         super().__init__(iterator)
-        self.max_yields_per_second = max_yields_per_second
+        self.freq = freq
         self.start = None
         self.num_yielded_elements = 0
 
     def __next__(self) -> T:
         if not self.start:
             self.start = time.time()
         while True:
             while (
                 self.num_yielded_elements
-                > (time.time() - self.start) * self.max_yields_per_second
+                > (time.time() - self.start) * self.freq
             ):
-                time.sleep(1 / self.max_yields_per_second)
+                time.sleep(1 / self.freq)
             self.num_yielded_elements += 1
             return super().__next__()
 
 
 class _BatchingPipe(Pipe[List[T]]):
     def __init__(
         self, iterator: Iterator[T], max_size: int, max_window_seconds: float
```

### Comparing `kissio-0.0.2/test/test.py` & `kissio-0.0.3/test/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,30 @@
         pipe = Pipe(range(8)).map(ten_millis_identity, num_threads=num_threads)
         self.assertAlmostEqual(
             pipe.timeit(),
             TEN_MS * 8 / num_threads,
             delta=0.3 * (TEN_MS * 8) / num_threads,
         )
 
+    def test_explode(self):
+        self.assertListEqual(
+            list(Pipe(["Hello World", "Happy to be here :)"]).map(str.split).explode()),
+            ["Hello", "World", "Happy", "to", "be", "here", ":)"],
+        )
+        self.assertEqual(
+            sum(
+                Pipe([["1 2 3", "4 5 6"], ["7", "8 9 10"]])
+                .explode()
+                .map(str.split)
+                .explode()
+                .map(int)
+            ),
+            55,
+        )
+
     def test_filter(self):
         self.assertListEqual(list(Pipe(range(8)).filter(lambda x: x % 2)), [1, 3, 5, 7])
 
         self.assertListEqual(list(Pipe(range(8)).filter(lambda _: False)), [])
 
     def test_batch(self):
         self.assertListEqual(
@@ -73,53 +89,49 @@
             list(Pipe(range(6)).batch(max_size=3)), [[0, 1, 2], [3, 4, 5]]
         )
         self.assertListEqual(
             list(Pipe(range(8)).batch(max_size=1)), list(map(lambda x: [x], range(8)))
         )
         self.assertListEqual(list(Pipe(range(8)).batch(max_size=8)), [list(range(8))])
 
-    def test_rate_limit(self):
-        max_yields_per_second = 64
-        pipe = Pipe(range(8)).map(ten_millis_identity).rate_limit(max_yields_per_second)
+    def test_slow(self):
+        freq = 64
+        pipe = Pipe(range(8)).map(ten_millis_identity).slow(freq)
         self.assertAlmostEqual(
             pipe.timeit(),
-            1 / max_yields_per_second * 8,
-            delta=0.3 * (1 / max_yields_per_second * 8),
+            1 / freq * 8,
+            delta=0.3 * (1 / freq * 8),
         )
 
     def test_head(self):
         self.assertListEqual(list(Pipe(range(8)).head(3)), [0, 1, 2])
         # stops after the second element
         self.assertAlmostEqual(
             Pipe(range(8)).map(ten_millis_identity).head(2).timeit(),
             TEN_MS * 2,
             delta=0.3 * TEN_MS * 2,
         )
 
-    def test_exhaust_into_limited_list(self):
-        self.assertListEqual(
-            Pipe(range(8)).exhaust_into_limited_list(limit=6), list(range(6))
-        )
-        self.assertListEqual(Pipe(range(8)).exhaust_into_limited_list(), list(range(8)))
+    def test_list(self):
+        self.assertListEqual(Pipe(range(8)).list(limit=6), list(range(6)))
+        self.assertListEqual(Pipe(range(8)).list(), list(range(8)))
         self.assertAlmostEqual(
             timeit.timeit(
-                lambda: Pipe(range(8))
-                .map(ten_millis_identity)
-                .exhaust_into_limited_list(0),
+                lambda: Pipe(range(8)).map(ten_millis_identity).list(0),
                 number=1,
             ),
             TEN_MS * 8,
             delta=0.3 * TEN_MS * 8,
         )
 
     def test_reduce(self):
         self.assertEqual(Pipe(range(8)).reduce(lambda count, elem: count + 1, 0), 8)
 
     def test_timeit(self):
-        get_pipe = lambda: Pipe(range(8)).rate_limit(64)
+        get_pipe = lambda: Pipe(range(8)).slow(64)
         start_time = time.time()
         list(get_pipe())
         execution_time = time.time() - start_time
         self.assertAlmostEqual(
             execution_time, get_pipe().timeit(), delta=0.3 * execution_time
         )
```

