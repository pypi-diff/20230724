# Comparing `tmp/speedtab-0.1.6.1.tar.gz` & `tmp/speedtab-0.1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.6.1.tar", max compression
+gzip compressed data, was "speedtab-0.1.6.2.tar", max compression
```

## Comparing `speedtab-0.1.6.1.tar` & `speedtab-0.1.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-07-21 20:57:46.159084 speedtab-0.1.6.1/pyproject.toml
--rw-r--r--   0        0        0      313 2023-07-21 14:14:08.403849 speedtab-0.1.6.1/speedtab/__init__.py
--rw-r--r--   0        0        0    51847 2023-07-21 20:57:46.065818 speedtab-0.1.6.1/speedtab/client.py
--rw-r--r--   0        0        0     6464 2023-07-21 14:14:08.469136 speedtab-0.1.6.1/speedtab/enums.py
--rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.6.1/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-07-21 20:58:04.014891 speedtab-0.1.6.1/setup.py
--rw-r--r--   0        0        0      808 2023-07-21 20:58:04.014891 speedtab-0.1.6.1/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-07-24 09:11:55.065664 speedtab-0.1.6.2/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-07-21 14:14:08.403849 speedtab-0.1.6.2/speedtab/__init__.py
+-rw-r--r--   0        0        0    51824 2023-07-21 20:59:49.745007 speedtab-0.1.6.2/speedtab/client.py
+-rw-r--r--   0        0        0     6464 2023-07-21 14:14:08.469136 speedtab-0.1.6.2/speedtab/enums.py
+-rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.6.2/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-07-24 09:12:13.094374 speedtab-0.1.6.2/setup.py
+-rw-r--r--   0        0        0      808 2023-07-24 09:12:13.095384 speedtab-0.1.6.2/PKG-INFO
```

### Comparing `speedtab-0.1.6.1/pyproject.toml` & `speedtab-0.1.6.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.6.1"
+version = "0.1.6.2"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.6.1/speedtab/client.py` & `speedtab-0.1.6.2/speedtab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import io
 import re
 from datetime import datetime, date
 from itertools import zip_longest
 from typing import Union
 
-from pprint import pp
 import numpy as np
 import pandas as pd
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaIoBaseDownload
```

### Comparing `speedtab-0.1.6.1/speedtab/enums.py` & `speedtab-0.1.6.2/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.6.1/speedtab/formats.py` & `speedtab-0.1.6.2/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.6.1/setup.py` & `speedtab-0.1.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.6.1',
+    'version': '0.1.6.2',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.6.1/PKG-INFO` & `speedtab-0.1.6.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.6.1
+Version: 0.1.6.2
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

