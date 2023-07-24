# Comparing `tmp/gearsllm-0.1.3.tar.gz` & `tmp/gearsllm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gearsllm-0.1.3.tar", max compression
+gzip compressed data, was "gearsllm-0.1.4.tar", max compression
```

## Comparing `gearsllm-0.1.3.tar` & `gearsllm-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.3/LICENSE
--rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.3/README.md
--rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.3/gears/__init__.py
--rw-r--r--   0        0        0     1978 2023-07-23 22:17:21.560333 gearsllm-0.1.3/gears/gear.py
--rw-r--r--   0        0        0     2635 2023-07-23 22:27:24.108862 gearsllm-0.1.3/gears/history.py
--rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.3/gears/llms/__init__.py
--rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.3/gears/llms/base.py
--rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.3/gears/llms/echo.py
--rw-r--r--   0        0        0     3680 2023-07-23 22:17:24.315177 gearsllm-0.1.3/gears/llms/oai.py
--rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.3/gears/utils.py
--rw-r--r--   0        0        0      537 2023-07-23 23:05:11.298595 gearsllm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.4/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.4/README.md
+-rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.4/gears/__init__.py
+-rw-r--r--   0        0        0     2120 2023-07-24 03:01:58.378599 gearsllm-0.1.4/gears/gear.py
+-rw-r--r--   0        0        0     2635 2023-07-24 00:59:40.750920 gearsllm-0.1.4/gears/history.py
+-rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.4/gears/llms/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.4/gears/llms/base.py
+-rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.4/gears/llms/echo.py
+-rw-r--r--   0        0        0     3779 2023-07-24 03:02:10.728788 gearsllm-0.1.4/gears/llms/oai.py
+-rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.4/gears/utils.py
+-rw-r--r--   0        0        0      554 2023-07-24 03:02:32.465474 gearsllm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.4/PKG-INFO
```

### Comparing `gearsllm-0.1.3/LICENSE` & `gearsllm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.3/gears/gear.py` & `gearsllm-0.1.4/gears/gear.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,25 @@
     def __init__(
         self,
         model: BaseLLM,
     ):
         self.model = model
         self.template = Template(self.template())
 
-    async def run(self, data: BaseModel, history: History, **kwargs):
+    async def run(
+        self,
+        data: BaseModel,
+        history: History,
+        **kwargs,
+    ):
         # Construct the template with the pydantic model
-        prompt = self.template.render(data.model_dump())
+        try:
+            prompt = self.template.render(data.model_dump())
+        except AttributeError:
+            prompt = self.template.render(data.dict())
 
         # Call the model
         logger.info(f"Running model with prompt: {prompt}")
         response = await self.model.run(prompt, history, **kwargs)
 
         # Transform the data from the response
         try:
```

### Comparing `gearsllm-0.1.3/gears/history.py` & `gearsllm-0.1.4/gears/history.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.3/gears/llms/echo.py` & `gearsllm-0.1.4/gears/llms/echo.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.3/gears/llms/oai.py` & `gearsllm-0.1.4/gears/llms/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,18 @@
         prompt: str,
         history: History,
         message_kwargs: dict = {},
     ) -> Any:
         # Construct chat history
         curr_message = Message(role="user", content=prompt, **message_kwargs)
         history.add(curr_message)
-        messages = [m.model_dump() for m in history]
+        try:
+            messages = [m.model_dump() for m in history]
+        except AttributeError:
+            messages = [m.dict() for m in history]
         request = {
             "model": self.model,
             "messages": messages,
             **self.api_kwargs,
         }
         response = await self.chat_api_call(request)
         returned_message = response["choices"][0]["message"]["content"]
```

### Comparing `gearsllm-0.1.3/gears/utils.py` & `gearsllm-0.1.4/gears/utils.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.3/pyproject.toml` & `gearsllm-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gearsllm"
-version = "0.1.3"
+version = "0.1.4"
 description = "Lightweight library for building LLM-based control flow."
 authors = ["Shreya Shankar <ss.shankar505@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gears"}]
 
 [tool.poetry.dependencies]
@@ -14,11 +14,12 @@
 openai = "^0.27.8"
 tenacity = "^8.2.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
+rich = "^13.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gearsllm-0.1.3/PKG-INFO` & `gearsllm-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearsllm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lightweight library for building LLM-based control flow.
 License: MIT
 Author: Shreya Shankar
 Author-email: ss.shankar505@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

