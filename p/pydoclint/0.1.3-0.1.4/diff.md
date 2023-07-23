# Comparing `tmp/pydoclint-0.1.3.tar.gz` & `tmp/pydoclint-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.1.3.tar", last modified: Fri Jul 21 22:08:33 2023, max compression
+gzip compressed data, was "pydoclint-0.1.4.tar", last modified: Sun Jul 23 23:13:37 2023, max compression
```

## Comparing `pydoclint-0.1.3.tar` & `pydoclint-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.794436 pydoclint-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-21 22:08:21.000000 pydoclint-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-21 22:08:33.794436 pydoclint-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-21 22:08:21.000000 pydoclint-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.790436 pydoclint-0.1.3/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.794436 pydoclint-0.1.3/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/return_anno.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/return_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    24031 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.794436 pydoclint-0.1.3/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-21 22:08:33.794436 pydoclint-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 22:08:21.000000 pydoclint-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.794436 pydoclint-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-21 22:08:21.000000 pydoclint-0.1.3/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-21 22:08:21.000000 pydoclint-0.1.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 22:08:21.000000 pydoclint-0.1.3/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:13:37.602824 pydoclint-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-23 23:13:26.000000 pydoclint-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-23 23:13:37.602824 pydoclint-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-23 23:13:26.000000 pydoclint-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:13:37.598824 pydoclint-0.1.4/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:13:37.598824 pydoclint-0.1.4/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/return_anno.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/return_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24031 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:13:37.598824 pydoclint-0.1.4/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-23 23:13:37.000000 pydoclint-0.1.4/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-23 23:13:37.000000 pydoclint-0.1.4/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 23:13:37.000000 pydoclint-0.1.4/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-23 23:13:37.000000 pydoclint-0.1.4/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-23 23:13:37.000000 pydoclint-0.1.4/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-23 23:13:37.000000 pydoclint-0.1.4/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-23 23:13:26.000000 pydoclint-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-23 23:13:37.602824 pydoclint-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-23 23:13:26.000000 pydoclint-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 23:13:37.602824 pydoclint-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-23 23:13:26.000000 pydoclint-0.1.4/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-23 23:13:26.000000 pydoclint-0.1.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-23 23:13:26.000000 pydoclint-0.1.4/tests/test_parse_config.py
```

### Comparing `pydoclint-0.1.3/LICENSE` & `pydoclint-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/flake8_entry.py` & `pydoclint-0.1.4/pydoclint/flake8_entry.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/main.py` & `pydoclint-0.1.4/pydoclint/main.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/parse_config.py` & `pydoclint-0.1.4/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/annotation.py` & `pydoclint-0.1.4/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/arg.py` & `pydoclint-0.1.4/pydoclint/utils/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/astTypes.py` & `pydoclint-0.1.4/pydoclint/utils/astTypes.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/doc.py` & `pydoclint-0.1.4/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/generic.py` & `pydoclint-0.1.4/pydoclint/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/return_anno.py` & `pydoclint-0.1.4/pydoclint/utils/return_anno.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.1.4/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/unparser.py` & `pydoclint-0.1.4/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/violation.py` & `pydoclint-0.1.4/pydoclint/utils/violation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/utils/walk.py` & `pydoclint-0.1.4/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint/visitor.py` & `pydoclint-0.1.4/pydoclint/visitor.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.1.4/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/setup.cfg` & `pydoclint-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.1.3
+version = 0.1.4
 description = A Python docstring linter that checks arguments, returns, yields, and raises sections
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.1.3/tests/test_generic.py` & `pydoclint-0.1.4/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/tests/test_main.py` & `pydoclint-0.1.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.3/tests/test_parse_config.py` & `pydoclint-0.1.4/tests/test_parse_config.py`

 * *Files identical despite different names*

