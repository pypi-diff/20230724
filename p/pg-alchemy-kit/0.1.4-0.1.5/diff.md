# Comparing `tmp/pg_alchemy_kit-0.1.4.tar.gz` & `tmp/pg_alchemy_kit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_alchemy_kit-0.1.4.tar", max compression
+gzip compressed data, was "pg_alchemy_kit-0.1.5.tar", max compression
```

## Comparing `pg_alchemy_kit-0.1.4.tar` & `pg_alchemy_kit-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685000 pg_alchemy_kit-0.1.4/README.md
--rw-r--r--   0        0        0     2315 2023-07-24 18:38:24.966281 pg_alchemy_kit-0.1.4/pg_alchemy_kit/PG.py
--rw-r--r--   0        0        0     6073 2023-07-24 18:39:48.162003 pg_alchemy_kit-0.1.4/pg_alchemy_kit/PGUtils.py
--rw-r--r--   0        0        0      138 2023-07-23 04:57:39.246000 pg_alchemy_kit-0.1.4/pg_alchemy_kit/__init__.py
--rw-r--r--   0        0        0      496 2023-07-24 18:45:21.557415 pg_alchemy_kit-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5850 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685538 pg_alchemy_kit-0.1.5/README.md
+-rw-r--r--   0        0        0     2315 2023-07-24 18:38:24.966000 pg_alchemy_kit-0.1.5/pg_alchemy_kit/PG.py
+-rw-r--r--   0        0        0     6073 2023-07-24 18:39:48.162000 pg_alchemy_kit-0.1.5/pg_alchemy_kit/PGUtils.py
+-rw-r--r--   0        0        0      138 2023-07-23 04:57:39.246037 pg_alchemy_kit-0.1.5/pg_alchemy_kit/__init__.py
+-rw-r--r--   0        0        0      495 2023-07-24 21:26:44.208953 pg_alchemy_kit-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5899 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.1.5/PKG-INFO
```

### Comparing `pg_alchemy_kit-0.1.4/README.md` & `pg_alchemy_kit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.1.4/pg_alchemy_kit/PG.py` & `pg_alchemy_kit-0.1.5/pg_alchemy_kit/PG.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.1.4/pg_alchemy_kit/PGUtils.py` & `pg_alchemy_kit-0.1.5/pg_alchemy_kit/PGUtils.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.1.4/PKG-INFO` & `pg_alchemy_kit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pg-alchemy-kit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple wrapper around sqlalchemy to make it easier to use with postgresql
 Home-page: https://github.com/jsaied99/pg-alchemy-kit
 Author: jsaied99
 Author-email: jsaied99@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Project-URL: Repository, https://github.com/jsaied99/pg-alchemy-kit
 Description-Content-Type: text/markdown
```

