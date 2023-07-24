# Comparing `tmp/clearconf-0.3.3.tar.gz` & `tmp/clearconf-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearconf-0.3.3.tar", max compression
+gzip compressed data, was "clearconf-0.3.4.tar", max compression
```

## Comparing `clearconf-0.3.3.tar` & `clearconf-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.3/README.md
--rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/assets/example_conf.py
--rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/assets/init.py
--rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/assets/stub_conf.py
--rw-r--r--   0        0        0     7278 2023-07-19 14:33:19.976638 clearconf-0.3.3/clearconf/base_config.py
--rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/cli/__init__.py
--rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/cli/defaults.py
--rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/cli/main.py
--rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/utils/conf.py
--rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/utils/file.py
--rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/utils/stdout.py
--rw-r--r--   0        0        0      723 2023-07-19 14:36:56.627521 clearconf-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3524 1970-01-01 00:00:00.000000 clearconf-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.4/README.md
+-rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/assets/example_conf.py
+-rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/assets/init.py
+-rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/assets/stub_conf.py
+-rw-r--r--   0        0        0     7364 2023-07-24 14:41:17.515170 clearconf-0.3.4/clearconf/base_config.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/cli/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/cli/defaults.py
+-rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/utils/conf.py
+-rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/utils/file.py
+-rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.4/clearconf/utils/stdout.py
+-rw-r--r--   0        0        0      723 2023-07-24 14:42:06.295410 clearconf-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3524 1970-01-01 00:00:00.000000 clearconf-0.3.4/PKG-INFO
```

### Comparing `clearconf-0.3.3/README.md` & `clearconf-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.3/clearconf/assets/example_conf.py` & `clearconf-0.3.4/clearconf/assets/example_conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.3/clearconf/assets/init.py` & `clearconf-0.3.4/clearconf/assets/init.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.3/clearconf/base_config.py` & `clearconf-0.3.4/clearconf/base_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,16 @@
                     # if we are executing the config the module is __main__. If we are importing it is config
                     # Not ideal but config could be anywhere in the name
                     # Need to find a better way to do this
                     if attr.__module__.split('.')[0] == '__main__' or 'config' in attr.__module__:
                         # This way the module keeps its subclasses but it is also subclassed by
                         # BaseConfig inheriting its method. A security check could be used to assure
                         # that the new methods are not overriding any old one.
-                        setattr(target, k, type(f'{k}_mod', (BaseConfig, ) + tuple(attr.__mro__), dict(list(dict(vars(BaseConfig)).items()) + list(dict(vars(attr)).items()))))
+                        if 'BaseConfig' not in [a.__name__ for a in attr.mro()]:
+                            setattr(target, k, type(f'{k}_mod', (BaseConfig, ) + tuple(attr.__mro__), dict(list(dict(vars(BaseConfig)).items()) + list(dict(vars(attr)).items()))))
         return res
 
     @classmethod
     def to_flat_dict(cls) -> dict:
         import torch
         res = cls.to_dict()
         res = flatten(res)
```

### Comparing `clearconf-0.3.3/clearconf/cli/defaults.py` & `clearconf-0.3.4/clearconf/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.3/clearconf/cli/main.py` & `clearconf-0.3.4/clearconf/cli/main.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.3/clearconf/utils/conf.py` & `clearconf-0.3.4/clearconf/utils/conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.3/clearconf/utils/file.py` & `clearconf-0.3.4/clearconf/utils/file.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.3/pyproject.toml` & `clearconf-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clearconf"
-version = "0.3.3"
+version = "0.3.4"
 description = "ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class."
 authors = ["andrearosasco <andrea.rosasco@iit.it>"]
 homepage = "https://github.com/andrearosasco/clearconf"
 repository = "https://github.com/andrearosasco/clearconf"
 readme = "README.md"
```

### Comparing `clearconf-0.3.3/PKG-INFO` & `clearconf-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearconf
-Version: 0.3.3
+Version: 0.3.4
 Summary: ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class.
 Home-page: https://github.com/andrearosasco/clearconf
 Author: andrearosasco
 Author-email: andrea.rosasco@iit.it
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

