# Comparing `tmp/middleware-apm-0.2.0rc4.tar.gz` & `tmp/middleware-apm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-apm-0.2.0rc4.tar", last modified: Fri Jul 21 07:29:22 2023, max compression
+gzip compressed data, was "middleware-apm-0.2.1.tar", last modified: Mon Jul 24 08:57:55 2023, max compression
```

## Comparing `middleware-apm-0.2.0rc4.tar` & `middleware-apm-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:29:22.917500 middleware-apm-0.2.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 07:29:22.917500 middleware-apm-0.2.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:29:22.913500 middleware-apm-0.2.0rc4/middleware_apm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 07:29:22.000000 middleware-apm-0.2.0rc4/middleware_apm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:29:22.917500 middleware-apm-0.2.0rc4/mw_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/mw_tracker/mw_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:29:22.917500 middleware-apm-0.2.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 07:28:55.000000 middleware-apm-0.2.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:57:55.683316 middleware-apm-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-24 08:57:55.683316 middleware-apm-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:57:55.679316 middleware-apm-0.2.1/middleware_apm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-24 08:57:55.000000 middleware-apm-0.2.1/middleware_apm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-24 08:57:55.000000 middleware-apm-0.2.1/middleware_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:57:55.000000 middleware-apm-0.2.1/middleware_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 08:57:55.000000 middleware-apm-0.2.1/middleware_apm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-24 08:57:55.000000 middleware-apm-0.2.1/middleware_apm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 08:57:55.000000 middleware-apm-0.2.1/middleware_apm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:57:55.679316 middleware-apm-0.2.1/mw_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/mw_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/mw_tracker/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/mw_tracker/_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/mw_tracker/_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/mw_tracker/_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/mw_tracker/mw_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:57:55.683316 middleware-apm-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-24 08:57:24.000000 middleware-apm-0.2.1/setup.py
```

### Comparing `middleware-apm-0.2.0rc4/LICENSE` & `middleware-apm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc4/mw_tracker/_logger.py` & `middleware-apm-0.2.1/mw_tracker/_logger.py`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc4/mw_tracker/_meter.py` & `middleware-apm-0.2.1/mw_tracker/_meter.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         unit="Bytes",
         callbacks=[_disk_usage_total_cb, _disk_usage_used_cb, _disk_usage_free_cb],
         description="The will show the disk usage of the process"
     )
 
 
 def _cpu_usage_cb(options: CallbackOptions):
-    print("--- Metrics Generated ---")
+    # print("--- Metrics Generated ---")
     yield Observation(value=psutil.Process(os.getpid()).cpu_percent())
 
 
 def _ram_usage_cb(options: CallbackOptions):
     yield Observation(value=psutil.Process(os.getpid()).memory_percent())
```

### Comparing `middleware-apm-0.2.0rc4/mw_tracker/_profiler.py` & `middleware-apm-0.2.1/mw_tracker/_profiler.py`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc4/mw_tracker/_tracer.py` & `middleware-apm-0.2.1/mw_tracker/_tracer.py`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc4/mw_tracker/mw_tracker.py` & `middleware-apm-0.2.1/mw_tracker/mw_tracker.py`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.2.0rc4/setup.py` & `middleware-apm-0.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 except IOError:
     requirements = []
 
 
 setuptools.setup(
 
     name="middleware-apm",
-    version="0.2.0rc4",
+    version="0.2.1",
     install_requires=requirements,
     author="middleware-dev",
-    description="This package is use to check the RAM and CPU Usage of Current Device.",
+    description="Middleware's APM tool enables Python developers to effortlessly monitor their applications, gathering distributed tracing, metrics, logs, and profiling data for valuable insights and performance optimization. Install the Middleware Host agent and integrate the APM package to leverage its powerful functionalities.",
     long_description=open('README.md').read(),
-    long_description_content_type='text/plain',
+    long_description_content_type='text/markdown',
     packages=["mw_tracker"],
     url = "https://github.com/middleware-labs/agent-apm-python.git",
     entry_points={
         'console_scripts': [
             'middleware-instrument = opentelemetry.instrumentation.auto_instrumentation:run',
             'middleware-bootstrap = opentelemetry.instrumentation.bootstrap:run',
         ],
```

