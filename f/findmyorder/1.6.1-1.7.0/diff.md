# Comparing `tmp/findmyorder-1.6.1.tar.gz` & `tmp/findmyorder-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.6.1.tar", max compression
+gzip compressed data, was "findmyorder-1.7.0.tar", max compression
```

## Comparing `findmyorder-1.6.1.tar` & `findmyorder-1.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-20 14:52:48.244794 findmyorder-1.6.1/LICENSE
--rw-r--r--   0        0        0     3022 2023-07-20 14:52:48.244794 findmyorder-1.6.1/README.md
--rw-r--r--   0        0        0      113 2023-07-20 14:52:57.316883 findmyorder-1.6.1/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-07-20 14:52:48.244794 findmyorder-1.6.1/findmyorder/config.py
--rw-r--r--   0        0        0     3221 2023-07-20 14:52:48.244794 findmyorder-1.6.1/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5903 2023-07-20 14:52:48.244794 findmyorder-1.6.1/findmyorder/main.py
--rw-r--r--   0        0        0     2959 2023-07-20 14:52:57.308883 findmyorder-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 findmyorder-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 11:13:37.828631 findmyorder-1.7.0/LICENSE
+-rw-r--r--   0        0        0     3022 2023-07-24 11:13:37.828631 findmyorder-1.7.0/README.md
+-rw-r--r--   0        0        0      113 2023-07-24 11:13:41.748626 findmyorder-1.7.0/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-24 11:13:37.828631 findmyorder-1.7.0/findmyorder/config.py
+-rw-r--r--   0        0        0     3221 2023-07-24 11:13:37.828631 findmyorder-1.7.0/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5931 2023-07-24 11:13:37.828631 findmyorder-1.7.0/findmyorder/main.py
+-rw-r--r--   0        0        0     2977 2023-07-24 11:13:41.740626 findmyorder-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 findmyorder-1.7.0/PKG-INFO
```

### Comparing `findmyorder-1.6.1/LICENSE` & `findmyorder-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.6.1/README.md` & `findmyorder-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.6.1/findmyorder/config.py` & `findmyorder-1.7.0/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.6.1/findmyorder/default_settings.toml` & `findmyorder-1.7.0/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.6.1/findmyorder/main.py` & `findmyorder-1.7.0/findmyorder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
  FindMyOrder Main
 """
-import logging
 from datetime import datetime
 
 import emoji
+from loguru import logger
 from pyparsing import (
     Combine,
     Optional,
     Suppress,
     Word,
     alphas,
     nums,
@@ -23,15 +23,16 @@
 
 class FindMyOrder:
     """find an order class """
 
     def __init__(
         self,
     ):
-        self.logger = logging.getLogger(name="FMO")
+        self.logger = logger
+        # logging.getLogger(name="FMO")
 
     async def search(
         self,
         my_string: str,
     ) -> bool:
         """Search an order."""
         if my_string:
```

### Comparing `findmyorder-1.6.1/pyproject.toml` & `findmyorder-1.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.6.1"
+version = "1.7.0"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -21,21 +21,22 @@
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
+loguru = "^0.7.0"
 pyparsing = "^3.0.9"
 emoji = "^2.5.1"
 
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^8.0.2"
-ruff = "^0.0.278"
+ruff = "^0.0.280"
 
 [tool.ruff]
 select = [
   "E",  # pycodestyle
   "F",  # pyflakes
   "I",  # isort
 ]
```

### Comparing `findmyorder-1.6.1/PKG-INFO` & `findmyorder-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.6.1
+Version: 1.7.0
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: emoji (>=2.5.1,<3.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
 <table style="border: 1px solid transparent">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.6.1 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.7.0 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
-(>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist:
-pyparsing (>=3.0.9,<4.0.0) Project-URL: Changelog, https://github.com/mraniki/
-findmyorder/blob/dev/CHANGELOG.rst Project-URL: Issues, https://github.com/
-mraniki/findmyorder/issues Project-URL: Support, https://github.com/mraniki/
-findmyorder/discussions Description-Content-Type: text/markdown
+(>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist: loguru
+(>=0.7.0,<0.8.0) Requires-Dist: pyparsing (>=3.0.9,<4.0.0) Project-URL:
+Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
+Project-URL: Issues, https://github.com/mraniki/findmyorder/issues Project-URL:
+Support, https://github.com/mraniki/findmyorder/discussions Description-
+Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white]
 [https://img.shields.io/badge/github-
 %23000000.svg?style=for-the-
 badge&logo=github&logoColor=white] [https://img.shields.io/
 docker/pulls/mraniki/tt?style=for-the-badge]                        [Logo]
 [https://img.shields.io/badge/tips-000000?style=for-the-
```

