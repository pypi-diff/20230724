# Comparing `tmp/autometrics-0.7.tar.gz` & `tmp/autometrics-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autometrics-0.7.tar", max compression
+gzip compressed data, was "autometrics-0.8.tar", max compression
```

## Comparing `autometrics-0.7.tar` & `autometrics-0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1022 2023-04-12 17:23:29.278864 autometrics-0.7/LICENSE
--rw-r--r--   0        0        0     9181 2023-07-19 14:50:31.112596 autometrics-0.7/README.md
--rw-r--r--   0        0        0     2081 2023-07-19 15:57:15.109845 autometrics-0.7/pyproject.toml
--rw-r--r--   0        0        0       25 2023-06-28 13:42:06.860107 autometrics-0.7/src/autometrics/__init__.py
--rw-r--r--   0        0        0     1489 2023-06-26 13:25:13.436175 autometrics-0.7/src/autometrics/constants.py
--rw-r--r--   0        0        0     5672 2023-07-19 14:50:31.113087 autometrics-0.7/src/autometrics/decorator.py
--rw-r--r--   0        0        0     3050 2023-04-13 12:18:19.449416 autometrics-0.7/src/autometrics/objectives.py
--rw-r--r--   0        0        0     2197 2023-05-11 12:02:53.378737 autometrics-0.7/src/autometrics/prometheus_url.py
--rw-r--r--   0        0        0     1125 2023-07-19 14:50:31.113230 autometrics-0.7/src/autometrics/test_caller.py
--rw-r--r--   0        0        0    16117 2023-07-19 14:50:31.113444 autometrics-0.7/src/autometrics/test_decorator.py
--rw-r--r--   0        0        0     3065 2023-05-11 12:02:53.378981 autometrics-0.7/src/autometrics/test_prometheus_url.py
--rw-r--r--   0        0        0       23 2023-05-05 10:51:08.826284 autometrics-0.7/src/autometrics/tracker/__init__.py
--rw-r--r--   0        0        0      680 2023-06-15 09:09:44.376855 autometrics-0.7/src/autometrics/tracker/exemplar.py
--rw-r--r--   0        0        0     6397 2023-07-19 15:54:12.041119 autometrics-0.7/src/autometrics/tracker/opentelemetry.py
--rw-r--r--   0        0        0     4767 2023-06-28 13:42:06.860732 autometrics-0.7/src/autometrics/tracker/prometheus.py
--rw-r--r--   0        0        0     2462 2023-07-19 14:50:31.114279 autometrics-0.7/src/autometrics/tracker/test_concurrency.py
--rw-r--r--   0        0        0     3027 2023-06-16 11:01:50.465190 autometrics-0.7/src/autometrics/tracker/test_tracker.py
--rw-r--r--   0        0        0     2824 2023-06-28 13:42:06.860895 autometrics-0.7/src/autometrics/tracker/tracker.py
--rw-r--r--   0        0        0     1551 2023-07-19 14:50:31.114920 autometrics-0.7/src/autometrics/utils.py
--rw-r--r--   0        0        0    10330 1970-01-01 00:00:00.000000 autometrics-0.7/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-12 17:23:29.278864 autometrics-0.8/LICENSE
+-rw-r--r--   0        0        0     9181 2023-07-19 14:50:31.112596 autometrics-0.8/README.md
+-rw-r--r--   0        0        0     2094 2023-07-24 10:43:33.776641 autometrics-0.8/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-06-28 13:42:06.860107 autometrics-0.8/src/autometrics/__init__.py
+-rw-r--r--   0        0        0     1489 2023-06-26 13:25:13.436175 autometrics-0.8/src/autometrics/constants.py
+-rw-r--r--   0        0        0     5672 2023-07-19 14:50:31.113087 autometrics-0.8/src/autometrics/decorator.py
+-rw-r--r--   0        0        0     3050 2023-04-13 12:18:19.449416 autometrics-0.8/src/autometrics/objectives.py
+-rw-r--r--   0        0        0     2197 2023-05-11 12:02:53.378737 autometrics-0.8/src/autometrics/prometheus_url.py
+-rw-r--r--   0        0        0     1125 2023-07-19 14:50:31.113230 autometrics-0.8/src/autometrics/test_caller.py
+-rw-r--r--   0        0        0    16117 2023-07-19 14:50:31.113444 autometrics-0.8/src/autometrics/test_decorator.py
+-rw-r--r--   0        0        0     3065 2023-05-11 12:02:53.378981 autometrics-0.8/src/autometrics/test_prometheus_url.py
+-rw-r--r--   0        0        0       23 2023-05-05 10:51:08.826284 autometrics-0.8/src/autometrics/tracker/__init__.py
+-rw-r--r--   0        0        0      680 2023-06-15 09:09:44.376855 autometrics-0.8/src/autometrics/tracker/exemplar.py
+-rw-r--r--   0        0        0     6397 2023-07-19 15:54:12.041119 autometrics-0.8/src/autometrics/tracker/opentelemetry.py
+-rw-r--r--   0        0        0     4767 2023-06-28 13:42:06.860732 autometrics-0.8/src/autometrics/tracker/prometheus.py
+-rw-r--r--   0        0        0     2462 2023-07-19 14:50:31.114279 autometrics-0.8/src/autometrics/tracker/test_concurrency.py
+-rw-r--r--   0        0        0     3027 2023-06-16 11:01:50.465190 autometrics-0.8/src/autometrics/tracker/test_tracker.py
+-rw-r--r--   0        0        0     2824 2023-06-28 13:42:06.860895 autometrics-0.8/src/autometrics/tracker/tracker.py
+-rw-r--r--   0        0        0     1551 2023-07-19 14:50:31.114920 autometrics-0.8/src/autometrics/utils.py
+-rw-r--r--   0        0        0    10345 1970-01-01 00:00:00.000000 autometrics-0.8/PKG-INFO
```

### Comparing `autometrics-0.7/LICENSE` & `autometrics-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/README.md` & `autometrics-0.8/README.md`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/pyproject.toml` & `autometrics-0.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autometrics"
-version = "0.7"
+version = "0.8"
 description = "Easily add metrics to your system – and actually understand them using automatically customized Prometheus queries"
 authors = ["Fiberplane <info@fiberplane.com>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/autometrics-dev/autometrics-py"
 homepage = "https://github.com/autometrics-dev/autometrics-py"
 keywords = ["metrics", "telemetry", "prometheus", "monitoring", "observability", "instrumentation"]
@@ -14,17 +14,17 @@
 # ]
 packages = [{include = "autometrics", from = "src"}]
 
 [tool.poetry.dependencies]
 opentelemetry-api = "^1.17.0"
 opentelemetry-exporter-prometheus = "^1.12.0rc1"
 opentelemetry-sdk = "^1.17.0"
-prometheus-client = "0.16.0"
+prometheus-client = "^0.16.0 || ^0.17.0"
 python = "^3.8"
-python-dotenv = "1.0.0"
+python-dotenv = "^1.0.0"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.307"
```

### Comparing `autometrics-0.7/src/autometrics/constants.py` & `autometrics-0.8/src/autometrics/constants.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/decorator.py` & `autometrics-0.8/src/autometrics/decorator.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/objectives.py` & `autometrics-0.8/src/autometrics/objectives.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/prometheus_url.py` & `autometrics-0.8/src/autometrics/prometheus_url.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/test_caller.py` & `autometrics-0.8/src/autometrics/test_caller.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/test_decorator.py` & `autometrics-0.8/src/autometrics/test_decorator.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/test_prometheus_url.py` & `autometrics-0.8/src/autometrics/test_prometheus_url.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/tracker/exemplar.py` & `autometrics-0.8/src/autometrics/tracker/exemplar.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/tracker/opentelemetry.py` & `autometrics-0.8/src/autometrics/tracker/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/tracker/prometheus.py` & `autometrics-0.8/src/autometrics/tracker/prometheus.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/tracker/test_concurrency.py` & `autometrics-0.8/src/autometrics/tracker/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/tracker/test_tracker.py` & `autometrics-0.8/src/autometrics/tracker/test_tracker.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/tracker/tracker.py` & `autometrics-0.8/src/autometrics/tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/src/autometrics/utils.py` & `autometrics-0.8/src/autometrics/utils.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.7/PKG-INFO` & `autometrics-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autometrics
-Version: 0.7
+Version: 0.8
 Summary: Easily add metrics to your system – and actually understand them using automatically customized Prometheus queries
 Home-page: https://github.com/autometrics-dev/autometrics-py
 License: MIT OR Apache-2.0
 Keywords: metrics,telemetry,prometheus,monitoring,observability,instrumentation
 Author: Fiberplane
 Author-email: info@fiberplane.com
 Requires-Python: >=3.8,<4.0
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: opentelemetry-api (>=1.17.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-prometheus (>=1.12.0rc1,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
-Requires-Dist: prometheus-client (==0.16.0)
-Requires-Dist: python-dotenv (==1.0.0)
+Requires-Dist: prometheus-client (>=0.16.0,<0.18.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/autometrics-dev/autometrics-py
 Description-Content-Type: text/markdown
 
 ![GitHub_headerImage](https://user-images.githubusercontent.com/3262610/221191767-73b8a8d9-9f8b-440e-8ab6-75cb3c82f2bc.png)
 
 [![Tests](https://github.com/autometrics-dev/autometrics-py/actions/workflows/main.yml/badge.svg)](https://github.com/autometrics-dev/autometrics-py/actions/workflows/main.yml)
```

