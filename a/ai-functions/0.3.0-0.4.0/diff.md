# Comparing `tmp/ai_functions-0.3.0.tar.gz` & `tmp/ai_functions-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_functions-0.3.0.tar", max compression
+gzip compressed data, was "ai_functions-0.4.0.tar", max compression
```

## Comparing `ai_functions-0.3.0.tar` & `ai_functions-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       94 2023-07-22 07:26:46.226935 ai_functions-0.3.0/ai_functions/__init__.py
--rw-r--r--   0        0        0     6495 2023-07-22 07:41:30.178292 ai_functions-0.3.0/ai_functions/functions.py
--rw-r--r--   0        0        0      614 2023-07-22 07:41:55.293422 ai_functions-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1520 2023-07-21 17:19:00.362094 ai_functions-0.3.0/README.md
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 ai_functions-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-07-22 07:26:46.226935 ai_functions-0.4.0/ai_functions/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-22 20:26:41.473071 ai_functions-0.4.0/ai_functions/functions.py
+-rw-r--r--   0        0        0      614 2023-07-22 20:27:56.171838 ai_functions-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1520 2023-07-21 17:19:00.362094 ai_functions-0.4.0/README.md
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 ai_functions-0.4.0/PKG-INFO
```

### Comparing `ai_functions-0.3.0/ai_functions/functions.py` & `ai_functions-0.4.0/ai_functions/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,55 +81,59 @@
         self.map.pop(name, None)
 
     def __iter__(self):
         return iter(self.map.values())
 
 def get_openai_args(sig):
     annotated_args: dict[str, dict[str, str]] = {}
+    required: list[str] = []
     for param_index, (param_name, param) in enumerate(sig.parameters.items()):
         if param_name in ("self", "cls") and param_index == 0:
             continue
         if param.kind == param.POSITIONAL_ONLY:
             return None
-        if param.annotation == inspect.Parameter.empty or param.annotation == Any:
-            if param.kind != param.VAR_KEYWORD:
-                return None
+        if param.annotation == inspect.Parameter.empty:
             continue
         if get_origin(param.annotation) is not Annotated:
-            return None
+            continue
         base_type = get_args(param.annotation)[0]
-        param_type = JSON_TYPE_MAP[base_type]
         param_description = param.annotation.__metadata__[0]
         if param_description is None:
             continue
+        if param.default == inspect.Parameter.empty:
+            required.append(param_name) 
+        param_type = JSON_TYPE_MAP[base_type]
         annotated_args[param_name] = {"type": param_type, "description": param_description}
-    return annotated_args
+    return annotated_args, required
 
 
 def get_openai_dict(funcs: Iterable[Callable] = None):
     ret = []
     for func in funcs:
         name = func.__name__
         docs = inspect.getdoc(func)
         sig = inspect.signature(func)
-        args = get_openai_args(sig)
+        args, required = get_openai_args(sig)
 
         if args is None or docs is None:
             raise ValueError(f"Invalid function {name}, must have annotated docs and arguments")
 
-        ret.append(dict(
+        d = dict(
             name=name,
             description=docs,
             parameters=dict(
                 type="object",
                 properties=dict(
                     **args
                 ),
             )
-        ))
+        )
+        if required:
+            d["required"] = required
+        ret.append(d)
 
     return ret
 
 
 def execute_function(funcs: Iterable[Callable], name: str, arguments: Union[str, dict], *, loop=None,
                      convert_output=convert_response, **kws):
     args, func = prepare_function(arguments, funcs, name)
```

### Comparing `ai_functions-0.3.0/pyproject.toml` & `ai_functions-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-functions"
-version = "0.3.0"
+version = "0.4.0"
 description = "manage openai functions and execution"
 authors = ["erik aronesty <erik@q32.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ai_functions"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ai_functions-0.3.0/README.md` & `ai_functions-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_functions-0.3.0/PKG-INFO` & `ai_functions-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-functions
-Version: 0.3.0
+Version: 0.4.0
 Summary: manage openai functions and execution
 License: MIT
 Author: erik aronesty
 Author-email: erik@q32.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

