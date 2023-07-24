# Comparing `tmp/isyveri-0.1.3.tar.gz` & `tmp/isyveri-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isyveri-0.1.3.tar", last modified: Mon Jul 24 17:34:56 2023, max compression
+gzip compressed data, was "isyveri-0.1.4.tar", last modified: Mon Jul 24 17:41:43 2023, max compression
```

## Comparing `isyveri-0.1.3.tar` & `isyveri-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 17:34:56.350675 isyveri-0.1.3/
--rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyveri-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4618 2023-07-24 17:34:56.343695 isyveri-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4086 2023-07-24 16:27:44.000000 isyveri-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 17:34:56.286845 isyveri-0.1.3/isyveri/
--rw-rw-rw-   0        0        0     3058 2023-07-24 13:39:38.000000 isyveri-0.1.3/isyveri/VeriCek.py
--rw-rw-rw-   0        0        0       29 2023-07-24 11:50:14.000000 isyveri-0.1.3/isyveri/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:34:56.338706 isyveri-0.1.3/isyveri.egg-info/
--rw-rw-rw-   0        0        0     4618 2023-07-24 17:34:55.000000 isyveri-0.1.3/isyveri.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-24 17:34:56.000000 isyveri-0.1.3/isyveri.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 17:34:55.000000 isyveri-0.1.3/isyveri.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-24 17:34:55.000000 isyveri-0.1.3/isyveri.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 17:34:55.000000 isyveri-0.1.3/isyveri.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 17:34:56.351672 isyveri-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-07-24 17:34:42.000000 isyveri-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:41:43.128067 isyveri-0.1.4/
+-rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyveri-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4618 2023-07-24 17:41:43.126070 isyveri-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4086 2023-07-24 16:27:44.000000 isyveri-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 17:41:43.031324 isyveri-0.1.4/isyveri/
+-rw-rw-rw-   0        0        0     3058 2023-07-24 13:39:38.000000 isyveri-0.1.4/isyveri/VeriCek.py
+-rw-rw-rw-   0        0        0       29 2023-07-24 11:50:14.000000 isyveri-0.1.4/isyveri/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 17:41:43.124081 isyveri-0.1.4/isyveri.egg-info/
+-rw-rw-rw-   0        0        0     4618 2023-07-24 17:41:42.000000 isyveri-0.1.4/isyveri.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-24 17:41:42.000000 isyveri-0.1.4/isyveri.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 17:41:42.000000 isyveri-0.1.4/isyveri.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-24 17:41:42.000000 isyveri-0.1.4/isyveri.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-24 17:41:42.000000 isyveri-0.1.4/isyveri.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 17:41:43.131069 isyveri-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-07-24 17:40:56.000000 isyveri-0.1.4/setup.py
```

### Comparing `isyveri-0.1.3/LICENSE.txt` & `isyveri-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isyveri-0.1.3/PKG-INFO` & `isyveri-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isyveri
-Version: 0.1.3
+Version: 0.1.4
 Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
 Home-page: https://github.com/urazakgul/isyveri
 Author: Uraz Akgül
 Author-email: urazdev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `isyveri-0.1.3/README.md` & `isyveri-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `isyveri-0.1.3/isyveri/VeriCek.py` & `isyveri-0.1.4/isyveri/VeriCek.py`

 * *Files identical despite different names*

### Comparing `isyveri-0.1.3/isyveri.egg-info/PKG-INFO` & `isyveri-0.1.4/isyveri.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isyveri
-Version: 0.1.3
+Version: 0.1.4
 Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
 Home-page: https://github.com/urazakgul/isyveri
 Author: Uraz Akgül
 Author-email: urazdev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `isyveri-0.1.3/setup.py` & `isyveri-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="isyveri",
-    version="0.1.3",
+    version="0.1.4",
     packages=["isyveri"],
     author="Uraz Akgül",
     author_email="urazdev@gmail.com",
     description="İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/urazakgul/isyveri",
```

