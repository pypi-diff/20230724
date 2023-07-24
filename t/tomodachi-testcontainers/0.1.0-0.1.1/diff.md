# Comparing `tmp/tomodachi_testcontainers-0.1.0.tar.gz` & `tmp/tomodachi_testcontainers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-0.1.0.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-0.1.1.tar", max compression
```

## Comparing `tomodachi_testcontainers-0.1.0.tar` & `tomodachi_testcontainers-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.1.0/LICENSE
--rw-r--r--   0        0        0    24828 2023-07-23 10:30:40.079394 tomodachi_testcontainers-0.1.0/README.md
--rw-r--r--   0        0        0     3562 2023-07-23 10:30:40.086579 tomodachi_testcontainers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0     2300 2023-07-23 10:30:40.087069 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/clients/snssqs_client.py
--rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0     1602 2023-07-23 10:30:40.087572 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/common.py
--rw-r--r--   0        0        0     1854 2023-07-23 10:30:40.087734 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2121 2023-07-23 10:30:40.087931 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     3150 2023-07-23 10:30:40.088136 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0      965 2023-07-23 10:30:40.088352 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     1346 2023-07-23 10:30:40.088641 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/__init__.py
--rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/assertions.py
--rw-r--r--   0        0        0     2290 2023-07-23 10:30:40.088974 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
--rw-r--r--   0        0        0     2109 2023-07-23 10:30:40.089100 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py
--rw-r--r--   0        0        0     1594 2023-07-23 10:30:40.089262 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
--rw-r--r--   0        0        0      605 2023-07-23 10:30:40.089418 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
--rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0    25968 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.1.1/LICENSE
+-rw-r--r--   0        0        0    24828 2023-07-23 10:30:40.079394 tomodachi_testcontainers-0.1.1/README.md
+-rw-r--r--   0        0        0     3490 2023-07-24 15:08:57.356890 tomodachi_testcontainers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0     2300 2023-07-23 10:30:40.087069 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/clients/snssqs_client.py
+-rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0     1602 2023-07-23 10:30:40.087572 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/common.py
+-rw-r--r--   0        0        0     1854 2023-07-23 10:30:40.087734 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2121 2023-07-23 10:30:40.087931 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     3150 2023-07-23 10:30:40.088136 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0      965 2023-07-23 10:30:40.088352 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     1346 2023-07-23 10:30:40.088641 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/__init__.py
+-rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/assertions.py
+-rw-r--r--   0        0        0     2290 2023-07-23 10:30:40.088974 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
+-rw-r--r--   0        0        0     2109 2023-07-23 10:30:40.089100 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py
+-rw-r--r--   0        0        0     1594 2023-07-23 10:30:40.089262 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
+-rw-r--r--   0        0        0      605 2023-07-23 10:30:40.089418 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
+-rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0    26017 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.1.1/PKG-INFO
```

### Comparing `tomodachi_testcontainers-0.1.0/LICENSE` & `tomodachi_testcontainers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/README.md` & `tomodachi_testcontainers-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/pyproject.toml` & `tomodachi_testcontainers-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "0.1.0"
+version = "0.1.1"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 aiobotocore = "^2.5.2"
 asyncssh = { version = "^2.13.2", optional = true }
 pytest = "^7.1.2"
+pytest-asyncio = "^0.21.1"
 testcontainers = "^3.7.1"
 types-aiobotocore = { extras = ["dynamodb", "s3", "sns", "sqs", "ssm"], version = "^2.5.2" }
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.2.0"
 bandit = "^1.7.5"
 black = "^23.7.0"
@@ -41,15 +42,14 @@
 flake8-warnings = "^0.4.0"
 httpx = "^0.24.1"
 isort = "^5.12.0"
 mypy = "^1.4.1"
 pre-commit = ">=3.3.3"
 pydantic = "^2.0.2"
 pylint = "^2.17.4"
-pytest-asyncio = "^0.21.1"
 pytest-cov = "^4.1.0"
 pytest-env = "^0.8.2"
 ruff = "^0.0.277"
 structlog = "^23.1.0"
 tomodachi = "^0.25.0"
 
 [tool.poetry.extras]
@@ -63,16 +63,14 @@
 tomodachi_testcontainers = "tomodachi_testcontainers.pytest"
 
 [tool.poetry.scripts]
 hooks = "dev:hooks"
 format = "dev:format"
 lint = "dev:lint"
 test = "dev:test"
-test-cov-term = "dev:test_cov_term"
-test-cov-html = "dev:test_cov_html"
 test-ci = "dev:test_ci"
 
 [tool.black]
 line-length = 120
 target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '\.git/|\.mypy_cache/|\.venv/|\.pytest_cache/|\.vscode/|__pycache__/|build/|dist/'
```

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/clients/snssqs_client.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/clients/snssqs_client.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/common.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/common.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/moto.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/__init__.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py` & `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.0/PKG-INFO` & `tomodachi_testcontainers-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: sftp
 Requires-Dist: aiobotocore (>=2.5.2,<3.0.0)
 Requires-Dist: asyncssh (>=2.13.2,<3.0.0) ; extra == "sftp"
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
+Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0)
 Requires-Dist: testcontainers (>=3.7.1,<4.0.0)
 Requires-Dist: types-aiobotocore[dynamodb,s3,sns,sqs,ssm] (>=2.5.2,<3.0.0)
 Project-URL: Repository, https://github.com/filipsnastins/tomodachi-testcontainers
 Description-Content-Type: text/markdown
 
 # tomodachi-testcontainers
```

