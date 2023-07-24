# Comparing `tmp/configcronos-0.0.4.tar.gz` & `tmp/configcronos-0.0.5.tar.gz`

## Comparing `configcronos-0.0.4.tar` & `configcronos-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configcronos-0.0.4/.env.example
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 configcronos-0.0.4/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 configcronos-0.0.4/requirements.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/client.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/database.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/oracle.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/phase1.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/phase2.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/pinger.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/schedule.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/segment.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/entities/sqls.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/errors/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/errors/no_connection.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/errors/no_data_found.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/client_repository.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/database_repository.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/phase1_repository.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/phase2_repository.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/pinger_repository.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/schedule_repository.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/segment_repository.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/repositories/sqls_repository.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/__init__.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/client.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/database.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/phase1.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/phase2.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/pinger.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/schedule.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/segment.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/core/usecases/sqls.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/__init__.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/api.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/configs/__init__.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/configs/configs.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/auth_repository.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/client_repository.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/database_repository.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/phase1_repository.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/phase2_repository.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/pinger_repository.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/schedule_repository.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/segment_repositoy.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/repositories/sqls_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configcronos-0.0.4/configcronos/infra/utils/__init__.py
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 configcronos-0.0.4/.gitignore
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 configcronos-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 configcronos-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configcronos-0.0.5/.env.example
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 configcronos-0.0.5/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 configcronos-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/client.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/database.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/oracle.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/phase1.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/phase2.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/pinger.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/schedule.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/segment.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/entities/sqls.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/errors/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/errors/no_connection.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/errors/no_data_found.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/client_repository.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/database_repository.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/phase1_repository.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/phase2_repository.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/pinger_repository.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/schedule_repository.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/segment_repository.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/repositories/sqls_repository.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/__init__.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/client.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/database.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/phase1.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/phase2.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/pinger.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/schedule.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/segment.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/core/usecases/sqls.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/__init__.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/api.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/configs/__init__.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/configs/configs.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/auth_repository.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/client_repository.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/database_repository.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/phase1_repository.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/phase2_repository.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/pinger_repository.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/schedule_repository.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/segment_repositoy.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/repositories/sqls_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configcronos-0.0.5/configcronos/infra/utils/__init__.py
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 configcronos-0.0.5/.gitignore
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 configcronos-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 configcronos-0.0.5/PKG-INFO
```

### Comparing `configcronos-0.0.4/README.md` & `configcronos-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/requirements.txt` & `configcronos-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/entities/client.py` & `configcronos-0.0.5/configcronos/core/entities/client.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/entities/phase1.py` & `configcronos-0.0.5/configcronos/core/entities/phase1.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/entities/phase2.py` & `configcronos-0.0.5/configcronos/core/entities/phase2.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/entities/schedule.py` & `configcronos-0.0.5/configcronos/core/entities/schedule.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/entities/segment.py` & `configcronos-0.0.5/configcronos/core/entities/segment.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/usecases/client.py` & `configcronos-0.0.5/configcronos/core/usecases/client.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/usecases/database.py` & `configcronos-0.0.5/configcronos/core/usecases/database.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/usecases/phase1.py` & `configcronos-0.0.5/configcronos/core/usecases/phase1.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/usecases/phase2.py` & `configcronos-0.0.5/configcronos/core/usecases/phase2.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/core/usecases/schedule.py` & `configcronos-0.0.5/configcronos/core/usecases/schedule.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/api.py` & `configcronos-0.0.5/configcronos/infra/api.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/configs/configs.py` & `configcronos-0.0.5/configcronos/infra/configs/configs.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/auth_repository.py` & `configcronos-0.0.5/configcronos/infra/repositories/auth_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/client_repository.py` & `configcronos-0.0.5/configcronos/infra/repositories/client_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/database_repository.py` & `configcronos-0.0.5/configcronos/infra/repositories/database_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/phase1_repository.py` & `configcronos-0.0.5/configcronos/infra/repositories/phase1_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/phase2_repository.py` & `configcronos-0.0.5/configcronos/infra/repositories/phase2_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/pinger_repository.py` & `configcronos-0.0.5/configcronos/infra/repositories/pinger_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/schedule_repository.py` & `configcronos-0.0.5/configcronos/infra/repositories/schedule_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/segment_repositoy.py` & `configcronos-0.0.5/configcronos/infra/repositories/segment_repositoy.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/configcronos/infra/repositories/sqls_repository.py` & `configcronos-0.0.5/configcronos/infra/repositories/sqls_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.4/.gitignore` & `configcronos-0.0.5/.gitignore`

 * *Files identical despite different names*

