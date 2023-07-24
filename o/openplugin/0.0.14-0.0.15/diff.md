# Comparing `tmp/openplugin-0.0.14.tar.gz` & `tmp/openplugin-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-0.0.14.tar", max compression
+gzip compressed data, was "openplugin-0.0.15.tar", max compression
```

## Comparing `openplugin-0.0.14.tar` & `openplugin-0.0.15.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     8321 2023-06-05 16:45:25.990949 openplugin-0.0.14/README.md
--rw-r--r--   0        0        0      755 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/__init__.py
--rw-r--r--   0        0        0       49 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/__main__.py
--rw-r--r--   0        0        0      855 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/api/__init__.py
--rw-r--r--   0        0        0      855 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/api/auth.py
--rw-r--r--   0        0        0      277 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/api/http_error.py
--rw-r--r--   0        0        0     1010 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/api/imprompt.py
--rw-r--r--   0        0        0     1013 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/api/langchain.py
--rw-r--r--   0        0        0     8098 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/bindings/imprompt/imprompt_plugin_selector.py
--rw-r--r--   0        0        0     5330 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/bindings/langchain/langchain_plugin_selector.py
--rw-r--r--   0        0        0     7329 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/interfaces/plugin_selector.py
--rw-r--r--   0        0        0      906 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/main.py
--rw-r--r--   0        0        0     1230 2023-06-05 16:45:25.998949 openplugin-0.0.14/openplugin/utils/run_plugin_selector.py
--rw-r--r--   0        0        0      522 2023-06-05 16:45:25.998949 openplugin-0.0.14/pyproject.toml
--rw-r--r--   0        0        0     9046 1970-01-01 00:00:00.000000 openplugin-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-07-22 20:21:23.014758 openplugin-0.0.15/README.md
+-rw-r--r--   0        0        0      936 2023-07-19 18:30:45.938182 openplugin-0.0.15/openplugin/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-06 13:54:56.177098 openplugin-0.0.15/openplugin/__main__.py
+-rw-r--r--   0        0        0     1254 2023-07-18 17:26:28.236218 openplugin-0.0.15/openplugin/api/__init__.py
+-rw-r--r--   0        0        0      855 2023-06-06 13:54:56.177760 openplugin-0.0.15/openplugin/api/auth.py
+-rw-r--r--   0        0        0     1624 2023-07-18 17:31:07.672783 openplugin-0.0.15/openplugin/api/genric_selector.py
+-rw-r--r--   0        0        0      277 2023-06-01 21:26:45.277312 openplugin-0.0.15/openplugin/api/http_error.py
+-rw-r--r--   0        0        0     1015 2023-07-18 18:17:45.860867 openplugin-0.0.15/openplugin/api/imprompt.py
+-rw-r--r--   0        0        0     1027 2023-07-18 18:23:39.434879 openplugin-0.0.15/openplugin/api/langchain.py
+-rw-r--r--   0        0        0     1015 2023-07-18 18:17:45.853531 openplugin-0.0.15/openplugin/api/openai.py
+-rw-r--r--   0        0        0     1179 2023-07-18 21:10:07.516382 openplugin-0.0.15/openplugin/api/openplugin.py
+-rw-r--r--   0        0        0     9095 2023-07-19 20:49:24.249838 openplugin-0.0.15/openplugin/bindings/imprompt/imprompt_plugin_selector.py
+-rw-r--r--   0        0        0     8711 2023-07-19 20:49:24.252426 openplugin-0.0.15/openplugin/bindings/langchain/langchain_plugin_selector.py
+-rw-r--r--   0        0        0     3944 2023-07-19 20:51:31.168500 openplugin-0.0.15/openplugin/bindings/openai/openai_plugin_selector.py
+-rw-r--r--   0        0        0    17837 2023-07-19 20:53:46.967081 openplugin-0.0.15/openplugin/interfaces/plugin_selector.py
+-rw-r--r--   0        0        0      906 2023-07-10 17:27:33.053788 openplugin-0.0.15/openplugin/main.py
+-rw-r--r--   0        0        0     2917 2023-07-19 20:49:24.246254 openplugin-0.0.15/openplugin/utils/manifest_handler.py
+-rw-r--r--   0        0        0     1230 2023-06-06 13:54:56.181740 openplugin-0.0.15/openplugin/utils/run_plugin_selector.py
+-rw-r--r--   0        0        0      728 2023-07-24 14:58:54.227775 openplugin-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 openplugin-0.0.15/PKG-INFO
```

### Comparing `openplugin-0.0.14/openplugin/__init__.py` & `openplugin-0.0.15/openplugin/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from openplugin.interfaces.plugin_selector import MessageType, PluginSelector, PluginOperation, Response, Message, LLM, \
-    Plugin, ToolSelectorConfig, Config, LLMProvider, ToolSelectorProvider
+    Plugin, ToolSelectorConfig, Config, LLMProvider, ToolSelectorProvider, Function, Functions, PluginDetected
 from openplugin.bindings.imprompt.imprompt_plugin_selector import ImpromptPluginSelector
 from openplugin.bindings.langchain.langchain_plugin_selector import LangchainPluginSelector
 from openplugin.utils.run_plugin_selector import run_plugin_selector
+from openplugin.bindings.openai.openai_plugin_selector import OpenAIPluginSelector
 
 __all__ = (
     "PluginSelector",
     "MessageType",
     "PluginOperation",
     "Response",
     "Message",
@@ -14,9 +15,12 @@
     "Plugin",
     "ToolSelectorConfig",
     "Config",
     "LLMProvider",
     "ToolSelectorProvider",
     "LangchainPluginSelector",
     "ImpromptPluginSelector",
-    "run_plugin_selector"
+    "run_plugin_selector",
+    "OpenAIPluginSelector",
+    "Function",
+    "Functions"
 )
```

### Comparing `openplugin-0.0.14/openplugin/api/auth.py` & `openplugin-0.0.15/openplugin/api/auth.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.14/openplugin/api/imprompt.py` & `openplugin-0.0.15/openplugin/api/imprompt.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     prefix="/imprompt",
     tags=["imprompt"],
     dependencies=[],
     responses={404: {"description": "Not found"}},
 )
 
 
-@router.post("/run-plugin")
+@router.post("/plugin-selector")
 def run_plugin(
         messages: List[Message],
         tool_selector_config: ToolSelectorConfig,
         plugins: List[Plugin],
         config: Optional[Config],
         llm: LLM,
         api_key: APIKey = Depends(auth.get_api_key)
```

### Comparing `openplugin-0.0.14/openplugin/api/langchain.py` & `openplugin-0.0.15/openplugin/api/langchain.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,24 +10,24 @@
     prefix="/langchain",
     tags=["langchain"],
     dependencies=[],
     responses={404: {"description": "Not found"}},
 )
 
 
-@router.post("/run-plugin")
+@router.post("/plugin-selector")
 def run_plugin(
         messages: List[Message],
         tool_selector_config: ToolSelectorConfig,
         plugins: List[Plugin],
         config: Config,
         llm: LLM,
         api_key: APIKey = Depends(auth.get_api_key)
 ):
-    print(api_key)
     selector = LangchainPluginSelector(tool_selector_config, plugins, config, llm)
     try:
         response = selector.run(messages)
         return response
     except Exception as e:
         print(e)
-        return JSONResponse(status_code=500, content={"message": "Failed to run plugin"})
+        return JSONResponse(status_code=500,
+                            content={"message": "Failed to run plugin"})
```

### Comparing `openplugin-0.0.14/openplugin/bindings/imprompt/imprompt_plugin_selector.py` & `openplugin-0.0.15/openplugin/bindings/imprompt/imprompt_plugin_selector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from typing import List, Optional, Set
 import openai, json, re, time, os
 from urllib.parse import urlparse, parse_qs
-from openplugin import MessageType, PluginSelector, PluginOperation, Response, Message, LLM, Plugin, \
+from openplugin import MessageType, PluginSelector, PluginDetected, Response, Message, \
+    LLM, Plugin, \
     ToolSelectorConfig, Config, LLMProvider
 
 plugin_prompt = """
 {name_for_model}: Call this tool to get the OpenAPI spec (and usage guide) for interacting with the {name_for_model} API. 
-You should only call this ONCE! What is the {name_for_model} API useful for? {description_for_model}.
+You should only call this ONCE! 
+
+What is the {name_for_model} API useful for? {description_for_model}.
 """
 
 plugin_identify_prompt = """
 Answer the following questions as best you can. You have access to the following tools:
 {all_plugin_info_prompt}
 Use the following format. Only reply with the action you want to take.:
 Question: the input question you must answer
 Thought: you should always think about what to do
-Action: the action to take, should be one of {all_plugin_names}
+Action: the action to take, should be one of {all_plugin_names}, None if you don't want to use any tool
 Begin!
 Question: {prompt}
 """
 
 plugin_operation_prompt = """
 // You are an AI assistant.
 // Here is a tool you can use, named {name_for_model}. The description for this plugin is: {description_for_model}.
@@ -29,103 +32,128 @@
 // 3. Create an HTTPS API url that represents this query.
 // 4. Use this format: <HTTP VERB> <URL>
 //   - An example: GET https://api.example.com/v1/products
 // 5. Remove any starting periods and new lines.
 // 6. Do not structure as a sentence.
 // 7. Never use https://api.example.com/ in the API.
 
+{pre_prompt}
+
 The openapi spec file = {openapi_spec}
 The instructions are: {prompt}
 """
 
 
 def _extract_urls(text):
-    url_pattern = re.compile(r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+')
+    url_pattern = re.compile(
+        r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+')
     urls = re.findall(url_pattern, text)
     return urls
 
 
 class ImpromptPluginSelector(PluginSelector):
+    def __init__(
+            self,
+            tool_selector_config: ToolSelectorConfig,
+            plugins: List[Plugin],
+            config: Optional[Config],
+            llm: Optional[LLM]):
+        super().__init__(tool_selector_config, plugins, config, llm)
+        self.llm = llm
+        self.total_tokens_used = 0
 
     def initialize_tool_selector(
             self,
             tool_selector_config: ToolSelectorConfig,
             plugins: List[Plugin],
             config: Optional[Config],
             llm: LLM
     ):
-        openai.api_key = os.environ["OPENAI_API_KEY"] if config.openai_api_key is None else config.openai_api_key
-        self.llm = llm
-        self.total_tokens_used = 0
+        openai.api_key = os.environ[
+            "OPENAI_API_KEY"] if config.openai_api_key is None else config.openai_api_key
         pass
 
     def run(self, messages: List[Message]) -> Response:
         start_test_case_time = time.time()
         plugin_operations = self.get_detected_plugin_with_operations(messages)
         response = Response(
             run_completed=True,
             final_text_response=None,
             detected_plugin_operations=plugin_operations,
             response_time=round(time.time() - start_test_case_time, 2),
-            tokens_used=0,
+            tokens_used=self.total_tokens_used,
             llm_api_cost=0
         )
         return response
 
-    def get_detected_plugin_with_operations(self, messages: List[Message]) -> List[PluginOperation]:
+    def get_detected_plugin_with_operations(self, messages: List[Message]) -> List[
+        PluginDetected]:
         prompt = ""
         for message in messages:
             prompt += f"{message.message_type}: {message.content}\n"
 
         plugin_info_prompts = []
         plugin_names = []
 
         for plugin in self.plugins:
-            plugin_names.append(plugin.name_for_model)
+            plugin_names.append(plugin.name)
             plugin_info_prompt = plugin_prompt.format(
-                name_for_model=plugin.name_for_model,
-                description_for_model=plugin.description_for_model
+                name_for_model=plugin.name,
+                description_for_model=plugin.description
             )
             plugin_info_prompts.append(plugin_info_prompt)
         plugin_detection_prompt = plugin_identify_prompt.format(
             all_plugin_info_prompt="".join(plugin_info_prompts),
-            all_plugin_names="".join(plugin_names),
+            all_plugin_names=", ".join(plugin_names),
             prompt=prompt
         )
+
         response = self.run_llm_prompt(plugin_detection_prompt)
         found_plugins = []
         for line in response.get('response').splitlines():
             if line.strip().startswith("Action"):
                 for val in line.split("Action:"):
                     if len(val.strip()) > 0:
                         if "-" in val:
                             val = val.split("-")[0].strip()
-                        found_plugins.append(self.get_plugin_by_name(val.strip()))
+                        if ',' in val:
+                            for v in val.split(','):
+                                found_plugins.append(
+                                    self.get_plugin_by_name(v.strip()))
+                        else:
+                            found_plugins.append(self.get_plugin_by_name(val.strip()))
+
         detected_plugins = []
-        for plugin in self.plugins:
-            openapi_spec_json = plugin.api.get_openapi_doc()
+
+        for plugin in found_plugins:
+            if plugin is None:
+                continue
+            api_called = None
+            mapped_operation_parameters = None
+            # TODO Find a better way to find the API called
+            openapi_spec_json = plugin.get_openapi_doc_json()
             formatted_plugin_operation_prompt = plugin_operation_prompt.format(
-                name_for_model=plugin.name_for_model,
-                description_for_model=plugin.description_for_model,
+                name_for_model=plugin.name,
+                description_for_model=plugin.description,
+                pre_prompt=plugin.get_plugin_pre_prompts(),
                 openapi_spec=json.dumps(openapi_spec_json),
                 prompt=prompt
             )
             response = self.run_llm_prompt(formatted_plugin_operation_prompt)
             urls = _extract_urls(response.get('response'))
-            api_called = None
-            mapped_operation_parameters = None
             for url in urls:
                 formatted_url = url.split("?")[0].strip()
-                if formatted_url in plugin.api.api_endpoints:
+                if formatted_url in plugin.api_endpoints:
                     api_called = formatted_url
                     query_dict = parse_qs(urlparse(url).query)
-                    mapped_operation_parameters = {k: v[0] if type(v) == list and len(v) == 1 else v for k, v in
-                                                   query_dict.items()}
+                    mapped_operation_parameters = {
+                        k: v[0] if type(v) == list and len(v) == 1 else v for k, v in
+                        query_dict.items()}
                     break
-            detected_plugins.append(PluginOperation(
+            detected_plugins.append(PluginDetected(
                 plugin=plugin,
                 api_called=api_called,
                 mapped_operation_parameters=mapped_operation_parameters
             ))
         return detected_plugins
 
     def run_llm_prompt(self, prompt):
@@ -166,14 +194,15 @@
             messages=messages,
             temperature=self.llm.temperature,
             max_tokens=self.llm.max_tokens,
             top_p=self.llm.top_p,
             frequency_penalty=self.llm.frequency_penalty,
             presence_penalty=self.llm.presence_penalty
         )
+        self.add_to_tokens(response.get("usage").get("total_tokens"))
         return {
             "response": response.get("choices")[0].get("message").get("content"),
             "usage": response.get("usage")
         }
 
     def openai_completion(self, prompt):
         response = openai.Completion.create(
@@ -181,11 +210,16 @@
             prompt=prompt,
             temperature=self.llm.temperature,
             max_tokens=self.llm.max_tokens,
             top_p=self.llm.top_p,
             frequency_penalty=self.llm.frequency_penalty,
             presence_penalty=self.llm.presence_penalty
         )
+        self.add_to_tokens(response.get("usage").get("total_tokens"))
         return {
             "response": response.get("choices")[0].get("text"),
             "usage": response.get("usage")
         }
+
+    def add_to_tokens(self, tokens):
+        if tokens:
+            self.total_tokens_used += tokens
```

### Comparing `openplugin-0.0.14/openplugin/main.py` & `openplugin-0.0.15/openplugin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,8 +25,8 @@
             typer.echo(f"OPENAI_API_KEY is not set.")
             raise typer.Exit(code=1)
     else:
         load_dotenv()
         os.environ["OPENAI_API_KEY"] = openai_api_key
 
     from openplugin.api import app
-    uvicorn.run(app, host=os.environ.get('HOST', '0.0.0.0'), port=int(os.environ.get('PORT', 8006)))
+    uvicorn.run(app, host=os.environ.get('HOST', '0.0.0.0'), port=int(os.environ.get('PORT', 8012)))
```

### Comparing `openplugin-0.0.14/openplugin/utils/run_plugin_selector.py` & `openplugin-0.0.15/openplugin/utils/run_plugin_selector.py`

 * *Files identical despite different names*

