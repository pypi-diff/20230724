# Comparing `tmp/kissio-0.0.6.tar.gz` & `tmp/kissio-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kissio-0.0.6.tar", last modified: Mon Jul 24 11:10:12 2023, max compression
+gzip compressed data, was "kissio-0.0.7.tar", last modified: Mon Jul 24 13:45:16 2023, max compression
```

## Comparing `kissio-0.0.6.tar` & `kissio-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:10:12.006350 kissio-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 11:09:56.000000 kissio-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 11:10:12.006350 kissio-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 11:09:56.000000 kissio-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:10:12.002350 kissio-0.0.6/kissio/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 11:09:56.000000 kissio-0.0.6/kissio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-24 11:09:56.000000 kissio-0.0.6/kissio/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:10:12.002350 kissio-0.0.6/kissio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 11:10:11.000000 kissio-0.0.6/kissio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 11:10:11.000000 kissio-0.0.6/kissio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:10:11.000000 kissio-0.0.6/kissio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 11:10:11.000000 kissio-0.0.6/kissio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:10:12.006350 kissio-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 11:09:56.000000 kissio-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:10:12.006350 kissio-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-24 11:09:56.000000 kissio-0.0.6/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:45:16.410017 kissio-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 13:44:59.000000 kissio-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 13:45:16.410017 kissio-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 13:44:59.000000 kissio-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:45:16.406017 kissio-0.0.7/kissio/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 13:44:59.000000 kissio-0.0.7/kissio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-07-24 13:44:59.000000 kissio-0.0.7/kissio/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:45:16.406017 kissio-0.0.7/kissio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 13:45:16.000000 kissio-0.0.7/kissio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 13:45:16.000000 kissio-0.0.7/kissio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:45:16.000000 kissio-0.0.7/kissio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 13:45:16.000000 kissio-0.0.7/kissio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:45:16.410017 kissio-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 13:44:59.000000 kissio-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:45:16.410017 kissio-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-24 13:44:59.000000 kissio-0.0.7/test/test.py
```

### Comparing `kissio-0.0.6/LICENSE` & `kissio-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kissio-0.0.6/README.md` & `kissio-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `kissio-0.0.6/kissio/pipe.py` & `kissio-0.0.7/kissio/pipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,21 @@
     def map(self, func: Callable[[T], R], num_threads: int = 0) -> "Pipe[R]":
         if num_threads <= 1:
             return Pipe(map(func, self))
         else:
 
             def iterable():
                 executor = ThreadPoolExecutor(max_workers=num_threads)
+                # non consumed map results block the worker that produced them, hence it makes it compatible with self.slow()
                 yield from executor.map(func, self)
                 executor.shutdown()
 
             return Pipe(iter(iterable()))
 
-    def explode(self) -> "Pipe":
+    def explode(self: List[R]) -> "Pipe[R]":
         return _ExplodingPipe(self)
 
     def filter(self, predicate: Callable[[T], bool]) -> "Pipe[R]":
         return Pipe(filter(predicate, self))
 
     def batch(
         self, max_size: int = 100, max_window_seconds: float = float("inf")
@@ -75,20 +76,20 @@
         def iterate():
             for _ in self:
                 pass
 
         return timeit.timeit(iterate, number=1)
 
 
-class _ExplodingPipe(Pipe[T]):
-    def __init__(self, iterator: Iterator[Iterable[T]]) -> None:
+class _ExplodingPipe(Pipe[R]):
+    def __init__(self, iterator: Iterator[Iterable[R]]) -> None:
         super().__init__(iterator)
         self.current_iterator_elem = iter(super().__next__())
 
-    def __next__(self) -> T:
+    def __next__(self) -> R:
         try:
             return next(self.current_iterator_elem)
         except StopIteration:
             self.current_iterator_elem = iter(super().__next__())
             return next(self)
 
 
@@ -189,22 +190,29 @@
             if batch:
                 return batch
             else:
                 raise
 
 
 class _ConcurrentlyMergingPipe(Pipe[T]):
+    MAX_QUEUE_SIZE = 64
+    MIN_SLEEP_TIME_MS = 0.005
+
     def __init__(self, iterators: List[Iterator[T]]) -> None:
         super().__init__(
             iter(_ConcurrentlyMergingPipe._concurrently_merging_iterable(iterators))
         )
 
     @staticmethod
     def _pull_in_queue(iterator: Iterator[T], queue: Queue) -> None:
         for elem in iterator:
+            backoffed_sleep_time = _ConcurrentlyMergingPipe.MIN_SLEEP_TIME_MS
+            while queue.qsize() > _ConcurrentlyMergingPipe.MAX_QUEUE_SIZE:
+                time.sleep(backoffed_sleep_time)
+                backoffed_sleep_time *= 2
             queue.put(elem)
 
     @staticmethod
     def _concurrently_merging_iterable(iterators: List[Iterator[T]]) -> Iterator[T]:
         queue = Queue()
         with ThreadPoolExecutor(max_workers=len(iterators)) as executor:
             futures = [
```

### Comparing `kissio-0.0.6/test/test.py` & `kissio-0.0.7/test/test.py`

 * *Files identical despite different names*

