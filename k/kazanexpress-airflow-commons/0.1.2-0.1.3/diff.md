# Comparing `tmp/kazanexpress_airflow_commons-0.1.2.tar.gz` & `tmp/kazanexpress_airflow_commons-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kazanexpress_airflow_commons-0.1.2.tar", max compression
+gzip compressed data, was "kazanexpress_airflow_commons-0.1.3.tar", max compression
```

## Comparing `kazanexpress_airflow_commons-0.1.2.tar` & `kazanexpress_airflow_commons-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    15951 2023-05-18 19:40:26.380239 kazanexpress_airflow_commons-0.1.2/README.md
--rw-r--r--   0        0        0      936 2023-05-18 20:28:58.206878 kazanexpress_airflow_commons-0.1.2/airflow_commons/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 11:22:17.983767 kazanexpress_airflow_commons-0.1.2/airflow_commons/helpers/__init__.py
--rw-r--r--   0        0        0     6344 2023-07-19 17:57:01.775159 kazanexpress_airflow_commons-0.1.2/airflow_commons/helpers/notify.py
--rw-r--r--   0        0        0        0 2023-02-24 11:22:17.983767 kazanexpress_airflow_commons-0.1.2/airflow_commons/hooks/__init__.py
--rw-r--r--   0        0        0     6343 2023-07-13 13:36:11.369949 kazanexpress_airflow_commons-0.1.2/airflow_commons/hooks/clickhouse_hook.py
--rw-r--r--   0        0        0     2500 2023-05-25 20:40:40.767745 kazanexpress_airflow_commons-0.1.2/airflow_commons/hooks/odd_hook.py
--rw-r--r--   0        0        0        0 2023-02-24 11:22:17.983767 kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/__init__.py
--rw-r--r--   0        0        0     3518 2023-05-25 20:40:22.215513 kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/clickhouse_execute_operator.py
--rw-r--r--   0        0        0     7111 2023-05-25 20:40:34.947672 kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/file_to_clickhouse_operator.py
--rw-r--r--   0        0        0    13353 2023-07-19 18:09:08.237856 kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/google_sheet_to_db_operator.py
--rw-r--r--   0        0        0    11095 2023-05-25 20:40:43.459778 kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/odd_sql_check_dq_test_operator.py
--rw-r--r--   0        0        0     5586 2023-05-25 20:40:48.075836 kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/postgres_to_clickhouse_operator.py
--rw-r--r--   0        0        0     3957 2023-05-25 20:41:14.312161 kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/sql_to_file_operator.py
--rw-r--r--   0        0        0     1114 2023-07-24 13:21:55.114662 kazanexpress_airflow_commons-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    17133 1970-01-01 00:00:00.000000 kazanexpress_airflow_commons-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    15951 2023-05-18 19:40:26.380239 kazanexpress_airflow_commons-0.1.3/README.md
+-rw-r--r--   0        0        0      936 2023-05-18 20:28:58.206878 kazanexpress_airflow_commons-0.1.3/airflow_commons/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-24 11:22:17.983767 kazanexpress_airflow_commons-0.1.3/airflow_commons/helpers/__init__.py
+-rw-r--r--   0        0        0     6344 2023-07-19 17:57:01.775159 kazanexpress_airflow_commons-0.1.3/airflow_commons/helpers/notify.py
+-rw-r--r--   0        0        0        0 2023-02-24 11:22:17.983767 kazanexpress_airflow_commons-0.1.3/airflow_commons/hooks/__init__.py
+-rw-r--r--   0        0        0     6343 2023-07-13 13:36:11.369949 kazanexpress_airflow_commons-0.1.3/airflow_commons/hooks/clickhouse_hook.py
+-rw-r--r--   0        0        0     2500 2023-05-25 20:40:40.767745 kazanexpress_airflow_commons-0.1.3/airflow_commons/hooks/odd_hook.py
+-rw-r--r--   0        0        0        0 2023-02-24 11:22:17.983767 kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/__init__.py
+-rw-r--r--   0        0        0     3518 2023-05-25 20:40:22.215513 kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/clickhouse_execute_operator.py
+-rw-r--r--   0        0        0     7111 2023-05-25 20:40:34.947672 kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/file_to_clickhouse_operator.py
+-rw-r--r--   0        0        0    13353 2023-07-19 18:09:08.237856 kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/google_sheet_to_db_operator.py
+-rw-r--r--   0        0        0    11095 2023-05-25 20:40:43.459778 kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/odd_sql_check_dq_test_operator.py
+-rw-r--r--   0        0        0     5586 2023-05-25 20:40:48.075836 kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/postgres_to_clickhouse_operator.py
+-rw-r--r--   0        0        0     3957 2023-05-25 20:41:14.312161 kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/sql_to_file_operator.py
+-rw-r--r--   0        0        0     1264 2023-07-24 14:52:52.926440 kazanexpress_airflow_commons-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    17133 1970-01-01 00:00:00.000000 kazanexpress_airflow_commons-0.1.3/PKG-INFO
```

### Comparing `kazanexpress_airflow_commons-0.1.2/README.md` & `kazanexpress_airflow_commons-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/__init__.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/__init__.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/helpers/notify.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/helpers/notify.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/hooks/clickhouse_hook.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/hooks/clickhouse_hook.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/hooks/odd_hook.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/hooks/odd_hook.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/clickhouse_execute_operator.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/clickhouse_execute_operator.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/file_to_clickhouse_operator.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/file_to_clickhouse_operator.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/google_sheet_to_db_operator.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/google_sheet_to_db_operator.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/odd_sql_check_dq_test_operator.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/odd_sql_check_dq_test_operator.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/postgres_to_clickhouse_operator.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/postgres_to_clickhouse_operator.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/airflow_commons/operators/sql_to_file_operator.py` & `kazanexpress_airflow_commons-0.1.3/airflow_commons/operators/sql_to_file_operator.py`

 * *Files identical despite different names*

### Comparing `kazanexpress_airflow_commons-0.1.2/pyproject.toml` & `kazanexpress_airflow_commons-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kazanexpress-airflow-commons"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python package framework to work with Apache Airflow developed in KazanExpress Data Office"
 readme = "README.md"
 authors = ["Your Name <you@example.com>"]
 packages = [{include = "airflow_commons"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -30,10 +30,16 @@
 wemake-python-styleguide = "^0.17.0"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 testcontainers = "^3.7.1"
 types-pyyaml = "^6.0.12.9"
 types-requests = "^2.30.0.0"
 
+[[tool.poetry.source]]
+name = "nexus"
+url = "https://nexus.infra.cluster.kznexpess.com/repository/ke-pypi/simple/"
+default = false
+secondary = false
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kazanexpress_airflow_commons-0.1.2/PKG-INFO` & `kazanexpress_airflow_commons-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kazanexpress-airflow-commons
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package framework to work with Apache Airflow developed in KazanExpress Data Office
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

