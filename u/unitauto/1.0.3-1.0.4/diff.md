# Comparing `tmp/unitauto-1.0.3.tar.gz` & `tmp/unitauto-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-mpwep_3f/unitauto-1.0.3.tar", last modified: Sun Jul 23 16:38:12 2023, max compression
+gzip compressed data, was "/home/runner/work/unitauto-py/unitauto-py/dist/.tmp-gi87mh_o/unitauto-1.0.4.tar", last modified: Mon Jul 24 16:53:30 2023, max compression
```

## Comparing `unitauto-1.0.3.tar` & `unitauto-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:38:12.000000 unitauto-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-23 16:37:56.000000 unitauto-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-23 16:38:12.000000 unitauto-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-23 16:37:56.000000 unitauto-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-23 16:37:56.000000 unitauto-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-23 16:38:12.000000 unitauto-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:38:12.000000 unitauto-1.0.3/unitauto/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-23 16:37:56.000000 unitauto-1.0.3/unitauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33695 2023-07-23 16:37:56.000000 unitauto-1.0.3/unitauto/methodutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-23 16:37:56.000000 unitauto-1.0.3/unitauto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:38:12.000000 unitauto-1.0.3/unitauto/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-23 16:37:56.000000 unitauto-1.0.3/unitauto/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-23 16:37:56.000000 unitauto-1.0.3/unitauto/test/testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:38:12.000000 unitauto-1.0.3/unitauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-23 16:38:12.000000 unitauto-1.0.3/unitauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-23 16:38:12.000000 unitauto-1.0.3/unitauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 16:38:12.000000 unitauto-1.0.3/unitauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 16:38:12.000000 unitauto-1.0.3/unitauto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:30.000000 unitauto-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 16:53:11.000000 unitauto-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-24 16:53:30.000000 unitauto-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-24 16:53:11.000000 unitauto-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 16:53:11.000000 unitauto-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-24 16:53:30.000000 unitauto-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:30.000000 unitauto-1.0.4/unitauto/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 16:53:11.000000 unitauto-1.0.4/unitauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35358 2023-07-24 16:53:11.000000 unitauto-1.0.4/unitauto/methodutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-24 16:53:11.000000 unitauto-1.0.4/unitauto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:30.000000 unitauto-1.0.4/unitauto/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-24 16:53:11.000000 unitauto-1.0.4/unitauto/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-24 16:53:11.000000 unitauto-1.0.4/unitauto/test/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:30.000000 unitauto-1.0.4/unitauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-24 16:53:30.000000 unitauto-1.0.4/unitauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 16:53:30.000000 unitauto-1.0.4/unitauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:53:30.000000 unitauto-1.0.4/unitauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 16:53:30.000000 unitauto-1.0.4/unitauto.egg-info/top_level.txt
```

### Comparing `unitauto-1.0.3/LICENSE` & `unitauto-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.3/PKG-INFO` & `unitauto-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 1.0.3
+Version: 1.0.4
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unitauto-1.0.3/README.md` & `unitauto-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.3/setup.cfg` & `unitauto-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unitauto
-version = 1.0.3
+version = 1.0.4
 author = TommyLemon
 author_email = tommylemon@qq.com
 description = An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TommyLemon/unitauto-py
 classifiers =
```

### Comparing `unitauto-1.0.3/unitauto/methodutil.py` & `unitauto-1.0.4/unitauto/methodutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import asyncio
 import builtins
 import json
 import os
 import re
 import time
 import inspect
+import types
+import typing
 from typing import Type
 
 null = None
 false = False
 true = True
 
 KEY_OK = 'ok'
@@ -65,14 +67,15 @@
 KEY_MOCK = "mock"
 KEY_QUERY = "query"
 KEY_DEPTH = "depth"
 KEY_RETURN = "return"
 KEY_TIME_DETAIL = "time:start|duration|end"
 KEY_CLASS_ARGS = "classArgs"
 KEY_METHOD_ARGS = "methodArgs"
+KEY_ARGS = "args"
 KEY_CALLBACK = "callback"
 KEY_GLOBAL = "global"
 
 KEY_CALL_LIST = "call()[]"
 KEY_CALL_MAP = "call(){}"
 KEY_PACKAGE_TOTAL = "packageTotal"
 KEY_CLASS_TOTAL = "classTotal"
@@ -237,65 +240,80 @@
         fl = split(clazz, '$')
 
         module_list = []
         import_fun = import_fun or __import__
 
         depth = depth or 0
         d = 0
-        for root, dirs, files in os.walk(package):
+        for root, dirs, files in os.walk(package.replace('.', '/')):
             d += 1
             if depth > 0 and d > depth:
                 break
 
+            # for name in dirs:
+            #     m = import_fun(('' if is_empty(root) else root.replace('/', '.') + '.') + name.replace('/', '.'), fromlist=['__init__'])
+            #     if not_none(m) and not module_list.__contains__(m):
+            #         module_list.append(m)
+
             for name in files:
                 if size(name) <= 3 or not name.endswith('.py'):
                     continue
 
                 name = name[:-3]
                 p = os.path.join(root, name).replace('/', '.')
                 m = import_fun(p, fromlist=name)
-                if is_none(m) or module_list.__contains__(m):
+                if is_none(m) or module_list.__contains__(m) or m in module_list:
                     continue
 
                 module_list.append(m)
 
         if is_empty(module_list):
             try:
                 mn = package if is_empty(fl) else package + '.' + fl[0]
                 root_module = import_fun(mn, fromlist=['__init__'] if is_empty(fl) else fl[0])
 
                 module_list.append(root_module)
                 mdl_dict = root_module.__dict__
                 vs = mdl_dict.values()
                 for v in vs:
-                    if type(v).__name__ == 'module' and str(v).endswith("/__init__.py'>"):  # if isinstance(v, module):
+                    if type(v).__name__ == 'module' and str(v).endswith("/__init__.py'>"):  # if is_instance(v, module):
                         module_list.append(v)
                         pass
 
             except Exception as e:
                 print(e)
 
         pkg_list = []
 
         for module_item in module_list:
             cl = []
             pkg = module_item.__name__
             pkg_str = str(module_item)
             is_file = pkg_str.endswith(".py'>") and not pkg_str.endswith("/__init__.py'>")
+            file_name = null
+
             if is_file:
-                ns = split(pkg, '.')  # 不存在这个函数 ind = lastindex(pkg, '.')
+                ns = split(pkg, '.')  # 不存在这个函数 ind = last_index(pkg, '.')
+                file_name = ns[-1]
                 pkg = pkg[:-1-len(ns[-1])]
+                # module_item = import_fun(pkg)
+                # if module_item not in cl and not cl.__contains__(module_item):
+                cl.append(module_item)
+
+            if pkg.endswith('.__init__'):
+                pkg = pkg[:-len('.__init__')]
 
             if is_empty(pkg):
                 continue
 
             mdl_list = dir(module_item)
             l = size(mdl_list)
 
             cls_list = []
+
             if l > 1 and not is_all_cls:
                 try:
                     cls = module_item
                     i = -1
                     for n in fl:
                         i += 1
                         if i <= 0:
@@ -307,31 +325,39 @@
             else:
                 for mdl in mdl_list:
                     pn = str(mdl)
                     if is_empty(pn) or pn.startswith('_') or pn.endswith('_'):
                         continue
                     try:
                         cls = getattr(module_item, pn)
+                        cm = cls.__module__ if hasattr(cls, '__module__') else null
+                        if is_empty(cm) or not cm.startswith(pkg):
+                            continue
 
                         ct = type(cls).__name__
                         s = str(cls)
                         if ct == 'function':
+                            if is_file:
+                                continue
+
                             mtd = parse_method(cls) if is_all_mtd or cls.__name__ == method else null
                             if is_empty(mtd):
                                 continue
 
                             cls_list.append({
-                                # KEY_CLASS: cls.__name__,
+                                KEY_CLASS: file_name,
                                 KEY_METHOD_LIST: [mtd]
                             })
                         if ct == 'class' or ct == 'type':
-                            cl.append(cls)
+                            if cls not in cl and not cl.__contains__(cls):
+                                cl.append(cls)
                         elif ct == 'module':
                             if is_file or (s.endswith(".py'>") and not s.endswith("/__init__.py'>")):
-                                cl.append(cls)
+                                if cls not in cl and not cl.__contains__(cls):
+                                    cl.append(cls)
                             # elif not (cls in module_list):
                             #     module_list.append(cls)
                     except Exception as e:
                         print(e)
 
             for cls in cl:
                 cn = cls.__name__
@@ -375,16 +401,16 @@
 
                                 try:
                                     func = getattr(cls, n)
                                     if callable(func):
                                         ft = type(func).__name__
                                         if ft == 'function':
                                             ml.append(func)
-                                        elif ft in ('type', 'class') and str(func) == ("<class '" + cn + "." + func.__name__ + "'>"):
-                                            cl.append(func)
+                                        # elif ft in ('type', 'class') and str(func) == ("<class '" + cn + "." + func.__name__ + "'>"):
+                                        #     cl.append(func)
                                 except Exception as e:
                                     print(e)
                         # cls.__class__.methods
 
                     mtd_list = []
                     for mtd in ml:
                         m = parse_method(mtd)
@@ -606,17 +632,22 @@
         method = req.get(KEY_METHOD)
         assert is_str(method), (KEY_METHOD + ' must be str!')
         assert not_empty(method), (KEY_CLASS + ' method be empty!')
 
         class_args = req.get(KEY_CLASS_ARGS)
         assert is_list(class_args), (KEY_CLASS_ARGS + ' must be list!')
 
+        args = req.get(KEY_ARGS)
+        assert is_list(args), (KEY_ARGS + ' must be list!')
+
         method_args = req.get(KEY_METHOD_ARGS)
         assert is_list(method_args), (KEY_METHOD_ARGS + ' must be list!')
 
+        assert args is None or method_args is None, (KEY_ARGS + ', ' + KEY_METHOD_ARGS + ' cannot both be not null!')
+
         constructor = req.get(KEY_CONSTRUCTOR)
         assert is_str(constructor), (KEY_CONSTRUCTOR + ' must be str!')
 
         this = req.get(KEY_THIS)
         assert is_dict(this), (KEY_THIS + ' must be dict!')
 
         instance = None
@@ -632,14 +663,15 @@
             init_args([this], this_keys, this_types, this_values, this_kwargs, import_fun=import_fun)
             instance = this_values[0]
 
         if class_args is not None:
             assert not static, KEY_CLASS_ARGS + ' cannot appear together with ' + KEY_STATIC + '!'
             assert this is None, KEY_CLASS_ARGS + ' cannot appear together with ' + KEY_THIS + '!'
 
+        method_args = method_args or args
         mal = size(method_args)
         ma_keys = [null] * mal
         ma_types = [null] * mal
         ma_values = [null] * mal
         m_kwargs = {}
 
         final_result = {}
@@ -678,17 +710,20 @@
 
             func = getattr(instance, method)
 
         final_result[KEY_THIS] = instance
         ksl = size(m_kwargs)
         start_time = cur_time_in_millis()
 
-        # TODO 自动识别 async 关键词
-        result = asyncio.run(func(*ma_values[:mal-ksl], **m_kwargs)) if is_async \
-            else func(*ma_values[:mal-ksl], **m_kwargs)  # asyncio.run 只允许调 async 函数 is_async != false
+        result = func(*ma_values[:mal - ksl], **m_kwargs)  # asyncio.run 只允许调 async 函数 is_async != false
+
+        # 自动识别 async 关键词
+        is_async = is_async or (is_async is None and is_instance(result, (types.CoroutineType, types.AsyncGeneratorType)))
+        if is_async:
+            result = asyncio.run(result)
 
         final_result[KEY_VALUE] = result
         res = wrap_result(
             instance, func, method_args, ma_types, ma_values, result, start_time,
             json_dumps=json_dumps, json_loads=json_loads
         )
     except Exception as e:
@@ -846,15 +881,15 @@
                 del ma_types[-1]
                 del ma_values[-1]
 
     return is_wait
 
 
 def cast(value, clazz, json_dumps: callable = null, json_loads: callable = null):
-    if value is not None and not isinstance(value, clazz):
+    if value is not None and not is_instance(value, clazz):
         json_dumps = json_dumps or json.dumps
         json_loads = json_loads or json.loads
 
         s = ''
         try:
             s = value if is_str(value) else json_dumps(value)
             if PRIMITIVE_CLASS_MAP.__contains__(clazz.__name__):
@@ -862,15 +897,15 @@
             else:
                 value = json_loads(s, cls=clazz)  # FIXME 目前仅支持继承 JSONDecoder 且重写了 decode 方法的类
         except Exception as e:
             print(e)
             if is_str(value):
                 value = json_loads(value)
 
-            if not isinstance(value, clazz):
+            if not is_instance(value, clazz):
                 if is_list(value):
                     value = clazz(*value)
                 elif is_dict(value):
                     value = clazz(**value)  # FIXME 目前仅支持继承 __init__ 传完整参数且顺序一致的类
                 else:
                     pass
 
@@ -922,35 +957,35 @@
 
 
 def is_contain(s: str, seperator: str = ',') -> bool:
     return false if is_empty(s) else seperator in s  # s.__contains__(seperator)
 
 
 def is_bool(obj, strict: bool = false) -> bool:
-    return (not strict) if obj is None else isinstance(obj, bool)
+    return (not strict) if obj is None else is_instance(obj, bool)
 
 
 def is_int(obj, strict: bool = false) -> bool:
-    return (not strict) if obj is None else isinstance(obj, int)
+    return (not strict) if obj is None else is_instance(obj, int)
 
 
 def is_float(obj, strict: bool = false) -> bool:
-    return (not strict) if obj is None else isinstance(obj, float)
+    return (not strict) if obj is None else is_instance(obj, float)
 
 
 def is_str(obj, strict: bool = false) -> bool:
-    return (not strict) if obj is None else isinstance(obj, str)
+    return (not strict) if obj is None else is_instance(obj, str)
 
 
 def is_list(obj, strict: bool = false) -> bool:
-    return (not strict) if obj is None else isinstance(obj, list)
+    return (not strict) if obj is None else is_instance(obj, list)
 
 
 def is_dict(obj, strict: bool = false) -> bool:
-    return (not strict) if obj is None else isinstance(obj, dict)
+    return (not strict) if obj is None else is_instance(obj, dict)
 
 
 def not_none(obj):
     return not is_none(obj)
 
 
 def is_none(obj):
@@ -966,17 +1001,24 @@
         return true
     if is_int(obj) or is_float(obj):
         return obj <= 0
 
     return size(obj) <= 0
 
 
+def is_instance(obj, typ):
+    if typ in [null, any, typing.Any]:  # fix isinstance() arg 2 must be a type or tuple of types
+        return true
+    return isinstance(obj, typ)
+
+
 def is_name(s: str) -> bool:
-    m = null if is_empty(s) else PATTERN_NUMBER.match(s[:1])
-    return is_none(m) and not_none(PATTERN_NAME.match(s))
+    if is_empty(s) or PATTERN_NUMBER.match(s[:1]):
+        return false
+    return not_none(PATTERN_NAME.match(s))
 
 
 def size(obj) -> int:
     if obj is None:
         return 0
 
     if is_bool(obj) or is_int(obj) or is_float(obj):
```

### Comparing `unitauto-1.0.3/unitauto/server.py` & `unitauto-1.0.4/unitauto/server.py`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.3/unitauto/test/__init__.py` & `unitauto-1.0.4/unitauto/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.3/unitauto/test/testutil.py` & `unitauto-1.0.4/unitauto/test/testutil.py`

 * *Files identical despite different names*

### Comparing `unitauto-1.0.3/unitauto.egg-info/PKG-INFO` & `unitauto-1.0.4/unitauto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 1.0.3
+Version: 1.0.4
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

