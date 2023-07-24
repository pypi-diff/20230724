# Comparing `tmp/bec-server-0.14.1.tar.gz` & `tmp/bec-server-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.14.1.tar", last modified: Mon Jul 24 11:48:11 2023, max compression
+gzip compressed data, was "bec-server-0.14.3.tar", last modified: Mon Jul 24 12:06:02 2023, max compression
```

## Comparing `bec-server-0.14.1.tar` & `bec-server-0.14.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:48:11.118708 bec-server-0.14.1/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 11:48:11.118708 bec-server-0.14.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:48:11.117708 bec-server-0.14.1/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:25:17.000000 bec-server-0.14.1/bec_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-07-23 06:17:58.000000 bec-server-0.14.1/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:25:17.000000 bec-server-0.14.1/bec_server/service_handler.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-07-23 06:17:58.000000 bec-server-0.14.1/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 11:48:11.118708 bec-server-0.14.1/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 11:48:11.000000 bec-server-0.14.1/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-24 11:48:11.119707 bec-server-0.14.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1866 2023-07-24 11:47:29.000000 bec-server-0.14.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:06:02.952386 bec-server-0.14.3/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 12:06:02.952386 bec-server-0.14.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:06:02.951386 bec-server-0.14.3/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.3/bec_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.3/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.3/bec_server/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.3/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:06:02.952386 bec-server-0.14.3/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 12:06:02.000000 bec-server-0.14.3/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-24 12:06:02.953385 bec-server-0.14.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-24 12:05:30.000000 bec-server-0.14.3/setup.py
```

### Comparing `bec-server-0.14.1/bec_server/launch.py` & `bec-server-0.14.3/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.1/bec_server/service_handler.py` & `bec-server-0.14.3/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.1/bec_server/tmux_launch.py` & `bec-server-0.14.3/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.1/setup.py` & `bec-server-0.14.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 import subprocess
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "0.14.1"
+__version__ = "0.14.3"
 
 
 def run_install(setup_args, bec_deps, editable=False):
     """
     Run the setup function with the given arguments. If editable is True, the dependencies are installed in editable mode.
     """
     if editable:
```

