# Comparing `tmp/pynisher-1.0.7.tar.gz` & `tmp/pynisher-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynisher-1.0.7.tar", last modified: Wed Jul 19 09:30:54 2023, max compression
+gzip compressed data, was "pynisher-1.0.8.tar", last modified: Mon Jul 24 09:34:42 2023, max compression
```

## Comparing `pynisher-1.0.7.tar` & `pynisher-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-19 09:30:54.340418 pynisher-1.0.7/
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1076 2023-03-13 20:53:22.000000 pynisher-1.0.7/LICENSE
--rw-r--r--   0 skantify  (1000) skantify  (1000)       37 2023-03-13 20:53:22.000000 pynisher-1.0.7/MANIFEST.in
--rw-r--r--   0 skantify  (1000) skantify  (1000)    14610 2023-07-19 09:30:54.340418 pynisher-1.0.7/PKG-INFO
--rw-r--r--   0 skantify  (1000) skantify  (1000)    13817 2023-07-19 09:28:17.000000 pynisher-1.0.7/README.md
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-19 09:30:54.340418 pynisher-1.0.7/pynisher/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      723 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/__init__.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      545 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/exceptions.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-19 09:30:54.340418 pynisher-1.0.7/pynisher/limiters/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      213 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/limiters/__init__.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)    11791 2023-07-17 09:27:44.000000 pynisher-1.0.7/pynisher/limiters/limiter.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2625 2023-07-17 09:31:11.000000 pynisher-1.0.7/pynisher/limiters/linux.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3214 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/limiters/mac.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4995 2023-07-17 09:27:44.000000 pynisher-1.0.7/pynisher/limiters/windows.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/py.typed
--rw-r--r--   0 skantify  (1000) skantify  (1000)    26738 2023-07-19 09:29:55.000000 pynisher-1.0.7/pynisher/pynisher.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3181 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/support.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6757 2023-03-14 15:30:00.000000 pynisher-1.0.7/pynisher/util.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      924 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/win_errcodes.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-19 09:30:54.340418 pynisher-1.0.7/pynisher.egg-info/
--rw-r--r--   0 skantify  (1000) skantify  (1000)    14610 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/PKG-INFO
--rw-r--r--   0 skantify  (1000) skantify  (1000)      497 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/SOURCES.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)        1 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/dependency_links.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)      171 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/requires.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)        9 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/top_level.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3029 2023-07-17 09:28:49.000000 pynisher-1.0.7/pyproject.toml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       38 2023-07-19 09:30:54.340418 pynisher-1.0.7/setup.cfg
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1600 2023-07-19 09:28:03.000000 pynisher-1.0.7/setup.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-24 09:34:42.587899 pynisher-1.0.8/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1076 2023-03-13 20:53:22.000000 pynisher-1.0.8/LICENSE
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       37 2023-03-13 20:53:22.000000 pynisher-1.0.8/MANIFEST.in
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    14610 2023-07-24 09:34:42.587899 pynisher-1.0.8/PKG-INFO
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    13817 2023-07-19 09:28:17.000000 pynisher-1.0.8/README.md
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-24 09:34:42.587899 pynisher-1.0.8/pynisher/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      723 2023-03-13 20:53:22.000000 pynisher-1.0.8/pynisher/__init__.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      545 2023-03-13 20:53:22.000000 pynisher-1.0.8/pynisher/exceptions.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-24 09:34:42.587899 pynisher-1.0.8/pynisher/limiters/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      213 2023-03-13 20:53:22.000000 pynisher-1.0.8/pynisher/limiters/__init__.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    11811 2023-07-24 09:28:45.000000 pynisher-1.0.8/pynisher/limiters/limiter.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2625 2023-07-24 09:29:21.000000 pynisher-1.0.8/pynisher/limiters/linux.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3844 2023-07-24 09:29:48.000000 pynisher-1.0.8/pynisher/limiters/mac.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4995 2023-07-17 09:27:44.000000 pynisher-1.0.8/pynisher/limiters/windows.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-03-13 20:53:22.000000 pynisher-1.0.8/pynisher/py.typed
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    27643 2023-07-24 09:29:29.000000 pynisher-1.0.8/pynisher/pynisher.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3181 2023-03-13 20:53:22.000000 pynisher-1.0.8/pynisher/support.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6757 2023-03-14 15:30:00.000000 pynisher-1.0.8/pynisher/util.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      924 2023-03-13 20:53:22.000000 pynisher-1.0.8/pynisher/win_errcodes.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-24 09:34:42.587899 pynisher-1.0.8/pynisher.egg-info/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    14610 2023-07-24 09:34:42.000000 pynisher-1.0.8/pynisher.egg-info/PKG-INFO
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      497 2023-07-24 09:34:42.000000 pynisher-1.0.8/pynisher.egg-info/SOURCES.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        1 2023-07-24 09:34:42.000000 pynisher-1.0.8/pynisher.egg-info/dependency_links.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      171 2023-07-24 09:34:42.000000 pynisher-1.0.8/pynisher.egg-info/requires.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        9 2023-07-24 09:34:42.000000 pynisher-1.0.8/pynisher.egg-info/top_level.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3029 2023-07-17 09:28:49.000000 pynisher-1.0.8/pyproject.toml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       38 2023-07-24 09:34:42.587899 pynisher-1.0.8/setup.cfg
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1600 2023-07-24 09:24:54.000000 pynisher-1.0.8/setup.py
```

### Comparing `pynisher-1.0.7/LICENSE` & `pynisher-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/PKG-INFO` & `pynisher-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynisher
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library to limit the resources used by functions using subprocesses
 Home-page: https://github.com/automl/pynisher
 Author: ('Stefan Falkner, Christina Hernandez-Wunsch, Samuel Mueller,Matthias Feurer, Francisco Rivera, Eddie Bergman and Rene Sass',)
 Author-email: feurerm@informatik.uni-freiburg.de
 License: MIT
 Keywords: resources
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pynisher-1.0.7/README.md` & `pynisher-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/pynisher/__init__.py` & `pynisher-1.0.8/pynisher/__init__.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/pynisher/exceptions.py` & `pynisher-1.0.8/pynisher/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/pynisher/limiters/limiter.py` & `pynisher-1.0.8/pynisher/limiters/limiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,21 +121,21 @@
                 self.limit_memory(self.memory)
 
             # Call our function
             result = self.func(*args, **kwargs)
             error = None
             tb = None
 
-        except Exception as e:
+        except BaseException as e:
             result = None
             error = e
             tb = "".join(traceback.format_exception(*sys.exc_info()))
 
         if error is not None:
-            error = self._wrap_error(error, *args, **kwargs)
+            error = self._wrap_error(error, *args, **kwargs)  # type: ignore
 
         # Now let's try to send the result back
         response = (result, error, tb)
         try:
             self.output.send(response)
             self.output.close()
             if self.terminate_child_processes is True:
```

### Comparing `pynisher-1.0.7/pynisher/limiters/linux.py` & `pynisher-1.0.8/pynisher/limiters/linux.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/pynisher/limiters/mac.py` & `pynisher-1.0.8/pynisher/limiters/mac.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,19 +22,39 @@
 # https://github.com/apple/darwin-xnu/blob/2ff845c2e033bd0ff64b5b6aa6063a1f8f65aa32/bsd/kern/kern_resource.c#L987
 
 This module and the Linux limiter share almost identical code but we keep them seperate
 incase of specific modules or changes needed
 """
 from __future__ import annotations
 
+from typing import Any
+
 import resource
 
+from pynisher.exceptions import CpuTimeoutException
 from pynisher.limiters.limiter import Limiter
 
 
+def raise_on_cpu_limit(signum: Any, frame: Any) -> None:
+    """Raise a `RuntimeError` when the CPU limit is reached.
+
+    This is a signal handler for `SIGXCPU` which is sent when the CPU time limit
+    is reached. This is a signal that is sent to the process, not the thread, so
+    we need to make sure that we only raise the exception in the main thread.
+
+    Parameters
+    ----------
+    signum : int
+        The signal number
+    frame : FrameType
+        The current stack frame
+    """
+    raise CpuTimeoutException("CPU time limit exceeded")
+
+
 class LimiterMac(Limiter):
     def limit_memory(self, memory: int) -> None:
         """Limit the addressable memory
 
         It seems that each of RLIMIT_AS, RLIMIT_DATA and RLIMIT_RSS do nothing.
         While they do set, nothing is done when those boundaries are exceeded.
```

### Comparing `pynisher-1.0.7/pynisher/limiters/windows.py` & `pynisher-1.0.8/pynisher/limiters/windows.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/pynisher/pynisher.py` & `pynisher-1.0.8/pynisher/pynisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
-from multiprocessing.context import BaseContext
 
 from typing import Any, Callable, Generic, Type, TypeVar, overload
 
 import multiprocessing
 import signal
 import sys
+import time
 from functools import wraps
+from multiprocessing.context import BaseContext
 
 import psutil
 from typing_extensions import Literal, ParamSpec
 
 from pynisher.exceptions import (
     CpuTimeoutException,
     MemoryLimitException,
@@ -357,26 +358,88 @@
         # Get a psutil handle to the process
         try:
             self._process = psutil.Process(subprocess.pid)
         except psutil.NoSuchProcess:
             # Likely only to occur when subprocess already finished
             pass
 
+        # 4 kinds of `response` we expect
+        #
+        # * (result, None, None)    | success
+        #                               => No error, we got a result
+        # * (None, error, traceback)| failed
+        #                               =>  Error, CPUtimeout linux/mac, MemoryError
+        # * None                    | failed
+        #                               => MemoryError during sending of real error
+        # * EMPTY                   | failed, nothing received from pipe
+        #                               => Walltime, CPUTimeout windows, Unknown
+        result: _EMPTY | T = EMPTY
+        err: Exception | None = None
+        tb: str | None = None
+
+        # Retrieve a result if we can. We have to manually loop this because if the
+        # subprocess abruptly crashes in such a way that the pipe never closes, we will
+        # hang forever
+        start = time.time()
+        interval = 0.01
+        try:
+            while True:
+                if (
+                    self.wall_time is not None
+                    and (time.time() - start) > self.wall_time
+                ):
+                    result = EMPTY
+                    tb = None
+                    err = WallTimeoutException(
+                        f"Your function took longer than {self.wall_time} seconds to"
+                        f" run.\n{callstring(self.func, *args, **kwargs)}",
+                    )
+                    break
+                elif receive_pipe.poll(interval):
+                    response = receive_pipe.recv()
+                    if response is not None:
+                        result, err, tb = response
+                    else:
+                        result = EMPTY
+                        tb = None
+                        err = MemoryLimitException(
+                            "While returning the result from your function,"
+                            " we could not retrieve the result or any error"
+                            " about why."
+                            f"\n{callstring(self.func, *args, **kwargs)}",
+                        )
+                    break
+                elif not subprocess.is_alive():
+                    result = EMPTY
+                    tb = None
+                    err = None
+                    break
+
+        # Otherwise, there was nothing to read
+        except EOFError:
+            result = EMPTY
+            tb = None
+            err = MemoryLimitException(
+                "There but could not a send response back."
+                " This is likely a MemoryError."
+                f"\n{callstring(self.func, *args, **kwargs)}"
+            )
+
         # If self.wall time is None, block until the subprocess finishes or
         # terminates. Otherwise, will return after wall_time and the process
         # will still be running
         if not self.forceful_keyboard_interrupt:
-            subprocess.join(self.wall_time)
+            subprocess.join(timeout=0.1)
         else:
             # The keyboard interrupt will be send to all processes simultaneuously
             # and handled by each of them. The default behaviour is to terminate
             # but this can be caught by a subprocess and ignored. To circumvent
             # this, we convert this keyboard interrupt into a SIGTERM and propgate it
             try:
-                subprocess.join(self.wall_time)
+                subprocess.join(timeout=0.1)
             except KeyboardInterrupt:
                 terminate_process(
                     subprocess.pid,
                     children=self.terminate_child_processes,
                     parent=True,
                 )
                 raise KeyboardInterrupt
@@ -391,54 +454,14 @@
 
         terminate_process(
             subprocess.pid,
             children=self.terminate_child_processes,
             parent=True,
         )
 
-        # 4 kinds of `response` we expect
-        #
-        # * (result, None, None)    | success
-        #                               => No error, we got a result
-        # * (None, error, traceback)| failed
-        #                               =>  Error, CPUtimeout linux/mac, MemoryError
-        # * None                    | failed
-        #                               => MemoryError during sending of real error
-        # * EMPTY                   | failed, nothing received from pipe
-        #                               => Walltime, CPUTimeout windows, Unknown
-        result: _EMPTY | T = EMPTY
-        err: Exception | None = None
-        tb: str | None = None
-
-        # Retrieve a result if we can,
-        if receive_pipe.poll() and not receive_pipe.closed:
-            try:
-                response = receive_pipe.recv()
-                if response is not None:
-                    result, err, tb = response
-                else:
-                    result = EMPTY
-                    tb = None
-                    err = MemoryLimitException(
-                        "While returning the result from your function,"
-                        " we could not retrieve the result or any error"
-                        " about why."
-                        f"\n{callstring(self.func, *args, **kwargs)}",
-                    )
-
-            # Otherwise, there was nothing to read
-            except EOFError:
-                result = EMPTY
-                tb = None
-                err = MemoryLimitException(
-                    "There but could not a send response back."
-                    " This is likely a MemoryError."
-                    f"\n{callstring(self.func, *args, **kwargs)}"
-                )
-
         # Cleanup pipes
         receive_pipe.close()
         send_pipe.close()
 
         # We got a result or an error
         if result is not EMPTY or err is not None:
             # If an error, the result must be empty
```

### Comparing `pynisher-1.0.7/pynisher/support.py` & `pynisher-1.0.8/pynisher/support.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/pynisher/util.py` & `pynisher-1.0.8/pynisher/util.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/pynisher/win_errcodes.py` & `pynisher-1.0.8/pynisher/win_errcodes.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/pynisher.egg-info/PKG-INFO` & `pynisher-1.0.8/pynisher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynisher
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library to limit the resources used by functions using subprocesses
 Home-page: https://github.com/automl/pynisher
 Author: ('Stefan Falkner, Christina Hernandez-Wunsch, Samuel Mueller,Matthias Feurer, Francisco Rivera, Eddie Bergman and Rene Sass',)
 Author-email: feurerm@informatik.uni-freiburg.de
 License: MIT
 Keywords: resources
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pynisher-1.0.7/pyproject.toml` & `pynisher-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.7/setup.py` & `pynisher-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 readme = Path(__file__).parent / "README.md"
 
 with readme.open("r") as fh:
     long_description = fh.read()
 
 setup(
     name="pynisher",
-    version="1.0.7",
+    version="1.0.8",
     packages=find_packages(where=".", include=["pynisher*"], exclude=["test*"]),
     include_package_data=True,
     install_requires=[
         "psutil",
         "typing_extensions",
         "pywin32; platform_system=='Windows'",
     ],
```

