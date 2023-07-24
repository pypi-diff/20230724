# Comparing `tmp/simpleaichat-0.2.1.tar.gz` & `tmp/simpleaichat-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaichat-0.2.1.tar", last modified: Mon Jul  3 17:55:16 2023, max compression
+gzip compressed data, was "simpleaichat-0.2.2.tar", last modified: Mon Jul 24 00:56:13 2023, max compression
```

## Comparing `simpleaichat-0.2.1.tar` & `simpleaichat-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-03 17:55:16.962859 simpleaichat-0.2.1/
--rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.2.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)    17755 2023-07-03 17:55:16.962521 simpleaichat-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    17318 2023-06-19 02:32:32.000000 simpleaichat-0.2.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-07-03 17:55:16.962959 simpleaichat-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      971 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-03 17:55:16.960523 simpleaichat-0.2.1/simpleaichat/
--rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.2.1/simpleaichat/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    13878 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/simpleaichat/chatgpt.py
--rw-r--r--   0 root         (0) staff       (20)      549 2023-06-08 03:28:41.000000 simpleaichat-0.2.1/simpleaichat/cli.py
--rw-r--r--   0 root         (0) staff       (20)     3098 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/simpleaichat/models.py
--rw-r--r--   0 root         (0) staff       (20)    13550 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/simpleaichat/simpleaichat.py
--rw-r--r--   0 root         (0) staff       (20)     2800 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/simpleaichat/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-03 17:55:16.962075 simpleaichat-0.2.1/simpleaichat.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    17755 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      387 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       67 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)      111 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 00:56:13.389055 simpleaichat-0.2.2/
+-rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)    17756 2023-07-24 00:56:13.388792 simpleaichat-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    17319 2023-07-18 03:38:47.000000 simpleaichat-0.2.2/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-07-24 00:56:13.389132 simpleaichat-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      971 2023-07-24 00:05:58.000000 simpleaichat-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 00:56:13.386546 simpleaichat-0.2.2/simpleaichat/
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.2.2/simpleaichat/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    13975 2023-07-24 00:15:01.000000 simpleaichat-0.2.2/simpleaichat/chatgpt.py
+-rw-r--r--   0 root         (0) staff       (20)      814 2023-07-18 03:38:47.000000 simpleaichat-0.2.2/simpleaichat/cli.py
+-rw-r--r--   0 root         (0) staff       (20)     3098 2023-07-03 17:43:58.000000 simpleaichat-0.2.2/simpleaichat/models.py
+-rw-r--r--   0 root         (0) staff       (20)    13479 2023-07-24 00:13:29.000000 simpleaichat-0.2.2/simpleaichat/simpleaichat.py
+-rw-r--r--   0 root         (0) staff       (20)     2820 2023-07-08 02:15:21.000000 simpleaichat-0.2.2/simpleaichat/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 00:56:13.388349 simpleaichat-0.2.2/simpleaichat.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    17756 2023-07-24 00:56:12.000000 simpleaichat-0.2.2/simpleaichat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      387 2023-07-24 00:56:13.000000 simpleaichat-0.2.2/simpleaichat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-24 00:56:12.000000 simpleaichat-0.2.2/simpleaichat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       67 2023-07-24 00:56:12.000000 simpleaichat-0.2.2/simpleaichat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)      111 2023-07-24 00:56:12.000000 simpleaichat-0.2.2/simpleaichat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2023-07-24 00:56:12.000000 simpleaichat-0.2.2/simpleaichat.egg-info/top_level.txt
```

### Comparing `simpleaichat-0.2.1/LICENSE` & `simpleaichat-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.2.1/PKG-INFO` & `simpleaichat-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleaichat
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
 Home-page: https://github.com/minimaxir/simpleaichat
 Author: Max Woolf
 Author-email: max@minimaxir.com
 License: MIT
 Keywords: chatgpt,openai,text generation,ai
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 
 - Create and run chats with only a few lines of code!
 - Optimized workflows which minimize the amount of tokens used, reducing costs and latency.
 - Run multiple independent chats at once.
 - Minimal codebase: no code dives to figure out what's going on under the hood needed!
 - Chat streaming responses and the ability to use tools.
 - Async support, including for streaming and tools.
-- Ablity to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
+- Ability to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
 - Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
 - Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
 - Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
```

### Comparing `simpleaichat-0.2.1/README.md` & `simpleaichat-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 - Create and run chats with only a few lines of code!
 - Optimized workflows which minimize the amount of tokens used, reducing costs and latency.
 - Run multiple independent chats at once.
 - Minimal codebase: no code dives to figure out what's going on under the hood needed!
 - Chat streaming responses and the ability to use tools.
 - Async support, including for streaming and tools.
-- Ablity to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
+- Ability to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
 - Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
 - Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
 - Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
```

### Comparing `simpleaichat-0.2.1/setup.py` & `simpleaichat-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="simpleaichat",
     packages=["simpleaichat"],  # this must be the same as the name above
-    version="0.2.1",
+    version="0.2.2",
     description="A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Max Woolf",
     author_email="max@minimaxir.com",
     url="https://github.com/minimaxir/simpleaichat",
     keywords=["chatgpt", "openai", "text generation", "ai"],
```

### Comparing `simpleaichat-0.2.1/simpleaichat/chatgpt.py` & `simpleaichat-0.2.2/simpleaichat/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic import HttpUrl, ConfigDict
+from pydantic import HttpUrl
 from httpx import Client, AsyncClient
 from typing import List, Dict, Union, Set, Any
 import orjson
 
 from .models import ChatMessage, ChatSession
 from .utils import remove_a_key
 
@@ -14,15 +14,14 @@
 
 
 class ChatGPTSession(ChatSession):
     api_url: HttpUrl = "https://api.openai.com/v1/chat/completions"
     input_fields: Set[str] = {"role", "content", "name"}
     system: str = "You are a helpful assistant."
     params: Dict[str, Any] = {"temperature": 0.7}
-    model_config: ConfigDict(arbitrary_types_allowed=True)
 
     def prepare_request(
         self,
         prompt: str,
         system: str = None,
         params: Dict[str, Any] = None,
         stream: bool = False,
@@ -71,14 +70,17 @@
                     data["function_call"] = {"name": output_schema.__name__}
             data["functions"] = functions
 
         return headers, data, user_message
 
     def schema_to_function(self, schema: Any):
         assert schema.__doc__, f"{schema.__name__} is missing a docstring."
+        assert (
+            "title" not in schema.__fields__.keys()
+        ), "`title` is a reserved keyword and cannot be used as a field name."
         schema_dict = schema.model_json_schema()
         remove_a_key(schema_dict, "title")
 
         return {
             "name": schema.__name__,
             "description": schema.__doc__,
             "parameters": schema_dict,
@@ -95,15 +97,15 @@
         output_schema: Any = None,
     ):
         headers, data, user_message = self.prepare_request(
             prompt, system, params, False, input_schema, output_schema
         )
 
         r = client.post(
-            self.api_url,
+            str(self.api_url),
             json=data,
             headers=headers,
             timeout=None,
         )
         r = r.json()
 
         try:
@@ -141,15 +143,15 @@
     ):
         headers, data, user_message = self.prepare_request(
             prompt, system, params, True, input_schema
         )
 
         with client.stream(
             "POST",
-            self.api_url,
+            str(self.api_url),
             json=data,
             headers=headers,
             timeout=None,
         ) as r:
             content = []
             for chunk in r.iter_lines():
                 if len(chunk) > 0:
@@ -253,15 +255,15 @@
         output_schema: Any = None,
     ):
         headers, data, user_message = self.prepare_request(
             prompt, system, params, False, input_schema, output_schema
         )
 
         r = await client.post(
-            self.api_url,
+            str(self.api_url),
             json=data,
             headers=headers,
             timeout=None,
         )
         r = r.json()
 
         try:
@@ -299,15 +301,15 @@
     ):
         headers, data, user_message = self.prepare_request(
             prompt, system, params, True, input_schema
         )
 
         async with client.stream(
             "POST",
-            self.api_url,
+            str(self.api_url),
             json=data,
             headers=headers,
             timeout=None,
         ) as r:
             content = []
             async for chunk in r.aiter_lines():
                 if len(chunk) > 0:
```

### Comparing `simpleaichat-0.2.1/simpleaichat/cli.py` & `simpleaichat-0.2.2/simpleaichat/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import fire
 import os
 from getpass import getpass
 from .simpleaichat import AIChat
 from dotenv import load_dotenv
+import argparse
 
 load_dotenv()
 
+parser = argparse.ArgumentParser()
+parser.add_argument("character", help="Specify the character", default=None, nargs='?')
+parser.add_argument("character_command", help="Specify the character command", default=None, nargs='?')
+parser.add_argument("--prime", action="store_true", help="Enable priming")
 
-def interactive_chat(character=None, character_command=None, prime=True):
+ARGS = parser.parse_args()
+
+def interactive_chat():
     gpt_api_key = os.getenv("OPENAI_API_KEY")
     if not gpt_api_key:
         gpt_api_key = getpass("Input your OpenAI key here: ")
     assert gpt_api_key, "An API key was not defined."
-    _ = AIChat(character=character, character_command=character_command, prime=prime)
-    return
-
+    _ = AIChat(ARGS.character, ARGS.character_command, ARGS.prime)
 
 if __name__ == "__main__":
     fire.Fire(interactive_chat)
```

### Comparing `simpleaichat-0.2.1/simpleaichat/models.py` & `simpleaichat-0.2.2/simpleaichat/models.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.2.1/simpleaichat/simpleaichat.py` & `simpleaichat-0.2.2/simpleaichat/simpleaichat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import datetime
 import dateutil
 from uuid import uuid4, UUID
 from contextlib import contextmanager, asynccontextmanager
 import csv
 
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel
 from httpx import Client, AsyncClient
 from typing import List, Dict, Union, Optional, Any
 import orjson
 from dotenv import load_dotenv
 from rich.console import Console
 
 from .utils import wikipedia_search_lookup
@@ -19,15 +19,14 @@
 load_dotenv()
 
 
 class AIChat(BaseModel):
     client: Any
     default_session: Optional[ChatSession]
     sessions: Dict[Union[str, UUID], ChatSession] = {}
-    model_config: ConfigDict(arbitrary_types_allowed=True)
 
     def __init__(
         self,
         character: str = None,
         character_command: str = None,
         system: str = None,
         id: Union[str, UUID] = uuid4(),
```

### Comparing `simpleaichat-0.2.1/simpleaichat/utils.py` & `simpleaichat-0.2.2/simpleaichat/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
 async def wikipedia_search_lookup_async(query: str, sentences: int = 1) -> str:
     return await wikipedia_lookup_async(
         await wikipedia_search_async(query, 1), sentences
     )
 
 
-def fd(description: str):
-    return Field(description=description)
+def fd(description: str, **kwargs):
+    return Field(description=description, **kwargs)
 
 
 # https://stackoverflow.com/a/58938747
 def remove_a_key(d, remove_key):
     if isinstance(d, dict):
         for key in list(d.keys()):
             if key == remove_key:
```

### Comparing `simpleaichat-0.2.1/simpleaichat.egg-info/PKG-INFO` & `simpleaichat-0.2.2/simpleaichat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleaichat
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
 Home-page: https://github.com/minimaxir/simpleaichat
 Author: Max Woolf
 Author-email: max@minimaxir.com
 License: MIT
 Keywords: chatgpt,openai,text generation,ai
 Platform: UNKNOWN
@@ -25,15 +25,15 @@
 
 - Create and run chats with only a few lines of code!
 - Optimized workflows which minimize the amount of tokens used, reducing costs and latency.
 - Run multiple independent chats at once.
 - Minimal codebase: no code dives to figure out what's going on under the hood needed!
 - Chat streaming responses and the ability to use tools.
 - Async support, including for streaming and tools.
-- Ablity to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
+- Ability to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
 - Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
 - Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
 - Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
```

