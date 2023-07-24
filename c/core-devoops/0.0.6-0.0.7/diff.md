# Comparing `tmp/core_devoops-0.0.6.tar.gz` & `tmp/core_devoops-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_devoops-0.0.6.tar", max compression
+gzip compressed data, was "core_devoops-0.0.7.tar", max compression
```

## Comparing `core_devoops-0.0.6.tar` & `core_devoops-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      802 2023-07-24 06:38:44.034844 core_devoops-0.0.6/README.md
--rw-r--r--   0        0        0     1606 2023-07-24 11:50:30.489076 core_devoops-0.0.6/core_devoops/__init__.py
--rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.6/core_devoops/auth_configuration.py
--rw-r--r--   0        0        0     4649 2023-07-24 11:50:30.505077 core_devoops-0.0.6/core_devoops/authentification.py
--rw-r--r--   0        0        0     9306 2023-07-24 11:50:30.497076 core_devoops-0.0.6/core_devoops/check_dependencies.py
--rw-r--r--   0        0        0     1731 2023-07-24 11:50:30.517076 core_devoops-0.0.6/core_devoops/db_connection.py
--rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.6/core_devoops/list_utils.py
--rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.6/core_devoops/logger.py
--rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.6/core_devoops/pandas_utils.py
--rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.6/core_devoops/permissions.py
--rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.6/core_devoops/pydantic_utils.py
--rw-r--r--   0        0        0      995 2023-07-24 07:17:14.179994 core_devoops-0.0.6/core_devoops/read_write.py
--rw-r--r--   0        0        0      658 2023-07-24 11:50:30.501077 core_devoops-0.0.6/core_devoops/rights.py
--rw-r--r--   0        0        0     5563 2023-07-24 11:50:30.509076 core_devoops-0.0.6/core_devoops/safe_utils.py
--rw-r--r--   0        0        0      774 2023-07-24 11:50:30.513076 core_devoops-0.0.6/core_devoops/user.py
--rw-r--r--   0        0        0     1767 2023-07-24 12:54:31.486305 core_devoops-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 core_devoops-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      801 2023-07-24 13:06:11.371573 core_devoops-0.0.7/README.md
+-rw-r--r--   0        0        0     2486 2023-07-24 13:15:13.374761 core_devoops-0.0.7/core_devoops/__init__.py
+-rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.7/core_devoops/auth_configuration.py
+-rw-r--r--   0        0        0     4648 2023-07-24 13:06:12.011570 core_devoops-0.0.7/core_devoops/authentification.py
+-rw-r--r--   0        0        0     9306 2023-07-24 11:50:30.497076 core_devoops-0.0.7/core_devoops/check_dependencies.py
+-rw-r--r--   0        0        0     1733 2023-07-24 13:06:11.999570 core_devoops-0.0.7/core_devoops/db_connection.py
+-rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.7/core_devoops/list_utils.py
+-rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.7/core_devoops/logger.py
+-rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.7/core_devoops/pandas_utils.py
+-rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.7/core_devoops/permissions.py
+-rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.7/core_devoops/pydantic_utils.py
+-rw-r--r--   0        0        0      996 2023-07-24 13:06:11.219573 core_devoops-0.0.7/core_devoops/read_write.py
+-rw-r--r--   0        0        0      658 2023-07-24 11:50:30.501077 core_devoops-0.0.7/core_devoops/rights.py
+-rw-r--r--   0        0        0     5599 2023-07-24 13:06:11.999570 core_devoops-0.0.7/core_devoops/safe_utils.py
+-rw-r--r--   0        0        0      774 2023-07-24 13:06:12.003570 core_devoops-0.0.7/core_devoops/user.py
+-rw-r--r--   0        0        0     1767 2023-07-24 13:15:13.366761 core_devoops-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 core_devoops-0.0.7/PKG-INFO
```

### Comparing `core_devoops-0.0.6/README.md` & `core_devoops-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
     <img src="https://github.com/FR-PAR-ECOACT/core_devoops/blob/main/badges/pylint.svg" alt="Publish">
 </a>
 <a href="https://github.com/FR-PAR-ECOACT/core_devoops/actions/workflows/code-quality.yml/badge.svg" target="_blank">
     <img src="https://github.com/FR-PAR-ECOACT/core_devoops/actions/workflows/code-quality.yml/badge.svg" alt="Package version">
 </a>
 </p>
 
-Low level ecoact generic code. Aimed at being published in open source with poetry 
+Low level ecoact generic code. Aimed at being published in open source with poetry
```

### Comparing `core_devoops-0.0.6/core_devoops/auth_configuration.py` & `core_devoops-0.0.7/core_devoops/auth_configuration.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.6/core_devoops/authentification.py` & `core_devoops-0.0.7/core_devoops/authentification.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from typing import Dict
 from typing import List
 from typing import Union
 
-from core_devoops.user import User
-from core_devoops.logger import logger_get
-from core_devoops.db_connection import engine
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import status
 from fastapi.security import OAuth2PasswordBearer
-from jose import JWTError
 from jose import jwt
+from jose import JWTError
 from passlib.context import CryptContext
-from sqlmodel import Session
 from sqlmodel import col
 from sqlmodel import select
+from sqlmodel import Session
 
 from core_devoops.auth_configuration import AUTH
+from core_devoops.db_connection import engine
+from core_devoops.logger import logger_get
 from core_devoops.pydantic_utils import Frozen
+from core_devoops.user import User
 
 
 SCHEME = OAuth2PasswordBearer(tokenUrl='login')
 auth_router = APIRouter(tags=['authentication'])
 CONTEXT = CryptContext(schemes=['bcrypt'], deprecated='auto')
 log = logger_get(__name__)
 
@@ -48,15 +48,15 @@
     id: int
 
 
 def get_app_services(user: User, session: Session) -> List[str]:
     """
     Retrieve all app services the passed user has access to
     """
-    if db_user :=  session.exec(select(User).where(col(User.id) == user.id)).first():
+    if db_user := session.exec(select(User).where(col(User.id) == user.id)).first():
         return [right.app_service for right in db_user.rights]
     return []
 
 
 def attempt_to_log(user: str,
                    password: str,
                    session: Session):
```

### Comparing `core_devoops-0.0.6/core_devoops/check_dependencies.py` & `core_devoops-0.0.7/core_devoops/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.6/core_devoops/db_connection.py` & `core_devoops-0.0.7/core_devoops/db_connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Module implementing postgresql connection
 """
 from typing import Callable
 
-from core_devoops.logger import logger_get
 from pydantic import BaseSettings
+from sqlalchemy import delete
 from sqlmodel import create_engine
 from sqlmodel import Session
 from sqlmodel import SQLModel
-from sqlalchemy import delete
+
+from core_devoops.logger import logger_get
 log = logger_get(__name__)
 
 
 class DbSettings(BaseSettings):
     """
     Settings class used to connect to the postgresql database
     """
@@ -37,14 +38,15 @@
 def create_db_and_tables(model: Callable) -> None:
     """
     Create all tables based on the declared schemas in core/models thanks to sqlmodel
     """
     log.info(f'Inserting on the fly {model} and all other domain tables')
     SQLModel.metadata.create_all(engine)
 
+
 def delete_table(model: Callable) -> None:
     """
     Delete all rows of the passed model from db
     """
     with Session(engine) as session:
         result = session.execute(delete(model))
         session.commit()
```

### Comparing `core_devoops-0.0.6/core_devoops/list_utils.py` & `core_devoops-0.0.7/core_devoops/list_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.6/core_devoops/logger.py` & `core_devoops-0.0.7/core_devoops/logger.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.6/core_devoops/pandas_utils.py` & `core_devoops-0.0.7/core_devoops/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.6/core_devoops/pydantic_utils.py` & `core_devoops-0.0.7/core_devoops/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.6/core_devoops/read_write.py` & `core_devoops-0.0.7/core_devoops/read_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Load a json file at file_path location
     """
     with open(file_path, 'r', encoding='utf-8') as f:
         loaded_json = json.load(f)
 
     return loaded_json
 
+
 def make_dir(directory: Path):
     """
     Helper that create the directory "directory" if it doesn't exist yet
     """
     try:
         os.umask(0)
         os.makedirs(directory)
```

### Comparing `core_devoops-0.0.6/core_devoops/rights.py` & `core_devoops-0.0.7/core_devoops/rights.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.6/core_devoops/safe_utils.py` & `core_devoops-0.0.7/core_devoops/safe_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 import shutil
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Union
 from unittest import TestCase
-from pydantic import Field
+
 import numpy as np
-from core_devoops.logger import logger_get, log_critical
+from pydantic import Field
+
+from core_devoops.logger import log_critical
+from core_devoops.logger import logger_get
 from core_devoops.pydantic_utils import Frozen
 
 
 log = logger_get(__name__)
 
 
 class SafeTestCase(TestCase):
@@ -98,14 +101,15 @@
             except exception:
                 self.tearDown()
                 self.doCleanups()
                 raise
 
         return _wrapped
 
+
 class SimpleReturn(Frozen):
     """
     Simple output for routes not returning anything
     """
     success: bool = Field(..., description=' True if the treatment went well.')
     error: Union[str, None] = Field(..., description='the error that happened, if any.')
 
@@ -119,27 +123,29 @@
     @classmethod
     def route_failure(cls, error: str) -> 'SimpleReturn':
         """
         Format DropDocumentReturn if the document failed to be dropped
         """
         return SimpleReturn(success=False, error=error)
 
+
 def safe_clt(func):
     """
     Safe execution of typer commands
     """
     def inner_function(*args, **kwargs):
         try:
             func(*args, **kwargs)
             return SimpleReturn.route_success()
         except Exception as error:
             log_critical(f'something wrong happened: {error}', log)
             return SimpleReturn.route_failure(str(error))
     return inner_function
 
+
 def stringify(x: Union[str, float]) -> Union[str, None]:
     """
     Safe conversion of a (str, np.nan) value into a (str,None) one
     """
     return _transformify(x, str)
```

### Comparing `core_devoops-0.0.6/core_devoops/user.py` & `core_devoops-0.0.7/core_devoops/user.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Module implementing the sqlmodel orm part of the user table
 """
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 
-from core_devoops.permissions import Permission
-
 from sqlmodel import Field
 from sqlmodel import Relationship
 from sqlmodel import SQLModel
+
+from core_devoops.permissions import Permission
 if TYPE_CHECKING:
     from core_devoops.rights import Right
 
 
 class User(SQLModel, table=True):  # type: ignore
     """
     Simple user class: an id associate to a user with a password
```

### Comparing `core_devoops-0.0.6/pyproject.toml` & `core_devoops-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "core-devoops"
-version = "0.0.6"
+version = "0.0.7"
 description = "Low level sqlmodel/fastapi/pydantic building blocks"
 authors = ["Thomas Epelbaum <tomepel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
```

### Comparing `core_devoops-0.0.6/PKG-INFO` & `core_devoops-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-devoops
-Version: 0.0.6
+Version: 0.0.7
 Summary: Low level sqlmodel/fastapi/pydantic building blocks
 License: MIT
 Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
@@ -51,9 +51,9 @@
     <img src="https://github.com/FR-PAR-ECOACT/core_devoops/blob/main/badges/pylint.svg" alt="Publish">
 </a>
 <a href="https://github.com/FR-PAR-ECOACT/core_devoops/actions/workflows/code-quality.yml/badge.svg" target="_blank">
     <img src="https://github.com/FR-PAR-ECOACT/core_devoops/actions/workflows/code-quality.yml/badge.svg" alt="Package version">
 </a>
 </p>
 
-Low level ecoact generic code. Aimed at being published in open source with poetry 
+Low level ecoact generic code. Aimed at being published in open source with poetry
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: core-devoops Version: 0.0.6 Summary: Low level
+Metadata-Version: 2.1 Name: core-devoops Version: 0.0.7 Summary: Low level
 sqlmodel/fastapi/pydantic building blocks License: MIT Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO Classifier: Framework :: FastAPI Classifier:
 Framework :: Pydantic Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: System Administrators
```

