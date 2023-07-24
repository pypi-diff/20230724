# Comparing `tmp/edfi-lms-file-utils-1.0.1.tar.gz` & `tmp/edfi_lms_file_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edfi-lms-file-utils-1.0.1.tar", max compression
+gzip compressed data, was "edfi_lms_file_utils-1.0.2.tar", max compression
```

## Comparing `edfi-lms-file-utils-1.0.1.tar` & `edfi_lms_file_utils-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      269 2021-06-12 18:49:46.461975 edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/__init__.py
--rw-r--r--   0        0        0     1286 2021-06-12 18:49:46.461975 edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/constants.py
--rw-r--r--   0        0        0     5639 2021-06-12 18:49:46.462975 edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/directory_repository.py
--rw-r--r--   0        0        0    22626 2021-06-12 18:49:46.462975 edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/file_reader.py
--rw-r--r--   0        0        0     6581 2021-06-12 18:49:46.463975 edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/file_repository.py
--rw-r--r--   0        0        0        0 2021-06-12 18:49:46.463975 edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/py.typed
--rw-r--r--   0        0        0      864 2022-01-13 14:28:15.017126 edfi-lms-file-utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      296 2021-06-12 18:49:46.465975 edfi-lms-file-utils-1.0.1/readme.md
--rw-r--r--   0        0        0     1056 2022-01-13 14:28:22.239566 edfi-lms-file-utils-1.0.1/setup.py
--rw-r--r--   0        0        0     1000 2022-01-13 14:28:22.239566 edfi-lms-file-utils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      269 2021-06-12 18:49:46.461975 edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/__init__.py
+-rw-r--r--   0        0        0     1286 2021-06-12 18:49:46.461975 edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/constants.py
+-rw-r--r--   0        0        0     5639 2021-06-12 18:49:46.462975 edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/directory_repository.py
+-rw-r--r--   0        0        0    22626 2021-06-12 18:49:46.462975 edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/file_reader.py
+-rw-r--r--   0        0        0     6581 2021-06-12 18:49:46.463975 edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/file_repository.py
+-rw-r--r--   0        0        0        0 2021-06-12 18:49:46.463975 edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/py.typed
+-rw-r--r--   0        0        0      833 2023-07-24 20:31:52.587863 edfi_lms_file_utils-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      296 2021-06-12 18:49:46.465975 edfi_lms_file_utils-1.0.2/readme.md
+-rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 edfi_lms_file_utils-1.0.2/setup.py
+-rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 edfi_lms_file_utils-1.0.2/PKG-INFO
```

### Comparing `edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/constants.py` & `edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/constants.py`

 * *Files identical despite different names*

### Comparing `edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/directory_repository.py` & `edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/directory_repository.py`

 * *Files identical despite different names*

### Comparing `edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/file_reader.py` & `edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/file_reader.py`

 * *Files identical despite different names*

### Comparing `edfi-lms-file-utils-1.0.1/edfi_lms_file_utils/file_repository.py` & `edfi_lms_file_utils-1.0.2/edfi_lms_file_utils/file_repository.py`

 * *Files identical despite different names*

### Comparing `edfi-lms-file-utils-1.0.1/pyproject.toml` & `edfi_lms_file_utils-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-[tool.poetry]
-name = "edfi-lms-file-utils"
-version = "1.0.1"
-homepage = "https://techdocs.ed-fi.org/display/EDFITOOLS/LMS+Toolkit"
-repository = "https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit"
-description = "Utilities to facilitate use of the filesystem created by Ed-Fi LMS Extractors"
-readme = "readme.md"
-authors = ["Ed-Fi Alliance, LLC and contributors"]
-license = "Apache-2.0"
-include = ["edfi_lms_file_utils/py.typed"]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-numpy = "1.19.3"
-pandas = "^1.1.4"
-
-[tool.poetry.dev-dependencies]
-black = "^20.8b1"
-mypy = "^0.790"
-pytest = "6.2.3"
-flake8 = "^3.8.4"
-pyfakefs = "4.2.1"
-pytest-describe = "^1.0.0"
-coverage = "^5.3"
-pytest-mock = "^3.3.1"
-pylint = "^2.6.0"
-twine = "^3.3.0"
-freezegun = "^1.1.0"
-
-[build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+[tool.poetry]
+name = "edfi-lms-file-utils"
+version = "1.0.2"
+homepage = "https://techdocs.ed-fi.org/display/EDFITOOLS/LMS+Toolkit"
+repository = "https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit"
+description = "Utilities to facilitate use of the filesystem created by Ed-Fi LMS Extractors"
+readme = "readme.md"
+authors = ["Ed-Fi Alliance, LLC and contributors"]
+license = "Apache-2.0"
+include = ["edfi_lms_file_utils/py.typed"]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+numpy = "1.19.3"
+pandas = "^1.1.4"
+
+[tool.poetry.dev-dependencies]
+black = "^20.8b1"
+mypy = "^0.790"
+pytest = "6.2.3"
+flake8 = "^3.8.4"
+pyfakefs = "^4.5.0"
+pytest-describe = "^1.0.0"
+coverage = "^5.3"
+pytest-mock = "^3.3.1"
+pylint = "^2.6.0"
+twine = "^3.3.0"
+freezegun = "^1.1.0"
+
+[build-system]
+requires = ["poetry>=0.12"]
+build-backend = "poetry.masonry.api"
```

### Comparing `edfi-lms-file-utils-1.0.1/setup.py` & `edfi_lms_file_utils-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy==1.19.3', 'pandas>=1.1.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'edfi-lms-file-utils',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Utilities to facilitate use of the filesystem created by Ed-Fi LMS Extractors',
     'long_description': '# file-utils\n\nContains a set of functions to help work with the files generated by the LMS\nextractors. Does not contain any stand-alone scripts for execution.\n\nFor more information, and to see them in action, open the [filesystem-tutorial\nnotebook](../notebooks/filesystem-tutorial.ipynb)\n',
     'author': 'Ed-Fi Alliance, LLC and contributors',
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

### Comparing `edfi-lms-file-utils-1.0.1/PKG-INFO` & `edfi_lms_file_utils-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: edfi-lms-file-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities to facilitate use of the filesystem created by Ed-Fi LMS Extractors
 Home-page: https://techdocs.ed-fi.org/display/EDFITOOLS/LMS+Toolkit
 License: Apache-2.0
 Author: Ed-Fi Alliance, LLC and contributors
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (==1.19.3)
 Requires-Dist: pandas (>=1.1.4,<2.0.0)
 Project-URL: Repository, https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit
 Description-Content-Type: text/markdown
 
 # file-utils
```

