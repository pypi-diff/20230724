# Comparing `tmp/gearsllm-0.1.5.tar.gz` & `tmp/gearsllm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gearsllm-0.1.5.tar", max compression
+gzip compressed data, was "gearsllm-0.1.6.tar", max compression
```

## Comparing `gearsllm-0.1.5.tar` & `gearsllm-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.5/LICENSE
--rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.5/README.md
--rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.5/gears/__init__.py
--rw-r--r--   0        0        0     2120 2023-07-24 03:01:58.378599 gearsllm-0.1.5/gears/gear.py
--rw-r--r--   0        0        0     2592 2023-07-24 03:07:29.911750 gearsllm-0.1.5/gears/history.py
--rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.5/gears/llms/__init__.py
--rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.5/gears/llms/base.py
--rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.5/gears/llms/echo.py
--rw-r--r--   0        0        0     3779 2023-07-24 03:02:10.728788 gearsllm-0.1.5/gears/llms/oai.py
--rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.5/gears/utils.py
--rw-r--r--   0        0        0      554 2023-07-24 03:08:12.394230 gearsllm-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.6/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.6/README.md
+-rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.6/gears/__init__.py
+-rw-r--r--   0        0        0     2108 2023-07-24 03:27:57.611972 gearsllm-0.1.6/gears/gear.py
+-rw-r--r--   0        0        0     2592 2023-07-24 03:10:17.813919 gearsllm-0.1.6/gears/history.py
+-rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.6/gears/llms/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.6/gears/llms/base.py
+-rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.6/gears/llms/echo.py
+-rw-r--r--   0        0        0     3779 2023-07-24 03:02:10.728788 gearsllm-0.1.6/gears/llms/oai.py
+-rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.6/gears/utils.py
+-rw-r--r--   0        0        0      554 2023-07-24 03:28:25.445179 gearsllm-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.6/PKG-INFO
```

### Comparing `gearsllm-0.1.5/LICENSE` & `gearsllm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.5/gears/gear.py` & `gearsllm-0.1.6/gears/gear.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,28 +24,30 @@
         self,
         data: BaseModel,
         history: History,
         **kwargs,
     ):
         # Construct the template with the pydantic model
         try:
-            prompt = self.template.render(data.model_dump())
+            items = data.model_dump()
         except AttributeError:
-            prompt = self.template.render(data.dict())
+            items = data.dict()
+
+        prompt = self.template.render(items)
 
         # Call the model
         logger.info(f"Running model with prompt: {prompt}")
         response = await self.model.run(prompt, history, **kwargs)
 
         # Transform the data from the response
         try:
             relevant_args = inspect.getfullargspec(self.transform)[0]
             relevant_data_dict = {
                 key: value
-                for key, value in data.model_dump().items()
+                for key, value in items.items()
                 if key in relevant_args
             }
             response = self.transform(response, **relevant_data_dict)
             # Verify that the structured data is a pydantic model
             if not isinstance(response, BaseModel):
                 raise TypeError(
                     "Transform must return a pydantic model instance"
```

### Comparing `gearsllm-0.1.5/gears/history.py` & `gearsllm-0.1.6/gears/history.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.5/gears/llms/echo.py` & `gearsllm-0.1.6/gears/llms/echo.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.5/gears/llms/oai.py` & `gearsllm-0.1.6/gears/llms/oai.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.5/gears/utils.py` & `gearsllm-0.1.6/gears/utils.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.5/pyproject.toml` & `gearsllm-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gearsllm"
-version = "0.1.5"
+version = "0.1.6"
 description = "Lightweight library for building LLM-based control flow."
 authors = ["Shreya Shankar <ss.shankar505@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gears"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gearsllm-0.1.5/PKG-INFO` & `gearsllm-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearsllm
-Version: 0.1.5
+Version: 0.1.6
 Summary: Lightweight library for building LLM-based control flow.
 License: MIT
 Author: Shreya Shankar
 Author-email: ss.shankar505@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

