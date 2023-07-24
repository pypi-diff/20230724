# Comparing `tmp/namekoplus-0.3.0.tar.gz` & `tmp/namekoplus-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namekoplus-0.3.0.tar", last modified: Mon Jul 24 07:08:27 2023, max compression
+gzip compressed data, was "namekoplus-0.3.1.tar", last modified: Mon Jul 24 10:03:44 2023, max compression
```

## Comparing `namekoplus-0.3.0.tar` & `namekoplus-0.3.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 07:08:12.000000 namekoplus-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 07:08:12.000000 namekoplus-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-24 07:08:27.299468 namekoplus-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-24 07:08:12.000000 namekoplus-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/chassis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/chassis/chassis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/chassis-agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/chassis-agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/chassis-agent/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/templates/all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/all/all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/all/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/demo/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/demo/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/event/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/event/events_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/http/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/http/http_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/rpc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/rpc/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/timer/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/timer/timer_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/tests/unit/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:08:27.299468 namekoplus-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-24 07:08:12.000000 namekoplus-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.340063 namekoplus-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 10:03:32.000000 namekoplus-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 10:03:32.000000 namekoplus-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-24 10:03:44.340063 namekoplus-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-24 10:03:32.000000 namekoplus-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/chassis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/chassis/chassis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/chassis-agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/chassis-agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/chassis-agent/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/templates/all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/all/all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/all/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/templates/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/demo/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/demo/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/templates/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/event/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/event/events_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/templates/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/http/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/http/http_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/templates/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/rpc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/rpc/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus/templates/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/timer/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/templates/timer/timer_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.340063 namekoplus-0.3.1/namekoplus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.340063 namekoplus-0.3.1/namekoplus/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 10:03:32.000000 namekoplus-0.3.1/namekoplus/tests/unit/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:44.336063 namekoplus-0.3.1/namekoplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-24 10:03:44.000000 namekoplus-0.3.1/namekoplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-24 10:03:44.000000 namekoplus-0.3.1/namekoplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:03:44.000000 namekoplus-0.3.1/namekoplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 10:03:44.000000 namekoplus-0.3.1/namekoplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 10:03:44.000000 namekoplus-0.3.1/namekoplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 10:03:44.000000 namekoplus-0.3.1/namekoplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:03:44.340063 namekoplus-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-24 10:03:32.000000 namekoplus-0.3.1/setup.py
```

### Comparing `namekoplus-0.3.0/LICENSE` & `namekoplus-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/PKG-INFO` & `namekoplus-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.3.0
+Version: 0.3.1
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
```

### Comparing `namekoplus-0.3.0/namekoplus/chassis/chassis.py` & `namekoplus-0.3.1/namekoplus/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml` & `namekoplus-0.3.1/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/command.py` & `namekoplus-0.3.1/namekoplus/command.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/all/all_demo.py` & `namekoplus-0.3.1/namekoplus/templates/all/all_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/all/config.yml` & `namekoplus-0.3.1/namekoplus/templates/all/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/event/config.yml` & `namekoplus-0.3.1/namekoplus/templates/event/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/event/events_demo.py` & `namekoplus-0.3.1/namekoplus/templates/event/events_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/http/config.yml` & `namekoplus-0.3.1/namekoplus/templates/http/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/http/http_demo.py` & `namekoplus-0.3.1/namekoplus/templates/http/http_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/rpc/config.yml` & `namekoplus-0.3.1/namekoplus/templates/rpc/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/rpc/rpc_demo.py` & `namekoplus-0.3.1/namekoplus/templates/rpc/rpc_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/templates/timer/config.yml` & `namekoplus-0.3.1/namekoplus/templates/timer/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/namekoplus/tests/unit/test_service.py` & `namekoplus-0.3.1/namekoplus/tests/unit/test_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 """
 Service unit testing best practice.
 """
 
+import pytest
 from nameko.testing.services import worker_factory
 
 
-def test_example_service():
+@pytest.mark.parametrize(
+    'value, expected',
+    [
+        ('John Doe', 'Hello, John Doe!'),
+        ('', 'Hello, !'),
+        ('Bryant', 'Hello, Bryant!'),
+    ],
+)
+def test_example_service(value, expected):
     """
     Test example service.
     """
     # create worker with mock dependencies
     service = worker_factory(ServiceName)  # TODO replace ServiceName with the name of the service and import it
 
     # add side effects to the mock rpc dependency on the "remote" service
     service.remote.hello.side_effect = lambda name: "Hello, {}!".format(name)
 
     # test remote_hello business logic
-    assert service.remote_hello("Bryant") == "Hello, Bryant!"
-    service.remote.hello.assert_called_once_with("Bryant")
+    assert service.remote_hello(value) == expected
+    service.remote.hello.assert_called_once_with(value)
```

### Comparing `namekoplus-0.3.0/namekoplus.egg-info/PKG-INFO` & `namekoplus-0.3.1/namekoplus.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.3.0
+Version: 0.3.1
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
```

### Comparing `namekoplus-0.3.0/namekoplus.egg-info/SOURCES.txt` & `namekoplus-0.3.1/namekoplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `namekoplus-0.3.0/setup.py` & `namekoplus-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='namekoplus',
-    version='0.3.0',
+    version='0.3.1',
     description='A lightweight Python distributed microservice solution',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     project_urls={
         'Documentation': 'https://doc.bearcatlog.com/',
         'Source Code': 'https://github.com/Bryanthelol/namekoplus',
```

