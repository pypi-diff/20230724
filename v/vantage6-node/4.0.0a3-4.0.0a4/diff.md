# Comparing `tmp/vantage6-node-4.0.0a3.tar.gz` & `tmp/vantage6-node-4.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-4.0.0a3.tar", last modified: Tue Jul 18 15:34:11 2023, max compression
+gzip compressed data, was "vantage6-node-4.0.0a4.tar", last modified: Mon Jul 24 13:22:28 2023, max compression
```

## Comparing `vantage6-node-4.0.0a3.tar` & `vantage6-node-4.0.0a4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.331262 vantage6-node-4.0.0a3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    41597 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/docker/squid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19632 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23828 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-18 15:33:57.000000 vantage6-node-4.0.0a3/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.335262 vantage6-node-4.0.0a3/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-18 15:34:11.000000 vantage6-node-4.0.0a3/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-18 15:34:11.000000 vantage6-node-4.0.0a3/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:34:11.000000 vantage6-node-4.0.0a3/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 15:34:11.000000 vantage6-node-4.0.0a3/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 15:34:11.000000 vantage6-node-4.0.0a3/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 15:34:11.000000 vantage6-node-4.0.0a3/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.184549 vantage6-node-4.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-24 13:22:28.184549 vantage6-node-4.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:28.184549 vantage6-node-4.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    41597 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/squid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19632 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23828 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.180549 vantage6-node-4.0.0a4/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-24 13:22:06.000000 vantage6-node-4.0.0a4/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.184549 vantage6-node-4.0.0a4/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 13:22:28.000000 vantage6-node-4.0.0a4/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-4.0.0a3/PKG-INFO` & `vantage6-node-4.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a4 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-4.0.0a3/setup.py` & `vantage6-node-4.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/__init__.py` & `vantage6-node-4.0.0a4/vantage6/node/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/_version.py` & `vantage6-node-4.0.0a4/vantage6/node/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 
 # Module version
 version_info = (4, 0, 0, 'alpha', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
-pre_release = f'' if version_info[3] == 'final' else \
-  '.'+_specifier_[version_info[3]]+str(version_info[4])
-post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
+pre_release = '' if version_info[3] == 'final' else \
+    _specifier_[version_info[3]]+str(version_info[4])
+post_release = '' if not version_info[5] else f'.post{version_info[5]}'
 
 # Module version accessible using thomas.__version__
 __version__ = f'{version}{pre_release}{post_release}'
```

### Comparing `vantage6-node-4.0.0a3/vantage6/node/cli/node.py` & `vantage6-node-4.0.0a4/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/context.py` & `vantage6-node-4.0.0a4/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/docker/docker_base.py` & `vantage6-node-4.0.0a4/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/docker/docker_manager.py` & `vantage6-node-4.0.0a4/vantage6/node/docker/docker_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/docker/exceptions.py` & `vantage6-node-4.0.0a4/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/docker/squid.py` & `vantage6-node-4.0.0a4/vantage6/node/docker/squid.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-4.0.0a4/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/docker/task_manager.py` & `vantage6-node-4.0.0a4/vantage6/node/docker/task_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/docker/vpn_manager.py` & `vantage6-node-4.0.0a4/vantage6/node/docker/vpn_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/globals.py` & `vantage6-node-4.0.0a4/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/proxy_server.py` & `vantage6-node-4.0.0a4/vantage6/node/proxy_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/socket.py` & `vantage6-node-4.0.0a4/vantage6/node/socket.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6/node/util/colorer.py` & `vantage6-node-4.0.0a4/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.0.0a3/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-4.0.0a4/vantage6_node.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.0.0a4 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-4.0.0a3/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-4.0.0a4/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

