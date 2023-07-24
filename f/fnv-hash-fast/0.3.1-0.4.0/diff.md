# Comparing `tmp/fnv_hash_fast-0.3.1.tar.gz` & `tmp/fnv_hash_fast-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnv_hash_fast-0.3.1.tar", max compression
+gzip compressed data, was "fnv_hash_fast-0.4.0.tar", max compression
```

## Comparing `fnv_hash_fast-0.3.1.tar` & `fnv_hash_fast-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-04-04 06:52:04.109710 fnv_hash_fast-0.3.1/LICENSE
--rw-r--r--   0        0        0     3603 2023-04-04 06:52:04.109710 fnv_hash_fast-0.3.1/README.md
--rw-r--r--   0        0        0     1160 2023-04-04 06:52:04.109710 fnv_hash_fast-0.3.1/build_ext.py
--rw-r--r--   0        0        0     2014 2023-04-04 06:52:06.301832 fnv_hash_fast-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-04 06:52:06.261830 fnv_hash_fast-0.3.1/src/fnv_hash_fast/__init__.py
--rw-r--r--   0        0        0      223 2023-04-04 06:52:04.109710 fnv_hash_fast-0.3.1/src/fnv_hash_fast/_fnv_impl.pyx
--rw-r--r--   0        0        0      447 2023-04-04 06:52:04.109710 fnv_hash_fast-0.3.1/src/fnv_hash_fast/fnv_impl.py
--rw-r--r--   0        0        0      354 2023-04-04 06:52:04.109710 fnv_hash_fast-0.3.1/src/fnv_hash_fast/fnv_wrapper.h
--rw-r--r--   0        0        0        0 2023-04-04 06:52:04.109710 fnv_hash_fast-0.3.1/src/fnv_hash_fast/py.typed
--rw-r--r--   0        0        0     4431 1970-01-01 00:00:00.000000 fnv_hash_fast-0.3.1/setup.py
--rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 fnv_hash_fast-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-24 16:28:51.392743 fnv_hash_fast-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3603 2023-07-24 16:28:51.392743 fnv_hash_fast-0.4.0/README.md
+-rw-r--r--   0        0        0     1160 2023-07-24 16:28:51.392743 fnv_hash_fast-0.4.0/build_ext.py
+-rw-r--r--   0        0        0     2014 2023-07-24 16:28:52.372747 fnv_hash_fast-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-24 16:28:52.332747 fnv_hash_fast-0.4.0/src/fnv_hash_fast/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-24 16:28:51.392743 fnv_hash_fast-0.4.0/src/fnv_hash_fast/_fnv_impl.pyx
+-rw-r--r--   0        0        0      447 2023-07-24 16:28:51.392743 fnv_hash_fast-0.4.0/src/fnv_hash_fast/fnv_impl.py
+-rw-r--r--   0        0        0      354 2023-07-24 16:28:51.392743 fnv_hash_fast-0.4.0/src/fnv_hash_fast/fnv_wrapper.h
+-rw-r--r--   0        0        0        0 2023-07-24 16:28:51.392743 fnv_hash_fast-0.4.0/src/fnv_hash_fast/py.typed
+-rw-r--r--   0        0        0     4431 1970-01-01 00:00:00.000000 fnv_hash_fast-0.4.0/setup.py
+-rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 fnv_hash_fast-0.4.0/PKG-INFO
```

### Comparing `fnv_hash_fast-0.3.1/LICENSE` & `fnv_hash_fast-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fnv_hash_fast-0.3.1/README.md` & `fnv_hash_fast-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fnv_hash_fast-0.3.1/build_ext.py` & `fnv_hash_fast-0.4.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `fnv_hash_fast-0.3.1/pyproject.toml` & `fnv_hash_fast-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fnv-hash-fast"
-version = "0.3.1"
+version = "0.4.0"
 description = "A fast version of fnv1a"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/fnv-hash-fast"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `fnv_hash_fast-0.3.1/setup.py` & `fnv_hash_fast-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['fnvhash>=0.1.0,<0.2.0']
 
 setup_kwargs = {
     'name': 'fnv-hash-fast',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'A fast version of fnv1a',
     'long_description': '# FNV Hash Fast\n\n<p align="center">\n  <a href="https://github.com/bdraco/fnv-hash-fast/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bdraco/fnv-hash-fast/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/fnv-hash-fast">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/fnv-hash-fast.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/fnv-hash-fast/">\n    <img src="https://img.shields.io/pypi/v/fnv-hash-fast.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/fnv-hash-fast.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/fnv-hash-fast.svg?style=flat-square" alt="License">\n</p>\n\nA fast version of fnv1a\n\nThis library will use a CPP implementation of fnv1a (32) if cython is available, and will fallback to pure python from the fnvhash package if it is not.\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install fnv-hash-fast`\n\n## Example\n\n```python\n>>> import fnv_hash_fast\n>>> fnv_hash_fast.fnv1a_32(b"hello")\n1335831723\n>>> fnv_hash_fast.fnv1a_32(b"goodbye")\n1188507472\n```\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/fnv-hash-fast',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['fnv_hash_fast'] package_data = \ {'': ['*']}
 install_requires = \ ['fnvhash>=0.1.0,<0.2.0'] setup_kwargs = { 'name': 'fnv-
-hash-fast', 'version': '0.3.1', 'description': 'A fast version of fnv1a',
+hash-fast', 'version': '0.4.0', 'description': 'A fast version of fnv1a',
 'long_description': '# FNV Hash Fast\n\n
             \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
 \n\nA fast version of fnv1a\n\nThis library will use a CPP implementation of
```

### Comparing `fnv_hash_fast-0.3.1/PKG-INFO` & `fnv_hash_fast-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnv-hash-fast
-Version: 0.3.1
+Version: 0.4.0
 Summary: A fast version of fnv1a
 Home-page: https://github.com/bdraco/fnv-hash-fast
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fnv-hash-fast Version: 0.3.1 Summary: A fast
+Metadata-Version: 2.1 Name: fnv-hash-fast Version: 0.4.0 Summary: A fast
 version of fnv1a Home-page: https://github.com/bdraco/fnv-hash-fast License:
 MIT Author: J. Nick Koston Author-email: nick@koston.org Requires-Python:
 >=3.7,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

