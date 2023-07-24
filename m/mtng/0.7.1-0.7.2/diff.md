# Comparing `tmp/mtng-0.7.1.tar.gz` & `tmp/mtng-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtng-0.7.1.tar", max compression
+gzip compressed data, was "mtng-0.7.2.tar", max compression
```

## Comparing `mtng-0.7.1.tar` & `mtng-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4820 2022-08-17 22:41:45.505290 mtng-0.7.1/README.md
--rw-r--r--   0        0        0      820 2023-07-12 09:44:20.462283 mtng-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       83 2022-08-11 10:46:06.387500 mtng-0.7.1/src/mtng/__init__.py
--rw-r--r--   0        0        0     6969 2023-07-12 09:28:26.387984 mtng-0.7.1/src/mtng/cli.py
--rw-r--r--   0        0        0     8250 2023-07-12 09:34:45.825269 mtng-0.7.1/src/mtng/collect.py
--rw-r--r--   0        0        0     1142 2023-07-12 09:04:23.800414 mtng-0.7.1/src/mtng/generate.py
--rw-r--r--   0        0        0     2244 2023-03-28 15:15:27.386088 mtng-0.7.1/src/mtng/spec.py
--rw-r--r--   0        0        0      437 2022-09-02 13:42:43.975478 mtng-0.7.1/src/mtng/template/base.tex
--rw-r--r--   0        0        0      119 2023-04-17 15:46:15.937707 mtng-0.7.1/src/mtng/template/item.tex
--rw-r--r--   0        0        0      261 2022-08-17 22:45:29.877915 mtng-0.7.1/src/mtng/template/item_context.tex
--rw-r--r--   0        0        0     2532 2023-04-17 15:59:47.711725 mtng-0.7.1/src/mtng/template/macros.tex
--rw-r--r--   0        0        0      725 2022-08-17 22:45:29.878621 mtng-0.7.1/src/mtng/template/main.tex
--rw-r--r--   0        0        0     3299 2022-09-02 13:55:37.778106 mtng-0.7.1/src/mtng/template/preamble.tex
--rw-r--r--   0        0        0      386 2022-09-02 13:54:57.808639 mtng-0.7.1/src/mtng/template/provides.tex
--rw-r--r--   0        0        0     3423 2023-07-12 09:04:23.800655 mtng-0.7.1/src/mtng/template/repo.tex
--rw-r--r--   0        0        0     5852 1970-01-01 00:00:00.000000 mtng-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     4820 2022-08-17 22:41:45.505290 mtng-0.7.2/README.md
+-rw-r--r--   0        0        0      820 2023-07-24 07:30:34.130095 mtng-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0       83 2022-08-11 10:46:06.387500 mtng-0.7.2/src/mtng/__init__.py
+-rw-r--r--   0        0        0     6969 2023-07-12 09:28:26.387984 mtng-0.7.2/src/mtng/cli.py
+-rw-r--r--   0        0        0     8250 2023-07-12 09:34:45.825269 mtng-0.7.2/src/mtng/collect.py
+-rw-r--r--   0        0        0     1142 2023-07-12 09:04:23.800414 mtng-0.7.2/src/mtng/generate.py
+-rw-r--r--   0        0        0     2244 2023-03-28 15:15:27.386088 mtng-0.7.2/src/mtng/spec.py
+-rw-r--r--   0        0        0      437 2022-09-02 13:42:43.975478 mtng-0.7.2/src/mtng/template/base.tex
+-rw-r--r--   0        0        0      119 2023-04-17 15:46:15.937707 mtng-0.7.2/src/mtng/template/item.tex
+-rw-r--r--   0        0        0      261 2022-08-17 22:45:29.877915 mtng-0.7.2/src/mtng/template/item_context.tex
+-rw-r--r--   0        0        0     2532 2023-04-17 15:59:47.711725 mtng-0.7.2/src/mtng/template/macros.tex
+-rw-r--r--   0        0        0      725 2022-08-17 22:45:29.878621 mtng-0.7.2/src/mtng/template/main.tex
+-rw-r--r--   0        0        0     3299 2022-09-02 13:55:37.778106 mtng-0.7.2/src/mtng/template/preamble.tex
+-rw-r--r--   0        0        0      386 2022-09-02 13:54:57.808639 mtng-0.7.2/src/mtng/template/provides.tex
+-rw-r--r--   0        0        0     3423 2023-07-12 09:04:23.800655 mtng-0.7.2/src/mtng/template/repo.tex
+-rw-r--r--   0        0        0     5852 1970-01-01 00:00:00.000000 mtng-0.7.2/PKG-INFO
```

### Comparing `mtng-0.7.1/README.md` & `mtng-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/pyproject.toml` & `mtng-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mtng"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 packages = [
 { include = "mtng", from = "src" },
 ]
 readme = "README.md"
 
@@ -17,15 +17,15 @@
 Jinja2 = "^3.1.1"
 requests = "^2.25.1"
 typer = "^0.6.1"
 python-dateutil = "^2.8.1"
 aiohttp = "^3.7.4"
 gidgethub = "^5.0.1"
 pydantic = "^1.8.2"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.1"
 pytest-asyncio = "^0.19.0"
 pytest-dotenv = "^0.5.2"
 appdirs = "^1.4.4"
 diskcache = "^5.4.0"
 rich = "^13.4.2"
 
 [tool.poetry.scripts]
```

### Comparing `mtng-0.7.1/src/mtng/cli.py` & `mtng-0.7.2/src/mtng/cli.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/src/mtng/collect.py` & `mtng-0.7.2/src/mtng/collect.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/src/mtng/generate.py` & `mtng-0.7.2/src/mtng/generate.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/src/mtng/spec.py` & `mtng-0.7.2/src/mtng/spec.py`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/src/mtng/template/macros.tex` & `mtng-0.7.2/src/mtng/template/macros.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/src/mtng/template/main.tex` & `mtng-0.7.2/src/mtng/template/main.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/src/mtng/template/preamble.tex` & `mtng-0.7.2/src/mtng/template/preamble.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/src/mtng/template/repo.tex` & `mtng-0.7.2/src/mtng/template/repo.tex`

 * *Files identical despite different names*

### Comparing `mtng-0.7.1/PKG-INFO` & `mtng-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mtng
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.1,<4.0.0)
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: diskcache (>=5.4.0,<6.0.0)
 Requires-Dist: gidgethub (>=5.0.1,<6.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pytest-asyncio (>=0.19.0,<0.20.0)
 Requires-Dist: pytest-dotenv (>=0.5.2,<0.6.0)
```

