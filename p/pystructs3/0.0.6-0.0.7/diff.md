# Comparing `tmp/pystructs3-0.0.6.tar.gz` & `tmp/pystructs3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystructs3-0.0.6.tar", last modified: Wed Jun 28 01:34:31 2023, max compression
+gzip compressed data, was "pystructs3-0.0.7.tar", last modified: Mon Jul 24 17:11:56 2023, max compression
```

## Comparing `pystructs3-0.0.6.tar` & `pystructs3-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:34:31.883695 pystructs3-0.0.6/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.6/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-06-28 01:34:31.883695 pystructs3-0.0.6/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.6/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:34:31.879695 pystructs3-0.0.6/pystructs/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1522 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2445 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/bytestr.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3997 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/codec.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2359 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/helpers.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3715 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/integer.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3178 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/lists.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4900 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/net.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2523 2023-06-25 18:11:05.000000 pystructs3-0.0.6/pystructs/struct.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:34:31.879695 pystructs3-0.0.6/pystructs/tests/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      323 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/tests/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1538 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/tests/bytestr.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1432 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/tests/helpers.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2156 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/tests/integer.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1824 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/tests/lists.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2336 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/tests/net.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1471 2023-06-25 07:59:42.000000 pystructs3-0.0.6/pystructs/tests/struct.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:34:31.883695 pystructs3-0.0.6/pystructs3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-06-28 01:34:31.000000 pystructs3-0.0.6/pystructs3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      538 2023-06-28 01:34:31.000000 pystructs3-0.0.6/pystructs3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-28 01:34:31.000000 pystructs3-0.0.6/pystructs3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       28 2023-06-28 01:34:31.000000 pystructs3-0.0.6/pystructs3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-06-28 01:34:31.000000 pystructs3-0.0.6/pystructs3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-28 01:34:31.883695 pystructs3-0.0.6/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      761 2023-06-28 01:34:18.000000 pystructs3-0.0.6/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:56.953293 pystructs3-0.0.7/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.7/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2518 2023-07-24 17:11:56.949293 pystructs3-0.0.7/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2039 2023-07-02 21:59:23.000000 pystructs3-0.0.7/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:56.949293 pystructs3-0.0.7/pystructs/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2943 2023-07-02 21:54:24.000000 pystructs3-0.0.7/pystructs/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2445 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/bytestr.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4070 2023-07-02 21:24:02.000000 pystructs3-0.0.7/pystructs/codec.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2359 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/helpers.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3715 2023-06-30 05:54:23.000000 pystructs3-0.0.7/pystructs/integer.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3178 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/lists.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4900 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/net.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3350 2023-07-24 16:48:38.000000 pystructs3-0.0.7/pystructs/struct.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:56.949293 pystructs3-0.0.7/pystructs/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      323 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1538 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/tests/bytestr.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1432 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/tests/helpers.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2156 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/tests/integer.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1824 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/tests/lists.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2336 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/tests/net.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1471 2023-06-25 07:59:42.000000 pystructs3-0.0.7/pystructs/tests/struct.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:56.949293 pystructs3-0.0.7/pystructs3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2518 2023-07-24 17:11:56.000000 pystructs3-0.0.7/pystructs3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      538 2023-07-24 17:11:56.000000 pystructs3-0.0.7/pystructs3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-07-24 17:11:56.000000 pystructs3-0.0.7/pystructs3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       42 2023-07-24 17:11:56.000000 pystructs3-0.0.7/pystructs3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-07-24 17:11:56.000000 pystructs3-0.0.7/pystructs3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-07-24 17:11:56.953293 pystructs3-0.0.7/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      775 2023-07-24 16:49:40.000000 pystructs3-0.0.7/setup.py
```

### Comparing `pystructs3-0.0.6/LICENSE` & `pystructs3-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/__init__.py` & `pystructs3-0.0.7/pystructs/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Python Struct Utilities Library
 """
-from typing import Any
+from typing import Any, Sequence, Tuple, overload
 
 #** Variables **#
 __all__ = [
+    'pack',
+    'unpack',
     'encode',
     'decode',
 
     'field',
     'Field',
     'Struct',
 
@@ -53,35 +55,72 @@
 
     'Const',
     'Wrap',
 ]
 
 #** Functions **#
 
-def encode(ctx: 'Context', value: Any, codec: Any) -> bytes:
+def pack(codecs: Any, *values: Any) -> bytes:
     """
     Encode the following value into bytes
 
-    :param value: value to encode in bytes using codec
-    :param codec: codec used to encode value
-    :return:      encoded bytes
+    :param codecs: codecs used to encode value
+    :param values: value to encode in bytes using codec
+    :return:       encoded bytes
     """
-    codec = deanno(codec, Codec)
-    return codec.encode(ctx, value)
+    ctx = Context()
+    return encode(ctx, codecs, *values)
 
-def decode(ctx: 'Context', raw: bytes, codec: Any) -> Any:
+def unpack(codecs: Any, raw: bytes) -> Tuple[Any, ...]:
     """
-    Decode the following bytes with the specified Codec
+    Decode the following bytes with specified Codec
 
-    :param raw:   raw bytes to decode
-    :param codec: codec implementation used to decode value
-    :return:      decoded bytes
+    :param raw:    raw bytes to decode
+    :param codecs: codec implementations used to decode value
+    :return:       decoded bytes
     """
-    codec = deanno(codec, Codec)
-    return codec.decode(ctx, raw)
+    ctx = Context()
+    return decode(ctx, codecs, raw)
+
+def encode(ctx: 'Context', codecs: Sequence[Any], *values: Any) -> bytes:
+    """
+    Encode the following value into bytes w/ Context
+
+    :param ctx:    context object used to encode value
+    :param codecs: codecs used to encode value
+    :param values: values to encode in bytes using codec
+    :return:       encoded bytes
+    """
+    codecs = (codecs, ) if not isinstance(codecs, Sequence) else codecs
+    if len(values) < len(codecs):
+        raise ValueError(f'Too few values. {len(codecs)} Specified.')
+    if len(values) > len(codecs):
+        raise ValueError(f'Too many values. {len(codecs)} Specified.')
+    content = bytearray()
+    for value, codec in zip(values, codecs):
+        codec    = deanno(codec, Codec)
+        content += codec.encode(ctx, value)
+    return bytes(content)
+
+def decode(ctx: 'Context', codecs: Sequence[Any], raw: bytes) -> Tuple[Any, ...]:
+    """
+    Decode the following bytes with the specified Codec w/ Context
+
+    :param ctx:    context object used to decode value
+    :param codecs: codec implementations used to decode value
+    :param raw:    raw bytes to decode
+    :return:       decoded bytes
+    """
+    codecs  = (codecs, ) if not isinstance(codecs, Sequence) else codecs
+    content = []
+    for codec in codecs:
+        codec = deanno(codec, Codec)
+        value = codec.decode(ctx, raw)
+        content.append(value)
+    return tuple(content)
 
 #** Imports **#
 from .struct import *
 from .codec import *
 from .integer import *
 from .bytestr import *
 from .lists import *
```

### Comparing `pystructs3-0.0.6/pystructs/bytestr.py` & `pystructs3-0.0.7/pystructs/bytestr.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/codec.py` & `pystructs3-0.0.7/pystructs/codec.py`

 * *Files 9% similar despite different names*

```diff
@@ -96,15 +96,17 @@
     """Encoding/Decoding Context Tracking"""
     index: int = 0
     index_to_domain: Dict[int, bytes] = field(default_factory=dict)
     domain_to_index: Dict[bytes, int] = field(default_factory=dict)
 
     def reset(self):
         """reset variables in context to their default state"""
-        self.__init__()
+        self.index = 0
+        self.index_to_domain.clear()
+        self.domain_to_index.clear()
 
     def slice(self, raw: bytes, length: int) -> bytes:
         """
         parse slice of n-length starting from current context index
 
         :param raw:    raw bytes to slice from
         :param length: length of slice to retrieve
```

### Comparing `pystructs3-0.0.6/pystructs/helpers.py` & `pystructs3-0.0.7/pystructs/helpers.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/integer.py` & `pystructs3-0.0.7/pystructs/integer.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/lists.py` & `pystructs3-0.0.7/pystructs/lists.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/net.py` & `pystructs3-0.0.7/pystructs/net.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/struct.py` & `pystructs3-0.0.7/pystructs/struct.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 DataClass-Like Struct Implementation
 """
 from typing import Any, Type, Optional, ClassVar
-from typing_extensions import Self, dataclass_transform
+from typing_extensions import Self, dataclass_transform, get_type_hints
 
 from pyderive import MISSING, BaseField, dataclass, fields, gen_slots
 
 from .codec import *
 
 #** Variables **#
 __all__ = ['field', 'Field', 'Struct']
@@ -32,32 +32,57 @@
 
 #** Classes **#
 
 @dataclass(slots=True)
 class Field(BaseField):
     codec: Optional[Type[Codec]] = None
 
-    def finalize(self):
+    def __compile__(self, _):
         """compile codec/annotation"""
         self.anno = deanno(self.codec or self.anno, (Codec, Struct))
 
 @protocol(checkable=False)
 @dataclass_transform(field_specifiers=(Field, field))
 class Struct(Codec):
     base_type: ClassVar[tuple] = ()
  
     def __init__(self):
         raise NotImplementedError
 
     def __init_subclass__(cls, **kwargs):
         compile(cls, **kwargs) 
         cls.base_type = (cls, )
+    
+    def pack(self) -> bytes:
+        """
+        pack contents into serialized bytes
+
+        :return: serialized struct contents
+        """
+        ctx = Context()
+        return self.encode(ctx)
+    
+    @classmethod
+    def unpack(cls, raw: bytes) -> Self:
+        """
+        unpack serialized bytes into struct object
+
+        :param raw: raw bytes to unpack into struct
+        :return:    deserialized struct object
+        """
+        ctx = Context()
+        return cls.decode(ctx, raw)
 
     def encode(self, ctx: Context) -> bytes:
-        """encode the compiled sequence fields into bytes"""
+        """
+        encode the compiled sequence fields into bytes
+
+        :param ctx: context helper used to encode bytes
+        :return:    packed and serialized struct object
+        """
         encoded = bytearray()
         for f in fields(self):
             value = getattr(self, f.name, f.default or MISSING)
             if value is MISSING:
                 raise ValueError(f'{cname(self)} missing attr {f.name!r}')
             if not isinstance(value, f.anno.base_type):
                 raise ValueError(f'{cname(self)}.{f.name} invalid value: {value!r}')
@@ -65,15 +90,21 @@
                 encoded += f.anno.encode(ctx, value)
             except (CodecError, ValueError, TypeError) as e:
                 raise ValueError(f'{cname(self)}.{f.name}: {e}') from None
         return bytes(encoded)
 
     @protomethod
     def decode(cls, ctx: Context, raw: bytes) -> Self:
-        """decode the given raw-bytes into a compiled sequence"""
+        """
+        decode the given raw-bytes into a compiled sequence
+        
+        :param ctx: context helper used to decode bytes
+        :param raw: raw bytes content to decode
+        :return:    decoded struct object
+        """
         kwargs = {}
         for f in fields(cls):
             try:
                 value = f.anno.decode(ctx, raw)
             except (CodecError, ValueError, TypeError) as e:
                 raise ValueError(f'{cname(cls)}.{f.name}: {e}') from None
             if f.init:
```

### Comparing `pystructs3-0.0.6/pystructs/tests/bytestr.py` & `pystructs3-0.0.7/pystructs/tests/bytestr.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/tests/helpers.py` & `pystructs3-0.0.7/pystructs/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/tests/integer.py` & `pystructs3-0.0.7/pystructs/tests/integer.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/tests/lists.py` & `pystructs3-0.0.7/pystructs/tests/lists.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/tests/net.py` & `pystructs3-0.0.7/pystructs/tests/net.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs/tests/struct.py` & `pystructs3-0.0.7/pystructs/tests/struct.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/pystructs3.egg-info/SOURCES.txt` & `pystructs3-0.0.7/pystructs3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.6/setup.py` & `pystructs3-0.0.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pystructs3',
-    version='0.0.6',
+    version='0.0.7',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pystruct',
     description="Dataclass-Like Serialization Helpers for More Complex Data-Types",
     long_description=readme,
     long_description_content_type="text/markdown",
     python_requires='>=3.8',
     packages=find_packages(),
     install_requires=[
-        'pyderive3',
-        'typing_extensions'
+        'pyderive3>=0.0.6',
+        'typing_extensions>=4.7.1'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 )
```

