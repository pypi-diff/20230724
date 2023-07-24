# Comparing `tmp/wtisdk-1.5.2.tar.gz` & `tmp/wtisdk-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtisdk-1.5.2.tar", last modified: Sat May 27 00:18:22 2023, max compression
+gzip compressed data, was "wtisdk-1.5.3.tar", last modified: Mon Jul 24 14:16:20 2023, max compression
```

## Comparing `wtisdk-1.5.2.tar` & `wtisdk-1.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:22.140042 wtisdk-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-27 00:18:04.000000 wtisdk-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-05-27 00:18:22.140042 wtisdk-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18877 2023-05-27 00:18:04.000000 wtisdk-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 00:18:22.140042 wtisdk-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-27 00:18:04.000000 wtisdk-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:22.140042 wtisdk-1.5.2/wtisdk/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 00:18:04.000000 wtisdk-1.5.2/wtisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:22.140042 wtisdk-1.5.2/wtisdk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:04.000000 wtisdk-1.5.2/wtisdk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-27 00:18:04.000000 wtisdk-1.5.2/wtisdk/tests/test_wtisdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-27 00:18:04.000000 wtisdk-1.5.2/wtisdk/wtisdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:22.140042 wtisdk-1.5.2/wtisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:20.805915 wtisdk-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 14:16:04.000000 wtisdk-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-07-24 14:16:20.805915 wtisdk-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-07-24 14:16:04.000000 wtisdk-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:16:20.805915 wtisdk-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-24 14:16:04.000000 wtisdk-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:20.805915 wtisdk-1.5.3/wtisdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 14:16:04.000000 wtisdk-1.5.3/wtisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:20.805915 wtisdk-1.5.3/wtisdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:04.000000 wtisdk-1.5.3/wtisdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-24 14:16:04.000000 wtisdk-1.5.3/wtisdk/tests/test_wtisdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-07-24 14:16:04.000000 wtisdk-1.5.3/wtisdk/wtisdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:16:20.805915 wtisdk-1.5.3/wtisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19838 2023-07-24 14:16:20.000000 wtisdk-1.5.3/wtisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-24 14:16:20.000000 wtisdk-1.5.3/wtisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:16:20.000000 wtisdk-1.5.3/wtisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 14:16:20.000000 wtisdk-1.5.3/wtisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 14:16:20.000000 wtisdk-1.5.3/wtisdk.egg-info/top_level.txt
```

### Comparing `wtisdk-1.5.2/LICENSE` & `wtisdk-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.2/PKG-INFO` & `wtisdk-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 ```sh
 pip install wtisdk
 ```
 
 
 ### Basic Usage
 ```sh
-(.venv) [mteke1@n6lans00001 test_infra]$ ipython
+(.venv) [mteke@devnet-server test_infra]$ ipython
 Python 3.10.8 (default, Aug 13 2020, 07:46:32) 
 Type 'copyright', 'credits' or 'license' for more information
 IPython 7.16.3 -- An enhanced Interactive Python. Type '?' for help.
 
 In [1]: device = { "host": "10.20.30.139",
    ...:            "username": "USERNAME",
    ...:            "password": "PASSWORD"
@@ -73,15 +73,15 @@
 Out[4]: 
 {'status': {'code': '0', 'text': 'OK'},
  'vendor': 'WTI',
  'product': 'CPM-800-2-EA',
  'totalports': '8',
  'totalplugs': '8',
  'softwareversion': '7.04 4 Sep 2022',
- 'serialnumber': '01910453453191131',
+ 'serialnumber': '01910453453191231',
  'assettag': '153561',
  'siteid': 'DEV6S01',
  'analogmodemphonenumber': '',
  'modeminstalled': 'No',
  'gig_dualphy': 'Yes, Yes',
  'cpu_boardprogramdate': 'ARM, 10-31-2019',
  'ram_flash': '512 MB, 128 MB',
```

### Comparing `wtisdk-1.5.2/README.md` & `wtisdk-1.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ```sh
 pip install wtisdk
 ```
 
 
 ### Basic Usage
 ```sh
-(.venv) [mteke1@n6lans00001 test_infra]$ ipython
+(.venv) [mteke@devnet-server test_infra]$ ipython
 Python 3.10.8 (default, Aug 13 2020, 07:46:32) 
 Type 'copyright', 'credits' or 'license' for more information
 IPython 7.16.3 -- An enhanced Interactive Python. Type '?' for help.
 
 In [1]: device = { "host": "10.20.30.139",
    ...:            "username": "USERNAME",
    ...:            "password": "PASSWORD"
@@ -51,15 +51,15 @@
 Out[4]: 
 {'status': {'code': '0', 'text': 'OK'},
  'vendor': 'WTI',
  'product': 'CPM-800-2-EA',
  'totalports': '8',
  'totalplugs': '8',
  'softwareversion': '7.04 4 Sep 2022',
- 'serialnumber': '01910453453191131',
+ 'serialnumber': '01910453453191231',
  'assettag': '153561',
  'siteid': 'DEV6S01',
  'analogmodemphonenumber': '',
  'modeminstalled': 'No',
  'gig_dualphy': 'Yes, Yes',
  'cpu_boardprogramdate': 'ARM, 10-31-2019',
  'ram_flash': '512 MB, 128 MB',
```

### Comparing `wtisdk-1.5.2/setup.py` & `wtisdk-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='wtisdk',
-    version='1.5.2',
+    version='1.5.3',
     author='Melih Teke',
     author_email='me@mteke.com',
     description='WTI SDK for interacting with WTI devices',
     long_description=f"{long_description}\n\nFor more information, visit the [PyPI page](https://pypi.org/project/wtisdk/).\n\nYou can also connect with me on [LinkedIn](https://www.linkedin.com/in/melih-teke/).",
     long_description_content_type='text/markdown',
     url='https://github.com/melihteke/wtisdk',
     packages=find_packages(),
```

### Comparing `wtisdk-1.5.2/wtisdk/tests/test_wtisdk.py` & `wtisdk-1.5.3/wtisdk/tests/test_wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.2/wtisdk/wtisdk.py` & `wtisdk-1.5.3/wtisdk/wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.2/wtisdk.egg-info/PKG-INFO` & `wtisdk-1.5.3/wtisdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,15 +51,15 @@
 ```sh
 pip install wtisdk
 ```
 
 
 ### Basic Usage
 ```sh
-(.venv) [mteke1@n6lans00001 test_infra]$ ipython
+(.venv) [mteke@devnet-server test_infra]$ ipython
 Python 3.10.8 (default, Aug 13 2020, 07:46:32) 
 Type 'copyright', 'credits' or 'license' for more information
 IPython 7.16.3 -- An enhanced Interactive Python. Type '?' for help.
 
 In [1]: device = { "host": "10.20.30.139",
    ...:            "username": "USERNAME",
    ...:            "password": "PASSWORD"
@@ -73,15 +73,15 @@
 Out[4]: 
 {'status': {'code': '0', 'text': 'OK'},
  'vendor': 'WTI',
  'product': 'CPM-800-2-EA',
  'totalports': '8',
  'totalplugs': '8',
  'softwareversion': '7.04 4 Sep 2022',
- 'serialnumber': '01910453453191131',
+ 'serialnumber': '01910453453191231',
  'assettag': '153561',
  'siteid': 'DEV6S01',
  'analogmodemphonenumber': '',
  'modeminstalled': 'No',
  'gig_dualphy': 'Yes, Yes',
  'cpu_boardprogramdate': 'ARM, 10-31-2019',
  'ram_flash': '512 MB, 128 MB',
```

