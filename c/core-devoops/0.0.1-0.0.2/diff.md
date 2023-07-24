# Comparing `tmp/core_devoops-0.0.1.tar.gz` & `tmp/core_devoops-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_devoops-0.0.1.tar", max compression
+gzip compressed data, was "core_devoops-0.0.2.tar", max compression
```

## Comparing `core_devoops-0.0.1.tar` & `core_devoops-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      802 2023-07-24 06:38:44.034844 core_devoops-0.0.1/README.md
--rw-r--r--   0        0        0     1498 2023-07-24 07:39:26.323608 core_devoops-0.0.1/app/__init__.py
--rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.1/app/auth_configuration.py
--rw-r--r--   0        0        0     4604 2023-07-24 07:06:58.977898 core_devoops-0.0.1/app/authentification.py
--rw-r--r--   0        0        0     9288 2023-07-24 06:58:40.607210 core_devoops-0.0.1/app/check_dependencies.py
--rw-r--r--   0        0        0     1722 2023-07-24 09:10:21.682875 core_devoops-0.0.1/app/db_connection.py
--rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.1/app/list_utils.py
--rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.1/app/logger.py
--rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.1/app/pandas_utils.py
--rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.1/app/permissions.py
--rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.1/app/pydantic_utils.py
--rw-r--r--   0        0        0      995 2023-07-24 07:17:14.179994 core_devoops-0.0.1/app/read_write.py
--rw-r--r--   0        0        0      649 2023-07-24 07:03:21.934510 core_devoops-0.0.1/app/rights.py
--rw-r--r--   0        0        0     5545 2023-07-24 07:24:41.858537 core_devoops-0.0.1/app/safe_utils.py
--rw-r--r--   0        0        0      756 2023-07-24 07:03:21.938510 core_devoops-0.0.1/app/user.py
--rw-r--r--   0        0        0      562 2023-07-24 09:55:46.618224 core_devoops-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 core_devoops-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      802 2023-07-24 06:38:44.034844 core_devoops-0.0.2/README.md
+-rw-r--r--   0        0        0     1498 2023-07-24 07:39:26.323608 core_devoops-0.0.2/app/__init__.py
+-rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.2/app/auth_configuration.py
+-rw-r--r--   0        0        0     4604 2023-07-24 07:06:58.977898 core_devoops-0.0.2/app/authentification.py
+-rw-r--r--   0        0        0     9288 2023-07-24 06:58:40.607210 core_devoops-0.0.2/app/check_dependencies.py
+-rw-r--r--   0        0        0     1722 2023-07-24 09:10:21.682875 core_devoops-0.0.2/app/db_connection.py
+-rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.2/app/list_utils.py
+-rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.2/app/logger.py
+-rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.2/app/pandas_utils.py
+-rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.2/app/permissions.py
+-rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.2/app/pydantic_utils.py
+-rw-r--r--   0        0        0      995 2023-07-24 07:17:14.179994 core_devoops-0.0.2/app/read_write.py
+-rw-r--r--   0        0        0      649 2023-07-24 07:03:21.934510 core_devoops-0.0.2/app/rights.py
+-rw-r--r--   0        0        0     5545 2023-07-24 07:24:41.858537 core_devoops-0.0.2/app/safe_utils.py
+-rw-r--r--   0        0        0      756 2023-07-24 07:03:21.938510 core_devoops-0.0.2/app/user.py
+-rw-r--r--   0        0        0      575 2023-07-24 10:03:34.796321 core_devoops-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 core_devoops-0.0.2/PKG-INFO
```

### Comparing `core_devoops-0.0.1/README.md` & `core_devoops-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/__init__.py` & `core_devoops-0.0.2/app/__init__.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/auth_configuration.py` & `core_devoops-0.0.2/app/auth_configuration.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/authentification.py` & `core_devoops-0.0.2/app/authentification.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/check_dependencies.py` & `core_devoops-0.0.2/app/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/db_connection.py` & `core_devoops-0.0.2/app/db_connection.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/list_utils.py` & `core_devoops-0.0.2/app/list_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/logger.py` & `core_devoops-0.0.2/app/logger.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/pandas_utils.py` & `core_devoops-0.0.2/app/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/pydantic_utils.py` & `core_devoops-0.0.2/app/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/read_write.py` & `core_devoops-0.0.2/app/read_write.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/rights.py` & `core_devoops-0.0.2/app/rights.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/safe_utils.py` & `core_devoops-0.0.2/app/safe_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/app/user.py` & `core_devoops-0.0.2/app/user.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.1/pyproject.toml` & `core_devoops-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "core-devoops"
-version = "0.0.1"
+version = "0.0.2"
 description = "Low level sqlmodel/fastapi/pydantic building blocks"
 authors = ["Thomas Epelbaum <tomepel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "app"}]
 
 [tool.poetry.dependencies]
@@ -16,12 +16,13 @@
 passlib = "~1"
 bcrypt = "~4"
 psycopg2 = "~2"
 pydantic = "~1"
 python-jose = "~1"
 python-dotenv = "~1"
 cryptography = "~41"
+numpy = "~1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `core_devoops-0.0.1/PKG-INFO` & `core_devoops-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: core-devoops
-Version: 0.0.1
+Version: 0.0.2
 Summary: Low level sqlmodel/fastapi/pydantic building blocks
 License: MIT
 Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4,<5)
 Requires-Dist: cryptography (>=41,<42)
 Requires-Dist: fastapi (>=0,<1)
+Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pandas (>=2,<3)
 Requires-Dist: passlib (>=1,<2)
 Requires-Dist: psycopg2 (>=2,<3)
 Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: python-dotenv (>=1,<2)
 Requires-Dist: python-jose (>=1,<2)
 Requires-Dist: python-multipart (>=0,<1)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: core-devoops Version: 0.0.1 Summary: Low level
+Metadata-Version: 2.1 Name: core-devoops Version: 0.0.2 Summary: Low level
 sqlmodel/fastapi/pydantic building blocks License: MIT Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: bcrypt (>=4,<5) Requires-
 Dist: cryptography (>=41,<42) Requires-Dist: fastapi (>=0,<1) Requires-Dist:
-pandas (>=2,<3) Requires-Dist: passlib (>=1,<2) Requires-Dist: psycopg2
-(>=2,<3) Requires-Dist: pydantic (>=1,<2) Requires-Dist: python-dotenv (>=1,<2)
-Requires-Dist: python-jose (>=1,<2) Requires-Dist: python-multipart (>=0,<1)
-Requires-Dist: sqlmodel (>=0,<1) Description-Content-Type: text/markdown #
-core_devoops
+numpy (>=1,<2) Requires-Dist: pandas (>=2,<3) Requires-Dist: passlib (>=1,<2)
+Requires-Dist: psycopg2 (>=2,<3) Requires-Dist: pydantic (>=1,<2) Requires-
+Dist: python-dotenv (>=1,<2) Requires-Dist: python-jose (>=1,<2) Requires-Dist:
+python-multipart (>=0,<1) Requires-Dist: sqlmodel (>=0,<1) Description-Content-
+Type: text/markdown # core_devoops
                     [Coverage] [Publish] [Package_version]
 Low level ecoact generic code. Aimed at being published in open source with
 poetry
```

