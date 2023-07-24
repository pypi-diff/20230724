# Comparing `tmp/openai_functools-1.0.80.tar.gz` & `tmp/openai_functools-1.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-1.0.80.tar", max compression
+gzip compressed data, was "openai_functools-1.0.81.tar", max compression
```

## Comparing `openai_functools-1.0.80.tar` & `openai_functools-1.0.81.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-24 13:55:55.974800 openai_functools-1.0.80/LICENSE
--rw-r--r--   0        0        0     6875 2023-07-24 13:55:55.974800 openai_functools-1.0.80/README.md
--rw-r--r--   0        0        0      342 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/__init__.py
--rw-r--r--   0        0        0      240 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/function_spec.py
--rw-r--r--   0        0        0     3825 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/functions_orchestrator.py
--rw-r--r--   0        0        0     1755 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/types.py
--rw-r--r--   0        0        0       69 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-07-24 13:56:23.580437 openai_functools-1.0.80/pyproject.toml
--rw-r--r--   0        0        0     7575 1970-01-01 00:00:00.000000 openai_functools-1.0.80/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-24 14:02:10.107602 openai_functools-1.0.81/LICENSE
+-rw-r--r--   0        0        0     6964 2023-07-24 14:02:10.107602 openai_functools-1.0.81/README.md
+-rw-r--r--   0        0        0      342 2023-07-24 14:02:10.123602 openai_functools-1.0.81/openai_functools/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-24 14:02:10.127602 openai_functools-1.0.81/openai_functools/function_spec.py
+-rw-r--r--   0        0        0     3825 2023-07-24 14:02:10.127602 openai_functools-1.0.81/openai_functools/functions_orchestrator.py
+-rw-r--r--   0        0        0     1755 2023-07-24 14:02:10.127602 openai_functools-1.0.81/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-24 14:02:10.127602 openai_functools-1.0.81/openai_functools/types.py
+-rw-r--r--   0        0        0       69 2023-07-24 14:02:10.127602 openai_functools-1.0.81/openai_functools/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-07-24 14:02:39.503575 openai_functools-1.0.81/pyproject.toml
+-rw-r--r--   0        0        0     7664 1970-01-01 00:00:00.000000 openai_functools-1.0.81/PKG-INFO
```

### Comparing `openai_functools-1.0.80/LICENSE` & `openai_functools-1.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.80/README.md` & `openai_functools-1.0.81/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # [openai-functools](https://github.com/Jakob-98/openai-functools)
 
 `openai-functools` is a Python library designed to enhance the functionality of OpenAI's `gpt-3.5-turbo-0613` and `gpt-4-0613` models for function calling. This library focuses on generating the required JSON/dictionary/metadata automatically by wrapping existing Python functions in our decorator. This removes the need for you to manually create and manage the JSON structures required for function calling in these models.
 
 ## Why openai-functools
 
-![example](./example.png)
+![example](https://github.com/Jakob-98/openai-functools/blob/7641fd5d34beca9c1b690d06cd18e40fde6a2a49/example.png)
 
 ## Installation
 
 This package is hosted on PyPI and can be installed with pip:
 
 ```sh
 pip install openai-functools
```

### Comparing `openai_functools-1.0.80/openai_functools/functions_orchestrator.py` & `openai_functools-1.0.81/openai_functools/functions_orchestrator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.80/openai_functools/metadata_generator.py` & `openai_functools-1.0.81/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-1.0.80/pyproject.toml` & `openai_functools-1.0.81/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai_functools"
-version = "1.0.80"
+version = "1.0.81"
 description = "python openai functions tooling"
 authors = ["Jakob Serlier <37184788+Jakob-98@users.noreply.github.com>", "Marc van Duyn <codingkitties@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_functools"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `openai_functools-1.0.80/PKG-INFO` & `openai_functools-1.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functools
-Version: 1.0.80
+Version: 1.0.81
 Summary: python openai functions tooling
 Author: Jakob Serlier
 Author-email: 37184788+Jakob-98@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 
 # [openai-functools](https://github.com/Jakob-98/openai-functools)
 
 `openai-functools` is a Python library designed to enhance the functionality of OpenAI's `gpt-3.5-turbo-0613` and `gpt-4-0613` models for function calling. This library focuses on generating the required JSON/dictionary/metadata automatically by wrapping existing Python functions in our decorator. This removes the need for you to manually create and manage the JSON structures required for function calling in these models.
 
 ## Why openai-functools
 
-![example](./example.png)
+![example](https://github.com/Jakob-98/openai-functools/blob/7641fd5d34beca9c1b690d06cd18e40fde6a2a49/example.png)
 
 ## Installation
 
 This package is hosted on PyPI and can be installed with pip:
 
 ```sh
 pip install openai-functools
```

