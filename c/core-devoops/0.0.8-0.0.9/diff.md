# Comparing `tmp/core_devoops-0.0.8.tar.gz` & `tmp/core_devoops-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_devoops-0.0.8.tar", max compression
+gzip compressed data, was "core_devoops-0.0.9.tar", max compression
```

## Comparing `core_devoops-0.0.8.tar` & `core_devoops-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      801 2023-07-24 13:06:11.371573 core_devoops-0.0.8/README.md
--rw-r--r--   0        0        0     2545 2023-07-24 13:44:06.133763 core_devoops-0.0.8/core_devoops/__init__.py
--rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.8/core_devoops/auth_configuration.py
--rw-r--r--   0        0        0     4648 2023-07-24 13:06:12.011570 core_devoops-0.0.8/core_devoops/authentification.py
--rw-r--r--   0        0        0     9306 2023-07-24 11:50:30.497076 core_devoops-0.0.8/core_devoops/check_dependencies.py
--rw-r--r--   0        0        0     1733 2023-07-24 13:06:11.999570 core_devoops-0.0.8/core_devoops/db_connection.py
--rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.8/core_devoops/list_utils.py
--rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.8/core_devoops/logger.py
--rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.8/core_devoops/pandas_utils.py
--rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.8/core_devoops/permissions.py
--rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.8/core_devoops/pydantic_utils.py
--rw-r--r--   0        0        0      996 2023-07-24 13:06:11.219573 core_devoops-0.0.8/core_devoops/read_write.py
--rw-r--r--   0        0        0      658 2023-07-24 11:50:30.501077 core_devoops-0.0.8/core_devoops/rights.py
--rw-r--r--   0        0        0     5599 2023-07-24 13:06:11.999570 core_devoops-0.0.8/core_devoops/safe_utils.py
--rw-r--r--   0        0        0      774 2023-07-24 13:06:12.003570 core_devoops-0.0.8/core_devoops/user.py
--rw-r--r--   0        0        0     1767 2023-07-24 13:44:49.889615 core_devoops-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 core_devoops-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      801 2023-07-24 13:06:11.371573 core_devoops-0.0.9/README.md
+-rw-r--r--   0        0        0     2678 2023-07-24 13:55:42.579425 core_devoops-0.0.9/core_devoops/__init__.py
+-rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.9/core_devoops/auth_configuration.py
+-rw-r--r--   0        0        0     4648 2023-07-24 13:06:12.011570 core_devoops-0.0.9/core_devoops/authentification.py
+-rw-r--r--   0        0        0     9306 2023-07-24 11:50:30.497076 core_devoops-0.0.9/core_devoops/check_dependencies.py
+-rw-r--r--   0        0        0     1733 2023-07-24 13:06:11.999570 core_devoops-0.0.9/core_devoops/db_connection.py
+-rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.9/core_devoops/list_utils.py
+-rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.9/core_devoops/logger.py
+-rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.9/core_devoops/pandas_utils.py
+-rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.9/core_devoops/permissions.py
+-rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.9/core_devoops/pydantic_utils.py
+-rw-r--r--   0        0        0      996 2023-07-24 13:06:11.219573 core_devoops-0.0.9/core_devoops/read_write.py
+-rw-r--r--   0        0        0      658 2023-07-24 11:50:30.501077 core_devoops-0.0.9/core_devoops/rights.py
+-rw-r--r--   0        0        0     5599 2023-07-24 13:06:11.999570 core_devoops-0.0.9/core_devoops/safe_utils.py
+-rw-r--r--   0        0        0      774 2023-07-24 13:06:12.003570 core_devoops-0.0.9/core_devoops/user.py
+-rw-r--r--   0        0        0     1767 2023-07-24 13:56:06.707344 core_devoops-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 core_devoops-0.0.9/PKG-INFO
```

### Comparing `core_devoops-0.0.8/README.md` & `core_devoops-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/__init__.py` & `core_devoops-0.0.9/core_devoops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from core_devoops.authentification import attempt_to_log
 from core_devoops.authentification import get_app_services
 from core_devoops.authentification import get_current_user
 from core_devoops.authentification import is_admin_user
 from core_devoops.authentification import SCHEME
 from core_devoops.authentification import Token
 from core_devoops.check_dependencies import compute_dependencies
-from core_devoops.db_connection import create_db_and_tables, DB_URL
+from core_devoops.db_connection import create_db_and_tables
+from core_devoops.db_connection import DB_URL
 from core_devoops.db_connection import delete_table
 from core_devoops.db_connection import engine
 from core_devoops.db_connection import get_session
 from core_devoops.db_connection import info_message
 from core_devoops.list_utils import first_or_default
 from core_devoops.list_utils import first_transformed_or_default
 from core_devoops.list_utils import group_by_value
 from core_devoops.list_utils import lselect
 from core_devoops.list_utils import lselectfirst
 from core_devoops.logger import log_critical
 from core_devoops.logger import logger_get
+from core_devoops.pandas_utils import pd_equals, jsonify_series
 from core_devoops.permissions import Permission
 from core_devoops.pydantic_utils import Basic
 from core_devoops.pydantic_utils import CustomFrozen
 from core_devoops.pydantic_utils import Frozen
 from core_devoops.pydantic_utils import OrmFrozen
 from core_devoops.read_write import load_json_file
 from core_devoops.read_write import make_dir
@@ -43,9 +45,9 @@
 __all__ = [
     'AUTH', 'Token', 'get_app_services', 'attempt_to_log', 'get_current_user', 'is_admin_user',
     'write_json_file', 'load_json_file', 'make_dir', 'check_dependencies', 'compute_dependencies',
     'engine', 'create_db_and_tables', 'get_session', 'info_message', 'group_by_value',
     'first_or_default', 'lselect', 'lselectfirst', 'first_transformed_or_default', 'log_critical',
     'logger_get', 'Permission', 'User', 'Right', 'Basic', 'Frozen', 'CustomFrozen', 'OrmFrozen',
     'SafeTestCase', 'SimpleReturn', 'safe_clt', 'stringify', 'boolify', 'intify', 'floatify',
-    'delete_table', 'SCHEME', 'DB_URL'
+    'delete_table', 'SCHEME', 'DB_URL', 'pd_equals', 'jsonify_series'
 ]
```

### Comparing `core_devoops-0.0.8/core_devoops/auth_configuration.py` & `core_devoops-0.0.9/core_devoops/auth_configuration.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/authentification.py` & `core_devoops-0.0.9/core_devoops/authentification.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/check_dependencies.py` & `core_devoops-0.0.9/core_devoops/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/db_connection.py` & `core_devoops-0.0.9/core_devoops/db_connection.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/list_utils.py` & `core_devoops-0.0.9/core_devoops/list_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/logger.py` & `core_devoops-0.0.9/core_devoops/logger.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/pandas_utils.py` & `core_devoops-0.0.9/core_devoops/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/pydantic_utils.py` & `core_devoops-0.0.9/core_devoops/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/read_write.py` & `core_devoops-0.0.9/core_devoops/read_write.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/rights.py` & `core_devoops-0.0.9/core_devoops/rights.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/safe_utils.py` & `core_devoops-0.0.9/core_devoops/safe_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/core_devoops/user.py` & `core_devoops-0.0.9/core_devoops/user.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.8/pyproject.toml` & `core_devoops-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "core-devoops"
-version = "0.0.8"
+version = "0.0.9"
 description = "Low level sqlmodel/fastapi/pydantic building blocks"
 authors = ["Thomas Epelbaum <tomepel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
```

### Comparing `core_devoops-0.0.8/PKG-INFO` & `core_devoops-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-devoops
-Version: 0.0.8
+Version: 0.0.9
 Summary: Low level sqlmodel/fastapi/pydantic building blocks
 License: MIT
 Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: core-devoops Version: 0.0.8 Summary: Low level
+Metadata-Version: 2.1 Name: core-devoops Version: 0.0.9 Summary: Low level
 sqlmodel/fastapi/pydantic building blocks License: MIT Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO Classifier: Framework :: FastAPI Classifier:
 Framework :: Pydantic Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: System Administrators
```

