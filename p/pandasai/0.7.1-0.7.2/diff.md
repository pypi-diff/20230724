# Comparing `tmp/pandasai-0.7.1.tar.gz` & `tmp/pandasai-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.7.1.tar", max compression
+gzip compressed data, was "pandasai-0.7.2.tar", max compression
```

## Comparing `pandasai-0.7.1.tar` & `pandasai-0.7.2.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1055 2023-07-22 21:11:48.623788 pandasai-0.7.1/LICENSE
--rw-r--r--   0        0        0     7705 2023-07-22 21:11:48.623788 pandasai-0.7.1/README.md
--rw-r--r--   0        0        0    26182 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/__init__.py
--rw-r--r--   0        0        0      522 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/callbacks/base.py
--rw-r--r--   0        0        0     1438 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     6404 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3070 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     3507 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4289 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    12126 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      585 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     3130 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1578 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1261 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1380 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1256 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1900 2023-07-22 21:11:48.635788 pandasai-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-24 10:38:30.978324 pandasai-0.7.2/LICENSE
+-rw-r--r--   0        0        0     7705 2023-07-24 10:38:30.978324 pandasai-0.7.2/README.md
+-rw-r--r--   0        0        0    26143 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/callbacks/__init__.py
+-rw-r--r--   0        0        0      519 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/callbacks/base.py
+-rw-r--r--   0        0        0      583 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/callbacks/file.py
+-rw-r--r--   0        0        0     1438 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     6404 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3070 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     3507 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4289 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    12126 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      585 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     3130 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1578 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1261 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1380 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1256 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1900 2023-07-24 10:38:30.990325 pandasai-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.7.2/PKG-INFO
```

### Comparing `pandasai-0.7.1/LICENSE` & `pandasai-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/README.md` & `pandasai-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/__init__.py` & `pandasai-0.7.2/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 from .middlewares.charts import ChartsMiddleware
 from .prompts.base import Prompt
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
-from .callbacks.base import BaseCallback, DefaultCallback
+from .callbacks.base import BaseCallback
 
 
 def get_version():
     """
     Get the version from the package metadata
     """
     from importlib.metadata import version
@@ -172,15 +172,15 @@
         save_charts=False,
         save_charts_path=None,
         enable_cache=True,
         middlewares=None,
         custom_whitelisted_dependencies=None,
         enable_logging=True,
         non_default_prompts: Optional[Dict[str, Type[Prompt]]] = None,
-        callback: BaseCallback = DefaultCallback,
+        callback: Optional[BaseCallback] = None,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
@@ -349,46 +349,47 @@
                     multiple_dataframes_instruction = self._non_default_prompts.get(
                         "multiple_dataframes", MultipleDataframesPrompt
                     )
                     code = self._llm.generate_code(
                         multiple_dataframes_instruction(dataframes=heads),
                         prompt,
                     )
-                    self.callback.on_code(code)
+
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": heads,
                     }
 
                 else:
                     df_head = data_frame.head(rows_to_display)
                     if anonymize_df:
                         df_head = anonymize_dataframe_head(df_head)
                     df_head = df_head.to_csv(index=False)
 
                     generate_code_instruction = self._non_default_prompts.get(
                         "generate_python_code", GeneratePythonCodePrompt
                     )(
-                        prompt=prompt,
                         df_head=df_head,
                         num_rows=data_frame.shape[0],
                         num_columns=data_frame.shape[1],
                     )
                     code = self._llm.generate_code(
                         generate_code_instruction,
                         prompt,
                     )
-                    self.callback.on_code(code)
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": df_head,
                         "num_rows": data_frame.shape[0],
                         "num_columns": data_frame.shape[1],
                     }
 
+                if self.callback:
+                    self.callback.on_code(code)
+
                 self.last_code_generated = code
                 self.log(
                     f"""
                         Code generated:
                         ```
                         {code}
                         ```
@@ -613,15 +614,16 @@
                 error_returned=e,
                 question=self._original_instructions["question"],
                 df_head=self._original_instructions["df_head"],
                 num_rows=self._original_instructions["num_rows"],
                 num_columns=self._original_instructions["num_columns"],
             )
         code = self._llm.generate_code(error_correcting_instruction, "")
-        self.callback.on_code(code)
+        if self.callback:
+            self.callback.on_code(code)
         return code
 
     def run_code(
         self,
         code: str,
         data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
```

### Comparing `pandasai-0.7.1/pandasai/constants.py` & `pandasai-0.7.2/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/exceptions.py` & `pandasai-0.7.2/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/helpers/_optional.py` & `pandasai-0.7.2/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/helpers/anonymizer.py` & `pandasai-0.7.2/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/helpers/cache.py` & `pandasai-0.7.2/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/helpers/from_excel.py` & `pandasai-0.7.2/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/helpers/notebook.py` & `pandasai-0.7.2/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/helpers/openai_info.py` & `pandasai-0.7.2/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/helpers/save_chart.py` & `pandasai-0.7.2/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/helpers/shortcuts.py` & `pandasai-0.7.2/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/llm/azure_openai.py` & `pandasai-0.7.2/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/llm/base.py` & `pandasai-0.7.2/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/llm/fake.py` & `pandasai-0.7.2/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/llm/falcon.py` & `pandasai-0.7.2/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/llm/google_palm.py` & `pandasai-0.7.2/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/llm/langchain.py` & `pandasai-0.7.2/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/llm/openai.py` & `pandasai-0.7.2/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/llm/starcoder.py` & `pandasai-0.7.2/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/middlewares/base.py` & `pandasai-0.7.2/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/middlewares/charts.py` & `pandasai-0.7.2/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/middlewares/streamlit.py` & `pandasai-0.7.2/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/prompts/base.py` & `pandasai-0.7.2/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.7.2/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.7.2/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/prompts/generate_python_code.py` & `pandasai-0.7.2/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.7.2/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.1/pyproject.toml` & `pandasai-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.7.1"
+version = "0.7.2"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.7.1/PKG-INFO` & `pandasai-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.7.1
+Version: 0.7.2
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

