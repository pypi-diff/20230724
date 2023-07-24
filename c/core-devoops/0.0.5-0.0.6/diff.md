# Comparing `tmp/core_devoops-0.0.5.tar.gz` & `tmp/core_devoops-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_devoops-0.0.5.tar", max compression
+gzip compressed data, was "core_devoops-0.0.6.tar", max compression
```

## Comparing `core_devoops-0.0.5.tar` & `core_devoops-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      802 2023-07-24 06:38:44.034844 core_devoops-0.0.5/README.md
--rw-r--r--   0        0        0     1606 2023-07-24 11:50:30.489076 core_devoops-0.0.5/core_devoops/__init__.py
--rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.5/core_devoops/auth_configuration.py
--rw-r--r--   0        0        0     4649 2023-07-24 11:50:30.505077 core_devoops-0.0.5/core_devoops/authentification.py
--rw-r--r--   0        0        0     9306 2023-07-24 11:50:30.497076 core_devoops-0.0.5/core_devoops/check_dependencies.py
--rw-r--r--   0        0        0     1731 2023-07-24 11:50:30.517076 core_devoops-0.0.5/core_devoops/db_connection.py
--rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.5/core_devoops/list_utils.py
--rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.5/core_devoops/logger.py
--rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.5/core_devoops/pandas_utils.py
--rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.5/core_devoops/permissions.py
--rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.5/core_devoops/pydantic_utils.py
--rw-r--r--   0        0        0      995 2023-07-24 07:17:14.179994 core_devoops-0.0.5/core_devoops/read_write.py
--rw-r--r--   0        0        0      658 2023-07-24 11:50:30.501077 core_devoops-0.0.5/core_devoops/rights.py
--rw-r--r--   0        0        0     5563 2023-07-24 11:50:30.509076 core_devoops-0.0.5/core_devoops/safe_utils.py
--rw-r--r--   0        0        0      774 2023-07-24 11:50:30.513076 core_devoops-0.0.5/core_devoops/user.py
--rw-r--r--   0        0        0      601 2023-07-24 11:52:58.144429 core_devoops-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 core_devoops-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      802 2023-07-24 06:38:44.034844 core_devoops-0.0.6/README.md
+-rw-r--r--   0        0        0     1606 2023-07-24 11:50:30.489076 core_devoops-0.0.6/core_devoops/__init__.py
+-rw-r--r--   0        0        0      541 2023-07-24 07:14:08.516585 core_devoops-0.0.6/core_devoops/auth_configuration.py
+-rw-r--r--   0        0        0     4649 2023-07-24 11:50:30.505077 core_devoops-0.0.6/core_devoops/authentification.py
+-rw-r--r--   0        0        0     9306 2023-07-24 11:50:30.497076 core_devoops-0.0.6/core_devoops/check_dependencies.py
+-rw-r--r--   0        0        0     1731 2023-07-24 11:50:30.517076 core_devoops-0.0.6/core_devoops/db_connection.py
+-rw-r--r--   0        0        0     2282 2023-03-09 18:46:03.513478 core_devoops-0.0.6/core_devoops/list_utils.py
+-rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 core_devoops-0.0.6/core_devoops/logger.py
+-rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819470 core_devoops-0.0.6/core_devoops/pandas_utils.py
+-rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 core_devoops-0.0.6/core_devoops/permissions.py
+-rw-r--r--   0        0        0     1006 2022-08-23 12:06:55.429612 core_devoops-0.0.6/core_devoops/pydantic_utils.py
+-rw-r--r--   0        0        0      995 2023-07-24 07:17:14.179994 core_devoops-0.0.6/core_devoops/read_write.py
+-rw-r--r--   0        0        0      658 2023-07-24 11:50:30.501077 core_devoops-0.0.6/core_devoops/rights.py
+-rw-r--r--   0        0        0     5563 2023-07-24 11:50:30.509076 core_devoops-0.0.6/core_devoops/safe_utils.py
+-rw-r--r--   0        0        0      774 2023-07-24 11:50:30.513076 core_devoops-0.0.6/core_devoops/user.py
+-rw-r--r--   0        0        0     1767 2023-07-24 12:54:31.486305 core_devoops-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 core_devoops-0.0.6/PKG-INFO
```

### Comparing `core_devoops-0.0.5/README.md` & `core_devoops-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/__init__.py` & `core_devoops-0.0.6/core_devoops/__init__.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/auth_configuration.py` & `core_devoops-0.0.6/core_devoops/auth_configuration.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/authentification.py` & `core_devoops-0.0.6/core_devoops/authentification.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/check_dependencies.py` & `core_devoops-0.0.6/core_devoops/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/db_connection.py` & `core_devoops-0.0.6/core_devoops/db_connection.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/list_utils.py` & `core_devoops-0.0.6/core_devoops/list_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/logger.py` & `core_devoops-0.0.6/core_devoops/logger.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/pandas_utils.py` & `core_devoops-0.0.6/core_devoops/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/pydantic_utils.py` & `core_devoops-0.0.6/core_devoops/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/read_write.py` & `core_devoops-0.0.6/core_devoops/read_write.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/rights.py` & `core_devoops-0.0.6/core_devoops/rights.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/safe_utils.py` & `core_devoops-0.0.6/core_devoops/safe_utils.py`

 * *Files identical despite different names*

### Comparing `core_devoops-0.0.5/core_devoops/user.py` & `core_devoops-0.0.6/core_devoops/user.py`

 * *Files identical despite different names*

