# Comparing `tmp/construct-typing-0.5.6.tar.gz` & `tmp/construct-typing-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "construct-typing-0.5.6.tar", last modified: Tue May  9 11:05:47 2023, max compression
+gzip compressed data, was "construct-typing-0.6.0.tar", last modified: Mon Jul 24 09:15:42 2023, max compression
```

## Comparing `construct-typing-0.5.6.tar` & `construct-typing-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-09 11:05:33.000000 construct-typing-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-09 11:05:47.748647 construct-typing-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-09 11:05:33.000000 construct-typing-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/construct-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    53656 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/expr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/construct-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/bitstream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/hex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/py3compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/construct_typed/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/dataclass_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/generic_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/tenum.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/construct_typing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:05:47.748647 construct-typing-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-09 11:05:33.000000 construct-typing-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:42.131501 construct-typing-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 09:15:27.000000 construct-typing-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-24 09:15:42.131501 construct-typing-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-24 09:15:27.000000 construct-typing-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:42.127500 construct-typing-0.6.0/construct-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    41373 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/expr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:42.127500 construct-typing-0.6.0/construct-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/lib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/lib/binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/lib/bitstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/lib/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/lib/hex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/lib/py3compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct-stubs/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:42.127500 construct-typing-0.6.0/construct_typed/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct_typed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct_typed/dataclass_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct_typed/generic_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct_typed/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct_typed/tenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 09:15:27.000000 construct-typing-0.6.0/construct_typed/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:42.131501 construct-typing-0.6.0/construct_typing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-24 09:15:42.000000 construct-typing-0.6.0/construct_typing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 09:15:42.000000 construct-typing-0.6.0/construct_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:15:42.000000 construct-typing-0.6.0/construct_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 09:15:42.000000 construct-typing-0.6.0/construct_typing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 09:15:42.000000 construct-typing-0.6.0/construct_typing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:15:42.131501 construct-typing-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-24 09:15:27.000000 construct-typing-0.6.0/setup.py
```

### Comparing `construct-typing-0.5.6/LICENSE` & `construct-typing-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/PKG-INFO` & `construct-typing-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-typing
-Version: 0.5.6
+Version: 0.6.0
 Summary: Extension for the python package 'construct' that adds typing features
 Home-page: https://github.com/timrid/construct-typing
 Author: Tim Riddermann
 License: MIT
 Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,annotation,type hint,typing,typed,bitstruct,PEP 561
 Platform: POSIX
 Platform: Windows
```

### Comparing `construct-typing-0.5.6/README.md` & `construct-typing-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/construct-stubs/__init__.pyi` & `construct-typing-0.6.0/construct-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from construct.core import *
 from construct.debug import *
 from construct.expr import *
 from construct.lib import *
 from construct.version import *
+from construct import lib
+
+__author__: str
+__version__: str
 
 #===============================================================================
 # exposed names
 #===============================================================================
 __all__ = [
     '__author__',
     '__version__',
```

### Comparing `construct-typing-0.5.6/construct-stubs/core.pyi` & `construct-typing-0.6.0/construct-stubs/core.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -13,27 +13,24 @@
     HexDisplayedInteger,
     HexDumpDisplayedBytes,
     HexDumpDisplayedDict,
     ListContainer,
     ListType,
     RebufferedBytesIO,
 )
+from typing_extensions import Buffer
 
 # unfortunately, there are a few duplications with "typing", e.g. Union and Optional, which is why the t. prefix must be used everywhere
 
 # Some of the Constructs can be optimised when the following typing optimisations are available:
 #   - Variadic Generics: https://mail.python.org/archives/list/typing-sig@python.org/thread/SQVTQYWIOI4TIO7NNBTFFWFMSMS2TA4J/
 #   - Higher Kinded Types: https://github.com/python/typing/issues/548
 #   - Higher Kinded Types: https://sobolevn.me/2020/10/higher-kinded-types-in-python
 
-# The type checkers mypy and pyright/pylance unfortunately work a little bit different with __init__ and __new__.
-# For supporting some constructs (eg. Enum, NamedTuple, Slicing) in mypy the __init__ self parameter has to have a
-# type hint. But for supporting pyright/pylance, the same type hint has to be used as the return type of __new__.
-# (see discussion here: https://github.com/python/typeshed/issues/4846).
-
+ReadableBuffer: t.TypeAlias = Buffer
 StreamType = t.IO[bytes]
 FilenameType = t.Union[str, bytes, os.PathLike[str], os.PathLike[bytes]]
 PathType = str
 ContextKWType = t.Any
 
 # ===============================================================================
 # exceptions
@@ -96,33 +93,35 @@
 BuildTypes = t.TypeVar("BuildTypes", contravariant=True)
 
 class Construct(t.Generic[ParsedType, BuildTypes]):
     name: t.Optional[str]
     docs: str
     flagbuildnone: bool
     parsed: t.Optional[t.Callable[[ParsedType, Context], None]]
-    def parse(self, data: bytes, **contextkw: ContextKWType) -> ParsedType: ...
+    def parse(self, data: ReadableBuffer, **contextkw: ContextKWType) -> ParsedType: ...
     def parse_stream(
         self, stream: StreamType, **contextkw: ContextKWType
     ) -> ParsedType: ...
     def parse_file(
         self, filename: FilenameType, **contextkw: ContextKWType
     ) -> ParsedType: ...
     def build(self, obj: BuildTypes, **contextkw: ContextKWType) -> bytes: ...
     def build_stream(
         self, obj: BuildTypes, stream: StreamType, **contextkw: ContextKWType
-    ) -> bytes: ...
+    ) -> None: ...
     def build_file(
         self, obj: BuildTypes, filename: FilenameType, **contextkw: ContextKWType
-    ) -> bytes: ...
+    ) -> None: ...
     def sizeof(self, **contextkw: ContextKWType) -> int: ...
     def compile(
         self, filename: FilenameType = ...
     ) -> Construct[ParsedType, BuildTypes]: ...
-    def benchmark(self, sampledata: bytes, filename: FilenameType = ...) -> str: ...
+    def benchmark(
+        self, sampledata: ReadableBuffer, filename: FilenameType = ...
+    ) -> str: ...
     def export_ksy(
         self, schemaname: str = ..., filename: FilenameType = ...
     ) -> str: ...
     def __rtruediv__(
         self, name: t.Optional[t.AnyStr]
     ) -> Renamed[ParsedType, BuildTypes]: ...
     __rdiv__: t.Callable[[str], Construct[ParsedType, BuildTypes]]
@@ -130,28 +129,19 @@
         self,
         other: t.Union[str, bytes, t.Callable[[ParsedType, Context], None]],
     ) -> Renamed[ParsedType, BuildTypes]: ...
     def __rmul__(
         self,
         other: t.Union[str, bytes, t.Callable[[ParsedType, Context], None]],
     ) -> Renamed[ParsedType, BuildTypes]: ...
-    def __add__(
-        self, other: Construct[t.Any, t.Any]
-    ) -> Struct[Container[t.Any], t.Optional[t.Dict[str, t.Any]]]: ...
-    def __rshift__(
-        self, other: Construct[t.Any, t.Any]
-    ) -> Sequence[ListContainer[t.Any], t.Optional[t.List[t.Any]]]: ...
+    def __add__(self, other: Construct[t.Any, t.Any]) -> Struct: ...
+    def __rshift__(self, other: Construct[t.Any, t.Any]) -> Sequence: ...
     def __getitem__(
         self, count: t.Union[int, t.Callable[[Context], int]]
-    ) -> Array[
-        ParsedType,
-        BuildTypes,
-        ListContainer[ParsedType],
-        t.List[BuildTypes],
-    ]: ...
+    ) -> Array[ParsedType, BuildTypes,]: ...
 
 @t.type_check_only
 class Context(Container[t.Any]):
     _: Context  # optional field
     _params: Context  # optional field
     _root: Context  # optional field
     _parsing: bool
@@ -170,33 +160,21 @@
 
 class Subconstruct(
     t.Generic[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes],
     Construct[ParsedType, BuildTypes],
 ):
     subcon: Construct[SubconParsedType, SubconBuildTypes]
     @t.overload
-    def __new__(
-        cls, subcon: Construct[SubconParsedType, SubconBuildTypes]
-    ) -> Subconstruct[
-        SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes
-    ]: ...
-    @t.overload
-    def __new__(
-        cls, *args: t.Any, **kwargs: t.Any
-    ) -> Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]: ...
-    @t.overload
     def __init__(
-        self: Subconstruct[
-            SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes
-        ],
+        self,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
     ) -> None: ...
     @t.overload
     def __init__(
-        self: Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes],
+        self,
         *args: t.Any,
         **kwargs: t.Any,
     ) -> None: ...
 
 class Adapter(
     Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes],
 ):
@@ -225,27 +203,32 @@
 
 class Tunnel(
     Subconstruct[SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes]
 ):
     def _decode(self, data: bytes, context: Context, path: PathType) -> bytes: ...
     def _encode(self, data: bytes, context: Context, path: PathType) -> bytes: ...
 
-# TODO: Compiled
+class Compiled(Construct[t.Any, t.Any]):
+    source: t.Optional[str]
+    defersubcon: t.Optional[Construct[t.Any, t.Any]]
+    parsefunc: t.Callable[[StreamType, Context], t.Any]
+    buildfunc: t.Callable[[t.Any, StreamType, Context], t.Any]
+    def __init__(
+        self,
+        parsefunc: t.Callable[[StreamType, Context], t.Any],
+        buildfunc: t.Callable[[t.Any, StreamType, Context], t.Any],
+    ) -> None: ...
 
 # ===============================================================================
 # bytes and bits
 # ===============================================================================
-class Bytes(Construct[ParsedType, BuildTypes]):
+class Bytes(Construct[bytes, t.Union[bytes, int]]):
     length: ConstantOrContextLambda[int]
-    def __new__(
-        cls,
-        length: ConstantOrContextLambda[int],
-    ) -> Bytes[bytes, t.Union[bytes, int]]: ...
     def __init__(
-        self: Bytes[bytes, t.Union[bytes, int]],
+        self,
         length: ConstantOrContextLambda[int],
     ) -> None: ...
 
 GreedyBytes: Construct[bytes, bytes]
 
 def Bitwise(
     subcon: Construct[SubconParsedType, SubconBuildTypes]
@@ -269,109 +252,69 @@
     if sys.version_info >= (3, 8):
         ENDIANITY = t.Union[t.Literal["=", "<", ">"], str]
         FORMAT_INT = t.Literal["B", "H", "L", "Q", "b", "h", "l", "q"]
         FORMAT_FLOAT = t.Literal["f", "d", "e"]
         FORMAT_BOOL = t.Literal["?"]
         @t.overload
         def __new__(
-            cls,
+            cls: "type[FormatField[int, int]]",
             endianity: str,
             format: FORMAT_INT,
         ) -> FormatField[int, int]: ...
         @t.overload
         def __new__(
-            cls,
+            cls: "type[FormatField[float, float]]",
             endianity: str,
             format: FORMAT_FLOAT,
         ) -> FormatField[float, float]: ...
         @t.overload
         def __new__(
-            cls,
+            cls: "type[FormatField[bool, bool]]",
             endianity: str,
             format: FORMAT_BOOL,
         ) -> FormatField[bool, bool]: ...
         @t.overload
         def __new__(
-            cls,
+            cls: "type[FormatField[t.Any, t.Any]]",
             endianity: str,
             format: str,
         ) -> FormatField[t.Any, t.Any]: ...
-        @t.overload
-        def __init__(
-            self: FormatField[int, int],
-            endianity: str,
-            format: FORMAT_INT,
-        ) -> None: ...
-        @t.overload
-        def __init__(
-            self: FormatField[float, float],
-            endianity: str,
-            format: FORMAT_FLOAT,
-        ) -> None: ...
-        @t.overload
-        def __init__(
-            self: FormatField[bool, bool],
-            endianity: str,
-            format: FORMAT_BOOL,
-        ) -> None: ...
-        @t.overload
-        def __init__(
-            self: FormatField[t.Any, t.Any],
-            endianity: str,
-            format: str,
-        ) -> None: ...
+
     else:
         def __new__(
-            cls,
+            cls: "type[FormatField[t.Any, t.Any]]",
             endianity: str,
             format: str,
         ) -> FormatField[t.Any, t.Any]: ...
-        def __init__(
-            self: FormatField[t.Any, t.Any],
-            endianity: str,
-            format: str,
-        ) -> None: ...
 
-class BytesInteger(Construct[ParsedType, BuildTypes]):
+class BytesInteger(Construct[int, int]):
     length: ConstantOrContextLambda[int]
     signed: bool
     swapped: ConstantOrContextLambda[bool]
-    def __new__(
-        cls,
-        length: ConstantOrContextLambda[int],
-        signed: bool = ...,
-        swapped: ConstantOrContextLambda[bool] = ...,
-    ) -> BytesInteger[int, int]: ...
     def __init__(
-        self: BytesInteger[int, int],
+        self,
         length: ConstantOrContextLambda[int],
         signed: bool = ...,
         swapped: ConstantOrContextLambda[bool] = ...,
     ) -> None: ...
 
-class BitsInteger(Construct[ParsedType, BuildTypes]):
+class BitsInteger(Construct[int, int]):
     length: ConstantOrContextLambda[int]
     signed: bool
     swapped: ConstantOrContextLambda[bool]
-    def __new__(
-        cls,
-        length: ConstantOrContextLambda[int],
-        signed: bool = ...,
-        swapped: ConstantOrContextLambda[bool] = ...,
-    ) -> BitsInteger[int, int]: ...
     def __init__(
-        self: BitsInteger[int, int],
+        self,
         length: ConstantOrContextLambda[int],
         signed: bool = ...,
         swapped: ConstantOrContextLambda[bool] = ...,
     ) -> None: ...
 
-Bit: BitsInteger[int, int]
-Nibble: BitsInteger[int, int]
-Octet: BitsInteger[int, int]
+Bit: BitsInteger
+Nibble: BitsInteger
+Octet: BitsInteger
 
 Int8ub: FormatField[int, int]
 Int16ub: FormatField[int, int]
 Int32ub: FormatField[int, int]
 Int64ub: FormatField[int, int]
 Int8sb: FormatField[int, int]
 Int16sb: FormatField[int, int]
@@ -409,256 +352,178 @@
 Float64l: FormatField[float, float]
 Float64n: FormatField[float, float]
 
 Half: FormatField[float, float]
 Single: FormatField[float, float]
 Double: FormatField[float, float]
 
-Int24ub: BytesInteger[int, int]
-Int24ul: BytesInteger[int, int]
-Int24un: BytesInteger[int, int]
-Int24sb: BytesInteger[int, int]
-Int24sl: BytesInteger[int, int]
-Int24sn: BytesInteger[int, int]
+Int24ub: BytesInteger
+Int24ul: BytesInteger
+Int24un: BytesInteger
+Int24sb: BytesInteger
+Int24sl: BytesInteger
+Int24sn: BytesInteger
 
 VarInt: Construct[int, int]
 ZigZag: Construct[int, int]
 
 # ===============================================================================
 # strings
 # ===============================================================================
-class StringEncoded(Construct[ParsedType, BuildTypes]):
+possiblestringencodings: t.Dict[str, int]
+
+class StringEncoded(Construct[str, str]):
     if sys.version_info >= (3, 8):
         ENCODING_1 = t.Literal["ascii", "utf8", "utf_8", "u8"]
         ENCODING_2 = t.Literal["utf16", "utf_16", "u16", "utf_16_be", "utf_16_le"]
         ENCODING_4 = t.Literal["utf32", "utf_32", "u32", "utf_32_be", "utf_32_le"]
         ENCODING = t.Union[str, ENCODING_1, ENCODING_2, ENCODING_4]
     else:
         ENCODING = str
     encoding: ENCODING
-    def __new__(
-        cls,
-        subcon: Construct[ParsedType, BuildTypes],
-        encoding: ENCODING,
-    ) -> StringEncoded[str, str]: ...
     def __init__(
-        self: StringEncoded[str, str],
-        subcon: Construct[ParsedType, BuildTypes],
+        self,
+        subcon: Construct[bytes, bytes],
         encoding: ENCODING,
     ) -> None: ...
 
 def PaddedString(
     length: ConstantOrContextLambda[int], encoding: StringEncoded.ENCODING
-) -> StringEncoded[str, str]: ...
+) -> StringEncoded: ...
 def PascalString(
     lengthfield: Construct[int, int], encoding: StringEncoded.ENCODING
-) -> StringEncoded[str, str]: ...
-def CString(encoding: StringEncoded.ENCODING) -> StringEncoded[str, str]: ...
-def GreedyString(encoding: StringEncoded.ENCODING) -> StringEncoded[str, str]: ...
+) -> StringEncoded: ...
+def CString(encoding: StringEncoded.ENCODING) -> StringEncoded: ...
+def GreedyString(encoding: StringEncoded.ENCODING) -> StringEncoded: ...
 
 # ===============================================================================
 # mappings
 # ===============================================================================
 Flag: Construct[bool, bool]
 
 class EnumInteger(int): ...
 
 class EnumIntegerString(str):
     @staticmethod
     def new(intvalue: int, stringvalue: str) -> EnumIntegerString: ...
 
-class Enum(Adapter[int, int, ParsedType, BuildTypes]):
+class Enum(
+    Adapter[int, int, t.Union[EnumInteger, EnumIntegerString], t.Union[int, str]]
+):
     encmapping: t.Dict[str, int]
     decmapping: t.Dict[int, EnumIntegerString]
     ksymapping: t.Dict[int, str]
-    def __new__(
-        cls,
-        subcon: Construct[int, int],
-        *merge: t.Union[t.Type[enum.IntEnum], t.Type[enum.IntFlag]],
-        **mapping: int,
-    ) -> Enum[t.Union[EnumInteger, EnumIntegerString], t.Union[int, str]]: ...
     def __init__(
-        self: Enum[t.Union[EnumInteger, EnumIntegerString], t.Union[int, str]],
+        self,
         subcon: Construct[int, int],
         *merge: t.Union[t.Type[enum.IntEnum], t.Type[enum.IntFlag]],
         **mapping: int,
     ) -> None: ...
     def __getattr__(self, name: str) -> EnumIntegerString: ...
 
 class BitwisableString(str):
     def __or__(self, other: BitwisableString) -> BitwisableString: ...
 
-class FlagsEnum(Adapter[int, int, ParsedType, BuildTypes]):
+class FlagsEnum(
+    Adapter[int, int, Container[bool], t.Union[int, str, t.Dict[str, bool]]]
+):
     flags: t.Dict[str, int]
     reverseflags: t.Dict[int, str]
-    def __new__(
-        cls,
-        subcon: Construct[int, int],
-        *merge: t.Union[t.Type[enum.IntEnum], t.Type[enum.IntFlag]],
-        **flags: int,
-    ) -> FlagsEnum[Container[bool], t.Union[int, str, t.Dict[str, bool]]]: ...
     def __init__(
-        self: FlagsEnum[Container[bool], t.Union[int, str, t.Dict[str, bool]]],
+        self,
         subcon: Construct[int, int],
         *merge: t.Union[t.Type[enum.IntEnum], t.Type[enum.IntFlag]],
         **flags: int,
     ) -> None: ...
     def __getattr__(self, name: str) -> BitwisableString: ...
 
 class Mapping(Adapter[SubconParsedType, SubconBuildTypes, t.Any, t.Any]):
     decmapping: t.Dict[int, str]
     encmapping: t.Dict[str, int]
-    def __new__(
-        cls,
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-        mapping: t.Dict[t.Any, t.Any],
-    ) -> Mapping[t.Any, t.Any]: ...
     def __init__(
-        self: Mapping[t.Any, t.Any],
+        self,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
         mapping: t.Dict[t.Any, t.Any],
     ) -> None: ...
 
 # ===============================================================================
 # structures and sequences
 # ===============================================================================
 # this can maybe made better when variadic generics are available
-class Struct(Construct[ParsedType, BuildTypes]):
+class Struct(Construct[Container[t.Any], t.Optional[t.Dict[str, t.Any]]]):
     subcons: t.List[Construct[t.Any, t.Any]]
     _subcons: t.Dict[str, Construct[t.Any, t.Any]]
-    def __new__(
-        cls,
-        *subcons: Construct[t.Any, t.Any],
-        **subconskw: Construct[t.Any, t.Any],
-    ) -> Struct[Container[t.Any], t.Optional[t.Dict[str, t.Any]]]: ...
     def __init__(
-        self: Struct[Container[t.Any], t.Optional[t.Dict[str, t.Any]]],
+        self,
         *subcons: Construct[t.Any, t.Any],
         **subconskw: Construct[t.Any, t.Any],
     ) -> None: ...
     def __getattr__(self, name: str) -> t.Any: ...
 
 # this can maybe made better when variadic generics are available
-class Sequence(Construct[ParsedType, BuildTypes]):
+class Sequence(Construct[ListContainer[t.Any], t.Optional[t.List[t.Any]]]):
     subcons: t.List[Construct[t.Any, t.Any]]
     _subcons: t.Dict[str, Construct[t.Any, t.Any]]
-    def __new__(
-        cls,
-        *subcons: Construct[t.Any, t.Any],
-        **subconskw: Construct[t.Any, t.Any],
-    ) -> Sequence[ListContainer[t.Any], t.Optional[t.List[t.Any]]]: ...
     def __init__(
-        self: Sequence[ListContainer[t.Any], t.Optional[t.List[t.Any]]],
+        self,
         *subcons: Construct[t.Any, t.Any],
         **subconskw: Construct[t.Any, t.Any],
     ) -> None: ...
     def __getattr__(self, name: str) -> t.Any: ...
 
 # ===============================================================================
 # arrays ranges and repeaters
 # ===============================================================================
 class Array(
     Subconstruct[
         SubconParsedType,
         SubconBuildTypes,
-        ParsedType,
-        BuildTypes,
+        ListContainer[SubconParsedType],  # type: ignore
+        t.List[SubconBuildTypes],  # type: ignore
     ]
 ):
     count: ConstantOrContextLambda[int]
     discard: bool
-    def __new__(
-        cls,
-        count: ConstantOrContextLambda[int],
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-        discard: bool = ...,
-    ) -> Array[
-        SubconParsedType,
-        SubconBuildTypes,
-        ListContainer[SubconParsedType],
-        t.List[SubconBuildTypes],
-    ]: ...
     def __init__(
-        self: Array[
-            SubconParsedType,
-            SubconBuildTypes,
-            ListContainer[SubconParsedType],
-            t.List[SubconBuildTypes],
-        ],
+        self,
         count: ConstantOrContextLambda[int],
         subcon: Construct[SubconParsedType, SubconBuildTypes],
         discard: bool = ...,
     ) -> None: ...
 
 class GreedyRange(
     Subconstruct[
         SubconParsedType,
         SubconBuildTypes,
-        ParsedType,
-        BuildTypes,
+        ListContainer[SubconParsedType],  # type: ignore
+        t.List[SubconBuildTypes],  # type: ignore
     ]
 ):
     discard: bool
-    def __new__(
-        cls,
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-        discard: bool = ...,
-    ) -> GreedyRange[
-        SubconParsedType,
-        SubconBuildTypes,
-        ListContainer[SubconParsedType],
-        t.List[SubconBuildTypes],
-    ]: ...
     def __init__(
-        self: GreedyRange[
-            SubconParsedType,
-            SubconBuildTypes,
-            ListContainer[SubconParsedType],
-            t.List[SubconBuildTypes],
-        ],
+        self,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
         discard: bool = ...,
     ) -> None: ...
 
 class RepeatUntil(
     Subconstruct[
         SubconParsedType,
         SubconBuildTypes,
-        ParsedType,
-        BuildTypes,
+        ListContainer[SubconParsedType],  # type: ignore
+        t.List[SubconBuildTypes],  # type: ignore
     ]
 ):
     predicate: t.Union[
         bool,
         t.Callable[[SubconParsedType, ListContainer[SubconParsedType], Context], bool],
     ]
     discard: bool
-    def __new__(
-        cls,
-        predicate: t.Union[
-            bool,
-            t.Callable[
-                [SubconParsedType, ListContainer[SubconParsedType], Context], bool
-            ],
-        ],
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-        discard: bool = ...,
-    ) -> RepeatUntil[
-        SubconParsedType,
-        SubconBuildTypes,
-        ListContainer[SubconParsedType],
-        t.List[SubconBuildTypes],
-    ]: ...
     def __init__(
-        self: RepeatUntil[
-            SubconParsedType,
-            SubconBuildTypes,
-            ListContainer[SubconParsedType],
-            t.List[SubconBuildTypes],
-        ],
+        self,
         predicate: t.Union[
             bool,
             t.Callable[
                 [SubconParsedType, ListContainer[SubconParsedType], Context], bool
             ],
         ],
         subcon: Construct[SubconParsedType, SubconBuildTypes],
@@ -678,97 +543,64 @@
         newdocs: t.Optional[str] = ...,
         newparsed: t.Optional[t.Callable[[t.Any, Context], None]] = ...,
     ) -> None: ...
 
 # ===============================================================================
 # miscellaneous
 # ===============================================================================
-class Const(Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
-    value: SubconBuildTypes
+class Const(Subconstruct[t.Any, t.Any, ParsedType, BuildTypes]):
+    value: BuildTypes
     @t.overload
     def __new__(
-        cls,
+        cls: "type[Const[bytes, t.Optional[bytes]]]",
         value: bytes,
-    ) -> Const[None, None, bytes, t.Optional[bytes]]: ...
+    ) -> Const[bytes, t.Optional[bytes]]: ...
     @t.overload
     def __new__(
-        cls,
+        cls: "type[Const[SubconParsedType, t.Optional[SubconBuildTypes]]]",
         value: SubconBuildTypes,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> Const[None, None, SubconParsedType, t.Optional[SubconBuildTypes]]: ...
+    ) -> Const[SubconParsedType, t.Optional[SubconBuildTypes]]: ...
 
-class Computed(Construct[ParsedType, BuildTypes]):
+class Computed(Construct[ParsedType, None]):
     func: ConstantOrContextLambda2[ParsedType]
-    @t.overload
-    def __new__(
-        cls,
-        func: ConstantOrContextLambda2[ParsedType],
-    ) -> Computed[ParsedType, None]: ...
-    @t.overload
-    def __new__(
-        cls,
-        func: ConstantOrContextLambda2[t.Any],
-    ) -> Computed[t.Any, None]: ...
-    @t.overload
     def __init__(
-        self: Computed[ParsedType, None],
+        self,
         func: ConstantOrContextLambda2[ParsedType],
     ) -> None: ...
-    @t.overload
-    def __init__(
-        self: Computed[t.Any, None],
-        func: ConstantOrContextLambda2[t.Any],
-    ) -> None: ...
 
 Index: Construct[int, t.Any]
 
-class Rebuild(Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
+class Rebuild(Subconstruct[SubconParsedType, SubconBuildTypes, SubconParsedType, None]):
     func: ConstantOrContextLambda[SubconBuildTypes]
-    def __new__(
-        cls,
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-        func: ConstantOrContextLambda[SubconBuildTypes],
-    ) -> Rebuild[SubconParsedType, SubconBuildTypes, SubconParsedType, None]: ...
     def __init__(
-        self: Rebuild[SubconParsedType, SubconBuildTypes, SubconParsedType, None],
+        self,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
         func: ConstantOrContextLambda[SubconBuildTypes],
     ) -> None: ...
 
-class Default(Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
-    value: ConstantOrContextLambda[SubconBuildTypes]
-    def __new__(
-        cls,
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-        value: ConstantOrContextLambda[SubconBuildTypes],
-    ) -> Default[
+class Default(
+    Subconstruct[
         SubconParsedType,
         SubconBuildTypes,
         SubconParsedType,
         t.Optional[SubconBuildTypes],
-    ]: ...
+    ]
+):
+    value: ConstantOrContextLambda[SubconBuildTypes]
     def __init__(
-        self: Default[
-            SubconParsedType,
-            SubconBuildTypes,
-            SubconParsedType,
-            t.Optional[SubconBuildTypes],
-        ],
+        self,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
         value: ConstantOrContextLambda[SubconBuildTypes],
     ) -> None: ...
 
-class Check(Construct[ParsedType, BuildTypes]):
+class Check(Construct[None, None]):
     func: ConstantOrContextLambda[bool]
-    def __new__(
-        cls,
-        func: ConstantOrContextLambda[bool],
-    ) -> Check[None, None]: ...
     def __init__(
-        self: Check[None, None],
+        self,
         func: ConstantOrContextLambda[bool],
     ) -> None: ...
 
 Error: Construct[None, None]
 
 class FocusedSeq(Construct[t.Any, t.Any]):
     subcons: t.List[Construct[t.Any, t.Any]]
@@ -785,39 +617,23 @@
 
 Numpy: Construct[t.Any, t.Any]
 
 class NamedTuple(
     Adapter[
         SubconParsedType,
         SubconBuildTypes,
-        ParsedType,
-        BuildTypes,
+        t.Tuple[t.Any, ...],
+        t.Union[t.Tuple[t.Any, ...], t.List[t.Any], t.Dict[str, t.Any]],
     ]
 ):
     tuplename: str
     tuplefields: str
     factory: Construct[SubconParsedType, SubconBuildTypes]
-    def __new__(
-        cls,
-        tuplename: str,
-        tuplefields: str,
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> NamedTuple[
-        SubconParsedType,
-        SubconBuildTypes,
-        t.Tuple[t.Any, ...],
-        t.Union[t.Tuple[t.Any, ...], t.List[t.Any], t.Dict[str, t.Any]],
-    ]: ...
     def __init__(
-        self: NamedTuple[
-            SubconParsedType,
-            SubconBuildTypes,
-            t.Tuple[t.Any, ...],
-            t.Union[t.Tuple[t.Any, ...], t.List[t.Any], t.Dict[str, t.Any]],
-        ],
+        self,
         tuplename: str,
         tuplefields: str,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
     ) -> None: ...
 
 if sys.version_info >= (3, 8):
     MSDOS = t.Literal["msdos"]
@@ -844,134 +660,68 @@
     unit: t.Union[int, float],
     epoch: t.Union[int, arrow.Arrow],
 ) -> TimestampAdapter[float, float]: ...
 
 K = t.TypeVar("K")
 V = t.TypeVar("V")
 
-class Hex(Adapter[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
+class Hex(Adapter[t.Any, t.Any, ParsedType, BuildTypes]):
     @t.overload
     def __new__(
-        cls, subcon: Construct[int, BuildTypes]
-    ) -> Hex[int, BuildTypes, HexDisplayedInteger, BuildTypes]: ...
+        cls: "type[Hex[HexDisplayedInteger, BuildTypes]]",
+        subcon: Construct[int, BuildTypes],
+    ) -> Hex[HexDisplayedInteger, BuildTypes]: ...
     @t.overload
     def __new__(
-        cls, subcon: Construct[bytes, BuildTypes]
-    ) -> Hex[bytes, BuildTypes, HexDisplayedBytes, BuildTypes]: ...
+        cls: "type[Hex[HexDisplayedBytes, BuildTypes]]",
+        subcon: Construct[bytes, BuildTypes],
+    ) -> Hex[HexDisplayedBytes, BuildTypes]: ...
     @t.overload
     def __new__(
-        cls, subcon: Construct[RawCopyObj[SubconParsedType], BuildTypes]
+        cls: "type[Hex[HexDisplayedDict[str, t.Union[int, bytes, SubconParsedType]], BuildTypes,]]",
+        subcon: Construct[RawCopyObj[SubconParsedType], BuildTypes],
     ) -> Hex[
-        RawCopyObj[SubconParsedType],
-        BuildTypes,
         HexDisplayedDict[str, t.Union[int, bytes, SubconParsedType]],
         BuildTypes,
     ]: ...
     @t.overload
     def __new__(
-        cls, subcon: Construct[Container[t.Any], BuildTypes]
-    ) -> Hex[
-        Container[t.Any], BuildTypes, HexDisplayedDict[str, t.Any], BuildTypes
-    ]: ...
-    @t.overload
-    def __new__(
-        cls, subcon: Construct[SubconParsedType, SubconBuildTypes]
-    ) -> Hex[
-        SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes
-    ]: ...
-    @t.overload
-    def __init__(
-        self: Hex[int, BuildTypes, HexDisplayedInteger, BuildTypes],
-        subcon: Construct[int, BuildTypes],
-    ) -> None: ...
-    @t.overload
-    def __init__(
-        self: Hex[bytes, BuildTypes, HexDisplayedBytes, BuildTypes],
-        subcon: Construct[bytes, BuildTypes],
-    ) -> None: ...
-    @t.overload
-    def __init__(
-        self: Hex[
-            RawCopyObj[SubconParsedType],
-            BuildTypes,
-            HexDisplayedDict[str, t.Union[int, bytes, SubconParsedType]],
-            BuildTypes,
-        ],
-        subcon: Construct[RawCopyObj[SubconParsedType], BuildTypes],
-    ) -> None: ...
-    @t.overload
-    def __init__(
-        self: Hex[
-            Container[t.Any], BuildTypes, HexDisplayedDict[str, t.Any], BuildTypes
-        ],
+        cls: "type[Hex[HexDisplayedDict[str, t.Any], BuildTypes]]",
         subcon: Construct[Container[t.Any], BuildTypes],
-    ) -> None: ...
+    ) -> Hex[HexDisplayedDict[str, t.Any], BuildTypes]: ...
     @t.overload
-    def __init__(
-        self: Hex[
-            SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes
-        ],
+    def __new__(
+        cls: "type[Hex[SubconParsedType, SubconBuildTypes]]",
         subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> None: ...
+    ) -> Hex[SubconParsedType, SubconBuildTypes]: ...
 
-class HexDump(Adapter[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
+class HexDump(Adapter[t.Any, t.Any, ParsedType, BuildTypes]):
     @t.overload
     def __new__(
-        cls, subcon: Construct[bytes, BuildTypes]
-    ) -> HexDump[bytes, BuildTypes, HexDumpDisplayedBytes, BuildTypes]: ...
+        cls: "type[HexDump[HexDumpDisplayedBytes, BuildTypes]]",
+        subcon: Construct[bytes, BuildTypes],
+    ) -> HexDump[HexDumpDisplayedBytes, BuildTypes]: ...
     @t.overload
     def __new__(
-        cls, subcon: Construct[RawCopyObj[SubconParsedType], BuildTypes]
+        cls: "type[HexDump[HexDumpDisplayedDict[str, t.Union[int, bytes, SubconParsedType]],BuildTypes,]]",
+        subcon: Construct[RawCopyObj[SubconParsedType], BuildTypes],
     ) -> HexDump[
-        RawCopyObj[SubconParsedType],
-        BuildTypes,
         HexDumpDisplayedDict[str, t.Union[int, bytes, SubconParsedType]],
         BuildTypes,
     ]: ...
     @t.overload
     def __new__(
-        cls, subcon: Construct[Container[t.Any], BuildTypes]
-    ) -> HexDump[
-        Container[t.Any], BuildTypes, HexDumpDisplayedDict[str, t.Any], BuildTypes
-    ]: ...
-    @t.overload
-    def __new__(
-        cls, subcon: Construct[SubconParsedType, SubconBuildTypes]
-    ) -> HexDump[
-        SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes
-    ]: ...
-    @t.overload
-    def __init__(
-        self: HexDump[bytes, BuildTypes, HexDumpDisplayedBytes, BuildTypes],
-        subcon: Construct[bytes, BuildTypes],
-    ) -> None: ...
-    @t.overload
-    def __init__(
-        self: HexDump[
-            RawCopyObj[SubconParsedType],
-            BuildTypes,
-            HexDumpDisplayedDict[str, t.Union[int, bytes, SubconParsedType]],
-            BuildTypes,
-        ],
-        subcon: Construct[RawCopyObj[SubconParsedType], BuildTypes],
-    ) -> None: ...
-    @t.overload
-    def __init__(
-        self: HexDump[
-            Container[t.Any], BuildTypes, HexDumpDisplayedDict[str, t.Any], BuildTypes
-        ],
+        cls: "type[HexDump[HexDumpDisplayedDict[str, t.Any], BuildTypes]]",
         subcon: Construct[Container[t.Any], BuildTypes],
-    ) -> None: ...
+    ) -> HexDump[HexDumpDisplayedDict[str, t.Any], BuildTypes]: ...
     @t.overload
-    def __init__(
-        self: HexDump[
-            SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes
-        ],
+    def __new__(
+        cls: "type[HexDump[SubconParsedType, SubconBuildTypes]]",
         subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> None: ...
+    ) -> HexDump[SubconParsedType, SubconBuildTypes]: ...
 
 # ===============================================================================
 # conditional
 # ===============================================================================
 # this can maybe made better when variadic generics are available
 class Union(Construct[Container[t.Any], t.Dict[str, t.Any]]):
     parsefrom: t.Optional[ConstantOrContextLambda[t.Union[int, str]]]
@@ -982,97 +732,80 @@
         parsefrom: t.Optional[ConstantOrContextLambda[t.Union[int, str]]],
         *subcons: Construct[t.Any, t.Any],
         **subconskw: Construct[t.Any, t.Any],
     ) -> None: ...
     def __getattr__(self, name: str) -> t.Any: ...
 
 # this can maybe made better when variadic generics are available
-class Select(Construct[ParsedType, BuildTypes]):
+class Select(Construct[t.Any, t.Any]):
     subcons: t.List[Construct[t.Any, t.Any]]
-    def __new__(
-        cls,
-        *subcons: Construct[t.Any, t.Any],
-        **subconskw: Construct[t.Any, t.Any],
-    ) -> Select[t.Any, t.Any]: ...
     def __init__(
-        self: Select[t.Any, t.Any],
+        self,
         *subcons: Construct[t.Any, t.Any],
         **subconskw: Construct[t.Any, t.Any],
     ) -> None: ...
 
 def Optional(
     subcon: Construct[SubconParsedType, SubconBuildTypes]
-) -> Select[t.Union[SubconParsedType, None], t.Union[SubconBuildTypes, None]]: ...
+) -> Construct[t.Union[SubconParsedType, None], t.Union[SubconBuildTypes, None]]: ...
 
 ThenParsedType = t.TypeVar("ThenParsedType")
 ThenBuildTypes = t.TypeVar("ThenBuildTypes")
 ElseParsedType = t.TypeVar("ElseParsedType")
 ElseBuildTypes = t.TypeVar("ElseBuildTypes")
 
 class IfThenElse(Construct[ParsedType, BuildTypes]):
     condfunc: ConstantOrContextLambda[bool]
-    thensubcon: Construct[ParsedType, BuildTypes]
-    elsesubcon: Construct[ParsedType, BuildTypes]
+    thensubcon: Construct[t.Any, t.Any]
+    elsesubcon: Construct[t.Any, t.Any]
+    @t.overload
     def __new__(
-        cls,
+        cls: "type[IfThenElse[t.Union[ThenParsedType, ElseParsedType], t.Union[ThenBuildTypes, ElseBuildTypes]]]",
         condfunc: ConstantOrContextLambda[bool],
         thensubcon: Construct[ThenParsedType, ThenBuildTypes],
         elsesubcon: Construct[ElseParsedType, ElseBuildTypes],
-    ) -> IfThenElse[
-        t.Union[ThenParsedType, ElseParsedType], t.Union[ThenBuildTypes, ElseBuildTypes]
-    ]: ...
+    ) -> "IfThenElse[t.Union[ThenParsedType, ElseParsedType], t.Union[ThenBuildTypes, ElseBuildTypes]]": ...
+    @t.overload
+    def __new__(
+        cls: "type[IfThenElse[t.Any, t.Any]]",
+        condfunc: ConstantOrContextLambda[bool],
+        thensubcon: Construct[t.Any, t.Any],
+        elsesubcon: Construct[t.Any, t.Any],
+    ) -> "IfThenElse[t.Any, t.Any]": ...
 
 def If(
     condfunc: ConstantOrContextLambda[bool],
     subcon: Construct[ThenParsedType, ThenBuildTypes],
-) -> IfThenElse[t.Union[ThenParsedType, None], t.Union[ThenBuildTypes, None]]: ...
+) -> IfThenElse[t.Optional[ThenParsedType], t.Optional[ThenBuildTypes]]: ...
 
 SwitchType = t.TypeVar("SwitchType")
 
 class Switch(Construct[ParsedType, BuildTypes]):
     keyfunc: ConstantOrContextLambda[t.Any]
     cases: t.Dict[t.Any, Construct[t.Any, t.Any]]
     default: Construct[t.Any, t.Any]
     @t.overload
     def __new__(
-        cls,
+        cls: "type[Switch[int, t.Optional[int]]]",
         keyfunc: ConstantOrContextLambda[SwitchType],
         cases: t.Dict[SwitchType, Construct[int, int]],
         default: t.Optional[Construct[int, int]] = ...,
     ) -> Switch[int, t.Optional[int]]: ...
     @t.overload
     def __new__(
-        cls,
+        cls: "type[Switch[t.Any, t.Any]]",
         keyfunc: ConstantOrContextLambda[t.Any],
         cases: t.Dict[t.Any, Construct[t.Any, t.Any]],
         default: t.Optional[Construct[t.Any, t.Any]] = ...,
     ) -> Switch[t.Any, t.Any]: ...
-    @t.overload
-    def __init__(
-        self: Switch[int, t.Optional[int]],
-        keyfunc: ConstantOrContextLambda[SwitchType],
-        cases: t.Dict[SwitchType, Construct[int, int]],
-        default: t.Optional[Construct[int, int]] = ...,
-    ) -> None: ...
-    @t.overload
-    def __init__(
-        self: Switch[t.Any, t.Any],
-        keyfunc: ConstantOrContextLambda[t.Any],
-        cases: t.Dict[t.Any, Construct[t.Any, t.Any]],
-        default: t.Optional[Construct[t.Any, t.Any]] = ...,
-    ) -> None: ...
 
-class StopIf(Construct[ParsedType, BuildTypes]):
+class StopIf(Construct[None, None]):
     condfunc: ConstantOrContextLambda[bool]
-    def __new__(
-        cls,
-        condfunc: ConstantOrContextLambda[bool],
-    ) -> StopIf[None, None]: ...
     def __init__(
-        self: StopIf[None, None],
+        self,
         condfunc: ConstantOrContextLambda[bool],
     ) -> None: ...
 
 # ===============================================================================
 # alignment and padding
 # ===============================================================================
 def Padding(
@@ -1103,15 +836,15 @@
         pattern: bytes = ...,
     ) -> None: ...
 
 def AlignedStruct(
     modulus: ConstantOrContextLambda[int],
     *subcons: Construct[t.Any, t.Any],
     **subconskw: Construct[t.Any, t.Any],
-) -> Struct[Container[t.Any], t.Optional[t.Dict[str, t.Any]]]: ...
+) -> Struct: ...
 def BitStruct(
     *subcons: Construct[t.Any, t.Any], **subconskw: Construct[t.Any, t.Any]
 ) -> t.Union[
     Transformed[Container[t.Any], t.Dict[str, t.Any]],
     Restreamed[Container[t.Any], t.Dict[str, t.Any]],
 ]: ...
 
@@ -1126,31 +859,24 @@
     def __init__(
         self,
         offset: ConstantOrContextLambda[int],
         subcon: Construct[SubconParsedType, SubconBuildTypes],
         stream: t.Optional[t.Callable[[Context], StreamType]] = ...,
     ) -> None: ...
 
-class Peek(Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
-    def __new__(
-        cls,
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> Peek[
+class Peek(
+    Subconstruct[
         SubconParsedType,
         SubconBuildTypes,
         SubconParsedType,
         t.Union[SubconBuildTypes, None],
-    ]: ...
+    ]
+):
     def __init__(
-        self: Peek[
-            SubconParsedType,
-            SubconBuildTypes,
-            SubconParsedType,
-            t.Union[SubconBuildTypes, None],
-        ],
+        self,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
     ) -> None: ...
 
 class Seek(Construct[int, None]):
     at: ConstantOrContextLambda[int]
     if sys.version_info >= (3, 8):
         WHENCE = t.Literal[0, 1, 2]
@@ -1174,31 +900,24 @@
 class RawCopyObj(t.Generic[ParsedType], Container[t.Any]):
     data: bytes
     value: ParsedType
     offset1: int
     offset2: int
     length: int
 
-class RawCopy(Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
-    def __new__(
-        cls,
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> RawCopy[
+class RawCopy(
+    Subconstruct[
         SubconParsedType,
         SubconBuildTypes,
         RawCopyObj[SubconParsedType],
         t.Optional[t.Dict[str, t.Union[SubconBuildTypes, bytes]]],
-    ]: ...
+    ]
+):
     def __init__(
-        self: RawCopy[
-            SubconParsedType,
-            SubconBuildTypes,
-            RawCopyObj[SubconParsedType],
-            t.Optional[t.Dict[str, t.Union[SubconBuildTypes, bytes]]],
-        ],
+        self,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
     ) -> None: ...
 
 def ByteSwapped(
     subcon: Construct[SubconParsedType, SubconBuildTypes]
 ) -> Transformed[SubconParsedType, SubconBuildTypes]: ...
 def BitsSwapped(
@@ -1219,20 +938,15 @@
         subcon: Construct[SubconParsedType, SubconBuildTypes],
         includelength: t.Optional[bool] = ...,
     ) -> None: ...
 
 def PrefixedArray(
     countfield: Construct[int, int],
     subcon: Construct[SubconParsedType, SubconBuildTypes],
-) -> Array[
-    SubconParsedType,
-    SubconBuildTypes,
-    ListContainer[SubconParsedType],
-    t.List[SubconBuildTypes],
-]: ...
+) -> Array[SubconParsedType, SubconBuildTypes,]: ...
 
 class FixedSized(
     Subconstruct[SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes]
 ):
     length: ConstantOrContextLambda[int]
     def __init__(
         self,
@@ -1257,15 +971,17 @@
     ) -> None: ...
 
 class NullStripped(
     Subconstruct[SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes]
 ):
     pad: bytes
     def __init__(
-        self, subcon: Construct[SubconParsedType, SubconBuildTypes], pad: bytes = ...
+        self,
+        subcon: Construct[SubconParsedType, SubconBuildTypes],
+        pad: bytes = ...,
     ) -> None: ...
 
 class RestreamData(
     Subconstruct[SubconParsedType, SubconBuildTypes, SubconParsedType, None]
 ):
     datafunc: t.Union[
         bytes, io.BytesIO, Construct[bytes, t.Any], t.Callable[[Context], bytes]
@@ -1312,38 +1028,27 @@
         sizecomputer: t.Callable[[int], int],
     ) -> None: ...
 
 class ProcessXor(
     Subconstruct[SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes]
 ):
     padfunc: ConstantOrContextLambda2[t.Union[int, bytes]]
-    def __new__(
-        cls,
-        padfunc: ConstantOrContextLambda2[t.Union[int, bytes]],
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> ProcessXor[SubconParsedType, SubconBuildTypes]: ...
     def __init__(
-        self: ProcessXor[SubconParsedType, SubconBuildTypes],
+        self,
         padfunc: ConstantOrContextLambda2[t.Union[int, bytes]],
         subcon: Construct[SubconParsedType, SubconBuildTypes],
     ) -> None: ...
 
 class ProcessRotateLeft(
     Subconstruct[SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes]
 ):
     amount: ConstantOrContextLambda2[int]
     group: ConstantOrContextLambda2[int]
-    def __new__(
-        cls,
-        amount: ConstantOrContextLambda2[int],
-        group: ConstantOrContextLambda2[int],
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> ProcessRotateLeft[SubconParsedType, SubconBuildTypes]: ...
     def __init__(
-        self: ProcessRotateLeft[SubconParsedType, SubconBuildTypes],
+        self,
         amount: ConstantOrContextLambda2[int],
         group: ConstantOrContextLambda2[int],
         subcon: Construct[SubconParsedType, SubconBuildTypes],
     ) -> None: ...
 
 T = t.TypeVar("T")
 
@@ -1385,97 +1090,66 @@
         subcon: Construct[SubconParsedType, SubconBuildTypes],
         tailcutoff: t.Optional[int] = ...,
     ) -> None: ...
 
 # ===============================================================================
 # lazy equivalents
 # ===============================================================================
-class Lazy(Subconstruct[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
-    def __new__(
-        cls,
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> Lazy[
+class Lazy(
+    Subconstruct[
         SubconParsedType,
         SubconBuildTypes,
         t.Callable[[], SubconParsedType],
         t.Union[t.Callable[[], SubconParsedType], SubconParsedType],
-    ]: ...
+    ]
+):
     def __init__(
-        self: Lazy[
-            SubconParsedType,
-            SubconBuildTypes,
-            t.Callable[[], SubconParsedType],
-            t.Union[t.Callable[[], SubconParsedType], SubconParsedType],
-        ],
+        self,
         subcon: Construct[SubconParsedType, SubconBuildTypes],
     ) -> None: ...
 
 class LazyContainer(t.Generic[ContainerType], t.Dict[str, ContainerType]):
     def __getattr__(self, name: str) -> ContainerType: ...
     def __getitem__(self, index: t.Union[str, int]) -> ContainerType: ...
     def keys(self) -> t.Iterator[str]: ...
     def values(self) -> t.List[ContainerType]: ...
     def items(self) -> t.List[t.Tuple[str, ContainerType]]: ...
 
-class LazyStruct(Construct[ParsedType, BuildTypes]):
+class LazyStruct(Construct[LazyContainer[t.Any], t.Optional[t.Dict[str, t.Any]]]):
     subcons: t.List[Construct[t.Any, t.Any]]
     _subcons: t.Dict[str, Construct[t.Any, t.Any]]
     _subconsindexes: t.Dict[str, int]
-    def __new__(
-        cls,
-        *subcons: Construct[t.Any, t.Any],
-        **subconskw: Construct[t.Any, t.Any],
-    ) -> LazyStruct[LazyContainer[t.Any], t.Optional[t.Dict[str, t.Any]]]: ...
     def __init__(
-        self: LazyStruct[LazyContainer[t.Any], t.Optional[t.Dict[str, t.Any]]],
+        self,
         *subcons: Construct[t.Any, t.Any],
         **subconskw: Construct[t.Any, t.Any],
     ) -> None: ...
     def __getattr__(self, name: str) -> t.Any: ...
 
 class LazyListContainer(t.List[ListType]): ...
 
 class LazyArray(
     Subconstruct[
         SubconParsedType,
         SubconBuildTypes,
-        ParsedType,
-        BuildTypes,
+        ListContainer[SubconParsedType],  # type: ignore
+        t.List[SubconBuildTypes],  # type: ignore
     ]
 ):
     count: ConstantOrContextLambda[int]
-    def __new__(
-        cls,
-        count: ConstantOrContextLambda[int],
-        subcon: Construct[SubconParsedType, SubconBuildTypes],
-    ) -> LazyArray[
-        SubconParsedType,
-        SubconBuildTypes,
-        ListContainer[SubconParsedType],
-        t.List[SubconBuildTypes],
-    ]: ...
     def __init__(
-        self: LazyArray[
-            SubconParsedType,
-            SubconBuildTypes,
-            ListContainer[SubconParsedType],
-            t.List[SubconBuildTypes],
-        ],
+        self,
         count: ConstantOrContextLambda[int],
         subcon: Construct[SubconParsedType, SubconBuildTypes],
     ) -> None: ...
 
 class LazyBound(Construct[ParsedType, BuildTypes]):
     subconfunc: t.Callable[[], Construct[ParsedType, BuildTypes]]
-    def __new__(
-        cls,
-        subconfunc: t.Callable[[], Construct[ParsedType, BuildTypes]],
-    ) -> LazyBound[ParsedType, BuildTypes]: ...
     def __init__(
-        self: LazyBound[ParsedType, BuildTypes],
+        self,
         subconfunc: t.Callable[[], Construct[ParsedType, BuildTypes]],
     ) -> None: ...
 
 # ===============================================================================
 # adapters and validators
 # ===============================================================================
 class ExprAdapter(Adapter[SubconParsedType, SubconBuildTypes, ParsedType, BuildTypes]):
@@ -1514,52 +1188,31 @@
     predicate: t.Callable[[SubconParsedType, Context], bool],
     subcon: Construct[SubconParsedType, SubconBuildTypes],
 ) -> ExprSymmetricAdapter[
     SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes
 ]: ...
 
 class Slicing(
-    Adapter[SubconParsedType, SubconBuildTypes, SubconParsedType, SubconBuildTypes]
+    Adapter[
+        SubconParsedType,
+        SubconBuildTypes,
+        ListContainer[SubconParsedType],  # type: ignore
+        t.List[SubconBuildTypes],  # type: ignore
+    ]
 ):
-    def __new__(
-        cls,
-        subcon: t.Union[
-            Array[
-                SubconParsedType,
-                SubconBuildTypes,
-                ListContainer[SubconParsedType],
-                t.List[SubconBuildTypes],
-            ],
-            GreedyRange[
-                SubconParsedType,
-                SubconBuildTypes,
-                ListContainer[SubconParsedType],
-                t.List[SubconBuildTypes],
-            ],
-        ],
-        count: int,
-        start: t.Optional[int],
-        stop: t.Optional[int],
-        step: int = ...,
-        empty: t.Optional[SubconParsedType] = ...,
-    ) -> Slicing[ListContainer[SubconParsedType], t.List[SubconBuildTypes]]: ...
     def __init__(
-        self: Slicing[ListContainer[SubconParsedType], t.List[SubconBuildTypes]],
+        self,
         subcon: t.Union[
             Array[
                 SubconParsedType,
                 SubconBuildTypes,
-                ListContainer[SubconParsedType],
-                t.List[SubconBuildTypes],
             ],
             GreedyRange[
                 SubconParsedType,
                 SubconBuildTypes,
-                ListContainer[SubconParsedType],
-                t.List[SubconBuildTypes],
             ],
         ],
         count: int,
         start: t.Optional[int],
         stop: t.Optional[int],
         step: int = ...,
         empty: t.Optional[SubconParsedType] = ...,
@@ -1570,21 +1223,17 @@
 ):
     def __init__(
         self,
         subcon: t.Union[
             Array[
                 SubconParsedType,
                 SubconBuildTypes,
-                ListContainer[SubconParsedType],
-                t.List[SubconBuildTypes],
             ],
             GreedyRange[
                 SubconParsedType,
                 SubconBuildTypes,
-                ListContainer[SubconParsedType],
-                t.List[SubconBuildTypes],
             ],
         ],
         count: int,
         index: int,
         empty: t.Optional[SubconParsedType] = ...,
     ) -> None: ...
```

### Comparing `construct-typing-0.5.6/construct-stubs/expr.pyi` & `construct-typing-0.6.0/construct-stubs/expr.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import operator
 import typing as t
 
 from construct.core import *
 
 UniOperator = t.Callable[[t.Any], t.Any]
 BinOperator = t.Callable[[t.Any, t.Any], t.Any]
 
@@ -494,33 +493,33 @@
     @t.overload
     def __neg__(self: ExprMixin[int]) -> BinExpr[int]: ...
     @t.overload
     def __neg__(self: ExprMixin[bool]) -> BinExpr[int]: ...
     @t.overload
     def __neg__(self: ExprMixin[float]) -> BinExpr[float]: ...
     @t.overload
-    def __neg__(self) -> UniExpr[t.Any]: ...
+    def __neg__(self) -> BinExpr[t.Any]: ...
 
     # __pos__ ##########################################################################################################
     @t.overload
     def __pos__(self: ExprMixin[int]) -> BinExpr[int]: ...
     @t.overload
     def __pos__(self: ExprMixin[bool]) -> BinExpr[int]: ...
     @t.overload
     def __pos__(self: ExprMixin[float]) -> BinExpr[float]: ...
     @t.overload
-    def __pos__(self) -> UniExpr[t.Any]: ...
+    def __pos__(self) -> BinExpr[t.Any]: ...
 
     # __invert__ #######################################################################################################
     @t.overload
     def __invert__(self: ExprMixin[int]) -> BinExpr[int]: ...
     @t.overload
     def __invert__(self: ExprMixin[bool]) -> BinExpr[int]: ...
     @t.overload
-    def __invert__(self) -> UniExpr[t.Any]: ...
+    def __invert__(self) -> BinExpr[t.Any]: ...
 
     # __inv__ ##########################################################################################################
     def __inv__(self) -> UniExpr[t.Any]: ...
 
 class UniExpr(ExprMixin[ReturnType]):
     def __init__(self, op: UniOperator, operand: t.Any) -> None: ...
     def __call__(self, obj: t.Union[Context, dict[str, t.Any], t.Any], *args: t.Any) -> ReturnType: ...
```

### Comparing `construct-typing-0.5.6/construct-stubs/lib/__init__.pyi` & `construct-typing-0.6.0/construct-stubs/lib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/construct-stubs/lib/binary.pyi` & `construct-typing-0.6.0/construct-stubs/lib/binary.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/construct-stubs/lib/bitstream.pyi` & `construct-typing-0.6.0/construct-stubs/lib/bitstream.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/construct-stubs/lib/containers.pyi` & `construct-typing-0.6.0/construct-stubs/lib/containers.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/construct-stubs/lib/py3compat.pyi` & `construct-typing-0.6.0/construct-stubs/lib/py3compat.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typing as t
 
+PY: t.Tuple[int, int]
 PY2: bool
 PY3: bool
 PYPY: bool
 ONWINDOWS: bool
 
 stringtypes: t.Tuple[t.Type[bytes], t.Type[str]]
 integertypes: t.Tuple[t.Type[int]]
```

### Comparing `construct-typing-0.5.6/construct_typed/__init__.py` & `construct-typing-0.6.0/construct_typed/__init__.py`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/construct_typed/dataclass_struct.py` & `construct-typing-0.6.0/construct_typed/dataclass_struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,18 @@
         default = None
     else:
         init = True
         default = dataclasses.MISSING
 
     # Set default values in case of special sucons
     if isinstance(orig_subcon, cs.Const):
-        const_subcon: "cs.Const[t.Any, t.Any, t.Any, t.Any]" = orig_subcon
+        const_subcon: "cs.Const[t.Any, t.Any]" = orig_subcon
         default = const_subcon.value
     elif isinstance(orig_subcon, cs.Default):
-        default_subcon: "cs.Default[t.Any, t.Any, t.Any, t.Any]" = orig_subcon
+        default_subcon: "cs.Default[t.Any, t.Any]" = orig_subcon
         if callable(default_subcon.value):
             default = None  # context lambda is only defined at parsing/building
         else:
             default = default_subcon.value
 
     return t.cast(
         ParsedType,
@@ -148,15 +148,15 @@
         ...     height: int = csfield(Int8ub)
         ...     pixels: bytes = csfield(Bytes(this.height * this.width))
         >>> d = DataclassStruct(Image)
         >>> d.parse(b"\x01\x0212")
         Image(width=1, height=2, pixels=b'12')
     """
 
-    subcon: "cs.Struct[t.Any, t.Any]"
+    subcon: "cs.Struct"
     if t.TYPE_CHECKING:
 
         def __new__(
             cls,
             dc_type: t.Type[DataclassType],
             reverse: bool = False,
         ) -> "DataclassStruct[DataclassType]":
```

### Comparing `construct-typing-0.5.6/construct_typed/generic_wrapper.py` & `construct-typing-0.6.0/construct_typed/generic_wrapper.py`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/construct_typed/tenum.py` & `construct-typing-0.6.0/construct_typed/tenum.py`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/construct_typing.egg-info/PKG-INFO` & `construct-typing-0.6.0/construct_typing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-typing
-Version: 0.5.6
+Version: 0.6.0
 Summary: Extension for the python package 'construct' that adds typing features
 Home-page: https://github.com/timrid/construct-typing
 Author: Tim Riddermann
 License: MIT
 Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,annotation,type hint,typing,typed,bitstruct,PEP 561
 Platform: POSIX
 Platform: Windows
```

### Comparing `construct-typing-0.5.6/construct_typing.egg-info/SOURCES.txt` & `construct-typing-0.6.0/construct_typing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.6/setup.py` & `construct-typing-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     description="Extension for the python package 'construct' that adds typing features",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     platforms=["POSIX", "Windows"],
     url="https://github.com/timrid/construct-typing",
     author="Tim Riddermann",
     python_requires=">=3.7",
-    install_requires=["construct==2.10.68"],
+    install_requires=[
+        "construct==2.10.68",
+        "typing_extensions>=4.6.0"
+    ],
     keywords=[
         "construct",
         "kaitai",
         "declarative",
         "data structure",
         "struct",
         "binary",
```

