# Comparing `tmp/edfi-sql-adapter-1.0.1a1.tar.gz` & `tmp/edfi_sql_adapter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edfi-sql-adapter-1.0.1a1.tar", max compression
+gzip compressed data, was "edfi_sql_adapter-1.0.2.tar", max compression
```

## Comparing `edfi-sql-adapter-1.0.1a1.tar` & `edfi_sql_adapter-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2021-06-16 21:15:51.746131 edfi-sql-adapter-1.0.1a1/edfi_sql_adapter/__init__.py
--rw-r--r--   0        0        0        0 2021-09-27 18:39:06.329642 edfi-sql-adapter-1.0.1a1/edfi_sql_adapter/py.typed
--rw-r--r--   0        0        0     7694 2021-11-29 16:36:55.760702 edfi-sql-adapter-1.0.1a1/edfi_sql_adapter/sql_adapter.py
--rw-r--r--   0        0        0      777 2021-11-29 16:31:24.427138 edfi-sql-adapter-1.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      994 2021-06-16 21:15:51.746131 edfi-sql-adapter-1.0.1a1/README.md
--rw-r--r--   0        0        0     1795 2021-11-29 16:37:11.091562 edfi-sql-adapter-1.0.1a1/setup.py
--rw-r--r--   0        0        0     1686 2021-11-29 16:37:11.091562 edfi-sql-adapter-1.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-06-16 21:15:51.746131 edfi_sql_adapter-1.0.2/edfi_sql_adapter/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-27 18:39:06.329642 edfi_sql_adapter-1.0.2/edfi_sql_adapter/py.typed
+-rw-r--r--   0        0        0     7694 2022-01-20 21:55:02.512732 edfi_sql_adapter-1.0.2/edfi_sql_adapter/sql_adapter.py
+-rw-r--r--   0        0        0      765 2023-07-24 19:25:29.781985 edfi_sql_adapter-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      994 2022-02-01 20:58:34.124895 edfi_sql_adapter-1.0.2/README.md
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 edfi_sql_adapter-1.0.2/setup.py
+-rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 edfi_sql_adapter-1.0.2/PKG-INFO
```

### Comparing `edfi-sql-adapter-1.0.1a1/edfi_sql_adapter/sql_adapter.py` & `edfi_sql_adapter-1.0.2/edfi_sql_adapter/sql_adapter.py`

 * *Files identical despite different names*

### Comparing `edfi-sql-adapter-1.0.1a1/pyproject.toml` & `edfi_sql_adapter-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "edfi-sql-adapter"
-version = "1.0.1-alpha.1"
+version = "1.0.2"
 description = "Lightweight wrapper to facilitate connections to SQL databases"
 authors = ["Ed-Fi Alliance, LLC, and contributors"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://techdocs.ed-fi.org/display/EDFITOOLS/LMS+Toolkit"
 repository = "https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit"
 include = ["edfi_sql_adapter/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyodbc = "^4.0.30"
 psycopg2 = "^2.8.6"
-SQLAlchemy = "1.3.23"
+SQLAlchemy = "~1"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.9.2"
 coverage = "^5.5"
 mypy = "^0.902"
 black = "^21.6b0"
 pytest = "^6.2.4"
```

### Comparing `edfi-sql-adapter-1.0.1a1/README.md` & `edfi_sql_adapter-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This package is light on unit tests, because the functions are well tested from
 an integration perspective. Would be nice to add unit tests for error handling
 in particular, but that would mean a lot of mocking of SQLAlchemy.
 
 ## Legal Information
 
-Copyright (c) 2021 Ed-Fi Alliance, LLC and contributors.
+Copyright (c) 2022 Ed-Fi Alliance, LLC and contributors.
 
 Licensed under the [Apache License, Version
 2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the
 "License").
 
 Unless required by applicable law or agreed to in writing, software distributed
 under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
```

### Comparing `edfi-sql-adapter-1.0.1a1/setup.py` & `edfi_sql_adapter-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['edfi_sql_adapter']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['SQLAlchemy==1.3.23', 'psycopg2>=2.8.6,<3.0.0', 'pyodbc>=4.0.30,<5.0.0']
+['SQLAlchemy>=1,<2', 'psycopg2>=2.8.6,<3.0.0', 'pyodbc>=4.0.30,<5.0.0']
 
 setup_kwargs = {
     'name': 'edfi-sql-adapter',
-    'version': '1.0.1a1',
+    'version': '1.0.2',
     'description': 'Lightweight wrapper to facilitate connections to SQL databases',
-    'long_description': '# edfi-sql-adapter\n\nLightweight wrapper to facilitate connections to SQL databases.\n\n## Developer Notes\n\nThis package is light on unit tests, because the functions are well tested from\nan integration perspective. Would be nice to add unit tests for error handling\nin particular, but that would mean a lot of mocking of SQLAlchemy.\n\n## Legal Information\n\nCopyright (c) 2021 Ed-Fi Alliance, LLC and contributors.\n\nLicensed under the [Apache License, Version\n2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the\n"License").\n\nUnless required by applicable law or agreed to in writing, software distributed\nunder the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR\nCONDITIONS OF ANY KIND, either express or implied. See the License for the\nspecific language governing permissions and limitations under the License.\n\nSee\n[NOTICES](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/NOTICES.md)\nfor additional copyright and license notifications.\n\n',
+    'long_description': '# edfi-sql-adapter\n\nLightweight wrapper to facilitate connections to SQL databases.\n\n## Developer Notes\n\nThis package is light on unit tests, because the functions are well tested from\nan integration perspective. Would be nice to add unit tests for error handling\nin particular, but that would mean a lot of mocking of SQLAlchemy.\n\n## Legal Information\n\nCopyright (c) 2022 Ed-Fi Alliance, LLC and contributors.\n\nLicensed under the [Apache License, Version\n2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the\n"License").\n\nUnless required by applicable law or agreed to in writing, software distributed\nunder the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR\nCONDITIONS OF ANY KIND, either express or implied. See the License for the\nspecific language governing permissions and limitations under the License.\n\nSee\n[NOTICES](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/NOTICES.md)\nfor additional copyright and license notifications.\n\n',
     'author': 'Ed-Fi Alliance, LLC, and contributors',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://techdocs.ed-fi.org/display/EDFITOOLS/LMS+Toolkit',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `edfi-sql-adapter-1.0.1a1/PKG-INFO` & `edfi_sql_adapter-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: edfi-sql-adapter
-Version: 1.0.1a1
+Version: 1.0.2
 Summary: Lightweight wrapper to facilitate connections to SQL databases
 Home-page: https://techdocs.ed-fi.org/display/EDFITOOLS/LMS+Toolkit
 License: Apache-2.0
 Author: Ed-Fi Alliance, LLC, and contributors
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: SQLAlchemy (==1.3.23)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: SQLAlchemy (>=1,<2)
 Requires-Dist: psycopg2 (>=2.8.6,<3.0.0)
 Requires-Dist: pyodbc (>=4.0.30,<5.0.0)
 Project-URL: Repository, https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit
 Description-Content-Type: text/markdown
 
 # edfi-sql-adapter
 
@@ -23,15 +25,15 @@
 
 This package is light on unit tests, because the functions are well tested from
 an integration perspective. Would be nice to add unit tests for error handling
 in particular, but that would mean a lot of mocking of SQLAlchemy.
 
 ## Legal Information
 
-Copyright (c) 2021 Ed-Fi Alliance, LLC and contributors.
+Copyright (c) 2022 Ed-Fi Alliance, LLC and contributors.
 
 Licensed under the [Apache License, Version
 2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the
 "License").
 
 Unless required by applicable law or agreed to in writing, software distributed
 under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
```

