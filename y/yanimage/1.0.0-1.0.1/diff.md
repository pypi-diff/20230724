# Comparing `tmp/yanimage-1.0.0.tar.gz` & `tmp/yanimage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yanimage-1.0.0.tar", last modified: Mon Jul 24 14:41:57 2023, max compression
+gzip compressed data, was "dist\yanimage-1.0.1.tar", last modified: Mon Jul 24 15:11:25 2023, max compression
```

## Comparing `yanimage-1.0.0.tar` & `yanimage-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 14:41:57.338184 yanimage-1.0.0/
--rw-rw-rw-   0        0        0     1233 2023-07-24 14:41:57.339183 yanimage-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      694 2023-07-24 14:35:20.000000 yanimage-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 14:41:57.342188 yanimage-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      532 2023-07-24 14:37:00.000000 yanimage-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:41:57.305160 yanimage-1.0.0/yanimage/
--rw-rw-rw-   0        0        0      540 2023-07-24 14:33:15.000000 yanimage-1.0.0/yanimage/Download.py
--rw-rw-rw-   0        0        0     1979 2023-07-24 12:49:33.000000 yanimage-1.0.0/yanimage/Parser.py
--rw-rw-rw-   0        0        0       58 2023-07-24 14:34:24.000000 yanimage-1.0.0/yanimage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:41:57.335993 yanimage-1.0.0/yanimage.egg-info/
--rw-rw-rw-   0        0        0     1233 2023-07-24 14:41:57.000000 yanimage-1.0.0/yanimage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-07-24 14:41:57.000000 yanimage-1.0.0/yanimage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 14:41:57.000000 yanimage-1.0.0/yanimage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 14:41:57.000000 yanimage-1.0.0/yanimage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 15:11:25.201071 yanimage-1.0.1/
+-rw-rw-rw-   0        0        0     1233 2023-07-24 15:11:25.202072 yanimage-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2023-07-24 14:35:20.000000 yanimage-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 15:11:25.212283 yanimage-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      532 2023-07-24 15:11:19.000000 yanimage-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:11:25.170338 yanimage-1.0.1/yanimage/
+-rw-rw-rw-   0        0        0      540 2023-07-24 14:33:15.000000 yanimage-1.0.1/yanimage/Download.py
+-rw-rw-rw-   0        0        0     1979 2023-07-24 12:49:33.000000 yanimage-1.0.1/yanimage/Parser.py
+-rw-rw-rw-   0        0        0       60 2023-07-24 15:08:30.000000 yanimage-1.0.1/yanimage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 15:11:25.198038 yanimage-1.0.1/yanimage.egg-info/
+-rw-rw-rw-   0        0        0     1233 2023-07-24 15:11:25.000000 yanimage-1.0.1/yanimage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-07-24 15:11:25.000000 yanimage-1.0.1/yanimage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 15:11:25.000000 yanimage-1.0.1/yanimage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 15:11:25.000000 yanimage-1.0.1/yanimage.egg-info/top_level.txt
```

### Comparing `yanimage-1.0.0/PKG-INFO` & `yanimage-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanimage
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python module for searching, getting links and downloading images from Yandex images
 Home-page: UNKNOWN
 Author: Elieren
 Author-email: kir102906@gmail.com
 License: UNKNOWN
 Description: # Yanimage
```

### Comparing `yanimage-1.0.0/README.md` & `yanimage-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `yanimage-1.0.0/setup.py` & `yanimage-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 """
 :author: Elieren
 """
 
-version = '1.0.0'
+version = '1.0.1'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='yanimage',
     version=version,
```

### Comparing `yanimage-1.0.0/yanimage/Download.py` & `yanimage-1.0.1/yanimage/Download.py`

 * *Files identical despite different names*

### Comparing `yanimage-1.0.0/yanimage/Parser.py` & `yanimage-1.0.1/yanimage/Parser.py`

 * *Files identical despite different names*

### Comparing `yanimage-1.0.0/yanimage.egg-info/PKG-INFO` & `yanimage-1.0.1/yanimage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanimage
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python module for searching, getting links and downloading images from Yandex images
 Home-page: UNKNOWN
 Author: Elieren
 Author-email: kir102906@gmail.com
 License: UNKNOWN
 Description: # Yanimage
```

