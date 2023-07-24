# Comparing `tmp/awyes-10.0.3.tar.gz` & `tmp/awyes-10.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.0.3.tar", last modified: Mon Jul 24 04:55:41 2023, max compression
+gzip compressed data, was "awyes-10.0.4.tar", last modified: Mon Jul 24 05:04:31 2023, max compression
```

## Comparing `awyes-10.0.3.tar` & `awyes-10.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:55:41.274737 awyes-10.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 04:55:41.274737 awyes-10.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 04:55:17.000000 awyes-10.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 04:55:40.000000 awyes-10.0.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:55:41.270738 awyes-10.0.3/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 04:55:41.000000 awyes-10.0.3/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 04:55:41.000000 awyes-10.0.3/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 04:55:41.000000 awyes-10.0.3/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 04:55:41.000000 awyes-10.0.3/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 04:55:41.000000 awyes-10.0.3/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 04:55:41.000000 awyes-10.0.3/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 04:55:41.274737 awyes-10.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-24 04:55:17.000000 awyes-10.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:31.794036 awyes-10.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 05:04:31.794036 awyes-10.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 05:04:11.000000 awyes-10.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 05:04:30.000000 awyes-10.0.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:04:31.794036 awyes-10.0.4/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 05:04:31.000000 awyes-10.0.4/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 05:04:31.000000 awyes-10.0.4/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:04:31.000000 awyes-10.0.4/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 05:04:31.000000 awyes-10.0.4/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 05:04:31.000000 awyes-10.0.4/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:04:31.000000 awyes-10.0.4/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 05:04:31.794036 awyes-10.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-24 05:04:11.000000 awyes-10.0.4/setup.py
```

### Comparing `awyes-10.0.3/PKG-INFO` & `awyes-10.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.0.3
+Version: 10.0.4
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.0.3/awyes.egg-info/PKG-INFO` & `awyes-10.0.4/awyes.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.0.3
+Version: 10.0.4
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.0.3/setup.py` & `awyes-10.0.4/setup.py`

 * *Files identical despite different names*

