# Comparing `tmp/shipdan_serializer_tester-0.0.3.tar.gz` & `tmp/shipdan_serializer_tester-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipdan_serializer_tester-0.0.3.tar", last modified: Mon Jul 24 02:32:08 2023, max compression
+gzip compressed data, was "shipdan_serializer_tester-0.0.4.tar", last modified: Mon Jul 24 02:36:02 2023, max compression
```

## Comparing `shipdan_serializer_tester-0.0.3.tar` & `shipdan_serializer_tester-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:32:08.717056 shipdan_serializer_tester-0.0.3/
--rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:32:08.716916 shipdan_serializer_tester-0.0.3/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.3/README.md
--rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-24 02:32:08.717096 shipdan_serializer_tester-0.0.3/setup.cfg
--rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-24 02:32:05.000000 shipdan_serializer_tester-0.0.3/setup.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:32:08.715370 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester/
--rw-r--r--   0 dare       (501) staff       (20)       60 2023-07-24 02:32:05.000000 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester/__init__.py
--rw-r--r--   0 dare       (501) staff       (20)     2458 2023-07-24 02:13:32.000000 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester/model_serializer_tester.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:32:08.716698 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester.egg-info/
--rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:32:08.000000 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester.egg-info/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-24 02:32:08.000000 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester.egg-info/SOURCES.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:32:08.000000 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester.egg-info/dependency_links.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:30:24.000000 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester.egg-info/not-zip-safe
--rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-24 02:32:08.000000 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester.egg-info/requires.txt
--rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-24 02:32:08.000000 shipdan_serializer_tester-0.0.3/shipdan_serializer_tester.egg-info/top_level.txt
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:36:02.066751 shipdan_serializer_tester-0.0.4/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:36:02.066644 shipdan_serializer_tester-0.0.4/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.4/README.md
+-rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-24 02:36:02.066790 shipdan_serializer_tester-0.0.4/setup.cfg
+-rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-24 02:35:52.000000 shipdan_serializer_tester-0.0.4/setup.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:36:02.065688 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester/
+-rw-r--r--   0 dare       (501) staff       (20)       60 2023-07-24 02:35:52.000000 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester/__init__.py
+-rw-r--r--   0 dare       (501) staff       (20)     2465 2023-07-24 02:35:30.000000 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester/model_serializer_tester.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:36:02.066496 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester.egg-info/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:36:02.000000 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester.egg-info/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-24 02:36:02.000000 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:36:02.000000 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:30:24.000000 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester.egg-info/not-zip-safe
+-rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-24 02:36:02.000000 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester.egg-info/requires.txt
+-rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-24 02:36:02.000000 shipdan_serializer_tester-0.0.4/shipdan_serializer_tester.egg-info/top_level.txt
```

### Comparing `shipdan_serializer_tester-0.0.3/setup.py` & `shipdan_serializer_tester-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='shipdan_serializer_tester',
-    version='0.0.3',
+    version='0.0.4',
     description='for shipdan_application, shipdan_operation basic ModelSerializer field test',
     author='dare',
     author_email='gdare1999@gmail.com',
     url='https://github.com/G-D4R3/shipdan_serializer_tester.git',
     install_requires=['django',],
     packages=find_packages(exclude=[]),
     keywords=['dare', 'darever', 'bunkerkids', 'shipdan', 'pypi'],
```

### Comparing `shipdan_serializer_tester-0.0.3/shipdan_serializer_tester/model_serializer_tester.py` & `shipdan_serializer_tester-0.0.4/shipdan_serializer_tester/model_serializer_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 
                 if set(model_fields) != set(serializer_fields):
                     diff_at_model = set(model_fields).difference(set(serializer_fields))
                     diff_at_serializer = set(serializer_fields).difference(set(model_fields))
                     raise cls.FieldDoesNotMatch(f'{model_name} model, serializer 간의 필드가 맞지 않음 \n    model: ',
                                                 diff_at_model, '\n    serializer', diff_at_serializer)
             except Exception as e:
-                raise cls.UnexpectedError(model_name, e)
+                raise cls.UnexpectedError(f'{model_name}: {e}')
```

