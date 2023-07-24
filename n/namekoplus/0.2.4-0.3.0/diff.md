# Comparing `tmp/namekoplus-0.2.4.tar.gz` & `tmp/namekoplus-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namekoplus-0.2.4.tar", last modified: Sat Jul 22 16:14:37 2023, max compression
+gzip compressed data, was "namekoplus-0.3.0.tar", last modified: Mon Jul 24 07:08:27 2023, max compression
```

## Comparing `namekoplus-0.2.4.tar` & `namekoplus-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.596272 namekoplus-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-22 16:14:21.000000 namekoplus-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-22 16:14:21.000000 namekoplus-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-22 16:14:37.596272 namekoplus-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-22 16:14:21.000000 namekoplus-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.592272 namekoplus-0.2.4/namekoplus/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.592272 namekoplus-0.2.4/namekoplus/chassis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/chassis/chassis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.592272 namekoplus-0.2.4/namekoplus/chassis-agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/chassis-agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.592272 namekoplus-0.2.4/namekoplus/chassis-agent/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.592272 namekoplus-0.2.4/namekoplus/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.592272 namekoplus-0.2.4/namekoplus/templates/all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/all/all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/all/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.596272 namekoplus-0.2.4/namekoplus/templates/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/demo/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/demo/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.596272 namekoplus-0.2.4/namekoplus/templates/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/event/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/event/events_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.596272 namekoplus-0.2.4/namekoplus/templates/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/http/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/http/http_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.596272 namekoplus-0.2.4/namekoplus/templates/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/rpc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/rpc/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.596272 namekoplus-0.2.4/namekoplus/templates/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/timer/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-22 16:14:21.000000 namekoplus-0.2.4/namekoplus/templates/timer/timer_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:14:37.592272 namekoplus-0.2.4/namekoplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-22 16:14:37.000000 namekoplus-0.2.4/namekoplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-22 16:14:37.000000 namekoplus-0.2.4/namekoplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:14:37.000000 namekoplus-0.2.4/namekoplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-22 16:14:37.000000 namekoplus-0.2.4/namekoplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-22 16:14:37.000000 namekoplus-0.2.4/namekoplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 16:14:37.000000 namekoplus-0.2.4/namekoplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:14:37.596272 namekoplus-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-22 16:14:21.000000 namekoplus-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 07:08:12.000000 namekoplus-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-24 07:08:12.000000 namekoplus-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-24 07:08:27.299468 namekoplus-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-24 07:08:12.000000 namekoplus-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/chassis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/chassis/chassis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/chassis-agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/chassis-agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/chassis-agent/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus/templates/all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/all/all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/all/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/demo/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/demo/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/event/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/event/events_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/http/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/http/http_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/rpc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/rpc/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/templates/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/timer/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/templates/timer/timer_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.299468 namekoplus-0.3.0/namekoplus/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 07:08:12.000000 namekoplus-0.3.0/namekoplus/tests/unit/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:27.295468 namekoplus-0.3.0/namekoplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 07:08:27.000000 namekoplus-0.3.0/namekoplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:08:27.299468 namekoplus-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-24 07:08:12.000000 namekoplus-0.3.0/setup.py
```

### Comparing `namekoplus-0.2.4/LICENSE` & `namekoplus-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/PKG-INFO` & `namekoplus-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.2.4
+Version: 0.3.0
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
@@ -20,15 +20,15 @@
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: ha
 Provides-Extra: apiflask
 Provides-Extra: rocketry
 Provides-Extra: gutter
 Provides-Extra: mysql
-Provides-Extra: ssl
+Provides-Extra: security
 Provides-Extra: dev
 License-File: LICENSE
 
 # namekoplus
 
 A lightweight Python distributed microservice solution
```

### Comparing `namekoplus-0.2.4/namekoplus/chassis/chassis.py` & `namekoplus-0.3.0/namekoplus/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml` & `namekoplus-0.3.0/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/command.py` & `namekoplus-0.3.0/namekoplus/command.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from contextlib import contextmanager
 
 import click
 from python_on_whales import DockerException, ClientNotFoundError, DockerClient, docker as docker_testing
 
 
 def check_docker():
+    """
+    Check if docker and docker compose are installed and running.
+    """
     try:
         docker_testing.ps()
     except ClientNotFoundError:
         click.echo('Please install docker first', err=True)
         raise
     except DockerException:
         click.echo('Please start docker correctly', err=True)
@@ -19,45 +22,49 @@
     if not docker_testing.compose.is_installed():
         click.echo('Please install docker-compose first', err=True)
         raise
 
 
 @contextmanager
 def status(status_msg: str, newline: bool = False, quiet: bool = False):
+    """
+    Show status message and yield.
+    """
     msg_suffix = ' ...' if not newline else ' ...\n'
     click.echo(status_msg + msg_suffix)
     try:
         yield
     except Exception as e:
         if not quiet:
             click.echo('  FAILED\n')
         raise
     else:
         if not quiet:
             click.echo('  Done\n')
 
 
-def get_template_directory() -> str:
+def get_directory(dir_name: str) -> str:
     """
-    Return the directory where nameko_plus setup templates are found.
+    Return the directory path of the given nameko-plus directory name.
     """
     import namekoplus
 
     package_dir = os.path.abspath(os.path.dirname(namekoplus.__file__))
-    return os.path.join(package_dir, 'templates')
+    return os.path.join(package_dir, dir_name)
 
 
-def get_agent_directory() -> str:
-    """
-    Return the directory where nameko_plus setup agent are found.
-    """
-    import namekoplus
+def copy_files(src_dir, dest_dir):
+    for file_ in os.listdir(src_dir):
+        if file_ == '__pycache__':
+            continue
 
-    package_dir = os.path.abspath(os.path.dirname(namekoplus.__file__))
-    return os.path.join(package_dir, 'chassis-agent')
+        src_file_path = os.path.join(src_dir, file_)
+        output_file = os.path.join(dest_dir, file_)
+        with status(f'Generating {os.path.abspath(output_file)}'):
+            shutil.copy(src_file_path, output_file)
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -74,32 +81,24 @@
     """
     Initialize a new service via templates.
     """
     if os.access(directory, os.F_OK) and os.listdir(directory):
         click.echo('Directory {} already exists and is not empty'.format(directory), err=True)
         return
 
-    template_dir = os.path.join(get_template_directory(), _type)
+    template_dir = os.path.join(get_directory('templates'), _type)
     if not os.access(template_dir, os.F_OK):
         click.echo('No such template type {}'.format(_type), err=True)
         return
 
-    # 创建目录
     if not os.access(directory, os.F_OK):
         with status(f'Creating directory {os.path.abspath(directory)!r}'):
             os.makedirs(directory)
 
-    # 把 templates 放入新建的目录
-    for file_ in os.listdir(template_dir):
-        if file_ == '__pycache__':
-            continue
-        src_file_path = os.path.join(template_dir, file_)
-        output_file = os.path.join(directory, file_)
-        with status(f'Generating {os.path.abspath(output_file)}'):
-            shutil.copy(src_file_path, output_file)
+    copy_files(template_dir, directory)
 
 
 @cli.command()
 @click.option('-m', '--middleware',
               required=True,
               type=click.Choice(['rabbitmq'], case_sensitive=False),
               help='The middleware name')
@@ -115,15 +114,15 @@
     """
     check_docker()
 
     if user and password:
         os.environ['RABBITMQ_DEFAULT_USER'] = user
         os.environ['RABBITMQ_DEFAULT_PASS'] = password
 
-    docker_compose_file_dir = os.path.join(get_agent_directory(), middleware)
+    docker_compose_file_dir = os.path.join(get_directory('chassis-agent'), middleware)
     for file_ in os.listdir(docker_compose_file_dir):
         compose_file_path = os.path.join(docker_compose_file_dir, file_)
         with status(f'Starting {middleware}'):
             docker = DockerClient(compose_files=[compose_file_path])
             docker.compose.up(detach=True)
 
 
@@ -134,17 +133,42 @@
               help='The middleware name')
 def stop(middleware):
     """
     Stop a middleware that the nameko service depends on.
     """
     check_docker()
 
-    docker_compose_file_dir = os.path.join(get_agent_directory(), middleware)
+    docker_compose_file_dir = os.path.join(get_directory('chassis-agent'), middleware)
     for file_ in os.listdir(docker_compose_file_dir):
         compose_file_path = os.path.join(docker_compose_file_dir, file_)
         with status(f'Stopping {middleware}'):
             docker = DockerClient(compose_files=[compose_file_path])
             docker.compose.down()
 
 
+@cli.command()
+@click.option('-e', '--existed_dir', 'directory',
+              required=True,
+              help='The existed directory name of the nameko service')
+@click.option('-t', '--type', '_type',
+              default='unit',
+              show_default=True,
+              type=click.Choice(['unit'], case_sensitive=False),
+              help='The test type of the nameko service')
+def test_gen(directory, _type):
+    """
+    Generate test files for nameko services.
+    """
+    if not os.access(directory, os.F_OK) or not os.listdir(directory):
+        click.echo('Directory {} dose not exist or is empty'.format(directory), err=True)
+        return
+
+    tests_dir = os.path.join(get_directory('tests'), _type)
+    if not os.access(tests_dir, os.F_OK):
+        click.echo('No such test type {}'.format(_type), err=True)
+        return
+
+    copy_files(tests_dir, directory)
+
+
 if __name__ == '__main__':
     cli()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `namekoplus-0.2.4/namekoplus/templates/all/all_demo.py` & `namekoplus-0.3.0/namekoplus/templates/all/all_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/templates/all/config.yml` & `namekoplus-0.3.0/namekoplus/templates/all/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/templates/event/config.yml` & `namekoplus-0.3.0/namekoplus/templates/event/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/templates/event/events_demo.py` & `namekoplus-0.3.0/namekoplus/templates/event/events_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/templates/http/config.yml` & `namekoplus-0.3.0/namekoplus/templates/http/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/templates/http/http_demo.py` & `namekoplus-0.3.0/namekoplus/templates/http/http_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/templates/rpc/config.yml` & `namekoplus-0.3.0/namekoplus/templates/rpc/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/templates/rpc/rpc_demo.py` & `namekoplus-0.3.0/namekoplus/templates/rpc/rpc_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus/templates/timer/config.yml` & `namekoplus-0.3.0/namekoplus/templates/timer/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.4/namekoplus.egg-info/PKG-INFO` & `namekoplus-0.3.0/namekoplus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.2.4
+Version: 0.3.0
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
@@ -20,15 +20,15 @@
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: ha
 Provides-Extra: apiflask
 Provides-Extra: rocketry
 Provides-Extra: gutter
 Provides-Extra: mysql
-Provides-Extra: ssl
+Provides-Extra: security
 Provides-Extra: dev
 License-File: LICENSE
 
 # namekoplus
 
 A lightweight Python distributed microservice solution
```

### Comparing `namekoplus-0.2.4/namekoplus.egg-info/SOURCES.txt` & `namekoplus-0.3.0/namekoplus.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,8 +28,11 @@
 namekoplus/templates/http/config.yml
 namekoplus/templates/http/http_demo.py
 namekoplus/templates/rpc/__init__.py
 namekoplus/templates/rpc/config.yml
 namekoplus/templates/rpc/rpc_demo.py
 namekoplus/templates/timer/__init__.py
 namekoplus/templates/timer/config.yml
-namekoplus/templates/timer/timer_demo.py
+namekoplus/templates/timer/timer_demo.py
+namekoplus/tests/__init__.py
+namekoplus/tests/unit/__init__.py
+namekoplus/tests/unit/test_service.py
```

### Comparing `namekoplus-0.2.4/setup.py` & `namekoplus-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='namekoplus',
-    version='0.2.4',
+    version='0.3.0',
     description='A lightweight Python distributed microservice solution',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     project_urls={
         'Documentation': 'https://doc.bearcatlog.com/',
         'Source Code': 'https://github.com/Bryanthelol/namekoplus',
@@ -67,12 +67,12 @@
                      'gunicorn==20.1.0'],
         'rocketry': ['rocketry==2.4.0'],
         'gutter': ['gutter==0.5.0'],
         'mysql': ['pymysql==1.0.3',
                   'sqlalchemy==2.0.15',
                   'sqlacodegen==2.3.0',
                   'alembic==1.11.1'],
-        'ssl': ['cryptography'],
+        'security': ['cryptography'],
         'dev': ['mako==1.2.4',
                 'environs==9.5.0']
     },
 )
```

