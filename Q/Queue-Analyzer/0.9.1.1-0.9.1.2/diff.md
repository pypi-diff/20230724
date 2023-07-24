# Comparing `tmp/Queue_Analyzer-0.9.1.1.tar.gz` & `tmp/Queue_Analyzer-0.9.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Queue_Analyzer-0.9.1.1.tar", last modified: Thu Jul 20 13:46:28 2023, max compression
+gzip compressed data, was "Queue_Analyzer-0.9.1.2.tar", last modified: Mon Jul 24 06:38:52 2023, max compression
```

## Comparing `Queue_Analyzer-0.9.1.1.tar` & `Queue_Analyzer-0.9.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:46:28.321335 Queue_Analyzer-0.9.1.1/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35148 2023-07-20 13:32:52.000000 Queue_Analyzer-0.9.1.1/LICENSE.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6749 2023-07-20 13:46:28.321335 Queue_Analyzer-0.9.1.1/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6288 2023-07-20 13:45:52.000000 Queue_Analyzer-0.9.1.1/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-20 13:46:28.321335 Queue_Analyzer-0.9.1.1/setup.cfg
--rwxrwxrwx   0 dipson    (1000) dipson    (1000)     1011 2023-07-20 13:46:02.000000 Queue_Analyzer-0.9.1.1/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:46:28.317335 Queue_Analyzer-0.9.1.1/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:46:28.317335 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    48625 2023-07-19 18:01:22.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-20 13:46:28.321335 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     6749 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      315 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       54 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       98 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       15 2023-07-20 13:46:28.000000 Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-24 06:38:52.238295 Queue_Analyzer-0.9.1.2/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35148 2023-07-20 15:16:16.000000 Queue_Analyzer-0.9.1.2/LICENSE.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6905 2023-07-24 06:38:52.238295 Queue_Analyzer-0.9.1.2/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6417 2023-07-20 15:16:16.000000 Queue_Analyzer-0.9.1.2/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-24 06:38:52.238295 Queue_Analyzer-0.9.1.2/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1043 2023-07-24 06:38:04.000000 Queue_Analyzer-0.9.1.2/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-24 06:38:52.238295 Queue_Analyzer-0.9.1.2/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-24 06:38:52.238295 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    48625 2023-07-20 15:16:16.000000 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-24 06:38:52.238295 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     6905 2023-07-24 06:38:52.000000 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      315 2023-07-24 06:38:52.000000 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-24 06:38:52.000000 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       54 2023-07-24 06:38:52.000000 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       98 2023-07-24 06:38:52.000000 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       15 2023-07-24 06:38:52.000000 Queue_Analyzer-0.9.1.2/src/Queue_Analyzer.egg-info/top_level.txt
```

### Comparing `Queue_Analyzer-0.9.1.1/LICENSE.txt` & `Queue_Analyzer-0.9.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Queue_Analyzer-0.9.1.1/PKG-INFO` & `Queue_Analyzer-0.9.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Queue_Analyzer
-Version: 0.9.1.1
-Summary: python package to retreive youtube comments and translate them
+Version: 0.9.1.2
+Summary: Generate a distribution for arrival objects and analyze the results from the Dosimis software.
 Home-page: https://github.com/dipson94/Queue-Analyzer
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
@@ -92,14 +92,19 @@
 **Running the App**
 
 Enter the following command in Terminal to run program
 
 ```
 queueanalyzer
 ```
+Run and install preview
+
+https://github.com/dipson94/Queue-Analyzer/assets/123653581/d6a0cac6-0086-4ecc-a708-a4f88f766a8b
+
+
 
 **Standalone running (without install)**
 
 1. Download .exe windows executable file.[Download Link](https://drive.google.com/file/d/112hH66TlmQ7xwqi7EwZhJhfROGHBMQms/view?usp=share_link).
 2. Build the .exe file using pyinstaller.run 'pyinstaller -w --onefile Queue_Analyzer.py' in terminal.
    find executable in dist folder.
    Or use auto-py-to-exe for GUI experience.
```

### Comparing `Queue_Analyzer-0.9.1.1/README.md` & `Queue_Analyzer-0.9.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,19 @@
 **Running the App**
 
 Enter the following command in Terminal to run program
 
 ```
 queueanalyzer
 ```
+Run and install preview
+
+https://github.com/dipson94/Queue-Analyzer/assets/123653581/d6a0cac6-0086-4ecc-a708-a4f88f766a8b
+
+
 
 **Standalone running (without install)**
 
 1. Download .exe windows executable file.[Download Link](https://drive.google.com/file/d/112hH66TlmQ7xwqi7EwZhJhfROGHBMQms/view?usp=share_link).
 2. Build the .exe file using pyinstaller.run 'pyinstaller -w --onefile Queue_Analyzer.py' in terminal.
    find executable in dist folder.
    Or use auto-py-to-exe for GUI experience.
```

### Comparing `Queue_Analyzer-0.9.1.1/setup.py` & `Queue_Analyzer-0.9.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup 
 with open("README.md", "r") as f:
 	long_description = f.read()
 setup(
 name="Queue_Analyzer",
-version="0.9.1.1",
-description="python package to retreive youtube comments and translate them",
+version="0.9.1.2",
+description="Generate a distribution for arrival objects and analyze the results from the Dosimis software.",
 package_dir={"": "src"},
 include_package_data=True,
 long_description=long_description,
 long_description_content_type="text/markdown",
 url="https://github.com/dipson94/Queue-Analyzer",
 author="Dipson",
 author_email="dipson94.coding@gmail.com",
```

### Comparing `Queue_Analyzer-0.9.1.1/src/Queue_Analyzer/__init__.py` & `Queue_Analyzer-0.9.1.2/src/Queue_Analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `Queue_Analyzer-0.9.1.1/src/Queue_Analyzer.egg-info/PKG-INFO` & `Queue_Analyzer-0.9.1.2/src/Queue_Analyzer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Queue-Analyzer
-Version: 0.9.1.1
-Summary: python package to retreive youtube comments and translate them
+Version: 0.9.1.2
+Summary: Generate a distribution for arrival objects and analyze the results from the Dosimis software.
 Home-page: https://github.com/dipson94/Queue-Analyzer
 Author: Dipson
 Author-email: dipson94.coding@gmail.com
 License: GNU GPL V3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
@@ -92,14 +92,19 @@
 **Running the App**
 
 Enter the following command in Terminal to run program
 
 ```
 queueanalyzer
 ```
+Run and install preview
+
+https://github.com/dipson94/Queue-Analyzer/assets/123653581/d6a0cac6-0086-4ecc-a708-a4f88f766a8b
+
+
 
 **Standalone running (without install)**
 
 1. Download .exe windows executable file.[Download Link](https://drive.google.com/file/d/112hH66TlmQ7xwqi7EwZhJhfROGHBMQms/view?usp=share_link).
 2. Build the .exe file using pyinstaller.run 'pyinstaller -w --onefile Queue_Analyzer.py' in terminal.
    find executable in dist folder.
    Or use auto-py-to-exe for GUI experience.
```

