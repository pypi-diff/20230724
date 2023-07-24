# Comparing `tmp/core_devoops-0.0.4.tar.gz` & `tmp/core_devoops-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_devoops-0.0.4.tar", max compression
+gzip compressed data, was "core_devoops-0.0.5.tar", max compression
```

## Comparing `core_devoops-0.0.4.tar` & `core_devoops-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      802 2023-07-24 06:38:44.034844 core_devoops-0.0.4/README.md
--rw-r--r--   0        0        0     1498 2023-07-24 07:39:26.323608 core_devoops-0.0.4/app/__init__.py
--rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.4/app/auth_configuration.py
--rw-r--r--   0        0        0     4604 2023-07-24 07:06:58.977898 core_devoops-0.0.4/app/authentification.py
--rw-r--r--   0        0        0     9288 2023-07-24 06:58:40.607210 core_devoops-0.0.4/app/check_dependencies.py
--rw-r--r--   0        0        0     1722 2023-07-24 09:10:21.682875 core_devoops-0.0.4/app/db_connection.py
--rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.4/app/list_utils.py
--rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.4/app/logger.py
--rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.4/app/pandas_utils.py
--rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.4/app/permissions.py
--rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.4/app/pydantic_utils.py
--rw-r--r--   0        0        0      995 2023-07-24 07:17:14.179994 core_devoops-0.0.4/app/read_write.py
--rw-r--r--   0        0        0      649 2023-07-24 07:03:21.934510 core_devoops-0.0.4/app/rights.py
--rw-r--r--   0        0        0     5545 2023-07-24 07:24:41.858537 core_devoops-0.0.4/app/safe_utils.py
--rw-r--r--   0        0        0      756 2023-07-24 07:03:21.938510 core_devoops-0.0.4/app/user.py
--rw-r--r--   0        0        0      592 2023-07-24 11:23:19.568331 core_devoops-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 core_devoops-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      802 2023-07-24 06:38:44.034844 core_devoops-0.0.5/README.md
+-rw-r--r--   0        0        0     1606 2023-07-24 11:50:30.489076 core_devoops-0.0.5/core_devoops/__init__.py
+-rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.5/core_devoops/auth_configuration.py
+-rw-r--r--   0        0        0     4649 2023-07-24 11:50:30.505077 core_devoops-0.0.5/core_devoops/authentification.py
+-rw-r--r--   0        0        0     9306 2023-07-24 11:50:30.497076 core_devoops-0.0.5/core_devoops/check_dependencies.py
+-rw-r--r--   0        0        0     1731 2023-07-24 11:50:30.517076 core_devoops-0.0.5/core_devoops/db_connection.py
+-rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.5/core_devoops/list_utils.py
+-rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.5/core_devoops/logger.py
+-rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.5/core_devoops/pandas_utils.py
+-rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.5/core_devoops/permissions.py
+-rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.5/core_devoops/pydantic_utils.py
+-rw-r--r--   0        0        0      995 2023-07-24 07:17:14.179994 core_devoops-0.0.5/core_devoops/read_write.py
+-rw-r--r--   0        0        0      658 2023-07-24 11:50:30.501077 core_devoops-0.0.5/core_devoops/rights.py
+-rw-r--r--   0        0        0     5563 2023-07-24 11:50:30.509076 core_devoops-0.0.5/core_devoops/safe_utils.py
+-rw-r--r--   0        0        0      774 2023-07-24 11:50:30.513076 core_devoops-0.0.5/core_devoops/user.py
+-rw-r--r--   0        0        0      601 2023-07-24 11:52:58.144429 core_devoops-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 core_devoops-0.0.5/PKG-INFO
```

### Comparing `core_devoops-0.0.4/README.md` & `core_devoops-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.4/app/auth_configuration.py` & `core_devoops-0.0.5/core_devoops/auth_configuration.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.4/app/authentification.py` & `core_devoops-0.0.5/core_devoops/authentification.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from typing import Dict
 from typing import List
 from typing import Union
 
-from app.user import User
-from app.logger import logger_get
-from app.db_connection import engine
+from core_devoops.user import User
+from core_devoops.logger import logger_get
+from core_devoops.db_connection import engine
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import status
 from fastapi.security import OAuth2PasswordBearer
 from jose import JWTError
 from jose import jwt
 from passlib.context import CryptContext
 from sqlmodel import Session
 from sqlmodel import col
 from sqlmodel import select
 
-from app.auth_configuration import AUTH
-from app.pydantic_utils import Frozen
+from core_devoops.auth_configuration import AUTH
+from core_devoops.pydantic_utils import Frozen
 
 
 SCHEME = OAuth2PasswordBearer(tokenUrl='login')
 auth_router = APIRouter(tags=['authentication'])
 CONTEXT = CryptContext(schemes=['bcrypt'], deprecated='auto')
 log = logger_get(__name__)
```

### Comparing `core_devoops-0.0.4/app/check_dependencies.py` & `core_devoops-0.0.5/core_devoops/check_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from subprocess import run
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Tuple
 from typing import Union
 
-from app.logger import logger_get
-from app.read_write import load_json_file
+from core_devoops.logger import logger_get
+from core_devoops.read_write import load_json_file
 
 CONF_FILE = 'dependencies.json'
 Dependency = Dict[str, List[str]]
 log = logger_get(__name__)
 
 
 def check_dependencies(conf_rel_path: str,
```

### Comparing `core_devoops-0.0.4/app/db_connection.py` & `core_devoops-0.0.5/core_devoops/db_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module implementing postgresql connection
 """
 from typing import Callable
 
-from app.logger import logger_get
+from core_devoops.logger import logger_get
 from pydantic import BaseSettings
 from sqlmodel import create_engine
 from sqlmodel import Session
 from sqlmodel import SQLModel
 from sqlalchemy import delete
 log = logger_get(__name__)
```

### Comparing `core_devoops-0.0.4/app/list_utils.py` & `core_devoops-0.0.5/core_devoops/list_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.4/app/logger.py` & `core_devoops-0.0.5/core_devoops/logger.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.4/app/pandas_utils.py` & `core_devoops-0.0.5/core_devoops/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.4/app/pydantic_utils.py` & `core_devoops-0.0.5/core_devoops/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.4/app/read_write.py` & `core_devoops-0.0.5/core_devoops/read_write.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.4/app/rights.py` & `core_devoops-0.0.5/core_devoops/rights.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from sqlmodel import Field
 from sqlmodel import Relationship
 from sqlmodel import SQLModel
 
 
 if TYPE_CHECKING:
-    from app.user import User
+    from core_devoops.user import User
 
 
 class Right(SQLModel, table=True):  # type: ignore
     """
     Simple right class: listing all app_services that a particular user can access to
     """
     id: Optional[int] = Field(default=None, primary_key=True)
```

### Comparing `core_devoops-0.0.4/app/safe_utils.py` & `core_devoops-0.0.5/core_devoops/safe_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Union
 from unittest import TestCase
 from pydantic import Field
 import numpy as np
-from app.logger import logger_get, log_critical
-from app.pydantic_utils import Frozen
+from core_devoops.logger import logger_get, log_critical
+from core_devoops.pydantic_utils import Frozen
 
 
 log = logger_get(__name__)
 
 
 class SafeTestCase(TestCase):
     """
```

### Comparing `core_devoops-0.0.4/app/user.py` & `core_devoops-0.0.5/core_devoops/user.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Module implementing the sqlmodel orm part of the user table
 """
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 
-from app.permissions import Permission
+from core_devoops.permissions import Permission
 
 from sqlmodel import Field
 from sqlmodel import Relationship
 from sqlmodel import SQLModel
 if TYPE_CHECKING:
-    from app.rights import Right
+    from core_devoops.rights import Right
 
 
 class User(SQLModel, table=True):  # type: ignore
     """
     Simple user class: an id associate to a user with a password
     """
     id: Optional[int] = Field(default=None, primary_key=True)
```

### Comparing `core_devoops-0.0.4/pyproject.toml` & `core_devoops-0.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "core-devoops"
-version = "0.0.4"
+version = "0.0.5"
 description = "Low level sqlmodel/fastapi/pydantic building blocks"
 authors = ["Thomas Epelbaum <tomepel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "app"}]
+packages = [{include = "core_devoops"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "~0"
 pandas = "~2"
 sqlmodel = "~0"
 numpy = "~1"
```

### Comparing `core_devoops-0.0.4/PKG-INFO` & `core_devoops-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-devoops
-Version: 0.0.4
+Version: 0.0.5
 Summary: Low level sqlmodel/fastapi/pydantic building blocks
 License: MIT
 Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: core-devoops Version: 0.0.4 Summary: Low level
+Metadata-Version: 2.1 Name: core-devoops Version: 0.0.5 Summary: Low level
 sqlmodel/fastapi/pydantic building blocks License: MIT Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fastapi (>=0,<1)
 Requires-Dist: numpy (>=1,<2) Requires-Dist: pandas (>=2,<3) Requires-Dist:
 passlib[bcyrypt] (>=1,<2) Requires-Dist: pydantic[python-dotenv] (>=1,<2)
```

