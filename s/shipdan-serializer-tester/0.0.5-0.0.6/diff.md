# Comparing `tmp/shipdan_serializer_tester-0.0.5.tar.gz` & `tmp/shipdan_serializer_tester-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipdan_serializer_tester-0.0.5.tar", last modified: Mon Jul 24 02:47:45 2023, max compression
+gzip compressed data, was "shipdan_serializer_tester-0.0.6.tar", last modified: Mon Jul 24 02:53:06 2023, max compression
```

## Comparing `shipdan_serializer_tester-0.0.5.tar` & `shipdan_serializer_tester-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:47:45.626468 shipdan_serializer_tester-0.0.5/
--rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:47:45.626365 shipdan_serializer_tester-0.0.5/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.5/README.md
--rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-24 02:47:45.626501 shipdan_serializer_tester-0.0.5/setup.cfg
--rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-24 02:47:23.000000 shipdan_serializer_tester-0.0.5/setup.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:47:45.625527 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester/
--rw-r--r--   0 dare       (501) staff       (20)       60 2023-07-24 02:47:23.000000 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester/__init__.py
--rw-r--r--   0 dare       (501) staff       (20)     2492 2023-07-24 02:46:40.000000 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester/model_serializer_tester.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:47:45.626218 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester.egg-info/
--rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:47:45.000000 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester.egg-info/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-24 02:47:45.000000 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester.egg-info/SOURCES.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:47:45.000000 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester.egg-info/dependency_links.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:30:24.000000 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester.egg-info/not-zip-safe
--rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-24 02:47:45.000000 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester.egg-info/requires.txt
--rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-24 02:47:45.000000 shipdan_serializer_tester-0.0.5/shipdan_serializer_tester.egg-info/top_level.txt
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:53:06.284545 shipdan_serializer_tester-0.0.6/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:53:06.284406 shipdan_serializer_tester-0.0.6/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.6/README.md
+-rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-24 02:53:06.284591 shipdan_serializer_tester-0.0.6/setup.cfg
+-rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-24 02:53:05.000000 shipdan_serializer_tester-0.0.6/setup.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:53:06.283279 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester/
+-rw-r--r--   0 dare       (501) staff       (20)       60 2023-07-24 02:53:05.000000 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester/__init__.py
+-rw-r--r--   0 dare       (501) staff       (20)     2633 2023-07-24 02:52:49.000000 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester/model_serializer_tester.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:53:06.284157 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester.egg-info/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:53:06.000000 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester.egg-info/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-24 02:53:06.000000 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:53:06.000000 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:30:24.000000 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester.egg-info/not-zip-safe
+-rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-24 02:53:06.000000 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester.egg-info/requires.txt
+-rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-24 02:53:06.000000 shipdan_serializer_tester-0.0.6/shipdan_serializer_tester.egg-info/top_level.txt
```

### Comparing `shipdan_serializer_tester-0.0.5/setup.py` & `shipdan_serializer_tester-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='shipdan_serializer_tester',
-    version='0.0.5',
+    version='0.0.6',
     description='for shipdan_application, shipdan_operation basic ModelSerializer field test',
     author='dare',
     author_email='gdare1999@gmail.com',
     url='https://github.com/G-D4R3/shipdan_serializer_tester.git',
     install_requires=['django',],
     packages=find_packages(exclude=[]),
     keywords=['dare', 'darever', 'bunkerkids', 'shipdan', 'pypi'],
```

### Comparing `shipdan_serializer_tester-0.0.5/shipdan_serializer_tester/model_serializer_tester.py` & `shipdan_serializer_tester-0.0.6/shipdan_serializer_tester/model_serializer_tester.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,17 +30,18 @@
                 continue
             model_name_ls.append(x)
 
         return model_name_ls
 
     @classmethod
     def test_model_serializer(cls, model_module, model_name_ls, basic_serializer_module):
+        total_count = len(model_name_ls)
 
-        for model_name in model_name_ls:
-
+        for idx, model_name in enumerate(model_name_ls):
+            print(f'[{idx}/{total_count}]: {model_name}')
             try:
                 model_class = getattr(model_module, model_name, None)
                 serializer_class = getattr(basic_serializer_module, f'{model_name}Serializer', None)
 
                 instances = model_class.objects.all()[:10]
                 serializer = serializer_class(instances, many=True)
                 try:
@@ -55,7 +56,8 @@
                 if set(model_fields) != set(serializer_fields):
                     diff_at_model = set(model_fields).difference(set(serializer_fields))
                     diff_at_serializer = set(serializer_fields).difference(set(model_fields))
                     raise cls.FieldDoesNotMatch(f'{model_name} model, serializer 간의 필드가 맞지 않음 \n    model: ',
                                                 diff_at_model, '\n    serializer', diff_at_serializer)
             except Exception as e:
                 raise cls.UnexpectedError(f'{model_name}: {e}')
+        print("Success!!")
```

