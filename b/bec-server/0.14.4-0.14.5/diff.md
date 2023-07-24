# Comparing `tmp/bec-server-0.14.4.tar.gz` & `tmp/bec-server-0.14.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.14.4.tar", last modified: Mon Jul 24 15:02:34 2023, max compression
+gzip compressed data, was "bec-server-0.14.5.tar", last modified: Mon Jul 24 17:00:37 2023, max compression
```

## Comparing `bec-server-0.14.4.tar` & `bec-server-0.14.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:34.881447 bec-server-0.14.4/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 15:02:34.882447 bec-server-0.14.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:34.880447 bec-server-0.14.4/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.4/bec_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.4/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.4/bec_server/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.4/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:02:34.881447 bec-server-0.14.4/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 15:02:34.000000 bec-server-0.14.4/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-24 15:02:34.882447 bec-server-0.14.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2073 2023-07-24 15:02:01.000000 bec-server-0.14.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:37.642593 bec-server-0.14.5/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 17:00:37.642593 bec-server-0.14.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:37.641593 bec-server-0.14.5/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.5/bec_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.5/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.5/bec_server/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.5/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:37.642593 bec-server-0.14.5/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-24 17:00:37.000000 bec-server-0.14.5/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-24 17:00:37.000000 bec-server-0.14.5/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 17:00:37.000000 bec-server-0.14.5/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 17:00:37.000000 bec-server-0.14.5/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-24 17:00:37.000000 bec-server-0.14.5/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 17:00:37.000000 bec-server-0.14.5/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-24 17:00:37.643593 bec-server-0.14.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-24 17:00:09.000000 bec-server-0.14.5/setup.py
```

### Comparing `bec-server-0.14.4/bec_server/launch.py` & `bec-server-0.14.5/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.4/bec_server/service_handler.py` & `bec-server-0.14.5/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.4/bec_server/tmux_launch.py` & `bec-server-0.14.5/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.4/setup.py` & `bec-server-0.14.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 import subprocess
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "0.14.4"
+__version__ = "0.14.5"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

