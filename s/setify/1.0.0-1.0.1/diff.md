# Comparing `tmp/setify-1.0.0.tar.gz` & `tmp/setify-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setify-1.0.0.tar", last modified: Wed Jun 28 13:00:31 2023, max compression
+gzip compressed data, was "setify-1.0.1.tar", last modified: Mon Jul 24 15:47:46 2023, max compression
```

## Comparing `setify-1.0.0.tar` & `setify-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 minagabriel   (501) staff       (20)        0 2023-06-28 13:00:31.867102 setify-1.0.0/
--rw-r--r--   0 minagabriel   (501) staff       (20)      933 2023-06-28 13:00:31.867382 setify-1.0.0/PKG-INFO
-drwxr-xr-x   0 minagabriel   (501) staff       (20)        0 2023-06-28 13:00:31.866980 setify-1.0.0/setify/
--rw-r--r--   0 minagabriel   (501) staff       (20)       66 2023-06-28 13:00:03.948629 setify-1.0.0/setify/__init__.py
--rw-r--r--   0 minagabriel   (501) staff       (20)     2035 2023-06-28 12:38:24.914074 setify-1.0.0/setify/datasets.py
--rw-r--r--   0 minagabriel   (501) staff       (20)     3334 2023-06-28 11:39:50.448823 setify-1.0.0/setify/utils.py
--rw-r--r--   0 minagabriel   (501) staff       (20)       61 2023-06-28 11:39:50.448963 setify-1.0.0/setup.cfg
--rw-r--r--   0 minagabriel   (501) staff       (20)     1244 2023-06-28 12:59:23.761554 setify-1.0.0/setup.py
+drwxr-xr-x   0 minagabriel   (501) staff       (20)        0 2023-07-24 15:47:46.004272 setify-1.0.1/
+-rw-r--r--   0 minagabriel   (501) staff       (20)      933 2023-07-24 15:47:46.004434 setify-1.0.1/PKG-INFO
+drwxr-xr-x   0 minagabriel   (501) staff       (20)        0 2023-07-24 15:47:46.004178 setify-1.0.1/setify/
+-rw-r--r--   0 minagabriel   (501) staff       (20)       66 2023-07-24 15:44:49.810994 setify-1.0.1/setify/__init__.py
+-rw-r--r--   0 minagabriel   (501) staff       (20)      295 2023-07-24 15:39:42.023375 setify-1.0.1/setify/datasets.py
+-rw-r--r--   0 minagabriel   (501) staff       (20)     3334 2023-06-28 11:39:50.448823 setify-1.0.1/setify/utils.py
+-rw-r--r--   0 minagabriel   (501) staff       (20)       61 2023-06-28 11:39:50.448963 setify-1.0.1/setup.cfg
+-rw-r--r--   0 minagabriel   (501) staff       (20)     1244 2023-07-24 15:47:22.424224 setify-1.0.1/setup.py
```

### Comparing `setify-1.0.0/PKG-INFO` & `setify-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: setify
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dataset packages
 Home-page: https://github.com/MinaGabriel/setify.git
 Author: Mina Gabriel
 Author-email: developer.mina@gmail.com
 License: MIT
-Download-URL: https://github.com/MinaGabriel/setify/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/MinaGabriel/setify/archive/refs/tags/v1.0.1.tar.gz
 Description: Setify is an open-source dataset package manager written in Python and designed to enable fast experimentation for Machine Learning, Setify allows you to reach hundreds of datasets with one command.
 Keywords: Dataset,Data
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `setify-1.0.0/setify/utils.py` & `setify-1.0.1/setify/utils.py`

 * *Files identical despite different names*

### Comparing `setify-1.0.0/setup.py` & `setify-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name='setify',
     packages=['setify'],
-    version='1.0.0',
+    version='1.0.1',
     license='MIT',
     description='Dataset packages',
     author='Mina Gabriel',
     author_email='developer.mina@gmail.com',
     url='https://github.com/MinaGabriel/setify.git',
-    download_url='https://github.com/MinaGabriel/setify/archive/refs/tags/v1.0.0.tar.gz',
+    download_url='https://github.com/MinaGabriel/setify/archive/refs/tags/v1.0.1.tar.gz',
     keywords=['Dataset', 'Data'],
     install_requires=[
         'pandas',
         'numpy',
         'tqdm',
         'colorama',
         'tables'
```

