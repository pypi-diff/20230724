# Comparing `tmp/airflow-docker-compose-0.1.9.tar.gz` & `tmp/airflow_docker_compose-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-docker-compose-0.1.9.tar", last modified: Thu Oct 24 15:04:45 2019, max compression
+gzip compressed data, was "airflow_docker_compose-0.2.0.tar", max compression
```

## Comparing `airflow-docker-compose-0.1.9.tar` & `airflow_docker_compose-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/LICENSE
--rw-r--r--   0        0        0     1108 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/README.md
--rw-r--r--   0        0        0     1108 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/README.md
--rw-r--r--   0        0        0     1206 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/pyproject.toml
--rw-r--r--   0        0        0        0 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/src/airflow_docker_compose/__init__.py
--rw-r--r--   0        0        0       81 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/src/airflow_docker_compose/__main__.py
--rw-r--r--   0        0        0    10693 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/src/airflow_docker_compose/airflow.cfg
--rw-r--r--   0        0        0    12450 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/src/airflow_docker_compose/cli.py
--rw-r--r--   0        0        0     1967 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/src/airflow_docker_compose/docker-compose-template.yml
--rw-r--r--   0        0        0      900 2019-10-24 15:04:37.635171 airflow-docker-compose-0.1.9/src/airflow_docker_compose/test.py
--rw-r--r--   0        0        0     2065 1970-01-01 00:00:00.000000 airflow-docker-compose-0.1.9/setup.py
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 airflow-docker-compose-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 13:59:16.047003 airflow_docker_compose-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1192 2023-07-24 14:00:21.769142 airflow_docker_compose-0.2.0/README.md
+-rw-r--r--   0        0        0     1186 2023-07-24 14:00:26.968689 airflow_docker_compose-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 13:59:16.048739 airflow_docker_compose-0.2.0/src/airflow_docker_compose/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-24 13:59:16.048982 airflow_docker_compose-0.2.0/src/airflow_docker_compose/__main__.py
+-rw-r--r--   0        0        0    10693 2023-07-24 13:59:16.049234 airflow_docker_compose-0.2.0/src/airflow_docker_compose/airflow.cfg
+-rw-r--r--   0        0        0    12450 2023-07-24 13:59:16.049478 airflow_docker_compose-0.2.0/src/airflow_docker_compose/cli.py
+-rw-r--r--   0        0        0     1967 2023-07-24 13:59:16.049796 airflow_docker_compose-0.2.0/src/airflow_docker_compose/docker-compose-template.yml
+-rw-r--r--   0        0        0      900 2023-07-24 13:59:16.050305 airflow_docker_compose-0.2.0/src/airflow_docker_compose/test.py
+-rw-r--r--   0        0        0     2133 1970-01-01 00:00:00.000000 airflow_docker_compose-0.2.0/setup.py
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 airflow_docker_compose-0.2.0/PKG-INFO
```

### Comparing `airflow-docker-compose-0.1.9/LICENSE` & `airflow_docker_compose-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-docker-compose-0.1.9/README.md` & `airflow_docker_compose-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 airflow-docker-compose --help
 airflow-docker-compose up
 ```
 
 
 ## Configuration
 
+Note, this library assumes the `docker-compose` utility is available in your path.
+
 In order to use this tool, you should have a local `dags` folder containing your dags.
 You should also have a `pyproject.toml` file which minimally looks like
 
 ```ini
 [tool.airflow-docker-compose]
 docker-network = 'network-name'
 ```
```

### Comparing `airflow-docker-compose-0.1.9/pyproject.toml` & `airflow_docker_compose-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-docker-compose"
-version = "0.1.9"
+version = "0.2.0"
 description = ""
 authors = [
     "Dan Cardin <ddcardin@gmail.com>"
 ]
 license = "Apache-2.0"
 keywords = [ "airflow", "docker", "docker-compose" ]
 repository = "https://github.com/airflowdocker/airflow-docker-compose"
@@ -14,18 +14,18 @@
 readme = 'README.md'
 include = [
     "*.md",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*"
+
 click = "*"
 docker = "*"
 toml = "*"
-docker-compose = "*"
 python-dotenv = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^4.4"
 pytest-cov = "^2.6"
 
 isort = "^4.3"
```

### Comparing `airflow-docker-compose-0.1.9/src/airflow_docker_compose/airflow.cfg` & `airflow_docker_compose-0.2.0/src/airflow_docker_compose/airflow.cfg`

 * *Files identical despite different names*

### Comparing `airflow-docker-compose-0.1.9/src/airflow_docker_compose/cli.py` & `airflow_docker_compose-0.2.0/src/airflow_docker_compose/cli.py`

 * *Files identical despite different names*

### Comparing `airflow-docker-compose-0.1.9/src/airflow_docker_compose/docker-compose-template.yml` & `airflow_docker_compose-0.2.0/src/airflow_docker_compose/docker-compose-template.yml`

 * *Files identical despite different names*

### Comparing `airflow-docker-compose-0.1.9/src/airflow_docker_compose/test.py` & `airflow_docker_compose-0.2.0/src/airflow_docker_compose/test.py`

 * *Files identical despite different names*

### Comparing `airflow-docker-compose-0.1.9/setup.py` & `airflow_docker_compose-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
-from distutils.core import setup
+from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['airflow_docker_compose']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click', 'docker', 'docker-compose', 'python-dotenv', 'toml']
+['click', 'docker', 'python-dotenv', 'toml']
 
 entry_points = \
 {'console_scripts': ['airflow-docker-compose = '
                      'airflow_docker_compose.__main__:run']}
 
 setup_kwargs = {
     'name': 'airflow-docker-compose',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': '',
-    'long_description': "# airflow-docker-compose\n[![CircleCI](https://circleci.com/gh/airflowdocker/airflow-docker-compose.svg?style=svg)](https://circleci.com/gh/airflowdocker/airflow-docker-compose) [![codecov](https://codecov.io/gh/airflowdocker/airflow-docker-compose/branch/master/graph/badge.svg)](https://codecov.io/gh/airflowdocker/airflow-docker-compose)\n\n## Description\nA reasonably light wrapper around `docker-compose` to make it simple to start a local\nairflow instance in docker.\n\n## Usage\n\n```bash\nairflow-docker-compose --help\nairflow-docker-compose up\n```\n\n\n## Configuration\n\nIn order to use this tool, you should have a local `dags` folder containing your dags.\nYou should also have a `pyproject.toml` file which minimally looks like\n\n```ini\n[tool.airflow-docker-compose]\ndocker-network = 'network-name'\n```\n\nIn order to set airflow configuration, you can use the `airflow-environment-variables` key.\nThis allows you to set any `airflow.cfg` variables like so:\n\n```ini\n[tool.airflow-docker-compose]\nairflow-environment-variables = {\n    AIRWFLOW_WORKER_COUNT = 4\n    AIRFLOW__AIRFLOWDOCKER__FORCE_PULL = 'false'\n}\n",
+    'long_description': "# airflow-docker-compose\n[![CircleCI](https://circleci.com/gh/airflowdocker/airflow-docker-compose.svg?style=svg)](https://circleci.com/gh/airflowdocker/airflow-docker-compose) [![codecov](https://codecov.io/gh/airflowdocker/airflow-docker-compose/branch/master/graph/badge.svg)](https://codecov.io/gh/airflowdocker/airflow-docker-compose)\n\n## Description\nA reasonably light wrapper around `docker-compose` to make it simple to start a local\nairflow instance in docker.\n\n## Usage\n\n```bash\nairflow-docker-compose --help\nairflow-docker-compose up\n```\n\n\n## Configuration\n\nNote, this library assumes the `docker-compose` utility is available in your path.\n\nIn order to use this tool, you should have a local `dags` folder containing your dags.\nYou should also have a `pyproject.toml` file which minimally looks like\n\n```ini\n[tool.airflow-docker-compose]\ndocker-network = 'network-name'\n```\n\nIn order to set airflow configuration, you can use the `airflow-environment-variables` key.\nThis allows you to set any `airflow.cfg` variables like so:\n\n```ini\n[tool.airflow-docker-compose]\nairflow-environment-variables = {\n    AIRWFLOW_WORKER_COUNT = 4\n    AIRFLOW__AIRFLOWDOCKER__FORCE_PULL = 'false'\n}\n",
     'author': 'Dan Cardin',
     'author_email': 'ddcardin@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/airflowdocker/airflow-docker-compose',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.5.0',
```

### Comparing `airflow-docker-compose-0.1.9/PKG-INFO` & `airflow_docker_compose-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: airflow-docker-compose
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/airflowdocker/airflow-docker-compose
 License: Apache-2.0
 Keywords: airflow,docker,docker-compose
 Author: Dan Cardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.5.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click
 Requires-Dist: docker
-Requires-Dist: docker-compose
 Requires-Dist: python-dotenv
 Requires-Dist: toml
 Project-URL: Repository, https://github.com/airflowdocker/airflow-docker-compose
 Description-Content-Type: text/markdown
 
 # airflow-docker-compose
 [![CircleCI](https://circleci.com/gh/airflowdocker/airflow-docker-compose.svg?style=svg)](https://circleci.com/gh/airflowdocker/airflow-docker-compose) [![codecov](https://codecov.io/gh/airflowdocker/airflow-docker-compose/branch/master/graph/badge.svg)](https://codecov.io/gh/airflowdocker/airflow-docker-compose)
@@ -34,14 +37,16 @@
 airflow-docker-compose --help
 airflow-docker-compose up
 ```
 
 
 ## Configuration
 
+Note, this library assumes the `docker-compose` utility is available in your path.
+
 In order to use this tool, you should have a local `dags` folder containing your dags.
 You should also have a `pyproject.toml` file which minimally looks like
 
 ```ini
 [tool.airflow-docker-compose]
 docker-network = 'network-name'
 ```
```

