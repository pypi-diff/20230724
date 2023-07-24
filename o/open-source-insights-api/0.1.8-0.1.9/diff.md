# Comparing `tmp/open_source_insights_api-0.1.8.tar.gz` & `tmp/open_source_insights_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_source_insights_api-0.1.8.tar", max compression
+gzip compressed data, was "open_source_insights_api-0.1.9.tar", max compression
```

## Comparing `open_source_insights_api-0.1.8.tar` & `open_source_insights_api-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1090 2023-06-29 12:25:06.013868 open_source_insights_api-0.1.8/LICENSE
--rw-r--r--   0        0        0     1398 2023-06-29 12:18:46.133876 open_source_insights_api-0.1.8/README.md
--rw-r--r--   0        0        0       92 2023-06-30 16:18:22.076458 open_source_insights_api-0.1.8/open_source_insights_api/__init__.py
--rw-r--r--   0        0        0    16632 2023-06-30 16:17:34.206457 open_source_insights_api-0.1.8/open_source_insights_api/os_insights.py
--rw-r--r--   0        0        0      958 2023-06-30 16:18:15.726458 open_source_insights_api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-29 12:25:06.013868 open_source_insights_api-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1398 2023-06-29 12:18:46.133876 open_source_insights_api-0.1.9/README.md
+-rw-r--r--   0        0        0       92 2023-07-01 21:12:54.446843 open_source_insights_api-0.1.9/open_source_insights_api/__init__.py
+-rw-r--r--   0        0        0    18244 2023-07-01 21:12:26.911962 open_source_insights_api-0.1.9/open_source_insights_api/os_insights.py
+-rw-r--r--   0        0        0      958 2023-07-01 21:12:48.226843 open_source_insights_api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.9/PKG-INFO
```

### Comparing `open_source_insights_api-0.1.8/LICENSE` & `open_source_insights_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `open_source_insights_api-0.1.8/README.md` & `open_source_insights_api-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `open_source_insights_api-0.1.8/pyproject.toml` & `open_source_insights_api-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-source-insights-api"
-version = "0.1.8"
+version = "0.1.9"
 license = "MIT"
 description = "Library to consume project Open Source Insights Project from Google"
 authors = ["Cristiano Henrique <cristianovisk@gmail.com>"]
 readme = "README.md"
 packages = [{include = "open_source_insights_api"}]
 classifiers = [
     "Topic :: Internet",
```

### Comparing `open_source_insights_api-0.1.8/PKG-INFO` & `open_source_insights_api-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-source-insights-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library to consume project Open Source Insights Project from Google
 License: MIT
 Author: Cristiano Henrique
 Author-email: cristianovisk@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

