# Comparing `tmp/gearsllm-0.1.1.tar.gz` & `tmp/gearsllm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gearsllm-0.1.1.tar", max compression
+gzip compressed data, was "gearsllm-0.1.2.tar", max compression
```

## Comparing `gearsllm-0.1.1.tar` & `gearsllm-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.1/LICENSE
--rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.1/README.md
--rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.1/gears/__init__.py
--rw-r--r--   0        0        0     1978 2023-07-23 22:17:21.560333 gearsllm-0.1.1/gears/gear.py
--rw-r--r--   0        0        0     2635 2023-07-23 22:27:24.108862 gearsllm-0.1.1/gears/history.py
--rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.1/gears/llms/__init__.py
--rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.1/gears/llms/base.py
--rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.1/gears/llms/echo.py
--rw-r--r--   0        0        0     3680 2023-07-23 22:17:24.315177 gearsllm-0.1.1/gears/llms/oai.py
--rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.1/gears/utils.py
--rw-r--r--   0        0        0      538 2023-07-23 22:50:43.095676 gearsllm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 gearsllm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.2/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.2/README.md
+-rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.2/gears/__init__.py
+-rw-r--r--   0        0        0     1978 2023-07-23 22:17:21.560333 gearsllm-0.1.2/gears/gear.py
+-rw-r--r--   0        0        0     2635 2023-07-23 22:27:24.108862 gearsllm-0.1.2/gears/history.py
+-rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.2/gears/llms/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.2/gears/llms/base.py
+-rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.2/gears/llms/echo.py
+-rw-r--r--   0        0        0     3680 2023-07-23 22:17:24.315177 gearsllm-0.1.2/gears/llms/oai.py
+-rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.2/gears/utils.py
+-rw-r--r--   0        0        0      538 2023-07-23 22:54:40.396544 gearsllm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 gearsllm-0.1.2/PKG-INFO
```

### Comparing `gearsllm-0.1.1/LICENSE` & `gearsllm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.1/gears/gear.py` & `gearsllm-0.1.2/gears/gear.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.1/gears/history.py` & `gearsllm-0.1.2/gears/history.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.1/gears/llms/echo.py` & `gearsllm-0.1.2/gears/llms/echo.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.1/gears/llms/oai.py` & `gearsllm-0.1.2/gears/llms/oai.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.1/gears/utils.py` & `gearsllm-0.1.2/gears/utils.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.1/pyproject.toml` & `gearsllm-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gearsllm"
-version = "0.1.1"
+version = "0.1.2"
 description = "Lightweight library for building LLM-based control flow."
 authors = ["Shreya Shankar <ss.shankar505@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gears"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gearsllm-0.1.1/PKG-INFO` & `gearsllm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearsllm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lightweight library for building LLM-based control flow.
 License: MIT
 Author: Shreya Shankar
 Author-email: ss.shankar505@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

