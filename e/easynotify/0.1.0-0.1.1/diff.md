# Comparing `tmp/easynotify-0.1.0.tar.gz` & `tmp/easynotify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easynotify-0.1.0.tar", last modified: Mon Jul 24 02:10:49 2023, max compression
+gzip compressed data, was "easynotify-0.1.1.tar", last modified: Mon Jul 24 02:11:56 2023, max compression
```

## Comparing `easynotify-0.1.0.tar` & `easynotify-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 02:10:49.505391 easynotify-0.1.0/
--rw-rw-rw-   0        0        0     1097 2021-09-26 07:25:25.000000 easynotify-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1023 2023-07-24 02:10:49.504452 easynotify-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-07-24 02:09:01.000000 easynotify-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 02:10:49.478357 easynotify-0.1.0/easynotify/
--rw-rw-rw-   0        0        0      105 2023-07-24 01:59:38.000000 easynotify-0.1.0/easynotify/__init__.py
--rw-rw-rw-   0        0        0     1350 2023-07-24 02:07:05.000000 easynotify-0.1.0/easynotify/easynotify.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:10:49.503357 easynotify-0.1.0/easynotify.egg-info/
--rw-rw-rw-   0        0        0     1023 2023-07-24 02:10:49.000000 easynotify-0.1.0/easynotify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-24 02:10:49.000000 easynotify-0.1.0/easynotify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 02:10:49.000000 easynotify-0.1.0/easynotify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 02:10:49.000000 easynotify-0.1.0/easynotify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 02:10:49.000000 easynotify-0.1.0/easynotify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 02:10:49.505391 easynotify-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      570 2023-07-24 02:10:46.000000 easynotify-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:11:56.294006 easynotify-0.1.1/
+-rw-rw-rw-   0        0        0     1097 2021-09-26 07:25:25.000000 easynotify-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1025 2023-07-24 02:11:56.293020 easynotify-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2023-07-24 02:09:01.000000 easynotify-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 02:11:56.276078 easynotify-0.1.1/easynotify/
+-rw-rw-rw-   0        0        0      105 2023-07-24 02:11:51.000000 easynotify-0.1.1/easynotify/__init__.py
+-rw-rw-rw-   0        0        0     1350 2023-07-24 02:07:05.000000 easynotify-0.1.1/easynotify/easynotify.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:11:56.291017 easynotify-0.1.1/easynotify.egg-info/
+-rw-rw-rw-   0        0        0     1025 2023-07-24 02:11:55.000000 easynotify-0.1.1/easynotify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-24 02:11:56.000000 easynotify-0.1.1/easynotify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 02:11:55.000000 easynotify-0.1.1/easynotify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 02:11:55.000000 easynotify-0.1.1/easynotify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 02:11:55.000000 easynotify-0.1.1/easynotify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 02:11:56.294006 easynotify-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-07-24 02:11:51.000000 easynotify-0.1.1/setup.py
```

### Comparing `easynotify-0.1.0/LICENSE` & `easynotify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easynotify-0.1.0/PKG-INFO` & `easynotify-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: easynotify
-Version: 0.1.0
-Home-page: https://github.com/CauchyComplete/EasyPyXL
+Version: 0.1.1
+Home-page: https://github.com/CauchyComplete/EasyNotify
 Author: CauchyComplete
 Author-email: corundum240@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EasyNotify
```

### Comparing `easynotify-0.1.0/README.md` & `easynotify-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `easynotify-0.1.0/easynotify/easynotify.py` & `easynotify-0.1.1/easynotify/easynotify.py`

 * *Files identical despite different names*

### Comparing `easynotify-0.1.0/easynotify.egg-info/PKG-INFO` & `easynotify-0.1.1/easynotify.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: easynotify
-Version: 0.1.0
-Home-page: https://github.com/CauchyComplete/EasyPyXL
+Version: 0.1.1
+Home-page: https://github.com/CauchyComplete/EasyNotify
 Author: CauchyComplete
 Author-email: corundum240@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EasyNotify
```

### Comparing `easynotify-0.1.0/setup.py` & `easynotify-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='easynotify',
-    version='0.1.0',
+    version='0.1.1',
     descripton='This package allows you to post messages with bots easily.',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/CauchyComplete/EasyPyXL',
+    url='https://github.com/CauchyComplete/EasyNotify',
     author='CauchyComplete',
     author_email='corundum240@gmail.com',
     license='MIT',
     packages=['easynotify'],
     install_requires=[
         'requests>=2.0'
     ],
```

