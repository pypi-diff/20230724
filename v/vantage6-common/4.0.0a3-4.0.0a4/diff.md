# Comparing `tmp/vantage6-common-4.0.0a3.tar.gz` & `tmp/vantage6-common-4.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-4.0.0a3.tar", last modified: Tue Jul 18 15:34:09 2023, max compression
+gzip compressed data, was "vantage6-common-4.0.0a4.tar", last modified: Mon Jul 24 13:22:26 2023, max compression
```

## Comparing `vantage6-common-4.0.0a3.tar` & `vantage6-common-4.0.0a4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:09.847228 vantage6-common-4.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 15:34:09.847228 vantage6-common-4.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:34:09.847228 vantage6-common-4.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:09.843228 vantage6-common-4.0.0a3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:09.843228 vantage6-common-4.0.0a3/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:09.843228 vantage6-common-4.0.0a3/vantage6/common/client/
--rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/client/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/client/node_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:09.843228 vantage6-common-4.0.0a3/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-18 15:33:57.000000 vantage6-common-4.0.0a3/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:09.847228 vantage6-common-4.0.0a3/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 15:34:09.000000 vantage6-common-4.0.0a3/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-18 15:34:09.000000 vantage6-common-4.0.0a3/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:34:09.000000 vantage6-common-4.0.0a3/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 15:34:09.000000 vantage6-common-4.0.0a3/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 15:34:09.000000 vantage6-common-4.0.0a3/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.280429 vantage6-common-4.0.0a4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.284429 vantage6-common-4.0.0a4/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.284429 vantage6-common-4.0.0a4/vantage6/common/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/client/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/client/node_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-24 13:22:06.000000 vantage6-common-4.0.0a4/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:26.288429 vantage6-common-4.0.0a4/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 13:22:26.000000 vantage6-common-4.0.0a4/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-4.0.0a3/PKG-INFO` & `vantage6-common-4.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a4 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-4.0.0a3/setup.py` & `vantage6-common-4.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/__init__.py` & `vantage6-common-4.0.0a4/vantage6/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/_version.py` & `vantage6-common-4.0.0a4/vantage6/common/_version.py`

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
-__version__ = f'{version}{pre_release}{post_release}'
+__version__ = f'{version}{pre_release}{post_release}'
```

### Comparing `vantage6-common-4.0.0a3/vantage6/common/client/client_base.py` & `vantage6-common-4.0.0a4/vantage6/common/client/client_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/client/node_client.py` & `vantage6-common-4.0.0a4/vantage6/common/client/node_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/client/utils.py` & `vantage6-common-4.0.0a4/vantage6/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/colors.py` & `vantage6-common-4.0.0a4/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/configuration_manager.py` & `vantage6-common-4.0.0a4/vantage6/common/configuration_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         Raises
         ------
         AssertionError
             If the configuration is not valid.
         """
         configuration = self.conf_class(config)
         if configuration.is_valid:
-            self.config = configuration
+            self.config = config
 
     def get(self) -> Configuration:
         """
         Get a configuration from the configuration manager.
 
         Returns
         -------
```

### Comparing `vantage6-common-4.0.0a3/vantage6/common/context.py` & `vantage6-common-4.0.0a4/vantage6/common/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/docker/addons.py` & `vantage6-common-4.0.0a4/vantage6/common/docker/addons.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/docker/network_manager.py` & `vantage6-common-4.0.0a4/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/encryption.py` & `vantage6-common-4.0.0a4/vantage6/common/encryption.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/globals.py` & `vantage6-common-4.0.0a4/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/log.py` & `vantage6-common-4.0.0a4/vantage6/common/log.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/task_status.py` & `vantage6-common-4.0.0a4/vantage6/common/task_status.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6/common/utest.py` & `vantage6-common-4.0.0a4/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.0.0a3/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-4.0.0a4/vantage6_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a4 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-4.0.0a3/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-4.0.0a4/vantage6_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

