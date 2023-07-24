# Comparing `tmp/pytreeclass-0.4.0.tar.gz` & `tmp/pytreeclass-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.4.0.tar", last modified: Tue Jul 18 19:30:40 2023, max compression
+gzip compressed data, was "pytreeclass-0.5.0.tar", last modified: Mon Jul 24 19:33:09 2023, max compression
```

## Comparing `pytreeclass-0.4.0.tar` & `pytreeclass-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.721926 pytreeclass-0.4.0/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/code_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    32764 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    18528 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.721926 pytreeclass-0.4.0/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21260 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.491657 pytreeclass-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-24 19:33:09.491657 pytreeclass-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.487656 pytreeclass-0.5.0/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.487656 pytreeclass-0.5.0/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26041 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28977 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.487656 pytreeclass-0.5.0/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:33:09.491657 pytreeclass-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.487656 pytreeclass-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.4.0/LICENSE` & `pytreeclass-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.4.0/PKG-INFO` & `pytreeclass-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.4.0
+Version: 0.5.0
 Summary: Visualize, create, and operate on JAX PyTree in the most intuitive way possible.
 Author-email: Mahmoud Asem <mahmoudasem00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pytreeclass-0.4.0/README.md` & `pytreeclass-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 <td>
 
 ```python
 import jax
 import jax.numpy as jnp
 import pytreeclass as pytc
 
-
+@pytc.autoinit
 class Tree(pytc.TreeClass):
     a: float = 1.0
     b: tuple[float, float] = (2.0, 3.0)
     c: jax.Array = jnp.array([4.0, 5.0, 6.0])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
@@ -131,15 +131,16 @@
 <td>
 
 ```python
 import jax
 import pytreeclass as pytc
 
 class Counter(pytc.TreeClass):
-    calls : int = 0
+    def __init__(self, calls: int = 0):
+        self.calls = calls
 
     def increment(self):
         self.calls += 1
 counter = Counter() # Counter(calls=0)
 ```
 
 </td>
```

### Comparing `pytreeclass-0.4.0/pyproject.toml` & `pytreeclass-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.4.0/pytreeclass/__init__.py` & `pytreeclass-0.5.0/pytreeclass/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pytreeclass._src.code_build import field, fields
+from pytreeclass._src.code_build import autoinit, field, fields
 from pytreeclass._src.tree_base import TreeClass
 from pytreeclass._src.tree_index import AtIndexer, BaseKey
 from pytreeclass._src.tree_mask import (
     freeze,
     is_frozen,
     is_nondiff,
     tree_mask,
@@ -32,25 +32,27 @@
     tree_str,
     tree_summary,
 )
 from pytreeclass._src.tree_util import (
     Partial,
     bcmap,
     is_tree_equal,
+    leafwise,
     tree_flatten_with_trace,
     tree_leaves_with_trace,
     tree_map_with_trace,
 )
 
 __all__ = (
     # general utils
     "TreeClass",
     "is_tree_equal",
     "field",
     "fields",
+    "autoinit",
     # pprint utils
     "tree_diagram",
     "tree_graph",
     "tree_mermaid",
     "tree_repr",
     "tree_str",
     "tree_summary",
@@ -67,14 +69,15 @@
     # tree utils
     "bcmap",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
     "Partial",
+    "leafwise",
 )
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 AtIndexer.__module__ = "pytreeclass"
 TreeClass.__module__ = "pytreeclass"
 Partial.__module__ = "pytreeclass"
```

### Comparing `pytreeclass-0.4.0/pytreeclass/_src/__init__.py` & `pytreeclass-0.5.0/pytreeclass/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.4.0/pytreeclass/_src/code_build.py` & `pytreeclass-0.5.0/pytreeclass/_src/code_build.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,47 +17,92 @@
 from __future__ import annotations
 
 import functools as ft
 import sys
 from collections import defaultdict
 from collections.abc import Callable, MutableMapping, MutableSequence, MutableSet
 from types import FunctionType, MappingProxyType
-from typing import Any, Literal, NamedTuple, Sequence, TypeVar, get_args
+from typing import Any, Literal, Sequence, TypeVar, get_args
+
+from typing_extensions import dataclass_transform
 
 T = TypeVar("T")
 PyTree = Any
 EllipsisType = type(Ellipsis)
 ArgKindType = Literal["POS_ONLY", "POS_OR_KW", "VAR_POS", "KW_ONLY", "VAR_KW"]
 ArgKind = get_args(ArgKindType)
 NULL = type("NULL", (), {"__repr__": lambda _: "NULL"})()
 MUTABLE_TYPES = (MutableSequence, MutableMapping, MutableSet)
 # https://github.com/google/jax/issues/14295
 
 
-class Field(NamedTuple):
-    name: str | None = None
-    type: type | None = None
-    default: Any = NULL
-    init: bool = True
-    repr: bool = True
-    kind: ArgKindType = "POS_OR_KW"
-    metadata: dict[str, Any] | None = None
-    callbacks: Sequence[Callable[[Any], Any]] = ()
-    alias: str | None = None
+class Field:
+    __slots__ = [
+        "name",
+        "type",
+        "default",
+        "init",
+        "repr",
+        "kind",
+        "metadata",
+        "callbacks",
+        "alias",
+    ]
+
+    def __init__(
+        self,
+        name: str | None = None,
+        type: type | None = None,
+        default: Any = NULL,
+        init: bool = True,
+        repr: bool = True,
+        kind: ArgKind = "POS_OR_KW",
+        metadata: dict[str, Any] | None = None,
+        callbacks: Sequence[Callable[[Any], Any]] = (),
+        alias: str | None = None,
+    ):
+        self.name = name
+        self.type = type
+        self.default = default
+        self.init = init
+        self.repr = repr
+        self.kind = kind
+        self.metadata = metadata
+        self.callbacks = callbacks
+        self.alias = alias
 
     def __call__(self, value: Any):
         """Call the callbacks on `value`."""
         for callback in self.callbacks:
             try:
                 value = callback(value)
             except Exception as e:
                 cname = getattr(callback, "__name__", callback)
                 raise type(e)(f"On applying {cname} for field=`{self.name}`:\n{e}")
         return value
 
+    def __repr__(self):
+        """Generate a string representation of the Field instance."""
+        return f"Field({', '.join(f'{k}={getattr(self, k)}' for k in self.__slots__)})"
+
+    def replace(self, **kwargs) -> "Field":
+        """Return a new Field instance with the given fields replaced."""
+        return Field(**{k: kwargs.get(k, getattr(self, k)) for k in self.__slots__})
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+        return vars(instance)[self.name]
+
+    def __set_name__(self, owner, name):
+        self.name = name
+
+    def __set__(self, instance, value):
+        vars(instance)[self.name] = self(value)
+
 
 def field(
     *,
     default: Any = NULL,
     init: bool = True,
     repr: bool = True,
     kind: ArgKindType = "POS_OR_KW",
@@ -65,36 +110,40 @@
     callbacks: Sequence[Any] = (),
     alias: str | None = None,
 ) -> Field:
     """Field placeholder for type hinted attributes.
 
     Args:
         default: The default value of the field.
-        init: Whether the field is included in the object's __init__ function.
-        repr: Whether the field is included in the object's __repr__ function.
-        kind: Argument kind, one of 'POS_ONLY', 'VAR_POS', 'KW_ONLY', 'VAR_KW'.
+        init: Whether the field is included in the object's ``__init__`` function.
+        repr: Whether the field is included in the object's ``__repr__`` function.
+        kind: Argument kind, one of: ``POS_ONLY``, ``VAR_POS``, ``POS_OR_KW`` ,
+            ``KW_ONLY``, ``VAR_KW``
         metadata: A mapping of user-defined data for the field.
         callbacks: A sequence of functions to called on ``__setattr__`` during
             initialization to modify the field value.
         alias: An a alias for the field name in the constructor.
 
     Example:
         >>> import pytreeclass as pytc
-        >>> class IsInstance(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class IsInstance(pytc.TreeClass):
         ...    klass: type
         ...    def __call__(self, x):
         ...        assert isinstance(x, self.klass)
         ...        return x
-        >>> class Range(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class Range(pytc.TreeClass):
         ...    start: int|float = float("-inf")
         ...    stop: int|float = float("inf")
         ...    def __call__(self, x):
         ...        assert self.start <= x <= self.stop
         ...        return x
-        >>> class Employee(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class Employee(pytc.TreeClass):
         ...    # assert employee ``name`` is str
         ...    name: str = pytc.field(callbacks=[IsInstance(str)])
         ...    # use callback compostion to assert employee ``age`` is int and positive
         ...    age: int = pytc.field(callbacks=[IsInstance(int), Range(1)])
         ...    # use ``id`` in the constructor for ``_id`` attribute
         ...    # this is useful for private attributes that are not supposed
         ...    # to be accessed directly and hide it from the repr
@@ -151,15 +200,15 @@
             raise ValueError("Field name cannot be `self`.")
 
         if isinstance(value, Field):
             if isinstance(value.default, MUTABLE_TYPES):
                 # example case: `x: Any = field(default=[1, 2, 3])`
                 raise TypeError(f"Mutable {value.default=} is not allowed.")
             # case: `x: Any = field(default=1)`
-            field_map[name] = value._replace(name=name, type=hint)
+            field_map[name] = value.replace(name=name, type=hint)
         else:
             if isinstance(value, MUTABLE_TYPES):
                 # example case: `x: Any = [1, 2, 3]`
                 raise TypeError(f"Mutable {value=} is not allowed")
             # case: `x: int = 1` or `x: Any`
             field_map[name] = Field(name=name, type=hint, default=value)
     return MappingProxyType(field_map)
@@ -228,7 +277,29 @@
     code += f"\n\t\t{';'.join(body)}"
     code += f"\n\t__init__.__qualname__ = '{klass.__qualname__}.__init__'"
     code += "\n\treturn __init__"
 
     exec(code, vars(sys.modules[klass.__module__]), namespace := dict())
     setattr(init := namespace["closure"](field_map), "__annotations__", hints)
     return init
+
+
+@dataclass_transform(field_specifiers=(Field, field))
+def autoinit(klass: type[T]) -> type[T]:
+    """A class decorator that generates the ``__init__`` method from type hints.
+
+    Similar to ``dataclasses.dataclass``, this decorator generates the ``__init__``
+    method for the given class from the type hints or the :func:`field` objects
+    set to the class attributes.
+
+    Example:
+        >>> import pytreeclass as pytc
+        >>> @pytc.autoinit
+        ... class Tree:
+        ...     x: int
+        ...     y: int
+        >>> tree = Tree(1, 2)
+        >>> tree.x, tree.y
+        (1, 2)
+    """
+    klass.__init__ = _build_init_method(klass)
+    return klass
```

### Comparing `pytreeclass-0.4.0/pytreeclass/_src/tree_base.py` & `pytreeclass-0.5.0/pytreeclass/_src/tree_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,35 +18,28 @@
 
 import abc
 from contextlib import contextmanager
 from typing import Any, Hashable, TypeVar
 
 import jax
 import jax.tree_util as jtu
-from typing_extensions import Unpack, dataclass_transform
+from typing_extensions import Unpack
 
-from pytreeclass._src.code_build import (
-    Field,
-    _build_field_map,
-    _build_init_method,
-    field,
-    fields,
-)
+from pytreeclass._src.code_build import fields
 from pytreeclass._src.tree_index import AtIndexer
 from pytreeclass._src.tree_pprint import (
     PPSpec,
     attr_value_pp,
     pp_dispatcher,
     pps,
     tree_repr,
     tree_str,
 )
 from pytreeclass._src.tree_util import (
     NamedSequenceKey,
-    _leafwise_transform,
     is_tree_equal,
     tree_copy,
     tree_hash,
 )
 
 T = TypeVar("T", bound=Hashable)
 S = TypeVar("S")
@@ -65,56 +58,26 @@
 def _mutable_context(tree, *, kopy: bool = False):
     tree = tree_copy(tree) if kopy else tree
     _mutable_instance_registry.add(id(tree))
     yield tree
     _mutable_instance_registry.discard(id(tree))
 
 
-def _register_treeclass(klass: type[T]) -> type[T]:
-    # handle all registration logic for `treeclass`
-
-    def tree_unflatten(keys: tuple[str, ...], leaves: tuple[Any, ...]) -> T:
-        # unflatten rule to use with `jax.tree_unflatten`
-        tree = getattr(object, "__new__")(klass)
-        vars(tree).update(zip(keys, leaves))
-        return tree
-
-    def tree_flatten(tree: T) -> tuple[tuple[Any, ...], tuple[str, ...]]:
-        # flatten rule to use with `jax.tree_flatten`
-        dynamic = vars(tree)
-        return tuple(dynamic.values()), tuple(dynamic.keys())
-
-    def tree_flatten_with_keys(tree: T):
-        # flatten rule to use with `jax.tree_util.tree_flatten_with_path`
-        dynamic = dict(vars(tree))
-        for idx, key in enumerate(vars(tree)):
-            entry = NamedSequenceKey(idx, key)
-            dynamic[key] = (entry, dynamic[key])
-        return tuple(dynamic.values()), tuple(dynamic.keys())
-
-    jtu.register_pytree_with_keys(
-        nodetype=klass,
-        flatten_func=tree_flatten,
-        flatten_with_keys=tree_flatten_with_keys,
-        unflatten_func=tree_unflatten,
-    )
-    return klass
-
-
 class TreeClassIndexer(AtIndexer):
     def __call__(self, *a, **k) -> tuple[Any, PyTree]:
         """Call a method on the tree instance and return result and new instance.
 
         Returns:
             A tuple of the result of the function call and a copy of the a
              new instance of the tree with the modified values.
 
         Example:
             >>> import pytreeclass as pytc
-            >>> class Tree(pytc.TreeClass):
+            >>> @pytc.autoinit
+            ... class Tree(pytc.TreeClass):
             ...     a: int
             ...     def add(self, x:int) -> int:
             ...         self.a += x
             ...         return self.a
             >>> tree = Tree(a=1)
             >>> # call `add` and return a tuple of
             >>> # (return value, new instance)
@@ -136,118 +99,88 @@
         with _mutable_context(self.tree, kopy=True) as tree:
             value = recursive_getattr(tree, self.where)(*a, **k)  # type: ignore
         return value, tree
 
 
 class TreeClassMeta(abc.ABCMeta):
     def __call__(klass: type[T], *a, **k) -> T:
-        self = getattr(klass, "__new__")(klass, *a, **k)
-
-        with _mutable_context(self):
-            # initialize the instance under the mutable context
-            # to allow setting instance attributes without
-            # throwing an `AttributeError`
+        with _mutable_context(self := getattr(klass, "__new__")(klass, *a, **k)):
             getattr(klass, "__init__")(self, *a, **k)
-
-        if keys := set(_build_field_map(klass)) - set(vars(self)):
-            raise AttributeError(f"Found uninitialized fields {keys}.")
         return self
 
 
-@dataclass_transform(field_specifiers=(Field, field))
 class TreeClass(metaclass=TreeClassMeta):
     """Convert a class to a JAX compatible tree structure.
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
-
         >>> # Tree leaves are instance attributes
-        >>> class Tree(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> jax.tree_util.tree_leaves(tree)
         [1, 2.0]
 
         >>> # Leaf-wise math operations are supported by setting `leafwise=True`
-        >>> class Tree(pytc.TreeClass, leafwise=True):
+        >>> @pytc.leafwise
+        ... @pytc.autoinit
+        ... class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> tree + 1
         Tree(a=2, b=3.0)
 
         >>> # Advanced indexing is supported using `at` property
-        >>> class Tree(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> tree.at["a"].get()
         Tree(a=1, b=None)
         >>> tree.at[0].get()
         Tree(a=1, b=None)
-
-    Note:
-        ``leafwise=True`` adds the following methods to the class
-
-        ==================      ============
-        Method                  Operator
-        ==================      ============
-        ``__add__``              ``+``
-        ``__and__``              ``&``
-        ``__ceil__``             ``math.ceil``
-        ``__divmod__``           ``divmod``
-        ``__eq__``               ``==``
-        ``__floor__``            ``math.floor``
-        ``__floordiv__``         ``//``
-        ``__ge__``               ``>=``
-        ``__gt__``               ``>``
-        ``__invert__``           ``~``
-        ``__le__``               ``<=``
-        ``__lshift__``           ``<<``
-        ``__lt__``               ``<``
-        ``__matmul__``           ``@``
-        ``__mod__``              ``%``
-        ``__mul__``              ``*``
-        ``__ne__``               ``!=``
-        ``__neg__``              ``-``
-        ``__or__``               ``|``
-        ``__pos__``              ``+``
-        ``__pow__``              ``**``
-        ``__round__``            ``round``
-        ``__sub__``              ``-``
-        ``__truediv__``          ``/``
-        ``__trunc__``            ``math.trunc``
-        ``__xor__``              ``^``
-        ==================      ============
-
     """
 
-    def __init_subclass__(klass: type[T], *a, leafwise: bool = False, **k) -> None:
-        if "__setattr__" in vars(klass) or "__delattr__" in vars(klass):
-            raise TypeError(
-                f"Unable to transform the class `{klass.__name__}` "
-                "with resereved methods: `__setattr__` or `__delattr__` "
-                "defined.\nReserved `setters` and `deleters` implements "
-                "the immutable functionality and cannot be overriden."
-            )
-
-        super().__init_subclass__(*a, **k)
-
-        if "__init__" not in vars(klass):
-            # generate the init method if not defined similar to `dataclass`
-            setattr(klass, "__init__", _build_init_method(klass))
-
-        if leafwise:
-            # transform the class to support leafwise operations
-            # useful to use with `bcmap` and creating masks by comparisons.
-            klass = _leafwise_transform(klass)
-
-        klass = _register_treeclass(klass)
+    def __init_subclass__(klass: type[T]):
+        if "__setattr__" in vars(klass):
+            raise TypeError(f"Reserved methods: `__setattr__` defined in `{klass}`.")
+        if "__delattr__" in vars(klass):
+            raise TypeError(f"Reserved methods: `__delattr__` defined in `{klass}`.")
+
+        super().__init_subclass__()
+
+        def tree_unflatten(keys: tuple[str, ...], leaves: tuple[Any, ...]) -> T:
+            # unflatten rule to use with `jax.tree_unflatten`
+            vars(tree := getattr(object, "__new__")(klass)).update(zip(keys, leaves))
+            return tree
+
+        def tree_flatten(tree: T) -> tuple[tuple[Any, ...], tuple[str, ...]]:
+            # flatten rule to use with `jax.tree_flatten`
+            dynamic = vars(tree)
+            return tuple(dynamic.values()), tuple(dynamic.keys())
+
+        def tree_flatten_with_keys(tree: T):
+            # flatten rule to use with `jax.tree_util.tree_flatten_with_path`
+            dynamic = dict(vars(tree))
+            for idx, key in enumerate(vars(tree)):
+                entry = NamedSequenceKey(idx, key)
+                dynamic[key] = (entry, dynamic[key])
+            return tuple(dynamic.values()), tuple(dynamic.keys())
+
+        jtu.register_pytree_with_keys(
+            nodetype=klass,
+            flatten_func=tree_flatten,
+            flatten_with_keys=tree_flatten_with_keys,
+            unflatten_func=tree_unflatten,
+        )
 
     def __setattr__(self, key: str, value: Any) -> None:
         if id(self) not in _mutable_instance_registry:
             # instance is not under a mutable context
             # mutable context is used for setting instance attributes
             # during initialization and when using the `at` property
             # with call method.
@@ -258,29 +191,24 @@
                 "to set the value immutably.\nExample:\n"
                 f">>> tree1 = {type(self).__name__}(...)\n"
                 f">>> tree2 = tree1.at['{key}'].set({value!r})\n"
                 ">>> assert not tree1 is tree2\n"
                 f">>> tree2.{key}\n{value}"
             )
 
-        if key in (field_map := _build_field_map(type(self))):
-            # apply field callbacks on the value before setting
-            value = field_map[key](value)
-
         getattr(object, "__setattr__")(self, key, value)
 
     def __delattr__(self, key: str) -> None:
         if id(self) not in _mutable_instance_registry:
             # instance is not under a mutable context
             raise AttributeError(
                 f"Cannot delete attribute `{key}` "
                 f"on immutable instance of `{type(self).__name__}`.\n"
                 f"Use `.at['{key}'].set(None)` instead."
             )
-
         getattr(object, "__delattr__")(self, key)
 
     @property
     def at(self) -> TreeClassIndexer:
         """Immutable out-of-place indexing.
 
         - ``.at[***].get()``:
@@ -299,15 +227,16 @@
             - a boolean mask of the same structure as the tree
             - ``re.Pattern`` to index all keys matching a regex pattern.
             - an instance of ``BaseKey`` with custom logic to index a pytree.
             - a tuple of the above types to index multiple keys at same level.
 
         Example:
             >>> import pytreeclass as pytc
-            >>> class Tree(pytc.TreeClass):
+            >>> @pytc.autoinit
+            ... class Tree(pytc.TreeClass):
             ...     a:int = 1
             ...     b:float = 2.0
             ...     def add(self, x:int) -> int:
             ...         self.a += x
             ...         return self.a
             >>> tree = Tree()
             >>> # get `a` and return a new instance
```

### Comparing `pytreeclass-0.4.0/pytreeclass/_src/tree_index.py` & `pytreeclass-0.5.0/pytreeclass/_src/tree_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,16 @@
             >>> # instead of using ``FuncKey(function)`` we can define an alias
             >>> # for `FuncKey`, for this example we will define any FunctionType
             >>> # as a `FuncKey` by default.
             >>> @pytc.BaseKey.def_alias(FunctionType)
             ... def _(func):
             ...    return FuncKey(func)
             >>> # create a simple pytree
-            >>> class Tree(pytc.TreeClass):
+            >>> @pytc.autoinit
+            ... class Tree(pytc.TreeClass):
             ...    a: int
             ...    b: str
             >>> tree = Tree(1, "string")
             >>> # now we can use the `FuncKey` alias to match all leaves that
             >>> # are strings and start with "a"
             >>> tree.at[lambda x: isinstance(x, str) and x.startswith("a")].get()
             Tree(a=1, b=None)
@@ -185,15 +186,15 @@
         return self.name == other
 
     @__eq__.register(jtu.GetAttrKey)
     def _(self, other: jtu.GetAttrKey) -> bool:
         return self.name == other.name
 
     @__eq__.register(jtu.DictKey)
-    def _(self, other: jtu.__doc__) -> bool:
+    def _(self, other: jtu.DictKey) -> bool:
         return self.name == other.key
 
 
 class EllipsisKey(BaseKey):
     def __init__(self, _):
         del _
 
@@ -216,15 +217,16 @@
 
     Args:
         pattern: regex pattern to match.
 
     Example:
         >>> import pytreeclass as pytc
         >>> import re
-        >>> class Tree(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class Tree(pytc.TreeClass):
         ...     weight_1: float = 1.0
         ...     weight_2: float = 2.0
         ...     weight_3: float = 3.0
         ...     bias: float = 0.0
         >>> tree = Tree()
         >>> tree.at[re.compile(r"weight_.*")].set(100.0)  # set all weights to 100.0
         Tree(weight_1=100.0, weight_2=100.0, weight_3=100.0, bias=0.0)
@@ -461,15 +463,16 @@
             >>> tree = {"level1_0": {"level2_0": 100, "level2_1": 200}, "level1_1": 300}
             >>> tree = pytc.AtIndexer(tree)
             >>> tree.at["level1_0"].at["level2_0"].get()
             {'level1_0': {'level2_0': 100, 'level2_1': None}, 'level1_1': None}
 
         Example:
             >>> import pytreeclass as pytc
-            >>> class Tree(pytc.TreeClass):
+            >>> @pytc.autoinit
+            ... class Tree(pytc.TreeClass):
             ...     a: int
             ...     b: int
             >>> tree = Tree(a=1, b=2)
             >>> # get ``a`` and return a new instance
             >>> # with ``None`` for all other leaves
             >>> tree.at['a'].get()
             Tree(a=1, b=None)
@@ -499,15 +502,16 @@
             >>> tree = {"level1_0": {"level2_0": 100, "level2_1": 200}, "level1_1": 300}
             >>> tree = pytc.AtIndexer(tree)
             >>> tree.at["level1_0"].at["level2_0"].set('SET')
             {'level1_0': {'level2_0': 'SET', 'level2_1': 200}, 'level1_1': 300}
 
         Example:
             >>> import pytreeclass as pytc
-            >>> class Tree(pytc.TreeClass):
+            >>> @pytc.autoinit
+            ... class Tree(pytc.TreeClass):
             ...     a: int
             ...     b: int
             >>> tree = Tree(a=1, b=2)
             >>> # set ``a`` and return a new instance
             >>> # with all other leaves unchanged
             >>> tree.at['a'].set(100)
             Tree(a=100, b=2)
@@ -548,15 +552,16 @@
             >>> tree = {"level1_0": {"level2_0": 100, "level2_1": 200}, "level1_1": 300}
             >>> tree = pytc.AtIndexer(tree)
             >>> tree.at["level1_0"].at["level2_0"].apply(lambda _: 'SET')
             {'level1_0': {'level2_0': 'SET', 'level2_1': 200}, 'level1_1': 300}
 
         Example:
             >>> import pytreeclass as pytc
-            >>> class Tree(pytc.TreeClass):
+            >>> @pytc.autoinit
+            ... class Tree(pytc.TreeClass):
             ...     a: int
             ...     b: int
             >>> tree = Tree(a=1, b=2)
             >>> # apply to ``a`` and return a new instance
             >>> # with all other leaves unchanged
             >>> tree.at['a'].apply(lambda _: 100)
             Tree(a=100, b=2)
@@ -604,15 +609,16 @@
             ({'level1_0': {'level2_0': 'SET', 'level2_1': 200}, 'level1_1': 300}, 1)
 
         Example:
             >>> import pytreeclass as pytc
             >>> from typing import NamedTuple
             >>> class State(NamedTuple):
             ...     func_evals: int = 0
-            >>> class Tree(pytc.TreeClass):
+            >>> @pytc.autoinit
+            ... class Tree(pytc.TreeClass):
             ...     a: int
             ...     b: int
             ...     c: int
             >>> tree = Tree(a=1, b=2, c=3)
             >>> def scan_func(leaf, state: State):
             ...     state = State(state.func_evals + 1)
             ...     return leaf + 1, state
@@ -668,15 +674,16 @@
             - ``reduce`` applies a binary ``func`` to each leaf values while accumulating
               a state a returns the final result. while ``scan`` applies ``func`` to each
               leaf value while carrying a state and returns the final state and
               the leaves of the tree with the result of applying ``func`` to each leaf.
 
         Example:
             >>> import pytreeclass as pytc
-            >>> class Tree(pytc.TreeClass):
+            >>> @pytc.autoinit
+            ... class Tree(pytc.TreeClass):
             ...     a: int
             ...     b: int
             >>> tree = Tree(a=1, b=2)
             >>> tree.at[...].reduce(lambda a, b: a + b, initializer=0)
             3
         """
         where = _resolve_where(self.tree, self.where, is_leaf)
```

### Comparing `pytreeclass-0.4.0/pytreeclass/_src/tree_mask.py` & `pytreeclass-0.5.0/pytreeclass/_src/tree_mask.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.4.0/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.5.0/pytreeclass/_src/tree_pprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import inspect
 import math
-from itertools import chain
+from contextlib import suppress
+from itertools import zip_longest
 from types import FunctionType
-from typing import Any, Callable, Iterable, Literal
+from typing import Any, Callable, Iterable, Literal, Sequence
 
 import jax
 import jax.tree_util as jtu
 import numpy as np
 from jax import custom_jvp
 from jax.util import unzip2
-from typing_extensions import TypedDict, Unpack
+from typing_extensions import TypeAlias, TypedDict, Unpack
 
 from pytreeclass._src.tree_util import (
     IsLeafType,
     Node,
     construct_tree,
     tree_leaves_with_trace,
     tree_map_with_trace,
@@ -47,15 +48,14 @@
     depth: int | float
     seen: set[int]
 
 
 PyTree = Any
 
 PP = Callable[[Any, Unpack[PPSpec]], str]
-from_iterable = chain.from_iterable
 
 
 @ft.singledispatch
 def pp_dispatcher(node: Any, **spec: Unpack[PPSpec]) -> str:
     """Register a new or override an existing pretty printer by type using."""
     return general_pp(node, **spec)
 
@@ -145,25 +145,32 @@
     if not issubclass(node.dtype.type, (np.integer, np.floating)) or node.size == 0:
         return base
 
     # Extended repr for numpy array, with extended information
     # this part of the function is inspired by
     # lovely-jax https://github.com/xl0/lovely-jax
 
-    # handle interval
-    low, high = np.min(node), np.max(node)
-    interval = "(" if math.isinf(low) else "["
-    is_integer = issubclass(node.dtype.type, np.integer)
-    interval += f"{low},{high}" if is_integer else f"{low:.2f},{high:.2f}"
-    interval += ")" if math.isinf(high) else "]"  # resolve closed/open interval
-    interval = interval.replace("inf", "∞")  # replace inf with infinity symbol
-    # handle mean and std
-    mean, std = f"{np.mean(node):.2f}", f"{np.std(node):.2f}"
+    with suppress(Exception):
+        # maybe the array is a jax tracers
+        low, high = np.min(node), np.max(node)
+
+        interval = (
+            ("(" if math.isinf(low) else "[")
+            + (
+                f"{low},{high}"
+                if issubclass(node.dtype.type, np.integer)
+                else f"{low:.2f},{high:.2f}"
+            )
+            + (")" if math.isinf(high) else "]")
+        ).replace("inf", "∞")
+
+        mean, std = f"{np.mean(node):.2f}", f"{np.std(node):.2f}"
+        return f"{base}(μ={mean}, σ={std}, ∈{interval})"
 
-    return f"{base}(μ={mean}, σ={std}, ∈{interval})"
+    return base
 
 
 @pp_dispatcher.register(FunctionType)
 @pp_dispatcher.register(custom_jvp)
 def func_pp(func: Callable, **spec: Unpack[PPSpec]) -> str:
     # Pretty print function
     # Example:
@@ -307,20 +314,22 @@
         tree: arbitrary pytree.
         depth: depth of the tree to print. default is max depth.
         is_leaf: function to determine if a node is a leaf. default is None.
         tabwidth: tab width of the repr string. default is 4.
 
     Example:
         >>> import pytreeclass as pytc
-        >>> class A(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class A(pytc.TreeClass):
         ...        x: int = 10
         ...        y: int = (20,30)
         ...        z: int = 40
 
-        >>> class B(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class B(pytc.TreeClass):
         ...     a: int = 10
         ...     b: tuple = (20,30, A())
 
         >>> print(pytc.tree_diagram(B(), depth=0))
         B(...)
 
         >>> print(pytc.tree_diagram(B(), depth=1))
@@ -396,21 +405,20 @@
         is_leaf: function to determine if a node is a leaf. default is None
         tabwidth: tab width of the repr string. default is 4.
 
     Note:
         - Copy the output and paste it in the mermaid live editor to interact with
           the diagram. https://mermaid.live
     """
-    ppspec = dict(indent=0, kind="REPR", width=80, depth=0, seen=set())
 
     def step(node: Node, depth: int = 0) -> str:
         if len(node.children) == 0:
             (key, _), value = node.data
             ppstr = f"{key}=" if key is not None else ""
-            ppstr += pp(value, **ppspec)
+            ppstr += tree_repr(value, depth=0)
             ppstr = "<b>" + ppstr + "</b>"
             return f'\tid{id(node.parent)} --- id{id(node)}("{ppstr}")\n'
 
         (key, type), _ = node.data
         ppstr = f"{key}:" if key is not None else ""
         ppstr += f"{type.__name__}"
         ppstr = "<b>" + ppstr + "</b>"
@@ -494,25 +502,24 @@
                 4685309312 -> 4685309568;
                 4685309632 [label="[2]:dict", shape=box];
                 4685309312 -> 4685309632;
                 4685309696 [label="['a']=3", shape=box];
                 4685309632 -> 4685309696;
             }
     """
-    ppspec = dict(indent=0, kind="REPR", width=80, depth=0, seen=set())
 
     def step(node: Node, depth: int = 0) -> str:
         (key, type), value = node.data
 
         # dispatch node style
         style = ", ".join(f"{k}={v}" for k, v in dot_dispatcher(value).items())
 
         if len(node.children) == 0:
             ppstr = f"{key}=" if key is not None else ""
-            ppstr += pp(value, **ppspec)
+            ppstr += tree_repr(value, depth=0)
             text = f'\t{id(node)} [label="{ppstr}", {style}];\n'
             text += f"\t{id(node.parent)} -> {id(node)};\n"
             return text
 
         ppstr = f"{key}:" if key is not None else ""
         ppstr += f"{type.__name__}"
 
@@ -544,175 +551,38 @@
     if children_length > width:
         return string
     return string.replace("\n", "").replace("\t", "")
 
 
 # table printing
 
+Row: TypeAlias = Sequence[str]  # list of columns
 
-def _hbox(*text) -> str:
-    # Create horizontally stacked text boxes
-    # Examples:
-    #     >>> _hbox("a","b")
-    #     ┌─┬─┐
-    #     │a│b│
-    #     └─┴─┘
-
-    boxes = list(map(_vbox, text))
-    boxes = [(box).split("\n") for box in boxes]
-    max_col_height = max([len(b) for b in boxes])
-    boxes = [b + [" " * len(b[0])] * (max_col_height - len(b)) for b in boxes]
-    return "\n".join([_resolve_line(line) for line in zip(*boxes)])
-
-
-def _vbox(*text) -> str:
-    # Create vertically stacked text boxes
-    # Example:
-    #     >>> _vbox("a","b")
-    #     ┌───┐
-    #     │a  │
-    #     ├───┤
-    #     │b  │
-    #     └───┘
-
-    #     >>> _vbox("a","","a")
-    #     ┌───┐
-    #     │a  │
-    #     ├───┤
-    #     │   │
-    #     ├───┤
-    #     │a  │
-    #     └───┘
-
-    max_width = (
-        max(from_iterable([[len(t) for t in item.split("\n")] for item in text])) + 0
-    )
-
-    top = f"┌{'─'*max_width}┐"
-    line = f"├{'─'*max_width}┤"
-    side = [
-        "\n".join([f"│{t}{' '*(max_width-len(t))}│" for t in item.split("\n")])
-        for item in text
-    ]
-
-    btm = f"└{'─'*max_width}┘"
-
-    text = ""
-
-    for i, s in enumerate(side):
-        if i == 0:
-            text += f"{top}\n{s}\n{line if len(side)>1 else btm}"
-
-        elif i == len(side) - 1:
-            text += f"\n{s}\n{btm}"
-
-        else:
-            text += f"\n{s}\n{line}"
-
-    return text
-
-
-def _hstack(*boxes):
-    # Create horizontally stacked text boxes
-    # Example:
-    #     >>> print(_hstack(_hbox("a"),_vbox("b","c")))
-    #     ┌─┬─┐
-    #     │a│b│
-    #     └─┼─┤
-    #       │c│
-    #       └─┘
-
-    boxes = [(box).split("\n") for box in boxes]
-    max_col_height = max([len(b) for b in boxes])
-    # expand height of each col before merging
-    boxes = [b + [" " * len(b[0])] * (max_col_height - len(b)) for b in boxes]
-    text = ""
-
-    _cells = tuple(zip(*boxes))
-
-    for i, line in enumerate(_cells):
-        text += _resolve_line(line) + ("\n" if i != (len(_cells) - 1) else "")
-
-    return text
-
-
-def _resolve_line(cols: list[str]) -> str:
-    # Combine columns of single line by merging their borders
-
-    # Args:
-    #     cols (Sequence[str,...]): Sequence of single line column string
-
-    # Returns:
-    #     str: resolved column string
-
-    # Example:
-    #     >>> _resolve_line(['ab','b│','│c'])
-    #     'abb│c'
-
-    #     >>> _resolve_line(['ab','b┐','┌c'])
-    #     'abb┬c'
-
-    cols = list(map(list, cols))  # convert each col to col of chars
-    alpha = ["│", "┌", "┐", "└", "┘", "┤", "├"]
-
-    for index in range(len(cols) - 1):
-        if cols[index][-1] == "┐" and cols[index + 1][0] in ["┌", "─"]:
-            cols[index][-1] = "┬"
-            cols[index + 1].pop(0)
-
-        elif cols[index][-1] == "┘" and cols[index + 1][0] in ["└", "─"]:
-            cols[index][-1] = "┴"
-            cols[index + 1].pop(0)
-
-        elif cols[index][-1] == "┤" and cols[index + 1][0] in ["├", "─", "└"]:  #
-            cols[index][-1] = "┼"
-            cols[index + 1].pop(0)
-
-        elif cols[index][-1] in ["┘", "┐", "─"] and cols[index + 1][0] in ["├"]:
-            cols[index][-1] = "┼"
-            cols[index + 1].pop(0)
 
-        elif cols[index][-1] == " ":
-            cols[index].pop()
+def _table(rows: list[Row]) -> str:
+    """Generate a table from a list of rows."""
 
-        elif cols[index][-1] in alpha and cols[index + 1][0] in [*alpha, " "]:
-            cols[index + 1].pop(0)
-
-    return "".join(map(lambda x: "".join(x), cols))
-
-
-def _table(rows: list[list[str]], transpose: bool = False) -> str:
-    # Create a table with self aligning rows and cols
-
-    # Args:
-    #     rows: list of lists of row values
-    #     transpose: transpose the table. i.e. rows become cols and cols become rows
-
-    # Returns:
-    #     str: box string
+    def line(text: Row, widths: list[int]) -> str:
+        return "\n".join(
+            "│"
+            + "│".join(col.ljust(width) for col, width in zip(line_row, widths))
+            + "│"
+            for line_row in zip_longest(*[t.split("\n") for t in text], fillvalue="")
+        )
 
-    # Example:
-    #     >>> col1 = ['1\n','2']
-    #     >>> col2 = ['3','4000']
-    #     >>> print(_table([col1,col2]))
-    #     ┌─┬────────┐
-    #     │1│3       │
-    #     │ │        │
-    #     ├─┼────────┤
-    #     │2│40000000│
-    #     └─┴────────┘
-
-    cols = rows if transpose else [list(c) for c in zip(*rows)]
-
-    for i, _cells in enumerate(zip(*cols)):
-        max_cell_height = max(map(lambda x: x.count("\n"), _cells))
-        for j in range(len(_cells)):
-            cols[j][i] += "\n" * (max_cell_height - cols[j][i].count("\n"))
+    widths = [max(map(len, "\n".join(col).split("\n"))) for col in zip(*rows)]
+    spaces: Row = ["─" * width for width in widths]
 
-    return _hstack(*(_vbox(*col) for col in cols))
+    return (
+        ("┌" + "┬".join(spaces) + "┐")
+        + "\n"
+        + ("\n├" + "┼".join(spaces) + "┤\n").join(line(row, widths) for row in rows)
+        + "\n"
+        + ("└" + "┴".join(spaces) + "┘")
+    )
 
 
 def size_pp(size: int, **spec: Unpack[PPSpec]):
     del spec
     order_alpha = ["B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"]
     size_order = int(math.log(size, 1024)) if size else 0
     text = f"{(size)/(1024**size_order):.2f}{order_alpha[size_order]}"
@@ -901,15 +771,16 @@
     Args:
         tree: pytree to summarize.
         is_leaf: function to determine if a node is a leaf. defaults to None.
         transpose: transpose the table. i.e. rows become cols and cols become rows.
 
     Example:
         >>> import pytreeclass as pytc
-        >>> class Test(pytc.TreeClass):
+        >>> @pytc.autoinit
+        ... class Test(pytc.TreeClass):
         ...    a:int = 1
         ...    b:float = 2.0
 
         >>> tree = Test()
         >>> print(pytc.tree_repr_with_trace(Test()))  # doctest: +NORMALIZE_WHITESPACE
         Test(
           a=
@@ -960,10 +831,11 @@
 
         types = "->".join(i.__name__ for i in trace[1])
         rows += [["Type path", types]]
 
         joiner = "\n" + "\t" * (len(trace[0]) + 1)
 
         # make a pretty table for each leaf
-        return joiner + (joiner).join(_table(rows, transpose=transpose).split("\n"))
+        rows = list(map(list, zip(*rows))) if transpose else rows
+        return joiner + (joiner).join(_table(rows).split("\n"))
 
     return tree_map_with_trace(leaf_trace_summary, tree, is_leaf=is_leaf)
```

### Comparing `pytreeclass-0.4.0/pytreeclass/_src/tree_util.py` & `pytreeclass-0.5.0/pytreeclass/_src/tree_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,21 +72,21 @@
             except Exception:
                 return verdict  # fail under `jit`
         return False
     return leaf == rhs
 
 
 def is_tree_equal(*trees: Any) -> bool | jax.Array:
-    """Return `True` if all pytrees are equal.
+    """Return ``True`` if all pytrees are equal.
 
     Note:
         trees are compared using their leaves and treedefs.
 
     Note:
-        Under `jit` the return type is boolean `jax.Array` instead of `bool`.
+        Under ``jit`` the return type is boolean `jax.Array` instead of ``bool``.
     """
     tree0, *rest = trees
     leaves0, treedef0 = jtu.tree_flatten(tree0)
     verdict = True
 
     for tree in rest:
         leaves, treedef = jtu.tree_flatten(tree)
@@ -114,28 +114,28 @@
         >>> # keyword arguments
         >>> f_b = pytc.Partial(f, b=2, c=3)
         >>> f_a(1)
         a: 1, b: 2, c: 3
         6
 
     Note:
-        - The `...` is used to indicate a placeholder for positional arguments.
+        - The ``...`` is used to indicate a placeholder for positional arguments.
         - See: https://stackoverflow.com/a/7811270
         - `Partial` is used internally by `bcmap` which maps a function over pytrees
           leaves with automatic broadcasting for scalar arguments.
     """
 
     __slots__ = ["func", "args", "kwargs", "__weakref__"]  # type: ignore
 
     def __init__(self, func: Callable[..., Any], *args: Any, **kwargs: Any):
         """Initialize a `Partial` function.
 
         Args:
             func: The function to be partially applied.
-            args: Positional arguments to be partially applied. use `...` as a
+            args: Positional arguments to be partially applied. use ``...`` as a
                 placeholder for positional arguments.
             kwargs: Keyword arguments to be partially applied.
         """
         self.func = func
         self.args = args
         self.kwargs = kwargs
 
@@ -169,15 +169,17 @@
         is_leaf: a predicate function that returns True if the node is a leaf
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> import functools as ft
 
-        >>> class Test(pytc.TreeClass, leafwise=True):
+        >>> @pytc.autoinit
+        ... @pytc.leafwise
+        ... class Test(pytc.TreeClass):
         ...    a: tuple[int] = (1,2,3)
         ...    b: tuple[int] = (4,5,6)
         ...    c: jax.Array = jnp.array([1,2,3])
 
         >>> tree = Test()
 
         >>> # 0 is broadcasted to all leaves of the pytree
@@ -280,18 +282,66 @@
 
 
 def swop(func):
     # swaping the arguments of a two-arg function
     return ft.wraps(func)(lambda leaf, rhs: func(rhs, leaf))
 
 
-def _leafwise_transform(klass: type[T]) -> type[T]:
-    # add leafwise transform methods to the class
-    # that enable the user to apply a function to
-    # all the leaves of the tree
+def leafwise(klass: type[T]) -> type[T]:
+    """A class decorator that adds leafwise operators to a class.
+
+    Leafwise operators are operators that are applied to the leaves of a pytree.
+    For example leafwise ``__add__`` is equivalent to:
+
+    - ``jax.tree_map(lambda x: x + rhs, tree)`` if ``rhs`` is a scalar.
+    - ``jax.tree_map(lambda x, y: x + y, tree, rhs)`` if ``rhs`` is a pytree
+      with the same structure as ``tree``.
+
+    Args:
+        klass: The class to be decorated.
+
+    Returns:
+        The decorated class.
+
+    Note:
+        If a mathematically equivalent operator is already defined on the class,
+        then it is not overridden.
+
+    ==================      ============
+    Method                  Operator
+    ==================      ============
+    ``__add__``              ``+``
+    ``__and__``              ``&``
+    ``__ceil__``             ``math.ceil``
+    ``__divmod__``           ``divmod``
+    ``__eq__``               ``==``
+    ``__floor__``            ``math.floor``
+    ``__floordiv__``         ``//``
+    ``__ge__``               ``>=``
+    ``__gt__``               ``>``
+    ``__invert__``           ``~``
+    ``__le__``               ``<=``
+    ``__lshift__``           ``<<``
+    ``__lt__``               ``<``
+    ``__matmul__``           ``@``
+    ``__mod__``              ``%``
+    ``__mul__``              ``*``
+    ``__ne__``               ``!=``
+    ``__neg__``              ``-``
+    ``__or__``               ``|``
+    ``__pos__``              ``+``
+    ``__pow__``              ``**``
+    ``__round__``            ``round``
+    ``__sub__``              ``-``
+    ``__truediv__``          ``/``
+    ``__trunc__``            ``math.trunc``
+    ``__xor__``              ``^``
+    ==================      ============
+
+    """
     for key, method in (
         ("__abs__", uop(abs)),
         ("__add__", bop(op.add)),
         ("__and__", bop(op.and_)),
         ("__ceil__", uop(ceil)),
         ("__divmod__", bop(divmod)),
         ("__eq__", bop(op.eq)),
```

### Comparing `pytreeclass-0.4.0/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.5.0/pytreeclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.4.0
+Version: 0.5.0
 Summary: Visualize, create, and operate on JAX PyTree in the most intuitive way possible.
 Author-email: Mahmoud Asem <mahmoudasem00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pytreeclass-0.4.0/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.5.0/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.4.0/tests/test_indexing.py` & `pytreeclass-0.5.0/tests/test_indexing.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,32 +26,38 @@
 
 import pytreeclass as pytc
 from pytreeclass import TreeClass
 from pytreeclass._src.tree_base import _mutable_context
 from pytreeclass._src.tree_util import construct_tree
 
 
-class Tree(TreeClass, leafwise=True):
+@pytc.leafwise
+@pytc.autoinit
+class Tree(TreeClass):
     a: float
     b: float
     c: float
     d: jnp.ndarray
     name: str
 
     def __post_init__(self):
         self.name = pytc.freeze(self.name)
 
 
 def test_getter_by_val():
-    class level1(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class level1(TreeClass):
         a: int
         b: int
         c: int
 
-    class level2(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class level2(TreeClass):
         d: level1
         e: level1
 
     A = level2(
         d=level1(a=1, b=10, c=jnp.array([1, 2, 3, 4, 5])),
         e=level1(a=2, b=20, c=jnp.array([-1, -2, -3, -4, -5])),
     )
@@ -84,26 +90,32 @@
         B = A.at[A].get()
 
     # with pytest.raises(NotImplementedError):
     #     B = A.at[0].get()
 
 
 def test_getter_by_param():
-    class L0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L0(TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
 
-    class L1(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L1(TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
         d: L0 = L0()
 
-    class L2(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L2(TreeClass):
         a: int = 10
         b: int = 20
         c: int = 30
         d: L1 = L1()
 
     # t = L2()
 
@@ -111,20 +123,24 @@
     #     t.at["s"].get()
 
     # with pytest.raises(AttributeError):
     #     t.at["s"].apply(lambda _: 100)
 
 
 def test_setter_by_val():
-    class level1(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class level1(TreeClass):
         a: int
         b: int
         c: int
 
-    class level2(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class level2(TreeClass):
         d: level1
         e: level1
 
     A = level2(
         d=level1(a=1, b=10, c=jnp.array([1, 2, 3, 4, 5])),
         e=level1(a=2, b=20, c=jnp.array([-1, -2, -3, -4, -5])),
     )
@@ -140,41 +156,48 @@
     A = Tree(10, 20, 30, jnp.array([1, 2, 3, 4, 5]), ("A"))
 
     with pytest.raises(NotImplementedError):
         B = A.at[A].set(0)
 
     # with pytest.raises(NotImplementedError):
     #     B = A.at[0].set(0)
-
-    class L0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L0(TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
 
-    class L1(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L1(TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
         d: L0 = L0()
 
-    class L2(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L2(TreeClass):
         a: int = 10
         b: int = 20
         c: int = 30
         d: L1 = L1()
 
     t = L2()
 
     tt = L2(100, 200, 300, L1(10, 20, 30, L0(10, 20, 30)))
     lhs = t.at[t == t].set(tt)
     assert pytc.is_tree_equal(lhs, tt)
 
 
 def test_apply_and_its_derivatives():
-    class A(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(TreeClass):
         a: int
         b: int
         c: jnp.ndarray
 
     init = A(1, 2, jnp.array([1, 2, 3, 4, 5]))
 
     # By boolean pytree
@@ -201,26 +224,32 @@
     lhs = A(20, 30, jnp.array([20, 30, 40, 50, 60]))
     rhs = init.at[...].apply(lambda x: (x + 1) * 10)
     assert pytc.is_tree_equal(lhs, rhs)
 
     with pytest.raises(NotImplementedError):
         init.at[init].apply(lambda x: (x + 1) * 10)
 
-    class L0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L0(TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
 
-    class L1(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L1(TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
         d: L0 = L0()
 
-    class L2(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L2(TreeClass):
         a: int = 10
         b: int = 20
         c: int = 30
         d: L1 = L1()
 
     lhs = A(2, 3, jnp.array([2, 3, 4, 5, 6]))
     rhs = init.at[init == init].apply(lambda x: x + 1)
@@ -275,15 +304,17 @@
 
     lhs = A(1, 4, jnp.array([1, 4, 3, 4, 5]))
     rhs = init.at[init == 2].apply(lambda x: x * 2)
     assert pytc.is_tree_equal(lhs, rhs)
 
 
 def test_reduce():
-    class A(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(TreeClass):
         a: int
         b: int
         c: jnp.ndarray
 
     init = A(1, 2, jnp.array([1, 2, 3, 4, 5]))
 
     lhs = 2 + 2 + 3 + 4 + 5
@@ -294,54 +325,54 @@
     rhs = init.at[init > 2].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
     lhs = 0
     rhs = init.at[init > 100].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
-    class B(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class B(TreeClass):
         a: int
         b: int
         c: jnp.ndarray
         d: tuple
 
     init = B(1, 2, jnp.array([1, 2, 3, 4, 5]), (10, 20, 30))
 
     lhs = 2 + 2 + 3 + 4 + 5 + 10 + 20 + 30
     rhs = init.at[init > 1].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
     with pytest.raises(NotImplementedError):
         init.at[init].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: tuple[int]
 
     lhs = Tree((1, 2, 3)).at["a"].reduce(lambda x, y: x + y, initializer=0)
     assert lhs == 6
 
 
 def test_reduce_and_its_derivatives():
-    class Linear(TreeClass, leafwise=True):
-        weight: jnp.ndarray
-        bias: jnp.ndarray
-
+    @pytc.leafwise
+    class Linear(TreeClass):
         def __init__(self, key, in_dim, out_dim):
             self.weight = jax.random.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(
                 2 / in_dim
             )
             self.bias = jnp.ones((1, out_dim))
 
         # def __call__(self, x):
         #     return x @ self.weight + self.bias
 
-    class StackedLinear(TreeClass, leafwise=True):
-        l1: Linear
-        l2: Linear
-
+    @pytc.leafwise
+    class StackedLinear(TreeClass):
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             keys = jax.random.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
             self.l2 = Linear(key=keys[2], in_dim=hidden_dim, out_dim=out_dim)
 
     tree = StackedLinear(in_dim=1, out_dim=1, hidden_dim=5, key=jax.random.PRNGKey(0))
@@ -363,15 +394,17 @@
     npt.assert_allclose(
         tree.at[tree > 0].reduce(lambda x, y: x * jnp.prod(y), initializer=1),
         1.8088213,
     )
 
 
 def test_is_leaf():
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int
 
     t = Tree([1, 2, 3, None])
 
     mask = jtu.tree_map(lambda x: True, t, is_leaf=lambda x: x is None)
 
     assert pytc.is_tree_equal(
@@ -381,63 +414,79 @@
     assert pytc.is_tree_equal(
         t.at[mask].apply(lambda x: 10, is_leaf=lambda x: x is None),
         Tree([10, 10, 10, 10]),
     )
 
 
 def test_attribute_get():
-    class l0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     assert pytc.is_tree_equal(t.at["a"].get(), Tree(1, l0(None)))
     assert pytc.is_tree_equal(t.at["b"].at["a"].get(), Tree(None, l0(2)))
 
 
 def test_attribute_set():
-    class l0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     t.at["a"].set(10)
 
     assert pytc.is_tree_equal(t, Tree())
     assert pytc.is_tree_equal(t.at["a"].set(10), Tree(10, l0()))
     assert pytc.is_tree_equal(t.at["b"].at["a"].set(100), Tree(1, l0(100)))
 
 
 def test_attributre_apply():
-    class l0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     t.at["a"].apply(lambda _: 10)
 
     assert pytc.is_tree_equal(t, Tree())
     assert pytc.is_tree_equal(t.at["a"].apply(lambda _: 10), Tree(10))
     assert pytc.is_tree_equal(t.at["b"].at["a"].apply(lambda _: 100), Tree(1, l0(100)))
 
 
 def test_trace_get():
-    class l0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     assert pytc.is_tree_equal(t.at[0].get(), Tree(1, l0(None)))
     assert pytc.is_tree_equal(t.at[1].at[0].get(), Tree(None, l0(2)))
 
@@ -449,81 +498,99 @@
     # with pytest.raises(IndexError):
     #     t.at[0].at[1].apply(lambda _: 10)
     # with pytest.raises(IndexError):
     #     t.at[0].at[1].reduce(lambda _, __: 10)
 
 
 def test_trace_set():
-    class l0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     t.at["a"].set(10)
 
     assert pytc.is_tree_equal(t, Tree())
     assert pytc.is_tree_equal(t.at[0].set(10), Tree(10, l0()))
     assert pytc.is_tree_equal(t.at[1].at[0].set(100), Tree(1, l0(100)))
 
 
 def test_trace_apply():
-    class l0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     t.at["a"].apply(lambda _: 10)
 
     assert pytc.is_tree_equal(t, Tree())
     assert pytc.is_tree_equal(t.at[0].apply(lambda _: 10), Tree(10))
     assert pytc.is_tree_equal(t.at[1].at[0].apply(lambda _: 100), Tree(1, l0(100)))
 
 
 def test_trace_reduce():
-    class A(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(TreeClass):
         a: int
         b: int
         c: jnp.ndarray
 
     init = A(1, 2, jnp.array([1, 2, 3, 4, 5]))
 
     lhs = 1 + 2 + 3 + 4 + 5
     rhs = init.at[2].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
 
 def test_mixed_get():
-    class l0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
         b: int = 1
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
     assert pytc.is_tree_equal(t.at[1].at[t == 2].get(), Tree(None, l0(2, None)))
     assert pytc.is_tree_equal(t.at[t == 2].at[1].get(), Tree(None, l0(2, None)))
 
     # with pytest.raises(IndexError):
     #     t.at[0].at[2].get()
 
 
 def test_mixed_set():
-    class l0(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
         b: int = 1
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
 
     assert pytc.is_tree_equal(t.at["b"].at[t == 2].set(100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at[t == 2].at["b"].set(100), Tree(1, l0(100)))
@@ -532,56 +599,63 @@
     assert pytc.is_tree_equal(t.at["b"].at[0].set(100), Tree(1, l0(100)))
 
     # with pytest.raises(IndexError):
     #     assert pytc.is_tree_equal(t.at[0].at["b"].set(100), Tree(1, l0(100, 2)))
 
 
 def test_mixed_apply():
-    class l0(TreeClass, leafwise=True):
+    @pytc.autoinit
+    class l0(TreeClass):
         a: int = 2
         b: int = 1
 
-    class Tree(TreeClass, leafwise=True):
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: l0 = l0()
 
     t = Tree()
 
     assert pytc.is_tree_equal(t.at[1].at[t == 2].apply(lambda _: 100), Tree(1, l0(100)))
     assert pytc.is_tree_equal(t.at["b"].at[0].apply(lambda _: 100), Tree(1, l0(100)))
 
     # with pytest.raises(IndexError):
     #     t.at[0].at["a"].apply(lambda _: 100), Tree(1, l0(100))
 
 
 def test_method_call():
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
 
         def increment(self):
             self.a += 1
 
         def show(self):
             return 1
 
     t = Tree()
 
+    @pytc.autoinit
     class Tree2(TreeClass):
         b: Tree = Tree()
 
     assert pytc.is_tree_equal(t.at["increment"]()[1], Tree(2))
     assert pytc.is_tree_equal(Tree2().at["b"].at["show"]()[0], 1)
 
     with pytest.raises(AttributeError):
         t.at["bla"]()
 
     with pytest.raises(TypeError):
         t.at["a"]()
 
-    class A(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(TreeClass):
         a: int
 
         def __call__(self, x):
             self.a += x
             return x
 
     a = A(1)
@@ -591,17 +665,16 @@
     assert jtu.tree_leaves(b) == [3]
 
     with pytest.raises(TypeError):
         a.at[0](1)
 
 
 def test_composed_at():
-    class Tree(TreeClass, leafwise=True):
-        a: jnp.ndarray
-
+    @pytc.leafwise
+    class Tree(TreeClass):
         def __init__(self, a=jnp.array([1, 2, 3, 4, 5])) -> None:
             self.a = a
 
     t = Tree()
 
     assert pytc.is_tree_equal(
         t.at[t > 0].at[t < 0].get(), Tree(jnp.array([], dtype=int))
@@ -611,45 +684,53 @@
         t.at[t > 0].bet
 
     with pytest.raises(AttributeError):
         t.at["a"].bet
 
 
 def test_repr_str():
-    class Tree(TreeClass, leafwise=True):
+    @pytc.autoinit
+    @pytc.leafwise
+    class Tree(TreeClass):
         a: int = 1
         b: int = 2
 
     t = Tree()
 
     assert repr(t.at["a"]) == "TreeClassIndexer(tree=Tree(a=1, b=2), where=('a',))"
     assert str(t.at["a"]) == "TreeClassIndexer(tree=Tree(a=1, b=2), where=('a',))"
     assert repr(t.at[...]) == "TreeClassIndexer(tree=Tree(a=1, b=2), where=(Ellipsis,))"
 
 
 def test_not_equal():
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int = 1
         b: float = 1.0
 
     t = Tree()
 
     assert pytc.is_tree_equal(t.at[t != 10].set(10.0), Tree(a=10.0, b=10.0))
 
 
 def test_iterable_node():
-    class Tree(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Tree(TreeClass):
         a: int
 
     t = Tree([1, 2, 3, 4])
     assert pytc.is_tree_equal(t.at[...].set(True), Tree([True, True, True, True]))
 
 
 def test_call_context():
-    class L2(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L2(TreeClass):
         a: int = 1
 
         def delete(self, name):
             del self.a
 
     t = L2()
 
@@ -657,15 +738,17 @@
         tx.delete("a")
 
     with pytest.raises(AttributeError):
         t.delete("a")
 
 
 def test_unsupported_indexing_type():
-    class L2(TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L2(TreeClass):
         a: int = 1
 
         def delete(self, name):
             del self.a
 
     t = L2()
 
@@ -687,15 +770,16 @@
 
 
 def test_nested_indexing():
     class Dict(dict):
         # test `FlattenedIndexKey`
         pass
 
-    class Tree(pytc.TreeClass, leafwise=True):
+    @pytc.autoinit
+    class Tree(pytc.TreeClass):
         a: Any = (1, {"b": Dict({"c": 1})})
 
     tree = Tree()
     assert jtu.tree_leaves(tree.at["a"].at[1].at["b"].get())[0] == Dict({"c": 1})
     assert jtu.tree_leaves(tree.at[0].at[1].at["b"].get())[0] == Dict({"c": 1})
 
 
@@ -705,14 +789,15 @@
     assert repr(tree) == "Node(data=((None, <class 'list'>), [1, 2, [3, 4]]))"
 
     with pytest.raises(TypeError):
         tree.add_child("a")
 
 
 def test_regexkey():
+    @pytc.autoinit
     class Tree(pytc.TreeClass):
         weight_1: float = 1.0
         weight_2: float = 2.0
         weight_3: float = 3.0
         bias: float = 0.0
 
     tree = Tree()
@@ -760,27 +845,29 @@
                 return other == (self.name, self.type)
             return False
 
     assert jax.tree_util.tree_leaves(tree.at[MatchNameType("a", int)].get()) == [1]
 
 
 def test_multi_key():
+    @pytc.autoinit
     class Tree(pytc.TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
 
     tree = Tree()
     assert pytc.is_tree_equal(
         tree.at["a"].set(100).at["b"].set(100),
         tree.at["a", "b"].set(100),
     )
 
 
 def test_scan():
+    @pytc.autoinit
     class Tree(pytc.TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
         d: jax.Array = jnp.array([4, 5])
 
     tree = Tree()
```

### Comparing `pytreeclass-0.4.0/tests/test_nn.py` & `pytreeclass-0.5.0/tests/test_nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
         def __init__(self, key, in_dim, out_dim):
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
-    class StackedLinear(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    class StackedLinear(pytc.TreeClass):
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             keys = jr.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
             self.l2 = Linear(key=keys[1], in_dim=hidden_dim, out_dim=hidden_dim)
             self.l3 = Linear(key=keys[2], in_dim=hidden_dim, out_dim=out_dim)
 
@@ -130,25 +131,27 @@
     for _ in range(1, 10_001):
         value, nn = update(nn, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.0031012), atol=1e-5)
 
 
 def test_freeze_nondiff():
-    class Linear(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    class Linear(pytc.TreeClass):
         def __init__(self, key, in_dim, out_dim):
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
             self.use_bias = True
             self.count = 0
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
-    class StackedLinear(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    class StackedLinear(pytc.TreeClass):
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             self.name = "stack"
             keys = jr.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
             self.l2 = Linear(key=keys[1], in_dim=hidden_dim, out_dim=hidden_dim)
             self.l3 = Linear(key=keys[2], in_dim=hidden_dim, out_dim=out_dim)
```

### Comparing `pytreeclass-0.4.0/tests/test_tree_freeze.py` & `pytreeclass-0.5.0/tests/test_tree_freeze.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 import pytest
 
 import pytreeclass as pytc
 from pytreeclass._src.tree_util import tree_hash
 
 
 def test_freeze_unfreeze():
-    class A(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(pytc.TreeClass):
         a: int
         b: int
 
     a = A(1, 2)
     b = a.at[...].apply(pytc.freeze)
     c = (
         a.at["a"]
@@ -40,23 +42,29 @@
 
     assert jtu.tree_leaves(a) == [1, 2]
     assert jtu.tree_leaves(b) == []
     assert jtu.tree_leaves(c) == [1, 2]
 
     assert pytc.unfreeze(pytc.freeze(1.0)) == 1.0
 
-    class A(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(pytc.TreeClass):
         a: int
         b: int
 
-    class B(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class B(pytc.TreeClass):
         c: int = 3
         d: A = A(1, 2)
 
-    class A(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(pytc.TreeClass):
         a: int
         b: int
 
     a = A(1, 2)
     b = jtu.tree_map(pytc.freeze, a)
     c = (
         a.at["a"]
@@ -65,70 +73,86 @@
         .apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
     )
 
     assert jtu.tree_leaves(a) == [1, 2]
     assert jtu.tree_leaves(b) == []
     assert jtu.tree_leaves(c) == [1, 2]
 
-    class l0(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(pytc.TreeClass):
         a: int = 0
 
-    class l1(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l1(pytc.TreeClass):
         b: l0 = l0()
 
-    class l2(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l2(pytc.TreeClass):
         c: l1 = l1()
 
     t = jtu.tree_map(pytc.freeze, l2())
 
     assert jtu.tree_leaves(t) == []
     assert jtu.tree_leaves(t.c) == []
     assert jtu.tree_leaves(t.c.b) == []
 
-    class l1(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    class l1(pytc.TreeClass):
         def __init__(self):
             self.b = l0()
 
-    class l2(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    class l2(pytc.TreeClass):
         def __init__(self):
             self.c = l1()
 
     t = jtu.tree_map(pytc.freeze, l2())
     assert jtu.tree_leaves(t.c) == []
     assert jtu.tree_leaves(t.c.b) == []
 
 
 def test_freeze_errors():
     class T:
         pass
 
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: Any
 
     t = Test(T())
 
     # with pytest.raises(Exception):
     t.at[...].set(0)
 
     with pytest.raises(TypeError):
         t.at[...].apply(jnp.sin)
 
     t.at[...].reduce(jnp.sin)
 
 
 def test_freeze_with_ops():
-    class A(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(pytc.TreeClass):
         a: int
         b: int
 
-    class B(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class B(pytc.TreeClass):
         c: int = 3
         d: A = A(1, 2)
 
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: int = 1
         b: float = pytc.freeze(1.0)
         c: str = pytc.freeze("test")
 
     t = Test()
     assert jtu.tree_leaves(t) == [1]
 
@@ -140,31 +164,32 @@
 
     hash(t)
 
     t = Test()
     jtu.tree_map(pytc.unfreeze, t, is_leaf=pytc.is_frozen)
     jtu.tree_map(pytc.freeze, t)
 
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: int
 
     t = jtu.tree_map(pytc.freeze, (Test(100)))
 
     with pytest.raises(LookupError):
         pytc.is_tree_equal(t.at[...].set(0), t)
 
     with pytest.raises(LookupError):
         pytc.is_tree_equal(t.at[...].apply(lambda x: x + 1), t)
 
     with pytest.raises(LookupError):
         pytc.is_tree_equal(t.at[...].reduce(jnp.add, initializer=0), t)
 
-    class Test(pytc.TreeClass, leafwise=True):
-        x: jnp.ndarray
-
+    @pytc.leafwise
+    class Test(pytc.TreeClass):
         def __init__(self, x):
             self.x = x
 
     t = Test(jnp.array([1, 2, 3]))
     assert pytc.is_tree_equal(t.at[...].set(None), Test(x=None))
 
     class t0:
@@ -173,80 +198,96 @@
     class t1:
         a: int = t0()
 
     t = t1()
 
 
 def test_freeze_diagram():
-    class A(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class A(pytc.TreeClass):
         a: int
         b: int
 
-    class B(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class B(pytc.TreeClass):
         c: int = 3
         d: A = A(1, 2)
 
     a = B()
     a = a.at["d"].set(pytc.freeze(a.d))
     a = B()
 
     a = a.at["d"].set(pytc.freeze(a.d))  # = a.d.freeze()
 
 
 def test_freeze_mask():
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: int = 1
         b: int = 2
         c: float = 3.0
 
     t = Test()
 
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, t)) == []
 
 
 def test_freeze_nondiff():
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: int = pytc.freeze(1)
         b: str = "a"
 
     t = Test()
 
     assert jtu.tree_leaves(t) == ["a"]
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, t)) == []
     assert jtu.tree_leaves(
         (jtu.tree_map(pytc.freeze, t))
         .at["b"]
         .apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
     ) == ["a"]
 
-    class T0(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class T0(pytc.TreeClass):
         a: Test = Test()
 
     t = T0()
 
     assert jtu.tree_leaves(t) == ["a"]
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, t)) == []
 
     assert jtu.tree_leaves(t) == ["a"]
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, t)) == []
 
 
 def test_freeze_nondiff_with_mask():
-    class L0(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L0(pytc.TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
 
-    class L1(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L1(pytc.TreeClass):
         a: int = 1
         b: int = 2
         c: int = 3
         d: L0 = L0()
 
-    class L2(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class L2(pytc.TreeClass):
         a: int = 10
         b: int = 20
         c: int = 30
         d: L1 = L1()
 
     t = L2()
     t = t.at["d"].at["d"].at["a"].apply(pytc.freeze)
@@ -256,19 +297,23 @@
 
 
 def test_non_dataclass_input_to_freeze():
     assert jtu.tree_leaves(pytc.freeze(1)) == []
 
 
 def test_tree_mask():
-    class l0(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(pytc.TreeClass):
         x: int = 2
         y: int = 3
 
-    class l1(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l1(pytc.TreeClass):
         a: int = 1
         b: l0 = l0()
 
     tree = l1()
 
     assert jtu.tree_leaves(tree) == [1, 2, 3]
     assert jtu.tree_leaves(jtu.tree_map(pytc.freeze, tree)) == []
@@ -281,19 +326,23 @@
     assert jtu.tree_leaves(tree.at["a"].apply(pytc.freeze)) == [2, 3]
     assert jtu.tree_leaves(tree.at["b"].apply(pytc.freeze)) == [1]
     assert jtu.tree_leaves(tree.at["b"].at["x"].apply(pytc.freeze)) == [1, 3]
     assert jtu.tree_leaves(tree.at["b"].at["y"].apply(pytc.freeze)) == [1, 2]
 
 
 def test_tree_unmask():
-    class l0(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(pytc.TreeClass):
         x: int = 2
         y: int = 3
 
-    class l1(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l1(pytc.TreeClass):
         a: int = 1
         b: l0 = l0()
 
     tree = l1()
 
     frozen_tree = tree.at[...].apply(pytc.freeze)
     assert jtu.tree_leaves(frozen_tree) == []
@@ -310,19 +359,23 @@
     assert jtu.tree_leaves(unfrozen_tree) == [1]
 
     unfrozen_tree = frozen_tree.at["b"].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # fmt: skip
     assert jtu.tree_leaves(unfrozen_tree) == [2, 3]
 
 
 def test_tree_mask_unfreeze():
-    class l0(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l0(pytc.TreeClass):
         x: int = 2
         y: int = 3
 
-    class l1(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class l1(pytc.TreeClass):
         a: int = 1
         b: l0 = l0()
 
     tree = l1()
 
     mask = tree == tree
     frozen_tree = tree.at[...].apply(pytc.freeze)
@@ -331,15 +384,17 @@
 
     frozen_tree = tree.at["a"].apply(pytc.freeze)
     unfrozen_tree = frozen_tree.at["a"].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # fmt: skip
     assert jtu.tree_leaves(unfrozen_tree) == [1, 2, 3]
 
 
 def test_freeze_nondiff_func():
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: int = 1.0
         b: int = 2
         c: int = 3
         act: Callable = jax.nn.tanh
 
         def __call__(self, x):
             return self.act(x + self.a)
```

### Comparing `pytreeclass-0.4.0/tests/test_tree_operator.py` & `pytreeclass-0.5.0/tests/test_tree_operator.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,16 @@
 import pytest
 
 import pytreeclass as pytc
 from pytreeclass._src.tree_util import bcmap
 
 
 def test_bcmap():
-    class Test(pytc.TreeClass, leafwise=True):
-        a: tuple[int]
-        b: tuple[int]
-        c: jnp.ndarray
-        d: int
-
+    @pytc.leafwise
+    class Test(pytc.TreeClass):
         def __init__(self, a=(1, 2, 3), b=(4, 5, 6), c=jnp.array([1, 2, 3]), d=1):
             self.a = a
             self.b = b
             self.c = c
             self.d = d
 
     tree = Test()
@@ -54,15 +50,17 @@
     assert pytc.is_tree_equal(lhs, rhs)
 
     lhs = bcmap(jnp.where)(condition=tree > 1, x=0, y=tree)
     assert pytc.is_tree_equal(lhs, rhs)
 
 
 def test_math_operations():
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: float
         b: float
         c: float
         name: str
 
         def __post_init__(self):
             self.name = pytc.freeze(self.name)
@@ -72,15 +70,17 @@
 
     assert (A + A) == Test(20, 40, 60, ("A"))
     assert (A - A) == Test(0, 0, 0, ("A"))
     # assert ((A["a"] + A) | A) == Test(20, 20, 30, ("A"))
     assert A.at[...].reduce(lambda x, y: x + jnp.sum(y)) == jnp.array(60)
     assert abs(A) == A
 
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: float
         b: float
         name: str
 
         def __post_init__(self):
             self.name = pytc.freeze(self.name)
 
@@ -119,15 +119,17 @@
     assert A**A == Test(-(10**-10), 20**20, ("A"))
     assert round(A) == Test(round(-10), round(20), ("A"))
     assert A - A == Test(-10 + 10, 20 - 20, ("A"))
     assert A ^ A == Test(-10 ^ -10, 20 ^ 20, ("A"))
 
 
 def test_math_operations_errors():
-    class Test(pytc.TreeClass, leafwise=True):
+    @pytc.leafwise
+    @pytc.autoinit
+    class Test(pytc.TreeClass):
         a: float
         b: float
         c: float
         name: str
         d: jnp.ndarray = None
 
         def __post_init__(self):
```

### Comparing `pytreeclass-0.4.0/tests/test_tree_pprint.py` & `pytreeclass-0.5.0/tests/test_tree_pprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     tree_repr,
     tree_repr_with_trace,
     tree_str,
     tree_summary,
 )
 
 
-class Repr1(TreeClass, leafwise=True):
+@pytc.leafwise
+@pytc.autoinit
+class Repr1(TreeClass):
     a: int = 1
     b: str = "string"
     c: float = 1.0
     d: tuple = "a" * 5
     e: list = None
     f: set = None
     g: dict = None
@@ -194,37 +196,42 @@
         a: int = 1
 
     assert pytc.tree_repr(Test()) == pytc.tree_str(Test()) == "Test(a=1)"
     assert pytc.tree_repr(Test(), depth=0) == "Test(...)"
 
 
 def test_extra_tree_diagram():
+    @pytc.autoinit
     class L0(TreeClass):
         a: int = 1
         b: int = 2
 
+    @pytc.autoinit
     class L1(TreeClass):
         c: L0 = L0()
         d: int = 3
 
+    @pytc.autoinit
     class L2(TreeClass):
         e: int = 4
         f: L1 = L1()
         g: L0 = L0()
         h: int = 5
 
     tree = L2()
     # trunk-ignore(flake8/E501)
     out = "L2\n├── .e=4\n├── .f:L1\n│   ├── .c:L0\n│   │   ├── .a=1\n│   │   └── .b=2\n│   └── .d=3\n├── .g:L0\n│   ├── .a=1\n│   └── .b=2\n└── .h=5"
 
     assert (tree_diagram(tree)) == out
 
+    @pytc.autoinit
     class L0(TreeClass):
         a: int = 1
 
+    @pytc.autoinit
     class L1(TreeClass):
         b: L0 = L0()
 
     tree = L1()
 
     assert tree_diagram(tree) == "L1\n└── .b:L0\n    └── .a=1"
 
@@ -235,15 +242,17 @@
     with pytest.raises(TypeError):
         tree_summary(1, depth="a")
     with pytest.raises(TypeError):
         tree_mermaid(1, depth="a")
 
 
 def test_tree_repr_with_trace():
-    class Test(TreeClass, leafwise=True):
+    @pytc.autoinit
+    @pytc.leafwise
+    class Test(TreeClass):
         a: int = 1
         b: float = 2.0
 
     tree = Test()
 
     assert (
         str(tree_repr_with_trace(tree))
```

### Comparing `pytreeclass-0.4.0/tests/test_tree_viz_util.py` & `pytreeclass-0.5.0/tests/test_tree_viz_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,40 +14,26 @@
 
 from __future__ import annotations
 
 import jax
 import jax.nn.initializers as ji
 import jax.tree_util as jtu
 
-from pytreeclass._src.tree_pprint import _hbox, _hstack, _table, _vbox, func_pp, pp
-
-
-def test_vbox():
-    assert _vbox("a", " a", "a ") == "┌──┐\n│a │\n├──┤\n│ a│\n├──┤\n│a │\n└──┘"
-    assert _vbox("a", "b") == "┌─┐\n│a│\n├─┤\n│b│\n└─┘"
-
-
-def test_hbox():
-    assert _hbox("a", "b", "c") == "┌─┬─┬─┐\n│a│b│c│\n└─┴─┴─┘"
-    assert _hbox("a") == "┌─┐\n│a│\n└─┘"
+from pytreeclass._src.tree_pprint import _table, func_pp, pp
 
 
 def test_table():
-    col1 = ["1\n", "2"]
-    col2 = ["3", "4000"]
+    col1 = ["1\n", "3"]
+    col2 = ["2", "4000"]
     assert (
-        _table([col1, col2], transpose=True)
+        _table([col1, col2])
         == "┌─┬────┐\n│1│3   │\n│ │    │\n├─┼────┤\n│2│4000│\n└─┴────┘"
     )
 
 
-def test_hstack():
-    assert _hstack(_hbox("a"), _vbox("b", "c")) == "┌─┬─┐\n│a│b│\n└─┼─┤\n  │c│\n  └─┘"
-
-
 def test_func_pp():
     def example(a: int, b=1, *c, d, e=2, **f) -> str:
         ...  # fmt: skip
 
     assert (
         func_pp(example, indent=0, kind="str", width=60, depth=0, seen=set())
         == "example(a, b, *c, d, e, **f)"
```

### Comparing `pytreeclass-0.4.0/tests/test_treeclass.py` & `pytreeclass-0.5.0/tests/test_treeclass.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 
 
 def test_fields():
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1, metadata={"meta": 1})
         b: int = 2
 
     assert len(pytc.fields(Test)) == 2
     assert pytc.fields(Test)[0].metadata == {"meta": 1}
 
@@ -40,109 +41,100 @@
 
 def test_field():
     assert pytc.field(default=1).default == 1
 
     with pytest.raises(TypeError):
         pytc.field(metadata=1)
 
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1, kind="POS_ONLY")
         b: int = 2
 
     with pytest.raises(TypeError):
         # positonal only for a
         Test(a=1, b=2)
 
     assert Test(1, b=2).a == 1
     assert Test(1, 2).b == 2
 
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1, kind="POS_ONLY")
         b: int = pytc.field(default=2, kind="POS_ONLY")
 
     assert Test(1, 2).a == 1
     assert Test(1, 2).b == 2
 
     # keyword only
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1, kind="KW_ONLY")
         b: int = 2
 
     with pytest.raises(TypeError):
         Test(1, 2)
 
     with pytest.raises(TypeError):
         Test(1, b=2)
 
     assert Test(a=1, b=2).a == 1
 
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1, kind="POS_ONLY")
         b: int = pytc.field(default=2, kind="KW_ONLY")
 
     with pytest.raises(TypeError):
         Test(1, 2)
 
     assert Test(1, b=2).b == 2
 
     with pytest.raises(TypeError):
         Test(a=1, b=2)
 
     # test when init is False
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1, init=False, kind="KW_ONLY")
         b: int = 2
 
     with pytest.raises(TypeError):
         Test(1, 2)
 
     assert Test(b=2).a == 1
 
-    class Test(pytc.TreeClass):
-        a: int = pytc.field(default=1)
-
-        def __init__(self) -> None:
-            pass
-
-    with pytest.raises(AttributeError):
-        Test()
-
 
 def test_field_alias():
+    @pytc.autoinit
     class Tree(pytc.TreeClass):
         _name: str = pytc.field(alias="name")
 
     tree = Tree(name="test")
     assert tree._name == "test"
 
     with pytest.raises(TypeError):
         pytc.field(alias=1)
 
 
 def test_field_nondiff():
     class Test(pytc.TreeClass):
-        a: jax.Array
-        b: jax.Array
-
         def __init__(
             self,
             a=pytc.freeze(jnp.array([1, 2, 3])),
             b=pytc.freeze(jnp.array([4, 5, 6])),
         ):
             self.a = a
             self.b = b
 
     test = Test()
 
     assert jtu.tree_leaves(test) == []
 
     class Test(pytc.TreeClass):
-        a: jax.Array
-        b: jax.Array
-
         def __init__(self, a=jnp.array([1, 2, 3]), b=jnp.array([4, 5, 6])):
             self.a = pytc.freeze(a)
             self.b = b
 
     test = Test()
     npt.assert_allclose(jtu.tree_leaves(test)[0], jnp.array([4, 5, 6]))
 
@@ -152,40 +144,43 @@
 #         a: jax.Array
 
 #     # with pytest.raises(TypeError):
 #     hash(T(jnp.array([1, 2, 3])))
 
 
 def test_post_init():
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = 1
 
         def __post_init__(self):
             self.a = 2
 
     t = Test()
 
     assert t.a == 2
 
 
 def test_subclassing():
+    @pytc.autoinit
     class L0(pytc.TreeClass):
         a: int = 1
         b: int = 3
         c: int = 5
 
         def inc(self, x):
             return x
 
         def sub(self, x):
             return x - 10
 
         def __post_init__(self):
             self.c = 5
 
+    @pytc.autoinit
     class L1(L0):
         a: int = 2
         b: int = 4
 
         def __post_init__(self):
             self.d = 5
 
@@ -195,14 +190,15 @@
     l1 = L1()
 
     assert jtu.tree_leaves(l1) == [2, 4, 5, 5]
     assert l1.inc(10) == 20
     assert l1.sub(10) == 0
     assert l1.d == 5
 
+    @pytc.autoinit
     class L1(L0):
         a: int = 2
         b: int = 4
 
     l1 = L1()
 
     assert jtu.tree_leaves(l1) == [2, 4, 5]
@@ -218,37 +214,40 @@
     tt = copy.copy(t)
 
     assert tt.a == 10
     assert tt.b == 20
 
 
 def test_copy():
+    @pytc.autoinit
     class L0(pytc.TreeClass):
         a: int = 1
         b: int = 3
         c: int = 5
 
     t = L0()
 
     assert copy.copy(t).a == 1
     assert copy.copy(t).b == 3
     assert copy.copy(t).c == 5
 
 
 def test_delattr():
+    @pytc.autoinit
     class L0(pytc.TreeClass):
         a: int = 1
         b: int = 3
         c: int = 5
 
     t = L0()
 
     with pytest.raises(AttributeError):
         del t.a
 
+    @pytc.autoinit
     class L2(pytc.TreeClass):
         a: int = 1
 
         def delete(self, name):
             del self.a
 
     t = L2()
@@ -290,75 +289,64 @@
 
 def test_is_tree_equal():
     assert pytc.is_tree_equal(1, 1)
     assert pytc.is_tree_equal(1, 2) is False
     assert pytc.is_tree_equal(1, 2.0) is False
     assert pytc.is_tree_equal([1, 2], [1, 2])
 
+    @pytc.autoinit
     class Test1(pytc.TreeClass):
         a: int = 1
 
     class Test2(pytc.TreeClass):
         a: jax.Array
 
         def __init__(self) -> None:
             self.a = jnp.array([1, 2, 3])
 
     assert pytc.is_tree_equal(Test1(), Test2()) is False
 
     assert pytc.is_tree_equal(jnp.array([1, 2, 3]), jnp.array([1, 2, 3]))
     assert pytc.is_tree_equal(jnp.array([1, 2, 3]), jnp.array([1, 3, 3])) is False
 
+    @pytc.autoinit
     class Test3(pytc.TreeClass):
         a: int = 1
         b: int = 2
 
     assert pytc.is_tree_equal(Test1(), Test3()) is False
 
     assert pytc.is_tree_equal(jnp.array([1, 2, 3]), 1) is False
 
 
-def test_params():
-    class l0(pytc.TreeClass):
-        a: int = 2
-
-    class l1(pytc.TreeClass):
-        a: int = 1
-        b: l0 = l0()
-
-    t1 = l1(1, l0(100))
-
-    # t2 = copy.copy(t1)
-    # t3 = l1(1, l0(100))
-
-    with pytest.raises(AttributeError):
-        t1.__FIELDS__["a"].default = 100
-
-
 def test_mutable_field():
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class Test(pytc.TreeClass):
             a: list = [1, 2, 3]
 
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class Test2(pytc.TreeClass):
             a: list = pytc.field(default=[1, 2, 3])
 
 
 def test_setattr_delattr():
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class Test(pytc.TreeClass):
             def __setattr__(self, k, v):
                 pass
 
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class _(pytc.TreeClass):
             def __delattr__(self, k):
                 pass
 
 
 def test_callbacks():
     def instance_validator(types):
@@ -373,90 +361,87 @@
         def _range_validator(x):
             if x < min or x > max:
                 raise AssertionError
             return x
 
         return _range_validator
 
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(callbacks=[instance_validator(int)])
 
     with pytest.raises(AssertionError):
         Test(a="a")
 
     assert Test(a=1).a == 1
 
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(callbacks=[instance_validator((int, float))])
 
     assert Test(a=1).a == 1
     assert Test(a=1.0).a == 1.0
 
     with pytest.raises(AssertionError):
         Test(a="a")
 
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(callbacks=[range_validator(0, 10)])
 
     with pytest.raises(AssertionError):
         Test(a=-1)
 
     assert Test(a=0).a == 0
 
     with pytest.raises(AssertionError):
         Test(a=11)
 
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(callbacks=[range_validator(0, 10), instance_validator(int)])
 
     with pytest.raises(AssertionError):
         Test(a=-1)
 
     with pytest.raises(AssertionError):
         Test(a=11)
 
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class Test(pytc.TreeClass):
             a: int = pytc.field(callbacks=1)
 
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class Test(pytc.TreeClass):
             a: int = pytc.field(callbacks=[1])
 
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class Test(pytc.TreeClass):
             a: int = pytc.field(callbacks=[lambda: True])
 
         Test(a=1)
 
 
 def test_treeclass_frozen_field():
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(callbacks=[pytc.freeze])
 
     t = Test(1)
 
     assert t.a == pytc.freeze(1)
     assert jtu.tree_leaves(t) == []
 
 
-def test_key_error():
-    class Test(pytc.TreeClass):
-        a: int = pytc.field()
-
-        def __init__(self) -> None:
-            return
-
-    with pytest.raises(AttributeError):
-        Test()
-
-
 def test_super():
     class Test(pytc.TreeClass):
         # a:int
         def __init__(self) -> None:
             super().__init__()
 
     Test()
@@ -485,14 +470,15 @@
             return 1
 
     assert Test().__repr__() == "a"
     assert Test() + Test() == 1
 
 
 def test_optional_param():
+    @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1)
 
     with pytest.raises(TypeError):
         Test() < Test()
 
 
@@ -522,22 +508,25 @@
 def test_benchmark_dataclass_class(benchmark):
     benchmark(benchmark_dataclass_class)
 
 
 def test_self_field_name():
     with pytest.raises(ValueError):
 
+        @pytc.autoinit
         class Tree(pytc.TreeClass):
             self: int = pytc.field()
 
 
 def test_instance_field_map():
+    @pytc.autoinit
     class Parameter(pytc.TreeClass):
         value: Any
 
+    @pytc.autoinit
     class Tree(pytc.TreeClass):
         bias: int = 0
 
         def add_param(self, name, param):
             return setattr(self, name, param)
 
     tree = Tree()
@@ -559,39 +548,43 @@
     assert f_b(2) == 6
 
     assert f_b == f_b
     assert hash(f_b) == hash(f_b)
 
 
 def test_kind():
+    @pytc.autoinit
     class Tree(pytc.TreeClass):
         a: int = pytc.field(kind="VAR_POS")
         b: int = pytc.field(kind="POS_ONLY")
         c: int = pytc.field(kind="VAR_KW")
         d: int
 
     params = dict(inspect.signature(Tree.__init__).parameters)
 
     assert params["a"].kind is inspect.Parameter.VAR_POSITIONAL
     assert params["b"].kind is inspect.Parameter.POSITIONAL_ONLY
     assert params["c"].kind is inspect.Parameter.VAR_KEYWORD
     assert params["d"].kind is inspect.Parameter.POSITIONAL_OR_KEYWORD
 
+    @pytc.autoinit
     class Tree(pytc.TreeClass):
         a: int = pytc.field(kind="VAR_POS")
         b: int = pytc.field(kind="KW_ONLY")
 
     params = dict(inspect.signature(Tree.__init__).parameters)
     assert params["a"].kind is inspect.Parameter.VAR_POSITIONAL
     assert params["b"].kind is inspect.Parameter.KEYWORD_ONLY
 
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class Tree(pytc.TreeClass):
             a: int = pytc.field(kind="VAR_POS")
             b: int = pytc.field(kind="VAR_POS")
 
     with pytest.raises(TypeError):
 
+        @pytc.autoinit
         class Tree(pytc.TreeClass):
             a: int = pytc.field(kind="VAR_KW")
             b: int = pytc.field(kind="VAR_KW")
```

### Comparing `pytreeclass-0.4.0/tests/test_under_jit.py` & `pytreeclass-0.5.0/tests/test_under_jit.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,20 +16,24 @@
 import jax
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 
 
 def test_ops_with_jit():
-    class T0(pytc.TreeClass, leafwise=True):
+    @pytc.autoinit
+    @pytc.leafwise
+    class T0(pytc.TreeClass):
         a: jax.Array = jnp.array(1)
         b: jax.Array = jnp.array(2)
         c: jax.Array = jnp.array(3)
 
-    class T1(pytc.TreeClass, leafwise=True):
+    @pytc.autoinit
+    @pytc.leafwise
+    class T1(pytc.TreeClass):
         a: jax.Array = jnp.array(1)
         b: jax.Array = jnp.array(2)
         c: jax.Array = jnp.array(3)
         d: jax.Array = jnp.array([1, 2, 3])
 
     @jax.jit
     def getter(tree):
```

