# Comparing `tmp/task3-0.1.0.tar.gz` & `tmp/task3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task3-0.1.0.tar", max compression
+gzip compressed data, was "task3-0.1.1.tar", max compression
```

## Comparing `task3-0.1.0.tar` & `task3-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task3-0.1.0/LICENSE
--rw-r--r--   0        0        0      300 2023-07-21 16:40:54.009144 task3-0.1.0/parse_xsv/__init__.py
--rw-r--r--   0        0        0      116 2023-07-12 14:27:57.699438 task3-0.1.0/parse_xsv/__main__.py
--rw-r--r--   0        0        0       23 2023-07-11 20:06:54.477708 task3-0.1.0/parse_xsv/__version__.py
--rw-r--r--   0        0        0      187 2023-07-23 21:21:28.183243 task3-0.1.0/parse_xsv/cli/__init__.py
--rw-r--r--   0        0        0      116 2023-07-12 14:27:57.680442 task3-0.1.0/parse_xsv/cli/__main__.py
--rw-r--r--   0        0        0    17417 2023-07-24 17:14:55.584168 task3-0.1.0/parse_xsv/cli/cli.py
--rw-r--r--   0        0        0    12448 2023-07-23 23:52:42.080268 task3-0.1.0/parse_xsv/parse_xsv.py
--rw-r--r--   0        0        0      113 2023-07-15 09:18:39.572916 task3-0.1.0/parse_xsv/sample_gen/__init__.py
--rw-r--r--   0        0        0      143 2023-07-15 09:18:39.582913 task3-0.1.0/parse_xsv/sample_gen/__main__.py
--rw-r--r--   0        0        0     8102 2023-07-24 12:33:10.476335 task3-0.1.0/parse_xsv/sample_gen/sample_gen.py
--rw-r--r--   0        0        0       97 2023-07-12 14:27:57.666460 task3-0.1.0/parse_xsv/showcase/__init__.py
--rw-r--r--   0        0        0      138 2023-07-12 14:27:57.687500 task3-0.1.0/parse_xsv/showcase/__main__.py
--rw-r--r--   0        0        0    25805 2023-07-24 17:03:10.652441 task3-0.1.0/parse_xsv/showcase/corrupted_sample.csv
--rw-r--r--   0        0        0    29527 2023-07-24 15:54:36.768020 task3-0.1.0/parse_xsv/showcase/sample.csv
--rw-r--r--   0        0        0    29527 2023-07-24 16:01:30.014978 task3-0.1.0/parse_xsv/showcase/sample.tsv
--rw-r--r--   0        0        0    22643 2023-07-24 17:06:10.126642 task3-0.1.0/parse_xsv/showcase/showcase.py
--rw-r--r--   0        0        0      563 2023-07-24 18:37:23.151104 task3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    17428 2023-07-11 12:14:12.015389 task3-0.1.0/README.md
--rw-r--r--   0        0        0    17619 1970-01-01 00:00:00.000000 task3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task3-0.1.1/LICENSE
+-rw-r--r--   0        0        0      300 2023-07-21 16:40:54.009144 task3-0.1.1/parse_xsv/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-12 14:27:57.699438 task3-0.1.1/parse_xsv/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-24 18:49:07.842637 task3-0.1.1/parse_xsv/__version__.py
+-rw-r--r--   0        0        0      187 2023-07-23 21:21:28.183243 task3-0.1.1/parse_xsv/cli/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-12 14:27:57.680442 task3-0.1.1/parse_xsv/cli/__main__.py
+-rw-r--r--   0        0        0    17417 2023-07-24 17:14:55.584168 task3-0.1.1/parse_xsv/cli/cli.py
+-rw-r--r--   0        0        0    12448 2023-07-23 23:52:42.080268 task3-0.1.1/parse_xsv/parse_xsv.py
+-rw-r--r--   0        0        0      113 2023-07-15 09:18:39.572916 task3-0.1.1/parse_xsv/sample_gen/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-15 09:18:39.582913 task3-0.1.1/parse_xsv/sample_gen/__main__.py
+-rw-r--r--   0        0        0     8102 2023-07-24 12:33:10.476335 task3-0.1.1/parse_xsv/sample_gen/sample_gen.py
+-rw-r--r--   0        0        0       97 2023-07-12 14:27:57.666460 task3-0.1.1/parse_xsv/showcase/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-12 14:27:57.687500 task3-0.1.1/parse_xsv/showcase/__main__.py
+-rw-r--r--   0        0        0    25805 2023-07-24 17:03:10.652441 task3-0.1.1/parse_xsv/showcase/corrupted_sample.csv
+-rw-r--r--   0        0        0    29527 2023-07-24 15:54:36.768020 task3-0.1.1/parse_xsv/showcase/sample.csv
+-rw-r--r--   0        0        0    29527 2023-07-24 16:01:30.014978 task3-0.1.1/parse_xsv/showcase/sample.tsv
+-rw-r--r--   0        0        0    22643 2023-07-24 17:06:10.126642 task3-0.1.1/parse_xsv/showcase/showcase.py
+-rw-r--r--   0        0        0      577 2023-07-24 18:49:07.847642 task3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    17428 2023-07-11 12:14:12.015389 task3-0.1.1/README.md
+-rw-r--r--   0        0        0    17733 1970-01-01 00:00:00.000000 task3-0.1.1/PKG-INFO
```

### Comparing `task3-0.1.0/parse_xsv/cli/cli.py` & `task3-0.1.1/parse_xsv/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task3-0.1.0/parse_xsv/parse_xsv.py` & `task3-0.1.1/parse_xsv/parse_xsv.py`

 * *Files identical despite different names*

### Comparing `task3-0.1.0/parse_xsv/sample_gen/sample_gen.py` & `task3-0.1.1/parse_xsv/sample_gen/sample_gen.py`

 * *Files identical despite different names*

### Comparing `task3-0.1.0/parse_xsv/showcase/corrupted_sample.csv` & `task3-0.1.1/parse_xsv/showcase/corrupted_sample.csv`

 * *Files identical despite different names*

### Comparing `task3-0.1.0/parse_xsv/showcase/sample.csv` & `task3-0.1.1/parse_xsv/showcase/sample.csv`

 * *Files identical despite different names*

### Comparing `task3-0.1.0/parse_xsv/showcase/sample.tsv` & `task3-0.1.1/parse_xsv/showcase/sample.tsv`

 * *Files identical despite different names*

### Comparing `task3-0.1.0/parse_xsv/showcase/showcase.py` & `task3-0.1.1/parse_xsv/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task3-0.1.0/pyproject.toml` & `task3-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "task3"
-version = "0.1.0"
-description = "Regex xSV parser"
+version = "0.1.1"
+description = "xSV file parser CLI and library"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "parse_xsv"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 questionary = "^1.10.0"
 faker = "^19.2.0"
 
 [tool.poetry.scripts]
 parse_xsv = "parse_xsv:parse_cli"
 parse_xsv_showcase = "parse_xsv.showcase:parse_showcase"
 xsv_sample_gen = "parse_xsv.sample_gen:generate_sample_data"
```

### Comparing `task3-0.1.0/README.md` & `task3-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `task3-0.1.0/PKG-INFO` & `task3-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: task3
-Version: 0.1.0
-Summary: Regex xSV parser
+Version: 0.1.1
+Summary: xSV file parser CLI and library
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=19.2.0,<20.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: task3 Version: 0.1.0 Summary: Regex xSV parser
-Author: Bill.Avramenko Author-email: billavramenko@gmail.com Requires-Python:
->=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: faker (>=19.2.0,<20.0.0) Requires-Dist:
-questionary (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: task3 Version: 0.1.1 Summary: xSV file parser CLI
+and library Author: Bill.Avramenko Author-email: billavramenko@gmail.com
+Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: faker
+(>=19.2.0,<20.0.0) Requires-Dist: questionary (>=1.10.0,<2.0.0) Description-
+Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                        Parsing xSV with Regex in Python.
                          Module 2: Python. Task 3A+B.
                    [TASK_3]  [License]  [POETRY]  [PYTHON] 
 ## Preface This project contains a solution to one of the tasks of the EPAM
 DevOps Initial Internal Training Course #7 in 2023. Detailed information about
 the course, as well as reports on each of the completed tasks (including this
```

