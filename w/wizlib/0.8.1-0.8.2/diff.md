# Comparing `tmp/wizlib-0.8.1.tar.gz` & `tmp/wizlib-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.8.1.tar", last modified: Sun Jul 23 22:46:21 2023, max compression
+gzip compressed data, was "wizlib-0.8.2.tar", last modified: Mon Jul 24 03:44:08 2023, max compression
```

## Comparing `wizlib-0.8.1.tar` & `wizlib-0.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:46:21.005479 wizlib-0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-23 22:45:32.000000 wizlib-0.8.1/.version
--rw-r--r--   0 root         (0) root         (0)     5384 2023-07-23 22:46:21.005479 wizlib-0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-23 22:46:12.000000 wizlib-0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-23 22:46:12.000000 wizlib-0.8.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-23 22:46:21.005479 wizlib-0.8.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:46:21.002479 wizlib-0.8.1/test/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-23 22:46:12.000000 wizlib-0.8.1/test/test_class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-23 22:46:12.000000 wizlib-0.8.1/test/test_command_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2023-07-23 22:46:12.000000 wizlib-0.8.1/test/test_config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-23 22:46:12.000000 wizlib-0.8.1/test/test_super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:46:21.003479 wizlib-0.8.1/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-23 22:46:12.000000 wizlib-0.8.1/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-23 22:46:12.000000 wizlib-0.8.1/wizlib/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2023-07-23 22:46:12.000000 wizlib-0.8.1/wizlib/command_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2211 2023-07-23 22:46:12.000000 wizlib-0.8.1/wizlib/config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-23 22:46:12.000000 wizlib-0.8.1/wizlib/rlinput.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-23 22:46:12.000000 wizlib-0.8.1/wizlib/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:46:21.004479 wizlib-0.8.1/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5384 2023-07-23 22:46:20.000000 wizlib-0.8.1/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-07-23 22:46:20.000000 wizlib-0.8.1/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-23 22:46:20.000000 wizlib-0.8.1/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-23 22:46:20.000000 wizlib-0.8.1/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-23 22:46:20.000000 wizlib-0.8.1/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 03:44:08.594240 wizlib-0.8.2/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-24 03:43:18.000000 wizlib-0.8.2/.version
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-24 03:44:08.594240 wizlib-0.8.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-24 03:43:59.000000 wizlib-0.8.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-24 03:43:59.000000 wizlib-0.8.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 03:44:08.594240 wizlib-0.8.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 03:44:08.591240 wizlib-0.8.2/test/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-24 03:43:59.000000 wizlib-0.8.2/test/test_class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-24 03:43:59.000000 wizlib-0.8.2/test/test_command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3150 2023-07-24 03:43:59.000000 wizlib-0.8.2/test/test_config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-24 03:43:59.000000 wizlib-0.8.2/test/test_super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 03:44:08.592239 wizlib-0.8.2/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 03:43:59.000000 wizlib-0.8.2/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-24 03:43:59.000000 wizlib-0.8.2/wizlib/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2023-07-24 03:43:59.000000 wizlib-0.8.2/wizlib/command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-24 03:43:59.000000 wizlib-0.8.2/wizlib/config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-24 03:43:59.000000 wizlib-0.8.2/wizlib/rlinput.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-24 03:43:59.000000 wizlib-0.8.2/wizlib/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 03:44:08.594240 wizlib-0.8.2/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-24 03:44:08.000000 wizlib-0.8.2/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      427 2023-07-24 03:44:08.000000 wizlib-0.8.2/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 03:44:08.000000 wizlib-0.8.2/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-24 03:44:08.000000 wizlib-0.8.2/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 03:44:08.000000 wizlib-0.8.2/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.8.1/PKG-INFO` & `wizlib-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.8.1
+Version: 0.8.2
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

### Comparing `wizlib-0.8.1/README.md` & `wizlib-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.1/pyproject.toml` & `wizlib-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.1/test/test_command_handler.py` & `wizlib-0.8.2/test/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.1/test/test_config_machine.py` & `wizlib-0.8.2/test/test_config_machine.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,7 +79,12 @@
 
     def works_another_way(self):
         with patch('pathlib.Path.cwd',
                    lambda: Path('test/data_config_machine')):
             test_machine = SampleOtherMachine()
             f = test_machine.config_get('bar-zing')
         self.assertEqual(f, 'waa')
+
+    def test_nested_as_attribute(self):
+        c = SampleMachine()
+        c.a_b = 'c'
+        self.assertEqual(c.config_get('a-b'), 'c')
```

### Comparing `wizlib-0.8.1/test/test_super_wrapper.py` & `wizlib-0.8.2/test/test_super_wrapper.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.1/wizlib/class_family.py` & `wizlib-0.8.2/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.1/wizlib/command_handler.py` & `wizlib-0.8.2/wizlib/command_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.1/wizlib/config_machine.py` & `wizlib-0.8.2/wizlib/config_machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,24 @@
 
     @staticmethod
     def env(name):
         if (envvar := name.upper().replace('-', '_')) in os.environ:
             return os.environ[envvar]
 
     def config_get(self, key: str):
-        if hasattr(self, key) and (result := getattr(self, key)):
+        attr = key.replace('-', '_')
+        if hasattr(self, attr) and (result := getattr(self, attr)):
             return result
         if (result := self.env(key)):
             return result
         if (yaml := self.config_yaml):
             split = key.split('-')
             while (val := split.pop(0)) and (val in yaml):
                 yaml = yaml[val] if val in yaml else None
                 if not split:
                     return yaml
 
     @classmethod
     def add_app_args(self, parser):
-        """Allows a Command class to also inherit from ConfigMachine."""
+        """Allows a Command class to also inherit from ConfigMachine. List
+        ConfigMachine first."""
         parser.add_argument('--config', action='store')
```

### Comparing `wizlib-0.8.1/wizlib/rlinput.py` & `wizlib-0.8.2/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.1/wizlib.egg-info/PKG-INFO` & `wizlib-0.8.2/wizlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.8.1
+Version: 0.8.2
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

