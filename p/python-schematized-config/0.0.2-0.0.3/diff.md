# Comparing `tmp/python-schematized-config-0.0.2.tar.gz` & `tmp/python-schematized-config-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-schematized-config-0.0.2.tar", last modified: Tue Jul 18 09:02:07 2023, max compression
+gzip compressed data, was "python-schematized-config-0.0.3.tar", last modified: Mon Jul 24 01:52:30 2023, max compression
```

## Comparing `python-schematized-config-0.0.2.tar` & `python-schematized-config-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-18 09:02:07.444052 python-schematized-config-0.0.2/
--rw-rw-r--   0 alexhuang   (501) wheel        (0)    11337 2023-04-27 10:12:58.000000 python-schematized-config-0.0.2/LICENSE
--rw-rw-r--   0 alexhuang   (501) wheel        (0)      111 2023-04-27 10:12:58.000000 python-schematized-config-0.0.2/MANIFEST.in
--rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-18 09:02:07.443913 python-schematized-config-0.0.2/PKG-INFO
--rw-r--r--   0 alexhuang   (501) wheel        (0)      452 2023-07-17 08:24:33.000000 python-schematized-config-0.0.2/README.md
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-18 09:02:07.443184 python-schematized-config-0.0.2/python_schematized_config.egg-info/
--rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/PKG-INFO
--rw-r--r--   0 alexhuang   (501) wheel        (0)      509 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/SOURCES.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/dependency_links.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)       58 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/entry_points.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-06-17 02:13:48.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/not-zip-safe
--rw-r--r--   0 alexhuang   (501) wheel        (0)       72 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/requires.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)       19 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/top_level.txt
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-18 09:02:07.443732 python-schematized-config-0.0.2/schematized_config/
--rw-r--r--   0 alexhuang   (501) wheel        (0)       22 2023-07-18 09:00:39.000000 python-schematized-config-0.0.2/schematized_config/__init__.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     4084 2023-07-18 09:00:39.000000 python-schematized-config-0.0.2/schematized_config/_modidx.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     2140 2023-07-18 09:00:39.000000 python-schematized-config-0.0.2/schematized_config/cli.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     6365 2023-07-18 09:00:39.000000 python-schematized-config-0.0.2/schematized_config/core.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)      993 2023-07-18 08:59:24.000000 python-schematized-config-0.0.2/settings.ini
--rw-r--r--   0 alexhuang   (501) wheel        (0)       38 2023-07-18 09:02:07.444095 python-schematized-config-0.0.2/setup.cfg
--rw-rw-r--   0 alexhuang   (501) wheel        (0)     2596 2023-04-27 10:12:58.000000 python-schematized-config-0.0.2/setup.py
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 01:52:30.772423 python-schematized-config-0.0.3/
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)    11337 2023-04-27 10:12:58.000000 python-schematized-config-0.0.3/LICENSE
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)      111 2023-04-27 10:12:58.000000 python-schematized-config-0.0.3/MANIFEST.in
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-24 01:52:30.772281 python-schematized-config-0.0.3/PKG-INFO
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      452 2023-07-17 08:24:33.000000 python-schematized-config-0.0.3/README.md
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 01:52:30.771254 python-schematized-config-0.0.3/python_schematized_config.egg-info/
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/PKG-INFO
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      509 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/SOURCES.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/dependency_links.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       58 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/entry_points.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-06-17 02:13:48.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/not-zip-safe
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       72 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/requires.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       19 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/top_level.txt
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 01:52:30.771991 python-schematized-config-0.0.3/schematized_config/
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       22 2023-07-24 01:51:34.000000 python-schematized-config-0.0.3/schematized_config/__init__.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     4084 2023-07-24 01:51:50.000000 python-schematized-config-0.0.3/schematized_config/_modidx.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     2140 2023-07-24 01:51:34.000000 python-schematized-config-0.0.3/schematized_config/cli.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     6739 2023-07-24 01:51:34.000000 python-schematized-config-0.0.3/schematized_config/core.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      993 2023-07-24 01:51:04.000000 python-schematized-config-0.0.3/settings.ini
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       38 2023-07-24 01:52:30.772467 python-schematized-config-0.0.3/setup.cfg
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)     2596 2023-04-27 10:12:58.000000 python-schematized-config-0.0.3/setup.py
```

### Comparing `python-schematized-config-0.0.2/LICENSE` & `python-schematized-config-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-schematized-config-0.0.2/PKG-INFO` & `python-schematized-config-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-schematized-config
-Version: 0.0.2
+Version: 0.0.3
 Summary: validate configs using json schema
 Home-page: https://github.com/tutankalex/python-schematized-config
 Author: tutankalex
 Author-email: 109660532+tutankalex@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-schematized-config-0.0.2/python_schematized_config.egg-info/PKG-INFO` & `python-schematized-config-0.0.3/python_schematized_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-schematized-config
-Version: 0.0.2
+Version: 0.0.3
 Summary: validate configs using json schema
 Home-page: https://github.com/tutankalex/python-schematized-config
 Author: tutankalex
 Author-email: 109660532+tutankalex@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-schematized-config-0.0.2/schematized_config/_modidx.py` & `python-schematized-config-0.0.3/schematized_config/_modidx.py`

 * *Files identical despite different names*

### Comparing `python-schematized-config-0.0.2/schematized_config/cli.py` & `python-schematized-config-0.0.3/schematized_config/cli.py`

 * *Files identical despite different names*

### Comparing `python-schematized-config-0.0.2/schematized_config/core.py` & `python-schematized-config-0.0.3/schematized_config/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,31 +94,33 @@
 class ConfigValidator(object):
 
     DEFAULT_STORAGE_DRIVER: FS = OSFS('.')
     
     CONFIG_VALIDATOR_JSON_SCHEMA_ENVVAR_NAME = 'CONFIG_VALIDATOR_JSON_SCHEMA'
 
     @classmethod
-    def load_json(cls, json_source: Union[str, dict]=None) -> dict:
+    def load_json(cls, json_source: Union[str, dict]=None, storage_driver: FS = None) -> dict:
         '''
         convenience method to return a dict from either
         a file path or an already-loaded dict
         '''
+        storage_driver = storage_driver or cls.DEFAULT_STORAGE_DRIVER
         if isinstance(json_source, str):
-            with cls.DEFAULT_STORAGE_DRIVER.open(json_source) as ifile:
+            with storage_driver.open(json_source) as ifile:
                 return json.load(ifile)
         elif isinstance(json_source, dict):
             return json_source
 
     @classmethod
-    def get_default_json_schema(cls):
+    def get_default_json_schema(cls, storage_driver: FS = None) -> dict:
+        storage_driver = storage_driver or cls.DEFAULT_STORAGE_DRIVER
         if cls.CONFIG_VALIDATOR_JSON_SCHEMA_ENVVAR_NAME in os.environ:
             expected_json_schema_path = \
                 os.environ[cls.CONFIG_VALIDATOR_JSON_SCHEMA_ENVVAR_NAME]
-            with cls.DEFAULT_STORAGE_DRIVER.open(expected_json_schema_path) as ifile:
+            with storage_driver.open(expected_json_schema_path) as ifile:
                 return json.load(ifile)
         return None
 
     def __init__(self, json_schema: Union[str, dict]=None, storage_driver: FS=None):
         '''
         :param json_schema: a str path to a json schema file, or a schema in dict form
         
@@ -143,19 +145,21 @@
         if errors:
             for error in errors:
                 logger.error(f'{error.json_path}:\t{error.message}')
             raise ConfigValidatorException(errors)
         return coerced_config
     
     @classmethod
-    def load_validated_config(cls, json_schema: Union[str, dict], config: dict):
-        return cls(json_schema).load_config(config)
+    def load_validated_config(cls, json_schema: Union[str, dict], config: dict, **kwargs):
+        return cls(json_schema, **kwargs).load_config(config)
 
     @classmethod
-    def load_validated_environment(cls, json_schema: Union[str, dict]=None):
-        return cls.load_validated_config(json_schema, dict(os.environ))
+    def load_validated_environment(cls, json_schema: Union[str, dict]=None, **kwargs):
+        return cls.load_validated_config(json_schema, dict(os.environ), **kwargs)
         
     @classmethod
-    def load_dotenv(cls, json_schema: Union[str, dict]=None, dotenv_path: str=None):
-        config = dotenv.dotenv_values(dotenv_path)
+    def load_dotenv(cls, json_schema: Union[str, dict]=None, dotenv_path: str=None, storage_driver: FS=None):
+        storage_driver = storage_driver or cls.DEFAULT_STORAGE_DRIVER
+        with storage_driver.open(dotenv_path) as ifile:
+            config = dotenv.dotenv_values(stream=ifile)
         return cls.load_validated_config(
             json_schema or cls.get_default_json_schema(), config)
```

### Comparing `python-schematized-config-0.0.2/settings.ini` & `python-schematized-config-0.0.3/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = python-schematized-config
 lib_name = python-schematized-config
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = schematized_config
 nbs_path = nbs
 recursive = True
```

### Comparing `python-schematized-config-0.0.2/setup.py` & `python-schematized-config-0.0.3/setup.py`

 * *Files identical despite different names*

