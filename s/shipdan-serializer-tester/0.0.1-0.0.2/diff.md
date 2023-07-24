# Comparing `tmp/shipdan_serializer_tester-0.0.1.tar.gz` & `tmp/shipdan_serializer_tester-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipdan_serializer_tester-0.0.1.tar", last modified: Wed Jul 19 09:49:30 2023, max compression
+gzip compressed data, was "shipdan_serializer_tester-0.0.2.tar", last modified: Mon Jul 24 02:25:41 2023, max compression
```

## Comparing `shipdan_serializer_tester-0.0.1.tar` & `shipdan_serializer_tester-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-19 09:49:30.887548 shipdan_serializer_tester-0.0.1/
--rw-r--r--   0 dare       (501) staff       (20)      475 2023-07-19 09:49:30.887438 shipdan_serializer_tester-0.0.1/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-19 09:49:30.887584 shipdan_serializer_tester-0.0.1/setup.cfg
--rw-r--r--   0 dare       (501) staff       (20)      710 2023-07-19 09:48:05.000000 shipdan_serializer_tester-0.0.1/setup.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-19 09:49:30.886409 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester/
--rw-r--r--   0 dare       (501) staff       (20)       21 2023-07-19 09:48:16.000000 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester/__init__.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-19 09:49:30.887272 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester.egg-info/
--rw-r--r--   0 dare       (501) staff       (20)      475 2023-07-19 09:49:30.000000 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester.egg-info/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)      338 2023-07-19 09:49:30.000000 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester.egg-info/SOURCES.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-19 09:49:30.000000 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester.egg-info/dependency_links.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-19 09:49:30.000000 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester.egg-info/not-zip-safe
--rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-19 09:49:30.000000 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester.egg-info/requires.txt
--rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-19 09:49:30.000000 shipdan_serializer_tester-0.0.1/shipdan_serializer_tester.egg-info/top_level.txt
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:25:41.451193 shipdan_serializer_tester-0.0.2/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:25:41.451075 shipdan_serializer_tester-0.0.2/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.2/README.md
+-rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-24 02:25:41.451234 shipdan_serializer_tester-0.0.2/setup.cfg
+-rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-24 02:25:19.000000 shipdan_serializer_tester-0.0.2/setup.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:25:41.450033 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester/
+-rw-r--r--   0 dare       (501) staff       (20)       78 2023-07-24 02:25:19.000000 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester/__init__.py
+-rw-r--r--   0 dare       (501) staff       (20)     2458 2023-07-24 02:13:32.000000 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester/model_serializer_tester.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:25:41.450900 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester.egg-info/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:25:41.000000 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester.egg-info/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-24 02:25:41.000000 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:25:41.000000 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:25:41.000000 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester.egg-info/not-zip-safe
+-rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-24 02:25:41.000000 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester.egg-info/requires.txt
+-rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-24 02:25:41.000000 shipdan_serializer_tester-0.0.2/shipdan_serializer_tester.egg-info/top_level.txt
```

### Comparing `shipdan_serializer_tester-0.0.1/setup.py` & `shipdan_serializer_tester-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='shipdan_serializer_tester',
-    version='0.0.1',
+    version='0.0.2',
     description='for shipdan_application, shipdan_operation basic ModelSerializer field test',
     author='dare',
     author_email='gdare1999@gmail.com',
-    url='https://github.com/teddylee777/teddynote', # todo
+    url='https://github.com/G-D4R3/shipdan_serializer_tester.git',
     install_requires=['django',],
     packages=find_packages(exclude=[]),
     keywords=['dare', 'darever', 'bunkerkids', 'shipdan', 'pypi'],
     python_requires='>=3.9',
     package_data={},
     zip_safe=False,
     classifiers=[
```

