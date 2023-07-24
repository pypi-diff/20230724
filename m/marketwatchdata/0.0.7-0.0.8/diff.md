# Comparing `tmp/marketwatchdata-0.0.7.tar.gz` & `tmp/marketwatchdata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketwatchdata-0.0.7.tar", last modified: Sat Jul 22 15:42:57 2023, max compression
+gzip compressed data, was "marketwatchdata-0.0.8.tar", last modified: Sat Jul 22 15:49:38 2023, max compression
```

## Comparing `marketwatchdata-0.0.7.tar` & `marketwatchdata-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:42:57.105152 marketwatchdata-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 15:42:57.105152 marketwatchdata-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:42:57.105152 marketwatchdata-0.0.7/marketwatchdata/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/marketwatchdata/MarketWatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/marketwatchdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:42:57.105152 marketwatchdata-0.0.7/marketwatchdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 15:42:57.000000 marketwatchdata-0.0.7/marketwatchdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 15:42:57.000000 marketwatchdata-0.0.7/marketwatchdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:42:57.000000 marketwatchdata-0.0.7/marketwatchdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 15:42:57.000000 marketwatchdata-0.0.7/marketwatchdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 15:42:57.000000 marketwatchdata-0.0.7/marketwatchdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:42:57.105152 marketwatchdata-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:42:57.105152 marketwatchdata-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-22 15:42:31.000000 marketwatchdata-0.0.7/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:49:38.709446 marketwatchdata-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 15:49:38.709446 marketwatchdata-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:49:38.709446 marketwatchdata-0.0.8/marketwatchdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/marketwatchdata/MarketWatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/marketwatchdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:49:38.709446 marketwatchdata-0.0.8/marketwatchdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 15:49:38.000000 marketwatchdata-0.0.8/marketwatchdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 15:49:38.000000 marketwatchdata-0.0.8/marketwatchdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:49:38.000000 marketwatchdata-0.0.8/marketwatchdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 15:49:38.000000 marketwatchdata-0.0.8/marketwatchdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 15:49:38.000000 marketwatchdata-0.0.8/marketwatchdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:49:38.709446 marketwatchdata-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:49:38.709446 marketwatchdata-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-22 15:49:10.000000 marketwatchdata-0.0.8/tests/test_func.py
```

### Comparing `marketwatchdata-0.0.7/LICENSE` & `marketwatchdata-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `marketwatchdata-0.0.7/PKG-INFO` & `marketwatchdata-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketwatchdata
-Version: 0.0.7
+Version: 0.0.8
 Summary: retrieve data from MarketWatch.com
 Home-page: https://github.com/yacper/marketwatchdata
 Author: yacper
 Author-email: yacper@gmail.com
 License: MIT
 Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `marketwatchdata-0.0.7/marketwatchdata/MarketWatch.py` & `marketwatchdata-0.0.8/marketwatchdata/MarketWatch.py`

 * *Files identical despite different names*

### Comparing `marketwatchdata-0.0.7/marketwatchdata.egg-info/PKG-INFO` & `marketwatchdata-0.0.8/marketwatchdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketwatchdata
-Version: 0.0.7
+Version: 0.0.8
 Summary: retrieve data from MarketWatch.com
 Home-page: https://github.com/yacper/marketwatchdata
 Author: yacper
 Author-email: yacper@gmail.com
 License: MIT
 Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `marketwatchdata-0.0.7/setup.py` & `marketwatchdata-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `marketwatchdata-0.0.7/tests/test_func.py` & `marketwatchdata-0.0.8/tests/test_func.py`

 * *Files identical despite different names*

