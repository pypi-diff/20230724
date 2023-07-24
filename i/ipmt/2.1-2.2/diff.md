# Comparing `tmp/ipmt-2.1.tar.gz` & `tmp/ipmt-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipmt-2.1.tar", max compression
+gzip compressed data, was "ipmt-2.2.tar", max compression
```

## Comparing `ipmt-2.1.tar` & `ipmt-2.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2022-11-23 13:48:31.127859 ipmt-2.1/LICENSE
--rw-r--r--   0        0        0     1935 2022-11-23 13:48:31.127859 ipmt-2.1/README.rst
--rw-r--r--   0        0        0        0 2022-11-23 13:48:31.127859 ipmt-2.1/ipmt/__init__.py
--rw-r--r--   0        0        0    11821 2022-11-23 13:48:31.127859 ipmt-2.1/ipmt/cli.py
--rw-r--r--   0        0        0    11707 2022-11-23 13:48:31.127859 ipmt-2.1/ipmt/db.py
--rw-r--r--   0        0        0      189 2022-11-23 13:48:31.127859 ipmt-2.1/ipmt/error.py
--rw-r--r--   0        0        0    35012 2022-11-23 13:48:31.127859 ipmt-2.1/ipmt/migration.py
--rw-r--r--   0        0        0     6492 2022-11-23 13:48:31.127859 ipmt-2.1/ipmt/misc.py
--rw-r--r--   0        0        0    14462 2022-11-23 13:48:31.127859 ipmt-2.1/ipmt/permissions.py
--rw-r--r--   0        0        0     1352 2022-11-23 13:49:21.279882 ipmt-2.1/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 ipmt-2.1/setup.py
--rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 ipmt-2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 11:06:32.876900 ipmt-2.2/LICENSE
+-rw-r--r--   0        0        0     1935 2023-07-24 11:06:32.876900 ipmt-2.2/README.rst
+-rw-r--r--   0        0        0        0 2023-07-24 11:06:32.880900 ipmt-2.2/ipmt/__init__.py
+-rw-r--r--   0        0        0    11821 2023-07-24 11:06:32.880900 ipmt-2.2/ipmt/cli.py
+-rw-r--r--   0        0        0    11707 2023-07-24 11:06:32.880900 ipmt-2.2/ipmt/db.py
+-rw-r--r--   0        0        0      189 2023-07-24 11:06:32.880900 ipmt-2.2/ipmt/error.py
+-rw-r--r--   0        0        0    35012 2023-07-24 11:06:32.880900 ipmt-2.2/ipmt/migration.py
+-rw-r--r--   0        0        0     6492 2023-07-24 11:06:32.880900 ipmt-2.2/ipmt/misc.py
+-rw-r--r--   0        0        0    14462 2023-07-24 11:06:32.880900 ipmt-2.2/ipmt/permissions.py
+-rw-r--r--   0        0        0     1378 2023-07-24 11:06:58.900702 ipmt-2.2/pyproject.toml
+-rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 ipmt-2.2/PKG-INFO
```

### Comparing `ipmt-2.1/LICENSE` & `ipmt-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipmt-2.1/README.rst` & `ipmt-2.2/README.rst`

 * *Files identical despite different names*

### Comparing `ipmt-2.1/ipmt/cli.py` & `ipmt-2.2/ipmt/cli.py`

 * *Files identical despite different names*

### Comparing `ipmt-2.1/ipmt/db.py` & `ipmt-2.2/ipmt/db.py`

 * *Files identical despite different names*

### Comparing `ipmt-2.1/ipmt/migration.py` & `ipmt-2.2/ipmt/migration.py`

 * *Files identical despite different names*

### Comparing `ipmt-2.1/ipmt/misc.py` & `ipmt-2.2/ipmt/misc.py`

 * *Files identical despite different names*

### Comparing `ipmt-2.1/ipmt/permissions.py` & `ipmt-2.2/ipmt/permissions.py`

 * *Files identical despite different names*

### Comparing `ipmt-2.1/pyproject.toml` & `ipmt-2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.black]
 line-length = 79
-target_version = ['py37', 'py38']
+target_version = ['py37', 'py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.mypy_cache
   | \.pytest_cache
   | \.venv
@@ -20,15 +20,15 @@
 [tool.pytest.ini_options]
 addopts = "-s -v --cov --cov-report term --cov-report=html --cov-config pyproject.toml"
 testpaths = ["tests"]
 filterwarnings = ["ignore::DeprecationWarning:distutils"]
 
 [tool.poetry]
 name = "ipmt"
-version = "2.1"
+version = "2.2"
 description = "Schema migration tools for PostgreSQL"
 authors = ["InPlat <dev@inplat.ru>"]
 keywords = ["ipmt"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
@@ -41,17 +41,17 @@
 [tool.poetry.scripts]
 ipmt = 'ipmt.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 psycopg2 = "^2.9.1"
 Jinja2 = "^3.0.1"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.1"
 Mako = "^1.1.4"
-docker = "^5.0.0"
+docker = "^6.1.3"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 mock = "^4.0.2"
 flake8 = "^5.0.4"
 pytest-cov = "^2.6.0"
@@ -59,9 +59,9 @@
 codecov = "^2.1.10"
 coverage = {extras = ["toml"], version = "^5.3"}
 toml = "^0.10.1"
 black = "^22.10.0"
 Sphinx = "^4.3.2"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ipmt-2.1/setup.py` & `ipmt-2.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,90 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ipmt
+Version: 2.2
+Summary: Schema migration tools for PostgreSQL
+Home-page: https://github.com/inplat/ipmt
+License: Apache-2.0
+Keywords: ipmt
+Author: InPlat
+Author-email: dev@inplat.ru
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: Russian
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
+Requires-Dist: Mako (>=1.1.4,<2.0.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: docker (>=6.1.3,<7.0.0)
+Requires-Dist: psycopg2 (>=2.9.1,<3.0.0)
+Description-Content-Type: text/x-rst
+
+IPMT
+====
+
+.. image:: https://img.shields.io/pypi/v/ipmt.svg
+    :target: https://pypi.python.org/pypi/ipmt
+
+.. image:: https://img.shields.io/travis/inplat/ipmt.svg
+    :target: https://travis-ci.org/inplat/ipmt
+
+.. image:: https://codecov.io/gh/inplat/ipmt/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/inplat/ipmt
+
+.. image:: https://readthedocs.org/projects/ipmt/badge/?version=latest
+    :target: http://ipmt.readthedocs.io/ru/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://pyup.io/repos/github/inplat/ipmt/shield.svg
+    :target: https://pyup.io/repos/github/inplat/ipmt/
+    :alt: Updates
+
+.. image:: https://landscape.io/github/inplat/ipmt/master/landscape.svg?style=flat
+   :target: https://landscape.io/github/inplat/ipmt/master
+   :alt: Code Health
+
+Иструмент миграций СУБД PostgreSQL
+
+
+Возможноти
+----------
+* Версионирование схемы БД
+* Ветвление в версиях
+* Управление привилегиями с помощью yaml файлов
+
+
+Документация
+-------------
+http://ipmt.readthedocs.io/ru/latest/
+
+
+Установка
+---------
+Для установки выполните в консоли::
+
+    $ pip install ipmt
+
+
+Использование
+-------------
+
+Выполните в консоли::
+
+    # инициализация репозитория
+    ipmt init
+    # создание первой версии
+    ipmt create baseline
+    # отредактируйте файл миграции разместив SQL в
+    # первом аргументе db.execute функции up для
+    # наката миграции и в аналогичном месте функции
+    # down для отката миграции
+    vim versions/000001#baseline.py
+    # накат версии на указанную БД
+    IPMT_DSN=username@hostname/dbname ipmt up
 
-packages = \
-['ipmt']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Jinja2>=3.0.1,<4.0.0',
- 'Mako>=1.1.4,<2.0.0',
- 'PyYAML>=5.4.1,<6.0.0',
- 'docker>=5.0.0,<6.0.0',
- 'psycopg2>=2.9.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['ipmt = ipmt.cli:main']}
-
-setup_kwargs = {
-    'name': 'ipmt',
-    'version': '2.1',
-    'description': 'Schema migration tools for PostgreSQL',
-    'long_description': 'IPMT\n====\n\n.. image:: https://img.shields.io/pypi/v/ipmt.svg\n    :target: https://pypi.python.org/pypi/ipmt\n\n.. image:: https://img.shields.io/travis/inplat/ipmt.svg\n    :target: https://travis-ci.org/inplat/ipmt\n\n.. image:: https://codecov.io/gh/inplat/ipmt/branch/master/graph/badge.svg\n    :target: https://codecov.io/gh/inplat/ipmt\n\n.. image:: https://readthedocs.org/projects/ipmt/badge/?version=latest\n    :target: http://ipmt.readthedocs.io/ru/latest/?badge=latest\n    :alt: Documentation Status\n\n.. image:: https://pyup.io/repos/github/inplat/ipmt/shield.svg\n    :target: https://pyup.io/repos/github/inplat/ipmt/\n    :alt: Updates\n\n.. image:: https://landscape.io/github/inplat/ipmt/master/landscape.svg?style=flat\n   :target: https://landscape.io/github/inplat/ipmt/master\n   :alt: Code Health\n\nИструмент миграций СУБД PostgreSQL\n\n\nВозможноти\n----------\n* Версионирование схемы БД\n* Ветвление в версиях\n* Управление привилегиями с помощью yaml файлов\n\n\nДокументация\n-------------\nhttp://ipmt.readthedocs.io/ru/latest/\n\n\nУстановка\n---------\nДля установки выполните в консоли::\n\n    $ pip install ipmt\n\n\nИспользование\n-------------\n\nВыполните в консоли::\n\n    # инициализация репозитория\n    ipmt init\n    # создание первой версии\n    ipmt create baseline\n    # отредактируйте файл миграции разместив SQL в\n    # первом аргументе db.execute функции up для\n    # наката миграции и в аналогичном месте функции\n    # down для отката миграции\n    vim versions/000001#baseline.py\n    # накат версии на указанную БД\n    IPMT_DSN=username@hostname/dbname ipmt up\n',
-    'author': 'InPlat',
-    'author_email': 'dev@inplat.ru',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/inplat/ipmt',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

