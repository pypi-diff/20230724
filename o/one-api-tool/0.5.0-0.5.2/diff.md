# Comparing `tmp/one-api-tool-0.5.0.tar.gz` & `tmp/one-api-tool-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.5.0.tar", last modified: Sat Jul 22 03:39:47 2023, max compression
+gzip compressed data, was "one-api-tool-0.5.2.tar", last modified: Mon Jul 24 03:53:58 2023, max compression
```

## Comparing `one-api-tool-0.5.0.tar` & `one-api-tool-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 03:39:47.842936 one-api-tool-0.5.0/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.5.0/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     7677 2023-07-22 03:39:47.842673 one-api-tool-0.5.0/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     7121 2023-07-21 08:10:20.000000 one-api-tool-0.5.0/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 03:39:47.840779 one-api-tool-0.5.0/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     7677 2023-07-22 03:39:47.000000 one-api-tool-0.5.0/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-07-22 03:39:47.000000 one-api-tool-0.5.0/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-22 03:39:47.000000 one-api-tool-0.5.0/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-22 03:39:47.000000 one-api-tool-0.5.0/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-22 03:39:47.000000 one-api-tool-0.5.0/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-22 03:39:47.000000 one-api-tool-0.5.0/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 03:39:47.841890 one-api-tool-0.5.0/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.5.0/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 03:39:47.842147 one-api-tool-0.5.0/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.5.0/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-07-22 02:56:10.000000 one-api-tool-0.5.0/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    21933 2023-07-22 03:36:52.000000 one-api-tool-0.5.0/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-07-22 02:58:15.000000 one-api-tool-0.5.0/oneapi/one_api_test.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.5.0/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-22 03:39:47.842989 one-api-tool-0.5.0/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-22 03:39:18.000000 one-api-tool-0.5.0/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:53:58.574556 one-api-tool-0.5.2/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.5.2/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8209 2023-07-24 03:53:58.574046 one-api-tool-0.5.2/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7653 2023-07-24 03:51:04.000000 one-api-tool-0.5.2/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:53:58.571337 one-api-tool-0.5.2/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8209 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       91 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-24 03:53:58.000000 one-api-tool-0.5.2/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:53:58.572987 one-api-tool-0.5.2/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.5.2/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-24 03:53:58.573512 one-api-tool-0.5.2/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.5.2/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-07-22 02:56:10.000000 one-api-tool-0.5.2/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    23648 2023-07-24 03:42:18.000000 one-api-tool-0.5.2/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1106 2023-07-24 03:49:05.000000 one-api-tool-0.5.2/oneapi/one_api_test.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.5.2/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-24 03:53:58.574629 one-api-tool-0.5.2/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1094 2023-07-24 03:51:47.000000 one-api-tool-0.5.2/setup.py
```

### Comparing `one-api-tool-0.5.0/LICENSE` & `one-api-tool-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.0/PKG-INFO` & `one-api-tool-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.5.0
+Version: 0.5.2
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -87,14 +87,28 @@
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
+### Batch request with asyncio
+```python
+from oneapi.one_api import batch_chat
+
+claude_config = 'anthropic_config.json'
+openai_config = 'openapi_config.json'
+azure_config = 'openapi_azure_config.json'
+# The coccurent number of requests would be 3, which is the same as the length of the configs list.
+configs = [claude_config, openai_config, azure_config]
+prompts = ['How\'s the weather today?', 'How\'s the weather today?', 'How\'s the weather today?']
+res = asyncio.run(batch_chat(configs, prompts, stream=False))
+print(res)
+
+```
 #### Simple function calling example:
 
 ```python
 from oneapi import OneAPITool
 
 def get_whether_of_city(city: str, date: str) -> dict:
     """Get the weather of a city at a date
@@ -221,12 +235,12 @@
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 0.9 will make the output more random, while lower values like 0.1 will make it more focused and deterministic. 
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
-- [ ] Batch requests.
+- [x] Batch requests.
 - [x] OpenAI function_call.
 - [x] Token number counting.
 - [x] Async requests.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.5.0/README.md` & `one-api-tool-0.5.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,28 @@
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
+### Batch request with asyncio
+```python
+from oneapi.one_api import batch_chat
+
+claude_config = 'anthropic_config.json'
+openai_config = 'openapi_config.json'
+azure_config = 'openapi_azure_config.json'
+# The coccurent number of requests would be 3, which is the same as the length of the configs list.
+configs = [claude_config, openai_config, azure_config]
+prompts = ['How\'s the weather today?', 'How\'s the weather today?', 'How\'s the weather today?']
+res = asyncio.run(batch_chat(configs, prompts, stream=False))
+print(res)
+
+```
 #### Simple function calling example:
 
 ```python
 from oneapi import OneAPITool
 
 def get_whether_of_city(city: str, date: str) -> dict:
     """Get the weather of a city at a date
@@ -209,12 +223,12 @@
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 0.9 will make the output more random, while lower values like 0.1 will make it more focused and deterministic. 
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
-- [ ] Batch requests.
+- [x] Batch requests.
 - [x] OpenAI function_call.
 - [x] Token number counting.
 - [x] Async requests.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.5.0/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.5.2/one_api_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.5.0
+Version: 0.5.2
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -87,14 +87,28 @@
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
 **Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
+### Batch request with asyncio
+```python
+from oneapi.one_api import batch_chat
+
+claude_config = 'anthropic_config.json'
+openai_config = 'openapi_config.json'
+azure_config = 'openapi_azure_config.json'
+# The coccurent number of requests would be 3, which is the same as the length of the configs list.
+configs = [claude_config, openai_config, azure_config]
+prompts = ['How\'s the weather today?', 'How\'s the weather today?', 'How\'s the weather today?']
+res = asyncio.run(batch_chat(configs, prompts, stream=False))
+print(res)
+
+```
 #### Simple function calling example:
 
 ```python
 from oneapi import OneAPITool
 
 def get_whether_of_city(city: str, date: str) -> dict:
     """Get the weather of a city at a date
@@ -221,12 +235,12 @@
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 0.9 will make the output more random, while lower values like 0.1 will make it more focused and deterministic. 
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
-- [ ] Batch requests.
+- [x] Batch requests.
 - [x] OpenAI function_call.
 - [x] Token number counting.
 - [x] Async requests.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.5.0/oneapi/commands/one_api_requst.py` & `one-api-tool-0.5.2/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.0/oneapi/one_api.py` & `one-api-tool-0.5.2/oneapi/one_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from pydantic import BaseModel
 from abc import ABC, abstractmethod
 import sys
 import os
 from typing import Callable, Optional, Sequence, List
 import tiktoken
 import logging
+import asyncio
+import aiohttp
 from openai.openai_object import OpenAIObject
+import time
+from tqdm import tqdm
 sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
 from oneapi.utils import generate_function_description
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(filename)s:%(lineno)d %(levelname)s] %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
@@ -248,25 +252,25 @@
         if args.stream:
             resp = await self.client.acompletion_stream(**args.dict())
             async for data in resp:
                 if data["stop_reason"] == "stop_sequence" or data["stop_reason"] == "max_tokens":
                     return data["completion"]
         else:
             resp = await self.client.acompletion(**args.dict())
-            return resp
+            return resp["completion"]
         
     def simple_chat(self, args: ClaudeDecodingArguments):
         if args.stream:
             resp = self.client.completion_stream(**args.dict())
             for  data in resp:
                 if data["stop_reason"] == "stop_sequence" or data["stop_reason"] == "max_tokens":
                     return data["completion"]
         else:
             resp = self.client.completion(**args.dict())
-            return resp
+            return resp["completion"]
 
             
             
 
 class OneAPITool():
     def __init__(self, tool: AbstractAPITool) -> None:
         self.tool = tool
@@ -323,15 +327,15 @@
                     functions = [generate_function_description(func) for func in functions]
                 if function_call is None and functions is not None:
                     function_call = "auto"
                 if function_call is not None and functions is None:
                     function_call = None
                 args = OpenAIDecodingArguments(messages=msgs, functions=functions, function_call=function_call, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
-            args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-v1.3-100k", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
+            args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-2", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
         return response
 
     async def asimple_chat(self, prompt: str|list|dict, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=False, **kwargs):
@@ -413,18 +417,14 @@
             msgs.append({"role": "function", "name": function_name, "content": json.dumps(api_response)})
             final_response = self.simple_chat(msgs, model=model, temperature=temperature, max_new_tokens=max_new_tokens, stream=stream, **kwargs)
             logger.debug(f"Function calling step3, Model summarize, final_response: {final_response}")
             return final_response
         else:
             raise AssertionError(f"Function chat currently only support api type: {type(self.tool)}")
 
-        
-
-
-
     def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
         if isinstance(self.tool, OpenAITool):
             return self.tool.get_embeddings(texts, engine)  
         else:
             raise AssertionError(f"Not supported api type for embeddings: {type(self.tool)}")
 
     def get_embedding(self, text: str, engine="text-embedding-ada-002") -> List[float]:
@@ -435,8 +435,41 @@
     
     def count_tokens(self, texts: List[str], encoding_name: str = 'cl100k_base') -> int:
         if isinstance(self.tool, OpenAITool):
             return self.tool.count_tokens(texts, encoding_name)
         elif isinstance(self.tool, ClaudeAITool):
             return sum([anthropic.count_tokens(text) for text in texts])
         else:
-            raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
+            raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
+
+
+async def bound_fetch(sem, pbar, tool: OneAPITool, prompt: str, model: str, **kwargs):
+    async with sem:
+        try:
+            res = await tool.asimple_chat(prompt=prompt, model=model, **kwargs)
+            pbar.update(1)
+            return res
+        except Exception as e:
+            logger.error(f"Error when calling {model} api: {e}")
+            return None
+
+async def batch_chat(api_config_files, texts, engines=None, request_interval=1, **kwargs):
+    process_num = len(api_config_files)
+    engines = engines if engines is not None else [''] * process_num
+    if engines is not None and len(engines) == 1:
+        engines = engines * process_num
+    if engines is not None and len(engines) > 1:
+        assert len(engines) == process_num, f'Number of engines must be equal to number of api config files when specific multiple engines, but got {len(engines)} engines and {process_num} api config files.'
+
+    sem = asyncio.Semaphore(process_num)
+    pbar = tqdm(total=len(texts))
+    tools = [OneAPITool.from_config_file(config_file) for config_file in api_config_files]
+    tasks = [asyncio.ensure_future(bound_fetch(sem, pbar, tools[i%process_num], prompt=prompt, model=engines[i%process_num], **kwargs))for i, prompt in enumerate(texts)]
+    task_batches = [tasks[i:i+process_num] for i in range(0, len(tasks), process_num)]
+    results = []
+    async with aiohttp.ClientSession() as session:
+        openai.aiosession.set(session)
+        for batch in task_batches:
+            batch_result = await asyncio.gather(*batch)
+            results.extend(batch_result)
+            time.sleep(request_interval)
+    return results
```

### Comparing `one-api-tool-0.5.0/oneapi/one_api_test.py` & `one-api-tool-0.5.2/oneapi/one_api_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 import os
 from typing import Callable, Optional, Sequence, List
 import tiktoken
 import asyncio
 import logging
 from openai.openai_object import OpenAIObject
 sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
-from oneapi.one_api import *
+from oneapi.one_api import batch_chat
 
 
 if __name__ == "__main__":
     claude_config = '../../ant/config/anthropic_config_personal.json'
     openai_config = '../../ant/config/openapi_official_chenghao.json'
     azure_config = '../../ant/config/openapi_azure_config_xiaoduo_dev.json'
     config_file = openai_config
-    tool = OneAPITool.from_config_file(config_file)
-    prompt = '今天天气不错？'
-    
-    res = asyncio.run(tool.asimple_chat(prompt, stream=False))
+    # tool = OneAPITool.from_config_file(config_file)
+    # prompt = '今天天气不错？'
+    # res = asyncio.run(tool.asimple_chat(prompt, stream=False))
+    # print(res)
+    res = asyncio.run(batch_chat([claude_config, openai_config, azure_config], ['今天天气不错？', '今天天气不错？', '今天天气不错？'], stream=False))
     print(res)
```

### Comparing `one-api-tool-0.5.0/oneapi/utils.py` & `one-api-tool-0.5.2/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.0/setup.py` & `one-api-tool-0.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.5.0",
+    version="0.5.2",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
         "httpx",
         "aiohttp",
         "tiktoken",
+        "tqdm",
         "tokenizers",
         "docstring_parser"
     ],
     entry_points={
         "console_scripts": [
             "one-api=oneapi.commands.one_api_requst:main"
         ]
```

