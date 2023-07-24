# Comparing `tmp/binapy-0.6.1.tar.gz` & `tmp/binapy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binapy-0.6.1.tar", max compression
+gzip compressed data, was "binapy-0.7.0.tar", max compression
```

## Comparing `binapy-0.6.1.tar` & `binapy-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1073 2023-06-21 12:59:11.684518 binapy-0.6.1/LICENSE
--rw-r--r--   0        0        0     1637 2023-06-21 12:59:11.684518 binapy-0.6.1/README.md
--rw-r--r--   0        0        0      471 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/__init__.py
--rw-r--r--   0        0        0    23456 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/binapy.py
--rw-r--r--   0        0        0       78 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/compression/__init__.py
--rw-r--r--   0        0        0     1606 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/compression/zlib.py
--rw-r--r--   0        0        0      203 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/encoding/__init__.py
--rw-r--r--   0        0        0     3392 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/encoding/base64.py
--rw-r--r--   0        0        0      958 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/encoding/hex.py
--rw-r--r--   0        0        0     1348 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/encoding/url.py
--rw-r--r--   0        0        0      104 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/hashing/__init__.py
--rw-r--r--   0        0        0     3008 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/hashing/sha.py
--rw-r--r--   0        0        0     1943 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/hashing/shake.py
--rw-r--r--   0        0        0      107 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/parsing/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/parsing/json.py
--rw-r--r--   0        0        0        0 2023-06-21 12:59:11.684518 binapy-0.6.1/binapy/py.typed
--rw-r--r--   0        0        0     2017 2023-06-21 12:59:11.688519 binapy-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       36 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0     6698 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_binapy.py
--rw-r--r--   0        0        0     2195 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_compression.py
--rw-r--r--   0        0        0     1361 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_encoding.py
--rw-r--r--   0        0        0     4447 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_hash.py
--rw-r--r--   0        0        0     1582 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_json.py
--rw-r--r--   0        0        0      785 2023-06-21 12:59:11.688519 binapy-0.6.1/tests/test_ldap_hash.py
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 binapy-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-24 07:33:49.677457 binapy-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1637 2023-07-24 07:33:49.677457 binapy-0.7.0/README.md
+-rw-r--r--   0        0        0      471 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/__init__.py
+-rw-r--r--   0        0        0    23344 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/binapy.py
+-rw-r--r--   0        0        0       78 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/compression/__init__.py
+-rw-r--r--   0        0        0     1606 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/compression/zlib.py
+-rw-r--r--   0        0        0      203 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/encoding/__init__.py
+-rw-r--r--   0        0        0     3392 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/encoding/base64.py
+-rw-r--r--   0        0        0      926 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/encoding/hex.py
+-rw-r--r--   0        0        0     1348 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/encoding/url.py
+-rw-r--r--   0        0        0      104 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/hashing/__init__.py
+-rw-r--r--   0        0        0     3008 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/hashing/sha.py
+-rw-r--r--   0        0        0     1943 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/hashing/shake.py
+-rw-r--r--   0        0        0      107 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/parsing/__init__.py
+-rw-r--r--   0        0        0     1734 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/parsing/json.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:33:49.677457 binapy-0.7.0/binapy/py.typed
+-rw-r--r--   0        0        0     1887 2023-07-24 07:33:49.681457 binapy-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-07-24 07:33:49.681457 binapy-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     6698 2023-07-24 07:33:49.681457 binapy-0.7.0/tests/test_binapy.py
+-rw-r--r--   0        0        0     2195 2023-07-24 07:33:49.681457 binapy-0.7.0/tests/test_compression.py
+-rw-r--r--   0        0        0     1331 2023-07-24 07:33:49.681457 binapy-0.7.0/tests/test_encoding.py
+-rw-r--r--   0        0        0     4441 2023-07-24 07:33:49.681457 binapy-0.7.0/tests/test_hash.py
+-rw-r--r--   0        0        0     1568 2023-07-24 07:33:49.681457 binapy-0.7.0/tests/test_json.py
+-rw-r--r--   0        0        0      785 2023-07-24 07:33:49.681457 binapy-0.7.0/tests/test_ldap_hash.py
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 binapy-0.7.0/PKG-INFO
```

### Comparing `binapy-0.6.1/LICENSE` & `binapy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/README.md` & `binapy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/binapy/binapy.py` & `binapy-0.7.0/binapy/binapy.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,22 @@
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Optional,
     SupportsBytes,
+    SupportsIndex,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
-from typing_extensions import Literal, SupportsIndex
+from typing_extensions import Literal
 
 
 class BinaPy(bytes):
     """A helper class for binary data manipulation.
 
     This subclass of `bytes` exposes various binary data manipulation methods. Since this is
     a `bytes` subclass, you can use instances of `BinaPy` anywhere you can use `bytes`. BinaPy
@@ -124,17 +125,15 @@
 
         Args:
             encoding: the encoding to use to decode the binary data
 
         Returns:
             the decoded text
         """
-        return self.re_match(
-            r'^[a-zA-Z0-9!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~ ]*$', encoding
-        )
+        return self.re_match(r'^[a-zA-Z0-9!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~ ]*$', encoding)
 
     def urlsafe(self) -> str:
         r"""Convert this BinaPy to a str, and check that it contains only url-safe characters.
 
         Url-safe characters are `[A-Za-z0-9_.\\-~]`.
 
         Returns:
@@ -146,17 +145,15 @@
         """Check that this BinaPy contains only alphanumeric characters.
 
         Returns:
             a str with only alphanumeric chars
         """
         return self.re_match(r"^[a-zA-Z]$")
 
-    def to_int(
-        self, byteorder: Literal["little", "big"] = "big", signed: bool = False
-    ) -> int:
+    def to_int(self, byteorder: Literal["little", "big"] = "big", signed: bool = False) -> int:
         """Convert this BinaPy to an `int`.
 
         This is a wrapper around
         [int.from_bytes()](https://docs.python.org/3/library/stdtypes.html#int.from_bytes) and takes
         the same parameters.
 
         Args:
@@ -181,17 +178,15 @@
             byteorder: byte order to use
             signed: True if 2 complement is used to represent negative values
 
         Returns:
             a BinaPy
         """
         s = s.replace(" ", "").replace("\t", "")
-        return cls(
-            int(s, 2).to_bytes((len(s) + 7) // 8, byteorder=byteorder, signed=signed)
-        )
+        return cls(int(s, 2).to_bytes((len(s) + 7) // 8, byteorder=byteorder, signed=signed))
 
     def to_binary_string(
         self,
         byteorder: Literal["little", "big"] = "big",
         signed: bool = False,
         pad: bool = True,
     ) -> str:
@@ -364,17 +359,15 @@
         return method
 
     @classmethod
     def _get_parser(cls, extension_name: str) -> Callable[..., Any]:
         extension_methods = cls._get_extension_methods(extension_name)
         method = extension_methods.get("parse")
         if method is None:
-            raise NotImplementedError(
-                f"Extension {extension_name} doesn't have a parse method"
-            )
+            raise NotImplementedError(f"Extension {extension_name} doesn't have a parse method")
         return method
 
     @classmethod
     def _get_serializer(cls, extension_name: str) -> "Callable[..., BinaPy]":
         extension_methods = cls._get_extension_methods(extension_name)
         method = extension_methods.get("serialize")
         if method is None:
@@ -422,17 +415,15 @@
         Returns:
             the resulting data
         """
         decoder = self._get_decoder(name)
 
         return decoder(self, *args, **kwargs)
 
-    def check(
-        self, name: str, decode: bool = False, raise_on_error: bool = False
-    ) -> bool:
+    def check(self, name: str, decode: bool = False, raise_on_error: bool = False) -> bool:
         """Check that this BinaPy conforms to a given format extension.
 
         Args:
             name: the name of the extension to check
             decode: if `True`, and the given extension doesn't have a checker method, try to decode this BinaPy using the decoder method to check if that works.
             raise_on_error: if True, Exceptions from the checker method, if any, will be raised instead of returning `False`.
 
@@ -515,17 +506,15 @@
             a BinaPy, resulting from serialization of the data
         """
         serializer = cls._get_serializer(name)
 
         return serializer(*args, **kwargs)
 
     @classmethod
-    def register_extension(
-        cls, name: str, feature: str, func: Callable[..., Any]
-    ) -> None:
+    def register_extension(cls, name: str, feature: str, func: Callable[..., Any]) -> None:
         """Register a new feature for the given extension name.
 
         Args:
             name: the extension name
             feature: name of the feature to register ("encode", "decode", etc.)
             func: the method implementing the feature
         """
```

### Comparing `binapy-0.6.1/binapy/compression/zlib.py` & `binapy-0.7.0/binapy/compression/zlib.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/binapy/encoding/base64.py` & `binapy-0.7.0/binapy/encoding/base64.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/binapy/encoding/hex.py` & `binapy-0.7.0/binapy/encoding/hex.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,12 +35,8 @@
 
     Args:
         bp: a value
 
     Returns:
         `True` if `bp` is a valid hexadecimal string
     """
-    return (
-        len(bp) % 2 == 0
-        and bp.isalnum()
-        and set(bp.lower()).issubset(b"abcdef0123456789")
-    )
+    return len(bp) % 2 == 0 and bp.isalnum() and set(bp.lower()).issubset(b"abcdef0123456789")
```

### Comparing `binapy-0.6.1/binapy/encoding/url.py` & `binapy-0.7.0/binapy/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/binapy/hashing/sha.py` & `binapy-0.7.0/binapy/hashing/sha.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/binapy/hashing/shake.py` & `binapy-0.7.0/binapy/hashing/shake.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/binapy/parsing/json.py` & `binapy-0.7.0/binapy/parsing/json.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/pyproject.toml` & `binapy-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 [tool]
 [tool.poetry]
 name = "binapy"
-version = "0.6.1"
+version = "0.7.0"
 homepage = "https://github.com/guillp/binapy"
 description = "Binary Data manipulation, for humans."
 authors = ["Guillaume Pujol <guill.p.linux@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
-    'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 packages = [
     { include = "binapy" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-typing-extensions = "^4.3.0"
+python = ">=3.8"
+typing-extensions = ">=4.3.0"
 
 [tool.poetry.dev-dependencies]
-black  = ">=22.1"
+black  = ">=23.7"
 coverage = ">=6.3.1"
-isort  = ">=5.10.1"
+isort  = ">=5.12.0"
 livereload = ">=2.6.3"
-mypy = ">=0.931"
+mypy = ">=1.4.1"
 mkdocs  = ">=1.3.1"
 mkdocs-autorefs = ">=0.3.1"
-mkdocs-include-markdown-plugin  = ">=3.2.3"
-mkdocs-material  = ">=8.1.10"
+mkdocs-material  = ">=9.1.19"
 mkdocs-material-extensions  = ">=1.0.1"
 mkdocstrings  = { version = ">=0.18.0", extras = ["python"] }
-pre-commit = ">=2.17.0"
-pytest  = ">=7.0.0"
+pre-commit = ">=3.3.3"
+pytest  = ">=7.4.0"
 pytest-mypy = ">=0.9.1"
 pytest-cov  = ">=3.0.0"
 toml = ">=0.10.2"
-tox  = ">=3.24.5"
+tox  = ">=4.6.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 88
+line-length = 96
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
@@ -84,8 +81,8 @@
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
-line_length = 88
+line_length = 96
```

### Comparing `binapy-0.6.1/tests/test_binapy.py` & `binapy-0.7.0/tests/test_binapy.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/tests/test_compression.py` & `binapy-0.7.0/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/tests/test_encoding.py` & `binapy-0.7.0/tests/test_encoding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pytest
 
 from binapy import BinaPy
 
 
-@pytest.mark.parametrize(
-    "random", [BinaPy.random(length) for length in (40, 41, 42, 43)]
-)
+@pytest.mark.parametrize("random", [BinaPy.random(length) for length in (40, 41, 42, 43)])
 @pytest.mark.parametrize("encoding", ["b32", "b64", "b64u"])
 def test_base64(random: BinaPy, encoding: str) -> None:
     # test multiple lengths to check for paddings
     assert random.encode_to(encoding).decode_from(encoding) == random
 
 
 def test_invalid_b64() -> None:
@@ -30,15 +28,12 @@
 
 
 def test_url() -> None:
     bp = BinaPy("https://localhost:3200/foo?bar=ab cd")
     assert bp.encode_to("url").decode_from("url") == bp
     assert bp.encode_to("url") == b"https%3A//localhost%3A3200/foo%3Fbar%3Dab+cd"
 
-    assert (
-        bp.encode_to("url", plus_spaces=False).decode_from("url", plus_spaces=False)
-        == bp
-    )
+    assert bp.encode_to("url", plus_spaces=False).decode_from("url", plus_spaces=False) == bp
     assert (
         bp.encode_to("url", plus_spaces=False)
         == b"https%3A//localhost%3A3200/foo%3Fbar%3Dab%20cd"
     )
```

### Comparing `binapy-0.6.1/tests/test_hash.py` & `binapy-0.7.0/tests/test_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,17 +118,15 @@
             "sshake256",
             False,
             512,
             "5e1c64356ffe5f085da56b3570d249eff55425565dfa42320d37521c8bd8b707bf550d639675546cda872cb8435beb66e1b1b905795ccb9b78013fbe6e2fe1ea",
         ),
     ),
 )
-def test_shake(
-    alg: str, append_salt: Optional[bool], length: int, hexhash: str
-) -> None:
+def test_shake(alg: str, append_salt: Optional[bool], length: int, hexhash: str) -> None:
     data = BinaPy("my_data")
     salt = BinaPy(b"my_salt")
 
     if append_salt is None:
         bp = data.encode_to(alg, length)
     else:
         bp = data.encode_to(alg, length, salt, append_salt)
```

### Comparing `binapy-0.6.1/tests/test_json.py` & `binapy-0.7.0/tests/test_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,14 @@
         "foo": "71509952-ec4f-4854-84e7-fa452994b51d",
     }
 
 
 def test_compact() -> None:
     bp = BinaPy.serialize_to("json", {"a": "b", "c": "d"}, sort_keys=True, compact=True)
     assert bp == b'{"a":"b","c":"d"}'
-    bp = BinaPy.serialize_to(
-        "json", {"a": "b", "c": "d"}, sort_keys=True, compact=False
-    )
+    bp = BinaPy.serialize_to("json", {"a": "b", "c": "d"}, sort_keys=True, compact=False)
     assert bp == b'{\n  "a": "b", \n  "c": "d"\n}'
 
     bp = BinaPy.serialize_to(
         "json", {"a": "b", "c": "d"}, sort_keys=True, compact=False, indent=4
     )
     assert bp == b'{\n    "a": "b", \n    "c": "d"\n}'
```

### Comparing `binapy-0.6.1/tests/test_ldap_hash.py` & `binapy-0.7.0/tests/test_ldap_hash.py`

 * *Files identical despite different names*

### Comparing `binapy-0.6.1/PKG-INFO` & `binapy-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: binapy
-Version: 0.6.1
+Version: 0.7.0
 Summary: Binary Data manipulation, for humans.
 Home-page: https://github.com/guillp/binapy
 License: MIT
 Author: Guillaume Pujol
 Author-email: guill.p.linux@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.3.0)
 Description-Content-Type: text/markdown
 
 # BinaPy
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Downloads](https://pepy.tech/badge/binapy/month)](https://pepy.tech/project/binapy)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/binapy.svg)](https://pypi.org/project/binapy)
```

