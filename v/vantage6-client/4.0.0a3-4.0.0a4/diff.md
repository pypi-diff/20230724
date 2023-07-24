# Comparing `tmp/vantage6-client-4.0.0a3.tar.gz` & `tmp/vantage6-client-4.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-client-4.0.0a3.tar", last modified: Tue Jul 18 15:34:10 2023, max compression
+gzip compressed data, was "vantage6-client-4.0.0a4.tar", last modified: Mon Jul 24 13:22:27 2023, max compression
```

## Comparing `vantage6-client-4.0.0a3.tar` & `vantage6-client-4.0.0a4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.435242 vantage6-client-4.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 15:34:10.435242 vantage6-client-4.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:34:10.435242 vantage6-client-4.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.435242 vantage6-client-4.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.431242 vantage6-client-4.0.0a3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.435242 vantage6-client-4.0.0a3/vantage6/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/client/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    58214 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/client/algorithm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.435242 vantage6-client-4.0.0a3/vantage6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/tools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/tools/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/tools/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-18 15:33:57.000000 vantage6-client-4.0.0a3/vantage6/tools/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:10.435242 vantage6-client-4.0.0a3/vantage6_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 15:34:10.000000 vantage6-client-4.0.0a3/vantage6_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-18 15:34:10.000000 vantage6-client-4.0.0a3/vantage6_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:34:10.000000 vantage6-client-4.0.0a3/vantage6_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 15:34:10.000000 vantage6-client-4.0.0a3/vantage6_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 15:34:10.000000 vantage6-client-4.0.0a3/vantage6_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.056478 vantage6-client-4.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.056478 vantage6-client-4.0.0a4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.056478 vantage6-client-4.0.0a4/vantage6/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    58214 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/algorithm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/vantage6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-24 13:22:06.000000 vantage6-client-4.0.0a4/vantage6/tools/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:27.060478 vantage6-client-4.0.0a4/vantage6_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 13:22:27.000000 vantage6-client-4.0.0a4/vantage6_client.egg-info/top_level.txt
```

### Comparing `vantage6-client-4.0.0a3/PKG-INFO` & `vantage6-client-4.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a4 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-4.0.0a3/setup.py` & `vantage6-client-4.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/tests/test_client.py` & `vantage6-client-4.0.0a4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/tests/test_docker_wrapper.py` & `vantage6-client-4.0.0a4/tests/test_docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/tests/test_serialization.py` & `vantage6-client-4.0.0a4/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6/client/__init__.py` & `vantage6-client-4.0.0a4/vantage6/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6/client/_version.py` & `vantage6-client-4.0.0a4/vantage6/client/_version.py`

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

### Comparing `vantage6-client-4.0.0a3/vantage6/client/algorithm_client.py` & `vantage6-client-4.0.0a4/vantage6/client/algorithm_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6/client/filter.py` & `vantage6-client-4.0.0a4/vantage6/client/filter.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6/tools/decorators.py` & `vantage6-client-4.0.0a4/vantage6/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6/tools/mock_client.py` & `vantage6-client-4.0.0a4/vantage6/tools/mock_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6/tools/util.py` & `vantage6-client-4.0.0a4/vantage6/tools/util.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6/tools/wrap.py` & `vantage6-client-4.0.0a4/vantage6/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6/tools/wrappers.py` & `vantage6-client-4.0.0a4/vantage6/tools/wrappers.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.0.0a3/vantage6_client.egg-info/PKG-INFO` & `vantage6-client-4.0.0a4/vantage6_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a4 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-4.0.0a3/vantage6_client.egg-info/SOURCES.txt` & `vantage6-client-4.0.0a4/vantage6_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

