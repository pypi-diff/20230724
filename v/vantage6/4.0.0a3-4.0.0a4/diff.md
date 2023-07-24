# Comparing `tmp/vantage6-4.0.0a3.tar.gz` & `tmp/vantage6-4.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-4.0.0a3.tar", last modified: Tue Jul 18 15:34:10 2023, max compression
+gzip compressed data, was "vantage6-4.0.0a4.tar", last modified: Mon Jul 24 13:22:27 2023, max compression
```

## Comparing `vantage6-4.0.0a3.tar` & `vantage6-4.0.0a4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.883252 vantage6-4.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-18 15:34:10.883252 vantage6-4.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:34:10.883252 vantage6-4.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.879252 vantage6-4.0.0a3/tests_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/tests_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/tests_cli/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/tests_cli/test_node_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/tests_cli/test_server_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/tests_cli/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.879252 vantage6-4.0.0a3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.883252 vantage6-4.0.0a3/vantage6/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/__build__
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    33998 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.883252 vantage6-4.0.0a3/vantage6/cli/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/rabbitmq/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/rabbitmq/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/rabbitmq/rabbitmq.config
--rw-r--r--   0 runner    (1001) docker     (123)    28331 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-18 15:33:57.000000 vantage6-4.0.0a3/vantage6/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.883252 vantage6-4.0.0a3/vantage6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-18 15:34:10.000000 vantage6-4.0.0a3/vantage6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-18 15:34:10.000000 vantage6-4.0.0a3/vantage6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:34:10.000000 vantage6-4.0.0a3/vantage6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 15:34:10.000000 vantage6-4.0.0a3/vantage6.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-18 15:34:10.000000 vantage6-4.0.0a3/vantage6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 15:34:10.000000 vantage6-4.0.0a3/vantage6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.608513 vantage6-4.0.0a4/tests_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/test_node_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/test_server_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/tests_cli/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.608513 vantage6-4.0.0a4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/vantage6/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/configuration_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33998 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.612513 vantage6-4.0.0a4/vantage6/cli/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/rabbitmq/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/rabbitmq/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/rabbitmq/rabbitmq.config
+-rw-r--r--   0 runner    (1001) docker     (123)    28331 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-24 13:22:06.000000 vantage6-4.0.0a4/vantage6/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.608513 vantage6-4.0.0a4/vantage6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 13:22:27.000000 vantage6-4.0.0a4/vantage6.egg-info/top_level.txt
```

### Comparing `vantage6-4.0.0a3/PKG-INFO` & `vantage6-4.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a3 Summary: vantage6 command
+Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a4 Summary: vantage6 command
 line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
 >=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-4.0.0a3/setup.py` & `vantage6-4.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/tests_cli/test_node_cli.py` & `vantage6-4.0.0a4/tests_cli/test_node_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/tests_cli/test_server_cli.py` & `vantage6-4.0.0a4/tests_cli/test_server_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/tests_cli/test_wizard.py` & `vantage6-4.0.0a4/tests_cli/test_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/_version.py` & `vantage6-4.0.0a4/vantage6/cli/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 # Module version
 version_info = (4, 0, 0, 'alpha', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = '' if version_info[3] == 'final' else \
-  '.'+_specifier_[version_info[3]]+str(version_info[4])
+    _specifier_[version_info[3]]+str(version_info[4])
 post_release = '' if not version_info[5] else f'.post{version_info[5]}'
 
 # Module version accessible using thomas.__version__
 __version__ = f'{version}{pre_release}{post_release}'
```

### Comparing `vantage6-4.0.0a3/vantage6/cli/configuration_manager.py` & `vantage6-4.0.0a4/vantage6/cli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/configuration_wizard.py` & `vantage6-4.0.0a4/vantage6/cli/configuration_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/context.py` & `vantage6-4.0.0a4/vantage6/cli/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/globals.py` & `vantage6-4.0.0a4/vantage6/cli/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/node.py` & `vantage6-4.0.0a4/vantage6/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/rabbitmq/__init__.py` & `vantage6-4.0.0a4/vantage6/cli/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/rabbitmq/definitions.py` & `vantage6-4.0.0a4/vantage6/cli/rabbitmq/definitions.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/rabbitmq/queue_manager.py` & `vantage6-4.0.0a4/vantage6/cli/rabbitmq/queue_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/server.py` & `vantage6-4.0.0a4/vantage6/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6/cli/utils.py` & `vantage6-4.0.0a4/vantage6/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.0.0a3/vantage6.egg-info/PKG-INFO` & `vantage6-4.0.0a4/vantage6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a3 Summary: vantage6 command
+Metadata-Version: 2.1 Name: vantage6 Version: 4.0.0a4 Summary: vantage6 command
 line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
 >=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-4.0.0a3/vantage6.egg-info/SOURCES.txt` & `vantage6-4.0.0a4/vantage6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

