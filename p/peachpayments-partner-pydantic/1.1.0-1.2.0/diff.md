# Comparing `tmp/peachpayments_partner_pydantic-1.1.0.tar.gz` & `tmp/peachpayments_partner_pydantic-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachpayments_partner_pydantic-1.1.0.tar", max compression
+gzip compressed data, was "peachpayments_partner_pydantic-1.2.0.tar", max compression
```

## Comparing `peachpayments_partner_pydantic-1.1.0.tar` & `peachpayments_partner_pydantic-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3087 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/README.md
--rw-r--r--   0        0        0       36 2023-05-12 07:07:24.502190 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/__init__.py
--rw-r--r--   0        0        0     3277 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/exception_handlers.py
--rw-r--r--   0        0        0     2793 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/helpers.py
--rw-r--r--   0        0        0     7973 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/inbound_schemas.py
--rw-r--r--   0        0        0    22033 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/outbound_schemas.py
--rw-r--r--   0        0        0     7762 2023-05-09 09:33:40.737809 peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/schemas.py
--rw-r--r--   0        0        0     1507 2023-05-12 13:13:40.533687 peachpayments_partner_pydantic-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 peachpayments_partner_pydantic-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-24 12:15:04.685238 peachpayments_partner_pydantic-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3087 2023-07-24 12:15:04.685238 peachpayments_partner_pydantic-1.2.0/README.md
+-rw-r--r--   0        0        0       36 2023-07-24 12:15:04.685238 peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/__init__.py
+-rw-r--r--   0        0        0     3277 2023-07-24 12:15:04.685238 peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/exception_handlers.py
+-rw-r--r--   0        0        0     2793 2023-07-24 12:15:04.685238 peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/helpers.py
+-rw-r--r--   0        0        0     7973 2023-07-24 12:15:04.685238 peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/inbound_schemas.py
+-rw-r--r--   0        0        0    22033 2023-07-24 12:15:04.689238 peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/outbound_schemas.py
+-rw-r--r--   0        0        0     7762 2023-07-24 12:15:04.689238 peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/schemas.py
+-rw-r--r--   0        0        0     1507 2023-07-24 12:15:04.689238 peachpayments_partner_pydantic-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 peachpayments_partner_pydantic-1.2.0/PKG-INFO
```

### Comparing `peachpayments_partner_pydantic-1.1.0/LICENSE.txt` & `peachpayments_partner_pydantic-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-1.1.0/README.md` & `peachpayments_partner_pydantic-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/exception_handlers.py` & `peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/helpers.py` & `peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/helpers.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/inbound_schemas.py` & `peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/inbound_schemas.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/outbound_schemas.py` & `peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/outbound_schemas.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-1.1.0/peachpayments_partner_pydantic/schemas.py` & `peachpayments_partner_pydantic-1.2.0/peachpayments_partner_pydantic/schemas.py`

 * *Files identical despite different names*

### Comparing `peachpayments_partner_pydantic-1.1.0/pyproject.toml` & `peachpayments_partner_pydantic-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peachpayments-partner-pydantic"
-version = "1.1.0"
+version = "1.2.0"
 description = "PeachPayments Partner Pydantic library contains Pydantic schemas to help integrate PeachPayments with their partners."
 readme = "README.md"
 license = "MIT"
 authors = ["PeachPayments <support@peachpayments.com>"]
 repository = "https://gitlab.com/peachpayments/peachpayments-partner-pydantic/"
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -18,15 +18,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ipaddress = "^1.0.23"
 pydantic = "^1.9.1"
 iso4217 = "^1.9.20220401"
 email-validator = "^1.2.1"
-peachpayments-partner = "^0.1.11"
+peachpayments-partner = "^0.1.12"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 autoflake = "^1.4"
 pydocstyle = "^6.1.1"
 ipaddress = "^1.0.23"
 python-dateutil = "^2.8.2"
```

### Comparing `peachpayments_partner_pydantic-1.1.0/PKG-INFO` & `peachpayments_partner_pydantic-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachpayments-partner-pydantic
-Version: 1.1.0
+Version: 1.2.0
 Summary: PeachPayments Partner Pydantic library contains Pydantic schemas to help integrate PeachPayments with their partners.
 Home-page: https://gitlab.com/peachpayments/peachpayments-partner-pydantic/
 License: MIT
 Author: PeachPayments
 Author-email: support@peachpayments.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: email-validator (>=1.2.1,<2.0.0)
 Requires-Dist: ipaddress (>=1.0.23,<2.0.0)
 Requires-Dist: iso4217 (>=1.9.20220401,<2.0.0)
-Requires-Dist: peachpayments-partner (>=0.1.11,<0.2.0)
+Requires-Dist: peachpayments-partner (>=0.1.12,<0.2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Repository, https://gitlab.com/peachpayments/peachpayments-partner-pydantic/
 Description-Content-Type: text/markdown
 
 # PeachPayments Partner Pydantic Library
 
 ## Overview
```

