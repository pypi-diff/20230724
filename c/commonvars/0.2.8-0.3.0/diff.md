# Comparing `tmp/commonvars-0.2.8.tar.gz` & `tmp/commonvars-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonvars-0.2.8.tar", max compression
+gzip compressed data, was "commonvars-0.3.0.tar", max compression
```

## Comparing `commonvars-0.2.8.tar` & `commonvars-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9623 2023-07-14 04:52:21.802097 commonvars-0.2.8/commonvars/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 10:15:47.964651 commonvars-0.2.8/commonvars/py.typed
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 commonvars-0.2.8/LICENSE
--rw-r--r--   0        0        0     3454 2023-07-14 04:52:48.015999 commonvars-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     3917 2023-07-14 00:08:34.938392 commonvars-0.2.8/README.md
--rw-r--r--   0        0        0     4270 1970-01-01 00:00:00.000000 commonvars-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-22 22:06:48.884451 commonvars-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3811 2023-07-24 05:06:35.202518 commonvars-0.3.0/README.md
+-rw-r--r--   0        0        0     9995 2023-07-24 05:01:48.350951 commonvars-0.3.0/commonvars/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 22:06:48.884451 commonvars-0.3.0/commonvars/py.typed
+-rw-r--r--   0        0        0     3587 2023-07-24 05:35:42.293747 commonvars-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 commonvars-0.3.0/PKG-INFO
```

### Comparing `commonvars-0.2.8/commonvars/__init__.py` & `commonvars-0.3.0/commonvars/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """`commonvars`.
 
 A simple & straight-forward Python library for creating common variables
 (context-dependent proxy objects).
 
 (C) bswck, 2023
 """
+from __future__ import annotations
+
 import operator
 from collections.abc import Callable
 from contextlib import suppress
 from functools import partial
-from typing import Any, Protocol, TypeVar, cast, runtime_checkable
+from typing import Any, Protocol, TypeVar, cast, overload, runtime_checkable
 
 __all__ = ("commonvar", "proxy")
 
 _T = TypeVar("_T")
+_MISSING = object()
 
 
 @runtime_checkable
 class Manager(Protocol[_T]):
     """Protocol for commonvars managers.
 
     Matches `contextvars.ContextVar`.
@@ -28,15 +31,15 @@
 
         Raises
         ------
         LookupError
             If no object is bound to the manager.
         """
 
-    def set(self, value: _T) -> Any:
+    def set(self, value: _T, /) -> Any:
         """Set the current value of the manager."""
 
 
 def commonvar_descriptor(
     cls: type[_T] | None,
     mgr: Manager[_T],
     getter: Callable[[Manager[_T]], _T],
@@ -73,53 +76,62 @@
     descriptor
         A descriptor object that can be used to create commonvars delegates.
 
     """
 
     class _ZeugVarDescriptor:
         attr_name: str
+        predefined_attr: Any = _MISSING
 
         def __init__(self) -> None:
             self.attr_name = None  # type: ignore[assignment]
 
         def __set_name__(self, owner: type[_T], name: str) -> None:
             self.attr_name = name
 
-        def __get__(self, instance: _T, owner: type[_T] | None) -> Any:
             if self.attr_name == "__getattr__":
 
-                def attribute(name: str) -> Any:
+                def predefined_getattr(name: str) -> Any:
                     return getattr(getter(mgr), name)
 
+                self.predefined_attr = predefined_getattr
+
             elif self.attr_name in ("__repr__", "__str__"):
-                with suppress(RuntimeError):
-                    return getattr(getter(mgr), self.attr_name)
 
-                def attribute() -> str:  # type: ignore[misc]
+                def predefined_repr() -> str:
                     if cls is None:
                         return "<unbound commonvar>"
                     return f"<unbound {cls.__name__!r} object>"
 
+                self.predefined_attr = predefined_repr
+
+        def __get__(self, instance: _T, owner: type[_T] | None) -> Any:
+            if self.attr_name in ("__repr__", "__str__"):
+                with suppress(RuntimeError):
+                    return getattr(getter(mgr), self.attr_name)
+
+            if self.predefined_attr is not _MISSING:
+                return self.predefined_attr
+
+            try:
+                obj = getter(mgr)
+            except RuntimeError:
+                if callable(undefined):
+                    attribute = undefined
+
+                else:
+                    raise
             else:
                 try:
-                    obj = getter(mgr)
-                except RuntimeError:
-                    if callable(undefined):
-                        attribute = undefined
-
-                    else:
+                    attribute = getattr(obj, self.attr_name)
+                except AttributeError:
+                    if not callable(fallback):
                         raise
-                else:
-                    try:
-                        attribute = getattr(obj, self.attr_name)
-                    except AttributeError:
-                        if not callable(fallback):
-                            raise
 
-                        attribute = partial(fallback, obj)
+                    attribute = partial(fallback, obj)
 
             if inplace:
 
                 def _apply_inplace(*args: Any, **kwargs: Any) -> _T:
                     ret = attribute(*args, **kwargs)
                     setter(mgr, ret)
                     return instance
@@ -152,16 +164,16 @@
 def _cv_setter(mgr: Manager[_T], value: _T) -> None:
     mgr.set(value)
 
 
 def commonvar(
     mgr: Manager[_T],
     cls: type[_T] | None = None,
-    getter: Callable[[Manager[_T]], _T] = None,  # type: ignore[assignment]
-    setter: Callable[[Manager[_T], _T], None] = None,  # type: ignore[assignment]
+    getter: Callable[[Manager[_T]], _T] | None = None,
+    setter: Callable[[Manager[_T], _T], None] | None = None,
 ) -> _T:
     """Create a common variable, i.e. a proxy object.
 
     Parameters
     ----------
     mgr
         Manager object. Must implement the `Manager` protocol.
@@ -179,25 +191,27 @@
         A proxy object.
     """
 
     # pylint: disable=too-many-statements
 
     if getter is None:
         getter = _cv_getter
+    getter_func = getter
 
     if setter is None:
         setter = _cv_setter
+    setter_func = setter
 
     if cls is None:
         with suppress(RuntimeError):
-            cls = type(getter(mgr))
+            cls = type(getter_func(mgr))
 
-    descriptor = partial(commonvar_descriptor, cls, mgr, getter, setter)
+    descriptor = partial(commonvar_descriptor, cls, mgr, getter_func, setter_func)
 
-    class _CommonVarMeta:
+    class _CommonVarClass:  # pylint: disable=too-few-public-methods
         __doc__ = descriptor()
         __wrapped__ = descriptor()
         __repr__ = descriptor()
         __str__ = descriptor()
         __bytes__ = descriptor()
         __format__ = descriptor()
         __lt__ = descriptor()
@@ -261,15 +275,15 @@
         __isub__ = descriptor(fallback=_op_fallback("__sub__"), inplace=True)
         __imul__ = descriptor(fallback=_op_fallback("__mul__"), inplace=True)
         __imatmul__ = descriptor(fallback=_op_fallback("__matmul__"), inplace=True)
         __itruediv__ = descriptor(fallback=_op_fallback("__truediv__"), inplace=True)
         __ifloordiv__ = descriptor(fallback=_op_fallback("__floordiv__"), inplace=True)
         __imod__ = descriptor(fallback=_op_fallback("__mod__"), inplace=True)
         __ipow__ = descriptor(fallback=_op_fallback("__pow__"), inplace=True)
-        __ilshift__ = descriptor(fallback=_op_fallback("__lshift_"), inplace=True)
+        __ilshift__ = descriptor(fallback=_op_fallback("__lshift__"), inplace=True)
         __irshift__ = descriptor(fallback=_op_fallback("__rshift__"), inplace=True)
         __iand__ = descriptor(fallback=_op_fallback("__and__"), inplace=True)
         __ixor__ = descriptor(fallback=_op_fallback("__xor__"), inplace=True)
         __ior__ = descriptor(fallback=_op_fallback("__or__"), inplace=True)
         __neg__ = descriptor()
         __pos__ = descriptor()
         __abs__ = descriptor()
@@ -289,14 +303,14 @@
         __anext__ = descriptor()
         __aenter__ = descriptor()
         __aexit__ = descriptor()
         __copy__ = descriptor()
         __deepcopy__ = descriptor()
 
     if cls is not None:
-        _CommonVarMeta.__name__ = _CommonVarMeta.__qualname__ = cls.__name__
+        _CommonVarClass.__name__ = _CommonVarClass.__qualname__ = cls.__name__
     else:
-        _CommonVarMeta.__name__ = _CommonVarMeta.__qualname__ = f"commonvar_{id(mgr):x}"
-    return cast(_T, _CommonVarMeta())
+        _CommonVarClass.__name__ = _CommonVarClass.__qualname__ = f"commonvar_{id(mgr):x}"
+    return cast(_T, _CommonVarClass())
 
 
 proxy = commonvar
```

### Comparing `commonvars-0.2.8/README.md` & `commonvars-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,130 @@
-## `commonvars`
-
-A simple & straight-forward Python library for creating type-safe, context-dependent proxy objects.
-
-## Example
-
-The following example shows how to use `commonvars` with `contextvars`:
-
-```python
->>> from contextvars import ContextVar
->>> from commonvars import commonvar
-...
->>> count_var = ContextVar("count_var")
->>> count = commonvar(counter, int)
-...
->>> count
-<unbound 'int' object>
->>> count_var.set(0)
->>> count
-0
->>> count += 1
->>> count
-1
->>> count_var.get()
-1
->>> count -= 1
->>> count
-0
->>> count_var.set(1000)
-<Token var=<ContextVar name='count_var' at ...> at ...>
->>> count
-1000
-```
-
-## Ok, but what is this?
-
-`commonvars` is a Python module for creating context-dependent proxy objects.
-
-By 'proxy' we mean any object that forwards attribute access to another
-object. By 'context-dependent' we mean that the object to which the proxy
-forwards attribute access can change depending on the context in which the
-proxy is used.
-
-### Have you ever wondered how `flask.request` works?
-
-How is it possible
-that [`flask.request`](https://tedboy.github.io/flask/interface_api.incoming_request_data.html?highlight=request#flask.request)
-is different for each request, despite being a global variable?
-
-The answer is that `flask.request` is a such a proxy object as an instance of `werkzeug.local.LocalProxy`.
-For every request, `flask.request` forwards attribute access to a different `flask.Request` object.
-
-The functionality of `commonvars.commonvar()` (or, as you prefer, `commonvars.proxy()`) is a more generic version of `werkzeug.local.LocalProxy`.
-
-It takes a `Manager` object and the class of the object to which the proxy points.
-
-The `Manager` object must have `get` and `set` methods. The `get` method returns
-the object to which the would forward attribute access. The `set` method sets it, obviously.
-`set` is called when the proxy is being inplace modified, for example within the `+=` reassigning operator.
-The class parameter is optional, but it is strongly recommended for some corner-cases.
-The user might provide custom `getter` and `setter` functions that change the way 
-`Manager.get()` and `Manage.set()` are called.
-This might be useful when there is the need to keep track of the tokens
-returned by `ContextVar.set()`, if using `ContextVar` as the manager.
-
-## When would you use `commonvars`?
-
-You could use `commonvars` when...
-* ...writing a thread-safe application that operates on resources specific for separate threads.
-* ...improving code readability by avoiding passing around the same object to every function.
-* ...writing a web application that operates on resources specific per request.
-* ...writing an asynchronous application that operates on resources specific between tasks.
-* ...having any other case where you could use common variables that are context-dependent!
-
-## Installation
-
-### pip
-```bash
-$ pip install commonvars
-```
-
-### poetry
-
-You can add `commonvars` as a dependency with the following command:
-
-```bash
-$ poetry add commonvars
-```
-
-Or by directly specifying it in the configuration like so:
-
-```toml
-[tool.poetry.dependencies]
-"commonvars" = "^0.2.0"
-```
-
-Alternatively, you can add it directly from the source:
-
-```toml
-[tool.poetry.dependencies.commonvars]
-git = "https://github.com/bswck/commonvars.git"
-```
-
-## Documentation
-
-### `commonvars.commonvar(mgr, cls=None, getter=None, setter=None)`
-
-Creates a context-dependent proxy object.
-
-#### Parameters
-* `manager`: Manager object. Must implement the `Manager` protocol. Matches `contextvars.ContextVar`.
-* `cls`: The class of the underlying variable accessed within the manager. Optional.
-* `getter`: A function that returns the underlying variable from the manager. Optional.
-* `setter`: A function that sets the underlying variable within the manager. Optional.
+Metadata-Version: 2.1
+Name: commonvars
+Version: 0.3.0
+Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
+Home-page: https://github.com/bswck/commonvars
+Author: bswck
+Author-email: bswck.dev@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+## `commonvars v0.3.0`
+
+A simple & straight-forward Python library for creating type-safe, context-dependent proxy objects.
+
+## Example
+
+The following example shows how to use `commonvars` with `contextvars`:
+
+```python
+>>> from contextvars import ContextVar
+>>> from commonvars import commonvar
+...
+>>> count_var = ContextVar("count_var")
+>>> count = commonvar(count_var, int)
+...
+>>> count
+<unbound 'int' object>
+>>> count_var.set(0)
+>>> count
+0
+>>> count += 1
+>>> count
+1
+>>> count_var.get()
+1
+>>> count -= 1
+>>> count
+0
+>>> count_var.set(1000)
+<Token var=<ContextVar name='count_var' at ...> at ...>
+>>> count
+1000
+```
+
+## Ok, but what is this?
+
+`commonvars` is a Python module for creating context-dependent proxy objects.
+
+By 'proxy' we mean any object that forwards attribute access to another
+object. By 'context-dependent' we mean that the object to which the proxy
+forwards attribute access can change depending on the context in which the
+proxy is used.
+
+### Have you ever wondered how `flask.request` works?
+
+How is it possible
+that [`flask.request`](https://tedboy.github.io/flask/interface_api.incoming_request_data.html?highlight=request#flask.request)
+is different for each request, despite being a global variable?
+
+The answer is that `flask.request` is a such a proxy object as an instance of `werkzeug.local.LocalProxy`.
+For every request, `flask.request` forwards attribute access to a different `flask.Request` object.
+
+The functionality of `commonvars.commonvar()` (or, as you prefer, `commonvars.proxy()`) is a more generic version of `werkzeug.local.LocalProxy`.
+
+It takes a `Manager` object and the class of the object to which the proxy points.
+
+The `Manager` object must have `get` and `set` methods. The `get` method returns
+the object to which the would forward attribute access. The `set` method sets it, obviously.
+`set` is called when the proxy is being inplace modified, for example within the `+=` reassigning operator.
+The class parameter is optional, but it is strongly recommended for some corner-cases.
+The user might provide custom `getter` and `setter` functions that change the way
+`Manager.get()` and `Manage.set()` are called.
+This might be useful when there is the need to keep track of the tokens
+returned by `ContextVar.set()`, if using `ContextVar` as the manager.
+
+## When would you use `commonvars`?
+
+You could use `commonvars` when...
+* ...writing a thread-safe application that operates on resources specific for separate threads.
+* ...improving code readability by avoiding passing around the same object to every function.
+* ...writing a web application that operates on resources specific per request.
+* ...writing an asynchronous application that operates on resources specific between tasks.
+* ...having any other case where you could use common variables that are context-dependent!
+
+## Installation
+
+### pip
+```bash
+$ pip install commonvars
+```
+
+### poetry
+
+You can add `commonvars` as a dependency with the following command:
+
+```bash
+$ poetry add commonvars
+```
+
+Or by directly specifying it in the configuration like so:
+
+```toml
+[tool.poetry.dependencies]
+"commonvars" = "^0.2.0"
+```
+
+Alternatively, you can add it directly from the source:
+
+```toml
+[tool.poetry.dependencies.commonvars]
+git = "https://github.com/bswck/commonvars.git"
+```
+
+## Documentation
+
+### `commonvars.commonvar(mgr, cls=None, getter=None, setter=None)`
+
+Creates a context-dependent proxy object.
+
+#### Parameters
+* `manager`: Manager object. Must implement the `Manager` protocol. Matches `contextvars.ContextVar`.
+* `cls`: The class of the underlying variable accessed within the manager. Optional.
+* `getter`: A function that returns the underlying variable from the manager. Optional.
+* `setter`: A function that sets the underlying variable within the manager. Optional.
+
```

### Comparing `commonvars-0.2.8/PKG-INFO` & `commonvars-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-Metadata-Version: 2.1
-Name: commonvars
-Version: 0.2.8
-Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
-Home-page: https://github.com/bswck/commonvars
-Author: bswck
-Author-email: bswck.dev@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
-## `commonvars`
+## `commonvars v0.3.0`
 
 A simple & straight-forward Python library for creating type-safe, context-dependent proxy objects.
 
 ## Example
 
 The following example shows how to use `commonvars` with `contextvars`:
 
 ```python
 >>> from contextvars import ContextVar
 >>> from commonvars import commonvar
 ...
 >>> count_var = ContextVar("count_var")
->>> count = commonvar(counter, int)
+>>> count = commonvar(count_var, int)
 ...
 >>> count
 <unbound 'int' object>
 >>> count_var.set(0)
 >>> count
 0
 >>> count += 1
@@ -67,15 +54,15 @@
 
 It takes a `Manager` object and the class of the object to which the proxy points.
 
 The `Manager` object must have `get` and `set` methods. The `get` method returns
 the object to which the would forward attribute access. The `set` method sets it, obviously.
 `set` is called when the proxy is being inplace modified, for example within the `+=` reassigning operator.
 The class parameter is optional, but it is strongly recommended for some corner-cases.
-The user might provide custom `getter` and `setter` functions that change the way 
+The user might provide custom `getter` and `setter` functions that change the way
 `Manager.get()` and `Manage.set()` are called.
 This might be useful when there is the need to keep track of the tokens
 returned by `ContextVar.set()`, if using `ContextVar` as the manager.
 
 ## When would you use `commonvars`?
 
 You could use `commonvars` when...
@@ -121,8 +108,7 @@
 Creates a context-dependent proxy object.
 
 #### Parameters
 * `manager`: Manager object. Must implement the `Manager` protocol. Matches `contextvars.ContextVar`.
 * `cls`: The class of the underlying variable accessed within the manager. Optional.
 * `getter`: A function that returns the underlying variable from the manager. Optional.
 * `setter`: A function that sets the underlying variable within the manager. Optional.
-
```

