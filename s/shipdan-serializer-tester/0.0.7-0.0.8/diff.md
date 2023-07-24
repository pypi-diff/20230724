# Comparing `tmp/shipdan_serializer_tester-0.0.7.tar.gz` & `tmp/shipdan_serializer_tester-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipdan_serializer_tester-0.0.7.tar", last modified: Mon Jul 24 02:54:06 2023, max compression
+gzip compressed data, was "shipdan_serializer_tester-0.0.8.tar", last modified: Mon Jul 24 09:24:54 2023, max compression
```

## Comparing `shipdan_serializer_tester-0.0.7.tar` & `shipdan_serializer_tester-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:54:06.951270 shipdan_serializer_tester-0.0.7/
--rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:54:06.951148 shipdan_serializer_tester-0.0.7/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.7/README.md
--rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-24 02:54:06.951314 shipdan_serializer_tester-0.0.7/setup.cfg
--rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-24 02:53:58.000000 shipdan_serializer_tester-0.0.7/setup.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:54:06.950036 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester/
--rw-r--r--   0 dare       (501) staff       (20)       60 2023-07-24 02:53:58.000000 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester/__init__.py
--rw-r--r--   0 dare       (501) staff       (20)     2635 2023-07-24 02:53:50.000000 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester/model_serializer_tester.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 02:54:06.950955 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester.egg-info/
--rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 02:54:06.000000 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester.egg-info/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-24 02:54:06.000000 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester.egg-info/SOURCES.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:54:06.000000 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester.egg-info/dependency_links.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:30:24.000000 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester.egg-info/not-zip-safe
--rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-24 02:54:06.000000 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester.egg-info/requires.txt
--rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-24 02:54:06.000000 shipdan_serializer_tester-0.0.7/shipdan_serializer_tester.egg-info/top_level.txt
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 09:24:54.339825 shipdan_serializer_tester-0.0.8/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 09:24:54.339686 shipdan_serializer_tester-0.0.8/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.8/README.md
+-rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-24 09:24:54.339865 shipdan_serializer_tester-0.0.8/setup.cfg
+-rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-24 09:24:27.000000 shipdan_serializer_tester-0.0.8/setup.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 09:24:54.338683 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester/
+-rw-r--r--   0 dare       (501) staff       (20)       60 2023-07-24 09:24:27.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester/__init__.py
+-rw-r--r--   0 dare       (501) staff       (20)     2932 2023-07-24 09:24:27.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester/model_serializer_tester.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 09:24:54.339509 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:30:24.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/not-zip-safe
+-rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/requires.txt
+-rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/top_level.txt
```

### Comparing `shipdan_serializer_tester-0.0.7/shipdan_serializer_tester/model_serializer_tester.py` & `shipdan_serializer_tester-0.0.8/shipdan_serializer_tester/model_serializer_tester.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
         def __init__(self, message=None):
             self.message = message
 
     class FieldDoesNotMatch(Exception):
         def __init__(self, message=None):
             self.message = message
 
+    class SerializerClassIsNotDefined(Exception):
+        def __init__(self, message=None):
+            self.message = message
+
     @classmethod
     def get_model_name_ls(cls, app):
         model_name_ls = []
         for x in dir(app.models):
             app_class = getattr(app.models, x)
             if not isclass(app_class):
                 continue
@@ -38,26 +42,29 @@
 
         for idx, model_name in enumerate(model_name_ls):
             print(f'[{idx+1}/{total_count}]: {model_name}')
             try:
                 model_class = getattr(model_module, model_name, None)
                 serializer_class = getattr(basic_serializer_module, f'{model_name}Serializer', None)
 
+                if serializer_class is None:
+                    raise cls.SerializerClassIsNotDefined(f'{model_name}Serializer가 정의되어있지 않습니다.')
+
                 instances = model_class.objects.all()[:10]
                 serializer = serializer_class(instances, many=True)
                 try:
                     serializer.data
                 except Exception as e:
                     raise cls.FieldNameError(message=f'{model_name}Serializer FieldNameError: {e}')
 
                 model_fields = [f.name for f in filter(lambda f: f.related_model is None, \
                                                        [f for f in model_class._meta.get_fields()])]
                 serializer_fields = serializer_class.Meta.fields
 
                 if set(model_fields) != set(serializer_fields):
                     diff_at_model = set(model_fields).difference(set(serializer_fields))
                     diff_at_serializer = set(serializer_fields).difference(set(model_fields))
-                    raise cls.FieldDoesNotMatch(f'{model_name} model, serializer 간의 필드가 맞지 않음 \n    model: ',
+                    raise cls.FieldDoesNotMatch(f'[{model_name}] model, serializer 간의 필드가 맞지 않음 \n    model: ',
                                                 diff_at_model, '\n    serializer', diff_at_serializer)
             except Exception as e:
                 raise cls.UnexpectedError(f'{model_name}: {e}')
         print("Success!!")
```

