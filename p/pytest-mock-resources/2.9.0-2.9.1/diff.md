# Comparing `tmp/pytest_mock_resources-2.9.0.tar.gz` & `tmp/pytest_mock_resources-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_mock_resources-2.9.0.tar", max compression
+gzip compressed data, was "pytest_mock_resources-2.9.1.tar", max compression
```

## Comparing `pytest_mock_resources-2.9.0.tar` & `pytest_mock_resources-2.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    15315 2023-07-12 20:13:38.614969 pytest_mock_resources-2.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1053 2023-07-12 20:13:38.614969 pytest_mock_resources-2.9.0/LICENSE
--rw-r--r--   0        0        0     5549 2023-07-12 20:13:38.614969 pytest_mock_resources-2.9.0/README.md
--rw-r--r--   0        0        0     3848 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     1792 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/__init__.py
--rw-r--r--   0        0        0     1305 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/action.py
--rw-r--r--   0        0        0     2174 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/cli.py
--rw-r--r--   0        0        0     1867 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/__init__.py
--rw-r--r--   0        0        0      822 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/import_.py
--rw-r--r--   0        0        0      923 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/sqlalchemy.py
--rw-r--r--   0        0        0     3013 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/config.py
--rw-r--r--   0        0        0      622 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/__init__.py
--rw-r--r--   0        0        0     6429 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/base.py
--rw-r--r--   0        0        0     1702 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/mongo.py
--rw-r--r--   0        0        0     1399 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/moto.py
--rw-r--r--   0        0        0     2792 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/mysql.py
--rw-r--r--   0        0        0     3713 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/postgres.py
--rw-r--r--   0        0        0     1369 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/redis.py
--rw-r--r--   0        0        0     1569 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/redshift.py
--rw-r--r--   0        0        0     3070 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/credentials.py
--rw-r--r--   0        0        0     1436 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/__init__.py
--rw-r--r--   0        0        0      951 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/base.py
--rw-r--r--   0        0        0     2364 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/mongo.py
--rw-r--r--   0        0        0      416 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/__init__.py
--rw-r--r--   0        0        0     1960 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/action.py
--rw-r--r--   0        0        0     5013 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/base.py
--rw-r--r--   0        0        0     3417 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/mysql.py
--rw-r--r--   0        0        0    11153 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/postgresql.py
--rw-r--r--   0        0        0     2713 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redis.py
--rw-r--r--   0        0        0     4659 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redshift/__init__.py
--rw-r--r--   0        0        0     4939 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redshift/udf.py
--rw-r--r--   0        0        0     9051 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/sqlite.py
--rw-r--r--   0        0        0     3813 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/hooks.py
--rw-r--r--   0        0        0        0 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/__init__.py
--rw-r--r--   0        0        0     7056 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py
--rw-r--r--   0        0        0     7290 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py
--rw-r--r--   0        0        0     2486 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/psycopg2.py
--rw-r--r--   0        0        0     2905 2023-07-12 20:13:38.622969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-07-12 20:13:38.622969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/py.typed
--rw-r--r--   0        0        0    10215 2023-07-12 20:13:38.622969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/sqlalchemy.py
--rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 pytest_mock_resources-2.9.0/setup.py
--rw-r--r--   0        0        0     7821 1970-01-01 00:00:00.000000 pytest_mock_resources-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0    15315 2023-07-24 19:47:37.849882 pytest_mock_resources-2.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1053 2023-07-24 19:47:37.849882 pytest_mock_resources-2.9.1/LICENSE
+-rw-r--r--   0        0        0     5549 2023-07-24 19:47:37.849882 pytest_mock_resources-2.9.1/README.md
+-rw-r--r--   0        0        0     3848 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1792 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/__init__.py
+-rw-r--r--   0        0        0     1305 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/action.py
+-rw-r--r--   0        0        0     2174 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/cli.py
+-rw-r--r--   0        0        0     1867 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/compat/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/compat/import_.py
+-rw-r--r--   0        0        0      923 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/compat/sqlalchemy.py
+-rw-r--r--   0        0        0     3013 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/config.py
+-rw-r--r--   0        0        0      622 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/__init__.py
+-rw-r--r--   0        0        0     6429 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/base.py
+-rw-r--r--   0        0        0     1702 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/mongo.py
+-rw-r--r--   0        0        0     1399 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/moto.py
+-rw-r--r--   0        0        0     2792 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/mysql.py
+-rw-r--r--   0        0        0     3713 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/postgres.py
+-rw-r--r--   0        0        0     1369 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/redis.py
+-rw-r--r--   0        0        0     1569 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/redshift.py
+-rw-r--r--   0        0        0     3070 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/credentials.py
+-rw-r--r--   0        0        0     1436 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/__init__.py
+-rw-r--r--   0        0        0      951 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/base.py
+-rw-r--r--   0        0        0     2364 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/mongo.py
+-rw-r--r--   0        0        0      416 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/moto/__init__.py
+-rw-r--r--   0        0        0     1960 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/moto/action.py
+-rw-r--r--   0        0        0     5050 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/moto/base.py
+-rw-r--r--   0        0        0     3417 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/mysql.py
+-rw-r--r--   0        0        0    11153 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/postgresql.py
+-rw-r--r--   0        0        0     2713 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/redis.py
+-rw-r--r--   0        0        0     4659 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/redshift/__init__.py
+-rw-r--r--   0        0        0     4939 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/redshift/udf.py
+-rw-r--r--   0        0        0     9051 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/sqlite.py
+-rw-r--r--   0        0        0     3813 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/hooks.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/__init__.py
+-rw-r--r--   0        0        0     7056 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py
+-rw-r--r--   0        0        0     7290 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py
+-rw-r--r--   0        0        0     2486 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/psycopg2.py
+-rw-r--r--   0        0        0     2905 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/py.typed
+-rw-r--r--   0        0        0    10215 2023-07-24 19:47:37.853882 pytest_mock_resources-2.9.1/src/pytest_mock_resources/sqlalchemy.py
+-rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 pytest_mock_resources-2.9.1/setup.py
+-rw-r--r--   0        0        0     7821 1970-01-01 00:00:00.000000 pytest_mock_resources-2.9.1/PKG-INFO
```

### Comparing `pytest_mock_resources-2.9.0/CHANGELOG.md` & `pytest_mock_resources-2.9.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/LICENSE` & `pytest_mock_resources-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/README.md` & `pytest_mock_resources-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/pyproject.toml` & `pytest_mock_resources-2.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-mock-resources"
-version = "2.9.0"
+version = "2.9.1"
 description = "A pytest plugin for easily instantiating reproducible mock resources."
 authors = [
     "Omar Khan <oakhan3@gmail.com>",
     "Dan Cardin <ddcardin@gmail.com>",
     "Gabriel Michael <gabriel.j.michael@gmail.com>",
     "Prateek Pisat <pisatprateek12@gmail.com>",
 ]
```

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/__init__.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/action.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/action.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/cli.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/cli.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/__init__.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/import_.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/compat/import_.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/sqlalchemy.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/compat/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/config.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/config.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/__init__.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/base.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/base.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/mongo.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/mongo.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/moto.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/moto.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/mysql.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/postgres.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/redis.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/redshift.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/container/redshift.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/credentials.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/credentials.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/__init__.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/base.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/base.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/mongo.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/mongo.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/action.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/moto/action.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/base.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/moto/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
             account_id = str(time.time_ns())[:12]
 
         sts = boto3.client(
             "sts",
             endpoint_url=url,
             aws_access_key_id="test",
             aws_secret_access_key="test",
+            region_name=region_name,
         )
         response = sts.assume_role(
             RoleArn=f"arn:aws:iam::{account_id}:role/my-role",
             RoleSessionName="test-session-name",
             ExternalId="test-external-id",
         )
```

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/mysql.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/postgresql.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/postgresql.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redis.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redshift/__init__.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redshift/udf.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/redshift/udf.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/sqlite.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/fixture/sqlite.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/hooks.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/psycopg2.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/psycopg2.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/sqlalchemy.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/patch/redshift/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/src/pytest_mock_resources/sqlalchemy.py` & `pytest_mock_resources-2.9.1/src/pytest_mock_resources/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.9.0/setup.py` & `pytest_mock_resources-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 entry_points = \
 {'console_scripts': ['pmr = pytest_mock_resources.cli:main'],
  'pytest11': ['pytest_mock_resources = pytest_mock_resources']}
 
 setup_kwargs = {
     'name': 'pytest-mock-resources',
-    'version': '2.9.0',
+    'version': '2.9.1',
     'description': 'A pytest plugin for easily instantiating reproducible mock resources.',
     'long_description': '![CircleCI](https://img.shields.io/circleci/build/gh/schireson/pytest-mock-resources/master)\n[![codecov](https://codecov.io/gh/schireson/pytest-mock-resources/branch/master/graph/badge.svg)](https://codecov.io/gh/schireson/pytest-mock-resources)\n[![Documentation\nStatus](https://readthedocs.org/projects/pytest-mock-resources/badge/?version=latest)](https://pytest-mock-resources.readthedocs.io/en/latest/?badge=latest)\n\n## Introduction\n\nCode which depends on external resources such a databases (postgres, redshift, etc) can be difficult\nto write automated tests for. Conventional wisdom might be to mock or stub out the actual database\ncalls and assert that the code works correctly before/after the calls.\n\nHowever take the following, _simple_ example:\n\n```python\ndef serialize(users):\n    return [\n        {\n            \'user\': user.serialize(),\n            \'address\': user.address.serialize(),\n            \'purchases\': [p.serialize() for p in user.purchases],\n        }\n        for user in users\n    ]\n\ndef view_function(session):\n    users = session.query(User).join(Address).options(selectinload(User.purchases)).all()\n    return serialize(users)\n```\n\nSure, you can test `serialize`, but whether the actual **query** did the correct thing _truly_\nrequires that you execute the query.\n\n## The Pitch\n\nHaving tests depend upon a **real** postgres instance running somewhere is a pain, very fragile, and\nprone to issues across machines and test failures.\n\nTherefore `pytest-mock-resources` (primarily) works by managing the lifecycle of docker containers\nand providing access to them inside your tests.\n\nAs such, this package makes 2 primary assumptions:\n\n- You\'re using `pytest` (hopefully that\'s appropriate, given the package name)\n- For many resources, `docker` is required to be available and running (or accessible through remote\n  docker).\n\nIf you aren\'t familiar with Pytest Fixtures, you can read up on them in the [Pytest\ndocumentation](https://docs.pytest.org/en/latest/fixture.html).\n\nIn the above example, your test file could look something like\n\n```python\nfrom pytest_mock_resources import create_postgres_fixture\nfrom models import ModelBase\n\npg = create_postgres_fixture(ModelBase, session=True)\n\ndef test_view_function_empty_db(pg):\n  response = view_function(pg)\n  assert response == ...\n\ndef test_view_function_user_without_purchases(pg):\n  pg.add(User(...))\n  pg.flush()\n\n  response = view_function(pg)\n  assert response == ...\n\ndef test_view_function_user_with_purchases(pg):\n  pg.add(User(..., purchases=[Purchase(...)]))\n  pg.flush()\n\n  response = view_function(pg)\n  assert response == ...\n```\n\n## Existing Resources (many more possible)\n\n- SQLite\n\n  ```python\n  from pytest_mock_resources import create_sqlite_fixture\n  ```\n\n- Postgres\n\n  ```python\n  from pytest_mock_resources import create_postgres_fixture\n  ```\n\n- Redshift\n\n  **note** Uses postgres under the hood, but the fixture tries to support as much redshift\n  functionality as possible (including redshift\'s `COPY`/`UNLOAD` commands).\n\n  ```python\n  from pytest_mock_resources import create_redshift_fixture\n  ```\n\n- Mongo\n\n  ```python\n  from pytest_mock_resources import create_mongo_fixture\n  ```\n\n- Redis\n\n  ```python\n  from pytest_mock_resources import create_redis_fixture\n  ```\n\n- MySQL\n\n  ```python\n  from pytest_mock_resources import create_mysql_fixture\n  ```\n\n- Moto\n\n  ```python\n  from pytest_mock_resources import create_moto_fixture\n  ```\n\n## Features\n\nGeneral features include:\n\n- Support for "actions" which pre-populate the resource you\'re mocking before the test\n- [Async fixtures](https://pytest-mock-resources.readthedocs.io/en/latest/async.html)\n- Custom configuration for container/resource startup\n\n## Installation\n\n```bash\n# Basic fixture support i.e. SQLite\npip install "pytest-mock-resources"\n\n# General, docker-based fixture support\npip install "pytest-mock-resources[docker]"\n\n# Mongo fixture support, installs `pymongo`\npip install "pytest-mock-resources[mongo]"\n\n# Moto fixture support, installs non-driver extras specific to moto support\npip install "pytest-mock-resources[moto]"\n\n# Redis fixture support, Installs `redis` client\npip install "pytest-mock-resources[redis]"\n\n# Redshift fixture support, installs non-driver extras specific to redshift support\npip install "pytest-mock-resources[redshift]"\n```\n\nAdditionally there are number of **convenience** extras currently provided\nfor installing drivers/clients of specific features. However in most cases,\nyou **should** already be installing the driver/client used for that fixture\nas as first-party dependency of your project.\n\nAs such, we recommend against using these extras, and instead explcitly depending\non the package in question in your own project\'s 1st party dependencies.\n\n```bash\n# Installs psycopg2/psycopg2-binary driver\npip install "pytest-mock-resources[postgres-binary]"\npip install "pytest-mock-resources[postgres]"\n\n# Installs asyncpg driver\npip install "pytest-mock-resources[postgres-async]"\n\n# Installs pymysql driver\npip install "pytest-mock-resources[mysql]"\n```\n\n## Possible Future Resources\n\n- Rabbit Broker\n- AWS Presto\n\nFeel free to file an [issue](https://github.com/schireson/pytest-mock-resources/issues) if you find\nany bugs or want to start a conversation around a mock resource you want implemented!\n\n## Python 2\n\nReleases in the 1.x series were supportive of python 2. However starting from 2.0.0, support for\npython 2 was dropped. We may accept bugfix PRs for the 1.x series, however new development and\nfeatures will not be backported.\n',
     'author': 'Omar Khan',
     'author_email': 'oakhan3@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/pytest-mock-resources',
```

### Comparing `pytest_mock_resources-2.9.0/PKG-INFO` & `pytest_mock_resources-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mock-resources
-Version: 2.9.0
+Version: 2.9.1
 Summary: A pytest plugin for easily instantiating reproducible mock resources.
 Home-page: https://github.com/schireson/pytest-mock-resources
 License: MIT
 Keywords: pytest,sqlalchemy,docker,fixture,mock
 Author: Omar Khan
 Author-email: oakhan3@gmail.com
 Requires-Python: >=3.7,<4
```

