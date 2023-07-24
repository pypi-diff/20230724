# Comparing `tmp/kissio-0.0.3.tar.gz` & `tmp/kissio-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kissio-0.0.3.tar", last modified: Mon Jul 24 10:38:24 2023, max compression
+gzip compressed data, was "kissio-0.0.4.tar", last modified: Mon Jul 24 10:46:25 2023, max compression
```

## Comparing `kissio-0.0.3.tar` & `kissio-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:24.806990 kissio-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 10:38:14.000000 kissio-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 10:38:24.806990 kissio-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 10:38:14.000000 kissio-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:24.806990 kissio-0.0.3/kissio/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 10:38:14.000000 kissio-0.0.3/kissio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-24 10:38:14.000000 kissio-0.0.3/kissio/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:24.806990 kissio-0.0.3/kissio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 10:38:24.000000 kissio-0.0.3/kissio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 10:38:24.000000 kissio-0.0.3/kissio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:38:24.000000 kissio-0.0.3/kissio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 10:38:24.000000 kissio-0.0.3/kissio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:38:24.806990 kissio-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 10:38:14.000000 kissio-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:38:24.806990 kissio-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-24 10:38:14.000000 kissio-0.0.3/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:46:25.985988 kissio-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 10:46:10.000000 kissio-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 10:46:25.985988 kissio-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 10:46:10.000000 kissio-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:46:25.985988 kissio-0.0.4/kissio/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 10:46:10.000000 kissio-0.0.4/kissio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-24 10:46:10.000000 kissio-0.0.4/kissio/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:46:25.985988 kissio-0.0.4/kissio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 10:46:25.000000 kissio-0.0.4/kissio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 10:46:25.000000 kissio-0.0.4/kissio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:46:25.000000 kissio-0.0.4/kissio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 10:46:25.000000 kissio-0.0.4/kissio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:46:25.985988 kissio-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 10:46:10.000000 kissio-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:46:25.985988 kissio-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-24 10:46:10.000000 kissio-0.0.4/test/test.py
```

### Comparing `kissio-0.0.3/LICENSE` & `kissio-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kissio-0.0.3/README.md` & `kissio-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kissio-0.0.3/kissio/pipe.py` & `kissio-0.0.4/kissio/pipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -151,26 +151,23 @@
 
 
 class _SlowingIterator(Pipe[T]):
     def __init__(self, iterator: Iterator[T], freq: int) -> None:
         super().__init__(iterator)
         self.freq = freq
         self.start = None
-        self.num_yielded_elements = 0
+        self.yields_count = 0
 
     def __next__(self) -> T:
         if not self.start:
             self.start = time.time()
         while True:
-            while (
-                self.num_yielded_elements
-                > (time.time() - self.start) * self.freq
-            ):
+            while self.yields_count > (time.time() - self.start) * self.freq:
                 time.sleep(1 / self.freq)
-            self.num_yielded_elements += 1
+            self.yields_count += 1
             return super().__next__()
 
 
 class _BatchingPipe(Pipe[List[T]]):
     def __init__(
         self, iterator: Iterator[T], max_size: int, max_window_seconds: float
     ) -> None:
```

### Comparing `kissio-0.0.3/test/test.py` & `kissio-0.0.4/test/test.py`

 * *Files identical despite different names*

