# Comparing `tmp/pykli-0.0.1.tar.gz` & `tmp/pykli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykli-0.0.1.tar", max compression
+gzip compressed data, was "pykli-1.0.0.tar", max compression
```

## Comparing `pykli-0.0.1.tar` & `pykli-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-07-24 15:46:13.892886 pykli-0.0.1/LICENSE
--rw-r--r--   0        0        0     1166 2023-07-24 15:46:13.892886 pykli-0.0.1/README.md
--rw-r--r--   0        0        0      549 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/__init__.py
--rw-r--r--   0        0        0     1081 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/__main__.py
--rw-r--r--   0        0        0     2402 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/completer.py
--rw-r--r--   0        0        0     1145 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/keybindgings.py
--rw-r--r--   0        0        0     1792 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/ksqldb.py
--rw-r--r--   0        0        0     2097 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/repl_eval.py
--rw-r--r--   0        0        0     9044 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/repl_print.py
--rw-r--r--   0        0        0     3291 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/repl_read.py
--rw-r--r--   0        0        0      960 2023-07-24 15:46:13.896886 pykli-0.0.1/pykli/tokens.py
--rw-r--r--   0        0        0      773 2023-07-24 15:46:13.896886 pykli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 pykli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-24 16:15:12.686440 pykli-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1166 2023-07-24 16:15:12.686440 pykli-1.0.0/README.md
+-rw-r--r--   0        0        0      549 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/__init__.py
+-rw-r--r--   0        0        0     1122 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/__main__.py
+-rw-r--r--   0        0        0     2402 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/completer.py
+-rw-r--r--   0        0        0     1145 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/keybindgings.py
+-rw-r--r--   0        0        0     1792 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/ksqldb.py
+-rw-r--r--   0        0        0     2097 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/repl_eval.py
+-rw-r--r--   0        0        0     9044 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/repl_print.py
+-rw-r--r--   0        0        0     3291 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/repl_read.py
+-rw-r--r--   0        0        0      960 2023-07-24 16:15:12.686440 pykli-1.0.0/pykli/tokens.py
+-rw-r--r--   0        0        0     1011 2023-07-24 16:15:12.686440 pykli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2071 1970-01-01 00:00:00.000000 pykli-1.0.0/PKG-INFO
```

### Comparing `pykli-0.0.1/LICENSE` & `pykli-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/README.md` & `pykli-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pykli/__init__.py` & `pykli-1.0.0/pykli/__init__.py`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pykli/__main__.py` & `pykli-1.0.0/pykli/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .tokens import Info, ErrMsg, initialize_sqlparse
 
 
 @click.command()
 @click.option('-f', '--file', help="execute commands from file, then exit",
     type=click.Path(exists=True, path_type=pathlib.Path))
 @click.argument("server", default = "http://localhost:8088")
+@click.version_option(prog_name="pyKLI")
 def main(server, file):
     """
     pyKLI - ksqlDB command line client.
 
     \b SERVER The address of the ksqlDB server."""
 
     LOG.info(f"pyKLI started: server={server}, file={file}")
```

### Comparing `pykli-0.0.1/pykli/completer.py` & `pykli-1.0.0/pykli/completer.py`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pykli/keybindgings.py` & `pykli-1.0.0/pykli/keybindgings.py`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pykli/ksqldb.py` & `pykli-1.0.0/pykli/ksqldb.py`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pykli/repl_eval.py` & `pykli-1.0.0/pykli/repl_eval.py`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pykli/repl_print.py` & `pykli-1.0.0/pykli/repl_print.py`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pykli/repl_read.py` & `pykli-1.0.0/pykli/repl_read.py`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pykli/tokens.py` & `pykli-1.0.0/pykli/tokens.py`

 * *Files identical despite different names*

### Comparing `pykli-0.0.1/pyproject.toml` & `pykli-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [tool.poetry]
-name = "pykli"
-version = "0.0.1"
-description = "ksqlDB command line client"
+name = "pyKLI"
+version = "1.0.0"
+description = "Interactive ksqlDB command line client with autocompletion and syntax highlighting"
+license = "MIT"
 authors = ["Ievgenii Shepeliuk <eshepelyuk@gmail.com>"]
 readme = "README.md"
+homepage = "https://github.com/eshepelyuk/pykli"
+repository = "https://github.com/eshepelyuk/pykli"
+keywords = ["cli", "kafka", "tui", "confluent", "ksql", "ksqldb"]
 packages = [{include = "pykli"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 click = "^8.1.3"
 prompt-toolkit = "^3.0.38"
 pygments = "^2.15.1"
```

### Comparing `pykli-0.0.1/PKG-INFO` & `pykli-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: pykli
-Version: 0.0.1
-Summary: ksqlDB command line client
+Version: 1.0.0
+Summary: Interactive ksqlDB command line client with autocompletion and syntax highlighting
+Home-page: https://github.com/eshepelyuk/pykli
+License: MIT
+Keywords: cli,kafka,tui,confluent,ksql,ksqldb
 Author: Ievgenii Shepeliuk
 Author-email: eshepelyuk@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cli_helpers[styles] (>=2.3.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx[http2] (>=0.24.1,<0.25.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
 Requires-Dist: xdg-base-dirs (>=6.0.0,<7.0.0)
+Project-URL: Repository, https://github.com/eshepelyuk/pykli
 Description-Content-Type: text/markdown
 
 # pyKLI
 
 Interactive [ksqlDB](https://ksqldb.io/) command line client
 with autocompletion and syntax highlighting written in Python.
```

