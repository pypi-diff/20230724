# Comparing `tmp/speedtab-0.1.6.5.tar.gz` & `tmp/speedtab-0.1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.6.5.tar", max compression
+gzip compressed data, was "speedtab-0.1.6.6.tar", max compression
```

## Comparing `speedtab-0.1.6.5.tar` & `speedtab-0.1.6.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-07-24 15:18:03.430087 speedtab-0.1.6.5/pyproject.toml
--rw-r--r--   0        0        0      354 2023-07-24 13:24:26.057717 speedtab-0.1.6.5/speedtab/__init__.py
--rw-r--r--   0        0        0    53041 2023-07-24 15:20:35.119532 speedtab-0.1.6.5/speedtab/client.py
--rw-r--r--   0        0        0     6520 2023-07-24 13:55:52.073795 speedtab-0.1.6.5/speedtab/enums.py
--rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.6.5/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-07-24 15:20:43.232000 speedtab-0.1.6.5/setup.py
--rw-r--r--   0        0        0      808 2023-07-24 15:20:43.232000 speedtab-0.1.6.5/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-07-24 15:43:35.768466 speedtab-0.1.6.6/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-07-24 13:24:26.057717 speedtab-0.1.6.6/speedtab/__init__.py
+-rw-r--r--   0        0        0    53087 2023-07-24 15:43:35.720422 speedtab-0.1.6.6/speedtab/client.py
+-rw-r--r--   0        0        0     6520 2023-07-24 13:55:52.073795 speedtab-0.1.6.6/speedtab/enums.py
+-rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.6.6/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-07-24 15:43:44.183059 speedtab-0.1.6.6/setup.py
+-rw-r--r--   0        0        0      808 2023-07-24 15:43:44.183059 speedtab-0.1.6.6/PKG-INFO
```

### Comparing `speedtab-0.1.6.5/pyproject.toml` & `speedtab-0.1.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.6.5"
+version = "0.1.6.6"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.6.5/speedtab/client.py` & `speedtab-0.1.6.6/speedtab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,22 +101,23 @@
     if isinstance(l, (list, tuple)):
         return max(map(depth, l)) + 1
     else:
         return 0
 
 
 class BooleanCondition:
-    def __init__(self, type: BooleanConditionTypes, value):
+    def __init__(self, type: BooleanConditionTypes, value=None):
         self.type = type
         self.value = value
 
     def boolean_condition(self):
-        if type in (BooleanConditionTypes.BLANK, BooleanConditionTypes.NOT_BLANK, BooleanConditionTypes.IS_NOT_EMPTY,
-                    BooleanConditionTypes.IS_EMPTY, BooleanConditionTypes.TEXT_IS_URL,
-                    BooleanConditionTypes.TEXT_IS_EMAIL, BooleanConditionTypes.DATE_IS_VALID):
+        if self.type in (BooleanConditionTypes.BLANK, BooleanConditionTypes.NOT_BLANK,
+                         BooleanConditionTypes.IS_NOT_EMPTY,
+                         BooleanConditionTypes.IS_EMPTY, BooleanConditionTypes.TEXT_IS_URL,
+                         BooleanConditionTypes.TEXT_IS_EMAIL, BooleanConditionTypes.DATE_IS_VALID):
             return {
                 'condition': {
                     'type': self.type
                 }}
         else:
             return {
                 'condition': {
```

### Comparing `speedtab-0.1.6.5/speedtab/enums.py` & `speedtab-0.1.6.6/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.6.5/speedtab/formats.py` & `speedtab-0.1.6.6/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.6.5/setup.py` & `speedtab-0.1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.6.5',
+    'version': '0.1.6.6',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.6.5/PKG-INFO` & `speedtab-0.1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.6.5
+Version: 0.1.6.6
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

