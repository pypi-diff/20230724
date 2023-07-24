# Comparing `tmp/speedtab-0.1.6.3.tar.gz` & `tmp/speedtab-0.1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.6.3.tar", max compression
+gzip compressed data, was "speedtab-0.1.6.4.tar", max compression
```

## Comparing `speedtab-0.1.6.3.tar` & `speedtab-0.1.6.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-07-24 13:34:35.103189 speedtab-0.1.6.3/pyproject.toml
--rw-r--r--   0        0        0      354 2023-07-24 13:24:26.057717 speedtab-0.1.6.3/speedtab/__init__.py
--rw-r--r--   0        0        0    52586 2023-07-24 13:32:31.325512 speedtab-0.1.6.3/speedtab/client.py
--rw-r--r--   0        0        0     6464 2023-07-21 14:14:08.469136 speedtab-0.1.6.3/speedtab/enums.py
--rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.6.3/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-07-24 13:34:51.155866 speedtab-0.1.6.3/setup.py
--rw-r--r--   0        0        0      808 2023-07-24 13:34:51.157283 speedtab-0.1.6.3/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-07-24 13:56:01.978805 speedtab-0.1.6.4/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-07-24 13:24:26.057717 speedtab-0.1.6.4/speedtab/__init__.py
+-rw-r--r--   0        0        0    52586 2023-07-24 13:32:31.325512 speedtab-0.1.6.4/speedtab/client.py
+-rw-r--r--   0        0        0     6520 2023-07-24 13:55:52.073795 speedtab-0.1.6.4/speedtab/enums.py
+-rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.6.4/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-07-24 13:56:26.649026 speedtab-0.1.6.4/setup.py
+-rw-r--r--   0        0        0      808 2023-07-24 13:56:26.650027 speedtab-0.1.6.4/PKG-INFO
```

### Comparing `speedtab-0.1.6.3/pyproject.toml` & `speedtab-0.1.6.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.6.3"
+version = "0.1.6.4"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.6.3/speedtab/client.py` & `speedtab-0.1.6.4/speedtab/client.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.6.3/speedtab/enums.py` & `speedtab-0.1.6.4/speedtab/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,17 @@
     DATE_ON_OR_AFTER = 'DATE_ON_OR_AFTER'
     DATE_BETWEEN = 'DATE_BETWEEN'
     DATE_NOT_BETWEEN = 'DATE_NOT_BETWEEN'
     DATE_IS_VALID = 'DATE_IS_VALID'
     ONE_OF_RANGE = 'ONE_OF_RANGE'
     ONE_OF_LIST = 'ONE_OF_LIST'
     BLANK = 'BLANK'
+    IS_EMPTY = 'BLANK'
     NOT_BLANK = 'NOT_BLANK'
+    IS_NOT_EMPTY = 'NOT_BLANK'
     CUSTOM_FORMULA = 'CUSTOM_FORMULA'
     BOOLEAN = 'BOOLEAN'
     TEXT_NOT_EQ = 'TEXT_NOT_EQ'
     DATE_NOT_EQ = 'DATE_NOT_EQ'
 
 
 class DefaultColors:
```

### Comparing `speedtab-0.1.6.3/speedtab/formats.py` & `speedtab-0.1.6.4/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.6.3/setup.py` & `speedtab-0.1.6.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.6.3',
+    'version': '0.1.6.4',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.6.3/PKG-INFO` & `speedtab-0.1.6.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.6.3
+Version: 0.1.6.4
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

