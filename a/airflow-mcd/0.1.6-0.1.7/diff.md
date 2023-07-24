# Comparing `tmp/airflow_mcd-0.1.6.tar.gz` & `tmp/airflow_mcd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.1.6.tar", last modified: Mon Jul 17 16:35:49 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.1.7.tar", last modified: Mon Jul 24 21:15:55 2023, max compression
```

## Comparing `airflow_mcd-0.1.6.tar` & `airflow_mcd-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/Makefile
--rw-r--r--   0 root         (0) root         (0)     7468 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     6655 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     6967 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     5412 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2784 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/operators/circuit_breaker_operators.py
--rw-r--r--   0 root         (0) root         (0)    15407 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7468 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1137 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1483 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12924 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_circuit_breaker_op.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_dbt_cli_config.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_dbt_default_config_provider.py
--rw-r--r--   0 root         (0) root         (0)    21136 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_dbt_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.552064 airflow_mcd-0.1.7/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.552064 airflow_mcd-0.1.7/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.552064 airflow_mcd-0.1.7/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     7042 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     6336 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/operators/circuit_breaker_operators.py
+-rw-r--r--   0 root         (0) root         (0)    15407 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/airflow_mcd/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.552064 airflow_mcd-0.1.7/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-24 21:15:55.000000 airflow_mcd-0.1.7/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15028 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:15:55.556064 airflow_mcd-0.1.7/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_circuit_breaker_op.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_dbt_cli_config.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_dbt_default_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)    21136 2023-07-24 21:14:48.000000 airflow_mcd-0.1.7/tests/operators/test_dbt_operator.py
```

### Comparing `airflow_mcd-0.1.6/.circleci/config.yml` & `airflow_mcd-0.1.7/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/.gitignore` & `airflow_mcd-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/LICENSE` & `airflow_mcd-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/Makefile` & `airflow_mcd-0.1.7/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/PKG-INFO` & `airflow_mcd-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_mcd
-Version: 0.1.6
+Version: 0.1.7
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.6/README-dev.md` & `airflow_mcd-0.1.7/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/README.md` & `airflow_mcd-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.1.7/airflow_mcd/callbacks/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     end_date: str
     next_retry_datetime: Optional[str]
     max_tries: int
     try_number: int
     exception_message: Optional[str]
     inlets: Optional[List[Dict]]
     outlets: Optional[List[Dict]]
+    original_dates: Optional[str]
 
 
 @dataclass_json
 @dataclass
 class BaseDagResult:
     dag_id: str
     env: AirflowEnv = field(init=False)
@@ -108,14 +109,15 @@
     tasks: Optional[List[DagTaskInstanceResult]]
     state: str
     execution_date: str
     start_date: str
     end_date: str
     reason: Optional[str]
     event_type: str = 'dag'
+    original_dates: Optional[str] = None
 
 
 @dataclass_json
 @dataclass
 class DagTaskResult(BaseDagRunResult):
     task: DagTaskInstanceResult
     event_type: str = 'task'
```

### Comparing `airflow_mcd-0.1.6/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.1.7/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.1.7/airflow_mcd/callbacks/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from copy import deepcopy
 
-import pytz
 from airflow.models import TaskInstance, SlaMiss, DagRun, DAG
 from attr import asdict
-from datetime import datetime
+from datetime import datetime, timezone
 
 from airflow_mcd.callbacks.client import DagResult, DagTaskResult, AirflowEventsClient, DagTaskInstanceResult, \
     SlaMissesResult, TaskSlaMiss
 from typing import Dict, List, Any, Optional
 
 
 logger = logging.getLogger(__name__)
@@ -33,17 +32,18 @@
         result = DagResult(
             dag_id=dag.dag_id,
             run_id=context['run_id'],
             success=success,
             reason=context.get('reason'),
             tasks=[cls._get_task_instance_result(ti) for ti in task_instances],
             state=dag_run.state,
-            execution_date=dag_run.execution_date.isoformat(),
-            start_date=dag_run.start_date.isoformat(),
-            end_date=dag_run.end_date.isoformat(),
+            execution_date=cls._get_datetime_isoformat(dag_run.execution_date),
+            start_date=cls._get_datetime_isoformat(dag_run.start_date),
+            end_date=cls._get_datetime_isoformat(dag_run.end_date),
+            original_dates=cls._get_original_dates(dag_run.execution_date, dag_run.start_date, dag_run.end_date),
         )
         cls._get_events_client(dag).upload_dag_result(result)
 
     @classmethod
     def mcd_post_task_result(cls, success: bool, context: Dict):
         if 'dag' not in context or 'run_id' not in context or 'task_instance' not in context:
             logger.error('Invalid context received in MCD task callback: dag, run_id and task_instance are expected')
@@ -63,16 +63,16 @@
     @classmethod
     def mcd_post_sla_misses(cls, dag: DAG, sla_misses: List[SlaMiss]):
         result = SlaMissesResult(
             dag_id=dag.dag_id,
             sla_misses=[
                 TaskSlaMiss(
                     task_id=sla_miss.task_id,
-                    execution_date=sla_miss.execution_date.isoformat(),
-                    timestamp=sla_miss.timestamp.isoformat(),
+                    execution_date=cls._get_datetime_isoformat(sla_miss.execution_date),
+                    timestamp=cls._get_datetime_isoformat(sla_miss.timestamp),
                 ) for sla_miss in sla_misses
             ]
         )
         cls._get_events_client(dag).upload_sla_misses(result)
 
     @classmethod
     def _get_task_instance_result(
@@ -82,25 +82,42 @@
     ) -> DagTaskInstanceResult:
         return DagTaskInstanceResult(
             task_id=ti.task_id,
             state=ti.state,
             log_url=ti.log_url,
             prev_attempted_tries=ti.prev_attempted_tries,
             duration=ti.duration or 0,
-            execution_date=ti.execution_date.isoformat(),
-            start_date=ti.start_date.isoformat(),
-            end_date=ti.end_date.isoformat() if ti.end_date else datetime.now(tz=pytz.UTC).isoformat(),
+            execution_date=cls._get_datetime_isoformat(ti.execution_date),
+            start_date=cls._get_datetime_isoformat(ti.start_date),
+            end_date=cls._get_datetime_isoformat(ti.end_date),
             next_retry_datetime=cls._get_next_retry_datetime(ti),
             max_tries=ti.max_tries,
             try_number=ti.try_number,
             exception_message=exception_message,
             inlets=cls._get_lineage_list(ti, 'inlets'),
             outlets=cls._get_lineage_list(ti, 'outlets'),
+            original_dates=cls._get_original_dates(ti.execution_date, ti.start_date, ti.end_date),
         )
 
+    @staticmethod
+    def _get_datetime_isoformat(d: Optional[datetime]) -> str:
+        return d.isoformat() if d else datetime.now(tz=timezone.utc).isoformat()
+
+    @staticmethod
+    def _get_original_dates(
+            execution_date: Optional[datetime],
+            start_date: Optional[datetime],
+            end_date: Optional[datetime]
+    ) -> str:
+        return f"execution={str(execution_date)}, start_date={str(start_date)}, end_date={str(end_date)}"
+
+    @staticmethod
+    def _get_optional_datetime_isoformat(d: Optional[datetime]) -> Optional[str]:
+        return d.isoformat() if d else None
+
     @classmethod
     def _get_events_client(cls, dag: DAG) -> AirflowEventsClient:
         dag_params = dag.params or {}
         mcd_session_conn_id = 'mcd_default_session'
 
         param_value = dag_params.get('mcd_connection_id')
         # in Airflow 2.2.x we're getting a Param object while in Airflow 2.6.x we're getting a string object
@@ -114,15 +131,15 @@
 
         return AirflowEventsClient(mcd_session_conn_id=mcd_session_conn_id, call_timeout=_DEFAULT_CALL_TIMEOUT)
 
     @classmethod
     def _get_next_retry_datetime(cls, ti: TaskInstance) -> Optional[str]:
         if not hasattr(ti, 'task') or not ti.end_date:
             return None
-        return ti.next_retry_datetime().isoformat()
+        return cls._get_optional_datetime_isoformat(ti.next_retry_datetime())
 
     @classmethod
     def _get_lineage_dict(cls, o: Any) -> Dict:
         attrs = deepcopy(asdict(o))
         attrs['type'] = str(type(o))
         return attrs
```

### Comparing `airflow_mcd-0.1.6/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.1.7/airflow_mcd/hooks/session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.1.7/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.1.7/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/airflow_mcd/operators/dbt.py` & `airflow_mcd-0.1.7/airflow_mcd/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.1.7/airflow_mcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-mcd
-Version: 0.1.6
+Version: 0.1.7
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.6/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.1.7/airflow_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/examples/sample_circuit_dag.py` & `airflow_mcd-0.1.7/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/setup.py` & `airflow_mcd-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.1.7/tests/callbacks/test_callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 import os
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from typing import Dict, List, Optional
 from unittest import TestCase
-from unittest.mock import create_autospec, patch
+from unittest.mock import create_autospec, patch, ANY
 
-import pytz
 from airflow.models import DagRun, TaskInstance, SlaMiss, DAG
 from sgqlc.types import Variable
 
 from airflow_mcd.callbacks.client import AirflowEventsClient, AirflowEnv
 from airflow_mcd.callbacks.utils import AirflowEventsClientUtils
+from freezegun import freeze_time
 
 
 # needed to have a successful assert_called_with as Variable doesn't implement __eq__
 class EqVariable(Variable):
     def __eq__(self, other):
         return other.name == self.name
 
 
-
 class CallbacksTests(TestCase):
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_dag_result_success(self,  mock_client_upload_result):
         self._test_upload_dag_result(True, mock_client_upload_result)
 
+    @freeze_time("2023-02-03 10:11:12", tz_offset=0)
+    @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
+    def test_upload_dag_result_success_no_dates(self,  mock_client_upload_result):
+        self._test_upload_dag_result(True, mock_client_upload_result, set_dates=False)
+
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_dag_result_failure(self, mock_client_upload_result):
         self._test_upload_dag_result(False, mock_client_upload_result)
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_success(self, mock_client_upload_result):
         self._test_upload_task_result(True, False, mock_client_upload_result)
 
+    @freeze_time("2023-02-03 10:11:12", tz_offset=0)
+    @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
+    def test_upload_task_result_success_no_dates(self, mock_client_upload_result):
+        self._test_upload_task_result(True, False, mock_client_upload_result, set_dates=False)
+
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_failure(self, mock_client_upload_result):
         self._test_upload_task_result(False, False, mock_client_upload_result)
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_running(self, mock_client_upload_result):
         self._test_upload_task_result(True, True, mock_client_upload_result)
@@ -46,21 +55,21 @@
 
         dag = create_autospec(DAG)
         dag.dag_id = "dag_123"
         dag.params = {}
 
         sla_miss_1 = create_autospec(SlaMiss)
         sla_miss_1.task_id = "task_123"
-        sla_miss_1.execution_date = datetime.now(tz=pytz.UTC) - timedelta(seconds=10)
-        sla_miss_1.timestamp = datetime.now(tz=pytz.UTC)
+        sla_miss_1.execution_date = datetime.now(tz=timezone.utc) - timedelta(seconds=10)
+        sla_miss_1.timestamp = datetime.now(tz=timezone.utc)
 
         sla_miss_2 = create_autospec(SlaMiss)
         sla_miss_2.task_id = "task_234"
-        sla_miss_2.execution_date = datetime.now(tz=pytz.UTC) - timedelta(seconds=10)
-        sla_miss_2.timestamp = datetime.now(tz=pytz.UTC)
+        sla_miss_2.execution_date = datetime.now(tz=timezone.utc) - timedelta(seconds=10)
+        sla_miss_2.timestamp = datetime.now(tz=timezone.utc)
 
         sla_misses = [
             sla_miss_1,
             sla_miss_2,
         ]
         utils.mcd_post_sla_misses(dag, sla_misses)
 
@@ -143,53 +152,56 @@
         self.assertEqual("id", params_env.env_id)
         self.assertEqual("1.0", params_env.version)
         self.assertEqual("url", params_env.base_url)
 
     def _test_upload_dag_result(
             self,
             success: bool,
-            mock_client_upload_result
+            mock_client_upload_result,
+            set_dates: bool = True,
     ):
-        dag_context = self._create_dag_context(success)
+        dag_context = self._create_dag_context(success, set_dates=set_dates)
         dag: DAG = dag_context["dag"]
         dag_run: DagRun = dag_context["dag_run"]
         task_instances: List[TaskInstance] = dag_run.get_task_instances()
 
         utils = AirflowEventsClientUtils()
         utils.mcd_post_dag_result(dag_context, success)
 
+        now_isoformat = datetime.now(tz=timezone.utc).isoformat()
         mock_client_upload_result.assert_called()
         mock_client_upload_result.assert_called_with(
             AirflowEventsClient._UPLOAD_AIRFLOW_DAG_RESULT_OPERATION,
             {
                 "dag_id": dag.dag_id,
                 "run_id": dag_context["run_id"],
                 "success": success,
                 "reason": dag_context.get("reason"),
                 "state": dag_run.state,
-                "execution_date": dag_run.execution_date.isoformat(),
-                "start_date": dag_run.start_date.isoformat(),
-                "end_date": dag_run.end_date.isoformat(),
+                "execution_date": dag_run.execution_date.isoformat() if set_dates else now_isoformat,
+                "start_date": dag_run.start_date.isoformat() if set_dates else now_isoformat,
+                "end_date": dag_run.end_date.isoformat() if set_dates else now_isoformat,
                 "env": self._get_graphql_env(),
                 "payload": EqVariable("payload"),
             },
             {
                 "dag_id": dag.dag_id,
                 "env": self._get_env(),
                 "run_id": dag_context["run_id"],
                 "success": success,
                 "tasks": [
-                    self._get_dag_task_instance_result(ti) for ti in task_instances
+                    self._get_dag_task_instance_result(ti, set_dates=set_dates) for ti in task_instances
                 ],
                 "state": dag_run.state,
-                "execution_date": dag_run.execution_date.isoformat(),
-                "start_date": dag_run.start_date.isoformat(),
-                "end_date": dag_run.end_date.isoformat(),
+                "execution_date": dag_run.execution_date.isoformat() if set_dates else now_isoformat,
+                "start_date": dag_run.start_date.isoformat() if set_dates else now_isoformat,
+                "end_date": dag_run.end_date.isoformat() if set_dates else now_isoformat,
                 "reason": dag_context.get("reason"),
                 "event_type": "dag",
+                "original_dates": ANY,
             }
         )
 
     @staticmethod
     def _get_graphql_env() -> Dict:
         return {
             "env_name": "airflow",
@@ -200,78 +212,87 @@
         return {
             "env_name": "airflow",
             "env_id": None,
             "version": None,
             "base_url": None
         }
 
-    def _create_dag_context(self, success: bool, task_running: bool = False) -> Dict:
+    def _create_dag_context(self, success: bool, task_running: bool = False, set_dates: bool = True) -> Dict:
         dag = create_autospec(DAG)
         dag.dag_id = "dag_123"
         dag.params = {}
         dag_run = create_autospec(DagRun)
         task_instances = [
             self._create_task_instance(
                 dag_id=dag.dag_id,
                 task_id="task_123",
                 state="running" if task_running else "success",
                 running=task_running,
+                set_dates=set_dates,
             ),
             self._create_task_instance(
                 dag_id=dag.dag_id,
                 task_id="task_234",
                 state="success",
+                set_dates=set_dates,
             ),
         ]
         state = "success" if success else "failed"
         dag_run.get_task_instances.return_value = task_instances
         dag_run.state = state
-        dag_run.execution_date = datetime.now(tz=pytz.UTC) - timedelta(seconds=10)
-        dag_run.start_date = datetime.now(tz=pytz.UTC) - timedelta(seconds=9)
-        dag_run.end_date = datetime.now(tz=pytz.UTC)
+        if set_dates:
+            dag_run.execution_date = datetime.now(tz=timezone.utc) - timedelta(seconds=10)
+            dag_run.start_date = datetime.now(tz=timezone.utc) - timedelta(seconds=9)
+            dag_run.end_date = datetime.now(tz=timezone.utc)
+        else:
+            dag_run.execution_date = None
+            dag_run.start_date = None
+            dag_run.end_date = None
 
         dag_context = {
             "dag": dag,
             "run_id": '123',
             "dag_run": dag_run,
             "reason": "succeeded" if success else "task failed",
         }
         return dag_context
 
     def _test_upload_task_result(
             self,
             success: bool,
             task_running: bool,
-            mock_client_upload_result
+            mock_client_upload_result,
+            set_dates: bool = True,
     ):
-        dag_context = self._create_dag_context(success, task_running)
+        dag_context = self._create_dag_context(success, task_running, set_dates=set_dates)
         state = "running" if task_running else "success" if success else "failed"
         exception_message: str = "task failed" if not success else None
         if not success:
             dag_context["exception"] = Exception(exception_message)
         dag: DAG = dag_context["dag"]
         dag_run: DagRun = dag_context["dag_run"]
         task_instances: List[TaskInstance] = dag_run.get_task_instances()
         task_instance = task_instances[0]
         task_instance.state = state
         dag_context["task_instance"] = task_instance
         utils = AirflowEventsClientUtils()
         utils.mcd_post_task_result(success, dag_context)
 
+        now_isoformat = datetime.now(tz=timezone.utc).isoformat()
         expected_graphql_payload = {
             "dag_id": dag.dag_id,
             "run_id": dag_context["run_id"],
             "task_id": task_instance.task_id,
             "success": success,
             "env": self._get_graphql_env(),
             "state": state,
             "log_url": f"http://airflow.com/{dag.dag_id}/{task_instance.task_id}/log",
-            "execution_date": task_instance.execution_date.isoformat(),
-            'start_date': task_instance.start_date.isoformat(),
-            'end_date': task_instance.end_date.isoformat(),
+            "execution_date": task_instance.execution_date.isoformat() if set_dates else now_isoformat,
+            'start_date': task_instance.start_date.isoformat() if set_dates else now_isoformat,
+            'end_date': task_instance.end_date.isoformat() if set_dates else now_isoformat,
             'duration': task_instance.duration or 0,
             'attempt_number': task_instance.prev_attempted_tries,
             "payload": EqVariable("payload"),
         }
         if exception_message and not success:
             expected_graphql_payload["exception_message"] = exception_message
 
@@ -280,46 +301,63 @@
             AirflowEventsClient._UPLOAD_AIRFLOW_TASK_RESULT_OPERATION,
             expected_graphql_payload,
             {
                 "dag_id": dag.dag_id,
                 "env": self._get_env(),
                 "run_id": dag_context["run_id"],
                 "success": success,
-                "task": self._get_dag_task_instance_result(task_instance, exception_message),
+                "task": self._get_dag_task_instance_result(task_instance, exception_message, set_dates=set_dates),
                 "event_type": "task",
             }
         )
 
     @staticmethod
-    def _create_task_instance(dag_id: str, task_id: str, state: str, running: bool = False) -> TaskInstance:
+    def _create_task_instance(
+            dag_id: str,
+            task_id: str,
+            state: str,
+            running: bool = False,
+            set_dates: bool = True,
+    ) -> TaskInstance:
         task_instance = create_autospec(TaskInstance)
         task_instance.task_id = task_id
         task_instance.state = state
         task_instance.log_url = f"http://airflow.com/{dag_id}/{task_instance.task_id}/log"
         task_instance.prev_attempted_tries = 0
         task_instance.duration = 10.5 if not running else None
-        task_instance.execution_date = datetime.now(tz=pytz.UTC) - timedelta(seconds=10)
-        task_instance.start_date = datetime.now(tz=pytz.UTC) - timedelta(seconds=9)
-        task_instance.end_date = datetime.now(tz=pytz.UTC)
+        if set_dates:
+            task_instance.execution_date = datetime.now(tz=timezone.utc) - timedelta(seconds=10)
+            task_instance.start_date = datetime.now(tz=timezone.utc) - timedelta(seconds=9)
+            task_instance.end_date = datetime.now(tz=timezone.utc)
+        else:
+            task_instance.execution_date = None
+            task_instance.start_date = None
+            task_instance.end_date = None
         task_instance.max_tries = 3
         task_instance.try_number = 1
         return task_instance
 
     @staticmethod
-    def _get_dag_task_instance_result(task_instance: TaskInstance, exception_message: Optional[str] = None) -> Dict:
+    def _get_dag_task_instance_result(
+            task_instance: TaskInstance,
+            exception_message: Optional[str] = None,
+            set_dates: bool = True,
+    ) -> Dict:
+        now_isoformat = datetime.now(tz=timezone.utc).isoformat()
         return {
             "task_id": task_instance.task_id,
             "state": task_instance.state,
             "log_url": task_instance.log_url,
             "prev_attempted_tries": task_instance.prev_attempted_tries,
             "duration": task_instance.duration or 0,
-            "execution_date": task_instance.execution_date.isoformat(),
-            "start_date": task_instance.start_date.isoformat(),
-            "end_date": task_instance.end_date.isoformat(),
+            "execution_date": task_instance.execution_date.isoformat() if set_dates else now_isoformat,
+            "start_date": task_instance.start_date.isoformat() if set_dates else now_isoformat,
+            "end_date": task_instance.end_date.isoformat() if set_dates else now_isoformat,
             "next_retry_datetime": None,
             "max_tries": task_instance.max_tries,
             "try_number": task_instance.try_number,
             "exception_message": exception_message,
             "inlets": None,
             "outlets": None,
+            "original_dates": ANY,
         }
```

### Comparing `airflow_mcd-0.1.6/tests/hooks/test_session_hook.py` & `airflow_mcd-0.1.7/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/tests/operators/test_base_op.py` & `airflow_mcd-0.1.7/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.1.7/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/tests/operators/test_dbt_cli_config.py` & `airflow_mcd-0.1.7/tests/operators/test_dbt_cli_config.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/tests/operators/test_dbt_default_config_provider.py` & `airflow_mcd-0.1.7/tests/operators/test_dbt_default_config_provider.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.6/tests/operators/test_dbt_operator.py` & `airflow_mcd-0.1.7/tests/operators/test_dbt_operator.py`

 * *Files identical despite different names*

