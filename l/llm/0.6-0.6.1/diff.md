# Comparing `tmp/llm-0.6.tar.gz` & `tmp/llm-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-0.6.tar", last modified: Tue Jul 18 21:39:17 2023, max compression
+gzip compressed data, was "llm-0.6.1.tar", last modified: Mon Jul 24 15:56:20 2023, max compression
```

## Comparing `llm-0.6.tar` & `llm-0.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:39:17.208360 llm-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 21:39:01.000000 llm-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 21:39:01.000000 llm-0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-18 21:39:17.208360 llm-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-18 21:39:01.000000 llm-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:39:17.204360 llm-0.6/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-18 21:39:01.000000 llm-0.6/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 21:39:01.000000 llm-0.6/llm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-07-18 21:39:01.000000 llm-0.6/llm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:39:17.208360 llm-0.6/llm/default_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:39:01.000000 llm-0.6/llm/default_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-18 21:39:01.000000 llm-0.6/llm/default_plugins/openai_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-18 21:39:01.000000 llm-0.6/llm/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 21:39:01.000000 llm-0.6/llm/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-18 21:39:01.000000 llm-0.6/llm/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-18 21:39:01.000000 llm-0.6/llm/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-18 21:39:01.000000 llm-0.6/llm/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-18 21:39:01.000000 llm-0.6/llm/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-18 21:39:01.000000 llm-0.6/llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:39:17.208360 llm-0.6/llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-18 21:39:17.000000 llm-0.6/llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-18 21:39:17.000000 llm-0.6/llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:39:17.000000 llm-0.6/llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 21:39:17.000000 llm-0.6/llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-18 21:39:17.000000 llm-0.6/llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 21:39:17.000000 llm-0.6/llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:39:17.208360 llm-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-18 21:39:01.000000 llm-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:56:20.928866 llm-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 15:55:58.000000 llm-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 15:55:58.000000 llm-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-24 15:56:20.928866 llm-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-24 15:55:58.000000 llm-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:56:20.924866 llm-0.6.1/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-24 15:55:58.000000 llm-0.6.1/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 15:55:58.000000 llm-0.6.1/llm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-07-24 15:55:58.000000 llm-0.6.1/llm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:56:20.928866 llm-0.6.1/llm/default_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:55:58.000000 llm-0.6.1/llm/default_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-24 15:55:58.000000 llm-0.6.1/llm/default_plugins/openai_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-24 15:55:58.000000 llm-0.6.1/llm/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-24 15:55:58.000000 llm-0.6.1/llm/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-24 15:55:58.000000 llm-0.6.1/llm/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-24 15:55:58.000000 llm-0.6.1/llm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-24 15:55:58.000000 llm-0.6.1/llm/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-24 15:55:58.000000 llm-0.6.1/llm/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 15:55:58.000000 llm-0.6.1/llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:56:20.928866 llm-0.6.1/llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-24 15:56:20.000000 llm-0.6.1/llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-24 15:56:20.000000 llm-0.6.1/llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:56:20.000000 llm-0.6.1/llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 15:56:20.000000 llm-0.6.1/llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-24 15:56:20.000000 llm-0.6.1/llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 15:56:20.000000 llm-0.6.1/llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:56:20.928866 llm-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-24 15:55:58.000000 llm-0.6.1/setup.py
```

### Comparing `llm-0.6/LICENSE` & `llm-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-0.6/PKG-INFO` & `llm-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm
-Version: 0.6
+Version: 0.6.1
 Summary: A CLI utility and Python library for interacting with Large Language Models, including OpenAI, PaLM and local models installed on your own machine.
 Home-page: https://github.com/simonw/llm
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://llm.datasette.io/
 Project-URL: Issues, https://github.com/simonw/llm/issues
 Project-URL: CI, https://github.com/simonw/llm/actions
@@ -34,17 +34,17 @@
 
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install llm
 ```
-Or using [Homebrew](https://brew.sh/) (much slower):
+Or using [Homebrew](https://brew.sh/):
 ```bash
-brew install simonw/llm/llm
+brew install llm
 ```
 [Detailed installation instructions](https://llm.datasette.io/en/stable/setup.html).
 
 ## Getting started
 
 If you have an [OpenAI API key](https://platform.openai.com/account/api-keys) you can get started using the OpenAI models right away.
```

### Comparing `llm-0.6/README.md` & `llm-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install llm
 ```
-Or using [Homebrew](https://brew.sh/) (much slower):
+Or using [Homebrew](https://brew.sh/):
 ```bash
-brew install simonw/llm/llm
+brew install llm
 ```
 [Detailed installation instructions](https://llm.datasette.io/en/stable/setup.html).
 
 ## Getting started
 
 If you have an [OpenAI API key](https://platform.openai.com/account/api-keys) you can get started using the OpenAI models right away.
```

### Comparing `llm-0.6/llm/__init__.py` & `llm-0.6.1/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-0.6/llm/cli.py` & `llm-0.6.1/llm/cli.py`

 * *Files identical despite different names*

### Comparing `llm-0.6/llm/default_plugins/openai_models.py` & `llm-0.6.1/llm/default_plugins/openai_models.py`

 * *Files identical despite different names*

### Comparing `llm-0.6/llm/migrations.py` & `llm-0.6.1/llm/migrations.py`

 * *Files identical despite different names*

### Comparing `llm-0.6/llm/models.py` & `llm-0.6.1/llm/models.py`

 * *Files identical despite different names*

### Comparing `llm-0.6/llm/templates.py` & `llm-0.6.1/llm/templates.py`

 * *Files identical despite different names*

### Comparing `llm-0.6/llm/utils.py` & `llm-0.6.1/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm-0.6/llm.egg-info/PKG-INFO` & `llm-0.6.1/llm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm
-Version: 0.6
+Version: 0.6.1
 Summary: A CLI utility and Python library for interacting with Large Language Models, including OpenAI, PaLM and local models installed on your own machine.
 Home-page: https://github.com/simonw/llm
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://llm.datasette.io/
 Project-URL: Issues, https://github.com/simonw/llm/issues
 Project-URL: CI, https://github.com/simonw/llm/actions
@@ -34,17 +34,17 @@
 
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install llm
 ```
-Or using [Homebrew](https://brew.sh/) (much slower):
+Or using [Homebrew](https://brew.sh/):
 ```bash
-brew install simonw/llm/llm
+brew install llm
 ```
 [Detailed installation instructions](https://llm.datasette.io/en/stable/setup.html).
 
 ## Getting started
 
 If you have an [OpenAI API key](https://platform.openai.com/account/api-keys) you can get started using the OpenAI models right away.
```

### Comparing `llm-0.6/setup.py` & `llm-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = "0.6"
+VERSION = "0.6.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

