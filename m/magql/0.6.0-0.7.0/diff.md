# Comparing `tmp/magql-0.6.0.tar.gz` & `tmp/magql-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magql-0.6.0.tar", last modified: Thu Jul 22 19:24:22 2021, max compression
+gzip compressed data, was "magql-0.7.0.tar", last modified: Tue Aug 23 01:37:51 2022, max compression
```

## Comparing `magql-0.6.0.tar` & `magql-0.7.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2021-07-22 19:24:22.335738 magql-0.6.0/
--rw-r--r--   0 david     (1000) david     (1000)     1143 2021-07-22 19:22:49.000000 magql-0.6.0/CHANGES.rst
--rw-r--r--   0 david     (1000) david     (1000)     1485 2020-09-05 14:38:36.000000 magql-0.6.0/LICENSE.rst
--rw-r--r--   0 david     (1000) david     (1000)      155 2021-07-22 19:24:03.000000 magql-0.6.0/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      908 2021-07-22 19:24:22.335738 magql-0.6.0/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      607 2020-09-05 14:38:36.000000 magql-0.6.0/README.rst
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2021-07-22 19:24:22.332405 magql-0.6.0/docs/
--rw-r--r--   0 david     (1000) david     (1000)      603 2020-09-05 14:38:36.000000 magql-0.6.0/docs/Makefile
--rw-r--r--   0 david     (1000) david     (1000)      960 2020-09-05 14:38:36.000000 magql-0.6.0/docs/conf.py
--rw-r--r--   0 david     (1000) david     (1000)       57 2020-09-05 14:38:36.000000 magql-0.6.0/docs/convert.rst
--rw-r--r--   0 david     (1000) david     (1000)      239 2020-09-05 14:38:36.000000 magql-0.6.0/docs/get_type.rst
--rw-r--r--   0 david     (1000) david     (1000)      267 2020-09-05 14:38:36.000000 magql-0.6.0/docs/index.rst
--rw-r--r--   0 david     (1000) david     (1000)      773 2020-09-05 14:38:36.000000 magql-0.6.0/docs/make.bat
--rw-r--r--   0 david     (1000) david     (1000)      712 2020-09-05 14:38:36.000000 magql-0.6.0/docs/resolvers.rst
--rw-r--r--   0 david     (1000) david     (1000)      563 2020-09-05 14:38:36.000000 magql-0.6.0/noxfile.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2021-07-22 19:24:22.332405 magql-0.6.0/requirements/
--rw-r--r--   0 david     (1000) david     (1000)     2212 2021-07-14 16:05:50.000000 magql-0.6.0/requirements/dev.txt
--rw-r--r--   0 david     (1000) david     (1000)     1407 2021-06-08 15:13:27.000000 magql-0.6.0/requirements/docs.txt
--rw-r--r--   0 david     (1000) david     (1000)      445 2021-06-08 15:13:27.000000 magql-0.6.0/requirements/tests.txt
--rw-r--r--   0 david     (1000) david     (1000)     1313 2021-07-22 19:24:22.335738 magql-0.6.0/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      278 2020-09-05 14:38:36.000000 magql-0.6.0/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2021-07-22 19:24:22.332405 magql-0.6.0/src/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2021-07-22 19:24:22.332405 magql-0.6.0/src/magql/
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-09-05 14:38:36.000000 magql-0.6.0/src/magql/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     7011 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/convert.py
--rw-r--r--   0 david     (1000) david     (1000)    10917 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/definitions.py
--rw-r--r--   0 david     (1000) david     (1000)      448 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/errors.py
--rw-r--r--   0 david     (1000) david     (1000)     8490 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/filter.py
--rw-r--r--   0 david     (1000) david     (1000)      644 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/flask_magql.py
--rw-r--r--   0 david     (1000) david     (1000)     2745 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/flask_magql_utils.py
--rw-r--r--   0 david     (1000) david     (1000)    18331 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/manager.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2021-07-22 19:21:28.000000 magql-0.6.0/src/magql/py.typed
--rw-r--r--   0 david     (1000) david     (1000)    27551 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/resolver_factory.py
--rw-r--r--   0 david     (1000) david     (1000)     1152 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/sort.py
--rw-r--r--   0 david     (1000) david     (1000)     6273 2021-07-14 16:05:50.000000 magql-0.6.0/src/magql/type.py
--rw-r--r--   0 david     (1000) david     (1000)     4788 2021-07-22 19:15:53.000000 magql-0.6.0/src/magql/validation.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2021-07-22 19:24:22.332405 magql-0.6.0/src/magql.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      908 2021-07-22 19:24:22.000000 magql-0.6.0/src/magql.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      859 2021-07-22 19:24:22.000000 magql-0.6.0/src/magql.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2021-07-22 19:24:22.000000 magql-0.6.0/src/magql.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       71 2021-07-22 19:24:22.000000 magql-0.6.0/src/magql.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        6 2021-07-22 19:24:22.000000 magql-0.6.0/src/magql.egg-info/top_level.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2021-07-22 19:24:22.335738 magql-0.6.0/tests/
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-09-05 14:38:36.000000 magql-0.6.0/tests/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     6060 2020-09-05 14:38:36.000000 magql-0.6.0/tests/conftest.py
--rw-r--r--   0 david     (1000) david     (1000)     3892 2020-09-05 14:38:36.000000 magql-0.6.0/tests/test_convert.py
--rw-r--r--   0 david     (1000) david     (1000)     1324 2020-09-05 14:38:36.000000 magql-0.6.0/tests/test_get_types.py
--rw-r--r--   0 david     (1000) david     (1000)    10496 2020-09-05 14:38:36.000000 magql-0.6.0/tests/test_manager.py
--rw-r--r--   0 david     (1000) david     (1000)     3052 2020-09-05 14:38:36.000000 magql-0.6.0/tests/test_resolvers.py
--rw-r--r--   0 david     (1000) david     (1000)     2029 2020-09-05 14:38:36.000000 magql-0.6.0/tests/test_schema.py
+drwxrwxr-x   0 jdavis    (1000) jdavis    (1000)        0 2022-08-23 01:37:51.313980 magql-0.7.0/
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     1281 2022-08-23 01:33:44.000000 magql-0.7.0/CHANGES.rst
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     1485 2022-06-09 18:22:37.000000 magql-0.7.0/LICENSE.rst
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      155 2022-06-09 18:22:37.000000 magql-0.7.0/MANIFEST.in
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      888 2022-08-23 01:37:51.313980 magql-0.7.0/PKG-INFO
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      607 2022-06-09 18:22:37.000000 magql-0.7.0/README.rst
+drwxrwxr-x   0 jdavis    (1000) jdavis    (1000)        0 2022-08-23 01:37:51.309980 magql-0.7.0/docs/
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      603 2022-06-09 18:22:37.000000 magql-0.7.0/docs/Makefile
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      960 2022-06-09 18:22:37.000000 magql-0.7.0/docs/conf.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)       57 2022-06-09 18:22:37.000000 magql-0.7.0/docs/convert.rst
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      239 2022-06-09 18:22:37.000000 magql-0.7.0/docs/get_type.rst
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      267 2022-06-09 18:22:37.000000 magql-0.7.0/docs/index.rst
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      773 2022-06-09 18:22:37.000000 magql-0.7.0/docs/make.bat
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      712 2022-06-09 18:22:37.000000 magql-0.7.0/docs/resolvers.rst
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      563 2022-06-09 18:22:37.000000 magql-0.7.0/noxfile.py
+drwxrwxr-x   0 jdavis    (1000) jdavis    (1000)        0 2022-08-23 01:37:51.309980 magql-0.7.0/requirements/
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     2212 2022-06-09 18:22:37.000000 magql-0.7.0/requirements/dev.txt
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     1407 2022-06-09 18:22:37.000000 magql-0.7.0/requirements/docs.txt
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      445 2022-06-09 18:22:37.000000 magql-0.7.0/requirements/tests.txt
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     1313 2022-08-23 01:37:51.313980 magql-0.7.0/setup.cfg
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      278 2022-06-09 18:22:37.000000 magql-0.7.0/setup.py
+drwxrwxr-x   0 jdavis    (1000) jdavis    (1000)        0 2022-08-23 01:37:51.305979 magql-0.7.0/src/
+drwxrwxr-x   0 jdavis    (1000) jdavis    (1000)        0 2022-08-23 01:37:51.309980 magql-0.7.0/src/magql/
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)        0 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/__init__.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     7011 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/convert.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)    10917 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/definitions.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      448 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/errors.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     8539 2022-08-23 01:33:44.000000 magql-0.7.0/src/magql/filter.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      644 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/flask_magql.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     2745 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/flask_magql_utils.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)    18331 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/manager.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)        0 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/py.typed
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)    27551 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/resolver_factory.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     1152 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/sort.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     6273 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/type.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     4788 2022-06-09 18:22:37.000000 magql-0.7.0/src/magql/validation.py
+drwxrwxr-x   0 jdavis    (1000) jdavis    (1000)        0 2022-08-23 01:37:51.313980 magql-0.7.0/src/magql.egg-info/
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      888 2022-08-23 01:37:51.000000 magql-0.7.0/src/magql.egg-info/PKG-INFO
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)      859 2022-08-23 01:37:51.000000 magql-0.7.0/src/magql.egg-info/SOURCES.txt
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)        1 2022-08-23 01:37:51.000000 magql-0.7.0/src/magql.egg-info/dependency_links.txt
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)       71 2022-08-23 01:37:51.000000 magql-0.7.0/src/magql.egg-info/requires.txt
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)        6 2022-08-23 01:37:51.000000 magql-0.7.0/src/magql.egg-info/top_level.txt
+drwxrwxr-x   0 jdavis    (1000) jdavis    (1000)        0 2022-08-23 01:37:51.313980 magql-0.7.0/tests/
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)        0 2022-06-09 18:22:37.000000 magql-0.7.0/tests/__init__.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     6060 2022-06-09 18:22:37.000000 magql-0.7.0/tests/conftest.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     3892 2022-06-09 18:22:37.000000 magql-0.7.0/tests/test_convert.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     1324 2022-06-09 18:22:37.000000 magql-0.7.0/tests/test_get_types.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)    10496 2022-06-09 18:22:37.000000 magql-0.7.0/tests/test_manager.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     3052 2022-06-09 18:22:37.000000 magql-0.7.0/tests/test_resolvers.py
+-rw-rw-r--   0 jdavis    (1000) jdavis    (1000)     2029 2022-06-09 18:22:37.000000 magql-0.7.0/tests/test_schema.py
```

### Comparing `magql-0.6.0/CHANGES.rst` & `magql-0.7.0/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+v0.7.0
+------
+
+Released 2022-08-22
+
+- Update the INCLUDES filter operator to be case-insensitive
+- Make EQUALS operator case insensitive
+
 v0.6.0
 ------
 
 Released 2021-07-22
 
 -   Add static typing annotations.
 -   Added validation helpers from autoinvent-example.
```

### Comparing `magql-0.6.0/LICENSE.rst` & `magql-0.7.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/PKG-INFO` & `magql-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: magql
-Version: 0.6.0
+Version: 0.7.0
 Summary: The magical GraphQL framework that generates an API for your data.
 Home-page: https://github.com/autoinvent/magql
 License: BSD-3-Clause
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 
 magql
 =====
 
@@ -28,9 +27,7 @@
     -   Update any set of fields.
     -   Delete, with "check delete" query to return affected related objects.
 
 -   Discrete, overridable steps instead of a single resolve function.
 -   Input validation and error messages per field.
 
 .. _GraphQL: https://graphql.org/
-
-
```

### Comparing `magql-0.6.0/README.rst` & `magql-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/docs/Makefile` & `magql-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/docs/conf.py` & `magql-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/docs/make.bat` & `magql-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/docs/resolvers.rst` & `magql-0.7.0/docs/resolvers.rst`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/noxfile.py` & `magql-0.7.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/requirements/dev.txt` & `magql-0.7.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/requirements/docs.txt` & `magql-0.7.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/setup.cfg` & `magql-0.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = magql
-version = 0.6.0
+version = 0.7.0
 url = https://github.com/autoinvent/magql
 license = BSD-3-Clause
 license_file = LICENSE.rst
 description = The magical GraphQL framework that generates an API for your data.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

### Comparing `magql-0.6.0/src/magql/convert.py` & `magql-0.7.0/src/magql/convert.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql/definitions.py` & `magql-0.7.0/src/magql/definitions.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql/filter.py` & `magql-0.7.0/src/magql/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from inflection import underscore
 from sqlalchemy import Date
 from sqlalchemy import DateTime
 from sqlalchemy import Text
 from sqlalchemy import Time
 from sqlalchemy import Unicode
 from sqlalchemy import UnicodeText
+from sqlalchemy import func
 from sqlalchemy.orm import RelationshipProperty
 from sqlalchemy.types import Boolean
 from sqlalchemy.types import Float
 from sqlalchemy.types import Integer
 from sqlalchemy.types import Numeric
 from sqlalchemy.types import String
 from sqlalchemy.types import VARCHAR
@@ -191,17 +192,17 @@
 @get_filter_comparator.register(EmailType)
 @get_filter_comparator.register(Time)
 @get_filter_comparator.register(String)
 @get_filter_comparator.register(VARCHAR)
 def _get_string_comparator(_: t.Any) -> t.Callable:
     def condition(filter_value: t.Any, filter_operator: str, field: t.Any) -> t.Any:
         if filter_operator == "INCLUDES":
-            return field.like(f"%{filter_value}%")
+            return field.ilike(f"%{filter_value}%")
         elif filter_operator == "EQUALS":
-            return field == filter_value
+            return func.lower(field) == filter_value.lower()
         elif filter_operator == "EXISTS":
             return field.like("%")
         elif filter_operator == "DOESNOTEXIST":
             return field.is_(None)
 
     return condition
```

### Comparing `magql-0.6.0/src/magql/flask_magql.py` & `magql-0.7.0/src/magql/flask_magql.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql/flask_magql_utils.py` & `magql-0.7.0/src/magql/flask_magql_utils.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql/manager.py` & `magql-0.7.0/src/magql/manager.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql/resolver_factory.py` & `magql-0.7.0/src/magql/resolver_factory.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql/sort.py` & `magql-0.7.0/src/magql/sort.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql/type.py` & `magql-0.7.0/src/magql/type.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql/validation.py` & `magql-0.7.0/src/magql/validation.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/src/magql.egg-info/PKG-INFO` & `magql-0.7.0/src/magql.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: magql
-Version: 0.6.0
+Version: 0.7.0
 Summary: The magical GraphQL framework that generates an API for your data.
 Home-page: https://github.com/autoinvent/magql
 License: BSD-3-Clause
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 
 magql
 =====
 
@@ -28,9 +27,7 @@
     -   Update any set of fields.
     -   Delete, with "check delete" query to return affected related objects.
 
 -   Discrete, overridable steps instead of a single resolve function.
 -   Input validation and error messages per field.
 
 .. _GraphQL: https://graphql.org/
-
-
```

### Comparing `magql-0.6.0/src/magql.egg-info/SOURCES.txt` & `magql-0.7.0/src/magql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/tests/conftest.py` & `magql-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/tests/test_convert.py` & `magql-0.7.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/tests/test_get_types.py` & `magql-0.7.0/tests/test_get_types.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/tests/test_manager.py` & `magql-0.7.0/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/tests/test_resolvers.py` & `magql-0.7.0/tests/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `magql-0.6.0/tests/test_schema.py` & `magql-0.7.0/tests/test_schema.py`

 * *Files identical despite different names*

