# Comparing `tmp/pyderive3-0.0.5.tar.gz` & `tmp/pyderive3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyderive3-0.0.5.tar", last modified: Wed Jun 28 01:33:05 2023, max compression
+gzip compressed data, was "pyderive3-0.0.6.tar", last modified: Mon Jul 24 17:11:08 2023, max compression
```

## Comparing `pyderive3-0.0.5.tar` & `pyderive3-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,36 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:33:05.309698 pyderive3-0.0.5/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2816 2023-06-28 01:33:05.309698 pyderive3-0.0.5/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2391 2023-05-28 09:26:37.000000 pyderive3-0.0.5/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:33:05.309698 pyderive3-0.0.5/pyderive/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1108 2023-06-25 18:08:28.000000 pyderive3-0.0.5/pyderive/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3212 2023-06-24 00:39:03.000000 pyderive3-0.0.5/pyderive/abc.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     8018 2023-06-28 01:31:36.000000 pyderive3-0.0.5/pyderive/compat.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    11414 2023-06-28 01:31:36.000000 pyderive3-0.0.5/pyderive/compile.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)    11400 2023-06-28 00:17:25.000000 pyderive3-0.0.5/pyderive/dataclasses.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6165 2023-06-26 05:42:29.000000 pyderive3-0.0.5/pyderive/parse.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:33:05.309698 pyderive3-0.0.5/pyderive/tests/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      119 2023-05-28 08:41:00.000000 pyderive3-0.0.5/pyderive/tests/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2642 2023-05-28 20:41:04.000000 pyderive3-0.0.5/pyderive/tests/dataclasses.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-28 01:33:05.309698 pyderive3-0.0.5/pyderive3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2816 2023-06-28 01:33:05.000000 pyderive3-0.0.5/pyderive3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      357 2023-06-28 01:33:05.000000 pyderive3-0.0.5/pyderive3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-28 01:33:05.000000 pyderive3-0.0.5/pyderive3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2023-06-28 01:33:05.000000 pyderive3-0.0.5/pyderive3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-06-28 01:33:05.000000 pyderive3-0.0.5/pyderive3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-28 01:33:05.309698 pyderive3-0.0.5/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      708 2023-06-28 01:32:21.000000 pyderive3-0.0.5/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:08.112448 pyderive3-0.0.6/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4081 2023-07-24 17:11:08.112448 pyderive3-0.0.6/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2473 2023-07-24 17:01:31.000000 pyderive3-0.0.6/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:08.112448 pyderive3-0.0.6/pyderive/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1202 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5245 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/abc.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     8018 2023-06-28 01:31:36.000000 pyderive3-0.0.6/pyderive/compat.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    12498 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/compile.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    14130 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/dataclasses.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:08.112448 pyderive3-0.0.6/pyderive/extensions/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      149 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/extensions/__init__.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:08.112448 pyderive3-0.0.6/pyderive/extensions/serde/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     9376 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/extensions/serde/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3111 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/extensions/serde/impl.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    16335 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/extensions/serde/serde.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     9555 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/extensions/serde/xml.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:08.112448 pyderive3-0.0.6/pyderive/extensions/validate/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4269 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/extensions/validate/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4611 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/extensions/validate/types.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    11920 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/extensions/validate/validators.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5863 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/parse.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:08.112448 pyderive3-0.0.6/pyderive/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      222 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3386 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/tests/dataclasses.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:08.112448 pyderive3-0.0.6/pyderive/tests/extensions/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      198 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/tests/extensions/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6221 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/tests/extensions/serde.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     8769 2023-07-24 17:01:31.000000 pyderive3-0.0.6/pyderive/tests/extensions/validate.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-24 17:11:08.112448 pyderive3-0.0.6/pyderive3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4081 2023-07-24 17:11:08.000000 pyderive3-0.0.6/pyderive3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      762 2023-07-24 17:11:08.000000 pyderive3-0.0.6/pyderive3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-07-24 17:11:08.000000 pyderive3-0.0.6/pyderive3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       25 2023-07-24 17:11:08.000000 pyderive3-0.0.6/pyderive3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-07-24 17:11:08.000000 pyderive3-0.0.6/pyderive3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-07-24 17:11:08.112448 pyderive3-0.0.6/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      715 2023-07-24 17:04:15.000000 pyderive3-0.0.6/setup.py
```

### Comparing `pyderive3-0.0.5/PKG-INFO` & `pyderive3-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-Metadata-Version: 2.1
-Name: pyderive3
-Version: 0.0.5
-Summary: Python3 Custom Data Class Helpers
-Home-page: https://github.com/imgurbot12/pyderive
-Author: Andrew Scott
-Author-email: imgurbot12@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 pyderive
 ---------
 
 Python3 Custom Dataclass Helpers
 
 ### Installation
 
 ```bash
 pip install pyderive3
 ```
 
 ### Features
 
+Additional Features availalbe via [Extensions](./pyderive/extensions/README.md).
+
 ##### Expanded Reimplementation of Dataclasses
 
 ###### Default Standards Implemented
 
 _'slots' kwarg now supported in older versions of python such as 3.8_
 
 ```python
```

### Comparing `pyderive3-0.0.5/pyderive/__init__.py` & `pyderive3-0.0.6/pyderive/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Custom DataClass Compilation Helpers
 """
-from typing import Type, Any
+from typing import Dict, Type, Any
 
 from .abc import *
 from .parse import *
 from .compile import *
 from .dataclasses import *
 from . import compat
 
@@ -36,23 +36,25 @@
     'gen_slots',
     'add_slots',
     'freeze_fields',
 
     'is_dataclass',
     'field',
     'fields',
+    'astuple',
     'asdict',
     'dataclass',
     'DataClassLike',
 
     'BaseField',
 ]
 
 #** Classes **#
 
-@dataclass(recurse=True)
-class BaseField(FieldDef):
+@dataclass(recurse=True, init=True)
+class BaseField(Field):
     """dataclass field instance w/ better defaults"""
     name:            str            = ''
     anno:            Type           = type
     default:         Any            = field(default_factory=lambda: MISSING)
-    default_factory: DefaultFactory = field(default_factory=lambda: MISSING) 
+    default_factory: DefaultFactory = field(default_factory=lambda: MISSING)
+    metadata:        Dict[str, Any] = field(default_factory=dict)
```

### Comparing `pyderive3-0.0.5/pyderive/compat.py` & `pyderive3-0.0.6/pyderive/compat.py`

 * *Files identical despite different names*

### Comparing `pyderive3-0.0.5/pyderive/compile.py` & `pyderive3-0.0.6/pyderive/compile.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     'create_hash',
     'assign_func',
     'gen_slots',
     'add_slots',
     'freeze_fields',
 ]
 
+#:TODO: add unit-test for validator added with default/default-factory/frozen
+
 #: post init function
 POST_INIT = '__post_init__'
 
 #: custom type to declare variable has a default factory
 HDF = type('HAS_DEFAULT_FACTORY', (), {})
 
 #: variable used to reference custom has-default-factory type
@@ -91,14 +93,29 @@
 
 def _init_assign(self_name: str, name: str, value: str, frozen: bool) -> str:
     """generate field variable assignment"""
     if frozen:
         return f'object.__setattr__({self_name}, {name!r}, {value})'
     return f'{self_name}.{name}={value}'
 
+def _init_validator(self_name: str, 
+    field: FieldDef, value: str, globals: dict) -> Tuple[List[str], str]:
+    """generate field validator function call"""
+    field_name = f'_field_{field.name}'
+    validator  = f'_validate_{field.name}'
+    globals[field_name] = field
+    globals[validator]  = field.validator
+    # generate validators/value code
+    validators = []
+    if field.default_factory is not MISSING:
+        validators.append(f'{field.name}={value}')
+        value = field.name
+    validators += [f'{value}={validator}({self_name}, {field_name}, {value})']
+    return validators, value
+
 def create_init(
     fields:    Fields,
     kw_only:   bool = False, 
     post_init: bool = False,
     frozen:    bool = False,
 ) -> Callable:
     """
@@ -108,42 +125,50 @@
     :param kw_only:   override kw-only to make everything kw-only 
     :param post_init: enable post-init when true
     :return:          generated init-function made from specifications
     """
     self_name = 'self'
     locals:  Dict[str, Any] = {}
     globals: Dict[str, Any] = {HDF_VAR: HDF}
-    args, post, body, kwonly = ['self'], [], [], []
+    args, post, body, validators, kwonly = ['self'], [], [], [], []
     for field in fields:
         # handle non-init edge cases
         name = field.name
-        if not field.init and field.default is MISSING \
-            and field.default_factory is MISSING:
+        if not field.init and not has_default(field): 
             # raise an error if field is an init-var
             if field.field_type == FieldType.INIT_VAR:
                 raise TypeError(f'field {name!r} must have init as InitVar')
             continue
         # build parameter code
         param = _init_param(field)
         value = _init_value(field, globals)
         if field.init:
             if kw_only or field.kw_only:
                 kwonly.append(param)
             else:
                 args.append(param)
+        # build validator function when enabled
+        if field.validator is not None:
+            if not callable(field.validator):
+                raise TypeError(f'field {name!r} validator is not callable')
+            validator, value = _init_validator(self_name, field, value, globals)
+            validators.extend(validator)
+        # track init-vars for later generation
         if field.field_type == FieldType.INIT_VAR:
             if field.default_factory is not MISSING:
                 raise TypeError(
                     f'init field {name!r} cannot have a default factory')
             post.append(name)
             continue
         # build body code
         assign = _init_assign(self_name, name, value, frozen or field.frozen)
         body.append(assign)
     # ensure body exists
+    if validators:
+        body = [*validators, *body]
     if post_init:
         params = ', '.join(post)
         body.append(f'self.{POST_INIT}({params})')
     if not body:
         body.append('pass')
     # generate function args/kwargs
     if kwonly:
```

### Comparing `pyderive3-0.0.5/pyderive/dataclasses.py` & `pyderive3-0.0.6/pyderive/dataclasses.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,37 +13,44 @@
 
 #** Variables **#
 __all__ = [
     'InitVar', 
     'MISSING', 
     'DataClassLike',
     'FrozenInstanceError',
- 
+    
+    'TupleFactory',
+    'DictFactory',
+
     'is_dataclass',
     'field', 
     'fields',
+    'astuple',
     'asdict',
     'dataclass'
 ]
 
+#: asdict/astuple custom encoder function
+EncoderFunc = Callable[[Any], Any] 
+
+#: optional asdict/astuple encoder function
+OptEncoderFunc = Optional[EncoderFunc]
+
+#: tuple factory
+TupleFactory = Union[Type[tuple], Callable[[Any, Any], Tuple]]
+
+#: dictionary factory
+DictFactory = Union[Type[dict], Callable[[Any, Any], Dict]]
+
 #: dataclass fields attribute
 FIELD_ATTR = '__datafields__'
 
 #: dataclas params attribute
 PARAMS_ATTR = '__dataparams__'
 
-#: field generic type
-F = TypeVar('F', bound=FieldDef)
-
-#: type for type-alias
-TypeT = Type[T]
-
-#: typehint for dataclass creator function
-DataFunc = Callable[[TypeT], TypeT] 
-
 _hash_add  = lambda _, fields: create_hash(fields)
 _hash_none = lambda *_: None
 def _hash_err(cls, _):
     raise TypeError(
         f'Cannot override attribute __hash__ in class {cls.__name__}')
 
 #: table of hash controls -> hash-action
@@ -103,51 +110,113 @@
     if not is_dataclass(cls):
         raise TypeError('fields() should with a dataclass type or instance')
     fields = getattr(cls, FIELD_ATTR)
     if not all_types:
         fields = [f for f in fields if f.field_type == FieldType.STANDARD]
     return fields
 
-def _asdict_inner(obj, rec: int, factory: Type[dict], lvl: int):
+def _astuple_inner(obj, rec: int, 
+    encoder: OptEncoderFunc, factory: TupleFactory, lvl: int) -> Any:
+    """inner tuple-ify function to convert dataclass fields to tuple"""
+    # stop recursin after limit
+    if rec > 0 and lvl >= rec:
+        return obj
+    # dataclass
+    lvl += 1
+    if is_dataclass(obj):
+        result = []
+        for f in fields(obj):
+            attr  = getattr(obj, f.name)
+            value = _astuple_inner(attr, rec, encoder, factory, lvl)
+            result.append(value)
+        if isinstance(factory, type):
+            return factory(result)
+        return factory(obj, result)
+    # named-tuple
+    elif isinstance(obj, tuple) and hasattr(obj, '_fields'):
+        return type(obj)(*[
+            _astuple_inner(v, rec, encoder, factory, lvl) for v in obj])
+    # standard list/tuple
+    elif isinstance(obj, (list, tuple)):
+        return type(obj)(
+            _astuple_inner(v, rec, encoder, factory, lvl) for v in obj)
+    elif isinstance(obj, dict):
+        return type(obj)((_astuple_inner(k, rec, encoder, factory, lvl),
+                          _astuple_inner(v, rec, encoder, factory, lvl))
+                         for k, v in obj.items())
+    else:
+        value = copy.deepcopy(obj)
+        return value if encoder is None else encoder(value)
+
+def astuple(cls, *, 
+    recurse:       int            = 0, 
+    encoder:       OptEncoderFunc = None, 
+    tuple_factory: TupleFactory   = tuple
+) -> tuple:
+    """
+    convert dataclass object into dictionary of field-values
+
+    :param cls:           dataclass object class instance
+    :param encoder:       python object encoder function
+    :param tuple_factory: factory used to generate tuple
+    :return:              field instances as dict
+    """
+    if not is_dataclass(cls):
+        raise TypeError('astuple() should be called on dataclass instances')
+    return _astuple_inner(cls, recurse, encoder, tuple_factory, 0)
+
+def _asdict_inner(obj, rec: int, 
+    encoder: OptEncoderFunc, factory: DictFactory, lvl: int) -> Any:
     """inner dictionary-ify function to convert dataclass fields into dict"""
     # stop recursin after limit
     if rec > 0 and lvl >= rec:
         return obj
     # dataclass
     lvl += 1
     if is_dataclass(obj):
         result = []
         for f in fields(obj):
             attr  = getattr(obj, f.name)
-            value = _asdict_inner(attr, rec, factory, lvl)
+            value = _asdict_inner(attr, rec, encoder, factory, lvl)
             result.append((f.name, value))
-        return factory(result)
+        if isinstance(factory, type):
+            return factory(result)
+        return factory(obj, result)
     # named-tuple
     elif isinstance(obj, tuple) and hasattr(obj, '_fields'):
-        return type(obj)(*[_asdict_inner(v, rec, factory, lvl) for v in obj])
+        return type(obj)(*[
+            _asdict_inner(v, rec, encoder, factory, lvl) for v in obj])
     # standard list/tuple
     elif isinstance(obj, (list, tuple)):
-        return type(obj)(_asdict_inner(v, rec, factory, lvl) for v in obj)
+        return type(obj)(
+            _asdict_inner(v, rec, encoder, factory, lvl) for v in obj)
     elif isinstance(obj, dict):
-        return type(obj)((_asdict_inner(k, rec, factory, lvl),
-                          _asdict_inner(v, rec, factory, lvl))
+        return type(obj)((_asdict_inner(k, rec, encoder, factory, lvl),
+                          _asdict_inner(v, rec, encoder, factory, lvl))
                          for k, v in obj.items())
     else:
-        return copy.deepcopy(obj) 
+        value = copy.deepcopy(obj)
+        return value if encoder is None else encoder(value)
 
-def asdict(cls, *, recurse: int = 0, dict_factory: Type[dict] = dict) -> dict:
+def asdict(cls, *, 
+    recurse:      int            = 0, 
+    encoder:      OptEncoderFunc = None, 
+    dict_factory: DictFactory    = dict
+) -> dict:
     """
     convert dataclass object into dictionary of field-values
 
-    :param cls: dataclass object class instance
-    :return:    field instances as dict
+    :param cls:          dataclass object class instance
+    :param encoder:      python object encoder function
+    :param dict_factory: factory used to generate tuple
+    :return:             field instances as dict
     """
     if not is_dataclass(cls):
         raise TypeError('asdict() should be called on dataclass instances')
-    return _asdict_inner(cls, recurse, dict_factory, 0) #type: ignore
+    return _asdict_inner(cls, recurse, encoder, dict_factory, 0)
 
 @dataclass_transform(field_specifiers=(FieldDef, Field, field))
 def _process_class(
     cls: TypeT,
     init:        Optional[bool] = None,
     repr:        Optional[bool] = None,
     eq:          bool = True,
@@ -165,16 +234,20 @@
         raise ValueError('eq must be true if order is true')
     # convert params for stdlib dataclasses
     isdataclass = is_dataclass(cls)
     if not isdataclass and is_stddataclass(cls):
         convert_params(cls)
     # parse and conregate fields
     struct = parse_fields(cls, factory=field, recurse=recurse)
-    fields = flatten_fields(struct)
+    fields = flatten_fields(struct, order_kw=not kw_only)
     freeze = frozen or any(f.frozen for f in fields)
+    # convert fields to kw-only if enabled
+    if kw_only:
+        for f in fields:
+            f.kw_only = True
     # validate settings and save fields/params
     params = DataParams(init, repr, eq, order, unsafe_hash, 
         frozen, match_args, kw_only, slots, recurse, field)
     if isdataclass:
         ofields = getattr(cls, FIELD_ATTR)
         oparams = getattr(cls, PARAMS_ATTR)
         # ensure there are no frozen conflicts
@@ -228,15 +301,15 @@
         match = tuple(f.name for f in fields if f.init)
         assign_func(cls, match, '__match_args__') #type: ignore
     # add slots
     if slots:
         cls = add_slots(cls, fields, freeze)
     # update abstraction-methods on re-creation and return
     if hasattr(abc, 'update_abstractmethods'):
-        abc.update_abstractmethods(cls)
+        abc.update_abstractmethods(cls) #type: ignore
     return cls
 
 @overload
 @dataclass_transform(field_specifiers=(FieldDef, Field, field))
 def dataclass(cls: Type[T], 
     init:        Optional[bool] = None,
     repr:        Optional[bool] = None,
```

### Comparing `pyderive3-0.0.5/pyderive/parse.py` & `pyderive3-0.0.6/pyderive/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,14 @@
     'parse_fields',
     'flatten_fields',
 ]
 
 #: raw field attribute name
 DERIVE_ATTR = '__derive__'
 
-#: track hashes of already compiled baseclasses
-COMPILED = set()
-
-COMPILED_ANNOTATIONS = set()
-
 #** Functions **#
 
 def remove_field(fields: ClassStruct, name: str):
     """
     remove field-name from fields heigharchy
     """
     current: Optional[ClassStruct] = fields
@@ -50,39 +45,36 @@
     :param base:    baseclass type to retrieve annotations/values from
     :param factory: field type factory used to produce fields
     :param recurse: enable recursive handling of field parsing if true
     :param delete:  delete values from class when found if true
     :param strict:  be strict on factory field type during parsing
     :return:        unprocessed dataclass field definitions
     """
-    global COMPILED, COMPILED_ANNOTATIONS
     bases  = list(cls.__mro__) if recurse else [cls]
     fields = None
     ftype: Type[FieldDef] = factory if strict else FieldDef
     while bases:
         # skip builtin bases
         base = bases.pop()
         if base is object:
             continue
-        # skip if recursive and already compiled
-        if recurse and hash(base) in COMPILED:
-            continue
-        COMPILED.add(hash(base))
         # convert stdlib dataclass fields to valid class-struct
         parent = getattr(base, DERIVE_ATTR, None)
         if parent is None and is_stddataclass(base):
             fields = convert_fields(base, ftype)
             names  = [f.name for f in fields]
             parent = ClassStruct(names, {f.name:f for f in fields})
         fields = ClassStruct(parent=parent)
+        # check if baseclass is already compiled
+        if fields.is_base_compiled(base):
+            continue
         # skip evaluations is annotations have already been checked
-        annotations = getattr(base, '__annotations__', {})
-        if id(annotations) in COMPILED_ANNOTATIONS:
+        annotations = getattr(base, '__annotations__', None) or dict()
+        if fields.is_anno_compiled(annotations):
             continue
-        COMPILED_ANNOTATIONS.add(id(annotations))
         # iterate annotations
         for name, anno in annotations.items():
             # handle ClassVar
             if get_origin(anno) is ClassVar:
                 remove_field(fields, name)
                 continue
             # retrieve default-value of variable (if exists)
@@ -107,31 +99,29 @@
             else:
                 field = factory(name, anno, default)
             # handle InitVar
             if not isinstance(anno, type) and isinstance(anno, InitVar):
                 field.anno = anno.type
                 field.field_type = FieldType.INIT_VAR 
             # finalize field build and assign to struct
-            field.finalize()
+            field.__compile__(cls)
             fields.fields[name] = field
         # apply fields to baseclass to allow for inheritance
+        fields.base        = base
+        fields.annotations = annotations
         if fields.fields:
             setattr(base, DERIVE_ATTR, fields)
     # ensure fields were parsed
     if fields is None:
         raise RuntimeError(f'DataClass Field-Parse Failed: {cls!r}')
     # ensure field-attr is set on top-level
     if not hasattr(cls, DERIVE_ATTR):
         setattr(cls, DERIVE_ATTR, fields)
     return fields
 
-def has_default(field: FieldDef) -> bool:
-    """return true if field has default"""
-    return field.default is not MISSING or field.default_factory is not MISSING
-
 def flatten_fields(
     fields: ClassStruct, order_kw: bool = True) -> Fields:
     """
     flatten field definitions using standard dataclass varaiable flattening
 
     :param fields:   list of higharchigal field definitions
     :param order_kw: ensure all fields w/o values appear before those that do
```

### Comparing `pyderive3-0.0.5/pyderive/tests/dataclasses.py` & `pyderive3-0.0.6/pyderive/tests/dataclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #** Variables **#
 __all__ = ['DataClassTests']
 
 #** Classes **#
 
 class DataClassTests(unittest.TestCase):
- 
+
     def test_initvar(self):
         """ensure InitVar works as intended"""
         @dataclass
         class T:
             a: int
             b: InitVar[int]
 
@@ -88,7 +88,32 @@
         @dataclass
         class Bar:
             foo: Foo
             b:   int       = 1
             c:   List[str] = field(default_factory=list)
         b = Bar(Foo(1), 2)
         self.assertDictEqual(asdict(b), {'foo': {'a': 1}, 'b': 2, 'c': []})
+
+    def test_astuple(self):
+        """ensure astuple function as intended"""
+        @dataclass
+        class Foo:
+            a: int = 0
+        @dataclass
+        class Bar:
+            foo: Foo
+            b:   int       = 1
+            c:   List[str] = field(default_factory=list)
+        bar = Bar(Foo(1), 2)
+        tup = astuple(bar)
+        self.assertIsInstance(tup, tuple)
+        self.assertListEqual(list(tup), [(1, ), 2, []])
+
+    def test_slots(self):
+        """ensure slots generation works as intended"""
+        @dataclass(slots=True)
+        class Foo:
+            a: int
+            b: int
+            c: InitVar[int]
+        self.assertTrue(hasattr(Foo, '__slots__'))
+        self.assertEqual(Foo.__slots__, ('a', 'b', ))
```

### Comparing `pyderive3-0.0.5/setup.py` & `pyderive3-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pyderive3',
-    version='0.0.5',
+    version='0.0.6',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pyderive',
     description="Python3 Custom Data Class Helpers",
     long_description=readme,
     long_description_content_type="text/markdown",
     python_requires='>=3.8',
     packages=find_packages(),
     install_requires=[
-        'typing_extensions'
+        'typing_extensions>=4.7.1'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
 )
```

