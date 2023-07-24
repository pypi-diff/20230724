# Comparing `tmp/python-schematized-config-0.0.3.tar.gz` & `tmp/python-schematized-config-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-schematized-config-0.0.3.tar", last modified: Mon Jul 24 01:52:30 2023, max compression
+gzip compressed data, was "python-schematized-config-0.0.4.tar", last modified: Mon Jul 24 04:32:38 2023, max compression
```

## Comparing `python-schematized-config-0.0.3.tar` & `python-schematized-config-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 01:52:30.772423 python-schematized-config-0.0.3/
--rw-rw-r--   0 alexhuang   (501) wheel        (0)    11337 2023-04-27 10:12:58.000000 python-schematized-config-0.0.3/LICENSE
--rw-rw-r--   0 alexhuang   (501) wheel        (0)      111 2023-04-27 10:12:58.000000 python-schematized-config-0.0.3/MANIFEST.in
--rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-24 01:52:30.772281 python-schematized-config-0.0.3/PKG-INFO
--rw-r--r--   0 alexhuang   (501) wheel        (0)      452 2023-07-17 08:24:33.000000 python-schematized-config-0.0.3/README.md
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 01:52:30.771254 python-schematized-config-0.0.3/python_schematized_config.egg-info/
--rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/PKG-INFO
--rw-r--r--   0 alexhuang   (501) wheel        (0)      509 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/SOURCES.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/dependency_links.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)       58 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/entry_points.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-06-17 02:13:48.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/not-zip-safe
--rw-r--r--   0 alexhuang   (501) wheel        (0)       72 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/requires.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)       19 2023-07-24 01:52:30.000000 python-schematized-config-0.0.3/python_schematized_config.egg-info/top_level.txt
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 01:52:30.771991 python-schematized-config-0.0.3/schematized_config/
--rw-r--r--   0 alexhuang   (501) wheel        (0)       22 2023-07-24 01:51:34.000000 python-schematized-config-0.0.3/schematized_config/__init__.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     4084 2023-07-24 01:51:50.000000 python-schematized-config-0.0.3/schematized_config/_modidx.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     2140 2023-07-24 01:51:34.000000 python-schematized-config-0.0.3/schematized_config/cli.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     6739 2023-07-24 01:51:34.000000 python-schematized-config-0.0.3/schematized_config/core.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)      993 2023-07-24 01:51:04.000000 python-schematized-config-0.0.3/settings.ini
--rw-r--r--   0 alexhuang   (501) wheel        (0)       38 2023-07-24 01:52:30.772467 python-schematized-config-0.0.3/setup.cfg
--rw-rw-r--   0 alexhuang   (501) wheel        (0)     2596 2023-04-27 10:12:58.000000 python-schematized-config-0.0.3/setup.py
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 04:32:38.370347 python-schematized-config-0.0.4/
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)    11337 2023-04-27 10:12:58.000000 python-schematized-config-0.0.4/LICENSE
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)      111 2023-04-27 10:12:58.000000 python-schematized-config-0.0.4/MANIFEST.in
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-24 04:32:38.370146 python-schematized-config-0.0.4/PKG-INFO
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      452 2023-07-17 08:24:33.000000 python-schematized-config-0.0.4/README.md
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 04:32:38.369130 python-schematized-config-0.0.4/python_schematized_config.egg-info/
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-24 04:32:38.000000 python-schematized-config-0.0.4/python_schematized_config.egg-info/PKG-INFO
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      509 2023-07-24 04:32:38.000000 python-schematized-config-0.0.4/python_schematized_config.egg-info/SOURCES.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-07-24 04:32:38.000000 python-schematized-config-0.0.4/python_schematized_config.egg-info/dependency_links.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       58 2023-07-24 04:32:38.000000 python-schematized-config-0.0.4/python_schematized_config.egg-info/entry_points.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-06-17 02:13:48.000000 python-schematized-config-0.0.4/python_schematized_config.egg-info/not-zip-safe
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       72 2023-07-24 04:32:38.000000 python-schematized-config-0.0.4/python_schematized_config.egg-info/requires.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       19 2023-07-24 04:32:38.000000 python-schematized-config-0.0.4/python_schematized_config.egg-info/top_level.txt
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-24 04:32:38.369924 python-schematized-config-0.0.4/schematized_config/
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       22 2023-07-24 04:30:50.000000 python-schematized-config-0.0.4/schematized_config/__init__.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     4084 2023-07-24 04:30:50.000000 python-schematized-config-0.0.4/schematized_config/_modidx.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     2140 2023-07-24 04:30:50.000000 python-schematized-config-0.0.4/schematized_config/cli.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     6881 2023-07-24 04:30:50.000000 python-schematized-config-0.0.4/schematized_config/core.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      993 2023-07-24 04:30:50.000000 python-schematized-config-0.0.4/settings.ini
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       38 2023-07-24 04:32:38.370410 python-schematized-config-0.0.4/setup.cfg
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)     2596 2023-04-27 10:12:58.000000 python-schematized-config-0.0.4/setup.py
```

### Comparing `python-schematized-config-0.0.3/LICENSE` & `python-schematized-config-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-schematized-config-0.0.3/PKG-INFO` & `python-schematized-config-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-schematized-config
-Version: 0.0.3
+Version: 0.0.4
 Summary: validate configs using json schema
 Home-page: https://github.com/tutankalex/python-schematized-config
 Author: tutankalex
 Author-email: 109660532+tutankalex@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-schematized-config-0.0.3/python_schematized_config.egg-info/PKG-INFO` & `python-schematized-config-0.0.4/python_schematized_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-schematized-config
-Version: 0.0.3
+Version: 0.0.4
 Summary: validate configs using json schema
 Home-page: https://github.com/tutankalex/python-schematized-config
 Author: tutankalex
 Author-email: 109660532+tutankalex@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-schematized-config-0.0.3/schematized_config/_modidx.py` & `python-schematized-config-0.0.4/schematized_config/_modidx.py`

 * *Files identical despite different names*

### Comparing `python-schematized-config-0.0.3/schematized_config/cli.py` & `python-schematized-config-0.0.4/schematized_config/cli.py`

 * *Files identical despite different names*

### Comparing `python-schematized-config-0.0.3/schematized_config/core.py` & `python-schematized-config-0.0.4/schematized_config/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,16 +127,16 @@
         if no value is provided, it will fall back to looking for
         an environment variable corresponding to the class variable
         `CONFIG_VALIDATOR_JSON_SCHEMA_ENVVAR_NAME`
         to find a JSON schema file
         '''
         self.storage_driver = storage_driver or self.__class__.DEFAULT_STORAGE_DRIVER
         if isinstance(json_schema, (str, dict)):
-            self._json_schema = self.__class__.load_json(json_schema)
-        elif (default_schema := self.__class__.get_default_json_schema()):
+            self._json_schema = self.__class__.load_json(json_schema, storage_driver=self.storage_driver)
+        elif (default_schema := self.__class__.get_default_json_schema(storage_driver=self.storage_driver)):
             self._json_schema = default_schema
         else:
             raise Exception('did not receive or find a JSON schema')
 
     def load_config(self, config: dict):
         extracted_config = extract_declared_items(self._json_schema, config)
         coerced_config = coerce_primitive_values(self._json_schema, extracted_config)
@@ -158,8 +158,9 @@
         
     @classmethod
     def load_dotenv(cls, json_schema: Union[str, dict]=None, dotenv_path: str=None, storage_driver: FS=None):
         storage_driver = storage_driver or cls.DEFAULT_STORAGE_DRIVER
         with storage_driver.open(dotenv_path) as ifile:
             config = dotenv.dotenv_values(stream=ifile)
         return cls.load_validated_config(
-            json_schema or cls.get_default_json_schema(), config)
+            json_schema or cls.get_default_json_schema(storage_driver=storage_driver),
+            config, storage_driver=storage_driver)
```

### Comparing `python-schematized-config-0.0.3/settings.ini` & `python-schematized-config-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = python-schematized-config
 lib_name = python-schematized-config
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = schematized_config
 nbs_path = nbs
 recursive = True
```

### Comparing `python-schematized-config-0.0.3/setup.py` & `python-schematized-config-0.0.4/setup.py`

 * *Files identical despite different names*

