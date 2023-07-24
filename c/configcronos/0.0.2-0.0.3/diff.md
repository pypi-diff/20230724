# Comparing `tmp/configcronos-0.0.2.tar.gz` & `tmp/configcronos-0.0.3.tar.gz`

## Comparing `configcronos-0.0.2.tar` & `configcronos-0.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configcronos-0.0.2/.env.example
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 configcronos-0.0.2/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 configcronos-0.0.2/requirements.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/client.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/database.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/oracle.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/phase1.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/phase2.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/pinger.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/schedule.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/segment.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/entities/sqls.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/errors/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/errors/no_connection.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/errors/no_data_found.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/client_repository.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/database_repository.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/phase1_repository.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/phase2_repository.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/pinger_repository.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/schedule_repository.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/segment_repository.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/repositories/sqls_repository.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/__init__.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/client.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/database.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/phase1.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/phase2.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/pinger.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/schedule.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/segment.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/core/usecases/sqls.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/__init__.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/api.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/configs/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/configs/configs.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/auth_repository.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/client_repository.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/database_repository.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/phase1_repository.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/phase2_repository.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/pinger_repository.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/schedule_repository.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/segment_repositoy.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/repositories/sqls_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configcronos-0.0.2/configcronos/infra/utils/__init__.py
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 configcronos-0.0.2/.gitignore
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 configcronos-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 configcronos-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configcronos-0.0.3/.env.example
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 configcronos-0.0.3/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 configcronos-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/client.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/database.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/oracle.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/phase1.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/phase2.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/pinger.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/schedule.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/segment.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/entities/sqls.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/errors/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/errors/no_connection.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/errors/no_data_found.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/client_repository.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/database_repository.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/phase1_repository.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/phase2_repository.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/pinger_repository.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/schedule_repository.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/segment_repository.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/repositories/sqls_repository.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/__init__.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/client.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/database.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/phase1.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/phase2.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/pinger.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/schedule.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/segment.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/core/usecases/sqls.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/__init__.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/api.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/configs/__init__.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/configs/configs.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/auth_repository.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/client_repository.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/database_repository.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/phase1_repository.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/phase2_repository.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/pinger_repository.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/schedule_repository.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/segment_repositoy.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/repositories/sqls_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configcronos-0.0.3/configcronos/infra/utils/__init__.py
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 configcronos-0.0.3/.gitignore
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 configcronos-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 configcronos-0.0.3/PKG-INFO
```

### Comparing `configcronos-0.0.2/README.md` & `configcronos-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/requirements.txt` & `configcronos-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/entities/client.py` & `configcronos-0.0.3/configcronos/core/entities/client.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/entities/phase1.py` & `configcronos-0.0.3/configcronos/core/entities/phase1.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/entities/phase2.py` & `configcronos-0.0.3/configcronos/core/entities/phase2.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/entities/schedule.py` & `configcronos-0.0.3/configcronos/core/entities/schedule.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/entities/segment.py` & `configcronos-0.0.3/configcronos/core/entities/segment.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/usecases/client.py` & `configcronos-0.0.3/configcronos/core/usecases/client.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/usecases/database.py` & `configcronos-0.0.3/configcronos/core/usecases/database.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/usecases/phase1.py` & `configcronos-0.0.3/configcronos/core/usecases/phase1.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/usecases/phase2.py` & `configcronos-0.0.3/configcronos/core/usecases/phase2.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/core/usecases/schedule.py` & `configcronos-0.0.3/configcronos/core/usecases/schedule.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/api.py` & `configcronos-0.0.3/configcronos/infra/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,9 @@
 def update_schedule(schedule_) -> bool:
     return ScheduleService(ScheduleRepositoryAPI(headers())).update_schedule(schedule_)
 
 
 if __name__  == '__main__':
     #authenticate("eyJhbGciOiJSUzI1NiIsImtpZCI6IjE2NjcyNDg1MTAtMTZiNzljZTQtNDM1YS00YzA2LTkxZDItZjBjNjk5MzEyNjNkIiwidHlwIjoiSldUIn0.eyJzdWIiOiIxNTkiLCJwcmVmZXJyZWRfdXNlcm5hbWUiOiJkYXZpX3NtYXJrZXQiLCJlbWFpbCI6ImRhdmlAc21hcmtldHNvbHV0aW9ucy5jb20uYnIiLCJjbGllbnRfaWQiOiJvbmJvYXJkaW5nIiwic3RvcmVzIjpbIjEiLCIxMCIsIjIiLCIyMDEiLCIyMDMiLCIyMiIsIjMiLCIzMDEiLCI0IiwiNSIsIjYiLCI3IiwiOCIsIjkiLCI5MDEiXSwicm9sZXMiOlsiYXByb3ZhY2FvIiwicmVsYXRvcmlvcyIsImRpYWdyYW1hZG9yIiwiZWRpdGFyX21hcGFzIiwibGlzdGFyX2Fjb2VzIiwibGlzdGFyX21hcGFzIiwiY29uZmlndXJhY29lcyIsImVkaXRhcl9jYXJ0YXoiLCJjYW5jZWxhcl9vZmVydGEiLCJkdXBsaWNhcl9vZmVydGEiLCJnZXJlbmNpYXJfYWNvZXMiLCJnZXJlbmNpYXJfYXJlYXMiLCJiYW5jb19kZV9pbWFnZW5zIiwiY3JpYXJfYXRpdmlkYWRlcyIsImVkaXRhcl9kZXNjcmljYW8iLCJnZXJlbmNpYXJfdG9rZW5zIiwibGlzdGFyX2NhbXBhbmhhcyIsInZlcl9sb2dzX29mZXJ0YXMiLCJnZXJlbmNpYXJfb2ZlcnRhcyIsInBlcmZpbF9wZXJtaXNzb2VzIiwiYXVkaXRhcl9hdGl2aWRhZGVzIiwiY3JpYXJfZWRpdGFyX2NpY2xvIiwiZWRpdGFyX3RleHRvX2xlZ2FsIiwiZ2VyZW5jaWFyX2NhcnRhemVzIiwiZ2VyZW5jaWFyX3VzdWFyaW9zIiwiZ2VyZW5jaWFyX2NhbXBhbmhhcyIsImdlcmVuY2lhcl9jb250cmF0b3MiLCJnZXJlbmNpYXJfZXRpcXVldGFzIiwiYWx0ZXJhcl9wcm9kdXRvX2FjYW8iLCJhbHRlcmFyX3Jlc3BvbnNhdmVpcyIsImdlcmVuY2lhcl90aXBvX2RlX2FyZWEiLCJlZGl0YXJfZGVzY3JpY2FvX2NhcnRheiIsImdlcmVuY2lhcl9wYXN0YXNfY2FydGF6Iiwic21hcmtldGZ5X2F0aXZvX3VzdWFyaW8iLCJhcHJvdmFyX29mZXJ0YXNfaW50ZXJuYXMiLCJ2aXN1YWxpemFyX2NpY2xvc19hdGVfZmltIiwiZ2VyZW5jaWFyX3Bhc3Rhc19ldGlxdWV0YXMiLCJhbHRlcmFyX2RhdGFfbGlzdGFfcHJvZHV0b3MiLCJnZXJlbmNpYXJfbW9kZWxvc19ldGlxdWV0YXMiLCJsaXN0YXJfdG9kb3NfdGlwb3NfYXJlYXNfYWNvZXMiLCJlZGl0YXJfY2FtcG9zX2FkaWNpb25haXNfY2FydGF6Il0sInNpZCI6IjE2ODA2OTk1MTktNGZlYmE5NGEtZjRmMS00ODRlLTlmYjMtZWQ0MDNiZmRlMzQ3IiwianRpIjoiMTY4MDY5OTUxOS0wNTk5ZjVmMS1iOTRmLTQ0ZDUtYmY0ZC01YTQ5YWRiYTEyOGEiLCJhdWQiOiJzbWFya2V0X3NvbHV0aW9ucyIsImlzcyI6InNtYXJrZXRfc29sdXRpb25zIiwiZXhwIjoxNjgwNzg1OTE5fQ.NMTrLc_J5rFvBQj4wmaQ2mzMPRt4iFojDDByfdD36eznphbWPamDLZzhTcN6xOcNngaB-qDWrKXq4q8JIQrQ1B66SveJOPgGcLPYOz03iorQ_zJRdWbCmFvJ3pw5d288gVnHwAT02jGnNBqaXxuKaFXRYJn5AIh8Oy7x-vM6R_U5mDo9DKdIspmDARziLSaULuETGnEwSG7qdOesW1rAuRPIwFDFC-QLpbYJ7dQekvqZsvIFIxZEAd8qWmoVmZlfqSi6s4XDzios1J5mom8r8v9MN4TPuLhUakfAxsvfCfY7NxuJKJHZ-kEZ70en49-drnQjhBHAIFehPJokKphgyw")
     print(cliente().client_id)
-    print()
+    print()
+    headers()
```

### Comparing `configcronos-0.0.2/configcronos/infra/configs/configs.py` & `configcronos-0.0.3/configcronos/infra/configs/configs.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 class Configs:
 
     def __init__(self):
 
         dotenv.load_dotenv()
         self.API_CONFIGS_URL = os.getenv("API_CONFIGS_URL", "https://api-gateway.smarketsolutions.com.br/v1/atenas")
-        self.USERNAME = os.getenv("USERNAME_SMARKET", "teste")
-        self.PASSWORD = os.getenv("PASSWORD_SMARKET", "teste")
-        self.CLIENT_ID = os.getenv("CLIENT_ID_SMARKET", "barcelos")
+        self.USERNAME = os.getenv("USERNAME_SMARKET", "davi_araujo")
+        self.PASSWORD = os.getenv("PASSWORD_SMARKET", "Smarket@2022")
+        self.CLIENT_ID = os.getenv("CLIENT_ID_SMARKET", "onboarding")
         self.API_CONFIGS_URL_AUTH = os.getenv("API_CONFIGS_URL_AUTH", "https://api-gateway.smarketsolutions.com.br/auth/token")
 
 @lru_cache()
 def get_configs():
     """Helper function to get env with lru cache"""
     return Configs()
```

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/auth_repository.py` & `configcronos-0.0.3/configcronos/infra/repositories/auth_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/client_repository.py` & `configcronos-0.0.3/configcronos/infra/repositories/client_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/database_repository.py` & `configcronos-0.0.3/configcronos/infra/repositories/database_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/phase1_repository.py` & `configcronos-0.0.3/configcronos/infra/repositories/phase1_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/phase2_repository.py` & `configcronos-0.0.3/configcronos/infra/repositories/phase2_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/pinger_repository.py` & `configcronos-0.0.3/configcronos/infra/repositories/pinger_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/schedule_repository.py` & `configcronos-0.0.3/configcronos/infra/repositories/schedule_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/segment_repositoy.py` & `configcronos-0.0.3/configcronos/infra/repositories/segment_repositoy.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/configcronos/infra/repositories/sqls_repository.py` & `configcronos-0.0.3/configcronos/infra/repositories/sqls_repository.py`

 * *Files identical despite different names*

### Comparing `configcronos-0.0.2/.gitignore` & `configcronos-0.0.3/.gitignore`

 * *Files identical despite different names*

