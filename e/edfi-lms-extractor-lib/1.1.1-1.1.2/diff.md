# Comparing `tmp/edfi-lms-extractor-lib-1.1.1.tar.gz` & `tmp/edfi_lms_extractor_lib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edfi-lms-extractor-lib-1.1.1.tar", max compression
+gzip compressed data, was "edfi_lms_extractor_lib-1.1.2.tar", max compression
```

## Comparing `edfi-lms-extractor-lib-1.1.1.tar` & `edfi_lms_extractor_lib-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      269 2021-06-12 18:49:46.448974 edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/__init__.py
--rw-r--r--   0        0        0      269 2021-06-12 18:49:46.449974 edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/api/__init__.py
--rw-r--r--   0        0        0    14283 2021-09-27 18:39:06.217644 edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/api/resource_sync.py
--rw-r--r--   0        0        0      269 2021-06-12 18:49:46.450974 edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/csv_generation/__init__.py
--rw-r--r--   0        0        0    10076 2021-06-12 18:49:46.451974 edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/csv_generation/write.py
--rw-r--r--   0        0        0      269 2021-06-12 18:49:46.452974 edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/helpers/__init__.py
--rw-r--r--   0        0        0      709 2021-06-12 18:49:46.452974 edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/helpers/decorators.py
--rw-r--r--   0        0        0        0 2021-06-12 18:49:46.453975 edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/py.typed
--rw-r--r--   0        0        0      793 2022-01-13 14:32:02.930760 edfi-lms-extractor-lib-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      813 2021-06-12 18:49:46.447974 edfi-lms-extractor-lib-1.1.1/README.md
--rw-r--r--   0        0        0     1704 2022-01-13 14:32:07.517607 edfi-lms-extractor-lib-1.1.1/setup.py
--rw-r--r--   0        0        0     1538 2022-01-13 14:32:07.517607 edfi-lms-extractor-lib-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      269 2021-06-12 18:49:46.448974 edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/__init__.py
+-rw-r--r--   0        0        0      269 2021-06-12 18:49:46.449974 edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/api/__init__.py
+-rw-r--r--   0        0        0    14283 2021-09-27 18:39:06.217644 edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/api/resource_sync.py
+-rw-r--r--   0        0        0      269 2021-06-12 18:49:46.450974 edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/csv_generation/__init__.py
+-rw-r--r--   0        0        0    10076 2021-06-12 18:49:46.451974 edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/csv_generation/write.py
+-rw-r--r--   0        0        0      269 2021-06-12 18:49:46.452974 edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/helpers/__init__.py
+-rw-r--r--   0        0        0      709 2021-06-12 18:49:46.452974 edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/helpers/decorators.py
+-rw-r--r--   0        0        0        0 2021-06-12 18:49:46.453975 edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/py.typed
+-rw-r--r--   0        0        0      759 2023-07-24 19:22:03.716003 edfi_lms_extractor_lib-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      792 2022-02-01 20:58:34.075894 edfi_lms_extractor_lib-1.1.2/README.md
+-rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 edfi_lms_extractor_lib-1.1.2/setup.py
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 edfi_lms_extractor_lib-1.1.2/PKG-INFO
```

### Comparing `edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/api/resource_sync.py` & `edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/api/resource_sync.py`

 * *Files identical despite different names*

### Comparing `edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/csv_generation/write.py` & `edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/csv_generation/write.py`

 * *Files identical despite different names*

### Comparing `edfi-lms-extractor-lib-1.1.1/edfi_lms_extractor_lib/helpers/decorators.py` & `edfi_lms_extractor_lib-1.1.2/edfi_lms_extractor_lib/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `edfi-lms-extractor-lib-1.1.1/README.md` & `edfi_lms_extractor_lib-1.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Extractor Shared Library
-
-Shared library for use in the [Ed-Fi LMS
-Toolkit](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit).
-
-## Legal Information
-
-Copyright (c) 2021 Ed-Fi Alliance, LLC and contributors.
-
-Licensed under the [Apache License, Version
-2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the
-"License").
-
-Unless required by applicable law or agreed to in writing, software distributed
-under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-CONDITIONS OF ANY KIND, either express or implied. See the License for the
-specific language governing permissions and limitations under the License.
-
-See
-[NOTICES](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/NOTICES.md)
-for additional copyright and license notifications.
+# Extractor Shared Library
+
+Shared library for use in the [Ed-Fi LMS
+Toolkit](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit).
+
+## Legal Information
+
+Copyright (c) 2022 Ed-Fi Alliance, LLC and contributors.
+
+Licensed under the [Apache License, Version
+2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the
+"License").
+
+Unless required by applicable law or agreed to in writing, software distributed
+under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
+CONDITIONS OF ANY KIND, either express or implied. See the License for the
+specific language governing permissions and limitations under the License.
+
+See
+[NOTICES](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/NOTICES.md)
+for additional copyright and license notifications.
```

### Comparing `edfi-lms-extractor-lib-1.1.1/setup.py` & `edfi_lms_extractor_lib-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,25 @@
  'edfi_lms_extractor_lib.csv_generation',
  'edfi_lms_extractor_lib.helpers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['SQLAlchemy>=1.3.19,<2.0.0', 'pandas>=1.1.1,<2.0.0', 'xxhash>=2.0.0,<3.0.0']
+['SQLAlchemy>=1,<2', 'pandas>=1.1.1,<2.0.0', 'xxhash>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'edfi-lms-extractor-lib',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'Shared functions library for Ed-Fi LMS Extractor projects',
-    'long_description': '# Extractor Shared Library\n\nShared library for use in the [Ed-Fi LMS\nToolkit](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit).\n\n## Legal Information\n\nCopyright (c) 2021 Ed-Fi Alliance, LLC and contributors.\n\nLicensed under the [Apache License, Version\n2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the\n"License").\n\nUnless required by applicable law or agreed to in writing, software distributed\nunder the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR\nCONDITIONS OF ANY KIND, either express or implied. See the License for the\nspecific language governing permissions and limitations under the License.\n\nSee\n[NOTICES](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/NOTICES.md)\nfor additional copyright and license notifications.\n',
+    'long_description': '# Extractor Shared Library\n\nShared library for use in the [Ed-Fi LMS\nToolkit](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit).\n\n## Legal Information\n\nCopyright (c) 2022 Ed-Fi Alliance, LLC and contributors.\n\nLicensed under the [Apache License, Version\n2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the\n"License").\n\nUnless required by applicable law or agreed to in writing, software distributed\nunder the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR\nCONDITIONS OF ANY KIND, either express or implied. See the License for the\nspecific language governing permissions and limitations under the License.\n\nSee\n[NOTICES](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/NOTICES.md)\nfor additional copyright and license notifications.\n',
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

### Comparing `edfi-lms-extractor-lib-1.1.1/PKG-INFO` & `edfi_lms_extractor_lib-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: edfi-lms-extractor-lib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Shared functions library for Ed-Fi LMS Extractor projects
 Home-page: https://techdocs.ed-fi.org/display/EDFITOOLS/LMS+Toolkit
 License: Apache-2.0
 Author: Ed-Fi Alliance, LLC, and contributors
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: SQLAlchemy (>=1.3.19,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: SQLAlchemy (>=1,<2)
 Requires-Dist: pandas (>=1.1.1,<2.0.0)
 Requires-Dist: xxhash (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit
 Description-Content-Type: text/markdown
 
 # Extractor Shared Library
 
 Shared library for use in the [Ed-Fi LMS
 Toolkit](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit).
 
 ## Legal Information
 
-Copyright (c) 2021 Ed-Fi Alliance, LLC and contributors.
+Copyright (c) 2022 Ed-Fi Alliance, LLC and contributors.
 
 Licensed under the [Apache License, Version
 2.0](https://github.com/Ed-Fi-Exchange-OSS/LMS-Toolkit/blob/main/LICENSE) (the
 "License").
 
 Unless required by applicable law or agreed to in writing, software distributed
 under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
```

