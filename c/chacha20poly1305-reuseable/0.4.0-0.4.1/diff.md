# Comparing `tmp/chacha20poly1305_reuseable-0.4.0.tar.gz` & `tmp/chacha20poly1305_reuseable-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chacha20poly1305_reuseable-0.4.0.tar", max compression
+gzip compressed data, was "chacha20poly1305_reuseable-0.4.1.tar", max compression
```

## Comparing `chacha20poly1305_reuseable-0.4.0.tar` & `chacha20poly1305_reuseable-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    12880 2023-07-24 17:04:26.289563 chacha20poly1305_reuseable-0.4.0/LICENSE
--rw-r--r--   0        0        0     4027 2023-07-24 17:04:26.289563 chacha20poly1305_reuseable-0.4.0/README.md
--rw-r--r--   0        0        0      905 2023-07-24 17:04:26.289563 chacha20poly1305_reuseable-0.4.0/build_ext.py
--rw-r--r--   0        0        0     2131 2023-07-24 17:04:27.433559 chacha20poly1305_reuseable-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1642 2023-07-24 17:04:26.289563 chacha20poly1305_reuseable-0.4.0/src/chacha20poly1305_reuseable/__init__.pxd
--rw-r--r--   0        0        0     8514 2023-07-24 17:04:27.385559 chacha20poly1305_reuseable-0.4.0/src/chacha20poly1305_reuseable/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 17:04:26.289563 chacha20poly1305_reuseable-0.4.0/src/chacha20poly1305_reuseable/py.typed
--rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.4.0/setup.py
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    12880 2023-07-24 17:24:52.456389 chacha20poly1305_reuseable-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4027 2023-07-24 17:24:52.456389 chacha20poly1305_reuseable-0.4.1/README.md
+-rw-r--r--   0        0        0      905 2023-07-24 17:24:52.456389 chacha20poly1305_reuseable-0.4.1/build_ext.py
+-rw-r--r--   0        0        0     2131 2023-07-24 17:24:53.272388 chacha20poly1305_reuseable-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1642 2023-07-24 17:24:52.456389 chacha20poly1305_reuseable-0.4.1/src/chacha20poly1305_reuseable/__init__.pxd
+-rw-r--r--   0        0        0     8532 2023-07-24 17:24:53.236388 chacha20poly1305_reuseable-0.4.1/src/chacha20poly1305_reuseable/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 17:24:52.456389 chacha20poly1305_reuseable-0.4.1/src/chacha20poly1305_reuseable/py.typed
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.4.1/setup.py
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.4.1/PKG-INFO
```

### Comparing `chacha20poly1305_reuseable-0.4.0/LICENSE` & `chacha20poly1305_reuseable-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.4.0/README.md` & `chacha20poly1305_reuseable-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.4.0/build_ext.py` & `chacha20poly1305_reuseable-0.4.1/build_ext.py`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.4.0/pyproject.toml` & `chacha20poly1305_reuseable-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chacha20poly1305-reuseable"
-version = "0.4.0"
+version = "0.4.1"
 description = "ChaCha20Poly1305 that is reuseable for asyncio"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/chacha20poly1305-reuseable"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `chacha20poly1305_reuseable-0.4.0/src/chacha20poly1305_reuseable/__init__.pxd` & `chacha20poly1305_reuseable-0.4.1/src/chacha20poly1305_reuseable/__init__.pxd`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.4.0/src/chacha20poly1305_reuseable/__init__.py` & `chacha20poly1305_reuseable-0.4.1/src/chacha20poly1305_reuseable/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 
 import os
@@ -38,18 +38,19 @@
 
 NULL = ffi.NULL
 
 _ENCRYPT = 1
 _DECRYPT = 0
 
 _bytes = bytes
+_int = int
 
 
 def _check_params(
-    nonce_len: int,
+    nonce_len: _int,
     nonce: Union[_bytes, bytearray],
     data: _bytes,
     associated_data: _bytes,
 ) -> None:
     if not isinstance(nonce, (bytes, bytearray)):
         raise TypeError("Nonce must be bytes or bytearray")
     if not isinstance(data, bytes):
@@ -156,29 +157,29 @@
             nonce,
             data,
             associated_data,
             TAG_LENGTH,
         )
 
 
-def _set_nonce(ctx: object, nonce: Union[_bytes, bytearray], operation: int) -> None:
+def _set_nonce(ctx: object, nonce: Union[_bytes, bytearray], operation: _int) -> None:
     nonce_ptr = ffi_from_buffer(nonce)
     res = EVP_CipherInit_ex(
         ctx,
         NULL,
         NULL,
         NULL,
         nonce_ptr,
         int(operation == _ENCRYPT),
     )
     openssl_assert(res != 0)
 
 
 def _aead_setup_with_fixed_nonce_len(
-    cipher_name: _bytes, key: Union[_bytes, bytearray], nonce_len: int, operation: int
+    cipher_name: _bytes, key: Union[_bytes, bytearray], nonce_len: _int, operation: _int
 ) -> object:
     # create the ctx
     ctx = EVP_CIPHER_CTX_new()
     ctx = ffi_gc(ctx, EVP_CIPHER_CTX_free)
     # set the cipher
     evp_cipher = EVP_get_cipherbyname(cipher_name)
     openssl_assert(evp_cipher != NULL)
@@ -231,22 +232,22 @@
 
 
 def _encrypt_with_fixed_nonce_len(
     ctx: object,
     nonce: Union[_bytes, bytearray],
     data: _bytes,
     associated_data: _bytes,
-    tag_length: int,
+    tag_length: _int,
 ) -> bytes:
     _set_nonce(ctx, nonce, _ENCRYPT)
     return _encrypt_data(ctx, data, associated_data, tag_length)
 
 
 def _encrypt_data(
-    ctx: object, data: _bytes, associated_data: _bytes, tag_length: int
+    ctx: object, data: _bytes, associated_data: _bytes, tag_length: _int
 ) -> bytes:
     _process_aad(ctx, associated_data)
     processed_data = _process_data(ctx, data)
     outlen = ffi_new("int *")
     res = EVP_CipherFinal_ex(ctx, NULL, outlen)
     openssl_assert(res != 0)
     openssl_assert(outlen[0] == 0)
@@ -258,15 +259,15 @@
 
 
 def _decrypt_with_fixed_nonce_len(
     ctx: object,
     nonce: Union[_bytes, bytearray],
     data: _bytes,
     associated_data: _bytes,
-    tag_length: int,
+    tag_length: _int,
 ) -> bytes:
     if len(data) < tag_length:
         raise InvalidTag
     negative_tag_length = -tag_length
     tag = data[negative_tag_length:]
     data = data[:negative_tag_length]
     _set_nonce(ctx, nonce, _DECRYPT)
```

### Comparing `chacha20poly1305_reuseable-0.4.0/setup.py` & `chacha20poly1305_reuseable-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cryptography>=36.0.2']
 
 setup_kwargs = {
     'name': 'chacha20poly1305-reuseable',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'ChaCha20Poly1305 that is reuseable for asyncio',
     'long_description': '# chacha20poly1305_reuseable\n\n<p align="center">\n  <a href="https://github.com/bdraco/chacha20poly1305-reuseable/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bdraco/chacha20poly1305-reuseable/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/chacha20poly1305-reuseable">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/chacha20poly1305-reuseable.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/chacha20poly1305-reuseable/">\n    <img src="https://img.shields.io/pypi/v/chacha20poly1305-reuseable.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/chacha20poly1305-reuseable.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/chacha20poly1305-reuseable.svg?style=flat-square" alt="License">\n</p>\n\nChaCha20Poly1305 that is reuseable for asyncio\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install chacha20poly1305-reuseable`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://github.com/bdraco"><img src="https://avatars.githubusercontent.com/u/663432?v=4?s=80" width="80px;" alt=""/><br /><sub><b>J. Nick Koston</b></sub></a><br /><a href="https://github.com/bdraco/chacha20poly1305-reuseable/commits?author=bdraco" title="Code">💻</a> <a href="#ideas-bdraco" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/bdraco/chacha20poly1305-reuseable/commits?author=bdraco" title="Documentation">📖</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/chacha20poly1305-reuseable',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['chacha20poly1305_reuseable'] package_data = \ {'': ['*']}
 install_requires = \ ['cryptography>=36.0.2'] setup_kwargs = { 'name':
-'chacha20poly1305-reuseable', 'version': '0.4.0', 'description':
+'chacha20poly1305-reuseable', 'version': '0.4.1', 'description':
 'ChaCha20Poly1305 that is reuseable for asyncio', 'long_description': '#
 chacha20poly1305_reuseable\n\n
             \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
```

### Comparing `chacha20poly1305_reuseable-0.4.0/PKG-INFO` & `chacha20poly1305_reuseable-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chacha20poly1305-reuseable
-Version: 0.4.0
+Version: 0.4.1
 Summary: ChaCha20Poly1305 that is reuseable for asyncio
 Home-page: https://github.com/bdraco/chacha20poly1305-reuseable
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chacha20poly1305-reuseable Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: chacha20poly1305-reuseable Version: 0.4.1 Summary:
 ChaCha20Poly1305 that is reuseable for asyncio Home-page: https://github.com/
 bdraco/chacha20poly1305-reuseable License: Apache Software License 2.0 Author:
 J. Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: Other/Proprietary License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

