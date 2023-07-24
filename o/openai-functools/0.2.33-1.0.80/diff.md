# Comparing `tmp/openai_functools-0.2.33.tar.gz` & `tmp/openai_functools-1.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functools-0.2.33.tar", max compression
+gzip compressed data, was "openai_functools-1.0.80.tar", max compression
```

## Comparing `openai_functools-0.2.33.tar` & `openai_functools-1.0.80.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-23 08:39:00.924455 openai_functools-0.2.33/LICENSE
--rw-r--r--   0        0        0     3916 2023-07-23 08:39:00.924455 openai_functools-0.2.33/README.md
--rw-r--r--   0        0        0      195 2023-07-23 08:39:00.928455 openai_functools-0.2.33/openai_functools/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-23 08:39:00.928455 openai_functools-0.2.33/openai_functools/metadata_generator.py
--rw-r--r--   0        0        0      470 2023-07-23 08:39:00.928455 openai_functools-0.2.33/openai_functools/types.py
--rw-r--r--   0        0        0     2318 2023-07-23 08:39:00.928455 openai_functools-0.2.33/openai_functools/utils/openai_service.py
--rw-r--r--   0        0        0      537 2023-07-23 08:39:30.412744 openai_functools-0.2.33/pyproject.toml
--rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 openai_functools-0.2.33/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-24 13:55:55.974800 openai_functools-1.0.80/LICENSE
+-rw-r--r--   0        0        0     6875 2023-07-24 13:55:55.974800 openai_functools-1.0.80/README.md
+-rw-r--r--   0        0        0      342 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/function_spec.py
+-rw-r--r--   0        0        0     3825 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/functions_orchestrator.py
+-rw-r--r--   0        0        0     1755 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/metadata_generator.py
+-rw-r--r--   0        0        0      470 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/types.py
+-rw-r--r--   0        0        0       69 2023-07-24 13:55:55.994801 openai_functools-1.0.80/openai_functools/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-07-24 13:56:23.580437 openai_functools-1.0.80/pyproject.toml
+-rw-r--r--   0        0        0     7575 1970-01-01 00:00:00.000000 openai_functools-1.0.80/PKG-INFO
```

### Comparing `openai_functools-0.2.33/LICENSE` & `openai_functools-1.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.33/openai_functools/metadata_generator.py` & `openai_functools-1.0.80/openai_functools/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `openai_functools-0.2.33/pyproject.toml` & `openai_functools-1.0.80/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "openai_functools"
-version = "0.2.33"
+version = "1.0.80"
 description = "python openai functions tooling"
 authors = ["Jakob Serlier <37184788+Jakob-98@users.noreply.github.com>", "Marc van Duyn <codingkitties@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_functools"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8.1"
 openai = "^0.27.8"
 pytest = "^7.4.0"
 flake8 = "^6.0.0"
 black = "^23.7.0"
 isort = "^5.12.0"
 docstring-parser = "^0.15"
```

