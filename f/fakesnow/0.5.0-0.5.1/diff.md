# Comparing `tmp/fakesnow-0.5.0.tar.gz` & `tmp/fakesnow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.5.0.tar", last modified: Sun Jul 23 12:35:59 2023, max compression
+gzip compressed data, was "fakesnow-0.5.1.tar", last modified: Mon Jul 24 12:09:47 2023, max compression
```

## Comparing `fakesnow-0.5.0.tar` & `fakesnow-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:35:59.002342 fakesnow-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-23 12:35:48.000000 fakesnow-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-23 12:35:48.000000 fakesnow-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-23 12:35:59.002342 fakesnow-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-23 12:35:48.000000 fakesnow-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:35:58.998342 fakesnow-0.5.0/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-23 12:35:48.000000 fakesnow-0.5.0/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-23 12:35:48.000000 fakesnow-0.5.0/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-23 12:35:48.000000 fakesnow-0.5.0/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-07-23 12:35:48.000000 fakesnow-0.5.0/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-23 12:35:48.000000 fakesnow-0.5.0/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-23 12:35:48.000000 fakesnow-0.5.0/fakesnow/info_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-23 12:35:48.000000 fakesnow-0.5.0/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-07-23 12:35:48.000000 fakesnow-0.5.0/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:35:58.998342 fakesnow-0.5.0/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-23 12:35:58.000000 fakesnow-0.5.0/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-23 12:35:58.000000 fakesnow-0.5.0/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 12:35:58.000000 fakesnow-0.5.0/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-23 12:35:58.000000 fakesnow-0.5.0/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-23 12:35:58.000000 fakesnow-0.5.0/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-23 12:35:48.000000 fakesnow-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 12:35:59.002342 fakesnow-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-23 12:35:48.000000 fakesnow-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:35:59.002342 fakesnow-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-23 12:35:48.000000 fakesnow-0.5.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-23 12:35:48.000000 fakesnow-0.5.0/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30651 2023-07-23 12:35:48.000000 fakesnow-0.5.0/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-23 12:35:48.000000 fakesnow-0.5.0/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-23 12:35:48.000000 fakesnow-0.5.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:09:47.344260 fakesnow-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 12:09:40.000000 fakesnow-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 12:09:40.000000 fakesnow-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-24 12:09:47.344260 fakesnow-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-24 12:09:40.000000 fakesnow-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:09:47.340260 fakesnow-0.5.1/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-24 12:09:40.000000 fakesnow-0.5.1/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-24 12:09:40.000000 fakesnow-0.5.1/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 12:09:40.000000 fakesnow-0.5.1/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-07-24 12:09:40.000000 fakesnow-0.5.1/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-24 12:09:40.000000 fakesnow-0.5.1/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-24 12:09:40.000000 fakesnow-0.5.1/fakesnow/info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-24 12:09:40.000000 fakesnow-0.5.1/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-07-24 12:09:40.000000 fakesnow-0.5.1/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:09:47.340260 fakesnow-0.5.1/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-24 12:09:47.000000 fakesnow-0.5.1/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 12:09:47.000000 fakesnow-0.5.1/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:09:47.000000 fakesnow-0.5.1/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-24 12:09:47.000000 fakesnow-0.5.1/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 12:09:47.000000 fakesnow-0.5.1/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-24 12:09:40.000000 fakesnow-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:09:47.344260 fakesnow-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 12:09:40.000000 fakesnow-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:09:47.344260 fakesnow-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-24 12:09:40.000000 fakesnow-0.5.1/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 12:09:40.000000 fakesnow-0.5.1/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31365 2023-07-24 12:09:40.000000 fakesnow-0.5.1/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-24 12:09:40.000000 fakesnow-0.5.1/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-24 12:09:40.000000 fakesnow-0.5.1/tests/test_transforms.py
```

### Comparing `fakesnow-0.5.0/LICENSE` & `fakesnow-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/PKG-INFO` & `fakesnow-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `fakesnow-0.5.0/README.md` & `fakesnow-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/fakesnow/__init__.py` & `fakesnow-0.5.1/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/fakesnow/checks.py` & `fakesnow-0.5.1/fakesnow/checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/fakesnow/expr.py` & `fakesnow-0.5.1/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/fakesnow/fakes.py` & `fakesnow-0.5.1/fakesnow/fakes.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 
     @staticmethod
     def _describe_as_result_metadata(describe_results: list) -> list[ResultMetadata]:
         # fmt: off
         def as_result_metadata(column_name: str, column_type: str, _: str) -> ResultMetadata:
             # see https://docs.snowflake.com/en/user-guide/python-connector-api.html#type-codes
             # and https://arrow.apache.org/docs/python/api/datatypes.html#type-checking
-            if column_type == "BIGINT":
+            if column_type in {"BIGINT", "INTEGER"}:
                 return ResultMetadata(
                     name=column_name, type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True               # noqa: E501
                 )
             elif column_type.startswith("DECIMAL"):
                 match = re.search(r'\((\d+),(\d+)\)', column_type)
                 if match:
                     precision = int(match[1])
```

### Comparing `fakesnow-0.5.0/fakesnow/info_schema.py` & `fakesnow-0.5.1/fakesnow/info_schema.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/fakesnow/transforms.py` & `fakesnow-0.5.1/fakesnow/transforms.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.5.1/fakesnow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `fakesnow-0.5.0/pyproject.toml` & `fakesnow-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run Snowflake DB locally."
-version = "0.5.0"
+version = "0.5.1"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
     "duckdb~=0.8.0",
```

### Comparing `fakesnow-0.5.0/tests/test_checks.py` & `fakesnow-0.5.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/tests/test_expr.py` & `fakesnow-0.5.1/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/tests/test_fakes.py` & `fakesnow-0.5.1/tests/test_fakes.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,14 +230,28 @@
 
     # test with params
     assert cur.describe("select * from example where XNUMBER = ?", (1,)) == expected_metadata
     cur.execute("select * from example where XNUMBER = ?", (1,))
     assert cur.description == expected_metadata
 
 
+def test_describe_info_schema(cur: snowflake.connector.cursor.SnowflakeCursor):
+    # tests we can handle the column types returned from the info schema, which are created by duckdb
+    # and so don't go through our transforms
+    cur.execute("select column_name, ordinal_position from information_schema.columns")
+    # fmt: off
+    expected_metadata = [
+        ResultMetadata(name='column_name', type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True),
+        ResultMetadata(name='ordinal_position', type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True)
+    ]
+    # fmt: on
+
+    assert cur.description == expected_metadata
+
+
 def test_executemany(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
 
     customers = [(1, "Jenny", "P"), (2, "Jasper", "M")]
     cur.executemany("insert into customers (id, first_name, last_name) values (%s,%s,%s)", customers)
 
     cur.execute("select id, first_name, last_name from customers")
```

### Comparing `fakesnow-0.5.0/tests/test_patch.py` & `fakesnow-0.5.1/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.5.0/tests/test_transforms.py` & `fakesnow-0.5.1/tests/test_transforms.py`

 * *Files identical despite different names*

