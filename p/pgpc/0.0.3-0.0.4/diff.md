# Comparing `tmp/pgpc-0.0.3.tar.gz` & `tmp/pgpc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpc-0.0.3.tar", last modified: Sun Jul 23 11:06:03 2023, max compression
+gzip compressed data, was "pgpc-0.0.4.tar", last modified: Mon Jul 24 02:58:03 2023, max compression
```

## Comparing `pgpc-0.0.3.tar` & `pgpc-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:06:03.763442 pgpc-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-23 11:05:50.000000 pgpc-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-23 11:05:50.000000 pgpc-0.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-23 11:06:03.763442 pgpc-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-23 11:05:50.000000 pgpc-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 11:06:03.763442 pgpc-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-23 11:05:50.000000 pgpc-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:06:03.759441 pgpc-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:06:03.763442 pgpc-0.0.3/src/pgpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 11:05:50.000000 pgpc-0.0.3/src/pgpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-23 11:05:50.000000 pgpc-0.0.3/src/pgpc/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-23 11:05:50.000000 pgpc-0.0.3/src/pgpc/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:06:03.763442 pgpc-0.0.3/src/pgpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-23 11:06:03.000000 pgpc-0.0.3/src/pgpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-23 11:06:03.000000 pgpc-0.0.3/src/pgpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 11:06:03.000000 pgpc-0.0.3/src/pgpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-23 11:06:03.000000 pgpc-0.0.3/src/pgpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-23 11:06:03.000000 pgpc-0.0.3/src/pgpc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:06:03.763442 pgpc-0.0.3/src/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 11:05:50.000000 pgpc-0.0.3/src/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-23 11:05:50.000000 pgpc-0.0.3/src/test/test_parse_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:58:03.596275 pgpc-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-24 02:57:50.000000 pgpc-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 02:57:50.000000 pgpc-0.0.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-24 02:58:03.596275 pgpc-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 02:57:50.000000 pgpc-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:58:03.596275 pgpc-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 02:57:50.000000 pgpc-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:58:03.592275 pgpc-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:58:03.592275 pgpc-0.0.4/src/pgpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:57:50.000000 pgpc-0.0.4/src/pgpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-24 02:57:50.000000 pgpc-0.0.4/src/pgpc/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-24 02:57:50.000000 pgpc-0.0.4/src/pgpc/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:58:03.592275 pgpc-0.0.4/src/pgpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-24 02:58:03.000000 pgpc-0.0.4/src/pgpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 02:58:03.000000 pgpc-0.0.4/src/pgpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:58:03.000000 pgpc-0.0.4/src/pgpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 02:58:03.000000 pgpc-0.0.4/src/pgpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 02:58:03.000000 pgpc-0.0.4/src/pgpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:58:03.596275 pgpc-0.0.4/src/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:57:50.000000 pgpc-0.0.4/src/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 02:57:50.000000 pgpc-0.0.4/src/test/test_parse_text.py
```

### Comparing `pgpc-0.0.3/LICENSE` & `pgpc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgpc-0.0.3/PKG-INFO` & `pgpc-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpc
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Generator based Parser Combinator library
 Home-page: https://github.com/neshkeev/pgpc
 Author: neshkeev
 Author-email: neshkeev@yandex.ru
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pgpc-0.0.3/README.md` & `pgpc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pgpc-0.0.3/setup.py` & `pgpc-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pgpc",
-    version="0.0.3",
+    version="0.0.4",
     description="A Python Generator based Parser Combinator library",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/neshkeev/pgpc",
     author="neshkeev",
```

### Comparing `pgpc-0.0.3/src/pgpc/parser.py` & `pgpc-0.0.4/src/pgpc/parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import copy
 
 from pgpc.scanner import Scanner, Position, ELEMENT
-from typing import TypeVar, Generic, Callable, Any, Sequence
+from typing import TypeVar, Generic, Callable, Any, Sequence, List
 from functools import wraps
 
 V = TypeVar('V')
 U = TypeVar('U')
 
 
 class Parser(Generic[V]):
@@ -19,17 +19,57 @@
     def and_then(self, consumer: Callable[[V], 'Parser[U]']) -> 'Parser[U]':
         def __with_scanner(scanner: Scanner) -> U:
             v = self.__parser(scanner)
             return consumer(v)(scanner)
 
         return Parser(__with_scanner)
 
-    def __call__(self, scanner: Scanner, *args, **kwargs):
+    def __call__(self, scanner: Scanner, *args, **kwargs) -> V:
         return self.__parser(scanner)
 
+    def alt(self, parser: 'Parser[U]') -> 'Parser[V | U]':
+        def __with_scanner(scanner: Scanner) -> V:
+            try:
+                scanner.mark()
+                return self.__parser(scanner)
+            except ValueError:
+                scanner.reset()
+                return parser(scanner)
+
+        return Parser(__with_scanner)
+
+    def map(self, mapper: Callable[[V], U]) -> 'Parser[U]':
+        def __with_scanner(scanner: Scanner) -> U:
+            result = self.__parser(scanner)
+            return mapper(result)
+
+        return Parser(__with_scanner)
+
+    def replace_with(self, parser: 'Parser[U]') -> 'Parser[U]':
+        return self.replace_lazy(lambda: parser)
+
+    def replace_lazy(self, parser: Callable[[], 'Parser[U]']) -> 'Parser[U]':
+        def __with_scanner(scanner: Scanner) -> U:
+            self.__parser(scanner)
+            value = parser()(scanner)
+            return value
+
+        return Parser(__with_scanner)
+
+    def drain_next(self, parser: 'Parser[V]') -> 'Parser[V]':
+        def __with_scanner(scanner: Scanner) -> V:
+            value = self.__parser(scanner)
+            parser(scanner)
+            return value
+
+        return Parser(__with_scanner)
+
+    def __or__(self, other: 'Parser[U]') -> 'Parser[V | U]':
+        return self.alt(other)
+
 
 def topology(parser_builder) -> Callable[..., Parser[V]]:
     @wraps(parser_builder)
     def wrapper(*args: Any, **kwargs: Any) -> Parser[V]:
         gen = parser_builder(*args, **kwargs)
 
         def __with_scanner(scanner: Scanner) -> V:
@@ -42,38 +82,78 @@
                 return e.value
 
         return Parser(__with_scanner)
 
     return wrapper
 
 
-def satisfy(predicate: Callable[[str], bool]) -> Parser[str]:
-    def __with_scanner(scanner: Scanner) -> str:
+def satisfy(predicate: Callable[[V], bool]) -> Parser[V]:
+    def __with_scanner(scanner: Scanner) -> V:
         result = scanner.advance_if(predicate)
         if not result:
             raise Parser.ParserError(f"Unexpected '{scanner.current}' at {scanner.pos}")
         return result
 
     return Parser(__with_scanner)
 
 
 def any_char() -> Parser[str]:
     return satisfy(lambda x: True)
 
 
-def char(c: str) -> Parser[str]:
+def char(c: V) -> Parser[V]:
     return satisfy(lambda x: c == x)
 
 
+def opt(parser: Parser[V]) -> Parser[V | None]:
+    def __with_scanner(scanner: Scanner) -> V | None:
+        try:
+            scanner.mark()
+            return parser(scanner)
+        except ValueError:
+            scanner.reset()
+            return None
+
+    return Parser(__with_scanner)
+
+
+def many(parser: Parser[V]) -> Parser[List[V]]:
+    def __with_scanner(scanner: Scanner) -> List[V]:
+        result = []
+        try:
+            while True:
+                element = parser(scanner)
+                result.append(element)
+        except ValueError:
+            return result
+
+    return Parser(__with_scanner)
+
+
+def ws() -> Parser[str]:
+    return satisfy(lambda x: type(x) is str and x.isspace())
+
+
+def letter() -> Parser[str]:
+    return satisfy(lambda x: type(x) is str and x.isalpha())
+
+
+def digit() -> Parser[str]:
+    return satisfy(lambda x: type(x) is str and x.isdigit())
+
+
+def alphanum() -> Parser[str]:
+    return satisfy(lambda x: type(x) is str and x.isalnum())
+
+
 def content() -> Parser[Sequence[ELEMENT]]:
     def __with_scanner(scanner: Scanner) -> Sequence[ELEMENT]:
         return scanner.content
 
     return Parser(__with_scanner)
 
 
 def position() -> Parser[Position]:
     def __with_scanner(scanner: Scanner) -> Position:
         return copy(scanner.pos)
 
     return Parser(__with_scanner)
-
```

### Comparing `pgpc-0.0.3/src/pgpc/scanner.py` & `pgpc-0.0.4/src/pgpc/scanner.py`

 * *Files identical despite different names*

### Comparing `pgpc-0.0.3/src/pgpc.egg-info/PKG-INFO` & `pgpc-0.0.4/src/pgpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpc
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Generator based Parser Combinator library
 Home-page: https://github.com/neshkeev/pgpc
 Author: neshkeev
 Author-email: neshkeev@yandex.ru
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pgpc-0.0.3/src/test/test_parse_text.py` & `pgpc-0.0.4/src/test/test_parse_text.py`

 * *Files identical despite different names*

